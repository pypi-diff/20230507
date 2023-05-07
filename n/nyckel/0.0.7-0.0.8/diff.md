# Comparing `tmp/nyckel-0.0.7.tar.gz` & `tmp/nyckel-0.0.8.tar.gz`

## Comparing `nyckel-0.0.7.tar` & `nyckel-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 nyckel-0.0.7/requirements.txt
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nyckel-0.0.7/.github/workflows/build.yml
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nyckel-0.0.7/.github/workflows/test.yml
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/__about__.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/__init__.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/auth.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/config.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/request_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/__init__.py
--rw-r--r--   0        0        0     5256 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/text_classification_function.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.7/src/nyckel/functions/utils.py
--rw-r--r--   0        0        0     1538 2020-02-02 00:00:00.000000 nyckel-0.0.7/tests/test_text_classification_function.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.7/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.7/LICENSE
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nyckel-0.0.7/README.md
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 nyckel-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nyckel-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nyckel-0.0.8/requirements.txt
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 nyckel-0.0.8/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 nyckel-0.0.8/.github/workflows/test.yml
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 nyckel-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/__about__.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/__init__.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/auth.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/config.py
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/request_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/__init__.py
+-rw-r--r--   0        0        0     6411 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/text_classification_function.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nyckel-0.0.8/src/nyckel/functions/utils.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 nyckel-0.0.8/tests/test_text_classification_function.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.8/LICENSE
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nyckel-0.0.8/README.md
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 nyckel-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 nyckel-0.0.8/PKG-INFO
```

### Comparing `nyckel-0.0.7/.github/workflows/build.yml` & `nyckel-0.0.8/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.7/.github/workflows/test.yml` & `nyckel-0.0.8/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.7/src/nyckel/auth.py` & `nyckel-0.0.8/src/nyckel/auth.py`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.7/src/nyckel/request_utils.py` & `nyckel-0.0.8/src/nyckel/request_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,16 +12,16 @@
         self._session = session
         self._endpoint = endpoint
 
     def _post_as_json(self, data: Dict):
         response = self._session.post(self._endpoint, json=data)
         return response
 
-    def __call__(self, bodies: List[Dict]) -> Dict[Dict, requests.Response]:
-        responses = [None] * len(bodies)
+    def __call__(self, bodies: List[Dict]) -> List[requests.Response]:
+        responses = [requests.Response()] * len(bodies)
         n_workers = min(len(bodies), NBR_CONCURRENT_REQUESTS)
 
         with concurrent.futures.ThreadPoolExecutor(max_workers=n_workers) as executor:
             index_by_future = {executor.submit(self._post_as_json, body): index for index, body in enumerate(bodies)}
             for future in tqdm(concurrent.futures.as_completed(index_by_future)):
                 index = index_by_future[future]
                 body = bodies[index]
```

### Comparing `nyckel-0.0.7/src/nyckel/functions/text_classification_function.py` & `nyckel-0.0.8/src/nyckel/functions/text_classification_function.py`

 * *Files 17% similar despite different names*

```diff
@@ -42,23 +42,36 @@
 
         assert response.status_code == 200, f"Something went wrong when creating function: {response.text}"
         prefixed_function_id = response.json()["id"]
         function_id = strip_nyckel_prefix(prefixed_function_id)
         print(f"Created function {name} with id: {function_id}")
         return TextClassificationFunction(function_id, auth)
 
+    @property
+    def train_page(self):
+        return f"{self._auth.server_url}/console/functions/{self._function_id}/train"
+
     def __str__(self):
         return self.train_page
 
     def __repr__(self):
         return self.train_page
 
-    @property
-    def train_page(self):
-        return f"{self._auth.server_url}/console/functions/{self._function_id}/train"
+    def __call__(self, sample_data: str) -> ClassificationPrediction:
+        self._refresh_auth_token()
+        body = {"data": sample_data}
+        endpoint = self.api_endpoint("invoke")
+        response = self._session.post(endpoint, json=body)
+        if "No model available" in response.text:
+            raise ValueError(f"No model trained yet for this function. Go to {self.train_page} to see function status.")
+
+        assert response.status_code == 200, f"Invoke failed with {response.status_code=}, {response.text=}"
+        return ClassificationPrediction(
+            label_name=response.json()["labelName"], confidence=response.json()["confidence"]
+        )
 
     def has_trained_model(self) -> bool:
         self._refresh_auth_token()
         body = {"data": "dummy data"}
         endpoint = self.api_endpoint("invoke")
         response = self._session.post(endpoint, json=body)
         if "No model available" in response.text:
@@ -72,28 +85,14 @@
             return f"{self._auth.server_url}/{api_version}/functions/{self._function_id}"
         else:
             return f"{self._auth.server_url}/{api_version}/functions/{self._function_id}/{slug}"
 
     def _refresh_auth_token(self):
         self._session.headers.update({"authorization": "Bearer " + self._auth.token})
 
-    def __call__(self, sample_data: str) -> ClassificationPrediction:
-        self._refresh_auth_token()
-        body = {"data": sample_data}
-        endpoint = self.api_endpoint("invoke")
-        response = self._session.post(endpoint, json=body)
-        if "No model available" in response.text:
-            print(f"No model trained yet for this function. Go to {self.train_page} to see function status.")
-            return None
-
-        assert response.status_code == 200, f"Invoke failed with {response.status_code=}, {response.text=}"
-        return ClassificationPrediction(
-            label_name=response.json()["labelName"], confidence=response.json()["confidence"]
-        )
-
     def invoke(self, sample_data_list: List[str]) -> List[ClassificationPrediction]:
         self._refresh_auth_token()
         print(f"Invoking {len(sample_data_list)} labels to {self.train_page} ...")
         bodies = [{"data": sample_data} for sample_data in sample_data_list]
         endpoint = self.api_endpoint("invoke")
         response_list = ParallelPoster(self._session, endpoint)(bodies)
         return [
@@ -121,9 +120,33 @@
         endpoint = self.api_endpoint("")
         response = self._session.delete(endpoint)
         assert response.status_code == 200, f"Delete failed with {response.status_code=}, {response.text=}"
         print(f"Function {self.train_page} deleted.")
 
     def get_samples(self) -> List[TextClassificationSample]:
         self._refresh_auth_token()
-        samples_return = repeated_get(self._session, self.api_endpoint("samples"))
-        return samples_return
+        samples_dict_list = repeated_get(self._session, self.api_endpoint("samples"))
+        labels_dict_list = repeated_get(self._session, self.api_endpoint("labels"))
+        labelname_by_labelid = {l["id"]: l["name"] for l in labels_dict_list}
+        samples_typed = []
+        for sample_dict in samples_dict_list:
+            if "annotation" in sample_dict:
+                annotation = labelname_by_labelid[sample_dict["annotation"]["labelId"]]
+            else:
+                annotation = None
+            if "prediction" in sample_dict:
+                prediction = ClassificationPrediction(
+                    label_name=labelname_by_labelid[sample_dict["prediction"]["labelId"]],
+                    confidence=sample_dict["prediction"]["confidence"],
+                )
+            else:
+                prediction = None
+            samples_typed.append(
+                TextClassificationSample(data=sample_dict["data"], annotation=annotation, prediction=prediction)
+            )
+        return samples_typed
+
+    def get_labels(self) -> List[str]:
+        self._refresh_auth_token()
+        labels_dict_list = repeated_get(self._session, self.api_endpoint("labels"))
+        label_names = [entry["name"] for entry in labels_dict_list]
+        return label_names
```

### Comparing `nyckel-0.0.7/tests/test_text_classification_function.py` & `nyckel-0.0.8/tests/test_text_classification_function.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,20 +21,31 @@
         TextClassificationSample(data="I'm leaving", annotation="Boo"),
         TextClassificationSample(data="Hi again"),
     ]
 
     rate_my_greeting_function = TextClassificationFunction.new("RateMyGreeting", auth)
 
     rate_my_greeting_function.add_labels(["Nice", "Boo"])
+    label_names_post_complete = False
+    while not label_names_post_complete:
+        print("Labels not posted yet. Sleeping 1 sec...")
+        time.sleep(1)
+        label_names = rate_my_greeting_function.get_labels()
+        label_names_post_complete = set(label_names) == set(["Nice", "Boo"])
+
     rate_my_greeting_function.add_samples(samples)
 
     has_trained_model = False
     while not has_trained_model:
+        print("No trained model yet. Sleeping 1 sec...")
         time.sleep(1)
         has_trained_model = rate_my_greeting_function.has_trained_model()
-        print("No trained model yet. Sleeping 1 sec.")
 
     assert isinstance(rate_my_greeting_function("Howdy"), ClassificationPrediction)
 
     assert len(rate_my_greeting_function.invoke(["Hej", "Hola", "Gruezi"])) == 3
 
+    returned_samples = rate_my_greeting_function.get_samples()
+    assert len(samples) == len(returned_samples)
+    assert isinstance(returned_samples[0], TextClassificationSample)
+
     rate_my_greeting_function.delete()
```

### Comparing `nyckel-0.0.7/.gitignore` & `nyckel-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.7/LICENSE` & `nyckel-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.7/pyproject.toml` & `nyckel-0.0.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -30,8 +30,15 @@
 "Homepage" = "https://github.com/NyckelAI/python-sdk"
 
 [tool.ruff]
 line-length = 120
 select = [
     "F401",
     "F403",
-]
+]
+
+[tool.mypy]
+python_version = "3.9"
+
+[[tool.mypy.overrides]]
+module = "src"
+disallow_untyped_defs = true
```

### Comparing `nyckel-0.0.7/PKG-INFO` & `nyckel-0.0.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyckel
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python package for the Nyckel API
 Project-URL: Homepage, https://github.com/NyckelAI/python-sdk
 Author-email: Oscar Beijbom <oscar@nyckel.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

