# Comparing `tmp/spacs-0.0.7.tar.gz` & `tmp/spacs-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacs-0.0.7.tar", max compression
+gzip compressed data, was "spacs-0.0.8.tar", max compression
```

## Comparing `spacs-0.0.7.tar` & `spacs-0.0.8.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.7/LICENSE
--rw-r--r--   0        0        0      418 2023-05-02 22:45:32.426000 spacs-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1763 2023-05-01 18:22:46.781118 spacs-0.0.7/README.md
--rw-r--r--   0        0        0      184 2023-05-01 15:11:43.780995 spacs-0.0.7/spacs/__init__.py
--rw-r--r--   0        0        0     8397 2023-05-02 22:42:09.370541 spacs-0.0.7/spacs/client.py
--rw-r--r--   0        0        0     2424 1970-01-01 00:00:00.000000 spacs-0.0.7/setup.py
--rw-r--r--   0        0        0     2172 1970-01-01 00:00:00.000000 spacs-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-04-26 20:46:06.053000 spacs-0.0.8/LICENSE
+-rw-r--r--   0        0        0      506 2023-05-07 14:12:28.762774 spacs-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     4046 2023-05-07 15:59:37.368789 spacs-0.0.8/README.md
+-rw-r--r--   0        0        0      217 2023-05-07 14:37:52.722081 spacs-0.0.8/spacs/__init__.py
+-rw-r--r--   0        0        0     8417 2023-05-07 14:37:34.446392 spacs-0.0.8/spacs/client.py
+-rw-r--r--   0        0        0       55 2023-05-04 13:54:47.377396 spacs-0.0.8/spacs/conf.py
+-rw-r--r--   0        0        0     4707 1970-01-01 00:00:00.000000 spacs-0.0.8/setup.py
+-rw-r--r--   0        0        0     4388 1970-01-01 00:00:00.000000 spacs-0.0.8/PKG-INFO
```

### Comparing `spacs-0.0.7/LICENSE` & `spacs-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spacs-0.0.7/spacs/client.py` & `spacs-0.0.8/spacs/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import datetime
 import json
-import logging
 from collections.abc import Callable
 from enum import StrEnum
 from typing import Any, Awaitable, ClassVar, Self, Type
 
 import aiohttp
 from aiohttp import ClientConnectorError, ClientResponse
 from pydantic import BaseModel
 
+from spacs.conf import logger
+
 ResponseModel = Type[BaseModel] | None
 ModelContent = BaseModel | list[BaseModel]
 JsonContent = dict[str, Any] | list[dict[str, Any]]
 RequestContent = JsonContent | ModelContent | None
-SpacsResponse = str | JsonContent | ModelContent
-
-_logger = logging.getLogger(__name__)
+SpacsResponse = str | JsonContent | ModelContent | None
 
 
 class ContentType(StrEnum):
     JSON = "application/json"
     FORM = "application/x-www-form-urlencoded"
     HTML = "text/html"
 
@@ -29,42 +28,51 @@
     params: RequestContent = None
     body: RequestContent = None
     headers: dict[str, str] = None
     content_type: ContentType = ContentType.JSON
     response_model: ResponseModel = None
 
 
+class SpacsRequestError(Exception):
+    status: int
+    reason: str
+
+    def __init__(self, status: int, reason: str):
+        self.status = status
+        self.reason = reason
+
+    def __repr__(self) -> str:
+        return f"SpacsRequestError(status={self.status}, reason={self.reason}"
+
+
 class SpacsClient:
     base_url: str | None
     path_prefix: str
+    error_handler: Callable[[SpacsRequestError], Awaitable[None]] | None
 
     _sessions: ClassVar[list[Self]] = []
-    _logger: logging.Logger
     _session: aiohttp.ClientSession | None = None
 
     def __init__(
         self,
         *,
         base_url: str | None = None,
         path_prefix: str = "",
-        logger: logging.Logger | None = None,
+        error_handler: Callable[[SpacsRequestError], Awaitable[None]] | None = None,
     ) -> None:
         """
 
         Keyword Args:
             base_url (str | None): Base url to be used for all requests
             path_prefix (str): Path partial to be prepended to paths for all requests
-            logger (logging.Logger | None): Override for logger
         """
         self._sessions.append(self)
         self.base_url = base_url
         self.path_prefix = path_prefix.strip("/")
-        self._logger = logger
-        if self._logger is None:
-            self._logger = logging.getLogger(__name__)
+        self.error_handler = error_handler
 
     def __del__(self) -> None:
         self._sessions.remove(self)
 
     @property
     def session(self) -> aiohttp.ClientSession:
         if not self.is_open:
@@ -74,15 +82,15 @@
     @property
     def is_open(self) -> bool:
         """Returns `True` if a session exists and is open."""
         return self._session and not self._session.closed
 
     async def close(self) -> None:
         if not self.is_open:
-            return _logger.warning("No session to close")
+            return logger.warning("No session to close")
         await self._session.close()
         self._session = None
 
     async def get(self, request: SpacsRequest) -> SpacsResponse:
         return await self._request(self.session.get, request)
 
     async def post(self, request: SpacsRequest) -> SpacsResponse:
@@ -106,49 +114,49 @@
         base_log_info = {
             "method": action.__name__,
             "base_url": self.base_url,
             "path": request.path,
         }
 
         try:
-            async with action(
+            response = await action(
                 request.path,
                 params=request.params,
                 data=request.body,
                 headers=request.headers,
-            ) as response:
-                end_time = datetime.datetime.now(tz=datetime.timezone.utc)
-                self._logger.debug(
-                    {
-                        "msg": "Request completed",
-                        **base_log_info,
-                        "status": response.status,
-                        "duration": str(end_time - start_time),
-                    }
+            )
+            end_time = datetime.datetime.now(tz=datetime.timezone.utc)
+            logger.debug(
+                {
+                    "msg": "Request completed",
+                    **base_log_info,
+                    "status": response.status,
+                    "duration": str(end_time - start_time),
+                }
+            )
+            if response.ok:
+                return await self._handle_ok_response(response, request.response_model)
+            else:
+                raise SpacsRequestError(
+                    status=response.status,
+                    reason=response.reason,
                 )
-                if response.ok:
-                    return await self._handle_ok_response(
-                        response, request.response_model
-                    )
-                else:
-                    raise SpacsRequestError(
-                        status_code=response.status,
-                        reason=response.reason,
-                    )
         except ClientConnectorError as error:
-            self._logger.error("Failed to connect to server.")
+            logger.error("Failed to connect to server.")
             raise error
         except Exception as error:
-            self._logger.error(
+            logger.error(
                 {
                     "msg": "Request error",
                     **base_log_info,
                     "error": repr(error),
                 }
             )
+            if self.error_handler is not None and isinstance(error, SpacsRequestError):
+                return await self.error_handler(error)
             raise error
 
     def _prepare_request(self, request: SpacsRequest) -> SpacsRequest:
         # Copy content to not modify inputs to `SpacsClient` actions
         result = request.copy(deep=True)
 
         if result.headers is None:
@@ -164,17 +172,18 @@
         # `content-type`, automatically stringify/encode the payload.
         if result.body is not None and result.content_type == ContentType.JSON:
             result.body = json.dumps(result.body).encode("utf-8")
 
         return result
 
     def _build_path(self, path: str) -> str:
-        result = f"/{path.strip('/')}"
+        prepend_slash = "/" if self.base_url else ""
+        result = f"{prepend_slash}{path.strip('/')}"
         if self.path_prefix:
-            result = f"/{self.path_prefix}{result}"
+            result = f"{prepend_slash}{self.path_prefix}{result}"
         return result
 
     @classmethod
     async def close_all(cls) -> None:
         for session in cls._sessions:
             if not session.is_open:
                 continue
@@ -226,16 +235,7 @@
     @staticmethod
     def _response_content_to_model(
         content: JsonContent, model: Type[BaseModel]
     ) -> ModelContent:
         if isinstance(content, list):
             return [model(**item) for item in content]
         return model(**content)
-
-
-class SpacsRequestError(Exception):
-    def __init__(self, status_code: int, reason: str):
-        self.status_code = status_code
-        self.reason = reason
-
-    def __repr__(self) -> str:
-        return f"SpacsRequestError(status_code={self.status_code}, reason={self.reason}"
```

