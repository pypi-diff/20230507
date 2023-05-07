# Comparing `tmp/cshelph-2.4.1.tar.gz` & `tmp/cshelph-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cshelph-2.4.1.tar", last modified: Sun May  7 17:15:59 2023, max compression
+gzip compressed data, was "cshelph-2.4.2.tar", last modified: Sun May  7 17:18:12 2023, max compression
```

## Comparing `cshelph-2.4.1.tar` & `cshelph-2.4.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:15:59.538681 cshelph-2.4.1/
--rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.4.1/LICENSE.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3067 2023-05-07 17:15:59.538546 cshelph-2.4.1/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)     2559 2023-05-06 18:41:33.000000 cshelph-2.4.1/README.md
-drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:15:59.538381 cshelph-2.4.1/cshelph.egg-info/
--rw-r--r--   0 nmthoma1   (503) staff       (20)     3067 2023-05-07 17:15:59.000000 cshelph-2.4.1/cshelph.egg-info/PKG-INFO
--rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-07 17:15:59.000000 cshelph-2.4.1/cshelph.egg-info/SOURCES.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-07 17:15:59.000000 cshelph-2.4.1/cshelph.egg-info/dependency_links.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-07 17:15:59.000000 cshelph-2.4.1/cshelph.egg-info/top_level.txt
--rw-r--r--   0 nmthoma1   (503) staff       (20)    18618 2023-05-06 15:38:00.000000 cshelph-2.4.1/cshelph.py
--rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-07 17:15:59.538723 cshelph-2.4.1/setup.cfg
--rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-07 17:15:18.000000 cshelph-2.4.1/setup.py
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:18:12.138103 cshelph-2.4.2/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    11358 2023-05-02 19:47:21.000000 cshelph-2.4.2/LICENSE.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-07 17:18:12.137965 cshelph-2.4.2/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     2564 2023-05-07 17:17:40.000000 cshelph-2.4.2/README.md
+drwxr-xr-x   0 nmthoma1   (503) staff       (20)        0 2023-05-07 17:18:12.137782 cshelph-2.4.2/cshelph.egg-info/
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     3072 2023-05-07 17:18:12.000000 cshelph-2.4.2/cshelph.egg-info/PKG-INFO
+-rw-r--r--   0 nmthoma1   (503) staff       (20)      165 2023-05-07 17:18:12.000000 cshelph-2.4.2/cshelph.egg-info/SOURCES.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        1 2023-05-07 17:18:12.000000 cshelph-2.4.2/cshelph.egg-info/dependency_links.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)        8 2023-05-07 17:18:12.000000 cshelph-2.4.2/cshelph.egg-info/top_level.txt
+-rw-r--r--   0 nmthoma1   (503) staff       (20)    18618 2023-05-06 15:38:00.000000 cshelph-2.4.2/cshelph.py
+-rw-r--r--   0 nmthoma1   (503) staff       (20)       38 2023-05-07 17:18:12.138143 cshelph-2.4.2/setup.cfg
+-rw-r--r--   0 nmthoma1   (503) staff       (20)     1669 2023-05-07 17:18:07.000000 cshelph-2.4.2/setup.py
```

### Comparing `cshelph-2.4.1/LICENSE.txt` & `cshelph-2.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cshelph-2.4.1/PKG-INFO` & `cshelph-2.4.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.4.1
+Version: 2.4.2
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -48,16 +48,16 @@
 ```
 ### Additional options can be specifed to customize runs and override defaults (which are based on some underlying assumptions) 
 
 ## FAQs
 
 ### **Why does C-SHELPh classify my water surface as bathy?**
 
-### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. These can be changed in the code.
+### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. Thresholds can be passed in as arguments.
 
 ### **Why isn't C-SHELPh detecting my bathy points**
 
-### C-SHELPh is classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
+### C-SHELPh classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
 
 ## Additional notes
 
 ### Note: The refraction correction currently uses photon level metrics (photon azimuth, photon elevation, satellite elev) to get an as accurate bathymetric model as possible. This requires some assuptions about the spacecraft orbit (its vertical movements are a constant rate thus linear interpolation holds true) and geometry and radius of the Earth. Ultimately, the advantages of increased precision of this implementation are believed to outweigh uncertainty introduced by the assumption. The refraction correction follows that outlined by the excellent Parrish et al., 2019 publication: https://www.mdpi.com/2072-4292/11/14/1634
```

### Comparing `cshelph-2.4.1/README.md` & `cshelph-2.4.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -33,16 +33,16 @@
 ```
 ### Additional options can be specifed to customize runs and override defaults (which are based on some underlying assumptions) 
 
 ## FAQs
 
 ### **Why does C-SHELPh classify my water surface as bathy?**
 
-### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. These can be changed in the code.
+### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. Thresholds can be passed in as arguments.
 
 ### **Why isn't C-SHELPh detecting my bathy points**
 
-### C-SHELPh is classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
+### C-SHELPh classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
 
 ## Additional notes
 
 ### Note: The refraction correction currently uses photon level metrics (photon azimuth, photon elevation, satellite elev) to get an as accurate bathymetric model as possible. This requires some assuptions about the spacecraft orbit (its vertical movements are a constant rate thus linear interpolation holds true) and geometry and radius of the Earth. Ultimately, the advantages of increased precision of this implementation are believed to outweigh uncertainty introduced by the assumption. The refraction correction follows that outlined by the excellent Parrish et al., 2019 publication: https://www.mdpi.com/2072-4292/11/14/1634
```

### Comparing `cshelph-2.4.1/cshelph.egg-info/PKG-INFO` & `cshelph-2.4.2/cshelph.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cshelph
-Version: 2.4.1
+Version: 2.4.2
 Summary: Classification of Sub-aquatic Height Extracted Photons
 Home-page: https://github.com/nmt28/C-SHELPh
 Author: Nathan Thomas and Brian Lee
 Author-email: nmthomas28@gmail.com
 License: LICENSE.txt
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -48,16 +48,16 @@
 ```
 ### Additional options can be specifed to customize runs and override defaults (which are based on some underlying assumptions) 
 
 ## FAQs
 
 ### **Why does C-SHELPh classify my water surface as bathy?**
 
-### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. These can be changed in the code.
+### C-SHELPh performs an orthometric correction that models the water surface at approximately 0m elevation in reference to the EGM2008 geoid. In some locations this is not true and so C-SHELPh gets confused and thresholds set in the code to help C-SHELPh find the water surface are not sufficient. Thresholds can be passed in as arguments.
 
 ### **Why isn't C-SHELPh detecting my bathy points**
 
-### C-SHELPh is classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
+### C-SHELPh classifies photons based on photon density. In cases where the noise is higher than the signal (e.g., a small quantity of steep/deep and/or turbid waters) C-SHELph struggles to perform well. Optimum conditions for C-SHELPh are clear shallow waters.
 
 ## Additional notes
 
 ### Note: The refraction correction currently uses photon level metrics (photon azimuth, photon elevation, satellite elev) to get an as accurate bathymetric model as possible. This requires some assuptions about the spacecraft orbit (its vertical movements are a constant rate thus linear interpolation holds true) and geometry and radius of the Earth. Ultimately, the advantages of increased precision of this implementation are believed to outweigh uncertainty introduced by the assumption. The refraction correction follows that outlined by the excellent Parrish et al., 2019 publication: https://www.mdpi.com/2072-4292/11/14/1634
```

### Comparing `cshelph-2.4.1/cshelph.py` & `cshelph-2.4.2/cshelph.py`

 * *Files identical despite different names*

### Comparing `cshelph-2.4.1/setup.py` & `cshelph-2.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,24 +23,24 @@
 #
 #
 # Purpose:  Installation of the C-SHELPh software
 #
 # Author: Nathan Thomas
 # Email: nmthomas28@gmail.com
 # Date: 05/05/2023
-# Version: 2.4.1
+# Version: 2.4.2
 #
 # History:
-# Version 2.4.1
+# Version 2.4.2
 
 from distutils.core import setup
 import os
 
 setup(name='cshelph',
-    version='2.4.1',
+    version='2.4.2',
     description='Classification of Sub-aquatic Height Extracted Photons',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Nathan Thomas and Brian Lee',
     author_email='nmthomas28@gmail.com',
     scripts=['cshelph.py'],
     package_dir={},
```

