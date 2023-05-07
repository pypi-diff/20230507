# Comparing `tmp/zimmauth-0.0.8.tar.gz` & `tmp/zimmauth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zimmauth-0.0.8.tar", last modified: Sun Apr  2 11:42:36 2023, max compression
+gzip compressed data, was "zimmauth-0.0.9.tar", last modified: Sun May  7 10:30:17 2023, max compression
```

## Comparing `zimmauth-0.0.8.tar` & `zimmauth-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      584 2023-04-02 11:42:30.695617 zimmauth-0.0.8/.github/workflows/test.yml
--rw-r--r--   0        0        0      566 2023-04-02 11:42:30.695617 zimmauth-0.0.8/.github/workflows/twine_release.yml
--rw-r--r--   0        0        0     1770 2023-04-02 11:42:30.695617 zimmauth-0.0.8/.gitignore
--rw-r--r--   0        0        0     1056 2023-04-02 11:42:30.695617 zimmauth-0.0.8/LICENSE
--rw-r--r--   0        0        0      423 2023-04-02 11:42:30.695617 zimmauth-0.0.8/README.md
--rw-r--r--   0        0        0      607 2023-04-02 11:42:30.695617 zimmauth-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      150 2023-04-02 11:42:30.695617 zimmauth-0.0.8/zimmauth/__init__.py
--rw-r--r--   0        0        0     6437 2023-04-02 11:42:30.695617 zimmauth-0.0.8/zimmauth/core.py
--rw-r--r--   0        0        0      882 2023-04-02 11:42:30.695617 zimmauth-0.0.8/zimmauth/local_conn.py
--rw-r--r--   0        0        0     6496 2023-04-02 11:42:30.695617 zimmauth-0.0.8/zimmauth/test_core.py
--rw-r--r--   0        0        0     1169 1970-01-01 00:00:00.000000 zimmauth-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      584 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0        0        0      566 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.github/workflows/twine_release.yml
+-rw-r--r--   0        0        0     1770 2023-05-07 10:30:11.134998 zimmauth-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1056 2023-05-07 10:30:11.134998 zimmauth-0.0.9/LICENSE
+-rw-r--r--   0        0        0      423 2023-05-07 10:30:11.134998 zimmauth-0.0.9/README.md
+-rw-r--r--   0        0        0      711 2023-05-07 10:30:11.134998 zimmauth-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/__init__.py
+-rw-r--r--   0        0        0     6437 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/core.py
+-rw-r--r--   0        0        0      882 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/local_conn.py
+-rw-r--r--   0        0        0     6496 2023-05-07 10:30:11.134998 zimmauth-0.0.9/zimmauth/test_core.py
+-rw-r--r--   0        0        0     1370 1970-01-01 00:00:00.000000 zimmauth-0.0.9/PKG-INFO
```

### Comparing `zimmauth-0.0.8/.github/workflows/test.yml` & `zimmauth-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/.github/workflows/twine_release.yml` & `zimmauth-0.0.9/.github/workflows/twine_release.yml`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/.gitignore` & `zimmauth-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/LICENSE` & `zimmauth-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/pyproject.toml` & `zimmauth-0.0.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 authors = [{name = "Endre Márk Borza", email = "endremborza@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = ["cryptography"]
 
 [project.optional-dependencies]
-test = ["branthebuilder", "mock-ssh-server", "dvc[s3,ssh]", "fabric", "boto3", "toml", "moto", "aiobotocore"]
+env = ["toml"]
+ssh = ["fabric", "decorator"]
+test = [
+    "branthebuilder", 
+    "mock-ssh-server", 
+    "dvc[s3,ssh]", 
+    "moto", 
+    "aiobotocore", 
+    "boto3", 
+    "fabric", 
+    "toml", 
+    "decorator"
+]
 doc = ["branthebuilder[doc]"]
 
 [project.urls]
 Homepage = "https://github.com/endremborza/zimmauth"
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
```

### Comparing `zimmauth-0.0.8/zimmauth/core.py` & `zimmauth-0.0.9/zimmauth/core.py`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/zimmauth/local_conn.py` & `zimmauth-0.0.9/zimmauth/local_conn.py`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/zimmauth/test_core.py` & `zimmauth-0.0.9/zimmauth/test_core.py`

 * *Files identical despite different names*

### Comparing `zimmauth-0.0.8/PKG-INFO` & `zimmauth-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 Metadata-Version: 2.1
 Name: zimmauth
-Version: 0.0.8
+Version: 0.0.9
 Summary: Authentication encryption and storage
 Author-email: Endre Márk Borza <endremborza@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: cryptography
 Requires-Dist: branthebuilder[doc] ; extra == "doc"
+Requires-Dist: toml ; extra == "env"
+Requires-Dist: fabric ; extra == "ssh"
+Requires-Dist: decorator ; extra == "ssh"
 Requires-Dist: branthebuilder ; extra == "test"
 Requires-Dist: mock-ssh-server ; extra == "test"
 Requires-Dist: dvc[s3,ssh] ; extra == "test"
-Requires-Dist: fabric ; extra == "test"
-Requires-Dist: boto3 ; extra == "test"
-Requires-Dist: toml ; extra == "test"
 Requires-Dist: moto ; extra == "test"
 Requires-Dist: aiobotocore ; extra == "test"
+Requires-Dist: boto3 ; extra == "test"
+Requires-Dist: fabric ; extra == "test"
+Requires-Dist: toml ; extra == "test"
+Requires-Dist: decorator ; extra == "test"
 Project-URL: Homepage, https://github.com/endremborza/zimmauth
 Provides-Extra: doc
+Provides-Extra: env
+Provides-Extra: ssh
 Provides-Extra: test
 
 # zimmauth
 
 [![codeclimate](https://img.shields.io/codeclimate/maintainability/endremborza/zimmauth.svg)](https://codeclimate.com/github/endremborza/zimmauth)
 [![codecov](https://img.shields.io/codecov/c/github/endremborza/zimmauth)](https://codecov.io/gh/endremborza/zimmauth)
 [![pypi](https://img.shields.io/pypi/v/zimmauth.svg)](https://pypi.org/project/zimmauth/)
```

