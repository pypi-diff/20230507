# Comparing `tmp/qwak_inference-0.1.1.tar.gz` & `tmp/qwak_inference-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak_inference-0.1.1.tar", max compression
+gzip compressed data, was "qwak_inference-0.1.2.tar", max compression
```

## Comparing `qwak_inference-0.1.1.tar` & `qwak_inference-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    10480 2023-05-02 13:55:52.013938 qwak_inference-0.1.1/LICENSE
--rw-r--r--   0        0        0      267 2023-05-02 13:55:52.013938 qwak_inference-0.1.1/README.md
--rw-r--r--   0        0        0     1892 2023-05-02 13:56:41.690164 qwak_inference-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      804 2023-05-02 13:56:41.690164 qwak_inference-0.1.1/qwak_inference/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/batch_client/__init__.py
--rw-r--r--   0        0        0    19390 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/batch_client/batch_client.py
--rw-r--r--   0        0        0     2172 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/batch_client/file_serialization.py
--rw-r--r--   0        0        0      739 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/batch_client/s3.py
--rw-r--r--   0        0        0       95 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/configuration/__init__.py
--rw-r--r--   0        0        0     3127 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/configuration/account.py
--rw-r--r--   0        0        0     2676 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/configuration/auth.py
--rw-r--r--   0        0        0      929 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/configuration/session.py
--rw-r--r--   0        0        0      688 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/constants.py
--rw-r--r--   0        0        0     1592 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/exceptions.py
--rw-r--r--   0        0        0     1999 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/feedback_client.py
--rw-r--r--   0        0        0       65 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/realtime_client/__init__.py
--rw-r--r--   0        0        0     4795 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/realtime_client/client.py
--rw-r--r--   0        0        0     1076 2023-05-02 13:55:52.017938 qwak_inference-0.1.1/qwak_inference/realtime_client/rest_helpers.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qwak_inference-0.1.1/setup.py
--rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 qwak_inference-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10480 2023-05-07 13:04:57.312812 qwak_inference-0.1.2/LICENSE
+-rw-r--r--   0        0        0      267 2023-05-07 13:04:57.312812 qwak_inference-0.1.2/README.md
+-rw-r--r--   0        0        0     1892 2023-05-07 13:05:53.421143 qwak_inference-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      804 2023-05-07 13:05:53.421143 qwak_inference-0.1.2/qwak_inference/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/batch_client/__init__.py
+-rw-r--r--   0        0        0    19390 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/batch_client/batch_client.py
+-rw-r--r--   0        0        0     2172 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/batch_client/file_serialization.py
+-rw-r--r--   0        0        0      739 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/batch_client/s3.py
+-rw-r--r--   0        0        0       95 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/configuration/__init__.py
+-rw-r--r--   0        0        0     3127 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/configuration/account.py
+-rw-r--r--   0        0        0     2676 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/configuration/auth.py
+-rw-r--r--   0        0        0      929 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/configuration/session.py
+-rw-r--r--   0        0        0      688 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/constants.py
+-rw-r--r--   0        0        0     1592 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/exceptions.py
+-rw-r--r--   0        0        0     1999 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/feedback_client.py
+-rw-r--r--   0        0        0       65 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/realtime_client/__init__.py
+-rw-r--r--   0        0        0     4810 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/realtime_client/client.py
+-rw-r--r--   0        0        0     1076 2023-05-07 13:04:57.316813 qwak_inference-0.1.2/qwak_inference/realtime_client/rest_helpers.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 qwak_inference-0.1.2/setup.py
+-rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 qwak_inference-0.1.2/PKG-INFO
```

### Comparing `qwak_inference-0.1.1/LICENSE` & `qwak_inference-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/pyproject.toml` & `qwak_inference-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qwak-inference"
-version = "0.1.1"
+version = "0.1.2"
 description = "Qwak Inference is a Python library for running predictions again Qwak Models."
 authors = ["Qwak <info@qwak.com>"]
 readme = "README.md"
 keywords = ["mlops", "ml", "deployment", "serving", "model"]
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.7",
```

### Comparing `qwak_inference-0.1.1/qwak_inference/__init__.py` & `qwak_inference-0.1.2/qwak_inference/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
     print(
         "Notice that BatchInferenceClient and FeedbackClient are not available in the skinny package. "
         'In order to use them, please install them as extras: pip install "qwak-inference[batch,feedback]".'
     )
 
 __all__ = clients
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
```

### Comparing `qwak_inference-0.1.1/qwak_inference/batch_client/batch_client.py` & `qwak_inference-0.1.2/qwak_inference/batch_client/batch_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/batch_client/file_serialization.py` & `qwak_inference-0.1.2/qwak_inference/batch_client/file_serialization.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/batch_client/s3.py` & `qwak_inference-0.1.2/qwak_inference/batch_client/s3.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/configuration/account.py` & `qwak_inference-0.1.2/qwak_inference/configuration/account.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/configuration/auth.py` & `qwak_inference-0.1.2/qwak_inference/configuration/auth.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/configuration/session.py` & `qwak_inference-0.1.2/qwak_inference/configuration/session.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/constants.py` & `qwak_inference-0.1.2/qwak_inference/constants.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/exceptions.py` & `qwak_inference-0.1.2/qwak_inference/exceptions.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/feedback_client.py` & `qwak_inference-0.1.2/qwak_inference/feedback_client.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/qwak_inference/realtime_client/client.py` & `qwak_inference-0.1.2/qwak_inference/realtime_client/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,17 +79,16 @@
 
             response = self.r_session.post(
                 self.model_api, data=feature_vectors, headers=rule_based_traffic
             )
 
             if response.status_code >= 400:
                 exception_class_name = response.headers.get("X-Exception-Class")
-                raise QwakHTTPException(
-                    response.status_code, response.json(), exception_class_name
-                )
+                msg = f"{response.status_code}: {response.text}"
+                raise QwakHTTPException(response.status_code, msg, exception_class_name)
 
             elif response.status_code != 200:
                 raise QwakHTTPException(response.status_code, response.content)
 
             if output_format == InferenceOutputFormat.DICTIONARY:
                 dict_response = json.loads(response.content)
                 return dict_response
```

### Comparing `qwak_inference-0.1.1/qwak_inference/realtime_client/rest_helpers.py` & `qwak_inference-0.1.2/qwak_inference/realtime_client/rest_helpers.py`

 * *Files identical despite different names*

### Comparing `qwak_inference-0.1.1/setup.py` & `qwak_inference-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'feedback:python_full_version >= "3.7.1" and python_version < "3.8"': ['pandas<1.4',
                                                                         'pandas<1.4'],
  'feedback:python_version >= "3.8" and python_version < "3.10"': ['pandas>=1.4.3,<2.0.0',
                                                                   'pandas>=1.4.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'qwak-inference',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': 'Qwak Inference is a Python library for running predictions again Qwak Models.',
     'long_description': '# Qwak Inference\n\nQwak is an end-to-end production ML platform designed to allow data scientists to build, deploy, and monitor their models in production with minimal engineering friction.\nQwak Inference contains tools that allow predicting against the Qwak Platform\n',
     'author': 'Qwak',
     'author_email': 'info@qwak.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `qwak_inference-0.1.1/PKG-INFO` & `qwak_inference-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-inference
-Version: 0.1.1
+Version: 0.1.2
 Summary: Qwak Inference is a Python library for running predictions again Qwak Models.
 License: Apache-2.0
 Keywords: mlops,ml,deployment,serving,model
 Author: Qwak
 Author-email: info@qwak.com
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: Apache Software License
```

