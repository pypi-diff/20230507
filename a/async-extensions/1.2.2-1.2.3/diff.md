# Comparing `tmp/async_extensions-1.2.2.tar.gz` & `tmp/async_extensions-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_extensions-1.2.2.tar", max compression
+gzip compressed data, was "async_extensions-1.2.3.tar", max compression
```

## Comparing `async_extensions-1.2.2.tar` & `async_extensions-1.2.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1092 2023-04-07 19:07:21.256431 async_extensions-1.2.2/LICENSE
--rw-r--r--   0        0        0     2578 2023-04-07 19:07:21.256431 async_extensions-1.2.2/README.md
--rw-r--r--   0        0        0     2888 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/__init__.py
--rw-r--r--   0        0        0      732 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/blocking.py
--rw-r--r--   0        0        0      431 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/cancel.py
--rw-r--r--   0        0        0     1174 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/channel.py
--rw-r--r--   0        0        0     1781 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/close.py
--rw-r--r--   0        0        0     7840 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/collect.py
--rw-r--r--   0        0        0      118 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/constants.py
--rw-r--r--   0        0        0       80 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/current.py
--rw-r--r--   0        0        0       88 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/errors.py
--rw-r--r--   0        0        0      101 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/file.py
--rw-r--r--   0        0        0      174 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/low_level.py
--rw-r--r--   0        0        0       44 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/path.py
--rw-r--r--   0        0        0       87 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/process.py
--rw-r--r--   0        0        0        0 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/py.typed
--rw-r--r--   0        0        0      385 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/run.py
--rw-r--r--   0        0        0       76 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/signal.py
--rw-r--r--   0        0        0       77 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/sleep.py
--rw-r--r--   0        0        0     1328 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/standard.py
--rw-r--r--   0        0        0      143 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/synchronization.py
--rw-r--r--   0        0        0       70 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/task_group.py
--rw-r--r--   0        0        0      176 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/types.py
--rw-r--r--   0        0        0      859 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/typing.py
--rw-r--r--   0        0        0      732 2023-04-07 19:07:21.256431 async_extensions-1.2.2/async_extensions/wait.py
--rw-r--r--   0        0        0     2230 2023-04-07 19:07:21.256431 async_extensions-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 async_extensions-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-07 12:20:20.359473 async_extensions-1.2.3/LICENSE
+-rw-r--r--   0        0        0     2578 2023-05-07 12:20:20.359473 async_extensions-1.2.3/README.md
+-rw-r--r--   0        0        0     2888 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/__init__.py
+-rw-r--r--   0        0        0      732 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/blocking.py
+-rw-r--r--   0        0        0      431 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/cancel.py
+-rw-r--r--   0        0        0     1174 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/channel.py
+-rw-r--r--   0        0        0     1781 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/close.py
+-rw-r--r--   0        0        0     7840 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/collect.py
+-rw-r--r--   0        0        0      118 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/constants.py
+-rw-r--r--   0        0        0       80 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/current.py
+-rw-r--r--   0        0        0       88 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/errors.py
+-rw-r--r--   0        0        0      101 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/file.py
+-rw-r--r--   0        0        0      174 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/low_level.py
+-rw-r--r--   0        0        0       44 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/path.py
+-rw-r--r--   0        0        0       87 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/process.py
+-rw-r--r--   0        0        0        0 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/py.typed
+-rw-r--r--   0        0        0      385 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/run.py
+-rw-r--r--   0        0        0       76 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/signal.py
+-rw-r--r--   0        0        0       77 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/sleep.py
+-rw-r--r--   0        0        0     1333 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/standard.py
+-rw-r--r--   0        0        0      143 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/synchronization.py
+-rw-r--r--   0        0        0       70 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/task_group.py
+-rw-r--r--   0        0        0      176 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/types.py
+-rw-r--r--   0        0        0      859 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/typing.py
+-rw-r--r--   0        0        0      732 2023-05-07 12:20:20.363473 async_extensions-1.2.3/async_extensions/wait.py
+-rw-r--r--   0        0        0     2230 2023-05-07 12:20:20.363473 async_extensions-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3707 1970-01-01 00:00:00.000000 async_extensions-1.2.3/PKG-INFO
```

### Comparing `async_extensions-1.2.2/LICENSE` & `async_extensions-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/README.md` & `async_extensions-1.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.2.2"
+async-extensions = "^1.2.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

### Comparing `async_extensions-1.2.2/async_extensions/__init__.py` & `async_extensions-1.2.3/async_extensions/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 __description__ = "Asynchronous extensions."
 __url__ = "https://github.com/nekitdev/async-extensions"
 
 __title__ = "async_extensions"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.2.2"
+__version__ = "1.2.3"
 
 from async_extensions.blocking import run_blocking_in_process, run_blocking_in_thread
 from async_extensions.cancel import CancelScope, create_cancel_scope, shield
 from async_extensions.channel import (
     MemoryChannel, MemoryChannelFactory, MemoryReceiveChannel, MemorySendChannel
 )
 from async_extensions.close import (
```

### Comparing `async_extensions-1.2.2/async_extensions/blocking.py` & `async_extensions-1.2.3/async_extensions/blocking.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/async_extensions/channel.py` & `async_extensions-1.2.3/async_extensions/channel.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/async_extensions/close.py` & `async_extensions-1.2.3/async_extensions/close.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/async_extensions/collect.py` & `async_extensions-1.2.3/async_extensions/collect.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/async_extensions/standard.py` & `async_extensions-1.2.3/async_extensions/standard.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 async def async_next(
     async_iterator: AsyncIterator[Any], default: Any = no_default
 ) -> Any:
     if is_instance(async_iterator, AsyncIterator):
         try:
             return await async_iterator.__anext__()
 
-        except StopIteration:
+        except StopAsyncIteration:
             if default is no_default:
                 raise
 
             return default
 
     raise TypeError(NOT_ASYNC_ITERATOR.format(repr(async_iterator)))
```

### Comparing `async_extensions-1.2.2/async_extensions/typing.py` & `async_extensions-1.2.3/async_extensions/typing.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/async_extensions/wait.py` & `async_extensions-1.2.3/async_extensions/wait.py`

 * *Files identical despite different names*

### Comparing `async_extensions-1.2.2/pyproject.toml` & `async_extensions-1.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-extensions"
-version = "1.2.2"
+version = "1.2.3"
 description = "Asynchronous extensions."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/async-extensions"
@@ -82,15 +82,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "async-extensions"
-version = "1.2.2"
+version = "1.2.3"
 url = "https://github.com/nekitdev/async-extensions"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `async_extensions-1.2.2/PKG-INFO` & `async_extensions-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-extensions
-Version: 1.2.2
+Version: 1.2.3
 Summary: Asynchronous extensions.
 Home-page: https://github.com/nekitdev/async-extensions
 License: MIT
 Keywords: python,async,extensions
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -65,15 +65,15 @@
 $ poetry add async-extensions
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-async-extensions = "^1.2.2"
+async-extensions = "^1.2.3"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.async-extensions]
 git = "https://github.com/nekitdev/async-extensions.git"
```

