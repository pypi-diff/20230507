# Comparing `tmp/zkt-1.0.2.tar.gz` & `tmp/zkt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zkt-1.0.2.tar", last modified: Fri Apr 28 00:57:38 2023, max compression
+gzip compressed data, was "zkt-1.0.3.tar", last modified: Sun May  7 18:43:51 2023, max compression
```

## Comparing `zkt-1.0.2.tar` & `zkt-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:57:38.746817 zkt-1.0.2/
--rw-rw-rw-   0        0        0     1910 2023-04-28 00:57:38.747814 zkt-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1600 2023-04-28 00:54:41.000000 zkt-1.0.2/README.md
--rw-rw-rw-   0        0        0      115 2023-04-28 00:57:38.750816 zkt-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      631 2023-04-28 00:57:33.000000 zkt-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:57:38.708599 zkt-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:57:38.717651 zkt-1.0.2/src/zkt/
--rw-rw-rw-   0        0        0     2549 2023-04-28 00:23:33.000000 zkt-1.0.2/src/zkt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:57:38.744805 zkt-1.0.2/src/zkt/steps/
--rw-rw-rw-   0        0        0     3000 2023-04-28 00:29:38.000000 zkt-1.0.2/src/zkt/steps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:57:38.742277 zkt-1.0.2/src/zkt.egg-info/
--rw-rw-rw-   0        0        0     1910 2023-04-28 00:57:38.000000 zkt-1.0.2/src/zkt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      228 2023-04-28 00:57:38.000000 zkt-1.0.2/src/zkt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:57:38.000000 zkt-1.0.2/src/zkt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-04-28 00:57:38.000000 zkt-1.0.2/src/zkt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-04-28 00:57:38.000000 zkt-1.0.2/src/zkt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 18:43:51.118953 zkt-1.0.3/
+-rw-rw-rw-   0        0        0     1910 2023-05-07 18:43:51.119948 zkt-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1600 2023-04-28 00:54:41.000000 zkt-1.0.3/README.md
+-rw-rw-rw-   0        0        0      115 2023-05-07 18:43:51.121461 zkt-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      631 2023-05-07 18:42:54.000000 zkt-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:43:51.071356 zkt-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 18:43:51.087881 zkt-1.0.3/src/zkt/
+-rw-rw-rw-   0        0        0     3116 2023-05-07 01:26:36.000000 zkt-1.0.3/src/zkt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:43:51.116941 zkt-1.0.3/src/zkt/steps/
+-rw-rw-rw-   0        0        0     5111 2023-05-07 12:39:41.000000 zkt-1.0.3/src/zkt/steps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 18:43:51.114432 zkt-1.0.3/src/zkt.egg-info/
+-rw-rw-rw-   0        0        0     1910 2023-05-07 18:43:50.000000 zkt-1.0.3/src/zkt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      228 2023-05-07 18:43:50.000000 zkt-1.0.3/src/zkt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 18:43:50.000000 zkt-1.0.3/src/zkt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-07 18:43:50.000000 zkt-1.0.3/src/zkt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-05-07 18:43:50.000000 zkt-1.0.3/src/zkt.egg-info/top_level.txt
```

### Comparing `zkt-1.0.2/PKG-INFO` & `zkt-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper tool for api test automation
 Home-page: UNKNOWN
 Author: Noé Cruz
 Author-email: contactozurckz@gmail.com
 License: MIT
 Keywords: zurckz test testing
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zkt Version: 1.0.2 Summary: Helper tool for api
+Metadata-Version: 2.1 Name: zkt Version: 1.0.3 Summary: Helper tool for api
 test automation Home-page: UNKNOWN Author: NoÃ© Cruz Author-email:
 contactozurckz@gmail.com License: MIT Keywords: zurckz test testing Platform:
 UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
                                    [Zurck'z]
                           Zkt for API Test Automation
 --- # Zkt > Zurck'z Testing Tool This package contains some helpers features
 for api test automation ZPy use the following packages: - zpy-api-core ##
```

### Comparing `zkt-1.0.2/README.md` & `zkt-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `zkt-1.0.2/setup.py` & `zkt-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="zkt",
-    version="1.0.2",
+    version="1.0.3",
     license="MIT",
     author="Noé Cruz",
     author_email="contactozurckz@gmail.com",
     description="Helper tool for api test automation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages("src"),
```

### Comparing `zkt-1.0.2/src/zkt/__init__.py` & `zkt-1.0.3/src/zkt/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 from dataclasses import dataclass
 from enum import Enum
 from time import sleep
 from abc import ABC, abstractmethod
 from typing import Generic, TypeVar
 import traceback
 from zpy.app import zapp_context as ctx
+
+
 class Emoji(Enum):
     GREEN_CIRCLE = "\U0001f7e2"
     BUILDING_CONSTRUCTION = "\U0001f3d7"
     ABACOUS = "\U0001f9ee"
     HIGH_VOLTAGE = "\U000026a1"
     PARTY_POPPER = "\U0001f389"
     CROSS_MARK = "\U0000274c"
     CHECK_MARK = "\U00002705"
+    ALEMBIC = "\U00002697"
 
     def __str__(self) -> str:
         return self.value
 
 
 T = TypeVar("T")
 
@@ -31,34 +34,42 @@
 
 class Step(ABC, Generic[T]):
     def __init__(self, name: str, init_data: dict = {}):
         self.name = name
         self.init_data = init_data
         self.global_data = {}
         self.verbose = False
+        self.terminable = False
 
     @abstractmethod
-    def run(self, input_data: T=None, shared_data: dict = {}) -> OutputStep:
+    def run(self, input_data: T = None, shared_data: dict = {}) -> OutputStep:
         return OutputStep(input_data)
 
 
 class Stepexecutor:
     def __init__(
-        self, scenario: str, steps: list[Step], global_data: dict = {}, verbose: bool = False
+        self,
+        scenario: str,
+        steps: list[Step],
+        global_data: dict = {},
+        verbose: bool = False,
+        end_mapper: Step = None,
     ) -> dict:
         self.scenario = scenario
         self.steps = steps
         self.global_data = global_data
         self.verbose = verbose
+        self.end_map_step = end_mapper
 
-    def execute(self, shared_data: dict = {}) -> dict:
+    def execute(self, shared_data: dict = {}) -> OutputStep:
         print(f"\n\t{Emoji.GREEN_CIRCLE} Scenario: {self.scenario}")
         print(f"\t\t{Emoji.ABACOUS} Summary:")
         print(f"\t\t   {Emoji.HIGH_VOLTAGE} Steps: {len(self.steps)}\n")
         transaction_data = {}
+        normal_exec = True
         for i, step in enumerate(self.steps):
             # print(f"\t\t \U000025b6 {step.name}")
             # sleep(0.7)
             step.global_data = self.global_data
             step.verbose = self.verbose
             try:
                 result = step.run(transaction_data, shared_data)
@@ -70,10 +81,21 @@
                 print(f"\t\t {Emoji.CHECK_MARK} S{i+1}: {step.name}\n")
                 sleep(0.2)
             if result and not result.is_ok:
                 print(f"\t\t {Emoji.CROSS_MARK} S{i+1}: {step.name}\n")
                 sleep(0.2)
             transaction_data = result
             self.global_data = step.global_data
+
+            if type(result) is OutputStep and result.can_continue is False:
+                normal_exec = False
+                break
+
+        if self.end_map_step and normal_exec:
+            print(f"\t\t {Emoji.ALEMBIC} Executing end map step")
+            sleep(0.2)
+            transaction_data = self.end_map_step.run(transaction_data)
+
         sleep(0.5)
         print(f"\n\t{Emoji.PARTY_POPPER} Finished scenario...\n")
+
         return transaction_data
```

### Comparing `zkt-1.0.2/src/zkt.egg-info/PKG-INFO` & `zkt-1.0.3/src/zkt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zkt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper tool for api test automation
 Home-page: UNKNOWN
 Author: Noé Cruz
 Author-email: contactozurckz@gmail.com
 License: MIT
 Keywords: zurckz test testing
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zkt Version: 1.0.2 Summary: Helper tool for api
+Metadata-Version: 2.1 Name: zkt Version: 1.0.3 Summary: Helper tool for api
 test automation Home-page: UNKNOWN Author: NoÃ© Cruz Author-email:
 contactozurckz@gmail.com License: MIT Keywords: zurckz test testing Platform:
 UNKNOWN Requires-Python: >=3.6 Description-Content-Type: text/markdown
                                    [Zurck'z]
                           Zkt for API Test Automation
 --- # Zkt > Zurck'z Testing Tool This package contains some helpers features
 for api test automation ZPy use the following packages: - zpy-api-core ##
```

