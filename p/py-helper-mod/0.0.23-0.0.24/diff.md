# Comparing `tmp/py-helper-mod-0.0.23.tar.gz` & `tmp/py-helper-mod-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp3rjnqx8j/py-helper-mod-0.0.23.tar", last modified: Fri Apr 14 20:29:57 2023, max compression
+gzip compressed data, was "/srv/storage/projects/scripts/py_helper/dist/tmp5cciwnzh/py-helper-mod-0.0.24.tar", last modified: Sun May  7 03:27:35 2023, max compression
```

## Comparing `py-helper-mod-0.0.23.tar` & `py-helper-mod-0.0.24.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/pyproject.toml
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/README.md
-drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/dependency_links.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/top_level.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/SOURCES.txt
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/py_helper_mod.egg-info/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.23/LICENSE
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.23/setup.py
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/PKG-INFO
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-04-14 20:29:57.000000 py-helper-mod-0.0.23/setup.cfg
--rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    78400 2023-04-14 20:29:24.000000 py-helper-mod-0.0.23/py_helper.py
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      104 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/pyproject.toml
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      117 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/README.md
+drwxrwsr-x   0 ejohnfelt  (1500) storage   (1499)        0 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)        1 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/dependency_links.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       10 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/top_level.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      212 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/SOURCES.txt
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/py_helper_mod.egg-info/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)     1069 2022-03-11 16:54:40.000000 py-helper-mod-0.0.24/LICENSE
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)       66 2022-03-13 03:55:54.000000 py-helper-mod-0.0.24/setup.py
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      681 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/PKG-INFO
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)      712 2023-05-07 03:27:35.000000 py-helper-mod-0.0.24/setup.cfg
+-rw-rw-r--   0 ejohnfelt  (1500) storage   (1499)    79547 2023-05-07 03:26:17.000000 py-helper-mod-0.0.24/py_helper.py
```

### Comparing `py-helper-mod-0.0.23/py_helper_mod.egg-info/PKG-INFO` & `py-helper-mod-0.0.24/py_helper_mod.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.23
+Version: 0.0.24
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.23/LICENSE` & `py-helper-mod-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `py-helper-mod-0.0.23/PKG-INFO` & `py-helper-mod-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-helper-mod
-Version: 0.0.23
+Version: 0.0.24
 Summary: Collection of my helpers (functions, classes, etc)
 Home-page: https://github.com/ejohnfel/py_helper
 Author: Eric Johnfelt
 Author-email: ejohnfel@hotmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/ejohnfel/py_helper/issues
 Platform: UNKNOWN
```

### Comparing `py-helper-mod-0.0.23/setup.cfg` & `py-helper-mod-0.0.24/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 formats = zip,tar
 
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = py-helper-mod
-version = 0.0.23
+version = 0.0.24
 author = Eric Johnfelt
 author_email = ejohnfel@hotmail.com
 description = Collection of my helpers (functions, classes, etc)
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejohnfel/py_helper
 project_urls =
```

### Comparing `py-helper-mod-0.0.23/py_helper.py` & `py-helper-mod-0.0.24/py_helper.py`

 * *Files 3% similar despite different names*

```diff
@@ -899,15 +899,15 @@
 		return self.gap
 
 #
 # Module Variables and Constants
 #
 
 # Version (Mine, and PEP defactos)
-VERSION=(0,0,23)
+VERSION=(0,0,24)
 Version = __version__ = ".".join([ str(x) for x in VERSION ])
 
 # Start Random Generator
 random.seed()
 
 # Signals Debug mode operations
 __DebugMode__ = False
@@ -2598,14 +2598,48 @@
 	crc = None
 
 	with open(fname,"rb") as file:
 		crc = zlib.crc32(file.read())
 
 	return crc
 
+def Gzip(filename,removeOriginal=True,removeArchive=True):
+	"""GZip a File"""
+
+	compressedFilename = f"{filename}.gz"
+
+	try:
+		if os.path.exists(compressedFilename) and removeArchive:
+			os.remove(compressedFilename)
+
+		with open(filename,"r") as uncompressedFile, gzip.open(compressedFilename,"wb") as compressedFile:
+			shutil.copyfileobj(uncompressedFile,compressedFile,4096)
+
+		if removeOriginal:
+			os.remove(filename)
+	except Exception as err:
+		ErrMsg(err,f"An error occurred while trying to compress {filename} or removing an existing archive")
+
+def Ungzip(filename,removeArchive=True,mode="w",clearOriginal=False):
+	"""Un Gzip A File"""
+
+	uncompressedFilename = filename.removesuffix(".gz")
+
+	try:
+		if os.path.exists(uncompressedFilename) and clearOriginal:
+			os.remove(uncompressedFilename)
+
+		with open(uncompressedFilename,mode) as uncompressedFile, gzip.open(filename,"rb") as compressedFile:
+			shutil.copyfileobj(compressedFile,uncompressedFile,4096)
+
+		if removeArchive:
+			os.remove(compressedFilename)
+	except Exception as err:
+		ErrMsg(err,f"An error occurrred while trying to uncompress {filename} or removing the archive")
+
 # Read List from file (will remove lines starting with a hash mark "#")
 def ReadList(fname,mode="r",removecomments=True,splitter=None):
 	"""
 	Read a simple list from file that may contain line comments that start with a hash mark.
 	Optionally retain the comments and optionally split the line using a custom splitter function.
 	"""
 	items = list()
```

