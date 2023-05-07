# Comparing `tmp/zipline_norgatedata-2.4.0-py3-none-any.whl.zip` & `tmp/zipline_norgatedata-2.4.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 36244 bytes, number of entries: 11
+Zip file size: 36240 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat     9308 b- defN 23-May-01 01:30 zipline_norgatedata/CHANGES.txt
 -rw-rw-rw-  2.0 fat    16020 b- defN 20-Sep-09 09:35 zipline_norgatedata/LICENSE.txt
 -rw-rw-rw-  2.0 fat       62 b- defN 19-Aug-27 04:23 zipline_norgatedata/__init__.py
 -rw-rw-rw-  2.0 fat    10981 b- defN 23-May-01 11:22 zipline_norgatedata/pipelines.py
--rw-rw-rw-  2.0 fat       23 b- defN 23-May-01 01:29 zipline_norgatedata/version.py
+-rw-rw-rw-  2.0 fat       23 b- defN 23-May-07 10:02 zipline_norgatedata/version.py
 -rw-rw-rw-  2.0 fat    43970 b- defN 23-May-05 08:06 zipline_norgatedata/zipline_norgatedata.py
--rw-rw-rw-  2.0 fat    16020 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT
--rw-rw-rw-  2.0 fat    25842 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      990 b- defN 23-May-07 00:57 zipline_norgatedata-2.4.0.dist-info/RECORD
-11 files, 123328 bytes uncompressed, 34546 bytes compressed:  72.0%
+-rw-rw-rw-  2.0 fat    16020 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT
+-rw-rw-rw-  2.0 fat    25839 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      990 b- defN 23-May-07 10:03 zipline_norgatedata-2.4.1.dist-info/RECORD
+11 files, 123325 bytes uncompressed, 34542 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: zipline_norgatedata/version.py
 Comment: 
 
 Filename: zipline_norgatedata/zipline_norgatedata.py
 Comment: 
 
-Filename: zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT
+Filename: zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: zipline_norgatedata-2.4.0.dist-info/METADATA
+Filename: zipline_norgatedata-2.4.1.dist-info/METADATA
 Comment: 
 
-Filename: zipline_norgatedata-2.4.0.dist-info/WHEEL
+Filename: zipline_norgatedata-2.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: zipline_norgatedata-2.4.0.dist-info/top_level.txt
+Filename: zipline_norgatedata-2.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: zipline_norgatedata-2.4.0.dist-info/RECORD
+Filename: zipline_norgatedata-2.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## zipline_norgatedata/version.py

```diff
@@ -1 +1 @@
-__version__ = '2.4.0'
+__version__ = '2.4.1'
```

## Comparing `zipline_norgatedata-2.4.0.dist-info/LICENSE.TXT` & `zipline_norgatedata-2.4.1.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

## Comparing `zipline_norgatedata-2.4.0.dist-info/METADATA` & `zipline_norgatedata-2.4.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zipline-norgatedata
-Version: 2.4.0
+Version: 2.4.1
 Summary: Zipline extension to provide bundles of data from Norgate Data into the Zipline algorithmic trading library for the Python programming language
 Home-page: https://norgatedata.com
 Author: NorgateData Pty Ltd
 Author-email: support@norgatedata.com
 License: EULA
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Development Status :: 5 - Production/Stable
@@ -62,15 +62,15 @@
 
 Start an Anaconda (base) prompt, create an environment and install the appropriate versions of packages:
 
 ````
 conda create -y -n zip310 python=3.10
 conda activate zip310
 conda install -y -c conda-forge mamba
-mamba install -y -c conda-forge -c zipline-reloaded pyfolio-reloaded
+mamba install -y -c conda-forge zipline-reloaded pyfolio-reloaded
 mamba install -y -c conda-forge jupyter logbook
 pip install norgatedata zipline-norgatedata
 if not exist %HOMEPATH%\.zipline mkdir %HOMEPATH%\.zipline
 if not exist %HOMEPATH%\.zipline\extension.py copy /b NUL %HOMEPATH%\.zipline\extension.py
 ````
 
 Note:  Mamba is used to install zipline-reloaded, because the Conda package manager becomes confused with so many dependencies required.  Mamba is also about 10 times quicker than Conda.
```

