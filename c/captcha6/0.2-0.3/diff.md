# Comparing `tmp/captcha6-0.2.tar.gz` & `tmp/captcha6-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captcha6-0.2.tar", last modified: Sun May  7 18:35:21 2023, max compression
+gzip compressed data, was "captcha6-0.3.tar", last modified: Sun May  7 19:26:08 2023, max compression
```

## Comparing `captcha6-0.2.tar` & `captcha6-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 18:35:21.325533 captcha6-0.2/
--rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.2/LICENSE
--rw-rw-rw-   0        0        0     1332 2023-05-07 18:35:21.324534 captcha6-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-05-07 18:28:15.000000 captcha6-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 18:35:21.273530 captcha6-0.2/captcha6/
--rw-rw-rw-   0        0        0     1185 2023-05-07 18:34:49.000000 captcha6-0.2/captcha6/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-07 18:35:21.322533 captcha6-0.2/captcha6.egg-info/
--rw-rw-rw-   0        0        0     1332 2023-05-07 18:35:20.000000 captcha6-0.2/captcha6.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      206 2023-05-07 18:35:20.000000 captcha6-0.2/captcha6.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 18:35:20.000000 captcha6-0.2/captcha6.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-07 18:35:20.000000 captcha6-0.2/captcha6.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-07 18:35:20.000000 captcha6-0.2/captcha6.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 18:35:21.325533 captcha6-0.2/setup.cfg
--rw-rw-rw-   0        0        0      887 2023-05-07 18:35:11.000000 captcha6-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.199348 captcha6-0.3/
+-rw-rw-rw-   0        0        0       36 2023-04-01 18:28:23.000000 captcha6-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1341 2023-05-07 19:26:08.197348 captcha6-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      772 2023-05-07 19:25:47.000000 captcha6-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.130344 captcha6-0.3/captcha6/
+-rw-rw-rw-   0        0        0     1185 2023-05-07 18:34:49.000000 captcha6-0.3/captcha6/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 19:26:08.194347 captcha6-0.3/captcha6.egg-info/
+-rw-rw-rw-   0        0        0     1341 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      206 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 19:26:07.000000 captcha6-0.3/captcha6.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 19:26:08.200349 captcha6-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      887 2023-05-07 19:25:30.000000 captcha6-0.3/setup.py
```

### Comparing `captcha6-0.2/PKG-INFO` & `captcha6-0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.2
+Version: 0.3
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
     
-<h1 style="color:red; text-align: center;">captcha6</h1>
+<h1 style="color:red; text-align: center;">2captcha.io</h1>
 
 ## This library is for captcha solving
 
 ### Use this library like this
 
 ```python 
 from captcha6 import CAPTCHAv 
@@ -55,10 +55,10 @@
 
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
-#### Yusef
+#### 2captcha.io
```

### Comparing `captcha6-0.2/README.md` & `captcha6-0.3/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
     
-<h1 style="color:red; text-align: center;">captcha6</h1>
+<h1 style="color:red; text-align: center;">2captcha.io</h1>
 
 ## This library is for captcha solving
 
 ### Use this library like this
 
 ```python 
 from captcha6 import CAPTCHAv 
@@ -39,10 +39,10 @@
 
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
-#### Yusef
+#### 2captcha.io
```

### Comparing `captcha6-0.2/captcha6/__init__.py` & `captcha6-0.3/captcha6/__init__.py`

 * *Files identical despite different names*

### Comparing `captcha6-0.2/captcha6.egg-info/PKG-INFO` & `captcha6-0.3/captcha6.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captcha6
-Version: 0.2
+Version: 0.3
 Summary: Omar_Style _ 〄🇵🇸
 Home-page: https://github.com/Omarail1/omarpoop.git
 Author: omar Style
 Author-email: omarllStyle@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
     
-<h1 style="color:red; text-align: center;">captcha6</h1>
+<h1 style="color:red; text-align: center;">2captcha.io</h1>
 
 ## This library is for captcha solving
 
 ### Use this library like this
 
 ```python 
 from captcha6 import CAPTCHAv 
@@ -55,10 +55,10 @@
 
 
 ----
 ## From here register on the site
 [Link](https://2captcha.io/auth-sign-in.php)
 
 ### The developer of this library
-#### Yusef
+#### 2captcha.io
```

### Comparing `captcha6-0.2/setup.py` & `captcha6-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 # with open('requirements.txt','r') as fr:
 #     requires = fr.read().split('\n')
 
 setuptools.setup(
     name='captcha6',
-    version="0.2",
+    version="0.3",
     author='omar Style',
     author_email='omarllStyle@gmail.com',
     description='Omar_Style _ 〄🇵🇸',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Omarail1/omarpoop.git',
     packages=['captcha6'],
```

