# Comparing `tmp/struct_gpt-0.2.2.tar.gz` & `tmp/struct_gpt-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-0.2.2.tar", last modified: Sun May  7 09:04:51 2023, max compression
+gzip compressed data, was "struct_gpt-0.3.0.tar", last modified: Sun May  7 09:41:23 2023, max compression
```

## Comparing `struct_gpt-0.2.2.tar` & `struct_gpt-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     3312 2023-05-07 09:04:29.283270 struct_gpt-0.2.2/README.md
--rw-r--r--   0        0        0      512 2023-05-07 09:04:51.259442 struct_gpt-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 07:47:49.753180 struct_gpt-0.2.2/struct_gpt/__init__.py
--rw-r--r--   0        0        0     4539 2023-05-07 08:43:40.720381 struct_gpt-0.2.2/struct_gpt/models.py
--rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 struct_gpt-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     3312 2023-05-07 09:41:05.488531 struct_gpt-0.3.0/README.md
+-rw-r--r--   0        0        0      560 2023-05-07 09:41:23.956816 struct_gpt-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 09:41:05.488531 struct_gpt-0.3.0/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3697 2023-05-07 09:41:05.488531 struct_gpt-0.3.0/struct_gpt/models.py
+-rw-r--r--   0        0        0     1985 2023-05-07 09:41:05.488531 struct_gpt-0.3.0/tests/test_models.py
+-rw-r--r--   0        0        0     3701 1970-01-01 00:00:00.000000 struct_gpt-0.3.0/PKG-INFO
```

### Comparing `struct_gpt-0.2.2/README.md` & `struct_gpt-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `struct_gpt-0.2.2/pyproject.toml` & `struct_gpt-0.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-[tool.pdm]
+[tool.pdm.dev-dependencies]
+dev = [
+    "pytest>=7.3.1",
+]
 
 [project]
 name = "struct-gpt"
-version = "0.2.2"
+version = "0.3.0"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-0.2.2/struct_gpt/models.py` & `struct_gpt-0.3.0/struct_gpt/models.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 Model = TypeVar("Model", bound=BaseModel)
 
 yaml = YAML(typ="safe")
 
 logger = logging.getLogger(__name__)
 
+
 class Example(TypedDict):
     input: str
     output: str
 
 
 class OpenAiMixin:
     @classmethod
@@ -37,15 +38,15 @@
             retries: Number of times to retry in case of failure.
             examples: List of input-output example pairs. Useful to improve the model's accuracy.
             **kwargs: Used to format the model's docstring.
 
         Returns:
             Model instance.
         """
-        assert (
+        assert cls.__doc__ and (
             doc := cls.__doc__.strip()
         ), "please add a docstring explaining how to destructure the prompt"
 
         assert (
             examples or kwargs
         ), "please provide either examples or keyword args for the docstring"
 
@@ -113,44 +114,7 @@
 
         if last_exception:
             raise last_exception
 
 
 class OpenAiBase(BaseModel, OpenAiMixin):
     ...
-
-
-if __name__ == "__main__":
-
-    class SentimentSchema(OpenAiBase):
-        """
-        Determine the sentiment of the given text:
-
-        {content}
-        """
-
-        sentiment: str = Field(description="Either -1, 0, or 1.")
-
-    examples = [
-        {
-            "input": "this library is neat!",
-            "output": SentimentSchema(sentiment="1").json(),
-        },
-        {
-            "input": "don't touch that",
-            "output": SentimentSchema(sentiment="-1").json(),
-        },
-    ]
-
-    positive = SentimentSchema.create(
-        content="I love pizza!",
-    )
-    negative = SentimentSchema.create(
-        content="I hate pizza!",
-        examples=examples,
-    )
-
-    print(f"{positive = }")
-    print(f"{negative = }")
-    # outputs:
-    # positive = SentimentSchema(sentiment='1')
-    # negative = SentimentSchema(sentiment='-1')
```

### Comparing `struct_gpt-0.2.2/PKG-INFO` & `struct_gpt-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: struct-gpt
-Version: 0.2.2
+Version: 0.3.0
 Summary: structured llm outputs
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: MIT
 Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
 Requires-Python: >=3.10
 Requires-Dist: openai>=0.27.6
 Requires-Dist: pydantic>=1.10.7
```

