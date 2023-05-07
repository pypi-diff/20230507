# Comparing `tmp/struct_gpt-0.2.0.tar.gz` & `tmp/struct_gpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-0.2.0.tar", last modified: Sun May  7 08:55:23 2023, max compression
+gzip compressed data, was "struct_gpt-0.2.2.tar", last modified: Sun May  7 09:04:51 2023, max compression
```

## Comparing `struct_gpt-0.2.0.tar` & `struct_gpt-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2211 2023-05-07 08:54:34.065400 struct_gpt-0.2.0/README.md
--rw-r--r--   0        0        0      512 2023-05-07 08:55:23.793667 struct_gpt-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.2.0/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4539 2023-05-07 08:43:40.720381 struct_gpt-0.2.0/struct_gpt/models.py
--rw-r--r--   0        0        0     2600 1970-01-01 00:00:00.000000 struct_gpt-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3312 2023-05-07 09:04:29.283270 struct_gpt-0.2.2/README.md
+-rw-r--r--   0        0        0      512 2023-05-07 09:04:51.259442 struct_gpt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.2.2/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     4539 2023-05-07 08:43:40.720381 struct_gpt-0.2.2/struct_gpt/models.py
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 struct_gpt-0.2.2/PKG-INFO
```

### Comparing `struct_gpt-0.2.0/README.md` & `struct_gpt-0.2.2/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -59,15 +59,17 @@
 
 print(
     SentimentAnalysis.create(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
-outputs:
+<details>
+<summary>outputs</summary>
+
 ```json
 {
   "words_to_sentiment": {
     "As": {
       "sentiment": "0"
     },
     "president,": {
@@ -106,7 +108,48 @@
   },
   "overall_sentiment": {
     "sentiment": "0"
   },
   "narrator": "president"
 }
 ```
+
+</details>
+
+## Improving reliability with examples
+
+`create` can accept a list of examples to guide the model and improve its accuracy. Each example is a dictionary containing an `input` and `output` key. The `input` is the user message and the `output` is the expected assistant message, which should be a valid instance of the schema serialized as a string.
+
+In this example, we are providing the model with examples of positive and negative sentiments:
+
+```python
+from struct_gpt import OpenAiBase
+from pydantic import Field
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
+examples = [
+    {
+        "input": "this library is neat!",
+        "output": SentimentSchema(sentiment="1").json(),
+    },
+    {
+        "input": "don't touch that",
+        "output": SentimentSchema(sentiment="-1").json(),
+    },
+]
+
+print(SentimentSchema.create(content="I love pizza!", examples=examples).json())
+```
+outputs:
+```json
+{
+  "sentiment": "1"
+}
+```
```

### Comparing `struct_gpt-0.2.0/pyproject.toml` & `struct_gpt-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "struct-gpt"
-version = "0.2.0"
+version = "0.2.2"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-0.2.0/struct_gpt/models.py` & `struct_gpt-0.2.2/struct_gpt/models.py`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.2.0/PKG-INFO` & `struct_gpt-0.2.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 0.2.0
+Version: 0.2.2
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
 Requires-Python: >=3.10
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
@@ -72,15 +72,17 @@
 
 print(
     SentimentAnalysis.create(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
-outputs:
+<details>
+<summary>outputs</summary>
+
 ```json
 {
   "words_to_sentiment": {
     "As": {
       "sentiment": "0"
     },
     "president,": {
@@ -119,7 +121,48 @@
   },
   "overall_sentiment": {
     "sentiment": "0"
   },
   "narrator": "president"
 }
 ```
+
+</details>
+
+## Improving reliability with examples
+
+`create` can accept a list of examples to guide the model and improve its accuracy. Each example is a dictionary containing an `input` and `output` key. The `input` is the user message and the `output` is the expected assistant message, which should be a valid instance of the schema serialized as a string.
+
+In this example, we are providing the model with examples of positive and negative sentiments:
+
+```python
+from struct_gpt import OpenAiBase
+from pydantic import Field
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
+examples = [
+    {
+        "input": "this library is neat!",
+        "output": SentimentSchema(sentiment="1").json(),
+    },
+    {
+        "input": "don't touch that",
+        "output": SentimentSchema(sentiment="-1").json(),
+    },
+]
+
+print(SentimentSchema.create(content="I love pizza!", examples=examples).json())
+```
+outputs:
+```json
+{
+  "sentiment": "1"
+}
+```
```

