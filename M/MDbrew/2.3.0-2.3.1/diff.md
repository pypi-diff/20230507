# Comparing `tmp/MDbrew-2.3.0.tar.gz` & `tmp/MDbrew-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MDbrew-2.3.0.tar", last modified: Fri May  5 11:52:39 2023, max compression
+gzip compressed data, was "MDbrew-2.3.1.tar", last modified: Sun May  7 05:37:54 2023, max compression
```

## Comparing `MDbrew-2.3.0.tar` & `MDbrew-2.3.1.tar`

### file list

```diff
@@ -1,37 +1,39 @@
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.305372 MDbrew-2.3.0/
--rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-05 06:22:51.000000 MDbrew-2.3.0/MANIFEST.in
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.302404 MDbrew-2.3.0/MDbrew/
--rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-05 11:52:26.000000 MDbrew-2.3.0/MDbrew/__init__.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303470 MDbrew-2.3.0/MDbrew/analysis/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/msd.py
--rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/rdf.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303723 MDbrew-2.3.0/MDbrew/application/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/application/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     9705 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/application/brewcp2k.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.304063 MDbrew-2.3.0/MDbrew/main/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     4770 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/brewery.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.304660 MDbrew-2.3.0/MDbrew/main/filetype/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)      842 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/lmps.py
--rw-r--r--   0 minu       (501) staff       (20)      715 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/pdb.py
--rw-r--r--   0 minu       (501) staff       (20)     1309 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/vasp.py
--rw-r--r--   0 minu       (501) staff       (20)      425 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/xyz.py
--rw-r--r--   0 minu       (501) staff       (20)     1170 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/opener.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.305263 MDbrew-2.3.0/MDbrew/tool/
--rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/__init__.py
--rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/colorfont.py
--rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/decorator.py
--rw-r--r--   0 minu       (501) staff       (20)      752 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/doctor.py
--rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/spacer.py
-drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303100 MDbrew-2.3.0/MDbrew.egg-info/
--rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)      684 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/SOURCES.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/dependency_links.txt
--rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-05 11:52:02.000000 MDbrew-2.3.0/MDbrew.egg-info/not-zip-safe
--rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/top_level.txt
--rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-05 11:52:39.305464 MDbrew-2.3.0/PKG-INFO
--rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-05 06:22:51.000000 MDbrew-2.3.0/requirement.txt
--rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-05 11:52:39.305722 MDbrew-2.3.0/setup.cfg
--rw-r--r--   0 minu       (501) staff       (20)      653 2023-05-05 11:51:29.000000 MDbrew-2.3.0/setup.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.150186 MDbrew-2.3.1/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-05 06:22:51.000000 MDbrew-2.3.1/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.146615 MDbrew-2.3.1/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-07 05:37:43.000000 MDbrew-2.3.1/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.147764 MDbrew-2.3.1/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.148005 MDbrew-2.3.1/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     9705 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/application/brewcp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.148429 MDbrew-2.3.1/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     5302 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.149316 MDbrew-2.3.1/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      896 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/gro.py
+-rw-r--r--   0 minu       (501) staff       (20)      860 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      777 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     4172 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/trr.py
+-rw-r--r--   0 minu       (501) staff       (20)     1370 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)      486 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1163 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/main/opener.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.150037 MDbrew-2.3.1/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      756 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-07 05:36:55.000000 MDbrew-2.3.1/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-07 05:37:54.147346 MDbrew-2.3.1/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      740 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-07 05:37:16.000000 MDbrew-2.3.1/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-07 05:37:54.000000 MDbrew-2.3.1/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-07 05:37:54.150258 MDbrew-2.3.1/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-05 06:22:51.000000 MDbrew-2.3.1/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-07 05:37:54.150480 MDbrew-2.3.1/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      653 2023-05-07 05:37:07.000000 MDbrew-2.3.1/setup.py
```

### Comparing `MDbrew-2.3.0/MDbrew/analysis/msd.py` & `MDbrew-2.3.1/MDbrew/analysis/msd.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew/analysis/rdf.py` & `MDbrew-2.3.1/MDbrew/analysis/rdf.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew/application/brewcp2k.py` & `MDbrew-2.3.1/MDbrew/application/brewcp2k.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew/main/brewery.py` & `MDbrew-2.3.1/MDbrew/main/brewery.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,34 +2,41 @@
 import numpy as np
 import pandas as pd
 from .opener import Opener
 from .filetype.lmps import lmpsOpener
 from .filetype.pdb import pdbOpener
 from .filetype.vasp import vaspOpener
 from .filetype.xyz import xyzOpener
+from .filetype.trr import trrOpener
 from ..tool.colorfont import color
 from ..tool.decorator import color_print_verbose
 
 
 class Brewery(object):
-    __support_opener__ = {"auto": None, "pdb": pdbOpener, "xyz": xyzOpener, "vasp": vaspOpener, "lmps": lmpsOpener}
+    __support_opener__: dict["str":Opener] = {
+        "auto": None,
+        "pdb": pdbOpener,
+        "xyz": xyzOpener,
+        "vasp": vaspOpener,
+        "lmps": lmpsOpener,
+        "trr": trrOpener,
+    }
     __print_option__ = {
         "brewery": f" #OPEN  {color.font_yellow}Brewery {color.reset}",
         "b_brewing": f" #BREW  {color.font_yellow}Some...  {color.reset}",
         "b_coords": f" #BREW  {color.font_yellow}Coords     {color.reset}",
         "b_atominfo": f" #BREW  {color.font_yellow}Atom Info  {color.reset}",
     }
 
-    def __init__(self, path: str, fmt: str = "auto", what: str = None, verbose: bool = True):
-        self._what = what
-        self._verbose = verbose
-        self._path = self._check_path(path=path)
-        self.fmt = self._check_fmt(fmt=fmt)
-        self._opener = self._init_opener()
-        self._set_atom_info(verbose=verbose)
+    def __init__(self, trj_file: str, fmt: str = "auto", *args, **kwrgs):
+        self._what = kwrgs.pop("what", None)
+        self._path = self._check_path(path=trj_file, **kwrgs)
+        self._fmt = self._check_fmt(fmt=fmt)
+        self._opener = self._init_opener(**kwrgs)
+        self._set_atom_info(verbose=kwrgs.pop("verbose", True))
         self._data = None
         self._coords = None
 
     def __str__(self) -> str:
         LINE_WIDTH = 60
         sep_line = "=" * LINE_WIDTH
         print("")
@@ -44,22 +51,24 @@
         print(sep_line)
         return f"\t    @CopyRight by  {color.font_blue}minu928@snu.ac.kr{color.reset}\n"
 
     @property
     def box_size(self):
         return self._opener.box_size
 
-    def set_box_size(self, box_size):
+    @box_size.setter
+    def box_size(self, box_size):
         self._opener.box_size = box_size
 
     @property
     def columns(self):
         return self._opener.column
 
-    def set_columns(self, colums):
+    @columns.setter
+    def columns(self, colums):
         self._opener.column = colums
 
     @property
     def coords(self):
         return self.brew(cols=["x", "y", "z"], verbose=False)
 
     @property
@@ -81,35 +90,41 @@
         data = data.loc[:, cols] if cols is not None else data
         return data.to_numpy().astype(dtype=dtype)
 
     def reset(self):
         self._opener.reset()
 
     def order(self, what: str = None):
-        return Brewery(path=self._path, fmt=self.fmt, what=what)
+        return Brewery(trj_file=self._path, fmt=self._fmt, what=what)
 
     @color_print_verbose(name=__print_option__["brewery"])
     def _set_atom_info(self, verbose: bool = True):
         atom_brew_data = self.brew(cols=self._opener._atom_keyword, dtype=str, verbose=False)
         self.atom_info = np.unique(atom_brew_data, return_counts=True)
         self.atom_kind = self.atom_info[0]
         self.atom_num = np.sum(self.atom_info[1])
 
-    def _init_opener(self) -> Opener:
-        return self.__support_opener__[self.fmt](path=self._path)
+    def _init_opener(self, **kwrgs) -> Opener:
+        trj_opener: Opener = self.__support_opener__[self._fmt]
+        if trj_opener.is_require_gro:
+            gro_file = kwrgs.pop("gro_file", None)
+            assert gro_file is not None, f"{self._fmt} format require gro file, plz input with gro_file='some_gro'"
+            return trj_opener(path=self._path, gro=gro_file)
+        else:
+            return trj_opener(path=self._path)
 
     def _check_fmt(self, fmt: str):
         fmt_list = list(self.__support_opener__.keys())
         assert fmt in fmt_list, f"fmt should be in {fmt_list}"
         if fmt == "auto":
             file_name = self._path.split("/")[-1]
             fmt = file_name.split(".")[-1]
         return fmt
 
-    def _check_path(self, path):
+    def _check_path(self, path, **kwrgs):
         path = os.path.join(os.getcwd(), path)
         assert os.path.isfile(path=path), f"Check your path || not {path}"
         return path
 
     def frange(self, __start: int = 0, __end: int = None, __step: int = 1):
         self.reset()
         assert __start >= 0, ValueError("Frame start idx should be positive")
```

### Comparing `MDbrew-2.3.0/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.1/MDbrew/main/filetype/lmps.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from ..opener import Opener
 
 
 class lmpsOpener(Opener):
-    def __init__(self, path: str) -> None:
-        super().__init__(path)
+    def __init__(self, path: str, *args, **kwrgs) -> None:
+        super().__init__(path, *args, **kwrgs)
         self._atom_keyword = "type"
-        self.gen_db()
+        super().gen_db()
 
-    def _make_one_frame_data(self, file, first_loop_line):
-        self.skip_line(file=file, num=2)
+    def _make_one_frame_data(self, file):
+        self.skip_line(file=file, num=3)
         atom_num = int(file.readline().split()[0])
         self.skip_line(file=file, num=1)
         self.box_size = [sum([abs(float(box_length)) for box_length in file.readline().split()]) for _ in range(3)]
         self.column = file.readline().split()[2:]
         return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
 
     def skip_line(self, file, num):
```

### Comparing `MDbrew-2.3.0/MDbrew/main/filetype/pdb.py` & `MDbrew-2.3.1/MDbrew/main/filetype/pdb.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from ..opener import Opener
 
 
 class pdbOpener(Opener):
-    def __init__(self, path: str) -> None:
-        super().__init__(path)
+    def __init__(self, path: str, *args, **kwrgs) -> None:
+        super().__init__(path, *args, **kwrgs)
         self.path = path
         self.skip_head = 2
         self.column = ["type", "id", "atom", "x", "y", "z", "ax", "bx", "residue"]
-        self.gen_db()
+        super().gen_db()
 
-    def _make_one_frame_data(self, file, first_loop_line):
+    def _make_one_frame_data(self, file):
+        first__loop_line = file.readline()
         second_loop_line = file.readline()
         self.box_size = [float(box_length) for box_length in second_loop_line.split()[1:4]]
         one_frame_data = []
         while True:
             line = file.readline()
             if "END" in line:
                 break
```

### Comparing `MDbrew-2.3.0/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.1/MDbrew/main/filetype/vasp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from ..opener import Opener
 
 
 class vaspOpener(Opener):
-    def __init__(self, path: str) -> None:
-        super().__init__(path)
+    def __init__(self, path: str, *args, **kwrgs) -> None:
+        super().__init__(path, *args, **kwrgs)
         self.skip_head = 7
         self.column = ["atom", "x", "y", "z"]
         self._set_box_and_atom(path=path)
-        self.gen_db()
+        super().gen_db()
 
-    def _make_one_frame_data(self, file, first_loop_line):
+    def _make_one_frame_data(self, file):
+        first_loop_line = file.readline()
         step = first_loop_line.split()[-1]
         num_atom = sum(self.atom_kind_num)
         database = []
         c_atom_num = 0
         pointer = 0
         for _ in range(num_atom):
             if c_atom_num >= self.atom_kind_num[pointer]:
```

### Comparing `MDbrew-2.3.0/MDbrew/main/opener.py` & `MDbrew-2.3.1/MDbrew/main/opener.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import abc
 
 
 class Opener(object):
     skip_head = 0
+    read_mode = "r"
+    is_require_gro = False
 
-    def __init__(self, path: str) -> None:
+    def __init__(self, path: str, *args, **kwrgs) -> None:
         self.path = path
-        # self.skip_head = 0
         self.column = []
         self.box_size = []
         self._atom_keyword = "atom"
 
     def gen_db(self):
         self.frame = -1
         self._database = self._generate_database()
@@ -24,24 +25,24 @@
         return self._database
 
     @property
     def data(self):
         return self._data
 
     def next_frame(self):
-        self._data = next(self.database)
+        self._data = next(self._database)
 
     @abc.abstractmethod
-    def _make_one_frame_data(self, file, first_loop_line):
+    def _make_one_frame_data(self, file):
         pass
 
     # Generation database
     def _generate_database(self):
-        with open(file=self.path, mode="r") as file:
+        with open(file=self.path, mode=self.read_mode) as file:
             for _ in range(self.skip_head):
                 file.readline()
             while True:
-                line = file.readline()
-                if not line:
+                try:
+                    self.frame += 1
+                    yield self._make_one_frame_data(file=file)
+                except:
                     break
-                self.frame += 1
-                yield self._make_one_frame_data(file=file, first_loop_line=line)
```

### Comparing `MDbrew-2.3.0/MDbrew/tool/colorfont.py` & `MDbrew-2.3.1/MDbrew/tool/colorfont.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew/tool/decorator.py` & `MDbrew-2.3.1/MDbrew/tool/decorator.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew/tool/doctor.py` & `MDbrew-2.3.1/MDbrew/tool/doctor.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .colorfont import color
 
 
 def doctor(path):
     LINE_WIDTH = 60
     sep_line = "=" * LINE_WIDTH
     print(sep_line)
-    mb = Brewery(path=path, fmt="lmps")
+    mb = Brewery(trj_file=path, fmt="lmps")
     coords = mb.coords
     atom_info = mb.atom_info
     order1 = mb.order(what="type == 1")
     order2 = mb.order(what="type == 2")
     print(sep_line)
     position = order1.coords
     ixiyiz = order1.brew(cols=["ix", "iy", "iz"])
```

### Comparing `MDbrew-2.3.0/MDbrew/tool/spacer.py` & `MDbrew-2.3.1/MDbrew/tool/spacer.py`

 * *Files identical despite different names*

### Comparing `MDbrew-2.3.0/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.1/MDbrew.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -13,16 +13,18 @@
 MDbrew/analysis/rdf.py
 MDbrew/application/__init__.py
 MDbrew/application/brewcp2k.py
 MDbrew/main/__init__.py
 MDbrew/main/brewery.py
 MDbrew/main/opener.py
 MDbrew/main/filetype/__init__.py
+MDbrew/main/filetype/gro.py
 MDbrew/main/filetype/lmps.py
 MDbrew/main/filetype/pdb.py
+MDbrew/main/filetype/trr.py
 MDbrew/main/filetype/vasp.py
 MDbrew/main/filetype/xyz.py
 MDbrew/tool/__init__.py
 MDbrew/tool/colorfont.py
 MDbrew/tool/decorator.py
 MDbrew/tool/doctor.py
 MDbrew/tool/spacer.py
```

