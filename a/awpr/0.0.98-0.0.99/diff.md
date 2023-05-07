# Comparing `tmp/awpr-0.0.98.tar.gz` & `tmp/awpr-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awpr-0.0.98.tar", max compression
+gzip compressed data, was "awpr-0.0.99.tar", max compression
```

## Comparing `awpr-0.0.98.tar` & `awpr-0.0.99.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1076 2022-12-27 18:38:20.046840 awpr-0.0.98/LICENSE
--rw-r--r--   0        0        0      533 2022-12-27 18:38:20.046840 awpr-0.0.98/README.md
--rw-r--r--   0        0        0        0 2022-12-27 18:38:20.046840 awpr-0.0.98/awpr/__init__.py
--rw-r--r--   0        0        0     2249 2022-12-27 18:38:20.046840 awpr-0.0.98/awpr/awpr.py
--rw-r--r--   0        0        0      918 2022-12-27 18:38:20.642854 awpr-0.0.98/pyproject.toml
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 awpr-0.0.98/setup.py
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 awpr-0.0.98/PKG-INFO
+-rw-r--r--   0        0        0     1076 2022-12-29 02:06:51.747604 awpr-0.0.99/LICENSE
+-rw-r--r--   0        0        0      533 2022-12-29 02:06:51.747604 awpr-0.0.99/README.md
+-rw-r--r--   0        0        0        0 2022-12-29 02:06:51.747604 awpr-0.0.99/awpr/__init__.py
+-rw-r--r--   0        0        0     2249 2022-12-29 02:06:51.747604 awpr-0.0.99/awpr/awpr.py
+-rw-r--r--   0        0        0      918 2022-12-29 02:06:52.315613 awpr-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 awpr-0.0.99/setup.py
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 awpr-0.0.99/PKG-INFO
```

### Comparing `awpr-0.0.98/LICENSE` & `awpr-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `awpr-0.0.98/README.md` & `awpr-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `awpr-0.0.98/awpr/awpr.py` & `awpr-0.0.99/awpr/awpr.py`

 * *Files identical despite different names*

### Comparing `awpr-0.0.98/pyproject.toml` & `awpr-0.0.99/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "awpr"
-version = "v0.0.98"
+version = "v0.0.99"
 description = "Library that helps an application report progress to Argo Workflows."
 authors = ["Michael Mohamed <michael@foundationstack.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fsai-dev/fsai-cli-tools"
 repository = "https://github.com/fsai-dev/fsai-cli-tools"
```

### Comparing `awpr-0.0.98/setup.py` & `awpr-0.0.99/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['beartype>=0.10.4,<0.11.0', 'loguru>=0.6.0,<0.7.0']
 
 setup_kwargs = {
     'name': 'awpr',
-    'version': '0.0.98',
+    'version': '0.0.99',
     'description': 'Library that helps an application report progress to Argo Workflows.',
     'long_description': '# awpr\nLibrary that helps an application report progress to Argo Workflows.\n\n\n## Installation \n```shell\npip install awpr\n```\n\n## Usage\nSet the environment variable and run your application:\n`ARGO_PROGRESS_FILE=/tmp/progress.txt`\n\n```shell\nfrom awpr.awpr import ArgoWorkflowsProgressReporter\n\nawpr = ArgoWorkflowsProgressReporter()\nawpr.set_total_progress(100)\nawpr.start_reporting()\n\nawpr.set_current_progress(20)\nawpr.set_current_progress(30)\nawpr.get_progress_percent()\n\nawpr.set_progress_complete()\nawpr.get_progress_percent()\n```',
     'author': 'Michael Mohamed',
     'author_email': 'michael@foundationstack.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/fsai-dev/fsai-cli-tools',
```

### Comparing `awpr-0.0.98/PKG-INFO` & `awpr-0.0.99/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awpr
-Version: 0.0.98
+Version: 0.0.99
 Summary: Library that helps an application report progress to Argo Workflows.
 Home-page: https://github.com/fsai-dev/fsai-cli-tools
 License: MIT
 Author: Michael Mohamed
 Author-email: michael@foundationstack.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

