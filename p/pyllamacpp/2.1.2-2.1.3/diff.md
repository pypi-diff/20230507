# Comparing `tmp/pyllamacpp-2.1.2.tar.gz` & `tmp/pyllamacpp-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-2.1.2.tar", last modified: Thu May  4 03:40:06 2023, max compression
+gzip compressed data, was "pyllamacpp-2.1.3.tar", last modified: Sun May  7 00:23:35 2023, max compression
```

## Comparing `pyllamacpp-2.1.2.tar` & `pyllamacpp-2.1.3.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-04 03:39:57.000000 pyllamacpp-2.1.2/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.613970 pyllamacpp-2.1.2/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.621970 pyllamacpp-2.1.2/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.625970 pyllamacpp-2.1.2/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.617970 pyllamacpp-2.1.2/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12464 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7449 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 03:40:06.000000 pyllamacpp-2.1.2/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 03:40:06.629970 pyllamacpp-2.1.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/llama.cpp_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27757 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-04 03:39:56.000000 pyllamacpp-2.1.2/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-07 00:23:24.000000 pyllamacpp-2.1.3/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.964303 pyllamacpp-2.1.3/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.972303 pyllamacpp-2.1.3/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.968303 pyllamacpp-2.1.3/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12982 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7454 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 00:23:35.000000 pyllamacpp-2.1.3/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 00:23:35.980304 pyllamacpp-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 00:23:35.976304 pyllamacpp-2.1.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/llama.cpp_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    28402 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-07 00:23:22.000000 pyllamacpp-2.1.3/src/main.h
```

### Comparing `pyllamacpp-2.1.2/CMakeLists.txt` & `pyllamacpp-2.1.3/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/LICENSE` & `pyllamacpp-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/PKG-INFO` & `pyllamacpp-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
@@ -204,15 +204,15 @@
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 # FAQs
 * [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
-* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [pyllamacpp does not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
 * [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
 
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
```

### Comparing `pyllamacpp-2.1.2/README.md` & `pyllamacpp-2.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -191,15 +191,15 @@
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 # FAQs
 * [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
-* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [pyllamacpp does not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
 * [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
 
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
```

### Comparing `pyllamacpp-2.1.2/llama.cpp/CMakeLists.txt` & `pyllamacpp-2.1.3/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-2.1.3/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/LICENSE` & `pyllamacpp-2.1.3/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/attr.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/cast.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/chrono.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/complex.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/eigen.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/embed.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/eval.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/functional.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/gil.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/iostream.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/numpy.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/operators.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/options.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/stl.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-2.1.3/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-2.1.3/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/FindCatch.cmake` & `pyllamacpp-2.1.3/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-2.1.3/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-2.1.3/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/check-style.sh` & `pyllamacpp-2.1.3/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-2.1.3/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/libsize.py` & `pyllamacpp-2.1.3/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/make_changelog.py` & `pyllamacpp-2.1.3/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-2.1.3/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-2.1.3/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-2.1.3/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-2.1.3/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/setup_global.py.in` & `pyllamacpp-2.1.3/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pybind11/tools/setup_main.py.in` & `pyllamacpp-2.1.3/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyllamacpp/_logger.py` & `pyllamacpp-2.1.3/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyllamacpp/cli.py` & `pyllamacpp-2.1.3/pyllamacpp/cli.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyllamacpp/model.py` & `pyllamacpp-2.1.3/pyllamacpp/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,14 +107,30 @@
         """Resets the context"""
         self._prompt_context_tokens = pp.llama_tokenize(self._ctx, self.prompt_cntext, True)
         self._prompt_prefix_tokens = pp.llama_tokenize(self._ctx, self.prompt_prefix, True)
         self._prompt_suffix_tokens = pp.llama_tokenize(self._ctx, self.prompt_suffix, True)
         self._last_n_tokens = [0] * self._n_ctx  # n_ctx elements
         self._n_past = 0
 
+    def tokenize(self, text:str):
+        """
+        Returns a list of tokens for the text
+        :param text: text to be tokenized
+        :return: List of tokens
+        """
+        return pp.llama_tokenize(self._ctx, text, True)
+
+    def detokenize(self, tokens:list):
+        """
+        Returns a list of tokens for the text
+        :param text: text to be tokenized
+        :return: A string representing the text extracted from the tokens
+        """
+        return pp.llama_tokens_to_str(self._ctx, tokens)
+
     def generate(self,
                  prompt: str,
                  n_predict: Union[None, int] = None,
                  antiprompt: str = None,
                  infinite_generation: bool = False,
                  n_threads: int = 4,
                  repeat_last_n: int = 64,
```

### Comparing `pyllamacpp-2.1.2/pyllamacpp/utils.py` & `pyllamacpp-2.1.3/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyllamacpp/webui.py` & `pyllamacpp-2.1.3/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-2.1.3/pyllamacpp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 2.1.2
+Version: 2.1.3
 Summary: Python bindings for llama.cpp
 Author: Abdeladim Sadiki
 License: MIT
 Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
 Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
 Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
 Requires-Python: >=3.8
@@ -204,15 +204,15 @@
 All functions from `llama.h` are exposed with the binding module [`_pyllamacpp`](https://abdeladim-s.github.io/pyllamacpp/#_pyllamacpp).
 
 # API reference
 You can check the [API reference documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
 # FAQs
 * [How to build pyllamacpp without AVX2 or FMA.](https://github.com/nomic-ai/pygpt4all/issues/71)
-* [pyllamacpp not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
+* [pyllamacpp does not support M1 chips MacBook](https://github.com/nomic-ai/pygpt4all/issues/57#issuecomment-1519197837)
 * [ImportError: DLL failed while importing _pyllamacpp](https://github.com/nomic-ai/pygpt4all/issues/53#issuecomment-1529772010)
 
 # Discussions and contributions
 If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
 
 If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
```

### Comparing `pyllamacpp-2.1.2/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-2.1.3/pyllamacpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/pyproject.toml` & `pyllamacpp-2.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/setup.py` & `pyllamacpp-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="2.1.2",
+    version="2.1.3",
     author="Abdeladim Sadiki",
     description="Python bindings for llama.cpp",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
```

### Comparing `pyllamacpp-2.1.2/src/llama.cpp_LICENSE` & `pyllamacpp-2.1.3/src/llama.cpp_LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-2.1.2/src/main.cpp` & `pyllamacpp-2.1.3/src/main.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,35 @@
 //    py::array_t<llama_token> tokens;
 //    py::buffer_info buf = tokens.request();
 //    llama_token *tokens_ptr = static_cast<llama_token *>(buf.ptr);
 //    llama_tokenize(ctx, text, tokens_ptr, n_max_tokens, add_bos);
 //    return tokens;
 //}
 
+std::string llama_tokens_to_str_wrapper(struct llama_context_wrapper* ctx_w, py::array_t<llama_token> tokens_array) {
+    std::string result;
+    struct llama_context * ctx = ctx_w->ptr;
+    bool all_tokens_valid = true;
+
+    for (int i = 0; i < tokens_array.size(); i++) {
+        llama_token token = tokens_array.at(i);
+        if (token >= llama_n_vocab(ctx)) {
+            all_tokens_valid = false;
+            break;
+        }
+
+        result += llama_token_to_str(ctx, token);
+    }
 
+    if (all_tokens_valid) {
+        return result;
+    } else {
+        return "";
+    }
+}
 
 int llama_n_vocab_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
     return llama_n_vocab(ctx);
 }
 int llama_n_ctx_wrapper(struct llama_context_wrapper * ctx_w){
     struct llama_context * ctx = ctx_w->ptr;
@@ -693,14 +713,16 @@
     m.def("llama_get_embeddings", &llama_get_embeddings_wrapper);
     m.def("llama_token_to_str", [](struct llama_context_wrapper * ctx_w, llama_token token){
         //@NOTE: model.generate() calls pp.llama_token_to_str -> llama_token_to_str_wrapper()
         //@NOTE: we need to make sure that llama_token_to_str_wrapper() returns raw bytes
         //@NOTE: to prevent implicit conversion of const char* to unicode on python side, leading to UnicodeDecodeError
         return py::bytes(llama_token_to_str_wrapper(ctx_w, token));
     });
+    m.def("llama_tokens_to_str", &llama_tokens_to_str_wrapper);
+
 
     m.def("llama_token_bos", &llama_token_bos);
     m.def("llama_token_eos", &llama_token_eos);
 
     m.def("llama_sample_top_p_top_k", &llama_sample_top_p_top_k_wrapper);
 
     m.def("llama_print_timings", &llama_print_timings_wrapper);
```

### Comparing `pyllamacpp-2.1.2/src/main.h` & `pyllamacpp-2.1.3/src/main.h`

 * *Files identical despite different names*

