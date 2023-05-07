# Comparing `tmp/systempath-1.0.9-py3-none-any.whl.zip` & `tmp/systempath-1.0a8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 26628 bytes, number of entries: 7
--rw-r--r--  2.0 unx    63906 b- defN 23-May-07 08:21 systempath/__init__.py
--rw-r--r--  2.0 unx    41175 b- defN 23-May-07 08:21 systempath/i systempath.py
--rw-r--r--  2.0 unx    11389 b- defN 23-May-07 08:22 systempath-1.0.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     2084 b- defN 23-May-07 08:22 systempath-1.0.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 08:22 systempath-1.0.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-07 08:22 systempath-1.0.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      566 b- defN 23-May-07 08:22 systempath-1.0.9.dist-info/RECORD
-7 files, 119223 bytes uncompressed, 25630 bytes compressed:  78.5%
+Zip file size: 27097 bytes, number of entries: 7
+-rw-r--r--  2.0 unx    66968 b- defN 23-Feb-11 00:51 systempath/__init__.py
+-rw-r--r--  2.0 unx    39467 b- defN 23-Feb-11 00:51 systempath/gqylpy systempath.py
+-rw-r--r--  2.0 unx    11389 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2083 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      571 b- defN 23-Feb-11 00:52 systempath-1.0a8.dist-info/RECORD
+7 files, 120581 bytes uncompressed, 26089 bytes compressed:  78.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: systempath/__init__.py
 Comment: 
 
-Filename: systempath/i systempath.py
+Filename: systempath/gqylpy systempath.py
 Comment: 
 
-Filename: systempath-1.0.9.dist-info/LICENSE
+Filename: systempath-1.0a8.dist-info/LICENSE
 Comment: 
 
-Filename: systempath-1.0.9.dist-info/METADATA
+Filename: systempath-1.0a8.dist-info/METADATA
 Comment: 
 
-Filename: systempath-1.0.9.dist-info/WHEEL
+Filename: systempath-1.0a8.dist-info/WHEEL
 Comment: 
 
-Filename: systempath-1.0.9.dist-info/top_level.txt
+Filename: systempath-1.0a8.dist-info/top_level.txt
 Comment: 
 
-Filename: systempath-1.0.9.dist-info/RECORD
+Filename: systempath-1.0a8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## systempath/__init__.py

```diff
@@ -1,8 +1,8 @@
-"""(OOP) Operating system paths and files.
+"""Operating system paths and files.
 
 Let Python operating system paths and files become Simple, Simpler, Simplest,
 Humanization, Unification, Flawless.
 
     >>> from systempath import SystemPath, Directory, File
 
     >>> root = SystemPath('/')
@@ -14,15 +14,15 @@
     >>> file: File = home['alpha.txt']
     >>> file
     /home/gqylpy/alpha.txt
 
     >>> file.open.rb().read()
     b'GQYLPY \xe6\x94\xb9\xe5\x8f\x98\xe4\xb8\x96\xe7\x95\x8c'
 
-    @version: 1.0.9
+    @version: 1.0.alpha8
     @author: 竹永康 <gqylpy@outlook.com>
     @source: https://github.com/gqylpy/systempath
 
 ────────────────────────────────────────────────────────────────────────────────
 Copyright (c) 2022, 2023 GQYLPY <http://gqylpy.com>. All rights reserved.
 
 Licensed under the Apache License, Version 2.0 (the "License");
@@ -35,18 +35,19 @@
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 import os
 import sys
+import warnings
 
 from typing import (
     TypeVar, Literal, Optional, Union, Tuple, List, BinaryIO, TextIO, Callable,
-    Generator, Iterator
+    Generator, Iterator, Any
 )
 
 BytesOrStr = TypeVar('BytesOrStr', bytes, str)
 PathLink   = BytesOrStr
 
 __all__ = ['SystemPath', 'Path', 'Directory', 'File', 'Open', 'Content', 'tree']
 
@@ -62,15 +63,16 @@
             dir_fd:          Optional[int]  = None,
             follow_symlinks: Optional[bool] = None
     ):
         """
         @param name
             A path link, hopefully absolute. If it is a relative path, the
             current working directory is used as the parent directory (the
-            return value of `os.getcwd()`).
+            return value of `os.getcwd()`). The current working directory is
+            used by default.
 
         @param autoabs
             Automatically normalize the path link and convert to absolute path,
             at initialization. Default False. It is always recommended that you
             enable the parameter when the passed path is a relative path.
 
         @param strict
@@ -116,25 +118,14 @@
             raise SystemPathNotFoundError
 
         self.name            = os.path.abspath(name) if autoabs else name
         self.strict          = strict
         self.dir_fd          = dir_fd
         self.follow_symlinks = follow_symlinks
 
-    def __bytes__(self) -> bytes:
-        """Return the path of type bytes."""
-
-    def __eq__(self, other: ['Path', PathLink], /) -> bool:
-        """Return True if the absolute path of the path instance is equal to the
-        absolute path of another path instance (can also be a path link
-        character) else False."""
-
-    def __ne__(self, other: ['Path', PathLink], /) -> bool:
-        return not self.__eq__(other)
-
     @property
     def basename(self) -> BytesOrStr:
         return os.path.basename(self.name)
 
     @property
     def dirname(self) -> 'Directory':
         return Directory(
@@ -461,15 +452,15 @@
         """Get the status of the file or directory, like `self.stat`, but do not
         follow symbolic links."""
         return self.__class__(
             self.name, dir_fd=self.dir_fd, follow_symlinks=False
         ).stat
 
     def getsize(self) -> int:
-        """Get the size of the file, return 0 if the path is a directory."""
+        """Get the size of the file, Return 0 if the path is a directory."""
         return os.path.getsize(self.name)
 
     def getctime(self) -> float:
         return os.path.getctime(self.name)
 
     def getmtime(self) -> float:
         return os.path.getmtime(self.name)
@@ -739,36 +730,40 @@
         """
 
 
 class Directory(Path):
     """Pass a directory path link to get a directory object, which you can then
     use to do anything a directory can do."""
 
+    def __getattr__(self, name: BytesOrStr) -> Any:
+        try:
+            return self[name]
+        except SystemPathNotFoundError:
+            raise AttributeError
+
     def __getitem__(
             self, name: BytesOrStr
-    ) -> Union['SystemPath', 'Directory', 'File', Path]:
+    ) -> Union['SystemPath', 'Directory', 'File']:
         path: PathLink = os.path.join(self.name, name)
 
         if self.strict:
             if os.path.isdir(path):
                 return Directory(path, strict=self.strict)
             if os.path.isfile(path):
                 return File(path)
-            if os.path.exists(name):
-                return Path(name)
-            else:
+            if not os.path.exists(path):
                 raise SystemPathNotFoundError
         else:
             return SystemPath(path)
 
     def __delitem__(self, name: BytesOrStr) -> None:
         Path(os.path.join(self.name, name)).delete()
 
     def __iter__(self) -> Generator:
-        return self.subpaths
+        return self.subpath
 
     @staticmethod
     def home(
             *,
             strict:          Optional[bool] = None,
             follow_symlinks: Optional[bool] = None
     ) -> 'Directory':
@@ -778,38 +773,38 @@
 
     @property
     def subpaths(self) -> Generator:
         """Get the instances of `Directory` or `File` for all subpaths (single
         layer) in the directory."""
 
     @property
-    def subpath_names(self) -> List[BytesOrStr]:
+    def subpaths_names(self) -> List[BytesOrStr]:
         """Get the names of all subpaths (single layer) in the directory. Call
         `os.listdir` internally."""
 
     def scandir(self) -> Iterator[os.DirEntry]:
         """Get instances of `os.DirEntry` for all files and subdirectories
         (single layer) in the directory, call `os.scandir` internally."""
 
     def tree(
             self,
             *,
-            level:      Optional[int]  = None,
-            bottom_up:  Optional[bool] = None,
-            omit_dir:   Optional[bool] = None,
-            mysophobia: Optional[bool] = None,
-            shortpath:  Optional[bool] = None
+            level:     Optional[int]  = None,
+            bottom_up: Optional[bool] = None,
+            omit_dir:  Optional[bool] = None,
+            idiocy:    Optional[bool] = None,
+            shortpath: Optional[bool] = None
     ) -> Generator:
         return tree(
             self.name,
-            level     =level,
-            bottom_up =bottom_up,
-            omit_dir  =omit_dir,
-            mysophobia=mysophobia,
-            shortpath =shortpath
+            level    =level,
+            bottom_up=bottom_up,
+            omit_dir =omit_dir,
+            idiocy   =idiocy,
+            shortpath=shortpath
         )
 
     def walk(
             self,
             *,
             topdown: Optional[bool]     = None,
             onerror: Optional[Callable] = None
@@ -1054,15 +1049,15 @@
         @param bufsize
             The buffer size, the length of each copy, default is 64K (if your
             platform is Windows then 1M). Passing -1 turns off buffering.
 
         @return: The parameter `dst` is passed in, without any modification.
         """
         warnings.warn(
-            f'will be deprecated soon, replaced to {self.contents.copy}.',
+            f'will be deprecated soon, replaced to {self.content.copy}.',
             DeprecationWarning
         )
 
     def link(self, dst: Union['File', PathLink], /) -> Union['File', PathLink]:
         """
         Create a hard link to the file, call `os.link` internally.
 
@@ -1085,18 +1080,18 @@
         os.truncate(self.name, length)
 
     def clear(self) -> None:
         self.truncate(0)
 
     def mknod(
             self,
-            mode:          Optional[int]  = None,
+            mode:          int  = None,
             *,
-            device:        Optional[int]  = None,
-            ignore_exists: Optional[bool] = None
+            device:        int  = None,
+            ignore_exists: bool = None
     ) -> None:
         """
         Create the file, call `os.mknod` internally, but if your platform is
         Windows then internally call `open(self.name, 'x')`.
 
         @param mode
             Specify the access permissions of the file, can be a permission
@@ -1112,48 +1107,50 @@
             If the file already exists, call this method will raise
             `FileExistsError`. But, if this parameter is set to True then
             silently skip. Default False.
         """
 
     def mknods(
             self,
-            mode:          Optional[int]  = None,
+            mode:          int  = None,
             *,
-            device:        Optional[int]  = None,
-            ignore_exists: Optional[bool] = None
+            device:        int  = None,
+            ignore_exists: bool = None
     ) -> None:
         """Create the file and all intermediate paths, super version of
         `self.mknod`."""
-        self.dirname.makedirs(mode, exist_ok=True)
+        parentdir = Directory(self.dirname)
+        if not parentdir.exists:
+            parentdir.makedirs(mode)
         self.mknod(mode, device=device, ignore_exists=ignore_exists)
 
     def remove(self, *, ignore_errors: Optional[bool] = None) -> None:
         """
         Remove the file, call `os.remove` internally.
 
         @param ignore_errors
             If the file does not exist will raise `FileNotFoundError`, can set
             this parameter to True to silence the exception. Default False.
         """
 
     def unlink(self) -> None:
-        """Remove the file, like `self.remove`, call `os.unlink` internally."""
+        os.unlink(self.name, dir_fd=self.dir_fd)
 
 
 class Open:
     """
     Open a file and return a file stream (or called handle).
 
     >>> f: BinaryIO = Open('alpha.bin').rb()  # open for reading in binary mode.
     >>> f: TextIO   = Open('alpha.txt').r()   # open for reading in text mode.
 
-    Pass in an instance of `File` (or a file path link) at instantiation time.
-    At instantiation time (do nothing) the file will not be opened, only when
-    you call one of the following methods, the file will be opened (call once,
-    open once), open mode equals method name (where method `rb_plus` equals mode
+    Pass in an instance of `File` (or a file path) at instantiation time. At
+    instantiation time (do nothing) the file will not be opened, only when you
+    call one of the following methods, the file will be opened (call once, open
+    once), open mode equals method name (where method `rb_plus` equals mode
     "rb+").
 
     ============================== IN BINARY MODE ==============================
     | Method  | Description                                                    |
     ----------------------------------------------------------------------------
     | rb      | open to read, if the file does not exist then raise            |
     |         | `FileNotFoundError`                                            |
@@ -1431,27 +1428,27 @@
 
     def __init__(self, file: Union[File, PathLink], /):
         self.file = file
 
     def __bytes__(self) -> bytes:
         return self.read()
 
-    def __ior__(self, content: Union['Content', bytes], /) -> 'Content':
+    def __ior__(self, content: Union['Content', bytes]) -> 'Content':
         self.overwrite(content)
         return self
 
-    def __iadd__(self, content: Union['Content', bytes], /) -> 'Content':
+    def __iadd__(self, content: Union['Content', bytes]) -> 'Content':
         self.append(content)
         return self
 
-    def __eq__(self, content: Union['Content', bytes], /) -> bool:
+    def __eq__(self, content: Union['Content', bytes]) -> bool:
         """Whether the current file content equals the another file content (or
         a bytes object)."""
 
-    def __ne__(self, content: Union['Content', bytes], /) -> bool:
+    def __ne__(self, content: Union['Content', bytes]) -> bool:
         """Whether the current file content is not equal to another file content
         (or a byte object)."""
 
     def __iter__(self) -> Generator:
         """Iterate over the file by line, omitting newline symbol and ignoring
         the last blank line."""
 
@@ -1464,15 +1461,15 @@
     def read(self, size: int = -1, /) -> bytes:
         return Open(self.file).rb().read(size)
 
     def overwrite(self, content: Union['Content', bytes], /) -> None:
         """Overwrite the current file content from another file content (or a
         bytes object)."""
 
-    def append(self, content: Union['Content', bytes], /) -> None:
+    def append(self, content: Union['Content', bytes]) -> None:
         """Append the another file contents (or a bytes object) to the current
         file."""
 
     def copy(
             self,
             dst:     Union['Content', BinaryIO],
             /, *,
@@ -1495,81 +1492,132 @@
         """Truncate the file content to specific length."""
 
     def clear(self) -> None:
         self.truncate(0)
 
 
 def tree(
-        dirpath:    Optional[PathLink] = None,
+        dirpath:   Optional[PathLink] = None,
         /, *,
-        level:      Optional[int]      = None,
-        bottom_up:  Optional[bool]     = None,
-        omit_dir:   Optional[bool]     = None,
-        mysophobia: Optional[bool]     = None,
-        shortpath:  Optional[bool]     = None
+        level:     Optional[int]      = None,
+        bottom_up: Optional[bool]     = None,
+        omit_dir:  Optional[bool]     = None,
+        idiocy:    Optional[bool]     = None,
+        shortpath: Optional[bool]     = None
 ) -> Generator:
     """
     Directory tree generator, recurse the directory to get all subdirectories
     and files.
 
-    @param dirpath
+    @param dirpath:
         Specify a directory path link, recurse this directory on call to get all
         subdirectories and files, default is current working directory (the
         return value of `os.getcwd()`).
 
-    @param level
-        Recursion depth of the directory, default is maximum recursive depth
-        (the return value of `sys.getrecursionlimit()`). An int must be passed
+    @param level:
+        Recursion depth of the directory, default deepest. An int must be passed
         in, any integer less than 1 is considered to be 1, warning passing
         decimals can cause depth confusion.
 
-    @param bottom_up
+    @param bottom_up:
         By default, the outer path is yielded first, from which the inner path
         is yielded. If your requirements are opposite, set this parameter to
         True.
 
-    @param omit_dir
+    @param omit_dir:
         Omit all subdirectories when yielding paths. Default False.
 
-    @param mysophobia
+    @param idiocy:
         By default, if the subpath is a directory then yield a `Directory`
         object, if the subpath is a file then yield a `File` object. If set this
-        parameter to True, directly yield the path link string (or bytes). This
-        parameter is not recommended for use.
+        parameter to True, directly yield the path link string (or bytes). Only
+        SB uses this parameter.
 
-    @param shortpath
+    @param shortpath:
         Yield short path link string, delete the `dirpath` from the left end of
-        the path, used with the parameter `mysophobia`. Default False.
+        the path, used with the parameter `idiocy`. Default False.
     """
 
 
 class SystemPath(Directory, File):
 
     def __init__(
             self,
             root:    Optional[PathLink] = None,
-            /, *,
-            autoabs: Optional[bool]     = None,
-            strict:  Optional[bool]     = None
+            /,
+            autoabs: Optional[bool]     = False,
+            strict:  Optional[bool]     = False
     ):
         super().__init__(
-            '.' if root in (None, '') else b'.' if root == b'' else root,
+            '.' if root == '' else b'.' if root == b'' else root,
             autoabs=autoabs,
             strict =strict
         )
 
 
 class _xe6_xad_x8c_xe7_x90_xaa_xe6_x80_xa1_xe7_x8e_xb2_xe8_x90_x8d_xe4_xba_x91:
-    gpack = globals()
-    gpath = f'{__name__}.i {__name__}'
-    gcode = __import__(gpath, fromlist=...)
-
-    for gname in gpack:
-        try:
-            assert gname[0] != '_'
-            gfunc = getattr(gcode, gname)
-            assert gfunc.__module__ == gpath
-        except (AssertionError, AttributeError):
-            continue
-        gfunc.__module__ = __package__
-        gfunc.__doc__ = gpack[gname].__doc__
-        gpack[gname] = gfunc
+    """  QYYYQLLYYYYYYYQLYYQYYQQQYQQYQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQYL
+        YYYYQYLLQYLLYYQYYYYYYYQQYQYQYQQQQQQQQQQQQQQQQQQQQQQQYYYQQQQQQ
+        QYYYYLPQYLPLYYYLLYYYYYYYYQQQYQQQQQQQQQQQQQQQQQQQQQQQYYYYQQQQQP
+        QYYQLPLQYLLYYQPLLLYYYYYYQYYQYQQQQQQQQQQQQQQYQQQQQQQQYYQYQQQQQQP
+       QYYQYLLYYYLLYQYLLYYYYYYYYQYYQYQYYYQQQQQQQQQQYQQQQQQYQQYQYYQQQQQYP
+      LQYQYYYYQYYYYYQYYYYYYYYYYYYYYYQQYYYYYYYYYQQQQYQQQQQQYQQYQYYQQQQQQ P
+      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYQQYYYQYQYYQQQQYQQQQQQQYQQYQYYQQQQQQ P
+      QYQQYYYYQYYYQQQYYYYYYYYQYQYYYYYQYYYYQYYYQQQQYQQQQQQQYQQYQQYQQQQYYP
+      QYQYYYYYQYYYQQQ PYLLLYP PLYYYYYYQYYYYYYQQQQYYQQQQQQYQQYQQQYQQQQYQ
+      PQQYYYYYQYYQQYQQQQQQQQQQYP        PPLYQYQYQYQLQQQQQYQQYQQQYYQQQYY
+       QQYYYYYQQYQLYQQPQQQQQL QYL           PPYYLYYLQYQQYYQYQQQQYYQPQYL
+       YQYYYYQQQYQ  LYLQQQQQQYQQ           YQQQQQGQQQQQQYQYYQQQQYQPQYQ P
+      L QYYYYQQLYQ   Y YPYQQQQQ           LQQQQQL YQQQQYQQYQYQQYYQQYQP P
+        YYQYYQQ  Q    LQQQQQQY            YQYQQQQQQYYQYLQYQQYQQYYQYQL P
+     Y  LYQLQQPL Y     P  P                QLLQQQQQ Q  PQQQQYQQYYQQL P
+    P   PYQYQQQQPQ                         PQQQQQQY    QQYQYYQQYYQPP
+    L    QQQYQ YYYY              PQ           L  P    LPQYQYYQQLQ P
+    Y   PPQQYYL LYQL                                 PQLQYQQYQYQ  L
+    Y     QQYQPP PYQY        PQ                      Q  QQYQYQYL  L
+    Y     QQYYQ L  QYQP         PLLLLLYL           LQQ LQYYQQQP P L
+     L   PPLQYYQ Y  LQQQ                         LQYQ  QYYYQQ     P
+      L    Q  QYQ  Y  QQPYL                   PQYYYYPPQYYQQQP    L
+       L    L  PQQL   LYQ  PQP             QL PYYYPLQLYQ  QY P   Y
+         P   P    PQQP  QY  QLLQQP   LYYLQ   PQYPQQQP P  QY P   L
+                       PYQYYY           PQ  PQ      L   Q P    L
+              PQYLYYYPQ PLPL             L QY YQYYQYLYQQQ    P
+            PYLLLLLYYYQ P  L    P         PYL  PQYYLLLLLLLQ
+           LYPLLLLLLYYYY   Y  YQY     LLLPPY   LYYYLLLLLLLLY
+           YLLLYLLLLLLYYQ  Q              PQ  YYYLLLLLLLLLLYP
+          YLLLLLLLLLLLLLLYQQ              PYYQYYLLLLLLLLYYYLQ
+          QLLLLLLLLLLLLLLLLLYYQYP        YQYYLLLLLLLLLLLLLLLQ
+          YLLLLLLLLLLLLLLLLLLLYYYLLYYYLLLLLLLLLLLLLLLLLLLLLLYP
+         PLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLLYLYLL
+         LLLLLLLLLLYYLLLLLLYLLLLLLLLLLLLLLLL GQYLPY LLLYLYLLLY
+         QLLLLYYLYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYYLLQ
+         QLLLLLYYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQLYYLLLQ
+        LYLLYLLLQYYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLQYYYYYLYQ
+        YLLLYYLLYQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLYYYYQLLLLY
+        QLLLYYYYYQLLLLLLLLLLLLLLYLLLLLLLLLLLLLLLLLLLLYYYLQLLPLLQ
+        YLYLLQYYYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYLLLLLYYQYYLLLLLQ
+       LYLLLLLYYYQLLYLLLLLLLLLLLLYLYLLYYLLLLYLLLLLLLYYYQQLLLLLLLY
+       YLLLLLLYYYQLLYLLLLLLLYLYLLLLLLLLLLLLLLLLLLLLYYYYQQLYLLLLLQ
+       QLLLYLLLQYQLQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYQYYLLLLLLLY
+       QLLLLLLLLQQYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYQYYLLLLLLLQ
+       QLLLLLLLLLQQYLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLYYYYLLLLLLLLLYL
+       QLLLLYLYYLYQLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLLQYYYLLLLLLLLLQ
+       YLLLLLLLYYLQLLLLLLLLLLLLLLLLLLLLLLLLLYLLLLLLLLYQYYLLLLLLLLLQ
+       QLLLLLYLYYYYLLLLLPLLLLLLLYLYLLLLLLLLLLLLLLLLLLLQYYLLLLLLLLYP
+       YYLYYLLYYYQLLLLLLLLYLLLLLLLLLLLLLLLLLLLLLLYLYLLYQYYLLLLLLYL
+        QLLLLLLYQYLLLLLLLLLLLLLLLLLLLLLYYLYLLLLLLLLLLLYQQQQQQQLYL  """
+    gpath = f'{__name__}.gqylpy {__name__}'
+    __import__(gpath)
+
+    gpack = sys.modules[__name__]
+    gcode = globals()[f'gqylpy {__name__}']
+
+    for gname in globals():
+        if gname[0] != '_':
+            try:
+                gfunc = getattr(gcode, gname)
+                if gfunc.__module__ is gpath:
+                    gfunc.__module__ = __package__
+                    gfunc.__doc__ = getattr(gpack, gname).__doc__
+                    setattr(gpack, gname, gfunc)
+            except AttributeError:
+                pass
```

## Comparing `systempath/i systempath.py` & `systempath/gqylpy systempath.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,34 +28,31 @@
     getcwd,  getcwdb
 )
 
 if sys.platform != 'win32':
     from os import mknod, chown, system, popen
 
     if sys.platform == 'linux':
-        try:
-            from os import getxattr, setxattr, listxattr, removexattr
-        except ImportError:
-            def getxattr(*a, **kw): raise NotImplementedError
-            setxattr = listxattr = removexattr = getxattr
+        from os import getxattr, setxattr, listxattr, removexattr
+
     try:
         from os import lchmod, lchown, chflags, lchflags
     except ImportError:
         def lchmod(*a, **kw): raise NotImplementedError
         lchown = chflags = lchflags = lchmod
     try:
         from pwd import getpwuid
         from grp import getgrgid
     except ModuleNotFoundError:
         def getpwuid(_): raise NotImplementedError
         getgrgid = getpwuid
 
-    __read_bufsize__ = 1024 * 64
+    READ_BUFFER_SIZE = 1024 * 64
 else:
-    __read_bufsize__ = 1024 * 1024
+    READ_BUFFER_SIZE = 1024 * 1024
 
 from os.path import (
     basename, dirname,    abspath,  realpath,   relpath,
     normpath, expanduser, expandvars,
     join,     split,      splitext, splitdrive,
     isabs,    exists,     isdir,    isfile,     islink,  ismount,
     getctime, getmtime,   getatime, getsize
@@ -66,22 +63,22 @@
 from pathlib import _ignore_error
 
 from stat import S_ISDIR, S_ISREG, S_ISBLK, S_ISCHR, S_ISFIFO
 
 from _io import (
     FileIO, BufferedReader, BufferedWriter, BufferedRandom, TextIOWrapper,
     _BufferedIOBase     as BufferedIOBase,
-    DEFAULT_BUFFER_SIZE as __io_bufsize__
+    DEFAULT_BUFFER_SIZE as IO_BUFFER_SIZE
 )
 
 from hashlib import md5
 
 from typing import (
-    TypeVar, Type, Literal, Optional, Union, Tuple, List, Final, Callable,
-    Generator, Iterator, Iterable, NoReturn, Any
+    TypeVar, Literal, Optional, Type, Union, Tuple, List, Callable, Generator,
+    Iterator, Iterable, NoReturn, Any
 )
 
 import gqylpy_exception as ge
 
 PathLink = BytesOrStr = Union[bytes, str]
 Closure = TypeVar('Closure', bound=Callable)
 
@@ -98,16 +95,14 @@
     'replace',
     'surrogateescape',
     'xmlcharrefreplace',
     'backslashreplace',
     'namereplace'
 ]
 
-__unique__: Final = object()
-
 
 class MasqueradeClass(type):
     # Masquerade one class as another.
     # Warning, masquerade the class can cause unexpected problems, use caution.
     __module__ = 'builtins'
 
     def __new__(mcs, __name__: str, __bases__: tuple, __dict__: dict):
@@ -124,15 +119,14 @@
             raise TypeError('"__masquerade_class__" is not a class.')
 
         cls = type.__new__(
             mcs, __masquerade_class__.__name__, __bases__, __dict__
         )
 
         mcs.__name__     = type.__name__
-        mcs.__qualname__ = type.__qualname__
         cls.__module__   = __masquerade_class__.__module__
         cls.__qualname__ = __masquerade_class__.__qualname__
 
         if getattr(builtins, __masquerade_class__.__name__, None) is \
                 __masquerade_class__:
             setattr(builtins, __name__, cls)
 
@@ -155,58 +149,52 @@
                 f'cannot set "{name}" attribute '
                 f'of immutable type "{cls.__name__}".'
             )
         type.__setattr__(cls, name, value)
 
     def __delattr__(cls, name: str) -> NoReturn:
         raise ge.DeleteAttributeError(
-            f'cannot delete "{name}" attribute '
+            f'cannot execute operation to delete attribute '
             f'of immutable type "{cls.__name__}".'
         )
 
 
 class ReadOnly(metaclass=ReadOnlyMode):
     # Disallow modifying the attributes of the instances externally.
-
-    # __dict__ = {}
-    # Tamper with attribute `__dict__` to avoid modifying its subclass instance
-    # attribute externally, but the serious problem is that it cannot
-    # deserialize its subclass instance after tampering. Stop tampering for the
-    # moment, the solution is still in the works.
+    __dict__ = {}
 
     def __setattr__(self, name: str, value: Any) -> None:
         if sys._getframe().f_back.f_globals['__name__'] != __name__ and not \
-                (isinstance(self, File) and name in ('content', 'contents')):
+                (isinstance(self, File) or name not in ('content', 'contents')):
             raise ge.SetAttributeError(
                 f'cannot set "{name}" attribute in instance '
                 f'of immutable type "{self.__class__.__name__}".'
             )
         object.__setattr__(self, name, value)
 
     def __delattr__(self, name: str) -> None:
         if not isinstance(self, File) or name != 'content':
             raise ge.DeleteAttributeError(
-                f'cannot delete "{name}" attribute in instance '
-                f'of immutable type "{self.__class__.__name__}".'
+                f'cannot execute operation to delete attribute in instance '
+                f'of immutable type "{File.__name__}".'
             )
         object.__delattr__(self, name)
 
 
 def dst2abs(func: Callable) -> Closure:
     # If the destination path is relative and is a single name, the parent path
     # of the source is used as the parent path of the destination instead of
     # using the current working directory, different from the traditional way.
     @functools.wraps(func)
     def core(path: 'Path', dst: PathLink) -> PathLink:
         try:
             singlename: bool = basename(dst) == dst
         except TypeError:
             raise ge.DestinationPathTypeError(
-                'destination path type can only be "bytes" or "str", '
-                f'not "{dst.__class__.__name__}".'
+                'destination path type can only be "bytes" or "str".'
             ) from None
         if singlename:
             try:
                 dst: PathLink = join(dirname(path.name), dst)
             except TypeError:
                 dst: PathLink = join(dirname(
                     path.name.decode() if dst.__class__ is str
@@ -261,28 +249,24 @@
     except ValueError:
         # Non-encodable path
         return False
 
 
 class Path(ReadOnly):
 
-    def __new__(
-            cls, name: PathLink = __unique__, /, strict: bool = False, **kw
-    ):
-        # Compatible object deserialization.
-        if name is not __unique__:
-            if name.__class__ not in (bytes, str):
-                raise ge.NotAPathError(
-                    'path type can only be "bytes" or "str", '
-                    f'not "{name.__class__.__name__}".'
-                )
-            if strict and not exists(name):
-                raise ge.SystemPathNotFoundError(
-                    f'system path {repr(name)} does not exist.'
-                )
+    def __new__(cls, name: PathLink, /, strict: bool = False, **kw):
+        if name.__class__ not in (bytes, str):
+            raise ge.NotAPathError(
+                'path type can only be "bytes" or "str", '
+                f'not "{name.__class__.__name__}".'
+            )
+        if strict and not exists(name):
+            raise ge.SystemPathNotFoundError(
+                f'system path {repr(name)} does not exist.'
+            )
         return object.__new__(cls)
 
     def __init__(
             self,
             name:            PathLink,
             /, *,
             autoabs:         bool          = False,
@@ -292,45 +276,20 @@
     ):
         self.name            = abspath(name) if autoabs else name
         self.strict          = strict
         self.dir_fd          = dir_fd
         self.follow_symlinks = follow_symlinks
 
     def __str__(self) -> str:
-        return self.name if self.name.__class__ is str else repr(self.name)
+        return self.name if self.name.__class__ is str else self.name.decode()
 
     def __repr__(self) -> str:
         return f'<{__package__}.{self.__class__.__name__} ' \
                f'name={repr(self.name)}>'
 
-    def __bytes__(self) -> bytes:
-        return self.name if self.name.__class__ is bytes else self.name.encode()
-
-    def __eq__(self, other: ['Path', PathLink], /) -> bool:
-        if isinstance(other, Path):
-            other_type   = other.__class__
-            other_path   = abspath(other.name)
-            other_dir_fd = other.dir_fd
-        elif other.__class__ in (bytes, str):
-            other_type   = Path
-            other_path   = abspath(other)
-            other_dir_fd = None
-        else:
-            return False
-
-        if self.name.__class__ is not other_path.__class__:
-            other_path = other_path.encode() \
-                if other_path.__class__ is str else other_path.decode()
-
-        return any((
-            self.__class__ == other_type,
-            self.__class__ in (Path, SystemPath),
-            other_type     in (Path, SystemPath)
-        )) and abspath(self.name) == other_path and self.dir_fd == other_dir_fd
-
     @property
     def basename(self) -> BytesOrStr:
         return basename(self.name)
 
     @property
     def dirname(self) -> 'Directory':
         return Directory(
@@ -594,31 +553,31 @@
         def chflags(self, flags: int) -> None:
             chflags(self.name, flags, follow_symlinks=self.follow_symlinks)
 
         def lchflags(self, flags: int) -> None:
             lchflags(self.name, flags)
 
         def chattr(self, operator: Literal['+', '-', '='], attrs: str) -> None:
-            warnings.warn(
+            warnings.warn(UserWarning(
                 'implementation of method `chattr` is to directly call the '
                 'system command `chattr`, so this is very unreliable.'
-            , stacklevel=2)
+            ))
             if operator not in ('+', '-', '='):
                 raise ge.ChattrError(
                     f'unsupported operation "{operator}", only "+", "-" or "=".'
                 )
             c: str = f'chattr {operator}{attrs} {self.name}'
             if system(f'sudo {c} &>/dev/null'):
                 raise ge.ChattrError(c)
 
         def lsattr(self) -> str:
-            warnings.warn(
+            warnings.warn(UserWarning(
                 'implementation of method `lsattr` is to directly call the '
                 'system command `lsattr`, so this is very unreliable.'
-            , stacklevel=2)
+            ))
             c: str = f'lsattr {self.name}'
             attrs: str = popen(
                 "sudo %s 2>/dev/null | awk '{print $1}'" % c
             ).read()[:-1]
             if len(attrs) != 16:
                 raise ge.LsattrError(c)
             return attrs
@@ -675,26 +634,30 @@
         if strict and not isdir(name):
             raise NotADirectoryError(
                 f'system path {repr(name)} is not a directory.'
             )
 
         return instance
 
+    def __getattr__(self, name: str) -> Any:
+        try:
+            return self[name]
+        except ge.SystemPathNotFoundError:
+            raise AttributeError(
+                f"'{self.__class__.__name__}' object has no attribute '{name}'"
+            ) from None
+
     @joinpath
-    def __getitem__(
-            self, name: PathLink
-    ) -> Union['SystemPath', 'Directory', 'File', Path]:
+    def __getitem__(self, name: PathLink) -> Union['Path', 'Directory', 'File']:
         if self.strict:
             if isdir(name):
                 return Directory(name, strict=self.strict)
             if isfile(name):
                 return File(name)
-            if exists(name):
-                return Path(name)
-            else:
+            if not exists(name):
                 raise ge.SystemPathNotFoundError(
                     f'system path {repr(name)} does not exist.'
                 )
         else:
             return SystemPath(name)
 
     @joinpath
@@ -716,36 +679,36 @@
         )
 
     @property
     def subpaths(self) -> Generator:
         return self.__iter__()
 
     @property
-    def subpath_names(self) -> List[BytesOrStr]:
+    def subpaths_names(self) -> List[BytesOrStr]:
         return listdir(self.name)
 
     def scandir(self) -> Iterator:
         return scandir(self.name)
 
     def tree(
             self,
             *,
-            level:      int  = sys.getrecursionlimit(),
-            bottom_up:  bool = False,
-            omit_dir:   bool = False,
-            mysophobia: bool = False,
-            shortpath:  bool = False
+            level:     int  = sys.getrecursionlimit(),
+            bottom_up: bool = False,
+            omit_dir:  bool = False,
+            idiocy:    bool = False,
+            shortpath: bool = False
     ) -> Generator:
         return tree(
             self.name,
-            level     =level,
-            bottom_up =bottom_up,
-            omit_dir  =omit_dir,
-            mysophobia=mysophobia,
-            shortpath =shortpath
+            level    =level,
+            bottom_up=bottom_up,
+            omit_dir =omit_dir,
+            idiocy   =idiocy,
+            shortpath=shortpath
         )
 
     def walk(
             self, *, topdown: bool = True, onerror: Optional[Callable] = None
     ) -> Iterator[Tuple[PathLink, List[BytesOrStr], List[BytesOrStr]]]:
         return walk(
             self.name,
@@ -813,17 +776,15 @@
 
     def chdir(self) -> None:
         chdir(self.name)
 
 
 class File(Path):
 
-    def __new__(
-            cls, name: PathLink = __unique__, /, strict: bool = False, **kw
-    ):
+    def __new__(cls, name: PathLink, /, strict: bool = False, **kw):
         instance = Path.__new__(cls, name, strict=strict, **kw)
 
         if strict and not isfile(name):
             raise ge.NotAFileError(f'system path {repr(name)} is not a file.')
 
         return instance
 
@@ -870,15 +831,15 @@
     def copy(self, dst: PathLink, /) -> None:
         copyfile(self.name, dst, follow_symlinks=self.follow_symlinks)
 
     def copycontent(
             self,
             other:   Union['File', FileIO],
             /, *,
-            bufsize: int                   = __read_bufsize__
+            bufsize: int                   = READ_BUFFER_SIZE
     ) -> Union['File', FileIO]:
         write, read = (
             FileIO(other.name, 'wb') if isinstance(other, File) else other
         ).write, FileIO(self.name).read
 
         while True:
             content = read(bufsize)
@@ -955,15 +916,15 @@
         unlink(self.name, dir_fd=self.dir_fd)
 
     def md5(self, salting: bytes = b'') -> str:
         m5 = md5(salting)
         read = FileIO(self.name).read
 
         while True:
-            content = read(__read_bufsize__)
+            content = read(READ_BUFFER_SIZE)
             if not content:
                 break
             m5.update(content)
 
         return m5.hexdigest()
 
 
@@ -1004,26 +965,28 @@
         methods = object.__dir__(self)
         methods.remove('__modes__')
         methods.remove('__pass__')
         methods.remove('__path__')
         methods += self.__modes__
         return methods
 
-    def __repr__(self) -> str:
+    def __str__(self) -> str:
         return f'<{__package__}.{self.__class__.__name__} ' \
                f'file={repr(self.__path__)}>'
 
+    __repr__ = __str__
+
     @property
     def __path__(self) -> PathLink:
         return self.file.name if isinstance(self.file, File) else self.file
 
     def __pass__(self, buffer: Type[BufferedIOBase], mode: OpenMode) -> Closure:
         def init_buffer_instance(
                 *,
-                bufsize:        int                            = __io_bufsize__,
+                bufsize:        int                            = IO_BUFFER_SIZE,
                 encoding:       Optional[str]                       = None,
                 errors:         Optional[EncodingErrorHandlingMode] = None,
                 newline:        Optional[str]                       = None,
                 line_buffering: bool                                = False,
                 write_through:  bool                                = False,
                 opener:         Optional[Callable[[PathLink, int], int]] = None
         ) -> Union[BufferedIOBase, TextIOWrapper]:
@@ -1054,24 +1017,24 @@
 
     def __dir__(self) -> Iterable[str]:
         return object.__dir__(self)
 
     def __bytes__(self) -> bytes:
         return self.rb().read()
 
-    def __ior__(self, content: Union['Content', bytes], /) -> 'Content':
+    def __ior__(self, content: Union['Content', bytes]) -> 'Content':
         if isinstance(content, Content):
             if abspath(content.__path__) == abspath(self.__path__):
                 raise ge.IsSameFileError(
                     'source and destination cannot be the same, '
                     f'path "{abspath(self.__path__)}".'
                 )
             read, write = content.rb().read, self.wb().write
             while True:
-                content = read(__read_bufsize__)
+                content = read(READ_BUFFER_SIZE)
                 if not content:
                     break
                 write(content)
         # Beware of original data loss due to write failures (the `content` type
         # error).
         elif content.__class__ is bytes:
             self.wb().write(content)
@@ -1079,60 +1042,63 @@
             raise TypeError(
                 'content type to be written can only be '
                 f'"{__package__}.{Content.__name__}" or "bytes", '
                 f'not "{content.__class__.__name__}".'
             )
         return self
 
-    def __iadd__(self, content: Union['Content', bytes], /) -> 'Content':
+    def __iadd__(self, content: Union['Content', bytes]) -> 'Content':
         if isinstance(content, Content):
             read, write = content.rb().read, self.ab().write
             while True:
-                content = read(__read_bufsize__)
+                content = read(READ_BUFFER_SIZE)
                 if not content:
                     break
                 write(content)
         elif content.__class__ is bytes:
             self.ab().write(content)
         else:
             raise TypeError(
                 'content type to be appended can only be '
                 f'"{__package__}.{Content.__name__}" or "bytes", '
                 f'not "{content.__class__.__name__}".'
             )
         return self
 
-    def __eq__(self, content: Union['Content', bytes], /) -> bool:
+    def __eq__(self, content: Union['Content', bytes]) -> bool:
         if isinstance(content, Content):
             read1, read2 = self.rb().read, content.rb().read
             while True:
-                content1 = read1(__read_bufsize__)
-                content2 = read2(__read_bufsize__)
+                content1 = read1(READ_BUFFER_SIZE)
+                content2 = read2(READ_BUFFER_SIZE)
                 if content1 == content2 == b'':
                     return True
                 if content1 != content2:
                     return False
         elif content.__class__ is bytes:
-            start, end = 0, __read_bufsize__
+            start, end = 0, READ_BUFFER_SIZE
             read1 = self.rb().read
             while True:
-                content1 = read1(__read_bufsize__)
+                content1 = read1(READ_BUFFER_SIZE)
                 if content1 == content[start:end] == b'':
                     return True
                 if content1 != content[start:end]:
                     return False
-                start += __read_bufsize__
-                end   += __read_bufsize__
+                start += READ_BUFFER_SIZE
+                end   += READ_BUFFER_SIZE
         else:
             raise TypeError(
                 'content type to be equality judgment operation can only be '
                 f'"{__package__}.{Content.__name__}" or "bytes", '
                 f'not "{content.__class__.__name__}".'
             )
 
+    def __ne__(self, content: Union['Content', bytes]) -> bool:
+        return not self.__eq__(content)
+
     def __iter__(self) -> Generator:
         return (line.rstrip(b'\r\n') for line in self.rb())
 
     def __len__(self) -> int:
         return getsize(self.__path__)
 
     def __bool__(self) -> bool:
@@ -1140,22 +1106,22 @@
 
     def read(self, size: int = -1, /) -> bytes:
         return self.rb().read(size)
 
     def overwrite(self, content: Union['Content', bytes], /) -> None:
         self.__ior__(content)
 
-    def append(self, content: Union['Content', bytes], /) -> None:
+    def append(self, content: Union['Content', bytes]) -> None:
         self.__iadd__(content)
 
     def copy(
             self,
             other:   Union['Content', FileIO],
             /, *,
-            bufsize: int                      = __read_bufsize__
+            bufsize: int                      = READ_BUFFER_SIZE
     ) -> None:
         write = (other.ab() if isinstance(other, Content) else other).write
         read  = self.rb().read
 
         while True:
             content = read(bufsize)
             if not content:
@@ -1169,124 +1135,120 @@
         truncate(self.__path__, 0)
 
     def md5(self, salting: bytes = b'') -> str:
         m5 = md5(salting)
         read = self.rb().read
 
         while True:
-            content = read(__read_bufsize__)
+            content = read(READ_BUFFER_SIZE)
             if not content:
                 break
             m5.update(content)
 
         return m5.hexdigest()
 
 
 def tree(
-        dirpath:    Optional[PathLink] = None,
+        dirpath:   Optional[PathLink] = None,
         /, *,
-        level:      int                = None,
-        bottom_up:  bool               = False,
-        omit_dir:   bool               = False,
-        mysophobia: bool               = False,
-        shortpath:  bool               = False
+        level:     int                = sys.getrecursionlimit(),
+        bottom_up: bool               = False,
+        omit_dir:  bool               = False,
+        idiocy:    bool               = False,
+        shortpath: bool               = False
 ) -> Generator:
     if dirpath == b'':
         dirpath: bytes = getcwdb()
     elif dirpath in (None, ''):
         dirpath: str = getcwd()
 
     return __tree__(
         dirpath,
-        level     =level or sys.getrecursionlimit(),
-        bottom_up =bottom_up,
-        omit_dir  =omit_dir,
-        root      =dirpath,
-        nullchar  =b'' if dirpath.__class__ is bytes else '',
-        mysophobia=mysophobia,
-        shortpath =shortpath
+        level    =level,
+        bottom_up=bottom_up,
+        omit_dir =omit_dir,
+        root     =dirpath,
+        nullchar =b'' if dirpath.__class__ is bytes else '',
+        idiocy   =idiocy,
+        shortpath=shortpath
     )
 
 
 def __tree__(
-        dirpath:    PathLink,
+        dirpath:   PathLink,
         /, *,
-        level:      int,
-        bottom_up:  bool,
-        omit_dir:   bool,
-        mysophobia: bool,
-        shortpath:  bool,
-        root:       PathLink,
-        nullchar:   BytesOrStr
+        level:     int,
+        bottom_up: bool,
+        omit_dir:  bool,
+        idiocy:    bool,
+        shortpath: bool,
+        root:      PathLink,
+        nullchar:  BytesOrStr
 ) -> Generator:
     for name in listdir(dirpath):
         path: PathLink = join(dirpath, name)
         is_dir: bool = isdir(path)
 
         if bottom_up:
             if level > 1 and is_dir:
                 yield from __tree__(
                     path,
-                    level     =level - 1,
-                    bottom_up =bottom_up,
-                    omit_dir  =omit_dir,
-                    mysophobia=mysophobia,
-                    shortpath =shortpath,
-                    root      =root,
-                    nullchar  =nullchar
+                    level    =level - 1,
+                    bottom_up=bottom_up,
+                    omit_dir =omit_dir,
+                    idiocy   =idiocy,
+                    shortpath=shortpath,
+                    root     =root,
+                    nullchar =nullchar
                 )
             if not is_dir or not omit_dir:
-                if mysophobia:
+                if idiocy:
                     if shortpath:
                         path: PathLink = path.replace(root, nullchar)
                         if path[0] in (47, 92, '/', '\\'):
                             path: PathLink = path[1:]
                     yield path
                 else:
                     yield Directory(path) if is_dir else \
                         File(path) if isfile(path) else Path(path)
         else:
             if not is_dir or not omit_dir:
-                if mysophobia:
+                if idiocy:
                     if not shortpath:
                         yield path
                     else:
                         shortpath: PathLink = path.replace(root, nullchar)
                         if shortpath[0] in (47, 92, '/', '\\'):
                             shortpath: PathLink = shortpath[1:]
                         yield shortpath
                 else:
                     yield Directory(path) if is_dir else \
                         File(path) if isfile(path) else Path(path)
             if level > 1 and is_dir:
                 yield from __tree__(
                     path,
-                    level     =level - 1,
-                    bottom_up =bottom_up,
-                    omit_dir  =omit_dir,
-                    mysophobia=mysophobia,
-                    shortpath =shortpath,
-                    root      =root,
-                    nullchar  =nullchar
+                    level    =level - 1,
+                    bottom_up=bottom_up,
+                    omit_dir =omit_dir,
+                    idiocy   =idiocy,
+                    shortpath=shortpath,
+                    root     =root,
+                    nullchar =nullchar
                 )
 
 
 class SystemPath(Directory, File):
     __new__ = Directory.__new__
 
     def __init__(
             self,
-            root:            PathLink      = '.',
-            /, *,
-            autoabs:         bool          = False,
-            strict:          bool          = False,
-            dir_fd:          Optional[int] = None,
-            follow_symlinks: bool          = True
+            root:    PathLink = '.',
+            /,
+            autoabs: bool     = False,
+            strict:  bool     = False
     ):
         Path.__init__(
             self,
             '.' if root == '' else b'.' if root == b'' else root,
-            autoabs        =autoabs,
-            strict         =strict,
-            dir_fd         =dir_fd,
-            follow_symlinks=follow_symlinks
+            autoabs=autoabs,
+            strict=strict
         )
```

## Comparing `systempath-1.0.9.dist-info/LICENSE` & `systempath-1.0a8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `systempath-1.0.9.dist-info/METADATA` & `systempath-1.0a8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systempath
-Version: 1.0.9
+Version: 1.0a8
 Summary: Operating system paths and files.
 Home-page: http://gqylpy.com
 Author: 竹永康
 Author-email: <gqylpy@outlook.com>
 License: Apache 2.0
 Project-URL: Source, https://github.com/gqylpy/systempath
 Classifier: Environment :: Web Environment
@@ -18,25 +18,25 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: gqylpy-exception (>=2.0.1)
+Requires-Dist: gqylpy-exception (<2.0,>=1.3.2)
 
 [<img alt="LOGO" src="http://www.gqylpy.com/static/img/favicon.ico" height="21" width="21"/>](http://www.gqylpy.com)
 [![Release](https://img.shields.io/github/release/gqylpy/systempath.svg?style=flat-square")](https://github.com/gqylpy/systempath/releases/latest)
 [![Python Versions](https://img.shields.io/pypi/pyversions/systempath)](https://pypi.org/project/systempath)
 [![License](https://img.shields.io/pypi/l/systempath)](https://github.com/gqylpy/systempath/blob/master/LICENSE)
 [![Downloads](https://pepy.tech/badge/systempath/month)](https://pepy.tech/project/systempath)
 
 # systempath
 
-> (OOP) Operating system paths and files.  
+> Operating system paths and files.  
 > Let Python operating system paths and files become Simple, Simpler, Simplest, Humanization, Unification, Flawless.
 
 <kbd>pip3 install systempath</kbd>
 
 ```python
 >>> from systempath import SystemPath, Directory, File
```

## Comparing `systempath-1.0.9.dist-info/RECORD` & `systempath-1.0a8.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-systempath/__init__.py,sha256=1YH_Cqxb8t_mQ-tS6bxz-0eCe5_fsOZ2yWUZ4DovRd8,63906
-systempath/i systempath.py,sha256=J3Cfc7HgXMzhHFuWJTgGOerSCgLauOrPST70jwfKuCA,41175
-systempath-1.0.9.dist-info/LICENSE,sha256=bLEM1yfc38Qf3r9KdVo81p4z2KLd41HT8sSzZ2DZQc4,11389
-systempath-1.0.9.dist-info/METADATA,sha256=XgPFt5AMg6jyQpgku-WSZyf3MrHcsySws7cF31dlRDc,2084
-systempath-1.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-systempath-1.0.9.dist-info/top_level.txt,sha256=i7q5WQPfisH1WfpASAiL4dBCNaexemSOC8lUawWke_A,11
-systempath-1.0.9.dist-info/RECORD,,
+systempath/__init__.py,sha256=nftrjXqzpOiOtgrLZLGNZNQAdnwToRQD1ag9yToaDZo,66968
+systempath/gqylpy systempath.py,sha256=FXzn3q_YamglRoEs-nffHH25XPNiz-kFQPX8jRa0dZQ,39467
+systempath-1.0a8.dist-info/LICENSE,sha256=bLEM1yfc38Qf3r9KdVo81p4z2KLd41HT8sSzZ2DZQc4,11389
+systempath-1.0a8.dist-info/METADATA,sha256=rYr5x214HbuVE0ZaPf2_54B8-VJ30M0QBrgCt5VLMsU,2083
+systempath-1.0a8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+systempath-1.0a8.dist-info/top_level.txt,sha256=i7q5WQPfisH1WfpASAiL4dBCNaexemSOC8lUawWke_A,11
+systempath-1.0a8.dist-info/RECORD,,
```

