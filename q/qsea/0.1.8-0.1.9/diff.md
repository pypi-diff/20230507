# Comparing `tmp/qsea-0.1.8.tar.gz` & `tmp/qsea-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\qsea-0.1.8.tar", last modified: Wed May  3 17:22:55 2023, max compression
+gzip compressed data, was "dist\qsea-0.1.9.tar", last modified: Wed May  3 17:30:23 2023, max compression
```

## Comparing `qsea-0.1.8.tar` & `qsea-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:22:55.680346 qsea-0.1.8/
--rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.8/LICENSE.txt
--rw-rw-rw-   0        0        0      606 2023-05-03 17:22:55.679346 qsea-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 17:22:55.659359 qsea-0.1.8/qsea/
--rw-rw-rw-   0        0        0    61145 2023-04-11 22:30:58.000000 qsea-0.1.8/qsea/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:22:55.678346 qsea-0.1.8/qsea.egg-info/
--rw-rw-rw-   0        0        0      606 2023-05-03 17:22:55.000000 qsea-0.1.8/qsea.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      186 2023-05-03 17:22:55.000000 qsea-0.1.8/qsea.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:22:55.000000 qsea-0.1.8/qsea.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-05-03 17:22:55.000000 qsea-0.1.8/qsea.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 17:22:55.000000 qsea-0.1.8/qsea.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 17:22:55.680346 qsea-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      856 2023-05-03 17:22:23.000000 qsea-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:30:23.980514 qsea-0.1.9/
+-rw-rw-rw-   0        0        0     1061 2023-01-13 17:31:55.000000 qsea-0.1.9/LICENSE.txt
+-rw-rw-rw-   0        0        0      606 2023-05-03 17:30:23.978436 qsea-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-01-13 17:37:30.000000 qsea-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 17:30:23.965444 qsea-0.1.9/qsea/
+-rw-rw-rw-   0        0        0    61156 2023-05-03 17:29:52.000000 qsea-0.1.9/qsea/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 17:30:23.977436 qsea-0.1.9/qsea.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-05-03 17:30:23.000000 qsea-0.1.9/qsea.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-05-03 17:30:23.000000 qsea-0.1.9/qsea.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 17:30:23.000000 qsea-0.1.9/qsea.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-03 17:30:23.000000 qsea-0.1.9/qsea.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-03 17:30:23.000000 qsea-0.1.9/qsea.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-03 17:30:23.980514 qsea-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      849 2023-05-03 17:30:04.000000 qsea-0.1.9/setup.py
```

### Comparing `qsea-0.1.8/LICENSE.txt` & `qsea-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qsea-0.1.8/PKG-INFO` & `qsea-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.8
+Version: 0.1.9
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.8/qsea/__init__.py` & `qsea-0.1.9/qsea/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # beta-версия к публикации
 
 import json
 import pandas as pd
 import datetime as dt
 import logging
 import websocket
+import ssl
 
 
 # In[78]:
 
 
 # version 0.1.12-04-23
```

### Comparing `qsea-0.1.8/qsea.egg-info/PKG-INFO` & `qsea-0.1.9/qsea.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsea
-Version: 0.1.8
+Version: 0.1.9
 Summary: Convenient way to work with Qlik Sense Engine API from Python
 Home-page: https://github.com/ncthuc/qsea
 Download-URL: https://pypi.org/project/qsea/
 Author: Lev Biriukov
 Author-email: lbiryukov@gmail.com
 License: MIT
 Keywords: QlikSense,Qlik
```

### Comparing `qsea-0.1.8/setup.py` & `qsea-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
 setup_args = dict(
     name='qsea',
-    version='0.1.8',
+    version='0.1.9',
     description='Convenient way to work with Qlik Sense Engine API from Python',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='Lev Biriukov',
     author_email='lbiryukov@gmail.com',
     keywords=['QlikSense', 'Qlik'],
     url='https://github.com/ncthuc/qsea',
     download_url='https://pypi.org/project/qsea/'
 )
 
-install_requires = ['pandas', 'datetime', 'websocket-client', 'ssl']
+install_requires = ['pandas', 'datetime', 'websocket-client']
 
 if __name__ == '__main__':
     setup(**setup_args, install_requires=install_requires)
```

