# Comparing `tmp/ecida-0.0.3.tar.gz` & `tmp/ecida-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecida-0.0.3.tar", last modified: Thu May  4 14:36:19 2023, max compression
+gzip compressed data, was "ecida-0.0.4.tar", last modified: Sun May  7 17:18:16 2023, max compression
```

## Comparing `ecida-0.0.3.tar` & `ecida-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-04 14:36:19.913546 ecida-0.0.3/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4773 2023-05-04 14:35:17.000000 ecida-0.0.3/Ecida.py
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-04 14:36:19.913546 ecida-0.0.3/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-03-09 17:51:25.000000 ecida-0.0.3/README.md
-drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-04 14:36:19.913546 ecida-0.0.3/ecida.egg-info/
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/PKG-INFO
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/SOURCES.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/dependency_links.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/requires.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-04 14:36:19.000000 ecida-0.0.3/ecida.egg-info/top_level.txt
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-04 14:36:19.913546 ecida-0.0.3/setup.cfg
--rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-04 14:35:24.000000 ecida-0.0.3/setup.py
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-07 17:18:16.388783 ecida-0.0.4/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)     4789 2023-05-07 17:17:33.000000 ecida-0.0.4/Ecida.py
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-07 17:18:16.388783 ecida-0.0.4/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      179 2023-03-09 17:51:25.000000 ecida-0.0.4/README.md
+drwxrwxr-x   0 mostafa   (1000) mostafa   (1000)        0 2023-05-07 17:18:16.388783 ecida-0.0.4/ecida.egg-info/
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      557 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/PKG-INFO
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      171 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/SOURCES.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/dependency_links.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       13 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/requires.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)        1 2023-05-07 17:18:16.000000 ecida-0.0.4/ecida.egg-info/top_level.txt
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)       38 2023-05-07 17:18:16.388783 ecida-0.0.4/setup.cfg
+-rw-rw-r--   0 mostafa   (1000) mostafa   (1000)      639 2023-05-07 17:17:57.000000 ecida-0.0.4/setup.py
```

### Comparing `ecida-0.0.3/Ecida.py` & `ecida-0.0.4/Ecida.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,9 +131,9 @@
             self._producer.send(self._topics_names[output], value= str(message).encode("utf-8"))
             return True
         return False
     
     def pull(self, input: str) -> any:
         if input in self._inputs:
             for msg in self._consumers[input]:
-                return msg.value
+                return msg.value.decode("utf-8")
         return None
```

### Comparing `ecida-0.0.3/PKG-INFO` & `ecida-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.3
+Version: 0.0.4
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.3/ecida.egg-info/PKG-INFO` & `ecida-0.0.4/ecida.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecida
-Version: 0.0.3
+Version: 0.0.4
 Summary: The ECiDA-python to make things easier
 Home-page: https://gitlab.com/ecida
 Author: Mostafa Hadadian
 Author-email: m.hadadian@rug.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ecida-0.0.3/setup.py` & `ecida-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r") as fh:
    long_description = fh.read()
    
 setuptools.setup(
    name='ecida',
-   version='0.0.3',
+   version='0.0.4',
    author="Mostafa Hadadian",
    author_email="m.hadadian@rug.nl",
    description="The ECiDA-python to make things easier",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://gitlab.com/ecida",
    packages=["."] or setuptools.find_packages(),
```

