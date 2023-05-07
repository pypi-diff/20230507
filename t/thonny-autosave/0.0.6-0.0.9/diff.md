# Comparing `tmp/thonny-autosave-0.0.6.tar.gz` & `tmp/thonny-autosave-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thonny-autosave-0.0.6.tar", last modified: Thu May  4 00:43:02 2023, max compression
+gzip compressed data, was "thonny-autosave-0.0.9.tar", last modified: Thu May  4 00:56:14 2023, max compression
```

## Comparing `thonny-autosave-0.0.6.tar` & `thonny-autosave-0.0.9.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:43:02.000000 thonny-autosave-0.0.6/src/thonny_autosave.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonnycontrib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:43:02.429878 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 00:42:52.000000 thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.223094 thonny-autosave-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.215094 thonny-autosave-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.219094 thonny-autosave-0.0.9/.github/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1328 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.219094 thonny-autosave-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 00:56:14.223094 thonny-autosave-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-05-04 00:56:14.223094 thonny-autosave-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.219094 thonny-autosave-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.223094 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-04 00:56:14.000000 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-04 00:56:14.000000 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:56:14.000000 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 00:56:14.000000 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:56:14.000000 thonny-autosave-0.0.9/src/thonny_autosave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.219094 thonny-autosave-0.0.9/src/thonnycontrib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:14.223094 thonny-autosave-0.0.9/src/thonnycontrib/thonny-autosave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/src/thonnycontrib/thonny-autosave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-04 00:56:06.000000 thonny-autosave-0.0.9/src/thonnycontrib/thonny-autosave/app.py
```

### Comparing `thonny-autosave-0.0.6/.github/scripts/release.py` & `thonny-autosave-0.0.9/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `thonny-autosave-0.0.6/LICENSE` & `thonny-autosave-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thonny-autosave-0.0.6/PKG-INFO` & `thonny-autosave-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: thonny-autosave
-Version: 0.0.6
+Version: 0.0.9
 Summary: Adds a checkbox to the File menu of Thonny editor, when activated , automatically saves current file every 10 seconds.
 Home-page: https://github.com/selmen2004/thonny-autosave
 Project-URL: Bug Tracker, https://github.com/selmen2004/thonny-autosave/issues
 Project-URL: Changelog, https://github.com/selmen2004/thonny-autosave/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-"# thonny-autosave
-Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds
+"# thonny-autosave\n
+Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds\n
 ![image](https://user-images.githubusercontent.com/3520243/236076489-a0196681-a98d-4d80-8539-ce45723606da.png)"
```

### Comparing `thonny-autosave-0.0.6/setup.cfg` & `thonny-autosave-0.0.9/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [metadata]
 name = thonny-autosave
 description = Adds a checkbox to the File menu of Thonny editor, when activated , automatically saves current file every 10 seconds.
-long_description = "# thonny-autosave
-	Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds
+long_description = "# thonny-autosave\n
+	Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds\n
 	![image](https://user-images.githubusercontent.com/3520243/236076489-a0196681-a98d-4d80-8539-ce45723606da.png)"
 long_description_content_type = text/markdown
 url = https://github.com/selmen2004/thonny-autosave
 project_urls = 
 	Bug Tracker = https://github.com/selmen2004/thonny-autosave/issues
 	Changelog = https://github.com/selmen2004/thonny-autosave/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
 	Intended Audience :: Developers
 
 [options]
+install_requires = 
+	thonny>=3.2.1
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.6
 
 [options.packages.find]
 where = src
```

### Comparing `thonny-autosave-0.0.6/src/thonny_autosave.egg-info/PKG-INFO` & `thonny-autosave-0.0.9/src/thonny_autosave.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: thonny-autosave
-Version: 0.0.6
+Version: 0.0.9
 Summary: Adds a checkbox to the File menu of Thonny editor, when activated , automatically saves current file every 10 seconds.
 Home-page: https://github.com/selmen2004/thonny-autosave
 Project-URL: Bug Tracker, https://github.com/selmen2004/thonny-autosave/issues
 Project-URL: Changelog, https://github.com/selmen2004/thonny-autosave/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-"# thonny-autosave
-Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds
+"# thonny-autosave\n
+Adds a checkbox to the File menu of Thonny editor, when activated , Automatically saves current file every 10 seconds\n
 ![image](https://user-images.githubusercontent.com/3520243/236076489-a0196681-a98d-4d80-8539-ce45723606da.png)"
```

### Comparing `thonny-autosave-0.0.6/src/thonnycontrib/thonny-autosave/app.py` & `thonny-autosave-0.0.9/src/thonnycontrib/thonny-autosave/app.py`

 * *Files identical despite different names*

