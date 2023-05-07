# Comparing `tmp/VoiceIdentification-1.5.tar.gz` & `tmp/VoiceIdentification-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoiceIdentification-1.5.tar", last modified: Sat May  6 17:30:48 2023, max compression
+gzip compressed data, was "VoiceIdentification-1.6.tar", last modified: Sat May  6 18:46:36 2023, max compression
```

## Comparing `VoiceIdentification-1.5.tar` & `VoiceIdentification-1.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/
--rw-rw-rw-   0        0        0    15395 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/PKG-INFO
--rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.085768 VoiceIdentification-1.5/VoiceIdentification.egg-info/
--rw-rw-rw-   0        0        0    15395 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      285 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-06 17:30:48.000000 VoiceIdentification-1.5/VoiceIdentification.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/setup.cfg
--rw-rw-rw-   0        0        0     2897 2023-05-06 17:29:26.000000 VoiceIdentification-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-06 17:30:48.101394 VoiceIdentification-1.5/voice_identification/
--rw-rw-rw-   0        0        0      101 2023-05-06 17:28:21.000000 VoiceIdentification-1.5/voice_identification/__init___.py
--rw-rw-rw-   0        0        0      313 2023-05-06 17:23:40.000000 VoiceIdentification-1.5/voice_identification/create.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:46:36.720358 VoiceIdentification-1.6/
+-rw-rw-rw-   0        0        0    15395 2023-05-06 18:46:36.720358 VoiceIdentification-1.6/PKG-INFO
+-rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 18:46:36.720358 VoiceIdentification-1.6/VoiceIdentification.egg-info/
+-rw-rw-rw-   0        0        0    15395 2023-05-06 18:46:36.000000 VoiceIdentification-1.6/VoiceIdentification.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-06 18:46:36.000000 VoiceIdentification-1.6/VoiceIdentification.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:46:36.000000 VoiceIdentification-1.6/VoiceIdentification.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      285 2023-05-06 18:46:36.000000 VoiceIdentification-1.6/VoiceIdentification.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-06 18:46:36.000000 VoiceIdentification-1.6/VoiceIdentification.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-06 18:46:36.720358 VoiceIdentification-1.6/setup.cfg
+-rw-rw-rw-   0        0        0     2897 2023-05-06 18:45:56.000000 VoiceIdentification-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:46:36.720358 VoiceIdentification-1.6/voice_identification/
+-rw-rw-rw-   0        0        0      101 2023-05-06 18:45:56.000000 VoiceIdentification-1.6/voice_identification/__init___.py
+-rw-rw-rw-   0        0        0      509 2023-05-06 18:44:23.000000 VoiceIdentification-1.6/voice_identification/create.py
```

### Comparing `VoiceIdentification-1.5/PKG-INFO` & `VoiceIdentification-1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.5
+Version: 1.6
 Summary: A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. 
 Home-page: https://github.com/SriBalajiSMVEC/voice_identification
 Author: BalajiSanthanam
 Author-email: sribalaji2112@gmail.com
 License: BSD 3-Clause License
 Keywords: biometric speaker recognition voice sphinx google wit bing api houndify ibm snowboy voice print identification security
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.5 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.6 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.5/README.md` & `VoiceIdentification-1.6/README.md`

 * *Files identical despite different names*

### Comparing `VoiceIdentification-1.5/VoiceIdentification.egg-info/PKG-INFO` & `VoiceIdentification-1.6/VoiceIdentification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.5
+Version: 1.6
 Summary: A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. 
 Home-page: https://github.com/SriBalajiSMVEC/voice_identification
 Author: BalajiSanthanam
 Author-email: sribalaji2112@gmail.com
 License: BSD 3-Clause License
 Keywords: biometric speaker recognition voice sphinx google wit bing api houndify ibm snowboy voice print identification security
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.5 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.6 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.5/setup.py` & `VoiceIdentification-1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Use the README.md content for the long description:
 with io.open("README.md", encoding="utf-8") as fileObj:
     long_description = fileObj.read()
 
 setup(
     name='VoiceIdentification',
-    version=1.5,
+    version=1.6,
     url='https://github.com/SriBalajiSMVEC/voice_identification',
     author='BalajiSanthanam',
     author_email='sribalaji2112@gmail.com',
     description=('A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. '),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='BSD 3-Clause License',
```

