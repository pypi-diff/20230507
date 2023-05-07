# Comparing `tmp/fabsync-1.0.0.tar.gz` & `tmp/fabsync-1.1.0.tar.gz`

## Comparing `fabsync-1.0.0.tar` & `fabsync-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,62 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fabsync-1.0.0/.coveragerc
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fabsync-1.0.0/.flake8
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fabsync-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fabsync-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fabsync-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0    20068 2020-02-02 00:00:00.000000 fabsync-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0    12526 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/__init__.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/config.py
--rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/files.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/fs.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/functools.py
--rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/md5.sh
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/src/fabsync/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/test_config.py
--rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/test_files.py
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/test_functools.py
--rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/test_sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/absent/.keepme
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/complete/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/empty/_sync.toml
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/schema_error/_sync.toml
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/tags/_sync.toml
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/tags2/_sync.toml
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/toml_error/_sync.toml
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/config/vars/_sync.toml
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/_sync.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dot-profile
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/file1.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/file2.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dir1/_sync.toml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dir1/file3.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dir1/ignore-me.txt
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dot-config/_sync.toml
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/dot-config/sync.toml
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/ignore-me/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/loading/ignore-me/file.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/selection/etc/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/selection/etc/pf.conf
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/selection/usr/local/bin/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/selection/usr/local/bin/myapp.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/files/selection/var/myapp/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/empty/tmp/_sync.toml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/group/home/hg/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/mode/var
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/mode/etc/_sync.toml
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/render/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/render/file.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/errors/user/home/hg/_sync.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/etc/pf.conf
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/home/hg/_sync.toml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/home/hg/dot-hgrc
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/home/hg/bin/_sync.toml
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/home/hg/bin/blob
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fabsync-1.0.0/tests/sync/general/home/hg/bin/hook.sh
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fabsync-1.0.0/.gitignore
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fabsync-1.0.0/.hgignore
--rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 fabsync-1.0.0/README.md
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fabsync-1.0.0/UNLICENSE
--rw-r--r--   0        0        0     2466 2020-02-02 00:00:00.000000 fabsync-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     6663 2020-02-02 00:00:00.000000 fabsync-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 fabsync-1.1.0/.coveragerc
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fabsync-1.1.0/.flake8
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 fabsync-1.1.0/.hgtags
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/make.bat
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/source/conf.py
+-rw-r--r--   0        0        0    20355 2020-02-02 00:00:00.000000 fabsync-1.1.0/docs/source/index.rst
+-rw-r--r--   0        0        0    12526 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/__init__.py
+-rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/config.py
+-rw-r--r--   0        0        0    11520 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/files.py
+-rw-r--r--   0        0        0     5068 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/fs.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/functools.py
+-rwxr-xr-x   0        0        0      365 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/md5.sh
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/src/fabsync/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_config.py
+-rw-r--r--   0        0        0     7168 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_files.py
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_functools.py
+-rw-r--r--   0        0        0    10802 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/test_sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/absent/.keepme
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/complete/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/empty/_sync.toml
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/schema_error/_sync.toml
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/tags/_sync.toml
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/tags2/_sync.toml
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/toml_error/_sync.toml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/config/vars/_sync.toml
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/_sync.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-profile
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/file1.txt
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/file2.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/_sync.toml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/file3.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dir1/ignore-me.txt
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-config/_sync.toml
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/dot-config/sync.toml
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/ignore-me/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/loading/ignore-me/file.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/etc/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/etc/pf.conf
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/usr/local/bin/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/usr/local/bin/myapp.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/files/selection/var/myapp/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/empty/tmp/_sync.toml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/group/home/hg/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/mode/var
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/mode/etc/_sync.toml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/render/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/render/file.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/errors/user/home/hg/_sync.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/etc/pf.conf
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/_sync.toml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/dot-hgrc
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/_sync.toml
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/blob
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 fabsync-1.1.0/tests/sync/general/home/hg/bin/hook.sh
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 fabsync-1.1.0/.gitignore
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 fabsync-1.1.0/.hgignore
+-rw-r--r--   0        0        0     5880 2020-02-02 00:00:00.000000 fabsync-1.1.0/README.md
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 fabsync-1.1.0/UNLICENSE
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 fabsync-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     6713 2020-02-02 00:00:00.000000 fabsync-1.1.0/PKG-INFO
```

### Comparing `fabsync-1.0.0/docs/Makefile` & `fabsync-1.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/docs/make.bat` & `fabsync-1.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/docs/source/conf.py` & `fabsync-1.1.0/docs/source/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'fabsync'
 project_copyright = "2022, Peter Sagerson"
 author = "Peter Sagerson"
 
 # The full version, including alpha/beta/rc tags
-release = '0.1.0'
+release = '1.1.0'
 version = '.'.join(release.split('.')[:2])
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `fabsync-1.0.0/docs/source/index.rst` & `fabsync-1.1.0/docs/source/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -488,14 +488,22 @@
 destinations and/or render vars. You could generate a source tree into a temp
 directory and sync that.
 
 And, of course, you can always just use your Fabric connection to manipulate the
 remote host directly. fabsync is a tool to be used where it's appropriate or
 convenient, and ignored otherwise.
 
+Local operation
+~~~~~~~~~~~~~~~
+
+Everything so far has been about syncing files to remote hosts, which is the
+primary intention of fabsync. However, if you pass an :class:`invoke.Context` to
+the sync API instead of a :class:`fabric.Connection`, it will manipulate the
+local filesystem.
+
 
 Reference
 ---------
 
 Loading sources
 ~~~~~~~~~~~~~~~
```

### Comparing `fabsync-1.0.0/src/fabsync/__init__.py` & `fabsync-1.1.0/src/fabsync/__init__.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/src/fabsync/config.py` & `fabsync-1.1.0/src/fabsync/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,24 @@
 
 from collections import ChainMap
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import AbstractSet, Any, cast, Mapping, MutableMapping, Union
 
 from jsonschema import validate, ValidationError
-import tomli as toml
 
 from .functools import fnone, update_in
 
 
+try:
+    import tomllib as toml  # type: ignore[import]
+except ModuleNotFoundError:
+    import tomli as toml
+
+
 #
 # Constants and types
 #
 
 CONFIG_NAME = '_sync.toml'
```

### Comparing `fabsync-1.0.0/src/fabsync/files.py` & `fabsync-1.1.0/src/fabsync/files.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/src/fabsync/fs.py` & `fabsync-1.1.0/src/fabsync/fs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,14 @@
 from functools import singledispatch
 import grp
 import hashlib
 import io
 import os
 from pathlib import Path
 import pwd
-
-#  import shlex
 from typing import cast, Iterator, Mapping, Optional, Tuple, TYPE_CHECKING, Union
 
 import fabric
 
 
 Pathable = Union[os.PathLike, str]
 
@@ -39,14 +37,15 @@
 
     This includes all of the high-level operations we perform on files and
     directories. It allows us to transparently support fabric connections,
     invoke contexts, and test environments.
 
     """
 
+    @abstractmethod
     def cleanup(self) -> None:
         pass
 
     @abstractmethod
     def sysinfo(self) -> SysInfo:
         pass
 
@@ -80,14 +79,17 @@
 
 
 class LocalFS(FS):
     """
     Local filesystem operations.
     """
 
+    def cleanup(self) -> None:
+        pass
+
     def sysinfo(self) -> SysInfo:
         return SysInfo(
             users={pw.pw_name: pw.pw_uid for pw in pwd.getpwall()},
             groups={gr.gr_name: gr.gr_gid for gr in grp.getgrall()},
         )
 
     def stat(self, path: Pathable) -> Optional[os.stat_result]:
```

### Comparing `fabsync-1.0.0/src/fabsync/functools.py` & `fabsync-1.1.0/src/fabsync/functools.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/tests/test_config.py` & `fabsync-1.1.0/tests/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from __future__ import annotations
 
 from pathlib import Path
 from unittest import TestCase
 
 import jsonschema
-import tomli as toml
 
 from fabsync.config import ConfigError, SyncConfig
 
 
+try:
+    import tomllib as toml  # type: ignore[import]
+except ModuleNotFoundError:
+    import tomli as toml
+
+
 class ConfigTestCase(TestCase):
     def test_absent(self):
         config = self.load("absent")
 
         self.assertEqual(config.name, "absent")
         self.assertEqual(config.files, {})
         self.assertEqual(config.defaults, SyncConfig.root().defaults)
```

### Comparing `fabsync-1.0.0/tests/test_files.py` & `fabsync-1.1.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/tests/test_functools.py` & `fabsync-1.1.0/tests/test_functools.py`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/tests/test_sync.py` & `fabsync-1.1.0/tests/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -354,15 +354,26 @@
     def run(self, command, **kwargs):
         def map_path(arg: str) -> str:
             if arg.startswith('/'):
                 arg = str(self.mock_path(arg))
             return arg
 
         args = [map_path(arg) for arg in shlex.split(command)]
-        result = subprocess.run(args, capture_output=True, check=True)
+        try:
+            result = subprocess.run(args, capture_output=True, check=True)
+        except FileNotFoundError:
+            # Fake getent if necessary to allow the tests to run on macOS.
+            if args[0] == 'getent' and args[1] in ['passwd', 'group']:
+                result = subprocess.run(
+                    ['grep', '-v', '^#', f'/etc/{args[1]}'],
+                    capture_output=True,
+                )
+            else:
+                raise
+
         return invoke.Result(result.stdout.decode())
 
     def sftp(self):
         return self._sftp
 
     @cached_property
     def _sftp(self):
```

### Comparing `fabsync-1.0.0/README.md` & `fabsync-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/UNLICENSE` & `fabsync-1.1.0/UNLICENSE`

 * *Files identical despite different names*

### Comparing `fabsync-1.0.0/pyproject.toml` & `fabsync-1.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'fabsync'
-version = '1.0.0'
+version = '1.1.0'
 description = "File syncing via Fabric."
 keywords = ['fabric']
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: The Unlicense (Unlicense)',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3 :: Only',
@@ -16,17 +16,17 @@
 license = 'Unlicense'
 license-files = { paths = ['UNLICENSE'] }
 authors = [
     { name = "Peter Sagerson", email = "psagers@ignorare.net" }
 ]
 
 dependencies = [
-    'fabric~=2.7',
-    'tomli~=2.0',
+    'fabric',
     'jsonschema~=4.5',
+    'tomli~=2.0; python_version < "3.11"',
 ]
 
 [project.urls]
 'Homepage' = 'https://sr.ht/~psagers/fabsync/'
 'Source code' = 'https://hg.sr.ht/~psagers/fabsync'
 'Documentation' = 'https://fabsync.ignorare.net/'
 
@@ -42,22 +42,30 @@
     'flake8-bugbear',
     'flake8~=5.0',
     'isort~=5.0',
     'mypy',
     'types-invoke',
     'types-jsonschema',
     'types-paramiko',
+
+    # TEMP: Work around https://github.com/fabric/fabric/issues/2263
+    'invoke<2.1',
 ]
 
 [tool.hatch.envs.default.scripts]
 lint = [
     'flake8 src',
-    'isort -c src',
-    'mypy --no-incremental src',
-    'black --check src',
+    'isort --check --quiet src',
+    'mypy --no-incremental --no-error-summary src',
+    'black --check --quiet src',
+]
+
+fix = [
+    'isort src',
+    'black src',
 ]
 
 test = 'python -m unittest {args}'
 
 cov = [
     'coverage run --source fabsync -m unittest {args}',
     'coverage report',
@@ -66,29 +74,35 @@
 check = ['lint', 'cov']
 
 
 # The docs environment is for building the documentation with Sphinx.
 [tool.hatch.envs.docs]
 python = '3'
 dependencies = [
+    # TEMP: Work around https://github.com/fabric/fabric/issues/2263
+    'invoke<2.1',
     'sphinx~=4.5',
 ]
 
 [tool.hatch.envs.docs.scripts]
-build = 'gmake -C docs html'
-open = 'command open docs/build/html/index.html'
+make = 'make -C docs html'
+gmake = 'gmake -C docs html'
+open = 'xdg-open docs/build/html/index.html'
 
 
 # The test environment just defines a test matrix. The test scripts are all
 # inherited from default.
 [tool.hatch.envs.test]
-dependencies = []
+dependencies = [
+    # TEMP: Work around https://github.com/fabric/fabric/issues/2263
+    'invoke<2.1',
+]
 
 [[tool.hatch.envs.test.matrix]]
-python = ['38', '39', '310']
+python = ['38', '39', '310', '311']
 
 
 [build-system]
 requires = ['hatchling']
 build-backend = 'hatchling.build'
```

### Comparing `fabsync-1.0.0/PKG-INFO` & `fabsync-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: fabsync
-Version: 1.0.0
+Version: 1.1.0
 Summary: File syncing via Fabric.
 Project-URL: Homepage, https://sr.ht/~psagers/fabsync/
 Project-URL: Source code, https://hg.sr.ht/~psagers/fabsync
 Project-URL: Documentation, https://fabsync.ignorare.net/
 Author-email: Peter Sagerson <psagers@ignorare.net>
+License-Expression: Unlicense
 License-File: UNLICENSE
 Keywords: fabric
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: fabric~=2.7
+Requires-Dist: fabric
 Requires-Dist: jsonschema~=4.5
-Requires-Dist: tomli~=2.0
+Requires-Dist: tomli~=2.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <!-- vim: set tw=80 lbr: -->
 # fabsync
 
 - Homepage: https://sr.ht/~psagers/fabsync/
 - Source code: https://hg.sr.ht/~psagers/fabsync
```

