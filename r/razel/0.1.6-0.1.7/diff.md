# Comparing `tmp/razel-0.1.6.tar.gz` & `tmp/razel-0.1.7.tar.gz`

## Comparing `razel-0.1.6.tar` & `razel-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.6/version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.6/src/razel/__init__.py
--rw-r--r--   0        0        0    10543 2020-02-02 00:00:00.000000 razel-0.1.6/src/razel/razel.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     5731 2020-02-02 00:00:00.000000 razel-0.1.6/README.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     6298 2020-02-02 00:00:00.000000 razel-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 razel-0.1.7/version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 razel-0.1.7/src/razel/__init__.py
+-rw-r--r--   0        0        0    11156 2020-02-02 00:00:00.000000 razel-0.1.7/src/razel/razel.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 razel-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 razel-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     6258 2020-02-02 00:00:00.000000 razel-0.1.7/README.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 razel-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 razel-0.1.7/PKG-INFO
```

### Comparing `razel-0.1.6/src/razel/razel.py` & `razel-0.1.7/src/razel/razel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 # allows annotations with types that are not yet defined
 from __future__ import annotations
 
 import abc
 import json
 import os
+from enum import Enum
 from typing import ClassVar, Optional, Any, TypeVar
 from collections.abc import Mapping, Sequence
 
 
 class Razel:
-    version: ClassVar[str] = "0.1.6"
+    version: ClassVar[str] = "0.1.7"
     _instance: ClassVar[Optional[Razel]] = None
 
+    class Tag(str, Enum):
+        QUIET = 'razel:quiet'
+        VERBOSE = 'razel:verbose'
+
     def __init__(self, workspace_dir: str) -> None:
         self._workspace_dir = workspace_dir
         self._commands: list[Command] = []
 
     @staticmethod
     def init(workspace_dir: str) -> Razel:
         assert Razel._instance is None
@@ -134,14 +139,15 @@
 class Command(abc.ABC):
     def __init__(self, name: str, inputs: Sequence[File], outputs: Sequence[File]) -> None:
         self._name = name
         self._inputs = inputs
         self._outputs = outputs
         self._stdout: File | None = None
         self._stderr: File | None = None
+        self._tags: Sequence[Razel.Tag | str] = []
         for out in self._outputs:
             out._created_by = self
 
     @property
     def name(self) -> str:
         return self._name
 
@@ -163,14 +169,26 @@
     def stdout(self) -> File | None:
         return self._stdout
 
     @property
     def stderr(self) -> File | None:
         return self._stderr
 
+    @property
+    def tags(self) -> Sequence[Razel.Tag | str]:
+        return self._tags
+
+    def add_tag(self, tag: Razel.Tag | str) -> Command:
+        self._tags.append(tag)
+        return self
+
+    def add_tags(self, tags: Sequence[Razel.Tag | str]) -> Command:
+        self._tags.extend(tags)
+        return self
+
     def ensure_equal(self, other: File | Command) -> None:
         Razel.instance().ensure_equal(self, other)
 
     def ensure_not_equal(self, other: File | Command) -> None:
         Razel.instance().ensure_not_equal(self, other)
 
     @abc.abstractmethod
@@ -241,14 +259,16 @@
         }
         if self.env:
             j["env"] = self.env
         if self._stdout:
             j["stdout"] = self._stdout.file_name
         if self._stderr:
             j["stderr"] = self._stderr.file_name
+        if self._tags:
+            j["tags"] = self._tags
         return j
 
 
 class Task(Command):
     @staticmethod
     def write_file(path: str, lines: Sequence[str]) -> File:
         file = Razel.instance().add_output_file(path)
@@ -266,19 +286,22 @@
         return self._task
 
     @property
     def args(self) -> Sequence[str | File]:
         return self._args
 
     def json(self) -> Mapping[str, Any]:
-        return {
+        j = {
             "name": self.name,
             "task": self.task,
             "args": [x.file_name if isinstance(x, File) else x for x in self.args],
         }
+        if self._tags:
+            j["tags"] = self._tags
+        return j
 
 
 def _map_arg_to_output_path(arg: str | File | Command) -> str:
     if isinstance(arg, Command):
         return arg.output.file_name
     elif isinstance(arg, File):
         return arg.file_name
```

### Comparing `razel-0.1.6/LICENSE.md` & `razel-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `razel-0.1.6/README.md` & `razel-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ![Rust](https://img.shields.io/badge/language-rust-blue.svg)
 [![MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/reu-dev/razel/blob/main/LICENSE.md)
 [![CI](https://github.com/reu-dev/razel/actions/workflows/ci.yml/badge.svg)](https://github.com/reu-dev/razel/actions/workflows/ci.yml)
 
 [![Deno module](https://shield.deno.dev/x/razel)](https://deno.land/x/razel)
 [![Python module](https://img.shields.io/pypi/v/razel.svg)](https://pypi.org/pypi/razel)
+[![Rust crate](https://img.shields.io/crates/v/razel.svg)](https://crates.io/crates/razel)
 
 A command executor with caching. It is:
 
 * Fast: caching avoids repeated execution of commands which haven't changed
 * Reliable: commands are executed in a sandbox to detect missing dependencies
 * Easy to use: commands are specified using a high-level TypeScript or Python API and convenience functions/tasks are
   built-in
@@ -101,22 +102,32 @@
   for testing,
   but it does not support caching and managing dependencies between tests is difficult.
 
 ## Features
 
 ### Measurements
 
-Razel parses the stdout of executed commands to capture runtime measurements and writes them to `razel-out/measurements.csv`.
+Razel parses the stdout of executed commands to capture runtime measurements and writes them to `razel-out/razel-metadata/measurements.csv`.
 Currently, the `<CTestMeasurement>` and `<DartMeasurement>` tags as used by [CTest/CDash](https://cmake.org/cmake/help/latest/command/ctest_test.html#additional-test-measurements) are supported:
 ```
 <CTestMeasurement type="numeric/double" name="score">12.3</CTestMeasurement>
 <CTestMeasurement type="text/string" name="result">ok</CTestMeasurement>
 ```
 Supporting custom formats is planned.
 
+### Tags
+
+Tags can be set on commands. Any custom string can be used as tag, a colon should be used for grouping.
+The tags are added to `razel-out/razel-metadata/execution_times.json`.
+Using tags for filtering commands and creating reports is planned. 
+
+Tags with `razel:` prefix are reserved and have special meaning:
+- `razel:quiet`: don't be verbose if command succeeded
+- `razel:verbose`: always show verbose output
+
 ### Param/Response files
 
 Commands with huge number of arguments might result in command lines which are too long to be executed by the OS.
 Razel detects those cases and replaces the arguments with a response file. The filename starts with @.
 
 ## Acknowledgements
```

### Comparing `razel-0.1.6/pyproject.toml` & `razel-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `razel-0.1.6/PKG-INFO` & `razel-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: razel
-Version: 0.1.6
+Version: 0.1.7
 Summary: a command executor with caching for data processing pipelines
 Project-URL: Homepage, https://github.com/reu-dev/razel
 Project-URL: Bug Tracker, https://github.com/reu-dev/razel/issues
 Author-email: Stefan Reuschl <stefan@reu-dev.de>, Kacper Sagnowski <ksagnowski@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,14 +16,15 @@
 
 ![Rust](https://img.shields.io/badge/language-rust-blue.svg)
 [![MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/reu-dev/razel/blob/main/LICENSE.md)
 [![CI](https://github.com/reu-dev/razel/actions/workflows/ci.yml/badge.svg)](https://github.com/reu-dev/razel/actions/workflows/ci.yml)
 
 [![Deno module](https://shield.deno.dev/x/razel)](https://deno.land/x/razel)
 [![Python module](https://img.shields.io/pypi/v/razel.svg)](https://pypi.org/pypi/razel)
+[![Rust crate](https://img.shields.io/crates/v/razel.svg)](https://crates.io/crates/razel)
 
 A command executor with caching. It is:
 
 * Fast: caching avoids repeated execution of commands which haven't changed
 * Reliable: commands are executed in a sandbox to detect missing dependencies
 * Easy to use: commands are specified using a high-level TypeScript or Python API and convenience functions/tasks are
   built-in
@@ -115,22 +116,32 @@
   for testing,
   but it does not support caching and managing dependencies between tests is difficult.
 
 ## Features
 
 ### Measurements
 
-Razel parses the stdout of executed commands to capture runtime measurements and writes them to `razel-out/measurements.csv`.
+Razel parses the stdout of executed commands to capture runtime measurements and writes them to `razel-out/razel-metadata/measurements.csv`.
 Currently, the `<CTestMeasurement>` and `<DartMeasurement>` tags as used by [CTest/CDash](https://cmake.org/cmake/help/latest/command/ctest_test.html#additional-test-measurements) are supported:
 ```
 <CTestMeasurement type="numeric/double" name="score">12.3</CTestMeasurement>
 <CTestMeasurement type="text/string" name="result">ok</CTestMeasurement>
 ```
 Supporting custom formats is planned.
 
+### Tags
+
+Tags can be set on commands. Any custom string can be used as tag, a colon should be used for grouping.
+The tags are added to `razel-out/razel-metadata/execution_times.json`.
+Using tags for filtering commands and creating reports is planned. 
+
+Tags with `razel:` prefix are reserved and have special meaning:
+- `razel:quiet`: don't be verbose if command succeeded
+- `razel:verbose`: always show verbose output
+
 ### Param/Response files
 
 Commands with huge number of arguments might result in command lines which are too long to be executed by the OS.
 Razel detects those cases and replaces the arguments with a response file. The filename starts with @.
 
 ## Acknowledgements
```

