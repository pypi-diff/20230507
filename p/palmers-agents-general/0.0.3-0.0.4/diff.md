# Comparing `tmp/palmers_agents_general-0.0.3.tar.gz` & `tmp/palmers_agents_general-0.0.4.tar.gz`

## Comparing `palmers_agents_general-0.0.3.tar` & `palmers_agents_general-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/src/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/src/base_mq_consumer.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/src/blobs_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/src/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/README.md
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/src/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/src/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/src/palmers_agents_general/base_mq_consumer.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/src/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/src/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/README.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.4/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.3/src/base_mq_consumer.py` & `palmers_agents_general-0.0.4/src/palmers_agents_general/base_mq_consumer.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.3/src/blobs_handler.py` & `palmers_agents_general-0.0.4/src/palmers_agents_general/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.3/src/models_handler.py` & `palmers_agents_general-0.0.4/src/palmers_agents_general/models_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.3/LICENSE` & `palmers_agents_general-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.3/pyproject.toml` & `palmers_agents_general-0.0.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

