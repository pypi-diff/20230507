# Comparing `tmp/struct_gpt-0.1.2.tar.gz` & `tmp/struct_gpt-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-0.1.2.tar", last modified: Sun May  7 08:18:30 2023, max compression
+gzip compressed data, was "struct_gpt-0.2.0.tar", last modified: Sun May  7 08:55:23 2023, max compression
```

## Comparing `struct_gpt-0.1.2.tar` & `struct_gpt-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1232 2023-05-07 08:18:27.804688 struct_gpt-0.1.2/README.md
--rw-r--r--   0        0        0      512 2023-05-07 08:18:30.136546 struct_gpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.1.2/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4539 2023-05-07 07:41:39.445343 struct_gpt-0.1.2/struct_gpt/models.py
--rw-r--r--   0        0        0     1621 1970-01-01 00:00:00.000000 struct_gpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2211 2023-05-07 08:54:34.065400 struct_gpt-0.2.0/README.md
+-rw-r--r--   0        0        0      512 2023-05-07 08:55:23.793667 struct_gpt-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.2.0/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4539 2023-05-07 08:43:40.720381 struct_gpt-0.2.0/struct_gpt/models.py
+-rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 struct_gpt-0.2.0/PKG-INFO
```

### Comparing `struct_gpt-0.1.2/pyproject.toml` & `struct_gpt-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "struct-gpt"
-version = "0.1.2"
+version = "0.2.0"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-0.1.2/struct_gpt/models.py` & `struct_gpt-0.2.0/struct_gpt/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import io
 import json
 import logging
-from typing import TypeVar, Literal, Mapping
+from typing import TypeVar, TypedDict
 
 import openai
 from pydantic import BaseModel, Field, ValidationError
 from ruamel.yaml import YAML
 
 Model = TypeVar("Model", bound=BaseModel)
-Example = Mapping[Literal["input", "output"], str]
 
 yaml = YAML(typ="safe")
 
 logger = logging.getLogger(__name__)
 
+class Example(TypedDict):
+    input: str
+    output: str
+
 
 class OpenAiMixin:
     @classmethod
     def create(
         cls: Model,
         temperature=0,
         model="gpt-3.5-turbo",
```

### Comparing `struct_gpt-0.1.2/PKG-INFO` & `struct_gpt-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,15 @@
-Metadata-Version: 2.1
-Name: struct-gpt
-Version: 0.1.2
-Summary: structured llm outputs
-Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
-License: MIT
-Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
-Requires-Python: >=3.10
-Requires-Dist: openai>=0.27.6
-Requires-Dist: pydantic>=1.10.7
-Requires-Dist: ruamel-yaml>=0.17.24
-Description-Content-Type: text/markdown
-
 # struct-gpt
 
 structured llm outputs
 
 ## Usage
 
+Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
+
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
@@ -35,58 +24,89 @@
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
 
+Your classes can reference one another. You can also use the `OpenAiMixin` to add functionality to your own classes.
+
 ```python
-class SentimentAnalysis(OpenAiBase):
+from struct_gpt import OpenAiBase, OpenAiMixin
+from pydantic import Field, BaseModel
+from typing import Mapping
+
+class SentimentSchema(OpenAiBase):
+    """
+    Determine the sentiment of the given text:
+
+    {content}
+    """
+
+    sentiment: str = Field(description="Either -1, 0, or 1.")
+
+# you can use the OpenAiMixin to add functionality to your own classes
+class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
+
+    Also determine the overall sentiment of the text and who the narrator is.
     """
 
-    sentiment: Mapping[str, SentimentSchema]
+    words_to_sentiment: Mapping[str, SentimentSchema]
+    overall_sentiment: SentimentSchema
+    narrator: str = Field(description="The narrator of the text.")
 
 
-analysis = SentimentAnalysis.create(
-    text="I love the beautiful scenery, but the long hike was exhausting."
+print(
+    SentimentAnalysis.create(
+        text="As president, I loved the beautiful scenery, but the long hike was exhausting."
+    ).json(indent=2)
 )
-print(analysis.json(indent=2))
 ```
 outputs:
 ```json
 {
-  "sentiment": {
-    "I": {
+  "words_to_sentiment": {
+    "As": {
+      "sentiment": "0"
+    },
+    "president,": {
       "sentiment": "1"
     },
-    "love": {
+    "I": {
+      "sentiment": "0"
+    },
+    "loved": {
       "sentiment": "1"
     },
     "the": {
       "sentiment": "0"
     },
     "beautiful": {
       "sentiment": "1"
     },
     "scenery,": {
       "sentiment": "1"
     },
     "but": {
-      "sentiment": "0"
+      "sentiment": "-1"
     },
     "long": {
       "sentiment": "-1"
     },
     "hike": {
       "sentiment": "-1"
     },
     "was": {
       "sentiment": "0"
     },
     "exhausting.": {
       "sentiment": "-1"
     }
-  }
+  },
+  "overall_sentiment": {
+    "sentiment": "0"
+  },
+  "narrator": "president"
 }
 ```
```

