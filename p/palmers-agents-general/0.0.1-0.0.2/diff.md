# Comparing `tmp/palmers_agents_general-0.0.1.tar.gz` & `tmp/palmers_agents_general-0.0.2.tar.gz`

## Comparing `palmers_agents_general-0.0.1.tar` & `palmers_agents_general-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/base_mq_consumer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/utils/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/utils/blobs_handler.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/utils/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/README.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/base_mq_consumer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/utils/__init__.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/utils/blobs_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/utils/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/.gitignore
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/README.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.2/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.1/base_mq_consumer.py` & `palmers_agents_general-0.0.2/base_mq_consumer.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.1/utils/blobs_handler.py` & `palmers_agents_general-0.0.2/utils/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.1/pyproject.toml` & `palmers_agents_general-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_agents_general-0.0.1/PKG-INFO` & `palmers_agents_general-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 Metadata-Version: 2.1
 Name: palmers_agents_general
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Roy  <roy@sdatta.ai>, Assaf <assafm@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+python -m build
+twine upload dist/*
```

