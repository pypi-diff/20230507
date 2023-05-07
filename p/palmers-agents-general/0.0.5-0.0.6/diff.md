# Comparing `tmp/palmers_agents_general-0.0.5.tar.gz` & `tmp/palmers_agents_general-0.0.6.tar.gz`

## Comparing `palmers_agents_general-0.0.5.tar` & `palmers_agents_general-0.0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/palmers_agents_general/__init__.py
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/palmers_agents_general/base_mq_consumer.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/palmers_agents_general/blobs_handler.py
--rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/palmers_agents_general/models_handler.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/LICENSE
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/README.md
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/__init__.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/base_mq_consumer.py
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/blobs_handler.py
+-rw-r--r--   0        0        0     1971 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/palmers_agents_general/models_handler.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/LICENSE
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/README.md
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 palmers_agents_general-0.0.6/PKG-INFO
```

### Comparing `palmers_agents_general-0.0.5/palmers_agents_general/base_mq_consumer.py` & `palmers_agents_general-0.0.6/palmers_agents_general/base_mq_consumer.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.5/palmers_agents_general/blobs_handler.py` & `palmers_agents_general-0.0.6/palmers_agents_general/blobs_handler.py`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.5/palmers_agents_general/models_handler.py` & `palmers_agents_general-0.0.6/palmers_agents_general/models_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             store_data = data_dict[store]
             df = store_data['data']
             model_url = store_data['model_url'] #serve/model_100_endpoint
 
             data_size = sys.getsizeof(df)
             print(f'store: {store}, data size: {data_size}')
             if data_size > message_max_size:
-                raise Exception(f'error: store {store} data size > {MESSAGE_MAX_SIZE / (1024 * 1024)} MB')
+                raise Exception(f'error: store {store} data size > {message_max_size / (1024 * 1024)} MB')
 
             # send to model
             pickled = pickle.dumps(df)
             pickled_b64 = base64.b64encode(pickled)
             data_str = pickled_b64.decode('utf-8')
             url = f'{inference_protocol}://{inference_url}/{inference_prefix}/{model_url}'  # Replace with your API endpoint
```

### Comparing `palmers_agents_general-0.0.5/LICENSE` & `palmers_agents_general-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `palmers_agents_general-0.0.5/pyproject.toml` & `palmers_agents_general-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "palmers_agents_general"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Assaf", email="assafm@sdatta.ai" },
   { name="Roy ", email="roy@sdatta.ai" },
   { name="Guy", email="assafm@sdatta.ai" },
   { name="Oran", email="assafm@sdatta.ai" },
   { name="Yotam", email="assafm@sdatta.ai" },
 ]
```

### Comparing `palmers_agents_general-0.0.5/PKG-INFO` & `palmers_agents_general-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: palmers_agents_general
-Version: 0.0.5
+Version: 0.0.6
 Summary: A package to preprocess data for Palmer's project
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Assaf <assafm@sdatta.ai>, Roy  <roy@sdatta.ai>, Guy <assafm@sdatta.ai>, Oran <assafm@sdatta.ai>, Yotam <assafm@sdatta.ai>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

