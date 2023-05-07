# Comparing `tmp/VoiceIdentification-1.7.tar.gz` & `tmp/VoiceIdentification-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VoiceIdentification-1.7.tar", last modified: Sun May  7 14:35:01 2023, max compression
+gzip compressed data, was "VoiceIdentification-1.8.tar", last modified: Sun May  7 15:40:34 2023, max compression
```

## Comparing `VoiceIdentification-1.7.tar` & `VoiceIdentification-1.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 14:35:01.693594 VoiceIdentification-1.7/
--rw-rw-rw-   0        0        0    15395 2023-05-07 14:35:01.693594 VoiceIdentification-1.7/PKG-INFO
--rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 14:35:01.693594 VoiceIdentification-1.7/VoiceIdentification.egg-info/
--rw-rw-rw-   0        0        0    15395 2023-05-07 14:35:01.000000 VoiceIdentification-1.7/VoiceIdentification.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-07 14:35:01.000000 VoiceIdentification-1.7/VoiceIdentification.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 14:35:01.000000 VoiceIdentification-1.7/VoiceIdentification.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      285 2023-05-07 14:35:01.000000 VoiceIdentification-1.7/VoiceIdentification.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-07 14:35:01.000000 VoiceIdentification-1.7/VoiceIdentification.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 14:35:01.693594 VoiceIdentification-1.7/setup.cfg
--rw-rw-rw-   0        0        0     2897 2023-05-07 14:34:22.000000 VoiceIdentification-1.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 14:35:01.693594 VoiceIdentification-1.7/voice_identification/
--rw-rw-rw-   0        0        0      101 2023-05-07 14:34:22.000000 VoiceIdentification-1.7/voice_identification/__init___.py
--rw-rw-rw-   0        0        0     1844 2023-05-07 14:34:22.000000 VoiceIdentification-1.7/voice_identification/create.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:40:34.487017 VoiceIdentification-1.8/
+-rw-rw-rw-   0        0        0    15395 2023-05-07 15:40:34.487017 VoiceIdentification-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0    13729 2023-04-23 17:04:02.000000 VoiceIdentification-1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 15:40:34.487017 VoiceIdentification-1.8/VoiceIdentification.egg-info/
+-rw-rw-rw-   0        0        0    15395 2023-05-07 15:40:34.000000 VoiceIdentification-1.8/VoiceIdentification.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-07 15:40:34.000000 VoiceIdentification-1.8/VoiceIdentification.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 15:40:34.000000 VoiceIdentification-1.8/VoiceIdentification.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      285 2023-05-07 15:40:34.000000 VoiceIdentification-1.8/VoiceIdentification.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-07 15:40:34.000000 VoiceIdentification-1.8/VoiceIdentification.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 15:40:34.487017 VoiceIdentification-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     2897 2023-05-07 15:40:19.000000 VoiceIdentification-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 15:40:34.487017 VoiceIdentification-1.8/voice_identification/
+-rw-rw-rw-   0        0        0      101 2023-05-07 15:37:23.000000 VoiceIdentification-1.8/voice_identification/__init___.py
+-rw-rw-rw-   0        0        0     1800 2023-05-07 15:35:42.000000 VoiceIdentification-1.8/voice_identification/create.py
```

### Comparing `VoiceIdentification-1.7/PKG-INFO` & `VoiceIdentification-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.7
+Version: 1.8
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
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.7 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.8 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.7/README.md` & `VoiceIdentification-1.8/README.md`

 * *Files identical despite different names*

### Comparing `VoiceIdentification-1.7/VoiceIdentification.egg-info/PKG-INFO` & `VoiceIdentification-1.8/VoiceIdentification.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VoiceIdentification
-Version: 1.7
+Version: 1.8
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
-Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.7 Summary: A
+Metadata-Version: 2.1 Name: VoiceIdentification Version: 1.8 Summary: A
 Voice_Identification (speaker recognition) library that works both online and
 offline and supports a number of engines and APIs. Home-page: https://
 github.com/SriBalajiSMVEC/voice_identification Author: BalajiSanthanam Author-
 email: sribalaji2112@gmail.com License: BSD 3-Clause License Keywords:
 biometric speaker recognition voice sphinx google wit bing api houndify ibm
 snowboy voice print identification security Classifier: Development Status :: 4
 - Beta Classifier: Environment :: Win32 (MS Windows) Classifier: Environment ::
```

### Comparing `VoiceIdentification-1.7/setup.py` & `VoiceIdentification-1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 # Use the README.md content for the long description:
 with io.open("README.md", encoding="utf-8") as fileObj:
     long_description = fileObj.read()
 
 setup(
     name='VoiceIdentification',
-    version=1.7,
+    version=1.8,
     url='https://github.com/SriBalajiSMVEC/voice_identification',
     author='BalajiSanthanam',
     author_email='sribalaji2112@gmail.com',
     description=('A Voice_Identification (speaker recognition) library that works both online and offline and supports a number of engines and APIs. '),
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='BSD 3-Clause License',
```

### Comparing `VoiceIdentification-1.7/voice_identification/create.py` & `VoiceIdentification-1.8/voice_identification/create.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 from git.repo.base import Repo
 import requests
 
 directory_to_project = dir_path = os.path.dirname(os.path.realpath(__file__)) + "\\VI"
 def create():
     if not os.path.exists(dir_path):
-        print("VI Module has Downloading")
-        Repo.clone_from("https://github.com/SriBalaji2112/pypi_voice_identification_downloader", dir_path)
 
         def download_file_from_google_drive(id, destination):
             URL = "https://docs.google.com/uc?export=download"
 
             session = requests.Session()
 
             response = session.get(URL, params={'id': id}, stream=True)
@@ -32,16 +30,19 @@
         def save_response_content(response, destination):
             CHUNK_SIZE = 32768
 
             with open(destination, "wb") as f:
                 for chunk in response.iter_content(CHUNK_SIZE):
                     if chunk:  # filter out keep-alive new chunks
                         f.write(chunk)
+        print("VI Module has Downloading")
+        Repo.clone_from("https://github.com/SriBalaji2112/pypi_voice_identification_downloader", dir_path)
+        file_id = '1LH2wmN5E_qTQrxzdVvGgBK9W_XBSJzV4'
+        destination = dir_path + '\\model\\saved_model\\variables\\variables.data-00000-of-00001'
+        download_file_from_google_drive(file_id, destination)
+        print("Download Finished please Remove create() function")
 
-        if __name__ == "__main__":
-            file_id = '1LH2wmN5E_qTQrxzdVvGgBK9W_XBSJzV4'
-            destination = dir_path + 'VI\\model\\saved_model\\variables\\variables.data-00000-of-00001'
-            download_file_from_google_drive(file_id, destination)
-            print("Download Finished please Remove create() function")
     else:
         print("VI was already downloaded")
         print("Please Remove create() function")
+
+create()
```

