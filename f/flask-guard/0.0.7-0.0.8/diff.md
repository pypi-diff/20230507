# Comparing `tmp/flask-guard-0.0.7.tar.gz` & `tmp/flask-guard-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-guard-0.0.7.tar", last modified: Sun May  7 14:01:00 2023, max compression
+gzip compressed data, was "flask-guard-0.0.8.tar", last modified: Sun May  7 16:41:25 2023, max compression
```

## Comparing `flask-guard-0.0.7.tar` & `flask-guard-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.327684 flask-guard-0.0.7/
--rw-rw-rw-   0        0        0     1107 2023-05-07 07:08:02.000000 flask-guard-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2647 2023-05-07 14:01:00.326682 flask-guard-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2166 2023-05-06 09:33:32.000000 flask-guard-0.0.7/README.md
--rw-rw-rw-   0        0        0      102 2023-05-07 07:17:25.000000 flask-guard-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 14:01:00.327684 flask-guard-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      783 2023-05-07 14:00:36.000000 flask-guard-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.285683 flask-guard-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.299676 flask-guard-0.0.7/src/FlaskGuard/
--rw-rw-rw-   0        0        0       86 2023-05-07 14:00:28.000000 flask-guard-0.0.7/src/FlaskGuard/__init__.py
--rw-rw-rw-   0        0        0     6937 2023-05-07 13:15:18.000000 flask-guard-0.0.7/src/FlaskGuard/flask_guard.py
--rw-rw-rw-   0        0        0     3160 2023-05-06 08:13:00.000000 flask-guard-0.0.7/src/FlaskGuard/request_parameter.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.319704 flask-guard-0.0.7/src/flask_guard.egg-info/
--rw-rw-rw-   0        0        0     2647 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 14:01:00.000000 flask-guard-0.0.7/src/flask_guard.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 14:01:00.324674 flask-guard-0.0.7/tests/
--rw-rw-rw-   0        0        0    24667 2023-05-07 13:16:37.000000 flask-guard-0.0.7/tests/test_flask_guard.py
--rw-rw-rw-   0        0        0     7282 2023-05-07 13:13:48.000000 flask-guard-0.0.7/tests/test_request_parameter.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:41:25.607133 flask-guard-0.0.8/
+-rw-rw-rw-   0        0        0     1107 2023-05-07 07:08:02.000000 flask-guard-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2920 2023-05-07 16:41:25.604128 flask-guard-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2439 2023-05-07 16:36:02.000000 flask-guard-0.0.8/README.md
+-rw-rw-rw-   0        0        0      102 2023-05-07 07:17:25.000000 flask-guard-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 16:41:25.607133 flask-guard-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      783 2023-05-07 16:40:32.000000 flask-guard-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:41:25.525128 flask-guard-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 16:41:25.547127 flask-guard-0.0.8/src/FlaskGuard/
+-rw-rw-rw-   0        0        0       86 2023-05-07 14:00:28.000000 flask-guard-0.0.8/src/FlaskGuard/__init__.py
+-rw-rw-rw-   0        0        0     6937 2023-05-07 13:15:18.000000 flask-guard-0.0.8/src/FlaskGuard/flask_guard.py
+-rw-rw-rw-   0        0        0     3160 2023-05-06 08:13:00.000000 flask-guard-0.0.8/src/FlaskGuard/request_parameter.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:41:25.573140 flask-guard-0.0.8/src/flask_guard.egg-info/
+-rw-rw-rw-   0        0        0     2920 2023-05-07 16:41:25.000000 flask-guard-0.0.8/src/flask_guard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-07 16:41:25.000000 flask-guard-0.0.8/src/flask_guard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 16:41:25.000000 flask-guard-0.0.8/src/flask_guard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 16:41:25.000000 flask-guard-0.0.8/src/flask_guard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 16:41:25.602131 flask-guard-0.0.8/tests/
+-rw-rw-rw-   0        0        0    24667 2023-05-07 13:16:37.000000 flask-guard-0.0.8/tests/test_flask_guard.py
+-rw-rw-rw-   0        0        0     7282 2023-05-07 13:13:48.000000 flask-guard-0.0.8/tests/test_request_parameter.py
```

### Comparing `flask-guard-0.0.7/LICENSE.txt` & `flask-guard-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.7/PKG-INFO` & `flask-guard-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-guard
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for checking if JSON requests have valid data.
 Home-page: https://github.com/beki1337/FlaskGuard
 Author: Belmin Batic
 Author-email: baticbelmin10@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,68 +19,81 @@
  requests, ensuring that only requests that meet the specified requirements are allowed to proceed. 
 
 
 ## Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to intall flask-request-gaurd.
 
 ```bash
-pip install flask-request-gaurd
+pip install flask-guard
 ```
 
-## Creat the keys
+## Create the keys
 
 
 ```python
-from FlaskRequestGuard import RequestParameter
+from FlaskGuard import RequestParameter
 
-# Creates a key that has the name "name" and type str with a minimum length of 0 and a maximum length of 10
+# Creates a key that has the name "name" and type str with a minimum length of 0 and 
+# a maximum length of 10
 name_key =  RequestParameter("name", str, 0, 10)
 
-# Creates a key that has the name "range" and type int with a minimum value of -10 and a maximum value of 10
+# Creates a key that has the name "range" and type int with a minimum value of -10 and
+#  a maximum value of 10
 range_key = RequestParameter("range", int, -10, 10)
 
 ```
 
-## Create validate function
+## Create the validation function
 
 ```python
-from FlaskRequestGuard import FlaskRequestGuard
+from FlaskGuard import  FlaskGuard
 
 # Init FlaskRequestGuard
 guard = FlaskRequestGuard("myapp")
 
+# Keys from the code snippet above
 required_keys = [range_key, name_key] 
 
 # Returns a function that is used to check a request
 validate_user_request = guard.create_validate_function(required_keys)
 
 ```
 
 ## Check request
 
 ```python
 request = {"name": "erik", "age": 23, "range": 2}
-# Returns True, {"error_messages": []} 
+# Returns (True, {"error_messages": []}) 
 is_valid, error_messages = validate_user_request(request)
 
 request = {"name": "eeeeeeeeeee", "age": 23, "range": 2}
-# Returns False, {"error_messages": ["The 'name' field must be 10 characters or less,
-#  and at least 0 characters or more, but is actually 11 characters long."]}
+# Returns (False, {"error_messages": ["The 'name' field must be 10 size or less,
+#  and at least 0 size or more, but is actually 11 characters long."]})
 is_valid, error_messages = validate_user_request(request)
 
 
 request = {"age": 23, "range": 2}
 # Returns False, {"error_messages": ["Missing name field in request body."]}
 is_valid, error_messages = validate_user_request(request)
 
 ```
 
+For an example where it's used with Flask, check out FlaskGuard-example [repo](https://github.com/beki1337/flaskguard-example).
 
 
 
+## Run tests
+
+Run this commad in FlaskGuard directory to run the tests
+
+```bash
+python -m unittest discover tests
+```
+
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `flask-guard-0.0.7/README.md` & `flask-guard-0.0.8/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,68 +5,81 @@
  requests, ensuring that only requests that meet the specified requirements are allowed to proceed. 
 
 
 ## Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to intall flask-request-gaurd.
 
 ```bash
-pip install flask-request-gaurd
+pip install flask-guard
 ```
 
-## Creat the keys
+## Create the keys
 
 
 ```python
-from FlaskRequestGuard import RequestParameter
+from FlaskGuard import RequestParameter
 
-# Creates a key that has the name "name" and type str with a minimum length of 0 and a maximum length of 10
+# Creates a key that has the name "name" and type str with a minimum length of 0 and 
+# a maximum length of 10
 name_key =  RequestParameter("name", str, 0, 10)
 
-# Creates a key that has the name "range" and type int with a minimum value of -10 and a maximum value of 10
+# Creates a key that has the name "range" and type int with a minimum value of -10 and
+#  a maximum value of 10
 range_key = RequestParameter("range", int, -10, 10)
 
 ```
 
-## Create validate function
+## Create the validation function
 
 ```python
-from FlaskRequestGuard import FlaskRequestGuard
+from FlaskGuard import  FlaskGuard
 
 # Init FlaskRequestGuard
 guard = FlaskRequestGuard("myapp")
 
+# Keys from the code snippet above
 required_keys = [range_key, name_key] 
 
 # Returns a function that is used to check a request
 validate_user_request = guard.create_validate_function(required_keys)
 
 ```
 
 ## Check request
 
 ```python
 request = {"name": "erik", "age": 23, "range": 2}
-# Returns True, {"error_messages": []} 
+# Returns (True, {"error_messages": []}) 
 is_valid, error_messages = validate_user_request(request)
 
 request = {"name": "eeeeeeeeeee", "age": 23, "range": 2}
-# Returns False, {"error_messages": ["The 'name' field must be 10 characters or less,
-#  and at least 0 characters or more, but is actually 11 characters long."]}
+# Returns (False, {"error_messages": ["The 'name' field must be 10 size or less,
+#  and at least 0 size or more, but is actually 11 characters long."]})
 is_valid, error_messages = validate_user_request(request)
 
 
 request = {"age": 23, "range": 2}
 # Returns False, {"error_messages": ["Missing name field in request body."]}
 is_valid, error_messages = validate_user_request(request)
 
 ```
 
+For an example where it's used with Flask, check out FlaskGuard-example [repo](https://github.com/beki1337/flaskguard-example).
 
 
 
+## Run tests
+
+Run this commad in FlaskGuard directory to run the tests
+
+```bash
+python -m unittest discover tests
+```
+
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `flask-guard-0.0.7/setup.py` & `flask-guard-0.0.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "flask-guard",
-    version = "0.0.7",
+    version = "0.0.8",
     author = "Belmin Batic",
     author_email = "baticbelmin10@gmail.com",
     description = "A library for checking if JSON requests have valid data.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/beki1337/FlaskGuard",
     classifiers = [
```

### Comparing `flask-guard-0.0.7/src/FlaskGuard/flask_guard.py` & `flask-guard-0.0.8/src/FlaskGuard/flask_guard.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.7/src/FlaskGuard/request_parameter.py` & `flask-guard-0.0.8/src/FlaskGuard/request_parameter.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.7/src/flask_guard.egg-info/PKG-INFO` & `flask-guard-0.0.8/src/flask_guard.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-guard
-Version: 0.0.7
+Version: 0.0.8
 Summary: A library for checking if JSON requests have valid data.
 Home-page: https://github.com/beki1337/FlaskGuard
 Author: Belmin Batic
 Author-email: baticbelmin10@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,68 +19,81 @@
  requests, ensuring that only requests that meet the specified requirements are allowed to proceed. 
 
 
 ## Installation
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to intall flask-request-gaurd.
 
 ```bash
-pip install flask-request-gaurd
+pip install flask-guard
 ```
 
-## Creat the keys
+## Create the keys
 
 
 ```python
-from FlaskRequestGuard import RequestParameter
+from FlaskGuard import RequestParameter
 
-# Creates a key that has the name "name" and type str with a minimum length of 0 and a maximum length of 10
+# Creates a key that has the name "name" and type str with a minimum length of 0 and 
+# a maximum length of 10
 name_key =  RequestParameter("name", str, 0, 10)
 
-# Creates a key that has the name "range" and type int with a minimum value of -10 and a maximum value of 10
+# Creates a key that has the name "range" and type int with a minimum value of -10 and
+#  a maximum value of 10
 range_key = RequestParameter("range", int, -10, 10)
 
 ```
 
-## Create validate function
+## Create the validation function
 
 ```python
-from FlaskRequestGuard import FlaskRequestGuard
+from FlaskGuard import  FlaskGuard
 
 # Init FlaskRequestGuard
 guard = FlaskRequestGuard("myapp")
 
+# Keys from the code snippet above
 required_keys = [range_key, name_key] 
 
 # Returns a function that is used to check a request
 validate_user_request = guard.create_validate_function(required_keys)
 
 ```
 
 ## Check request
 
 ```python
 request = {"name": "erik", "age": 23, "range": 2}
-# Returns True, {"error_messages": []} 
+# Returns (True, {"error_messages": []}) 
 is_valid, error_messages = validate_user_request(request)
 
 request = {"name": "eeeeeeeeeee", "age": 23, "range": 2}
-# Returns False, {"error_messages": ["The 'name' field must be 10 characters or less,
-#  and at least 0 characters or more, but is actually 11 characters long."]}
+# Returns (False, {"error_messages": ["The 'name' field must be 10 size or less,
+#  and at least 0 size or more, but is actually 11 characters long."]})
 is_valid, error_messages = validate_user_request(request)
 
 
 request = {"age": 23, "range": 2}
 # Returns False, {"error_messages": ["Missing name field in request body."]}
 is_valid, error_messages = validate_user_request(request)
 
 ```
 
+For an example where it's used with Flask, check out FlaskGuard-example [repo](https://github.com/beki1337/flaskguard-example).
 
 
 
+## Run tests
+
+Run this commad in FlaskGuard directory to run the tests
+
+```bash
+python -m unittest discover tests
+```
+
+
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
 
 Please make sure to update tests as appropriate.
```

### Comparing `flask-guard-0.0.7/tests/test_flask_guard.py` & `flask-guard-0.0.8/tests/test_flask_guard.py`

 * *Files identical despite different names*

### Comparing `flask-guard-0.0.7/tests/test_request_parameter.py` & `flask-guard-0.0.8/tests/test_request_parameter.py`

 * *Files identical despite different names*

