# Comparing `tmp/pyaxetool-1.1.0.tar.gz` & `tmp/pyaxetool-1.1.1.tar.gz`

## Comparing `pyaxetool-1.1.0.tar` & `pyaxetool-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/.gitignore
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/LICENSE
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/README.md
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/TODO.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4855 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/CMake.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/MD5.py
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/PyInstaller.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PyAxeTool/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/oldbak/MANIFEST.in
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/oldbak/setup.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pyaxetool-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      732 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/.gitignore
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/LICENSE
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/TODO.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/PyAxeTool/CMake.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/PyAxeTool/MD5.py
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/PyAxeTool/PyInstaller.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/PyAxeTool/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/oldbak/MANIFEST.in
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/oldbak/setup.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 pyaxetool-1.1.1/PKG-INFO
```

### Comparing `pyaxetool-1.1.0/.gitignore` & `pyaxetool-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.1.0/LICENSE` & `pyaxetool-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.1.0/pyproject.toml` & `pyaxetool-1.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "PyAxeTool"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="Sun Jin", email="412640665@qq.com" },
 ]
 description = "An utility tool collection for make life easily"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `pyaxetool-1.1.0/PyAxeTool/CMake.py` & `pyaxetool-1.1.1/PyAxeTool/CMake.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 install(TARGETS $(fuba) 
   ARCHIVE DESTINATION lib
   LIBRARY DESTINATION lib)
 install(DIRECTORY ${CMAKE_SOURCE_DIR}/include/ DESTINATION include)
 """
     test_CMakeLists_content = """SetupGTest()
 
-AddTest(test_$(fuba) $(fuba))
+AddTest($(fuba)_test $(fuba))
 """
     cmake_CMakeUtil = """#================================================================
 # 安装gtest 
 #================================================================
 macro(SetupGTest)
   include(ExternalProject)
   
@@ -85,22 +85,22 @@
 int Sum(int a, int b) {
   return a + b;
 }
 
 }  // namespace $(fuba)
 """
 
-    test_lib_cc = """#include "$(fuba)/$(fuba).h"
+    lib_test_cc = """#include "$(fuba)/$(fuba).h"
 
 #include <iostream>
 
 #include "gtest/gtest.h"
 
-TEST(test_$(fuba), Sum) {
-  EXPECT_TRUE(foo::Sum(1, 2) == 3);
+TEST($(fuba)_test, Sum) {
+  EXPECT_TRUE($(fuba)::Sum(1, 2) == 3);
 }
 """
     if args.libname is None:
         print('missing --libname=<LIBNAME>')
         sys.exit(1)
     print(args.libname)
     
@@ -117,15 +117,15 @@
         AFile.write(os.path.join('src', 'CMakeLists.txt'), AStr.format(src_CMakeLists_content, '$(', ')', **fu_ba_map), 'utf8')
         AFile.write(os.path.join('test', 'CMakeLists.txt'), AStr.format(test_CMakeLists_content, '$(', ')', **fu_ba_map), 'utf8')
         AFile.write(os.path.join('cmake', 'CMakeUtil.cmake'), cmake_CMakeUtil, 'utf8')
         
         # 源码相关
         AFile.write(os.path.join('include', fu_ba_map['fuba'], fu_ba_map['fuba']+'.h'), AStr.format(lib_h, '$(', ')', **fu_ba_map), 'utf8')
         AFile.write(os.path.join('src', fu_ba_map['fuba']+'.cc'), AStr.format(lib_cc, '$(', ')', **fu_ba_map), 'utf8')
-        AFile.write(os.path.join('test', 'test_'+fu_ba_map['fuba']+'.cc'), AStr.format(test_lib_cc, '$(', ')', **fu_ba_map), 'utf8')
+        AFile.write(os.path.join('test', fu_ba_map['fuba']+'_test.cc'), AStr.format(lib_test_cc, '$(', ')', **fu_ba_map), 'utf8')
     
 def handle_sub_cmd_archetype_generate(args):
     funcs = {
         'lib': handle_sub_cmd_archetype_generate_lib,
     }
     funcs[args.archetype](args)
```

### Comparing `pyaxetool-1.1.0/PyAxeTool/MD5.py` & `pyaxetool-1.1.1/PyAxeTool/MD5.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.1.0/PyAxeTool/PyInstaller.py` & `pyaxetool-1.1.1/PyAxeTool/PyInstaller.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.1.0/oldbak/setup.py` & `pyaxetool-1.1.1/oldbak/setup.py`

 * *Files identical despite different names*

### Comparing `pyaxetool-1.1.0/PKG-INFO` & `pyaxetool-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaxetool
-Version: 1.1.0
+Version: 1.1.1
 Summary: An utility tool collection for make life easily
 Project-URL: Bug Tracker, https://github.com/sunjinopensource/PyAxeTool/issues
 Project-URL: Homepage, https://github.com/sunjinopensource/PyAxeTool
 Author-email: Sun Jin <412640665@qq.com>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

