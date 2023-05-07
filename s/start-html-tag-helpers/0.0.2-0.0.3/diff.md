# Comparing `tmp/start_html_tag_helpers-0.0.2.tar.gz` & `tmp/start_html_tag_helpers-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "start_html_tag_helpers-0.0.2.tar", max compression
+gzip compressed data, was "start_html_tag_helpers-0.0.3.tar", max compression
```

## Comparing `start_html_tag_helpers-0.0.2.tar` & `start_html_tag_helpers-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1491 2023-04-24 21:29:14.558962 start_html_tag_helpers-0.0.2/LICENSE
--rw-r--r--   0        0        0      280 2023-04-24 21:49:12.647932 start_html_tag_helpers-0.0.2/README.md
--rw-r--r--   0        0        0     1480 2023-04-24 22:07:15.353002 start_html_tag_helpers-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      141 2023-04-24 22:06:07.720239 start_html_tag_helpers-0.0.2/start_html_tag_helpers/__init__.py
--rw-r--r--   0        0        0     2884 2023-04-24 22:03:35.442680 start_html_tag_helpers-0.0.2/start_html_tag_helpers/filter_attrs.py
--rw-r--r--   0        0        0     3098 2023-04-24 22:05:42.960424 start_html_tag_helpers-0.0.2/start_html_tag_helpers/wrap_svg.py
--rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 start_html_tag_helpers-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-04-24 21:29:14.558962 start_html_tag_helpers-0.0.3/LICENSE
+-rw-r--r--   0        0        0      280 2023-04-24 21:49:12.647932 start_html_tag_helpers-0.0.3/README.md
+-rw-r--r--   0        0        0     1417 2023-05-06 10:27:56.899059 start_html_tag_helpers-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      130 2023-05-06 10:27:01.867678 start_html_tag_helpers-0.0.3/start_html_tag_helpers/__init__.py
+-rw-r--r--   0        0        0     4130 2023-05-06 10:31:34.231766 start_html_tag_helpers-0.0.3/start_html_tag_helpers/filter_attrs.py
+-rw-r--r--   0        0        0     3478 2023-05-06 10:32:44.599561 start_html_tag_helpers-0.0.3/start_html_tag_helpers/wrap_svg.py
+-rw-r--r--   0        0        0     1140 1970-01-01 00:00:00.000000 start_html_tag_helpers-0.0.3/PKG-INFO
```

### Comparing `start_html_tag_helpers-0.0.2/LICENSE` & `start_html_tag_helpers-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `start_html_tag_helpers-0.0.2/pyproject.toml` & `start_html_tag_helpers-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "start-html-tag-helpers"
 description = "Some utility functions for dealing with html attributes and tags."
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/start-html-tag-helpers"
 documentation = "https://mv3.dev/start-html-tag-helpers"
 classifiers = [
@@ -17,36 +17,32 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.12.2"
 
 [tool.poetry.group.dev.dependencies]
 rich = "^13.3"
-black = "^23.3.0"
 pytest = "^7.2"
 pytest-datadir = "^1.4.1"
 pytest-cov = "^2.12.1"
 pre-commit = "^2.21"
 mkdocs = "^1.4.2"
 mkdocstrings = { extras = ["python"], version = "^0.20.0" }
 mkdocs-material = "^9.1"
 ipykernel = "^6.22.0"
 
-
 [tool.pytest.ini_options]
 minversion = "7.2"
 addopts = "-ra -q --doctest-modules --cov"
-testpaths = ["tests"]
+testpaths = ["tests", "start_html_tag_helpers"]
 
 [tool.ruff]
-ignore = ["F401"]
-
-[tool.curlylint.rules]
-image_alt = true
-
+ignore = ["F401", "F403"]
+fixable = ["F", "E", "W", "I001"]
+select = ["F", "E", "W", "I001"]
 [tool.black]
 target-version = ['py311']
 line-length = 79
 include = '.pyi?$'
 exclude = '''
 /(
     .git
@@ -57,16 +53,10 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 '''
 
-[tool.isort]
-profile = "black"
-multi_line_output = 3
-line_length = 79
-include_trailing_comma = 'True'
-
 [build-system]
 requires = ["poetry-core>=1.3.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `start_html_tag_helpers-0.0.2/start_html_tag_helpers/filter_attrs.py` & `start_html_tag_helpers-0.0.3/start_html_tag_helpers/filter_attrs.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,46 @@
         dict[str, str]: dict to be used for a html tag's aria-* attributes.
     """  # noqa: E501
     return {
         k.replace("_", "-"): v for k, v in d.items() if k.startswith("aria_")
     }
 
 
+def help_key(key: str, d: dict, remove_prefix: bool = False) -> dict[str, str]:
+    """Filter `k`, `v` from `d` based on keys prefixed with `key`. Based on this result, rename the key,
+    if `remove_prefix` is marked `True`. This enables a shortcut for gathering all attributes that should
+    be applied to the element's neighbouring tags, e.g. parent, post, pre.
+
+    Examples:
+        >>> parent_res = help_key(key="parent", d={"non-a-parent": "test", "parent_css":"flex items-center", "parent_title": "I should be centered"})
+        >>> "parent_css" in parent_res
+        True
+        >>> "parent_title" in parent_res
+        True
+        >>> "non-a-parent" in parent_res
+        False
+        >>> pre_res = help_key(key="pre", d={"pre_class":"sr-only", "post_class":"whatever"})
+        >>> "pre_class" in pre_res
+        True
+
+    Args:
+        d (dict): Values from a template tag.
+
+    Returns:
+        dict[str, str]: dict to be used for an html tag's parent element's attributes.
+    """  # noqa: E501
+    if remove_prefix:
+        return {
+            k.removeprefix(f"{key}_"): v
+            for k, v in d.items()
+            if k.startswith(f"{key}_")
+        }
+    return {k: v for k, v in d.items() if k.startswith(f"{key}_")}
+
+
 def help_hx(d: dict) -> dict[str, str]:
     """Filter `k`, `v` from `d` based on keys prefixed with `hx_`. Based on this result, rename the key.
     This enables a shortcut for gathering all hx-* attributes found in the dict `d` and parse them properly
     before inserting them into html tags.
 
     Examples:
         >>> res = help_hx(d={"hx_get":"https://test.html",  "hx_target":"body"})
```

### Comparing `start_html_tag_helpers-0.0.2/PKG-INFO` & `start_html_tag_helpers-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: start-html-tag-helpers
-Version: 0.0.2
+Version: 0.0.3
 Summary: Some utility functions for dealing with html attributes and tags.
 Home-page: https://mv3.dev
 License: MIT
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

