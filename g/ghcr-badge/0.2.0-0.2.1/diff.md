# Comparing `tmp/ghcr_badge-0.2.0.tar.gz` & `tmp/ghcr_badge-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghcr_badge-0.2.0.tar", max compression
+gzip compressed data, was "ghcr_badge-0.2.1.tar", max compression
```

## Comparing `ghcr_badge-0.2.0.tar` & `ghcr_badge-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1049 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0     3673 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/README.md
--rw-r--r--   0        0        0      125 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/__init__.py
--rw-r--r--   0        0        0     1436 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/dicts.py
--rw-r--r--   0        0        0    12955 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/generate.py
--rw-r--r--   0        0        0     2859 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/main.py
--rw-r--r--   0        0        0        0 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/py.typed
--rw-r--r--   0        0        0     6826 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/server.py
--rw-r--r--   0        0        0      721 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/svg/mark-github.svg
--rw-r--r--   0        0        0      540 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/ghcr_badge/svg/package-16.svg
--rw-r--r--   0        0        0     1670 2023-03-21 18:27:05.986169 ghcr_badge-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4956 1970-01-01 00:00:00.000000 ghcr_badge-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/LICENSE.txt
+-rw-r--r--   0        0        0     3617 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/README.md
+-rw-r--r--   0        0        0      125 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/__init__.py
+-rw-r--r--   0        0        0     1282 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/dicts.py
+-rw-r--r--   0        0        0    13171 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/generate.py
+-rw-r--r--   0        0        0     2859 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/main.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:23:20.181370 ghcr_badge-0.2.1/ghcr_badge/py.typed
+-rw-r--r--   0        0        0     6763 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/server.py
+-rw-r--r--   0        0        0      721 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/svg/mark-github.svg
+-rw-r--r--   0        0        0      540 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/ghcr_badge/svg/package-16.svg
+-rw-r--r--   0        0        0     1670 2023-05-07 12:23:20.185370 ghcr_badge-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     4900 1970-01-01 00:00:00.000000 ghcr_badge-0.2.1/PKG-INFO
```

### Comparing `ghcr_badge-0.2.0/LICENSE.txt` & `ghcr_badge-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.0/README.md` & `ghcr_badge-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,27 +36,27 @@
   - [![Website](https://img.shields.io/website?label=egpl.dev&url=https%3A%2F%2Fghcr-badge.egpl.dev)](https://ghcr-badge.egpl.dev)
 
 - <https://ghcr-badge.deta.dev/>
   - [![Website](https://img.shields.io/website?label=deta.dev&url=https%3A%2F%2Fghcr-badge.deta.dev)](https://ghcr-badge.deta.dev)
 
 ## Available paths
 
-- `/<string:package_owner>/<string:package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `ignore=latest`, `n=3`, `label=image tags`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
   - 👉: ![1]
-- `/<string:package_owner>/<string:package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `ignore=latest`, `label=version`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
   - 👉: ![2]
-- `/<string:package_owner>/<string:package_name>/develop_tag?color=...&label=...`
+- `/<package_owner>/<package_name>/develop_tag?color=...&label=...`
   - defaults: `color=#e05d44`, `label=develop`
   - <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
   - 👉: ![3]
-- `/<string:package_owner>/<string:package_name>/size?color=...&tag=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/size?color=...&tag=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `tag=latest`, `label=image size`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
   - 👉: ![4]
 
 ## Common parameters
 
 ### `label` parameter
```

### Comparing `ghcr_badge-0.2.0/ghcr_badge/dicts.py` & `ghcr_badge-0.2.1/ghcr_badge/dicts.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,57 +7,57 @@
 
 from __future__ import annotations
 
 from typing import TypedDict
 
 
 class _ManifestV2Layer(TypedDict):
-    mediaType: str  # noqa: N815
+    mediaType: str
     digest: str
     size: int
 
 
 class ManifestV2(TypedDict):
     """Image Manifest V2."""
 
-    mediaType: str  # noqa: N815
-    schemaVersion: int  # noqa: N815
+    mediaType: str
+    schemaVersion: int
     config: _ManifestV2Layer
     layers: list[_ManifestV2Layer]
 
 
 class ManifestListV2(TypedDict):
     """Manifest List V2."""
 
-    mediaType: str  # noqa: N815
-    schemaVersion: int  # noqa: N815
+    mediaType: str
+    schemaVersion: int
     manifests: list[_ManifestV2Layer]
 
 
 class _OCIImageManifestV1Config(TypedDict):
-    mediaType: str  # noqa: N815
+    mediaType: str
     size: int
     digest: str
 
 
 class _OCIImageManifestV1Layer(TypedDict):
-    mediaType: str  # noqa: N815
+    mediaType: str
     size: int
     digest: str
 
 
 class OCIImageManifestV1(TypedDict):
     """Manifest V1 for OCI Image."""
 
-    schemaVersion: int  # noqa: N815
-    mediaType: str  # noqa: N815
+    schemaVersion: int
+    mediaType: str
     config: _OCIImageManifestV1Config
     layers: list[_OCIImageManifestV1Layer]
     annotations: dict[str, str]
 
 
 class OCIImageIndexV1(TypedDict):
     """Index V1 for OCI Image."""
 
-    schemaVersion: int  # noqa: N815
-    mediaType: str  # noqa: N815
+    schemaVersion: int
+    mediaType: str
     manifests: list[OCIImageManifestV1]
```

### Comparing `ghcr_badge-0.2.0/ghcr_badge/generate.py` & `ghcr_badge-0.2.1/ghcr_badge/generate.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from .dicts import ManifestListV2, ManifestV2, OCIImageIndexV1, OCIImageManifestV1
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 _TIMEOUT = 10
 
+# force to cast badge value into str
+Badge.value_type = str
+
 
 class InvalidTokenError(Exception):
     """Exception for invalid token."""
 
 
 class InvalidTagError(Exception):
     """Exception for invalid tag."""
@@ -123,17 +126,18 @@
         if n < 0:
             msg = f"{n} should be positive."
             raise ValueError(msg)
         try:
             tags = self.filter_tags(package_owner, package_name)[::-1][:n][::-1]
         except InvalidTagListError:
             return self.get_invalid_badge(label)
+        badge_value = " " + " | ".join(tags)
         badge = Badge(
             label=label,
-            value=" | ".join(tags),
+            value=badge_value,
             default_color=self.color,
         )
         return str(badge.badge_svg_text)
 
     def generate_latest_tag(
         self: Self,
         package_owner: str,
@@ -159,17 +163,18 @@
         str
             svg string of generated badge of latest tag
         """
         try:
             latest_tag = self.filter_tags(package_owner, package_name)[-1]
         except InvalidTagListError:
             return self.get_invalid_badge(label)
+        badge_value = str(latest_tag)
         badge = Badge(
             label=label,
-            value=str(latest_tag),
+            value=badge_value,
             default_color=self.color,
         )
         return str(badge.badge_svg_text)
 
     def generate_develop_tag(
         self: Self,
         package_owner: str,
@@ -198,15 +203,20 @@
         try:
             tags = [tag for tag in self.get_tags(package_owner, package_name) if tag != "latest"]
             if "develop" not in tags or tags.index("develop") + 1 == len(tags):
                 return self.get_invalid_badge(label)
             develop_tag = tags[tags.index("develop") + 1]
         except InvalidTagListError:
             return self.get_invalid_badge(label)
-        badge = Badge(label=label, value=str(develop_tag), default_color=self.color)
+        badge_value = str(develop_tag)
+        badge = Badge(
+            label=label,
+            value=badge_value,
+            default_color=self.color,
+        )
         return str(badge.badge_svg_text)
 
     def generate_size(
         self: Self,
         package_owner: str,
         package_name: str,
         tag: str = "latest",
```

### Comparing `ghcr_badge-0.2.0/ghcr_badge/main.py` & `ghcr_badge-0.2.1/ghcr_badge/main.py`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.0/ghcr_badge/server.py` & `ghcr_badge-0.2.1/ghcr_badge/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from . import __version__
 from .generate import GHCRBadgeGenerator
 
 if TYPE_CHECKING:
     from flask.wrappers import Response
 
-_PACKAGE_PARAM_RULE = "/<string:package_owner>/<path:package_name>"
+_PACKAGE_PARAM_RULE = "/<package_owner>/<path:package_name>"
 
 app = Flask(__name__)
 app.config["JSONIFY_PRETTYPRINT_REGULAR"] = True
 
 
 def return_svg(svg: str) -> Response:
     """Return a generated svg as `Flask.Response`.
@@ -56,18 +56,18 @@
         JSON
     """
     try:
         return jsonify(
             {
                 "available_paths": [
                     "/",
-                    "/<string:package_owner>/<string:package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...",
-                    "/<string:package_owner>/<string:package_name>/latest_tag?color=...&ignore=...&label=...&trim=...",
-                    "/<string:package_owner>/<string:package_name>/develop_tag?color=...&label=...",
-                    "/<string:package_owner>/<string:package_name>/size?tag=...&color=...&label=...&trim=...",
+                    "/<package_owner>/<package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...",
+                    "/<package_owner>/<package_name>/latest_tag?color=...&ignore=...&label=...&trim=...",
+                    "/<package_owner>/<package_name>/develop_tag?color=...&label=...",
+                    "/<package_owner>/<package_name>/size?tag=...&color=...&label=...&trim=...",
                 ],
                 "example_paths": [
                     "/",
                     "/eggplants/ghcr-badge/tags",
                     "/eggplants/ghcr-badge/latest_tag",
                     "/ptr727/plexcleaner/develop_tag",
                     "/eggplants/ghcr-badge/size",
```

### Comparing `ghcr_badge-0.2.0/ghcr_badge/svg/mark-github.svg` & `ghcr_badge-0.2.1/ghcr_badge/svg/mark-github.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.0/ghcr_badge/svg/package-16.svg` & `ghcr_badge-0.2.1/ghcr_badge/svg/package-16.svg`

 * *Files identical despite different names*

### Comparing `ghcr_badge-0.2.0/pyproject.toml` & `ghcr_badge-0.2.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -43,29 +43,29 @@
 description = "Generate ghcr.io container's status badge"
 keywords = ["github-container-registry", "badge", "ghcr"]
 name = "ghcr_badge"
 packages = [{include = "ghcr_badge"}]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/eggplants/ghcr-badge"
-version = "0.2.0"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 anybadge="^1.9.0"
 flask="^2.1.2"
 gunicorn="^20.1.0"
 humanfriendly="^10.0"
 requests="^2.28.0"
 types-humanfriendly="^10.0"
 types-requests="^2.28.0"
 typing-extensions = "^4.5.0"
 
 [tool.poetry.group.dev.dependencies]
-mypy = ">=0.991,<1.2"
+mypy = ">=0.991,<1.3"
 pre-commit = ">=2.20,<4.0"
 taskipy = "^1.10.3"
 
 [tool.poetry.scripts]
 ghcr-badge-server = "ghcr_badge.server:main"
 ghcr-badge = "ghcr_badge.main:main"
```

### Comparing `ghcr_badge-0.2.0/PKG-INFO` & `ghcr_badge-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghcr-badge
-Version: 0.2.0
+Version: 0.2.1
 Summary: Generate ghcr.io container's status badge
 Home-page: https://github.com/eggplants/ghcr-badge
 License: MIT
 Keywords: github-container-registry,badge,ghcr
 Author: eggplants
 Author-email: w10776e8w@yahoo.co.jp
 Requires-Python: >=3.8,<3.12
@@ -67,27 +67,27 @@
   - [![Website](https://img.shields.io/website?label=egpl.dev&url=https%3A%2F%2Fghcr-badge.egpl.dev)](https://ghcr-badge.egpl.dev)
 
 - <https://ghcr-badge.deta.dev/>
   - [![Website](https://img.shields.io/website?label=deta.dev&url=https%3A%2F%2Fghcr-badge.deta.dev)](https://ghcr-badge.deta.dev)
 
 ## Available paths
 
-- `/<string:package_owner>/<string:package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/tags?color=...&ignore=...&n=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `ignore=latest`, `n=3`, `label=image tags`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/tags?trim=major>
   - 👉: ![1]
-- `/<string:package_owner>/<string:package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/latest_tag?color=...&ignore=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `ignore=latest`, `label=version`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/latest_tag?trim=major&label=latest>
   - 👉: ![2]
-- `/<string:package_owner>/<string:package_name>/develop_tag?color=...&label=...`
+- `/<package_owner>/<package_name>/develop_tag?color=...&label=...`
   - defaults: `color=#e05d44`, `label=develop`
   - <https://ghcr-badge.egpl.dev/ptr727/plexcleaner/develop_tag>
   - 👉: ![3]
-- `/<string:package_owner>/<string:package_name>/size?color=...&tag=...&label=...&trim=...`
+- `/<package_owner>/<package_name>/size?color=...&tag=...&label=...&trim=...`
   - defaults: `color=#e05d44`, `tag=latest`, `label=image size`
   - <https://ghcr-badge.egpl.dev/eggplants/ghcr-badge/size>
   - 👉: ![4]
 
 ## Common parameters
 
 ### `label` parameter
```

