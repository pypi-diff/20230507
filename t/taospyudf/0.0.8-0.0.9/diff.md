# Comparing `tmp/taospyudf-0.0.8.tar.gz` & `tmp/taospyudf-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taospyudf-0.0.8.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "taospyudf-0.0.9.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `taospyudf-0.0.8.tar` & `taospyudf-0.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.clang-format
--rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.github/dependabot.yml
--rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.github/workflows/conda.yml
--rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.github/workflows/pip.yml
--rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.github/workflows/wheels.yml
--rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 taospyudf-0.0.8/.vscode/settings.json
--rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 taospyudf-0.0.8/CMakeLists.txt
--rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 taospyudf-0.0.8/LICENSE
--rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 taospyudf-0.0.8/README.md
--rw-r--r--   0        0        0      472 2022-11-09 12:37:21.000000 taospyudf-0.0.8/conda.recipe/meta.yaml
--rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/AndroidAppender.h
--rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/ColorConsoleAppender.h
--rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/ConsoleAppender.h
--rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/DebugOutputAppender.h
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/DynamicAppender.h
--rw-r--r--   0        0        0     3924 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/EventLogAppender.h
--rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/IAppender.h
--rw-r--r--   0        0        0     4143 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Appenders/RollingFileAppender.h
--rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Converters/NativeEOLConverter.h
--rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Converters/UTF8Converter.h
--rw-r--r--   0        0        0     2183 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Formatters/CsvFormatter.h
--rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Formatters/FuncMessageFormatter.h
--rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Formatters/MessageOnlyFormatter.h
--rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Formatters/TxtFormatter.h
--rw-r--r--   0        0        0     1098 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Helpers/AscDump.h
--rw-r--r--   0        0        0     2184 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Helpers/HexDump.h
--rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Helpers/PrintVar.h
--rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Init.h
--rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Initializers/ConsoleInitializer.h
--rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Initializers/RollingFileInitializer.h
--rw-r--r--   0        0        0    11648 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Log.h
--rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Logger.h
--rw-r--r--   0        0        0    12150 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Record.h
--rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Severity.h
--rw-r--r--   0        0        0    15314 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/Util.h
--rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 taospyudf-0.0.8/extern/plog/include/plog/WinApi.h
--rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 taospyudf-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    21954 2022-11-09 12:37:21.000000 taospyudf-0.0.8/src/taospyudf.cpp
--rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 taospyudf-0.0.8/src/taospyudf.h
--rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 taospyudf-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     2623 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.clang-format
+-rw-r--r--   0        0        0      162 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      922 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.github/workflows/conda.yml
+-rw-r--r--   0        0        0      589 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.github/workflows/pip.yml
+-rw-r--r--   0        0        0     1590 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0       64 2022-11-09 12:37:21.000000 taospyudf-0.0.9/.vscode/settings.json
+-rw-r--r--   0        0        0      683 2022-11-09 12:37:21.000000 taospyudf-0.0.9/CMakeLists.txt
+-rw-r--r--   0        0        0     1065 2022-11-09 12:37:21.000000 taospyudf-0.0.9/LICENSE
+-rw-r--r--   0        0        0      330 2022-11-09 12:37:21.000000 taospyudf-0.0.9/README.md
+-rw-r--r--   0        0        0      472 2022-11-09 12:37:21.000000 taospyudf-0.0.9/conda.recipe/meta.yaml
+-rw-r--r--   0        0        0     1193 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/AndroidAppender.h
+-rw-r--r--   0        0        0     3367 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/ColorConsoleAppender.h
+-rw-r--r--   0        0        0     2103 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/ConsoleAppender.h
+-rw-r--r--   0        0        0      370 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/DebugOutputAppender.h
+-rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/DynamicAppender.h
+-rw-r--r--   0        0        0     3924 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/EventLogAppender.h
+-rw-r--r--   0        0        0      243 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/IAppender.h
+-rw-r--r--   0        0        0     4143 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Appenders/RollingFileAppender.h
+-rw-r--r--   0        0        0     1017 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Converters/NativeEOLConverter.h
+-rw-r--r--   0        0        0      565 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Converters/UTF8Converter.h
+-rw-r--r--   0        0        0     2183 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Formatters/CsvFormatter.h
+-rw-r--r--   0        0        0      512 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Formatters/FuncMessageFormatter.h
+-rw-r--r--   0        0        0      435 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Formatters/MessageOnlyFormatter.h
+-rw-r--r--   0        0        0     1631 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Formatters/TxtFormatter.h
+-rw-r--r--   0        0        0     1098 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Helpers/AscDump.h
+-rw-r--r--   0        0        0     2184 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Helpers/HexDump.h
+-rw-r--r--   0        0        0     1674 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Helpers/PrintVar.h
+-rw-r--r--   0        0        0      522 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Init.h
+-rw-r--r--   0        0        0      750 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Initializers/ConsoleInitializer.h
+-rw-r--r--   0        0        0     3285 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Initializers/RollingFileInitializer.h
+-rw-r--r--   0        0        0    11648 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Log.h
+-rw-r--r--   0        0        0     2033 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Logger.h
+-rw-r--r--   0        0        0    12150 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Record.h
+-rw-r--r--   0        0        0     1197 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Severity.h
+-rw-r--r--   0        0        0    15314 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/Util.h
+-rw-r--r--   0        0        0     6125 2022-11-09 12:37:21.000000 taospyudf-0.0.9/extern/plog/include/plog/WinApi.h
+-rw-r--r--   0        0        0      997 2022-11-09 12:37:21.000000 taospyudf-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    22085 2022-11-09 12:37:21.000000 taospyudf-0.0.9/src/taospyudf.cpp
+-rw-r--r--   0        0        0     1636 2022-11-09 12:37:21.000000 taospyudf-0.0.9/src/taospyudf.h
+-rw-r--r--   0        0        0     1019 2022-11-09 12:37:21.000000 taospyudf-0.0.9/PKG-INFO
```

### Comparing `taospyudf-0.0.8/.clang-format` & `taospyudf-0.0.9/.clang-format`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/.github/workflows/conda.yml` & `taospyudf-0.0.9/.github/workflows/conda.yml`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/.github/workflows/pip.yml` & `taospyudf-0.0.9/.github/workflows/pip.yml`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/.github/workflows/wheels.yml` & `taospyudf-0.0.9/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/CMakeLists.txt` & `taospyudf-0.0.9/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/LICENSE` & `taospyudf-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/AndroidAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/AndroidAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/ColorConsoleAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/ColorConsoleAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/ConsoleAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/ConsoleAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/DynamicAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/DynamicAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/EventLogAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/EventLogAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Appenders/RollingFileAppender.h` & `taospyudf-0.0.9/extern/plog/include/plog/Appenders/RollingFileAppender.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Converters/NativeEOLConverter.h` & `taospyudf-0.0.9/extern/plog/include/plog/Converters/NativeEOLConverter.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Converters/UTF8Converter.h` & `taospyudf-0.0.9/extern/plog/include/plog/Converters/UTF8Converter.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Formatters/CsvFormatter.h` & `taospyudf-0.0.9/extern/plog/include/plog/Formatters/CsvFormatter.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Formatters/FuncMessageFormatter.h` & `taospyudf-0.0.9/extern/plog/include/plog/Formatters/FuncMessageFormatter.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Formatters/TxtFormatter.h` & `taospyudf-0.0.9/extern/plog/include/plog/Formatters/TxtFormatter.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Helpers/AscDump.h` & `taospyudf-0.0.9/extern/plog/include/plog/Helpers/AscDump.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Helpers/HexDump.h` & `taospyudf-0.0.9/extern/plog/include/plog/Helpers/HexDump.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Helpers/PrintVar.h` & `taospyudf-0.0.9/extern/plog/include/plog/Helpers/PrintVar.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Init.h` & `taospyudf-0.0.9/extern/plog/include/plog/Init.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Initializers/ConsoleInitializer.h` & `taospyudf-0.0.9/extern/plog/include/plog/Initializers/ConsoleInitializer.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Initializers/RollingFileInitializer.h` & `taospyudf-0.0.9/extern/plog/include/plog/Initializers/RollingFileInitializer.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Log.h` & `taospyudf-0.0.9/extern/plog/include/plog/Log.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Logger.h` & `taospyudf-0.0.9/extern/plog/include/plog/Logger.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Record.h` & `taospyudf-0.0.9/extern/plog/include/plog/Record.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Severity.h` & `taospyudf-0.0.9/extern/plog/include/plog/Severity.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/Util.h` & `taospyudf-0.0.9/extern/plog/include/plog/Util.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/extern/plog/include/plog/WinApi.h` & `taospyudf-0.0.9/extern/plog/include/plog/WinApi.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/pyproject.toml` & `taospyudf-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core", "pybind11"]
 build-backend = "scikit_build_core.build"
 
 
 [project]
 name = "taospyudf"
-version = "0.0.8"
+version = "0.0.9"
 description="taos python udf"
 readme = "README.md"
 authors = [
   { name = "taos data", email = "slzhou@taosdata.com" },
 ]
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `taospyudf-0.0.8/src/taospyudf.cpp` & `taospyudf-0.0.9/src/taospyudf.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,22 @@
 
  public:
   virtual void loadFunctions() {
     _init = _module.attr("init");
     _destroy = _module.attr("destroy");
   }
 
+  virtual void init() {
+    _init();
+  }
+
+  virtual void destroy() {
+    _destroy();
+  }
+
   virtual ~PyUdf() {}
 
   static PyUdf *createPyUdf(const SScriptUdfInfo *udfInfo);
 
  protected:
   py::module_ _module;
   std::string _name;
@@ -448,27 +456,29 @@
 }
 
 int32_t doPyUdfInit(SScriptUdfInfo *udf, void **pUdfCtx) {
   PLOGD << "python udf init. path: " << udf->path << ", name: " << udf->name;
   try {
     PyUdf *pyUdf = PyUdf::createPyUdf(udf);
     pyUdf->loadFunctions();
+    pyUdf->init();
     *pUdfCtx = pyUdf;
   } catch (std::exception &e) {
     PLOGE << "call pyUdf init function. error " << e.what();
     return TSDB_UDF_PYTHON_EXEC_FAILURE;
   }
   PLOGI << "python udf init. name " << udf->name << ". context: " << static_cast<void *>(*pUdfCtx);
   return 0;
 }
 
 int32_t doPyUdfDestroy(void *udfCtx) {
   PLOGD << "python udf destory. context: " << static_cast<void *>(udfCtx);
   try {
     PyUdf *pyUdf = static_cast<PyUdf *>(udfCtx);
+    pyUdf->destroy();
     delete pyUdf;
   } catch (std::exception &e) {
     PLOGE << "call pyUdf destory function. error " << e.what();
     return TSDB_UDF_PYTHON_EXEC_FAILURE;
   }
   return 0;
 }
```

### Comparing `taospyudf-0.0.8/src/taospyudf.h` & `taospyudf-0.0.9/src/taospyudf.h`

 * *Files identical despite different names*

### Comparing `taospyudf-0.0.8/PKG-INFO` & `taospyudf-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taospyudf
-Version: 0.0.8
+Version: 0.0.9
 Summary: taos python udf
 Author-Email: taos data <slzhou@taosdata.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

