# Comparing `tmp/piwwwaterflow-0.0.5.tar.gz` & `tmp/piwwwaterflow-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwwwaterflow-0.0.5.tar", last modified: Sat Jan 23 15:49:09 2021, max compression
+gzip compressed data, was "piwwwaterflow-0.1.1.tar", last modified: Sun May  7 09:07:56 2023, max compression
```

## Comparing `piwwwaterflow-0.0.5.tar` & `piwwwaterflow-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,17 @@
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.857093 piwwwaterflow-0.0.5/
--rw-rw-rw-   0        0        0       23 2021-01-23 15:46:51.000000 piwwwaterflow-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      601 2021-01-23 15:49:09.856094 piwwwaterflow-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       67 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.827094 piwwwaterflow-0.0.5/piwwwaterflow/
--rw-rw-rw-   0        0        0       25 2021-01-23 10:43:11.000000 piwwwaterflow-0.0.5/piwwwaterflow/__init__.py
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.816093 piwwwaterflow-0.0.5/piwwwaterflow/static/
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.839094 piwwwaterflow-0.0.5/piwwwaterflow/static/css/
--rw-rw-rw-   0        0        0     1804 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/css/iepngfix.htc
--rw-rw-rw-   0        0        0     7838 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/css/view.css
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.851095 piwwwaterflow-0.0.5/piwwwaterflow/static/img/
--rw-rw-rw-   0        0        0       49 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/blank.gif
--rw-rw-rw-   0        0        0      431 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/bottom.png
--rw-rw-rw-   0        0        0    33683 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/icon-256.png
--rw-rw-rw-   0        0        0     2373 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/icon-32.png
--rw-rw-rw-   0        0        0      762 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/play.png
--rw-rw-rw-   0        0        0       46 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/shadow.gif
--rw-rw-rw-   0        0        0      417 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/img/top.png
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.852094 piwwwaterflow-0.0.5/piwwwaterflow/static/js/
--rw-rw-rw-   0        0        0     2598 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/static/js/code.js
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.854095 piwwwaterflow-0.0.5/piwwwaterflow/templates/
--rw-rw-rw-   0        0        0     3894 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/templates/form.html
--rw-rw-rw-   0        0        0     6252 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/webservice.py
--rw-rw-rw-   0        0        0       73 2021-01-22 16:33:57.000000 piwwwaterflow-0.0.5/piwwwaterflow/wsgi.py
-drwxrwxrwx   0        0        0        0 2021-01-23 15:49:09.836094 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/
--rw-rw-rw-   0        0        0      601 2021-01-23 15:49:09.000000 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      677 2021-01-23 15:49:09.000000 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-01-23 15:49:09.000000 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2021-01-23 15:49:09.000000 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2021-01-23 15:49:09.000000 piwwwaterflow-0.0.5/piwwwaterflow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-01-23 15:49:09.857093 piwwwaterflow-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      848 2021-01-23 15:49:03.000000 piwwwaterflow-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:07:56.753506 piwwwaterflow-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-07 09:07:56.753506 piwwwaterflow-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:07:56.749506 piwwwaterflow-0.1.1/piwwwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/piwwwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/piwwwaterflow/webservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/piwwwaterflow/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:07:56.753506 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-07 09:07:56.000000 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-07 09:07:56.000000 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 09:07:56.000000 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-07 09:07:56.000000 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 09:07:56.000000 piwwwaterflow-0.1.1/piwwwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 09:07:56.753506 piwwwaterflow-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 09:07:56.753506 piwwwaterflow-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 09:07:45.000000 piwwwaterflow-0.1.1/tests/__init__.py
```

### Comparing `piwwwaterflow-0.0.5/PKG-INFO` & `piwwwaterflow-0.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-Metadata-Version: 2.1
-Name: piwwwaterflow
-Version: 0.0.5
-Summary: Raspberry Pi Waterflow Web interface
-Home-page: https://github.com/Phornee/piwwwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # piwwwaterflow
-        Flask/Gunicorn Webservice for piwaterflow system
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwwwaterflow
+Version: 0.1.1
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwwwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # piwwwaterflow
+        Flask/Gunicorn Webservice for piwaterflow system
+        
+        + 1.1.0
+          + Avoid service caching by adding timestamp to URL
+        + 1.1.1
+          + Point to new grafana 
+        + 1.2.2
+          + New waterflow config & LAN influxdb
+        + 1.2.3
+          + Black header & config fix
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `piwwwaterflow-0.0.5/piwwwaterflow.egg-info/PKG-INFO` & `piwwwaterflow-0.1.1/piwwwaterflow.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,27 @@
-Metadata-Version: 2.1
-Name: piwwwaterflow
-Version: 0.0.5
-Summary: Raspberry Pi Waterflow Web interface
-Home-page: https://github.com/Phornee/piwwwaterflow
-Author: Ismael Raya
-Author-email: phornee@gmail.com
-License: UNKNOWN
-Description: # piwwwaterflow
-        Flask/Gunicorn Webservice for piwaterflow system
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Topic :: Home Automation
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: piwwwaterflow
+Version: 0.1.1
+Summary: Raspberry Pi Waterflow resilient system
+Home-page: https://github.com/Phornee/piwwwaterflow
+Author: Ismael Raya
+Author-email: phornee@gmail.com
+License: UNKNOWN
+Description: # piwwwaterflow
+        Flask/Gunicorn Webservice for piwaterflow system
+        
+        + 1.1.0
+          + Avoid service caching by adding timestamp to URL
+        + 1.1.1
+          + Point to new grafana 
+        + 1.2.2
+          + New waterflow config & LAN influxdb
+        + 1.2.3
+          + Black header & config fix
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Home Automation
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
```

### Comparing `piwwwaterflow-0.0.5/setup.py` & `piwwwaterflow-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-import setuptools
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="piwwwaterflow",
-    version="0.0.5",
-    author="Ismael Raya",
-    author_email="phornee@gmail.com",
-    description="Raspberry Pi Waterflow Web interface",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/Phornee/piwwwaterflow",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: POSIX :: Linux",
-        "Topic :: Home Automation"
-    ],
-    install_requires=[
-        'piwaterflow>=0.0.5',
-        'Flask>=1.1.2'
-    ],
-    python_requires='>=3.6',
+""" Pypi stup """
+import setuptools
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="piwwwaterflow",
+    version="0.1.1",
+    author="Ismael Raya",
+    author_email="phornee@gmail.com",
+    description="Raspberry Pi Waterflow resilient system",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/Phornee/piwwwaterflow",
+    packages=setuptools.find_packages(),
+    package_data={
+        '': ['*.yml'],
+    },
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Topic :: Home Automation",
+    ],
+    install_requires=[
+        'Flask>=1.1.2',
+        'flask-compress>=1.9.0',
+        'importlib-metadata>=4.5.0',
+        'python-socketio>=5.8.0',
+        'flask-socketio>=5.3.3',
+        'eventlet>=0.33.3',
+        'piwaterflow>=0.5.2'
+    ],
+    python_requires='>=3.6',
 )
```

