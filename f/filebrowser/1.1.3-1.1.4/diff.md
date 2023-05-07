# Comparing `tmp/filebrowser-1.1.3-py3-none-any.whl.zip` & `tmp/filebrowser-1.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 95035 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 22-May-12 10:44 filebrowser/__init__.py
--rw-r--r--  2.0 unx     8238 b- defN 22-Jul-12 13:18 filebrowser/app.py
+Zip file size: 95043 bytes, number of entries: 17
+-rw-r--r--  2.0 unx       21 b- defN 23-May-07 15:11 filebrowser/__init__.py
+-rw-r--r--  2.0 unx     8230 b- defN 23-May-07 15:01 filebrowser/app.py
 -rw-r--r--  2.0 unx     1529 b- defN 22-Jul-14 01:23 filebrowser/funcs.py
--rw-r--r--  2.0 unx     1465 b- defN 22-Jul-14 01:23 filebrowser/main.py
+-rw-r--r--  2.0 unx     1443 b- defN 23-May-07 15:11 filebrowser/main.py
 -rw-r--r--  2.0 unx    22591 b- defN 22-Jun-12 07:30 filebrowser/static/css/file.css
 -rw-r--r--  2.0 unx     3322 b- defN 22-Jun-12 07:37 filebrowser/static/css/file1.css
 -rw-r--r--  2.0 unx    44300 b- defN 22-May-12 10:44 filebrowser/static/fonts/MaterialIcons-Regular.570eb838.woff2
 -rwxr-xr-x  2.0 unx    89476 b- defN 22-May-12 10:44 filebrowser/static/js/jquery.min.js
 -rw-r--r--  2.0 unx    19702 b- defN 22-Jul-09 07:59 filebrowser/static/js/main.js
 -rw-r--r--  2.0 unx     1249 b- defN 22-May-12 11:38 filebrowser/templates/data.html
 -rw-r--r--  2.0 unx    16123 b- defN 22-Jul-06 04:11 filebrowser/templates/index.html
--rw-r--r--  2.0 unx     1075 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1630 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       53 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       12 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1465 b- defN 22-Jul-14 01:25 filebrowser-1.1.3.dist-info/RECORD
-17 files, 212322 bytes uncompressed, 92613 bytes compressed:  56.4%
+-rw-r--r--  2.0 unx     1075 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1621 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       12 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1466 b- defN 23-May-07 15:12 filebrowser-1.1.4.dist-info/RECORD
+17 files, 212306 bytes uncompressed, 92621 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: filebrowser/templates/data.html
 Comment: 
 
 Filename: filebrowser/templates/index.html
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/LICENSE
+Filename: filebrowser-1.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/METADATA
+Filename: filebrowser-1.1.4.dist-info/METADATA
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/WHEEL
+Filename: filebrowser-1.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/entry_points.txt
+Filename: filebrowser-1.1.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/top_level.txt
+Filename: filebrowser-1.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: filebrowser-1.1.3.dist-info/RECORD
+Filename: filebrowser-1.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## filebrowser/__init__.py

```diff
@@ -0,0 +1,2 @@
+00000000: 5f5f 7665 7273 696f 6e5f 5f20 3d20 2231  __version__ = "1
+00000010: 2e31 2e34 22                             .1.4"
```

## filebrowser/app.py

```diff
@@ -216,19 +216,19 @@
             temp_dir = tempfile.gettempdir()
             zipname = os.path.join(temp_dir, foldername)
 
             try:
                 with ZipFile(f"{foldername}.zip", "w") as zip:
                     for file in file_paths:
                         zip.write(file)
-                return send_from_directory(directory=os.path.dirname(target), filename=f"{foldername}.zip", as_attachment=True)
+                return send_from_directory(directory=os.path.dirname(target), path=f"{foldername}.zip", as_attachment=True)
 
             finally:
                 if os.path.exists(f"{foldername}.zip"):
                     os.remove(f"{foldername}.zip")
         else:
             try:
-                return send_from_directory(directory=os.path.dirname(target), filename=os.path.basename(target), as_attachment=True)
+                return send_from_directory(directory=os.path.dirname(target), path=os.path.basename(target), as_attachment=True)
             except IOError:
                 return "can't download"
         
     app.run(host=host, port=port, debug=True)
```

## filebrowser/main.py

```diff
@@ -1,12 +1,11 @@
 import argparse
 from pathlib import Path
 from filebrowser.app import server
 
-__version__ = "1.1.3"
 package_name = "filebrowser"
 
 example_uses = '''example:
    filebrowser 
    filebrowser --host {custom_address} --port {custom_port} --dir {folder_path}
    filebrowser --host {custom_address} -p {custom_port} -d {folder_path}'''
```

## Comparing `filebrowser-1.1.3.dist-info/LICENSE` & `filebrowser-1.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `filebrowser-1.1.3.dist-info/METADATA` & `filebrowser-1.1.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: filebrowser
-Version: 1.1.3
+Version: 1.1.4
 Summary: Simple web file browser
 Home-page: https://github.com/jakbin/filebrowser
 Author: jakbin
 License: MIT License
 Keywords: filebrowser,web,file,browser,web browser
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: flask (<=2.0)
+Requires-Dist: flask
 
 # filebrowser
 
 The single page web file browser that use ajax.
 
  ![flask](https://img.shields.io/badge/flask-≤2.0-green.svg)
  [![PyPI version](https://badge.fury.io/py/filebrowser.svg)](https://pypi.org/project/filebrowser/)
@@ -52,8 +52,7 @@
 
 filebrowser --host {custom_address} -p {custom_port} -d {folder_path}
 ```
 
 ## To do
 - [ ] Use pure js.
 - [ ] Comment code.
-
```

## Comparing `filebrowser-1.1.3.dist-info/RECORD` & `filebrowser-1.1.4.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-filebrowser/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-filebrowser/app.py,sha256=ISfUYgYK5DCMkisrmiK9-NsWh_2Jk1s4Yhfu_X5p9tE,8238
+filebrowser/__init__.py,sha256=PDawFA4JZ6VmetYHnwoA5t79JrblMQ6S08w36AKgCB8,21
+filebrowser/app.py,sha256=EB2Xu2MvfQiJyoCgAm05mKa0Fl6Dski-YIP7weoYE70,8230
 filebrowser/funcs.py,sha256=jTKLqegaWEqj698RW4R9-EAhHqf8orDVuG2K95SkJN4,1529
-filebrowser/main.py,sha256=vfDZhamPCQuAUZd0n8JlPcI08uK1bznEtowSTMAcoqg,1465
+filebrowser/main.py,sha256=0YPGYdSYjUIdS_k49NbKKvm4i7IHKznauN-JCksb7XE,1443
 filebrowser/static/css/file.css,sha256=KNB_WhhZ_0EccYbuTt68qUc9-WF17WjtKHULEFIStZg,22591
 filebrowser/static/css/file1.css,sha256=Qt_R9LyobipXE4kLXoHYEGJ-w2SGXqgtvYQ_b6ERHRg,3322
 filebrowser/static/fonts/MaterialIcons-Regular.570eb838.woff2,sha256=qH1myRsufcVTCu92wDvWo9JepYJhEL9IA7VhuBHMhyY,44300
 filebrowser/static/js/jquery.min.js,sha256=9_aliU8dGd2tb6OSsuzixeV4y_faTqgFtohetphbbj0,89476
 filebrowser/static/js/main.js,sha256=yXg8lxoCYQ0dRJouTRhRARloogC2mHuFc8hMnIozOtc,19702
 filebrowser/templates/data.html,sha256=382IrDurqxD9JZmkGtaJbL7i5HI9DAy8VlsEXo1-oU4,1249
 filebrowser/templates/index.html,sha256=8NazMDUN6lyn1YCf153ptzfy8HGms74PBCd2Gwved8M,16123
-filebrowser-1.1.3.dist-info/LICENSE,sha256=cHEEujGGhzJsSsay79nimRhwIp5BortOd8p9Pl5ihIQ,1075
-filebrowser-1.1.3.dist-info/METADATA,sha256=m5dNLw7Z_B4PDi5fSjbwMfFvb7F0dVZN2OAL6oDAXyE,1630
-filebrowser-1.1.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-filebrowser-1.1.3.dist-info/entry_points.txt,sha256=4XiI5aadq-IgK2xgCKH5LSTqeBcG86ANxlv9mKqvmZE,53
-filebrowser-1.1.3.dist-info/top_level.txt,sha256=WnSAG9Mf-wbFSy7Q5yr0jx0TX0wEdw04Fu37H-A6rFE,12
-filebrowser-1.1.3.dist-info/RECORD,,
+filebrowser-1.1.4.dist-info/LICENSE,sha256=cHEEujGGhzJsSsay79nimRhwIp5BortOd8p9Pl5ihIQ,1075
+filebrowser-1.1.4.dist-info/METADATA,sha256=zQQDXCyijfcgLRUuiUp4KMDC4Lj_VxwJ1gNWdlpJ-Yk,1621
+filebrowser-1.1.4.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+filebrowser-1.1.4.dist-info/entry_points.txt,sha256=eeKC5nziRgn7-xQJtLMQCce8iwCCerNL2TWvvbOqFpM,54
+filebrowser-1.1.4.dist-info/top_level.txt,sha256=WnSAG9Mf-wbFSy7Q5yr0jx0TX0wEdw04Fu37H-A6rFE,12
+filebrowser-1.1.4.dist-info/RECORD,,
```

