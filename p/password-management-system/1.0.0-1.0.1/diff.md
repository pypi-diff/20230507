# Comparing `tmp/password-management-system-1.0.0.tar.gz` & `tmp/password-management-system-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "password-management-system-1.0.0.tar", last modified: Sun May  7 08:25:20 2023, max compression
+gzip compressed data, was "password-management-system-1.0.1.tar", last modified: Sun May  7 08:54:52 2023, max compression
```

## Comparing `password-management-system-1.0.0.tar` & `password-management-system-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 08:25:20.170805 password-management-system-1.0.0/
--rw-rw-rw-   0        0        0     1784 2023-05-07 08:25:20.170805 password-management-system-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1412 2023-05-07 08:18:52.000000 password-management-system-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 08:25:20.151974 password-management-system-1.0.0/password_management_system.egg-info/
--rw-rw-rw-   0        0        0     1784 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      561 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       35 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-07 08:25:20.000000 password-management-system-1.0.0/password_management_system.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 08:25:20.164305 password-management-system-1.0.0/pms/
--rw-rw-rw-   0        0        0        0 2023-05-03 11:19:30.000000 password-management-system-1.0.0/pms/__init__.py
--rw-rw-rw-   0        0        0     4122 2023-05-07 07:25:33.000000 password-management-system-1.0.0/pms/__main__.py
--rw-rw-rw-   0        0        0     2065 2023-05-03 13:05:24.000000 password-management-system-1.0.0/pms/db_functions.py
--rw-rw-rw-   0        0        0     8685 2023-05-07 08:25:03.000000 password-management-system-1.0.0/pms/models.py
--rw-rw-rw-   0        0        0     1884 2023-05-04 07:43:36.000000 password-management-system-1.0.0/pms/password_controller.py
--rw-rw-rw-   0        0        0     1713 2023-05-04 13:45:11.000000 password-management-system-1.0.0/pms/user_controller.py
--rw-rw-rw-   0        0        0     2890 2023-05-03 13:09:02.000000 password-management-system-1.0.0/pms/utility_functions.py
--rw-rw-rw-   0        0        0      632 2023-05-07 08:22:53.000000 password-management-system-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 08:25:20.171801 password-management-system-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 08:25:20.168812 password-management-system-1.0.0/tests/
--rw-rw-rw-   0        0        0     3884 2023-05-04 08:16:38.000000 password-management-system-1.0.0/tests/test_password_functions.py
--rw-rw-rw-   0        0        0     2543 2023-05-03 12:43:08.000000 password-management-system-1.0.0/tests/test_user_functions.py
--rw-rw-rw-   0        0        0     1310 2023-05-03 13:09:02.000000 password-management-system-1.0.0/tests/test_utility_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-07 08:54:52.443601 password-management-system-1.0.1/
+-rw-rw-rw-   0        0        0     1807 2023-05-07 08:54:52.442600 password-management-system-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1435 2023-05-07 08:53:33.000000 password-management-system-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 08:54:52.431422 password-management-system-1.0.1/password_management_system.egg-info/
+-rw-rw-rw-   0        0        0     1807 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      561 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       35 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-07 08:54:52.000000 password-management-system-1.0.1/password_management_system.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 08:54:52.438637 password-management-system-1.0.1/pms/
+-rw-rw-rw-   0        0        0        0 2023-05-03 11:19:30.000000 password-management-system-1.0.1/pms/__init__.py
+-rw-rw-rw-   0        0        0     4122 2023-05-07 07:25:33.000000 password-management-system-1.0.1/pms/__main__.py
+-rw-rw-rw-   0        0        0     2065 2023-05-03 13:05:24.000000 password-management-system-1.0.1/pms/db_functions.py
+-rw-rw-rw-   0        0        0     8685 2023-05-07 08:25:03.000000 password-management-system-1.0.1/pms/models.py
+-rw-rw-rw-   0        0        0     1884 2023-05-04 07:43:36.000000 password-management-system-1.0.1/pms/password_controller.py
+-rw-rw-rw-   0        0        0     1713 2023-05-04 13:45:11.000000 password-management-system-1.0.1/pms/user_controller.py
+-rw-rw-rw-   0        0        0     2890 2023-05-03 13:09:02.000000 password-management-system-1.0.1/pms/utility_functions.py
+-rw-rw-rw-   0        0        0      632 2023-05-07 08:54:35.000000 password-management-system-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 08:54:52.443601 password-management-system-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 08:54:52.441602 password-management-system-1.0.1/tests/
+-rw-rw-rw-   0        0        0     3884 2023-05-04 08:16:38.000000 password-management-system-1.0.1/tests/test_password_functions.py
+-rw-rw-rw-   0        0        0     2543 2023-05-03 12:43:08.000000 password-management-system-1.0.1/tests/test_user_functions.py
+-rw-rw-rw-   0        0        0     1310 2023-05-03 13:09:02.000000 password-management-system-1.0.1/tests/test_utility_functions.py
```

### Comparing `password-management-system-1.0.0/PKG-INFO` & `password-management-system-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: password-management-system
-Version: 1.0.0
+Version: 1.0.1
 Summary: password management system through cli
 Keywords: cli
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 password management system (pms) is a cli app to store and manage your passwords
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pms.
 
 ```bash
-pip install pms
+pip install password-management-system
 ```
 
 ## User
 Signup and login user to add passwords for them:
 ```bash
 pms signup ahmad 123
 pms login ahmad 123
```

### Comparing `password-management-system-1.0.0/README.md` & `password-management-system-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 password management system (pms) is a cli app to store and manage your passwords
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pms.
 
 ```bash
-pip install pms
+pip install password-management-system
 ```
 
 ## User
 Signup and login user to add passwords for them:
 ```bash
 pms signup ahmad 123
 pms login ahmad 123
```

### Comparing `password-management-system-1.0.0/password_management_system.egg-info/PKG-INFO` & `password-management-system-1.0.1/password_management_system.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: password-management-system
-Version: 1.0.0
+Version: 1.0.1
 Summary: password management system through cli
 Keywords: cli
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -15,15 +15,15 @@
 password management system (pms) is a cli app to store and manage your passwords
 
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install pms.
 
 ```bash
-pip install pms
+pip install password-management-system
 ```
 
 ## User
 Signup and login user to add passwords for them:
 ```bash
 pms signup ahmad 123
 pms login ahmad 123
```

### Comparing `password-management-system-1.0.0/password_management_system.egg-info/SOURCES.txt` & `password-management-system-1.0.1/password_management_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/__main__.py` & `password-management-system-1.0.1/pms/__main__.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/db_functions.py` & `password-management-system-1.0.1/pms/db_functions.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/models.py` & `password-management-system-1.0.1/pms/models.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/password_controller.py` & `password-management-system-1.0.1/pms/password_controller.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/user_controller.py` & `password-management-system-1.0.1/pms/user_controller.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pms/utility_functions.py` & `password-management-system-1.0.1/pms/utility_functions.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/pyproject.toml` & `password-management-system-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "password-management-system"
-version = "1.0.0"
+version = "1.0.1"
 description = "password management system through cli"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `password-management-system-1.0.0/tests/test_password_functions.py` & `password-management-system-1.0.1/tests/test_password_functions.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/tests/test_user_functions.py` & `password-management-system-1.0.1/tests/test_user_functions.py`

 * *Files identical despite different names*

### Comparing `password-management-system-1.0.0/tests/test_utility_functions.py` & `password-management-system-1.0.1/tests/test_utility_functions.py`

 * *Files identical despite different names*

