# Comparing `tmp/rpmdyn-2023.5.tar.gz` & `tmp/rpmdyn-2023.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpmdyn-2023.5.tar", last modified: Tue May  2 00:16:18 2023, max compression
+gzip compressed data, was "rpmdyn-2023.5.7.tar", last modified: Sun May  7 01:28:01 2023, max compression
```

## Comparing `rpmdyn-2023.5.tar` & `rpmdyn-2023.5.7.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.463508 rpmdyn-2023.5/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       54 2023-05-02 00:06:30.000000 rpmdyn-2023.5/MANIFEST.in
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      108 2023-05-02 00:16:18.463508 rpmdyn-2023.5/PKG-INFO
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)        0 2021-10-27 06:05:22.000000 rpmdyn-2023.5/README.md
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.461508 rpmdyn-2023.5/custom_build/
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.461508 rpmdyn-2023.5/custom_build/__pycache__/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     3633 2023-05-02 00:16:17.000000 rpmdyn-2023.5/custom_build/__pycache__/backend.cpython-311.pyc
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     2304 2023-05-02 00:06:56.000000 rpmdyn-2023.5/custom_build/backend.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      378 2023-05-02 00:06:30.000000 rpmdyn-2023.5/pyproject.toml
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        5 2023-05-02 00:06:30.000000 rpmdyn-2023.5/requirements.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       38 2023-05-02 00:16:18.463508 rpmdyn-2023.5/setup.cfg
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.461508 rpmdyn-2023.5/src/
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.462508 rpmdyn-2023.5/src/rpmdyn/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)       60 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn/__init__.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)    24226 2023-05-02 00:06:30.000000 rpmdyn-2023.5/src/rpmdyn/_const.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     3809 2023-05-02 00:06:30.000000 rpmdyn-2023.5/src/rpmdyn/_ffi.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      157 2023-05-02 00:06:30.000000 rpmdyn-2023.5/src/rpmdyn/_keyring.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)      614 2021-10-27 06:05:22.000000 rpmdyn-2023.5/src/rpmdyn/_pth_hook.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      513 2023-05-02 00:06:30.000000 rpmdyn-2023.5/src/rpmdyn/_rpm.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     3445 2023-05-02 00:06:30.000000 rpmdyn-2023.5/src/rpmdyn/_transaction.py
--rw-rw-r--   0 rmcgover (20551) rmcgover (20551)       24 2021-10-27 06:05:22.000000 rpmdyn-2023.5/src/rpmdyn/rpmdyn.pth
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.463508 rpmdyn-2023.5/src/rpmdyn.egg-info/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      108 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn.egg-info/PKG-INFO
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      575 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn.egg-info/SOURCES.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        1 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn.egg-info/dependency_links.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        5 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn.egg-info/requires.txt
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)        7 2023-05-02 00:16:18.000000 rpmdyn-2023.5/src/rpmdyn.egg-info/top_level.txt
-drwxr-xr-x   0 rmcgover (20551) rmcgover (20551)        0 2023-05-02 00:16:18.463508 rpmdyn-2023.5/tests/
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      105 2023-05-02 00:06:30.000000 rpmdyn-2023.5/tests/test_constants.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)     2115 2023-05-02 00:06:30.000000 rpmdyn-2023.5/tests/test_headers.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      610 2023-05-02 00:06:30.000000 rpmdyn-2023.5/tests/test_labelcompare.py
--rw-r--r--   0 rmcgover (20551) rmcgover (20551)      637 2023-05-02 00:06:30.000000 rpmdyn-2023.5/tests/test_transactionset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/custom_build/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/custom_build/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-05-07 01:28:00.000000 rpmdyn-2023.5.7/custom_build/__pycache__/backend.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/custom_build/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.529428 rpmdyn-2023.5.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/src/rpmdyn/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24226 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_ffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_keyring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_pth_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_rpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/src/rpmdyn/rpmdyn.pth
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/src/rpmdyn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    43843 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 01:28:01.000000 rpmdyn-2023.5.7/src/rpmdyn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 01:28:01.533428 rpmdyn-2023.5.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_labelcompare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 01:27:49.000000 rpmdyn-2023.5.7/tests/test_transactionset.py
```

### Comparing `rpmdyn-2023.5/custom_build/__pycache__/backend.cpython-311.pyc` & `rpmdyn-2023.5.7/custom_build/__pycache__/backend.cpython-311.pyc`

 * *Files 15% similar despite different names*

#### Python bytecode

```diff
@@ -1,34 +1,33 @@
 magic:    0xa70d0d0a
-moddate:  0x20545064 (Tue May  2 00:06:56 2023 UTC)
-files sz: 2304
+moddate:  0x95fe5664 (Sun May  7 01:27:49 2023 UTC)
+files sz: 2248
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 7
+   stacksize : 5
    flags     : 0
    code
       0x9700640064016c005a00640064016c015a01640064016c025a02640064
-      016c035a03640064016c045a04640064026c056d065a060100640064016c
-      075a07640064036c07540065006a080000000000000000a0090000000000
-      000000000000000000000000000000640464056406a6030000ab03000000
-      00000000005a0a0900640d6407650b64086506650c650b19000000000000
-      000000190000000000000000006409650b6606640a84055a0d640e640b84
-      015a0e640e640c84015a0f64015300
+      016c035a03640064016c045a04640064016c055a05640064026c05540065
+      016a060000000000000000a0070000000000000000000000000000000000
+      000000640364046405a6030000ab0300000000000000005a08640b640665
+      09640765096604640884055a0a640c640984015a0b640c640a84015a0c64
+      015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (os)
-                 8 STORE_NAME               0 (os)
+                 6 IMPORT_NAME              0 (glob)
+                 8 STORE_NAME               0 (glob)
    
      2          10 LOAD_CONST               0 (0)
                 12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (glob)
-                16 STORE_NAME               1 (glob)
+                14 IMPORT_NAME              1 (os)
+                16 STORE_NAME               1 (os)
    
      3          18 LOAD_CONST               0 (0)
                 20 LOAD_CONST               1 (None)
                 22 IMPORT_NAME              2 (shutil)
                 24 STORE_NAME               2 (shutil)
    
      4          26 LOAD_CONST               0 (0)
@@ -37,86 +36,63 @@
                 32 STORE_NAME               3 (subprocess)
    
      5          34 LOAD_CONST               0 (0)
                 36 LOAD_CONST               1 (None)
                 38 IMPORT_NAME              4 (tempfile)
                 40 STORE_NAME               4 (tempfile)
    
-     6          42 LOAD_CONST               0 (0)
-                44 LOAD_CONST               2 (('Optional',))
-                46 IMPORT_NAME              5 (typing)
-                48 IMPORT_FROM              6 (Optional)
-                50 STORE_NAME               6 (Optional)
-                52 POP_TOP
-   
-     7          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               1 (None)
-                58 IMPORT_NAME              7 (buildsys_dateversion)
-                60 STORE_NAME               7 (buildsys_dateversion)
-   
-     8          62 LOAD_CONST               0 (0)
-                64 LOAD_CONST               3 (('*',))
-                66 IMPORT_NAME              7 (buildsys_dateversion)
-                68 IMPORT_STAR
-   
-    10          70 LOAD_NAME                0 (os)
-                72 LOAD_ATTR                8 (path)
-                82 LOAD_METHOD              9 (join)
-               104 LOAD_CONST               4 ('src')
-               106 LOAD_CONST               5 ('rpmdyn')
-               108 LOAD_CONST               6 ('rpmdyn.pth')
-               110 PRECALL                  3
-               114 CALL                     3
-               124 STORE_NAME              10 (PTH_PATH)
-   
-    14         126 NOP
-   
-    13         128 LOAD_CONST              13 ((None,))
-               130 LOAD_CONST               7 ('wheel_path')
-   
-    14         132 LOAD_NAME               11 (str)
-   
-    13         134 LOAD_CONST               8 ('wheel_pack_args')
-   
-    14         136 LOAD_NAME                6 (Optional)
-               138 LOAD_NAME               12 (list)
-               140 LOAD_NAME               11 (str)
-               142 BINARY_SUBSCR
-               152 BINARY_SUBSCR
-   
-    13         162 LOAD_CONST               9 ('return')
-   
-    15         164 LOAD_NAME               11 (str)
-   
-    13         166 BUILD_TUPLE              6
-               168 LOAD_CONST              10 (<code object repack_with_pth, file "/home/rmcgover/src/rpmdyn/custom_build/backend.py", line 13>)
-               170 MAKE_FUNCTION            5 (defaults, annotations)
-               172 STORE_NAME              13 (repack_with_pth)
-   
-    57         174 LOAD_CONST              14 ((None, None))
-               176 LOAD_CONST              11 (<code object build_editable, file "/home/rmcgover/src/rpmdyn/custom_build/backend.py", line 57>)
-               178 MAKE_FUNCTION            1 (defaults)
-               180 STORE_NAME              14 (build_editable)
-   
-    67         182 LOAD_CONST              14 ((None, None))
-               184 LOAD_CONST              12 (<code object build_wheel, file "/home/rmcgover/src/rpmdyn/custom_build/backend.py", line 67>)
-               186 MAKE_FUNCTION            1 (defaults)
-               188 STORE_NAME              15 (build_wheel)
-               190 LOAD_CONST               1 (None)
-               192 RETURN_VALUE
+     7          42 LOAD_CONST               0 (0)
+                44 LOAD_CONST               1 (None)
+                46 IMPORT_NAME              5 (buildsys_dateversion)
+                48 STORE_NAME               5 (buildsys_dateversion)
+   
+     8          50 LOAD_CONST               0 (0)
+                52 LOAD_CONST               2 (('*',))
+                54 IMPORT_NAME              5 (buildsys_dateversion)
+                56 IMPORT_STAR
+   
+    10          58 LOAD_NAME                1 (os)
+                60 LOAD_ATTR                6 (path)
+                70 LOAD_METHOD              7 (join)
+                92 LOAD_CONST               3 ('src')
+                94 LOAD_CONST               4 ('rpmdyn')
+                96 LOAD_CONST               5 ('rpmdyn.pth')
+                98 PRECALL                  3
+               102 CALL                     3
+               112 STORE_NAME               8 (PTH_PATH)
+   
+    13         114 LOAD_CONST              11 ((None,))
+               116 LOAD_CONST               6 ('wheel_path')
+               118 LOAD_NAME                9 (str)
+               120 LOAD_CONST               7 ('return')
+               122 LOAD_NAME                9 (str)
+               124 BUILD_TUPLE              4
+               126 LOAD_CONST               8 (<code object repack_with_pth, file "/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py", line 13>)
+               128 MAKE_FUNCTION            5 (defaults, annotations)
+               130 STORE_NAME              10 (repack_with_pth)
+   
+    55         132 LOAD_CONST              12 ((None, None))
+               134 LOAD_CONST               9 (<code object build_editable, file "/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py", line 55>)
+               136 MAKE_FUNCTION            1 (defaults)
+               138 STORE_NAME              11 (build_editable)
+   
+    65         140 LOAD_CONST              12 ((None, None))
+               142 LOAD_CONST              10 (<code object build_wheel, file "/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py", line 65>)
+               144 MAKE_FUNCTION            1 (defaults)
+               146 STORE_NAME              12 (build_wheel)
+               148 LOAD_CONST               1 (None)
+               150 RETURN_VALUE
    consts
       0
       None
-      ('Optional',)
       ('*',)
       'src'
       'rpmdyn'
       'rpmdyn.pth'
       'wheel_path'
-      'wheel_pack_args'
       'return'
       code
          argcount  : 2
          nlocals   : 10
          stacksize : 8
          flags     : 3
          code
@@ -155,198 +131,198 @@
             006a0d00000000000000007c097c02a6020000ab02000000000000000001
             00640064006400a6020000ab02000000000000000001006e0b2300310073
             04770278035900770101005900010001007400000000000000000000006a
             010000000000000000a01000000000000000000000000000000000000000
             007c09a6010000ab0100000000000000005300
           13           0 RESUME                   0
          
-          16           2 LOAD_FAST                1 (wheel_pack_args)
+          14           2 LOAD_FAST                1 (wheel_pack_args)
                        4 JUMP_IF_TRUE_OR_POP      1 (to 8)
                        6 BUILD_LIST               0
                  >>    8 STORE_FAST               1 (wheel_pack_args)
          
-          18          10 LOAD_GLOBAL              0 (os)
+          16          10 LOAD_GLOBAL              0 (os)
                       22 LOAD_ATTR                1 (path)
                       32 LOAD_METHOD              2 (dirname)
                       54 LOAD_FAST                0 (wheel_path)
                       56 PRECALL                  1
                       60 CALL                     1
                       70 STORE_FAST               2 (wheel_dir)
          
-          20          72 LOAD_GLOBAL              7 (NULL + tempfile)
+          18          72 LOAD_GLOBAL              7 (NULL + tempfile)
                       84 LOAD_ATTR                4 (TemporaryDirectory)
                       94 LOAD_CONST               1 ('rpmdyn_build')
                       96 KW_NAMES                 2
                       98 PRECALL                  1
                      102 CALL                     1
                      112 BEFORE_WITH
                      114 STORE_FAST               3 (tmpdir)
          
-          21         116 LOAD_GLOBAL              0 (os)
+          19         116 LOAD_GLOBAL              0 (os)
                      128 LOAD_ATTR                1 (path)
                      138 LOAD_METHOD              5 (join)
                      160 LOAD_FAST                3 (tmpdir)
                      162 LOAD_CONST               3 ('unpacked')
                      164 PRECALL                  2
                      168 CALL                     2
                      178 STORE_FAST               4 (unpacked)
          
-          22         180 LOAD_GLOBAL              0 (os)
+          20         180 LOAD_GLOBAL              0 (os)
                      192 LOAD_ATTR                1 (path)
                      202 LOAD_METHOD              5 (join)
                      224 LOAD_FAST                3 (tmpdir)
                      226 LOAD_CONST               4 ('output')
                      228 PRECALL                  2
                      232 CALL                     2
                      242 STORE_FAST               5 (output)
          
-          23         244 LOAD_GLOBAL              1 (NULL + os)
+          21         244 LOAD_GLOBAL              1 (NULL + os)
                      256 LOAD_ATTR                6 (makedirs)
                      266 LOAD_FAST                4 (unpacked)
                      268 PRECALL                  1
                      272 CALL                     1
                      282 POP_TOP
          
-          24         284 LOAD_GLOBAL              1 (NULL + os)
+          22         284 LOAD_GLOBAL              1 (NULL + os)
                      296 LOAD_ATTR                6 (makedirs)
                      306 LOAD_FAST                5 (output)
                      308 PRECALL                  1
                      312 CALL                     1
                      322 POP_TOP
          
-          26         324 LOAD_GLOBAL             15 (NULL + subprocess)
+          24         324 LOAD_GLOBAL             15 (NULL + subprocess)
                      336 LOAD_ATTR                8 (run)
                      346 LOAD_CONST               5 ('wheel')
                      348 LOAD_CONST               6 ('unpack')
                      350 LOAD_CONST               7 ('--dest')
                      352 LOAD_FAST                4 (unpacked)
                      354 LOAD_FAST                0 (wheel_path)
                      356 BUILD_LIST               5
                      358 LOAD_CONST               8 (True)
                      360 KW_NAMES                 9
                      362 PRECALL                  2
                      366 CALL                     2
                      376 POP_TOP
          
-          29         378 LOAD_GLOBAL              1 (NULL + os)
+          27         378 LOAD_GLOBAL              1 (NULL + os)
                      390 LOAD_ATTR                9 (unlink)
                      400 LOAD_FAST                0 (wheel_path)
                      402 PRECALL                  1
                      406 CALL                     1
                      416 POP_TOP
          
-          32         418 LOAD_GLOBAL             21 (NULL + glob)
+          30         418 LOAD_GLOBAL             21 (NULL + glob)
                      430 LOAD_ATTR               10 (glob)
                      440 LOAD_GLOBAL              0 (os)
                      452 LOAD_ATTR                1 (path)
                      462 LOAD_METHOD              5 (join)
                      484 LOAD_FAST                4 (unpacked)
                      486 LOAD_CONST              10 ('*')
                      488 PRECALL                  2
                      492 CALL                     2
                      502 PRECALL                  1
                      506 CALL                     1
                      516 STORE_FAST               6 (subdirs)
          
-          33         518 LOAD_GLOBAL             23 (NULL + len)
+          31         518 LOAD_GLOBAL             23 (NULL + len)
                      530 LOAD_FAST                6 (subdirs)
                      532 PRECALL                  1
                      536 CALL                     1
                      546 LOAD_CONST              11 (1)
                      548 COMPARE_OP               2 (==)
                      554 POP_JUMP_FORWARD_IF_TRUE     2 (to 560)
                      556 LOAD_ASSERTION_ERROR
                      558 RAISE_VARARGS            1
          
-          34     >>  560 LOAD_FAST                6 (subdirs)
+          32     >>  560 LOAD_FAST                6 (subdirs)
                      562 LOAD_CONST              12 (0)
                      564 BINARY_SUBSCR
                      574 STORE_FAST               7 (subdir)
          
-          37         576 LOAD_GLOBAL             25 (NULL + shutil)
+          35         576 LOAD_GLOBAL             25 (NULL + shutil)
                      588 LOAD_ATTR               13 (copy)
                      598 LOAD_GLOBAL             28 (PTH_PATH)
                      610 LOAD_GLOBAL              0 (os)
                      622 LOAD_ATTR                1 (path)
                      632 LOAD_METHOD              5 (join)
                      654 LOAD_FAST                7 (subdir)
                      656 LOAD_CONST              13 ('rpmdyn.pth')
                      658 PRECALL                  2
                      662 CALL                     2
                      672 PRECALL                  2
                      676 CALL                     2
                      686 POP_TOP
          
-          40         688 LOAD_GLOBAL             15 (NULL + subprocess)
+          38         688 LOAD_GLOBAL             15 (NULL + subprocess)
                      700 LOAD_ATTR                8 (run)
          
-          41         710 LOAD_CONST               5 ('wheel')
+          39         710 LOAD_CONST               5 ('wheel')
                      712 LOAD_CONST              14 ('pack')
                      714 BUILD_LIST               2
                      716 LOAD_FAST                1 (wheel_pack_args)
                      718 BINARY_OP                0 (+)
                      722 LOAD_CONST              15 ('--dest-dir')
                      724 LOAD_FAST                5 (output)
                      726 LOAD_FAST                7 (subdir)
                      728 BUILD_LIST               3
                      730 BINARY_OP                0 (+)
          
-          42         734 LOAD_CONST               8 (True)
+          40         734 LOAD_CONST               8 (True)
          
-          40         736 KW_NAMES                 9
+          38         736 KW_NAMES                 9
                      738 PRECALL                  2
                      742 CALL                     2
                      752 POP_TOP
          
-          46         754 LOAD_GLOBAL             21 (NULL + glob)
+          44         754 LOAD_GLOBAL             21 (NULL + glob)
                      766 LOAD_ATTR               10 (glob)
                      776 LOAD_GLOBAL              0 (os)
                      788 LOAD_ATTR                1 (path)
                      798 LOAD_METHOD              5 (join)
                      820 LOAD_FAST                5 (output)
                      822 LOAD_CONST              16 ('*.whl')
                      824 PRECALL                  2
                      828 CALL                     2
                      838 PRECALL                  1
                      842 CALL                     1
                      852 STORE_FAST               8 (wheels)
          
-          47         854 LOAD_GLOBAL             23 (NULL + len)
+          45         854 LOAD_GLOBAL             23 (NULL + len)
                      866 LOAD_FAST                8 (wheels)
                      868 PRECALL                  1
                      872 CALL                     1
                      882 LOAD_CONST              11 (1)
                      884 COMPARE_OP               2 (==)
                      890 POP_JUMP_FORWARD_IF_TRUE     2 (to 896)
                      892 LOAD_ASSERTION_ERROR
                      894 RAISE_VARARGS            1
          
-          48     >>  896 LOAD_FAST                8 (wheels)
+          46     >>  896 LOAD_FAST                8 (wheels)
                      898 LOAD_CONST              12 (0)
                      900 BINARY_SUBSCR
                      910 STORE_FAST               9 (wheel_path_tmp)
          
-          50         912 LOAD_GLOBAL             31 (NULL + print)
+          48         912 LOAD_GLOBAL             31 (NULL + print)
                      924 LOAD_CONST              17 ('copy')
                      926 LOAD_FAST                9 (wheel_path_tmp)
                      928 LOAD_CONST              18 ('to')
                      930 LOAD_FAST                2 (wheel_dir)
                      932 PRECALL                  4
                      936 CALL                     4
                      946 POP_TOP
          
-          52         948 LOAD_GLOBAL             25 (NULL + shutil)
+          50         948 LOAD_GLOBAL             25 (NULL + shutil)
                      960 LOAD_ATTR               13 (copy)
                      970 LOAD_FAST                9 (wheel_path_tmp)
                      972 LOAD_FAST                2 (wheel_dir)
                      974 PRECALL                  2
                      978 CALL                     2
                      988 POP_TOP
          
-          20         990 LOAD_CONST               0 (None)
+          18         990 LOAD_CONST               0 (None)
                      992 LOAD_CONST               0 (None)
                      994 LOAD_CONST               0 (None)
                      996 PRECALL                  2
                     1000 CALL                     2
                     1010 POP_TOP
                     1012 JUMP_FORWARD            11 (to 1036)
                  >> 1014 PUSH_EXC_INFO
@@ -357,15 +333,15 @@
                     1024 POP_EXCEPT
                     1026 RERAISE                  1
                  >> 1028 POP_TOP
                     1030 POP_EXCEPT
                     1032 POP_TOP
                     1034 POP_TOP
          
-          54     >> 1036 LOAD_GLOBAL              0 (os)
+          52     >> 1036 LOAD_GLOBAL              0 (os)
                     1048 LOAD_ATTR                1 (path)
                     1058 LOAD_METHOD             16 (basename)
                     1080 LOAD_FAST                9 (wheel_path_tmp)
                     1082 PRECALL                  1
                     1086 CALL                     1
                     1096 RETURN_VALUE
          ExceptionTable:
@@ -392,57 +368,57 @@
             '*.whl'
             'copy'
             'to'
          names      ('os', 'path', 'dirname', 'tempfile', 'TemporaryDirectory', 'join', 'makedirs', 'subprocess', 'run', 'unlink', 'glob', 'len', 'shutil', 'copy', 'PTH_PATH', 'print', 'basename')
          varnames   ('wheel_path', 'wheel_pack_args', 'wheel_dir', 'tmpdir', 'unpacked', 'output', 'subdirs', 'subdir', 'wheels', 'wheel_path_tmp')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/rpmdyn/custom_build/backend.py'
+         filename   '/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py'
          name       'repack_with_pth'
          firstlineno 13
          lnotab
-            0x020308023e022c0140014001280128023603280364012a011003700316
+            0x020108023e022c0140014001280128023603280364012a011003700316
             01180102fe120664012a01100224022ae02e22
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c007c017c
             02ac01a6030000ab0300000000000000007d037404000000000000000000
             006a030000000000000000a0040000000000000000000000000000000000
             0000007c007c03a6020000ab0200000000000000007d04740b0000000000
             00000000007c04640264036702a6020000ab0200000000000000005300
-          57           0 RESUME                   0
+          55           0 RESUME                   0
          
-          58           2 LOAD_GLOBAL              1 (NULL + buildsys_dateversion)
+          56           2 LOAD_GLOBAL              1 (NULL + buildsys_dateversion)
                       14 LOAD_ATTR                1 (build_editable)
          
-          59          24 LOAD_FAST                0 (wheel_directory)
+          57          24 LOAD_FAST                0 (wheel_directory)
          
-          60          26 LOAD_FAST                1 (config_settings)
+          58          26 LOAD_FAST                1 (config_settings)
          
-          61          28 LOAD_FAST                2 (metadata_directory)
+          59          28 LOAD_FAST                2 (metadata_directory)
          
-          58          30 KW_NAMES                 1
+          56          30 KW_NAMES                 1
                       32 PRECALL                  3
                       36 CALL                     3
                       46 STORE_FAST               3 (basename)
          
-          63          48 LOAD_GLOBAL              4 (os)
+          61          48 LOAD_GLOBAL              4 (os)
                       60 LOAD_ATTR                3 (path)
                       70 LOAD_METHOD              4 (join)
                       92 LOAD_FAST                0 (wheel_directory)
                       94 LOAD_FAST                3 (basename)
                       96 PRECALL                  2
                      100 CALL                     2
                      110 STORE_FAST               4 (path)
          
-          64         112 LOAD_GLOBAL             11 (NULL + repack_with_pth)
+          62         112 LOAD_GLOBAL             11 (NULL + repack_with_pth)
                      124 LOAD_FAST                4 (path)
                      126 LOAD_CONST               2 ('--build-number')
                      128 LOAD_CONST               3 ('0.editable')
                      130 BUILD_LIST               2
                      132 PRECALL                  2
                      136 CALL                     2
                      146 RETURN_VALUE
@@ -451,75 +427,73 @@
             ('config_settings', 'metadata_directory')
             '--build-number'
             '0.editable'
          names      ('buildsys_dateversion', 'build_editable', 'os', 'path', 'join', 'repack_with_pth')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'basename', 'path')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/rpmdyn/custom_build/backend.py'
+         filename   '/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py'
          name       'build_editable'
-         firstlineno 57
+         firstlineno 55
          lnotab 0x020116010201020102fd12054001
       code
          argcount  : 3
          nlocals   : 5
          stacksize : 5
          flags     : 3
          code
             0x97007401000000000000000000006a0100000000000000007c007c017c
             02ac01a6030000ab0300000000000000007d037404000000000000000000
             006a030000000000000000a0040000000000000000000000000000000000
             0000007c007c03a6020000ab0200000000000000007d04740b0000000000
             00000000007c04a6010000ab0100000000000000005300
-          67           0 RESUME                   0
+          65           0 RESUME                   0
          
-          68           2 LOAD_GLOBAL              1 (NULL + buildsys_dateversion)
+          66           2 LOAD_GLOBAL              1 (NULL + buildsys_dateversion)
                       14 LOAD_ATTR                1 (build_wheel)
          
-          69          24 LOAD_FAST                0 (wheel_directory)
+          67          24 LOAD_FAST                0 (wheel_directory)
          
-          70          26 LOAD_FAST                1 (config_settings)
+          68          26 LOAD_FAST                1 (config_settings)
          
-          71          28 LOAD_FAST                2 (metadata_directory)
+          69          28 LOAD_FAST                2 (metadata_directory)
          
-          68          30 KW_NAMES                 1
+          66          30 KW_NAMES                 1
                       32 PRECALL                  3
                       36 CALL                     3
                       46 STORE_FAST               3 (basename)
          
-          73          48 LOAD_GLOBAL              4 (os)
+          71          48 LOAD_GLOBAL              4 (os)
                       60 LOAD_ATTR                3 (path)
                       70 LOAD_METHOD              4 (join)
                       92 LOAD_FAST                0 (wheel_directory)
                       94 LOAD_FAST                3 (basename)
                       96 PRECALL                  2
                      100 CALL                     2
                      110 STORE_FAST               4 (path)
          
-          74         112 LOAD_GLOBAL             11 (NULL + repack_with_pth)
+          72         112 LOAD_GLOBAL             11 (NULL + repack_with_pth)
                      124 LOAD_FAST                4 (path)
                      126 PRECALL                  1
                      130 CALL                     1
                      140 RETURN_VALUE
          consts
             None
             ('config_settings', 'metadata_directory')
          names      ('buildsys_dateversion', 'build_wheel', 'os', 'path', 'join', 'repack_with_pth')
          varnames   ('wheel_directory', 'config_settings', 'metadata_directory', 'basename', 'path')
          freevars   ()
          cellvars   ()
-         filename   '/home/rmcgover/src/rpmdyn/custom_build/backend.py'
+         filename   '/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py'
          name       'build_wheel'
-         firstlineno 67
+         firstlineno 65
          lnotab 0x020116010201020102fd12054001
       (None,)
       (None, None)
-   names      ('os', 'glob', 'shutil', 'subprocess', 'tempfile', 'typing', 'Optional', 'buildsys_dateversion', 'path', 'join', 'PTH_PATH', 'str', 'list', 'repack_with_pth', 'build_editable', 'build_wheel')
+   names      ('glob', 'os', 'shutil', 'subprocess', 'tempfile', 'buildsys_dateversion', 'path', 'join', 'PTH_PATH', 'str', 'repack_with_pth', 'build_editable', 'build_wheel')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/rmcgover/src/rpmdyn/custom_build/backend.py'
+   filename   '/home/runner/work/rpmdyn/rpmdyn/custom_build/backend.py'
    name       '<module>'
    firstlineno 1
-   lnotab
-      0x00ff0201080108010801080108010c0108010802380402ff040102ff02
-      011aff020202fe082c080a
+   lnotab 0x00ff020108010801080108010802080108023803122a080a
```

### Comparing `rpmdyn-2023.5/custom_build/backend.py` & `rpmdyn-2023.5.7/custom_build/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import os
 import glob
+import os
 import shutil
 import subprocess
 import tempfile
-from typing import Optional
+
 import buildsys_dateversion
 from buildsys_dateversion import *
 
 PTH_PATH = os.path.join("src", "rpmdyn", "rpmdyn.pth")
 
 
-def repack_with_pth(
-    wheel_path: str, wheel_pack_args: Optional[list[str]] = None
-) -> str:
+def repack_with_pth(wheel_path: str, wheel_pack_args=None) -> str:
     wheel_pack_args = wheel_pack_args or []
 
     wheel_dir = os.path.dirname(wheel_path)
 
     with tempfile.TemporaryDirectory(prefix="rpmdyn_build") as tmpdir:
         unpacked = os.path.join(tmpdir, "unpacked")
         output = os.path.join(tmpdir, "output")
```

### Comparing `rpmdyn-2023.5/src/rpmdyn/_const.py` & `rpmdyn-2023.5.7/src/rpmdyn/_const.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/src/rpmdyn/_ffi.py` & `rpmdyn-2023.5.7/src/rpmdyn/_ffi.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/src/rpmdyn/_pth_hook.py` & `rpmdyn-2023.5.7/src/rpmdyn/_pth_hook.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/src/rpmdyn/_rpm.py` & `rpmdyn-2023.5.7/src/rpmdyn/_rpm.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/src/rpmdyn/_transaction.py` & `rpmdyn-2023.5.7/src/rpmdyn/_transaction.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/src/rpmdyn.egg-info/SOURCES.txt` & `rpmdyn-2023.5.7/src/rpmdyn.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-requirements.txt
+requirements.in
 custom_build/backend.py
 custom_build/__pycache__/backend.cpython-311.pyc
 src/rpmdyn/__init__.py
 src/rpmdyn/_const.py
 src/rpmdyn/_ffi.py
 src/rpmdyn/_keyring.py
 src/rpmdyn/_pth_hook.py
```

### Comparing `rpmdyn-2023.5/tests/test_headers.py` & `rpmdyn-2023.5.7/tests/test_headers.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/tests/test_labelcompare.py` & `rpmdyn-2023.5.7/tests/test_labelcompare.py`

 * *Files identical despite different names*

### Comparing `rpmdyn-2023.5/tests/test_transactionset.py` & `rpmdyn-2023.5.7/tests/test_transactionset.py`

 * *Files identical despite different names*

