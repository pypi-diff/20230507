# Comparing `tmp/dynamic_qrcode_image-0.0.6.tar.gz` & `tmp/dynamic_qrcode_image-0.0.7.tar.gz`

## Comparing `dynamic_qrcode_image-0.0.6.tar` & `dynamic_qrcode_image-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/__init__.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/__main__.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/config.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/form.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qr2.py
--rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qrc.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/w2.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/docs/generate.html
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/docs/index.md
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/templates/submit.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/tests/__init__.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/LICENSE
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/CONTRIBUTING.md
+-rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/SECURITY.md
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/.github/ISSUE_TEMPLATE/custom.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/__init__.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/__main__.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/config.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/form.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/qr2.py
+-rw-r--r--   0        0        0     3254 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/qrc.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/w2.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/docs/generate.html
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/docs/index.md
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/templates/submit.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/tests/__init__.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/LICENSE
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/README.md
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 dynamic_qrcode_image-0.0.7/PKG-INFO
```

### Comparing `dynamic_qrcode_image-0.0.6/.github/workflows/python-publish.yml` & `dynamic_qrcode_image-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qr2.py` & `dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/qr2.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/qrc.py` & `dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/qrc.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/src/dynamic_qrcode_image/w2.py` & `dynamic_qrcode_image-0.0.7/src/dynamic_qrcode_image/w2.py`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/.gitignore` & `dynamic_qrcode_image-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/LICENSE` & `dynamic_qrcode_image-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dynamic_qrcode_image-0.0.6/pyproject.toml` & `dynamic_qrcode_image-0.0.7/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dynamic_qrcode_image"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
-    { name="Duke Bode", email="DukeBode@hotmail.com"},
+    { name="Duke Bode"},
 ]
 description = "dynamic_qrcode_image"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: 3.11"
@@ -20,7 +20,10 @@
     "pillow",
     "qrcode",
     "pyzbar"
 ]
 [project.urls]
 "Homepage" = "https://github.com/DukeBode/dynamic-qrcode-image"
 "Bug Tracker" = "https://github.com/DukeBode/dynamic-qrcode-image/issues"
+
+[project.scripts]
+qrcode-server = "dynamic_qrcode_image.w2:app.run"
```

### Comparing `dynamic_qrcode_image-0.0.6/PKG-INFO` & `dynamic_qrcode_image-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: dynamic_qrcode_image
-Version: 0.0.6
+Version: 0.0.7
 Summary: dynamic_qrcode_image
 Project-URL: Homepage, https://github.com/DukeBode/dynamic-qrcode-image
 Project-URL: Bug Tracker, https://github.com/DukeBode/dynamic-qrcode-image/issues
-Author-email: Duke Bode <DukeBode@hotmail.com>
+Author: Duke Bode
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Requires-Dist: flask
 Requires-Dist: pillow
 Requires-Dist: pyzbar
```

