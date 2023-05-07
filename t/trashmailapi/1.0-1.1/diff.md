# Comparing `tmp/trashmailapi-1.0.tar.gz` & `tmp/trashmailapi-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trashmailapi-1.0.tar", last modified: Sun May  7 19:19:23 2023, max compression
+gzip compressed data, was "trashmailapi-1.1.tar", last modified: Sun May  7 20:09:21 2023, max compression
```

## Comparing `trashmailapi-1.0.tar` & `trashmailapi-1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 19:19:23.379917 trashmailapi-1.0/
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1078 2023-05-03 09:43:31.000000 trashmailapi-1.0/LICENSE
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1159 2023-05-07 19:19:23.379917 trashmailapi-1.0/PKG-INFO
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)      625 2023-05-07 19:14:55.000000 trashmailapi-1.0/README.md
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)      793 2023-05-03 09:43:31.000000 trashmailapi-1.0/pyproject.toml
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)       38 2023-05-07 19:19:23.379917 trashmailapi-1.0/setup.cfg
-drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 19:19:23.376584 trashmailapi-1.0/src/
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)        0 2023-05-03 09:43:31.000000 trashmailapi-1.0/src/__init__.py
-drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 19:19:23.376584 trashmailapi-1.0/src/trashmailapi/
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)        0 2023-05-03 09:43:31.000000 trashmailapi-1.0/src/trashmailapi/__init__.py
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)     2502 2023-05-07 17:56:08.000000 trashmailapi-1.0/src/trashmailapi/vsimcard.py
-drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 19:19:23.379917 trashmailapi-1.0/src/trashmailapi.egg-info/
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1159 2023-05-07 19:19:23.000000 trashmailapi-1.0/src/trashmailapi.egg-info/PKG-INFO
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)      305 2023-05-07 19:19:23.000000 trashmailapi-1.0/src/trashmailapi.egg-info/SOURCES.txt
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)        1 2023-05-07 19:19:23.000000 trashmailapi-1.0/src/trashmailapi.egg-info/dependency_links.txt
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)      129 2023-05-07 19:19:23.000000 trashmailapi-1.0/src/trashmailapi.egg-info/requires.txt
--rw-r--r--   0 johndoe   (1000) johndoe   (1000)       22 2023-05-07 19:19:23.000000 trashmailapi-1.0/src/trashmailapi.egg-info/top_level.txt
+drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 20:09:21.756797 trashmailapi-1.1/
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1078 2023-05-03 09:43:31.000000 trashmailapi-1.1/LICENSE
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1159 2023-05-07 20:09:21.756797 trashmailapi-1.1/PKG-INFO
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)      625 2023-05-07 19:14:55.000000 trashmailapi-1.1/README.md
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)      793 2023-05-07 20:08:09.000000 trashmailapi-1.1/pyproject.toml
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)       38 2023-05-07 20:09:21.756797 trashmailapi-1.1/setup.cfg
+drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 20:09:21.756797 trashmailapi-1.1/src/
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)        0 2023-05-03 09:43:31.000000 trashmailapi-1.1/src/__init__.py
+drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 20:09:21.756797 trashmailapi-1.1/src/trashmailapi/
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)        0 2023-05-03 09:43:31.000000 trashmailapi-1.1/src/trashmailapi/__init__.py
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)     2253 2023-05-07 20:08:10.000000 trashmailapi-1.1/src/trashmailapi/vsimcard.py
+drwxr-xr-x   0 johndoe   (1000) johndoe   (1000)        0 2023-05-07 20:09:21.756797 trashmailapi-1.1/src/trashmailapi.egg-info/
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)     1159 2023-05-07 20:09:21.000000 trashmailapi-1.1/src/trashmailapi.egg-info/PKG-INFO
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)      305 2023-05-07 20:09:21.000000 trashmailapi-1.1/src/trashmailapi.egg-info/SOURCES.txt
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)        1 2023-05-07 20:09:21.000000 trashmailapi-1.1/src/trashmailapi.egg-info/dependency_links.txt
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)      129 2023-05-07 20:09:21.000000 trashmailapi-1.1/src/trashmailapi.egg-info/requires.txt
+-rw-r--r--   0 johndoe   (1000) johndoe   (1000)       22 2023-05-07 20:09:21.000000 trashmailapi-1.1/src/trashmailapi.egg-info/top_level.txt
```

### Comparing `trashmailapi-1.0/LICENSE` & `trashmailapi-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `trashmailapi-1.0/PKG-INFO` & `trashmailapi-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trashmailapi
-Version: 1.0
+Version: 1.1
 Summary: Unofficial API for trash/temporary mail services in Python
 Author-email: mazer <DO-NOT-EMAIL@example.com>
 Project-URL: Homepage, https://codeberg.org/m3r/trashmailapi
 Project-URL: Bug Tracker, https://codeberg.org/m3r/trashmailapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trashmailapi-1.0/README.md` & `trashmailapi-1.1/README.md`

 * *Files identical despite different names*

### Comparing `trashmailapi-1.0/pyproject.toml` & `trashmailapi-1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trashmailapi"
-version = "1.0"
+version = "1.1"
 authors = [
   { name="mazer", email="DO-NOT-EMAIL@example.com" },
 ]
 
 description = "Unofficial API for trash/temporary mail services in Python"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `trashmailapi-1.0/src/trashmailapi/vsimcard.py` & `trashmailapi-1.1/src/trashmailapi/vsimcard.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,20 +52,7 @@
             if mail.content and mail.id == mailid:
                 return mail.content
             elif not mail.content and mail.id == mailid:
                 retrievedcontent = req.get(f"{TRASHCONTENT}{self.addy}&nr={mailid}").text
                 mail.content = retrievedcontent
                 self.contentbox.append(mail.content)
                 return mail.content
-
-
-user = Vsimcard("emailaddress")
-
-user.get_emails() # fetch emails except for content
-
-mail = None
-
-for i in user.inbox:
-    if "verify" in i.subject:
-        mail = user.get_content(i.id) # gets the email body/content using mail ID's
-
-print(mail)
```

### Comparing `trashmailapi-1.0/src/trashmailapi.egg-info/PKG-INFO` & `trashmailapi-1.1/src/trashmailapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trashmailapi
-Version: 1.0
+Version: 1.1
 Summary: Unofficial API for trash/temporary mail services in Python
 Author-email: mazer <DO-NOT-EMAIL@example.com>
 Project-URL: Homepage, https://codeberg.org/m3r/trashmailapi
 Project-URL: Bug Tracker, https://codeberg.org/m3r/trashmailapi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

