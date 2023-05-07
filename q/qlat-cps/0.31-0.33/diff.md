# Comparing `tmp/qlat_cps-0.31.tar.gz` & `tmp/qlat_cps-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qlat_cps-0.31.tar", last modified: Thu May  4 04:33:31 2023, max compression
+gzip compressed data, was "qlat_cps-0.33.tar", last modified: Sun May  7 20:30:37 2023, max compression
```

## Comparing `qlat_cps-0.31.tar` & `qlat_cps-0.33.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_cps-0.31/README.md
--rwxrwxr-x   0        0        0       96 1970-01-01 00:00:00.000000 qlat_cps-0.31/bin/qlat-cps-include
--rw-rw-r--   0        0        0     1393 1970-01-01 00:00:00.000000 qlat_cps-0.31/depend-cps/meson.build
--rw-rw-r--   0        0        0     2382 1970-01-01 00:00:00.000000 qlat_cps-0.31/depend-qlat/meson.build
--rw-rw-r--   0        0        0       54 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/meson.build
--rw-rw-r--   0        0        0      293 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/qlat-cps/meson.build
--rw-rw-r--   0        0        0      413 1970-01-01 00:00:00.000000 qlat_cps-0.31/include/qlat-cps/qlat-cps.h
--rw-rw-r--   0        0        0      570 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/init.cpp
--rw-rw-r--   0        0        0      380 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/meson.build
--rw-rw-r--   0        0        0     2041 1970-01-01 00:00:00.000000 qlat_cps-0.31/lib/prop.cpp
--rw-rw-r--   0        0        0     1267 1970-01-01 00:00:00.000000 qlat_cps-0.31/meson.build
--rw-rw-r--   0        0        0       19 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/meson.build
--rw-rw-r--   0        0        0      117 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/__init__.py
--rw-rw-r--   0        0        0       70 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/all.pxd
--rw-rw-r--   0        0        0      147 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/c.py
--rw-rw-r--   0        0        0       67 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/cp.pxd
--rw-rw-r--   0        0        0      858 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/cp.pyx
--rw-rw-r--   0        0        0      430 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/everything.pxd
--rw-rw-r--   0        0        0      876 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/get_include_dir.py
--rw-rw-r--   0        0        0       44 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/init.py
--rw-rw-r--   0        0        0     1315 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/meson.build
--rw-rw-r--   0        0        0       58 1970-01-01 00:00:00.000000 qlat_cps-0.31/pylib/qlat_cps/prop.py
--rw-rw-r--   0        0        0      529 1970-01-01 00:00:00.000000 qlat_cps-0.31/pyproject.toml
--rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 qlat_cps-0.31/PKG-INFO
+-rw-rw-r--   0        0        0       42 1970-01-01 00:00:00.000000 qlat_cps-0.33/README.md
+-rwxrwxr-x   0        0        0       96 1970-01-01 00:00:00.000000 qlat_cps-0.33/bin/qlat-cps-include
+-rw-rw-r--   0        0        0     1393 1970-01-01 00:00:00.000000 qlat_cps-0.33/depend-cps/meson.build
+-rw-rw-r--   0        0        0     2382 1970-01-01 00:00:00.000000 qlat_cps-0.33/depend-qlat/meson.build
+-rw-rw-r--   0        0        0       54 1970-01-01 00:00:00.000000 qlat_cps-0.33/include/meson.build
+-rw-rw-r--   0        0        0      293 1970-01-01 00:00:00.000000 qlat_cps-0.33/include/qlat-cps/meson.build
+-rw-rw-r--   0        0        0      413 1970-01-01 00:00:00.000000 qlat_cps-0.33/include/qlat-cps/qlat-cps.h
+-rw-rw-r--   0        0        0      570 1970-01-01 00:00:00.000000 qlat_cps-0.33/lib/init.cpp
+-rw-rw-r--   0        0        0      380 1970-01-01 00:00:00.000000 qlat_cps-0.33/lib/meson.build
+-rw-rw-r--   0        0        0     2041 1970-01-01 00:00:00.000000 qlat_cps-0.33/lib/prop.cpp
+-rw-rw-r--   0        0        0     1267 1970-01-01 00:00:00.000000 qlat_cps-0.33/meson.build
+-rw-rw-r--   0        0        0       19 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/meson.build
+-rw-rw-r--   0        0        0      117 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/__init__.py
+-rw-rw-r--   0        0        0       70 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/all.pxd
+-rw-rw-r--   0        0        0      147 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/c.py
+-rw-rw-r--   0        0        0       67 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/cp.pxd
+-rw-rw-r--   0        0        0      858 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/cp.pyx
+-rw-rw-r--   0        0        0      430 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/everything.pxd
+-rw-rw-r--   0        0        0      876 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/get_include_dir.py
+-rw-rw-r--   0        0        0       44 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/init.py
+-rw-rw-r--   0        0        0     1315 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/meson.build
+-rw-rw-r--   0        0        0       58 1970-01-01 00:00:00.000000 qlat_cps-0.33/pylib/qlat_cps/prop.py
+-rw-rw-r--   0        0        0      529 1970-01-01 00:00:00.000000 qlat_cps-0.33/pyproject.toml
+-rw-r--r--   0        0        0      309 1970-01-01 00:00:00.000000 qlat_cps-0.33/PKG-INFO
```

### Comparing `qlat_cps-0.31/depend-cps/meson.build` & `qlat_cps-0.33/depend-cps/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/depend-qlat/meson.build` & `qlat_cps-0.33/depend-qlat/meson.build`

 * *Files 0% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 message('numpy include', qlat_numpy_include)
 
 qlat_numpy = declare_dependency(
   include_directories:  include_directories(qlat_numpy_include),
   dependencies: [ qlat_py3.dependency(), ],
   ).as_system()
 
-if qlat_cpp.check_header('Grid/Eigen/Eigen')
+if qlat_cpp.check_header('Eigen/Eigen')
   qlat_eigen = dependency('', required: false)
-elif qlat_cpp.check_header('Eigen/Eigen')
+elif qlat_cpp.check_header('Grid/Eigen/Eigen')
   qlat_eigen = dependency('', required: false)
 else
   qlat_eigen = dependency('eigen3').as_system()
 endif
 
 qlat_include = run_command(qlat_py3, '-c', 'import qlat as q ; print("\\n".join(q.get_include_list()))',
   env: environment({'q_verbose': '-1'}),
```

### Comparing `qlat_cps-0.31/lib/init.cpp` & `qlat_cps-0.33/lib/init.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/lib/prop.cpp` & `qlat_cps-0.33/lib/prop.cpp`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/meson.build` & `qlat_cps-0.33/meson.build`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project('qlat-cps', 'cpp', 'cython',
-  version: '0.31',
+  version: '0.33',
   license: 'GPL-3.0-or-later',
   default_options: [
     'warning_level=3',
     'cpp_std=c++14',
     'libdir=lib',
     'optimization=2',
     'debug=false',
```

### Comparing `qlat_cps-0.31/pylib/qlat_cps/cp.pyx` & `qlat_cps-0.33/pylib/qlat_cps/cp.pyx`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/pylib/qlat_cps/get_include_dir.py` & `qlat_cps-0.33/pylib/qlat_cps/get_include_dir.py`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/pylib/qlat_cps/meson.build` & `qlat_cps-0.33/pylib/qlat_cps/meson.build`

 * *Files identical despite different names*

### Comparing `qlat_cps-0.31/pyproject.toml` & `qlat_cps-0.33/pyproject.toml`

 * *Files identical despite different names*

