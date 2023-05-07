# Comparing `tmp/easierfile-2.3.0.tar.gz` & `tmp/easierfile-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easierfile-2.3.0.tar", max compression
+gzip compressed data, was "easierfile-3.0.0.tar", max compression
```

## Comparing `easierfile-2.3.0.tar` & `easierfile-3.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-2.3.0/easierfile/__init__.py
--rw-r--r--   0        0        0     6446 2023-05-06 08:03:38.837573 easierfile-2.3.0/easierfile/file.py
--rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-2.3.0/LICENSE
--rw-r--r--   0        0        0      608 2023-05-06 07:00:41.465172 easierfile-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     1768 2023-05-06 05:19:38.035670 easierfile-2.3.0/README.md
--rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 easierfile-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-04-21 13:34:36.835394 easierfile-3.0.0/easierfile/__init__.py
+-rw-r--r--   0        0        0     6439 2023-05-07 05:44:53.277058 easierfile-3.0.0/easierfile/file.py
+-rw-r--r--   0        0        0     1092 2023-04-11 00:52:37.919987 easierfile-3.0.0/LICENSE
+-rw-r--r--   0        0        0      608 2023-05-07 05:44:53.281043 easierfile-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1768 2023-05-07 02:41:55.757461 easierfile-3.0.0/README.md
+-rw-r--r--   0        0        0     2630 1970-01-01 00:00:00.000000 easierfile-3.0.0/PKG-INFO
```

### Comparing `easierfile-2.3.0/easierfile/file.py` & `easierfile-3.0.0/easierfile/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         if self.__m_is_lock:
             try:
                 self.__lock(False)
             except FileNotFoundError:  # Indicates that the file lock does not exist and no further exception handling is required.
                 pass
 
     def __lock(self, is_lock):
-        if self.status["exist"]:
+        if self.state["exist"]:
             if is_lock:
                 self.__m_file = open(self.__m_static_info["path"])
                 _lock_file(self.__m_file)
                 self.__m_is_lock = is_lock
             else:
                 _unlock_file(self.__m_file)
                 self.__m_file.close()
@@ -68,15 +68,15 @@
         else:
             if is_lock:
                 raise FileNotFoundError("File was about to be occupied, but not found: " + self.__m_static_info["path"])
             else:
                 raise FileNotFoundError("File was about to be unoccupied, but not found: " + self.__m_static_info["path"])
 
     def create(self):
-        if not self.status["exist"]:
+        if not self.state["exist"]:
             if not os.path.exists(self.__m_static_info["dir_path"]):  # Create the file directory if it doesn't exist, so that code<open()> doesn't throw the exception.
                 os.mkdir(self.__m_static_info["dir_path"])
             try:
                 file_temp = open(self.__m_static_info["path"], "x")
             except FileExistsError:  # Avoid exception caused by creating corresponding file in other ways during program execution intervals.
                 pass
             else:
@@ -85,41 +85,41 @@
                 self.__lock(True)
         else:
             raise FileExistsError("File exists: " + self.__m_static_info["path"])
 
     def delete(self):
         if self.__m_is_lock:
             self.__lock(False)
-        if self.status["exist"]:
+        if self.state["exist"]:
             os.remove(self.__m_static_info["path"])
 
     def rewrite(self,content):
-        if self.status["exist"]:
+        if self.state["exist"]:
             """
             Automatically obtain the most suitable encoding format for the input content.
             
             :samp: chardet.detect(content.encode())["encoding"]
             """
             file_temp = open(self.__m_static_info["path"], "w", encoding=chardet.detect(content.encode())["encoding"])
             file_temp.write(content)
             file_temp.close()
         else:
             raise FileNotFoundError("File not found: " + self.__m_static_info["path"])
 
     def append(self,content):
-        if self.status["exist"]:
+        if self.state["exist"]:
             file_temp = open(self.__m_static_info["path"], "a", encoding=chardet.detect(content.encode())["encoding"])
             file_temp.write(content)
             file_temp.close()
         else:
             raise FileNotFoundError("File not found: " + self.__m_static_info["path"])
 
     @property
     def content(self):
-        if self.status["exist"]:
+        if self.state["exist"]:
             """
             Automatically obtain the most suitable encoding format for the output content.
             
             :samp: self.info["encoding"]
             
             In fact, it gets the encoding format of the read file. 
             """
@@ -150,15 +150,15 @@
 
         # Store the acquisition way of dynamic file information.
         info["encoding"] = get_info_encoding
 
         return info
 
     @property
-    def status(self):
+    def state(self):
         def get_status_file_lock():
             return self.__m_is_lock
 
         def get_status_exist():
             return os.path.isfile(self.__m_static_info["path"])
 
         status = DynamicDict()
```

### Comparing `easierfile-2.3.0/LICENSE` & `easierfile-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `easierfile-2.3.0/pyproject.toml` & `easierfile-3.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "easierfile"
-version = "2.3.0"
+version = "3.0.0"
 description = "An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations."
 license = "MIT"
 authors = ["leoweyr <leoweyr@foxmail.com>"]
 readme = "README.md"
 repository = "https://github.com/leoweyr/Python-Easierfile"
 classifiers = [
     "Development Status :: 4 - Beta"
```

### Comparing `easierfile-2.3.0/README.md` & `easierfile-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `easierfile-2.3.0/PKG-INFO` & `easierfile-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easierfile
-Version: 2.3.0
+Version: 3.0.0
 Summary: An easier-to-use Python package that object-oriented encapsulates Python traditional built-in file operations.
 Home-page: https://github.com/leoweyr/Python-Easierfile
 License: MIT
 Author: leoweyr
 Author-email: leoweyr@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

