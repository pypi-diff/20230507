# Comparing `tmp/cpymad-1.9.2.tar.gz` & `tmp/cpymad-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cpymad-1.9.2.tar", last modified: Tue Jan 18 22:12:57 2022, max compression
+gzip compressed data, was "dist/cpymad-1.9.3.tar", last modified: Mon Feb 28 18:01:32 2022, max compression
```

## Comparing `cpymad-1.9.2.tar` & `cpymad-1.9.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/
--rw-r--r--   0 runner    (1001) runner     (121)        1 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner     (121)        1 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) runner     (121)      180 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner     (121)        7 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) runner     (121)      746 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner     (121)     5615 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad/
--rw-r--r--   0 runner    (1001) runner     (121)     8635 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/clibmadx.pxd
--rw-r--r--   0 runner    (1001) runner     (121)     1381 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/_rpc.py
--rw-r--r--   0 runner    (1001) runner     (121)     5805 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/parsing.py
--rw-r--r--   0 runner    (1001) runner     (121)      925 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/__init__.py
--rw-r--r--   0 runner    (1001) runner     (121)    41553 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/libmadx.pyx
--rw-r--r--   0 runner    (1001) runner     (121)  1569476 2022-01-18 22:12:56.000000 cpymad-1.9.2/src/cpymad/libmadx.c
--rw-r--r--   0 runner    (1001) runner     (121)    16907 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/util.py
--rw-r--r--   0 runner    (1001) runner     (121)     2860 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/types.py
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/src/cpymad/COPYING/
--rw-r--r--   0 runner    (1001) runner     (121)        0 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/COPYING/__init__.py
--rw-r--r--   0 runner    (1001) runner     (121)     1237 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/COPYING/madx.rst
--rw-r--r--   0 runner    (1001) runner     (121)     1580 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/COPYING/cpymad.rst
--rw-r--r--   0 runner    (1001) runner     (121)    41617 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/madx.py
--rw-r--r--   0 runner    (1001) runner     (121)     2482 2022-01-18 22:08:08.000000 cpymad-1.9.2/src/cpymad/stream.py
--rw-r--r--   0 runner    (1001) runner     (121)    26948 2022-01-18 22:08:08.000000 cpymad-1.9.2/CHANGES.rst
--rw-r--r--   0 runner    (1001) runner     (121)     5573 2022-01-18 22:08:08.000000 cpymad-1.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/test/
--rw-r--r--   0 runner    (1001) runner     (121)    29435 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/test_madx.py
--rw-r--r--   0 runner    (1001) runner     (121)       29 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/answer_call42.madx
--rw-r--r--   0 runner    (1001) runner     (121)     3044 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/test_transfer_map.py
--rw-r--r--   0 runner    (1001) runner     (121)       13 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/answer_42.madx
--rw-r--r--   0 runner    (1001) runner     (121)     7911 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/test_util.py
--rw-r--r--   0 runner    (1001) runner     (121)     1118 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/test_regression.py
--rw-r--r--   0 runner    (1001) runner     (121)       13 2022-01-18 22:08:08.000000 cpymad-1.9.2/test/answer_43.madx
--rw-r--r--   0 runner    (1001) runner     (121)     1542 2022-01-18 22:12:57.000000 cpymad-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) runner     (121)     4544 2022-01-18 22:08:08.000000 cpymad-1.9.2/README.rst
--rw-r--r--   0 runner    (1001) runner     (121)     5615 2022-01-18 22:12:57.000000 cpymad-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) runner     (121)     3219 2022-01-18 22:08:08.000000 cpymad-1.9.2/COPYING.rst
-drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-01-18 22:12:57.000000 cpymad-1.9.2/LICENSE/
--rw-r--r--   0 runner    (1001) runner     (121)    35147 2022-01-18 22:08:08.000000 cpymad-1.9.2/LICENSE/GPLv3
--rw-r--r--   0 runner    (1001) runner     (121)    11358 2022-01-18 22:08:08.000000 cpymad-1.9.2/LICENSE/Apache
--rw-r--r--   0 runner    (1001) runner     (121)      199 2022-01-18 22:08:08.000000 cpymad-1.9.2/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/LICENSE/
+-rw-r--r--   0 runner    (1001) runner     (121)    11358 2022-02-28 17:08:27.000000 cpymad-1.9.3/LICENSE/Apache
+-rw-r--r--   0 runner    (1001) runner     (121)    35147 2022-02-28 17:08:27.000000 cpymad-1.9.3/LICENSE/GPLv3
+-rw-r--r--   0 runner    (1001) runner     (121)      199 2022-02-28 17:08:27.000000 cpymad-1.9.3/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad/
+-rw-r--r--   0 runner    (1001) runner     (121)     8635 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/clibmadx.pxd
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad/COPYING/
+-rw-r--r--   0 runner    (1001) runner     (121)     1237 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/COPYING/madx.rst
+-rw-r--r--   0 runner    (1001) runner     (121)        0 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/COPYING/__init__.py
+-rw-r--r--   0 runner    (1001) runner     (121)     1580 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/COPYING/cpymad.rst
+-rw-r--r--   0 runner    (1001) runner     (121)     5805 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/parsing.py
+-rw-r--r--   0 runner    (1001) runner     (121)     2860 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/types.py
+-rw-r--r--   0 runner    (1001) runner     (121)    16907 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/util.py
+-rw-r--r--   0 runner    (1001) runner     (121)     1381 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/_rpc.py
+-rw-r--r--   0 runner    (1001) runner     (121)    41553 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/libmadx.pyx
+-rw-r--r--   0 runner    (1001) runner     (121)     2482 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/stream.py
+-rw-r--r--   0 runner    (1001) runner     (121)      925 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/__init__.py
+-rw-r--r--   0 runner    (1001) runner     (121)    41617 2022-02-28 17:08:27.000000 cpymad-1.9.3/src/cpymad/madx.py
+-rw-r--r--   0 runner    (1001) runner     (121)  1570124 2022-02-28 18:01:31.000000 cpymad-1.9.3/src/cpymad/libmadx.c
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/
+-rw-r--r--   0 runner    (1001) runner     (121)        1 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) runner     (121)        7 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) runner     (121)     5615 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner     (121)      746 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner     (121)      180 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner     (121)        1 2022-02-28 18:01:32.000000 cpymad-1.9.3/src/cpymad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner     (121)     5573 2022-02-28 17:08:27.000000 cpymad-1.9.3/setup.py
+-rw-r--r--   0 runner    (1001) runner     (121)     1542 2022-02-28 18:01:32.000000 cpymad-1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner     (121)        0 2022-02-28 18:01:32.000000 cpymad-1.9.3/test/
+-rw-r--r--   0 runner    (1001) runner     (121)     3044 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/test_transfer_map.py
+-rw-r--r--   0 runner    (1001) runner     (121)       13 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/answer_43.madx
+-rw-r--r--   0 runner    (1001) runner     (121)     1118 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/test_regression.py
+-rw-r--r--   0 runner    (1001) runner     (121)    29435 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/test_madx.py
+-rw-r--r--   0 runner    (1001) runner     (121)       29 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/answer_call42.madx
+-rw-r--r--   0 runner    (1001) runner     (121)       13 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/answer_42.madx
+-rw-r--r--   0 runner    (1001) runner     (121)     7911 2022-02-28 17:08:27.000000 cpymad-1.9.3/test/test_util.py
+-rw-r--r--   0 runner    (1001) runner     (121)     5615 2022-02-28 18:01:32.000000 cpymad-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner     (121)    27007 2022-02-28 17:08:27.000000 cpymad-1.9.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) runner     (121)     4544 2022-02-28 17:08:27.000000 cpymad-1.9.3/README.rst
+-rw-r--r--   0 runner    (1001) runner     (121)     3219 2022-02-28 17:08:27.000000 cpymad-1.9.3/COPYING.rst
```

### Comparing `cpymad-1.9.2/src/cpymad.egg-info/SOURCES.txt` & `cpymad-1.9.3/src/cpymad.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad.egg-info/PKG-INFO` & `cpymad-1.9.3/src/cpymad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymad
-Version: 1.9.2
+Version: 1.9.3
 Summary: Cython binding to MAD-X
 Home-page: https://github.com/hibtc/cpymad
 Author: Thomas Gläßle
 Author-email: t_glaessle@gmx.de
 License: GPLv3+
 Project-URL: Source Code, https://github.com/hibtc/cpymad
 Project-URL: Bug Tracker, https://github.com/hibtc/cpymad/issues
```

### Comparing `cpymad-1.9.2/src/cpymad/clibmadx.pxd` & `cpymad-1.9.3/src/cpymad/clibmadx.pxd`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/_rpc.py` & `cpymad-1.9.3/src/cpymad/_rpc.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/parsing.py` & `cpymad-1.9.3/src/cpymad/parsing.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/__init__.py` & `cpymad-1.9.3/src/cpymad/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import unicode_literals
 import sys
 import warnings
 
 
 __title__ = 'cpymad'
-__version__ = '1.9.2'
+__version__ = '1.9.3'
 
 __summary__ = 'Cython binding to MAD-X'
 __uri__ = 'https://github.com/hibtc/cpymad'
 
 __credits__ = """
 Current cpymad maintainer:
```

### Comparing `cpymad-1.9.2/src/cpymad/libmadx.pyx` & `cpymad-1.9.3/src/cpymad/libmadx.pyx`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/libmadx.c` & `cpymad-1.9.3/src/cpymad/libmadx.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/* Generated by Cython 0.29.26 */
+/* Generated by Cython 0.29.28 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [],
         "extra_compile_args": [
             "-std=gnu99"
@@ -36,16 +36,16 @@
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_26"
-#define CYTHON_HEX_VERSION 0x001D1AF0
+#define CYTHON_ABI "0_29_28"
+#define CYTHON_HEX_VERSION 0x001D1CF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -199,30 +199,36 @@
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
-  #ifndef CYTHON_FAST_THREAD_STATE
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_FAST_THREAD_STATE
+    #define CYTHON_FAST_THREAD_STATE 0
+  #elif !defined(CYTHON_FAST_THREAD_STATE)
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL (PY_VERSION_HEX < 0x030B00A1)
   #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
   #ifndef CYTHON_USE_DICT_VERSIONS
     #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
   #endif
-  #ifndef CYTHON_USE_EXC_INFO_STACK
+  #if PY_VERSION_HEX >= 0x030B00A4
+    #undef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK 0
+  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if CYTHON_USE_PYLONG_INTERNALS
@@ -1812,15 +1818,15 @@
 /* StrEquals.proto */
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyString_Equals __Pyx_PyUnicode_Equals
 #else
 #define __Pyx_PyString_Equals __Pyx_PyBytes_Equals
 #endif
 
-/* None.proto */
+/* DivInt[Py_ssize_t].proto */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t, Py_ssize_t);
 
 /* UnaryNegOverflows.proto */
 #define UNARY_NEG_WOULD_OVERFLOW(x)\
         (((x) < 0) & ((unsigned long)(x) == 0-(unsigned long)(x)))
 
 static CYTHON_UNUSED int __pyx_array_getbuffer(PyObject *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /*proto*/
@@ -1882,15 +1888,15 @@
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
-/* None.proto */
+/* DivInt[long].proto */
 static CYTHON_INLINE long __Pyx_div_long(long, long);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
@@ -30490,21 +30496,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_array __pyx_vtable_array;
 
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_array_obj *p;
@@ -30682,21 +30688,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -30804,21 +30810,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -31068,21 +31074,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -31217,21 +31223,21 @@
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
   0, /*tp_finalize*/
   #endif
-  #if PY_VERSION_HEX >= 0x030800b1
+  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -35961,21 +35967,21 @@
     0,
     0,
     0,
     0,
 #if PY_VERSION_HEX >= 0x030400a1
     0,
 #endif
-#if PY_VERSION_HEX >= 0x030800b1
+#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM+0 >= 0x06000000
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -36845,15 +36851,15 @@
     }
     PyErr_Format(PyExc_TypeError,
         "Argument '%.200s' has incorrect type (expected %.200s, got %.200s)",
         name, type->tp_name, Py_TYPE(obj)->tp_name);
     return 0;
 }
 
-/* None */
+/* DivInt[Py_ssize_t] */
 static CYTHON_INLINE Py_ssize_t __Pyx_div_Py_ssize_t(Py_ssize_t a, Py_ssize_t b) {
     Py_ssize_t q = a / b;
     Py_ssize_t r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
 
@@ -37228,15 +37234,15 @@
 #endif
 
 /* None */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname) {
     PyErr_Format(PyExc_UnboundLocalError, "local variable '%s' referenced before assignment", varname);
 }
 
-/* None */
+/* DivInt[long] */
 static CYTHON_INLINE long __Pyx_div_long(long a, long b) {
     long q = a / b;
     long r = a - q*b;
     q -= ((r != 0) & ((r ^ b) < 0));
     return q;
 }
```

### Comparing `cpymad-1.9.2/src/cpymad/util.py` & `cpymad-1.9.3/src/cpymad/util.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/types.py` & `cpymad-1.9.3/src/cpymad/types.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/COPYING/madx.rst` & `cpymad-1.9.3/src/cpymad/COPYING/madx.rst`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/COPYING/cpymad.rst` & `cpymad-1.9.3/src/cpymad/COPYING/cpymad.rst`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/madx.py` & `cpymad-1.9.3/src/cpymad/madx.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/src/cpymad/stream.py` & `cpymad-1.9.3/src/cpymad/stream.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/CHANGES.rst` & `cpymad-1.9.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 Changelog
 ~~~~~~~~~
 
+1.9.3
+=====
+Date: 28.02.2022
+
+- update to MAD-X 5.08.01
+
+
 1.9.2
 =====
 Date: 18.01.2022
 
 - update to MAD-X 5.08.00
 
+
 1.9.1
 =====
 Date: 24.11.2021
 
 Build updates:
 
 - add wheels for python 3.10 (EXPERIMENTAL)
```

### Comparing `cpymad-1.9.2/setup.py` & `cpymad-1.9.3/setup.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/test/test_madx.py` & `cpymad-1.9.3/test/test_madx.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/test/test_transfer_map.py` & `cpymad-1.9.3/test/test_transfer_map.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/test/test_util.py` & `cpymad-1.9.3/test/test_util.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/test/test_regression.py` & `cpymad-1.9.3/test/test_regression.py`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/setup.cfg` & `cpymad-1.9.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/README.rst` & `cpymad-1.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/PKG-INFO` & `cpymad-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpymad
-Version: 1.9.2
+Version: 1.9.3
 Summary: Cython binding to MAD-X
 Home-page: https://github.com/hibtc/cpymad
 Author: Thomas Gläßle
 Author-email: t_glaessle@gmx.de
 License: GPLv3+
 Project-URL: Source Code, https://github.com/hibtc/cpymad
 Project-URL: Bug Tracker, https://github.com/hibtc/cpymad/issues
```

### Comparing `cpymad-1.9.2/COPYING.rst` & `cpymad-1.9.3/COPYING.rst`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/LICENSE/GPLv3` & `cpymad-1.9.3/LICENSE/GPLv3`

 * *Files identical despite different names*

### Comparing `cpymad-1.9.2/LICENSE/Apache` & `cpymad-1.9.3/LICENSE/Apache`

 * *Files identical despite different names*

