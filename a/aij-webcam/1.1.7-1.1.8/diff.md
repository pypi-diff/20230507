# Comparing `tmp/aij-webcam-1.1.7.tar.gz` & `tmp/aij-webcam-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.1.7.tar", last modified: Sun May  7 13:58:52 2023, max compression
+gzip compressed data, was "aij-webcam-1.1.8.tar", last modified: Sun May  7 14:03:22 2023, max compression
```

## Comparing `aij-webcam-1.1.7.tar` & `aij-webcam-1.1.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.7/README.md
--rw-rw-rw-   0        0        0     6416 2023-05-07 13:58:42.000000 aij-webcam-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      430 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/intro/
--rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-webcam-1.1.7/src/intro/__init__.py
--rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-webcam-1.1.7/src/intro/intro.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-webcam-1.1.7/src/news/__init__.py
--rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-webcam-1.1.7/src/news/core.py
--rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-webcam-1.1.7/src/news/thread.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/setup/
--rw-rw-rw-   0        0        0      988 2023-05-07 13:53:50.000000 aij-webcam-1.1.7/src/setup/__init__.py
--rw-rw-rw-   0        0        0     1983 2023-05-07 13:54:16.000000 aij-webcam-1.1.7/src/setup/install.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:58:54.000000 aij-webcam-1.1.7/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-webcam-1.1.7/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-07 14:03:24.000000 aij-webcam-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.8/README.md
+-rw-rw-rw-   0        0        0     6416 2023-05-07 14:03:12.000000 aij-webcam-1.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:03:24.000000 aij-webcam-1.1.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      430 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      175 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/intro/
+-rw-rw-rw-   0        0        0      440 2023-05-07 13:08:58.000000 aij-webcam-1.1.8/src/intro/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-05-07 13:07:50.000000 aij-webcam-1.1.8/src/intro/intro.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-07 13:07:50.000000 aij-webcam-1.1.8/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4492 2023-05-07 13:16:16.000000 aij-webcam-1.1.8/src/news/core.py
+-rw-rw-rw-   0        0        0     1407 2023-05-07 13:18:00.000000 aij-webcam-1.1.8/src/news/thread.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/setup/
+-rw-rw-rw-   0        0        0      961 2023-05-07 14:03:04.000000 aij-webcam-1.1.8/src/setup/__init__.py
+-rw-rw-rw-   0        0        0     1983 2023-05-07 13:54:16.000000 aij-webcam-1.1.8/src/setup/install.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:03:22.000000 aij-webcam-1.1.8/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-webcam-1.1.8/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.1.7/LICENSE.txt` & `aij-webcam-1.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/PKG-INFO` & `aij-webcam-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.7
+Version: 1.1.8
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.7/README.md` & `aij-webcam-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/pyproject.toml` & `aij-webcam-1.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.7"
+version = "1.1.8"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-webcam-1.1.7/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.1.8/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.7
+Version: 1.1.8
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.7/src/intro/intro.py` & `aij-webcam-1.1.8/src/intro/intro.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/src/news/__init__.py` & `aij-webcam-1.1.8/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/src/news/core.py` & `aij-webcam-1.1.8/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/src/news/thread.py` & `aij-webcam-1.1.8/src/news/thread.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/src/setup/__init__.py` & `aij-webcam-1.1.8/src/setup/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from setup.install import ErLangInstallerThread
-from setup.rabbitmq import RabbitMQInstallerThread
+from setup.install import ErLangInstallerThread, RabbitMQInstallerThread
 
 def main():
     """
     This method is the main method which will install all the dependencies required for the project.
     ERLang: It is a programming language used to build massively scalable soft real-time systems with requirements on high availability.
     RabbitMQ: It is an open-source message-broker software that originally implemented the Advanced Message Queuing Protocol and has since been extended with a plug-in architecture to support Streaming Text Oriented Messaging Protocol, MQ Telemetry Transport, and other protocols.
     """
```

### Comparing `aij-webcam-1.1.7/src/setup/install.py` & `aij-webcam-1.1.8/src/setup/install.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.7/src/webcam/__init__.py` & `aij-webcam-1.1.8/src/webcam/__init__.py`

 * *Files identical despite different names*

