# Comparing `tmp/pylovelace-2023.1.5-py3-none-any.whl.zip` & `tmp/pylovelace-2023.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 18008 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat      228 b- defN 23-Apr-20 02:18 pylovelace/__init__.py
+Zip file size: 18072 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat      228 b- defN 23-May-07 16:52 pylovelace/__init__.py
 -rw-rw-rw-  2.0 fat     8086 b- defN 23-Apr-19 05:09 pylovelace/__main__.py
--rw-rw-rw-  2.0 fat     4383 b- defN 23-Apr-19 05:09 pylovelace/protect.py
--rw-rw-rw-  2.0 fat    35149 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1743 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       56 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat       11 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      753 b- defN 23-Apr-20 02:19 pylovelace-2023.1.5.dist-info/RECORD
-9 files, 50501 bytes uncompressed, 16702 bytes compressed:  66.9%
+-rw-rw-rw-  2.0 fat     4552 b- defN 23-May-07 16:51 pylovelace/protect.py
+-rw-rw-rw-  2.0 fat    35149 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1805 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       56 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat       11 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      753 b- defN 23-May-07 16:53 pylovelace-2023.2.0.dist-info/RECORD
+9 files, 50732 bytes uncompressed, 16766 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: pylovelace/__main__.py
 Comment: 
 
 Filename: pylovelace/protect.py
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/LICENSE
+Filename: pylovelace-2023.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/METADATA
+Filename: pylovelace-2023.2.0.dist-info/METADATA
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/WHEEL
+Filename: pylovelace-2023.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/entry_points.txt
+Filename: pylovelace-2023.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/top_level.txt
+Filename: pylovelace-2023.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pylovelace-2023.1.5.dist-info/RECORD
+Filename: pylovelace-2023.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pylovelace/__init__.py

```diff
@@ -4,9 +4,9 @@
 Copyright (c) 2023 PyLovelace
 All rights reserved.
 
 @Author: nshout
 @File: __init__.py
 """
 
-__version__ = "2023.1.5"
+__version__ = "2023.2.0"
 __description__ = "Python code protection/obfuscation tool"
```

## pylovelace/protect.py

```diff
@@ -6,14 +6,15 @@
 
 @Author: nshout
 @File: protect.py
 """
 import logging
 import os
 import shutil
+import platform
 
 from .kernel import PyLovelace, get_runtime_module, protect_code, compile_module, finalize
 
 logging.basicConfig(
     level=logging.DEBUG,
     format='%(levelname)s - %(message)s'
 )
@@ -128,15 +129,19 @@
             compile_module(output_file)
             logging.info("compiled file: " + os.path.basename(self.file))
 
         if not os.path.exists(os.path.join(output_dir, "pylovelace_runtime")):
             os.makedirs(os.path.join(output_dir, "pylovelace_runtime"), exist_ok=True)
 
         runtime_folder = os.path.join(output_dir, "pylovelace_runtime")
-        get_runtime_module(os.path.join(runtime_folder, "pylovelace_runtime.pyd"))
+
+        if platform.system() == 'Windows':
+            get_runtime_module(os.path.join(runtime_folder, "pylovelace_runtime.pyd"))
+        else:
+            get_runtime_module(os.path.join(runtime_folder, "pylovelace_runtime.so"))
 
         with open(os.path.join(runtime_folder, "__init__.py"), "w") as f:
             f.write('''"""
 pyintellect_runtime
 """
 from .pylovelace_runtime import __ada__, __lovelace__''')
```

## Comparing `pylovelace-2023.1.5.dist-info/LICENSE` & `pylovelace-2023.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pylovelace-2023.1.5.dist-info/METADATA` & `pylovelace-2023.2.0.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: pylovelace
-Version: 2023.1.5
+Version: 2023.2.0
 Summary: Python code protection/obfuscation tool
 Home-page: https://github.com/pylovelace/pylovelace
 Author: nshout
 Keywords: obfuscate obfuscation distribute production tool
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: Topic :: Security
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.10, <3.13
 License-File: LICENSE
-Requires-Dist: pylovelace.kernel (>2023.1.4)
+Requires-Dist: pylovelace.kernel (>=2023.2.0)
 
 PyLovelace Python protection tool.
 ===================================
 
 PyLovelace is a Python protection tool that can be used to protect
 Python source code from being reverse engineered.
```

