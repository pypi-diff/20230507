# Comparing `tmp/nyckel-0.0.8.tar.gz` & `tmp/nyckel-0.0.9.tar.gz`

## Comparing `nyckel-0.0.8.tar` & `nyckel-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nyckel-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nyckel-0.0.8/.github/workflows/build.yml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nyckel-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/auth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/config.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/request_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/text_classification_function.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 nyckel-0.0.8/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.8/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.8/LICENSE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nyckel-0.0.8/README.md
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nyckel-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nyckel-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nyckel-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nyckel-0.0.9/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nyckel-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/auth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/config.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/functions/text_classification_function.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.9/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 nyckel-0.0.9/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.9/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nyckel-0.0.9/README.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nyckel-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nyckel-0.0.9/PKG-INFO
```

### Comparing `nyckel-0.0.8/.github/workflows/build.yml` & `nyckel-0.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/.github/workflows/test.yml` & `nyckel-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/src/nyckel/auth.py` & `nyckel-0.0.9/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/src/nyckel/request_utils.py` & `nyckel-0.0.9/src/nyckel/request_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,12 +37,12 @@
 def repeated_get(session: requests.Session, endpoint: str):
     base_url, slug = endpoint.split(".com")
     base_url += ".com"
     resp = session.get(base_url + slug)
     resource_list = resp.json()
     while "next" in resp.links:
         slug = resp.links["next"]["url"]
-        response = session.get(base_url + slug)
-        assert resp.status_code == 200, f"GET from {base_url+slug} failed with {response.status_code}, {response.text}."
+        resp = session.get(base_url + slug)
+        assert resp.status_code == 200, f"GET from {base_url+slug} failed with {resp.status_code}, {resp.text}."
         resource_list.extend(resp.json())
 
     return resource_list
```

### Comparing `nyckel-0.0.8/src/nyckel/functions/text_classification_function.py` & `nyckel-0.0.9/src/nyckel/functions/text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/tests/test_text_classification_function.py` & `nyckel-0.0.9/tests/test_text_classification_function.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/.gitignore` & `nyckel-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/LICENSE` & `nyckel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.8/pyproject.toml` & `nyckel-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `nyckel-0.0.8/PKG-INFO` & `nyckel-0.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyckel
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

