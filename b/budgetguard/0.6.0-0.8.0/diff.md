# Comparing `tmp/budgetguard-0.6.0.tar.gz` & `tmp/budgetguard-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetguard-0.6.0.tar", max compression
+gzip compressed data, was "budgetguard-0.8.0.tar", max compression
```

## Comparing `budgetguard-0.6.0.tar` & `budgetguard-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       23 2023-05-07 17:09:02.484878 budgetguard-0.6.0/budgetguard/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.248599 budgetguard-0.6.0/budgetguard/budgetguard/pipelines/__init__.py
--rw-r--r--   0        0        0      352 2023-05-03 17:14:30.249601 budgetguard-0.6.0/budgetguard/budgetguard/pipelines/base.py
--rw-r--r--   0        0        0        0 2023-05-03 17:14:30.249601 budgetguard-0.6.0/budgetguard/budgetguard/scripts/__init__.py
--rw-r--r--   0        0        0      513 2023-05-05 00:11:56.001550 budgetguard-0.6.0/budgetguard/tests/__init__.py
--rw-r--r--   0        0        0     1022 2023-05-04 23:02:25.622629 budgetguard-0.6.0/budgetguard/tests/test_dummy.py
--rw-r--r--   0        0        0     1235 2023-05-03 11:46:24.500492 budgetguard-0.6.0/LICENSE
--rw-r--r--   0        0        0      704 2023-05-07 17:09:02.496876 budgetguard-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      712 2023-05-06 00:24:12.216445 budgetguard-0.6.0/README.md
--rw-r--r--   0        0        0     1220 1970-01-01 00:00:00.000000 budgetguard-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-07 17:22:54.378658 budgetguard-0.8.0/LICENSE
+-rw-r--r--   0        0        0      680 2023-05-07 17:22:54.378658 budgetguard-0.8.0/README.md
+-rw-r--r--   0        0        0       22 2023-05-07 17:24:06.962719 budgetguard-0.8.0/budgetguard/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/pipelines/__init__.py
+-rw-r--r--   0        0        0      335 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/pipelines/base.py
+-rw-r--r--   0        0        0        0 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/budgetguard/scripts/__init__.py
+-rw-r--r--   0        0        0      493 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/tests/__init__.py
+-rw-r--r--   0        0        0      994 2023-05-07 17:22:54.378658 budgetguard-0.8.0/budgetguard/tests/test_dummy.py
+-rw-r--r--   0        0        0      610 2023-05-07 17:24:06.962719 budgetguard-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1113 1970-01-01 00:00:00.000000 budgetguard-0.8.0/PKG-INFO
```

### Comparing `budgetguard-0.6.0/LICENSE` & `budgetguard-0.8.0/LICENSE`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-This is free and unencumbered software released into the public domain.
-
-Anyone is free to copy, modify, publish, use, compile, sell, or
-distribute this software, either in source code form or as a compiled
-binary, for any purpose, commercial or non-commercial, and by any
-means.
-
-In jurisdictions that recognize copyright laws, the author or authors
-of this software dedicate any and all copyright interest in the
-software to the public domain. We make this dedication for the benefit
-of the public at large and to the detriment of our heirs and
-successors. We intend this dedication to be an overt act of
-relinquishment in perpetuity of all present and future rights to this
-software under copyright law.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
-IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
-OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
-ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
-OTHER DEALINGS IN THE SOFTWARE.
-
-For more information, please refer to <https://unlicense.org>
+This is free and unencumbered software released into the public domain.
+
+Anyone is free to copy, modify, publish, use, compile, sell, or
+distribute this software, either in source code form or as a compiled
+binary, for any purpose, commercial or non-commercial, and by any
+means.
+
+In jurisdictions that recognize copyright laws, the author or authors
+of this software dedicate any and all copyright interest in the
+software to the public domain. We make this dedication for the benefit
+of the public at large and to the detriment of our heirs and
+successors. We intend this dedication to be an overt act of
+relinquishment in perpetuity of all present and future rights to this
+software under copyright law.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
+IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
+OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
+ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
+OTHER DEALINGS IN THE SOFTWARE.
+
+For more information, please refer to <https://unlicense.org>
```

### Comparing `budgetguard-0.6.0/README.md` & `budgetguard-0.8.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,47 @@
-
-# BudgetGuard
-[![codecov](https://codecov.io/gh/M-Borsuk/BudgetGuard/branch/main/graph/badge.svg?token=BudgetGuard_token_here)](https://codecov.io/gh/M-Borsuk/BudgetGuard)
-[![CI](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml/badge.svg)](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml)
-
-BudgetGuard created by M-Borsuk
-
-## Install it from PyPI
-
-```bash
-pip install budgetguard
-```
-
-## Usage
-
-```py
-from budgetguard import BaseClass
-from budgetguard import base_function
-
-BaseClass().base_method()
-base_function()
-```
-
-```bash
-$ python -m budgetguard
-#or
-$ budgetguard
-```
-
-## Development
-
-Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+Metadata-Version: 2.1
+Name: budgetguard
+Version: 0.8.0
+Summary: 
+Author: Mateusz Borsuk
+Author-email: mtszborsuk212@gmail.com
+Requires-Python: >=3.8.8,<4.0.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pyspark (==3.2.0)
+Description-Content-Type: text/markdown
+
+
+# BudgetGuard
+[![codecov](https://codecov.io/gh/M-Borsuk/BudgetGuard/branch/main/graph/badge.svg?token=BudgetGuard_token_here)](https://codecov.io/gh/M-Borsuk/BudgetGuard)
+[![CI](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml/badge.svg)](https://github.com/M-Borsuk/BudgetGuard/actions/workflows/main.yml)
+
+BudgetGuard created by M-Borsuk
+
+## Install it from PyPI
+
+```bash
+pip install budgetguard
+```
+
+## Usage
+
+```py
+from budgetguard import BaseClass
+from budgetguard import base_function
+
+BaseClass().base_method()
+base_function()
+```
+
+```bash
+$ python -m budgetguard
+#or
+$ budgetguard
+```
+
+## Development
+
+Read the [CONTRIBUTING.md](CONTRIBUTING.md) file.
+
```

