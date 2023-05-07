# Comparing `tmp/cos_uploader-2.0.0a2.tar.gz` & `tmp/cos_uploader-2.0.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cos_uploader-2.0.0a2.tar", max compression
+gzip compressed data, was "cos_uploader-2.0.0a3.tar", max compression
```

## Comparing `cos_uploader-2.0.0a2.tar` & `cos_uploader-2.0.0a3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       15 2023-05-07 14:40:37.069441 cos_uploader-2.0.0a2/README.md
--rw-r--r--   0        0        0     4259 2023-05-07 15:47:35.650972 cos_uploader-2.0.0a2/cos_uploader/__init__.py
--rw-r--r--   0        0        0      716 2023-05-07 15:23:47.518741 cos_uploader-2.0.0a2/cos_uploader/common.py
--rw-r--r--   0        0        0      631 2023-05-07 14:43:29.630252 cos_uploader-2.0.0a2/cos_uploader/config.toml
--rw-r--r--   0        0        0     2052 2023-05-07 15:25:57.984080 cos_uploader-2.0.0a2/cos_uploader/history.py
--rw-r--r--   0        0        0     1192 2023-05-07 15:48:09.394167 cos_uploader-2.0.0a2/cos_uploader/install.py
--rw-r--r--   0        0        0      618 2023-05-07 15:48:13.584301 cos_uploader-2.0.0a2/pyproject.toml
--rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cos_uploader-2.0.0a2/PKG-INFO
+-rw-r--r--   0        0        0       15 2023-05-07 14:40:37.069441 cos_uploader-2.0.0a3/README.md
+-rw-r--r--   0        0        0     4604 2023-05-07 16:05:21.427269 cos_uploader-2.0.0a3/cos_uploader/__init__.py
+-rw-r--r--   0        0        0      716 2023-05-07 15:23:47.518741 cos_uploader-2.0.0a3/cos_uploader/common.py
+-rw-r--r--   0        0        0      631 2023-05-07 14:43:29.630252 cos_uploader-2.0.0a3/cos_uploader/config.toml
+-rw-r--r--   0        0        0     2052 2023-05-07 15:25:57.984080 cos_uploader-2.0.0a3/cos_uploader/history.py
+-rw-r--r--   0        0        0     1237 2023-05-07 15:55:54.170237 cos_uploader-2.0.0a3/cos_uploader/install.py
+-rw-r--r--   0        0        0      618 2023-05-07 16:05:57.906519 cos_uploader-2.0.0a3/pyproject.toml
+-rw-r--r--   0        0        0      639 1970-01-01 00:00:00.000000 cos_uploader-2.0.0a3/PKG-INFO
```

### Comparing `cos_uploader-2.0.0a2/cos_uploader/__init__.py` & `cos_uploader-2.0.0a3/cos_uploader/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import sys
 import uuid
 import time
 import json
 import argparse
 import datetime
+import traceback
 import urllib.parse
 from qcloud_cos import CosConfig
 from qcloud_cos import CosS3Client
 from cos_uploader.common import load_config
 
 
 def progress_callback(consumed_bytes, total_bytes):
@@ -104,16 +105,24 @@
         hf.write(json.dumps(history, ensure_ascii=False) + "\n")
 
 
 def main():
     parser = argparse.ArgumentParser(description='Upload files to Tencent Cloud COS')
     parser.add_argument("files", metavar="FILE", type=str, nargs="+")
     parser.add_argument("--typora", dest="typora", action="store_true")
+    parser.add_argument("--windows-sendto", dest="windows_sendto", action="store_true")
     args = parser.parse_args()
 
     config = load_config()    
     for file in args.files:
-        upload_to_cos(file, config, args.typora)
+        try:
+            upload_to_cos(file, config, args.typora)
+        except Exception as e:
+            print(f"ERROR: {e}", file=sys.stderr)
+            traceback.print_exc()
+            continue
+    if args.windows_sendto:
+        input("Done! Press Enter to close this window...")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cos_uploader-2.0.0a2/cos_uploader/common.py` & `cos_uploader-2.0.0a3/cos_uploader/common.py`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0a2/cos_uploader/config.toml` & `cos_uploader-2.0.0a3/cos_uploader/config.toml`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0a2/cos_uploader/history.py` & `cos_uploader-2.0.0a3/cos_uploader/history.py`

 * *Files identical despite different names*

### Comparing `cos_uploader-2.0.0a2/cos_uploader/install.py` & `cos_uploader-2.0.0a3/cos_uploader/install.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 
 def install_windiws_shortcut():
     binary_path = os.path.join(os.path.dirname(sys.argv[0]), "cos-uploader.exe")
     script = f"""
     $shortcut = (New-Object -COM WScript.Shell).CreateShortcut("$($env:APPDATA)\Microsoft\Windows\SendTo\COS Uploader.lnk")
     $shortcut.TargetPath = "{binary_path}"
+    $shortcut.Arguments = "--windows-sendto"
     $shortcut.Save()
     """
     import subprocess
     result = subprocess.run(["powershell", script], capture_output=True, text=True)
     print(result.stdout)
     print(result.stderr)
     print("Installed COS Uploader to SendTo menu")
```

### Comparing `cos_uploader-2.0.0a2/pyproject.toml` & `cos_uploader-2.0.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cos-uploader"
-version = "2.0.0-alpha.2"
+version = "2.0.0-alpha.3"
 description = "Upload files to Tencent COS"
 authors = ["Joseph Chris <joseph@josephcz.xyz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "cos_uploader"}]
 include = ["LICENSE", "cos_uploader/config.toml"]
```

### Comparing `cos_uploader-2.0.0a2/PKG-INFO` & `cos_uploader-2.0.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cos-uploader
-Version: 2.0.0a2
+Version: 2.0.0a3
 Summary: Upload files to Tencent COS
 License: MIT
 Author: Joseph Chris
 Author-email: joseph@josephcz.xyz
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

