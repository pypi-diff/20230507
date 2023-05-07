# Comparing `tmp/butterflymx-0.0.2.tar.gz` & `tmp/butterflymx-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "butterflymx-0.0.2.tar", max compression
+gzip compressed data, was "butterflymx-0.1.0.tar", max compression
```

## Comparing `butterflymx-0.0.2.tar` & `butterflymx-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1070 2023-05-01 12:35:35.508797 butterflymx-0.0.2/LICENSE
--rw-r--r--   0        0        0       63 2023-05-01 12:35:35.508862 butterflymx-0.0.2/README.md
--rw-r--r--   0        0        0       93 2023-05-06 01:46:26.714043 butterflymx-0.0.2/butterflymx/__init__.py
--rw-r--r--   0        0        0     5230 2023-05-06 15:03:11.286697 butterflymx-0.0.2/butterflymx/butterflymx.py
--rw-r--r--   0        0        0       49 2023-05-06 01:36:17.661480 butterflymx-0.0.2/butterflymx/graphql/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-06 02:15:53.991406 butterflymx-0.0.2/butterflymx/graphql/query_builder.py
--rw-r--r--   0        0        0      150 2023-05-06 01:45:36.640453 butterflymx-0.0.2/butterflymx/models/__init__.py
--rw-r--r--   0        0        0      424 2023-05-06 01:45:06.261959 butterflymx-0.0.2/butterflymx/models/butterflymx.py
--rw-r--r--   0        0        0      519 2023-05-06 01:45:10.029747 butterflymx-0.0.2/butterflymx/models/login.py
--rw-r--r--   0        0        0     7480 2023-05-06 00:26:15.660429 butterflymx-0.0.2/butterflymx/request_client.py
--rw-r--r--   0        0        0      203 2023-05-06 00:16:46.612362 butterflymx-0.0.2/butterflymx/utils.py
--rw-r--r--   0        0        0      675 2023-05-06 15:40:34.344758 butterflymx-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 butterflymx-0.0.2/setup.py
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 butterflymx-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-01 12:35:35.508797 butterflymx-0.1.0/LICENSE
+-rw-r--r--   0        0        0       63 2023-05-01 12:35:35.508862 butterflymx-0.1.0/README.md
+-rw-r--r--   0        0        0       93 2023-05-06 01:46:26.714043 butterflymx-0.1.0/butterflymx/__init__.py
+-rw-r--r--   0        0        0     5230 2023-05-06 15:03:11.286697 butterflymx-0.1.0/butterflymx/butterflymx.py
+-rw-r--r--   0        0        0       49 2023-05-06 01:36:17.661480 butterflymx-0.1.0/butterflymx/graphql/__init__.py
+-rw-r--r--   0        0        0     3013 2023-05-06 02:15:53.991406 butterflymx-0.1.0/butterflymx/graphql/query_builder.py
+-rw-r--r--   0        0        0      150 2023-05-06 01:45:36.640453 butterflymx-0.1.0/butterflymx/models/__init__.py
+-rw-r--r--   0        0        0      424 2023-05-06 01:45:06.261959 butterflymx-0.1.0/butterflymx/models/butterflymx.py
+-rw-r--r--   0        0        0      519 2023-05-06 01:45:10.029747 butterflymx-0.1.0/butterflymx/models/login.py
+-rw-r--r--   0        0        0        0 2023-05-07 16:02:09.666488 butterflymx-0.1.0/butterflymx/py.typed
+-rw-r--r--   0        0        0     6854 2023-05-07 16:05:53.102547 butterflymx-0.1.0/butterflymx/request_client.py
+-rw-r--r--   0        0        0      203 2023-05-06 00:16:46.612362 butterflymx-0.1.0/butterflymx/utils.py
+-rw-r--r--   0        0        0      675 2023-05-07 16:06:49.893362 butterflymx-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 butterflymx-0.1.0/setup.py
+-rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 butterflymx-0.1.0/PKG-INFO
```

### Comparing `butterflymx-0.0.2/LICENSE` & `butterflymx-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `butterflymx-0.0.2/butterflymx/butterflymx.py` & `butterflymx-0.1.0/butterflymx/butterflymx.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.0.2/butterflymx/graphql/query_builder.py` & `butterflymx-0.1.0/butterflymx/graphql/query_builder.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.0.2/butterflymx/models/login.py` & `butterflymx-0.1.0/butterflymx/models/login.py`

 * *Files identical despite different names*

### Comparing `butterflymx-0.0.2/butterflymx/request_client.py` & `butterflymx-0.1.0/butterflymx/request_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,36 +29,24 @@
             raise TypeError('Either refresh_token or email_and_password must be specified.')
 
         self.__http = http
         self.__oauth_credentials = oauth_credentials
         self.__email_and_password = email_and_password
         self.__refresh_token = refresh_token
 
-        self.__access_token: str | None = None
-        self.__access_token_expires_at: float | None = None
-
-        if access_token is not None:
-            self.__access_token = access_token.token
-            self.__access_token_expires_at = access_token.expires_at
+        self.__access_token = access_token
 
     @property
-    def access_token(self) -> str:
+    def access_token(self) -> AccessToken:
         if self.__access_token is None:
             raise RuntimeError('access_token has not yet been initialized.')
 
         return self.__access_token
 
     @property
-    def access_token_expires_at(self) -> float:
-        if self.__access_token_expires_at is None:
-            raise RuntimeError('access_token_expires_at has not yet been initialized.')
-
-        return self.__access_token_expires_at
-
-    @property
     def refresh_token(self) -> str:
         if self.__refresh_token is None:
             raise RuntimeError('refresh_token has not yet been initialized.')
 
         return self.__refresh_token
 
     async def __oauth_login(self) -> tuple[AccessToken, str]:
@@ -78,26 +66,24 @@
                 'response_type': 'code',
             },
             authenticate=False,
             allow_redirects=False,
         )
 
         # Fetch authenticity token from login page
-        # 3
         response = await self.request(
             'GET', 'https://accounts.butterflymx.com/login/new', authenticate=False
         )
 
         authenticity_token_input = bs4.BeautifulSoup(await response.text(), 'html.parser').find(
             'input', attrs={'name': 'authenticity_token'}
         )
         assert isinstance(authenticity_token_input, bs4.Tag)
 
         # Submit email and password
-        # 7
         response = await self.request(
             'POST',
             'https://accounts.butterflymx.com/login',
             data=FormData(
                 {
                     'utf8': '✓',  # Wtf is this
                     'authenticity_token': authenticity_token_input.attrs['value'],
@@ -112,15 +98,14 @@
                 'User-Agent': SPOOF_USER_AGENT,
             },
             authenticate=False,
             allow_redirects=False,
         )
 
         # Oauth flow
-        # 8
         response = await self.request(
             'GET',
             response.headers['Location'],
             headers={
                 'User-Agent': SPOOF_USER_AGENT,
                 'Referer': 'https://accounts.butterflymx.com/login/new',
             },
@@ -176,27 +161,25 @@
             ),
             token_data['refresh_token'],
         )
 
     async def ensure_access_token(self) -> None:
         if (
             self.__access_token is None
-            or self.__access_token_expires_at is None
-            or time.time() > self.__access_token_expires_at
+            or time.time() > self.access_token.expires_at
         ):
             access_token: AccessToken
             refresh_token: str
 
             if self.__refresh_token is None:
                 (access_token, refresh_token) = await self.__oauth_login()
             else:
                 (access_token, refresh_token) = await self.__oauth_refresh()
 
-            self.__access_token = access_token.token
-            self.__access_token_expires_at = access_token.expires_at
+            self.__access_token = access_token
             self.__refresh_token = refresh_token
 
     async def request(
         self,
         method: str,
         url: str,
         *,
@@ -208,12 +191,12 @@
         **kwargs,
     ) -> aiohttp.ClientResponse:
         if headers is None:
             headers = {}
 
         if authenticate:
             await self.ensure_access_token()
-            headers['Authorization'] = self.access_token
+            headers['Authorization'] = self.access_token.token
 
         return await self.__http.request(
             method, url, data=data, json=json, params=params, headers=headers, **kwargs
         )
```

### Comparing `butterflymx-0.0.2/pyproject.toml` & `butterflymx-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "butterflymx"
-version = "0.0.2"
+version = "0.1.0"
 description = "A reverse-engineered ButterflyMX app API wrapper"
 authors = ["Milo Weinberg <iapetus011@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiohttp = "^3.8.4"
```

### Comparing `butterflymx-0.0.2/setup.py` & `butterflymx-0.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['aiohttp>=3.8.4,<4.0.0',
  'beautifulsoup4>=4.12.2,<5.0.0',
  'ruff>=0.0.265,<0.0.266']
 
 setup_kwargs = {
     'name': 'butterflymx',
-    'version': '0.0.2',
+    'version': '0.1.0',
     'description': 'A reverse-engineered ButterflyMX app API wrapper',
     'long_description': '# ButterflyMX\nA reverse-engineered ButterflyMX app API wrapper\n',
     'author': 'Milo Weinberg',
     'author_email': 'iapetus011@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `butterflymx-0.0.2/PKG-INFO` & `butterflymx-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: butterflymx
-Version: 0.0.2
+Version: 0.1.0
 Summary: A reverse-engineered ButterflyMX app API wrapper
 Author: Milo Weinberg
 Author-email: iapetus011@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

