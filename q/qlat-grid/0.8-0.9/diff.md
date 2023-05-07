# Comparing `tmp/qlat_grid-0.8.tar.gz` & `tmp/qlat_grid-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat_grid-0.8.tar", last modified: Sun Nov 27 17:51:23 2022, max compression
+gzip compressed data, was "qlat_grid-0.9.tar", last modified: Sat Dec 10 16:32:20 2022, max compression
```

## Comparing `qlat_grid-0.8.tar` & `qlat_grid-0.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_grid-0.8/README.md
--rwxrwxr-x   0        0        0      101 1970-01-01 00:00:00.000000 qlat_grid-0.8/bin/qlat-grid-include
--rw-rw-r--   0        0        0       55 1970-01-01 00:00:00.000000 qlat_grid-0.8/include/meson.build
--rw-rw-r--   0        0        0      213 1970-01-01 00:00:00.000000 qlat_grid-0.8/include/qlat-grid/meson.build
--rw-rw-r--   0        0        0       46 1970-01-01 00:00:00.000000 qlat_grid-0.8/include/qlat-grid/qlat-grid.h
--rw-rw-r--   0        0        0     4046 1970-01-01 00:00:00.000000 qlat_grid-0.8/meson.build
--rw-rw-r--   0        0        0      186 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/exports.h
--rw-r--r--   0        0        0     1020 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/init.cpp
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/lib.cpp
--rw-rw-r--   0        0        0     2253 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/lib.h
--rw-rw-r--   0        0        0      365 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/meson.build
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/prop.cpp
--rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/cqlat_grid/update.sh
--rw-rw-r--   0        0        0       41 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/meson.build
--rw-rw-r--   0        0        0      126 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/__init__.py
--rw-rw-r--   0        0        0      154 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/cg.py
--rw-rw-r--   0        0        0      244 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/get_include_dir.py
--rw-rw-r--   0        0        0      350 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/init.py
--rw-rw-r--   0        0        0      178 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/meson.build
--rw-rw-r--   0        0        0      293 1970-01-01 00:00:00.000000 qlat_grid-0.8/pylib/qlat_grid/prop.py
--rw-rw-r--   0        0        0      427 1970-01-01 00:00:00.000000 qlat_grid-0.8/pyproject.toml
--rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 qlat_grid-0.8/PKG-INFO
+-rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_grid-0.9/README.md
+-rwxrwxr-x   0        0        0      101 1970-01-01 00:00:00.000000 qlat_grid-0.9/bin/qlat-grid-include
+-rw-rw-r--   0        0        0       55 1970-01-01 00:00:00.000000 qlat_grid-0.9/include/meson.build
+-rw-rw-r--   0        0        0      213 1970-01-01 00:00:00.000000 qlat_grid-0.9/include/qlat-grid/meson.build
+-rw-rw-r--   0        0        0       46 1970-01-01 00:00:00.000000 qlat_grid-0.9/include/qlat-grid/qlat-grid.h
+-rw-rw-r--   0        0        0     4102 1970-01-01 00:00:00.000000 qlat_grid-0.9/meson.build
+-rw-rw-r--   0        0        0      155 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/exports.h
+-rw-r--r--   0        0        0      800 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/init.cpp
+-rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/lib.cpp
+-rw-rw-r--   0        0        0     2253 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/lib.h
+-rw-rw-r--   0        0        0      365 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/meson.build
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/prop.cpp
+-rwxr-xr-x   0        0        0      766 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/cqlat_grid/update.sh
+-rw-rw-r--   0        0        0       41 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/meson.build
+-rw-rw-r--   0        0        0      165 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/__init__.pxd
+-rw-rw-r--   0        0        0      125 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/__init__.py
+-rw-rw-r--   0        0        0      172 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/c.py
+-rw-rw-r--   0        0        0      116 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/cp.pyx
+-rw-rw-r--   0        0        0      467 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/get_include_dir.py
+-rw-rw-r--   0        0        0      349 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/init.py
+-rw-rw-r--   0        0        0      443 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/meson.build
+-rw-rw-r--   0        0        0      292 1970-01-01 00:00:00.000000 qlat_grid-0.9/pylib/qlat_grid/prop.py
+-rw-rw-r--   0        0        0      427 1970-01-01 00:00:00.000000 qlat_grid-0.9/pyproject.toml
+-rw-r--r--   0        0        0      287 1970-01-01 00:00:00.000000 qlat_grid-0.9/PKG-INFO
```

### Comparing `qlat_grid-0.8/meson.build` & `qlat_grid-0.9/meson.build`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-project('qlat-grid', 'cpp',
-  version: '0.8',
+project('qlat-grid', 'cpp', 'cython',
+  version: '0.9',
   license: 'GPL-3.0-or-later',
   default_options: [
     'warning_level=3',
     'cpp_std=c++14',
     'libdir=lib',
     'optimization=2',
     'debug=false',
+    'cython_language=cpp',
     ])
 
 add_project_arguments('-fno-strict-aliasing', language: ['c', 'cpp'])
 
 cpp = meson.get_compiler('cpp')
 
+fs = import('fs')
+
 py_mod = import('python')
 py3 = py_mod.find_installation('python3')
 message(py3.path())
 message(py3.get_install_dir())
 
 message('Collecting Grid information using \'grid-config\':')
 grid_prefix = run_command('grid-config', '--prefix', check: true).stdout().strip()
```

### Comparing `qlat_grid-0.8/pylib/cqlat_grid/init.cpp` & `qlat_grid-0.9/pylib/cqlat_grid/init.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -22,17 +22,7 @@
   //
   int argc = (int)sargs.size();
   char** argv = (char**)&cargs[0];
   //
   grid_begin(&argc, &argv, node_size_list);
   Py_RETURN_NONE;
 })
-
-EXPORT(end_with_grid, {
-  using namespace qlat;
-  bool is_preserving_cache = false;
-  if (!PyArg_ParseTuple(args, "b", &is_preserving_cache)) {
-    return NULL;
-  }
-  grid_end(is_preserving_cache);
-  Py_RETURN_NONE;
-})
```

### Comparing `qlat_grid-0.8/pylib/cqlat_grid/lib.cpp` & `qlat_grid-0.9/pylib/cqlat_grid/lib.cpp`

 * *Files identical despite different names*

### Comparing `qlat_grid-0.8/pylib/cqlat_grid/lib.h` & `qlat_grid-0.9/pylib/cqlat_grid/lib.h`

 * *Files identical despite different names*

### Comparing `qlat_grid-0.8/pylib/cqlat_grid/prop.cpp` & `qlat_grid-0.9/pylib/cqlat_grid/prop.cpp`

 * *Files identical despite different names*

### Comparing `qlat_grid-0.8/pylib/cqlat_grid/update.sh` & `qlat_grid-0.9/pylib/cqlat_grid/update.sh`

 * *Files identical despite different names*

