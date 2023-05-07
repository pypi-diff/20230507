# Comparing `tmp/struct_gpt-1.0.1.tar.gz` & `tmp/struct_gpt-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "struct_gpt-1.0.1.tar", last modified: Sun May  7 19:58:03 2023, max compression
+gzip compressed data, was "struct_gpt-2.0.0.tar", last modified: Sun May  7 20:28:41 2023, max compression
```

## Comparing `struct_gpt-1.0.1.tar` & `struct_gpt-2.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     3625 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/README.md
--rw-r--r--   0        0        0      583 2023-05-07 19:58:03.008738 struct_gpt-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/struct_gpt/__init__.py
--rw-r--r--   0        0        0     3839 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/struct_gpt/models.py
--rw-r--r--   0        0        0     4177 2023-05-07 19:57:24.756725 struct_gpt-1.0.1/tests/test_models.py
--rw-r--r--   0        0        0     4014 1970-01-01 00:00:00.000000 struct_gpt-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3647 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/README.md
+-rw-r--r--   0        0        0      583 2023-05-07 20:28:41.456481 struct_gpt-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/struct_gpt/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/struct_gpt/models.py
+-rw-r--r--   0        0        0     4222 2023-05-07 20:27:58.323813 struct_gpt-2.0.0/tests/test_models.py
+-rw-r--r--   0        0        0     4036 1970-01-01 00:00:00.000000 struct_gpt-2.0.0/PKG-INFO
```

### Comparing `struct_gpt-1.0.1/README.md` & `struct_gpt-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,23 @@
+Metadata-Version: 2.1
+Name: struct-gpt
+Version: 2.0.0
+Summary: structured llm outputs
+Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
+License: MIT
+Project-URL: Source, https://github.com/knowsuchagency/struct-gpt
+Requires-Python: >=3.10
+Requires-Dist: openai>=0.27.6
+Requires-Dist: pydantic>=1.10.7
+Requires-Dist: ruamel-yaml>=0.17.24
+Description-Content-Type: text/markdown
+
 # struct-gpt
 
+
 [![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
 
 ## Features
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
@@ -16,24 +30,26 @@
 
 Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
-print(SentimentSchema.create(content="I love pizza!").json())
+
+print(SentimentSchema.from_openai(content="I love pizza!").json())
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
@@ -41,38 +57,40 @@
 Your classes can reference one another. You can also use the `OpenAiMixin` to add functionality to your own classes.
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
+
 # you can use the OpenAiMixin to add functionality to your own classes
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
 
     Also determine the overall sentiment of the text and who the narrator is.
     """
 
     words_to_sentiment: Mapping[str, SentimentSchema]
     overall_sentiment: SentimentSchema
     narrator: str
 
 
 print(
-    SentimentAnalysis.create(
+    SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
 <details>
 <summary>outputs</summary>
 
@@ -131,35 +149,37 @@
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
+
 examples = [
     {
         "input": "this library is neat!",
         "output": SentimentSchema(sentiment="1").json(),
     },
     {
         "input": "don't touch that",
         "output": SentimentSchema(sentiment="-1").json(),
     },
 ]
 
-print(SentimentSchema.create(content="I love pizza!", examples=examples).json())
+print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
```

### Comparing `struct_gpt-1.0.1/pyproject.toml` & `struct_gpt-2.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 dev = [
     "pytest>=7.3.1",
     "coverage>=7.2.5",
 ]
 
 [project]
 name = "struct-gpt"
-version = "1.0.1"
+version = "2.0.0"
 description = "structured llm outputs"
 authors = [
     { name = "Stephan Fitzpatrick", email = "knowsuchagency@gmail.com" },
 ]
 dependencies = [
     "openai>=0.27.6",
     "pydantic>=1.10.7",
```

### Comparing `struct_gpt-1.0.1/struct_gpt/models.py` & `struct_gpt-2.0.0/struct_gpt/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 class Example(TypedDict):
     input: str
     output: str
 
 
 class OpenAiMixin:
     @classmethod
-    def create(
+    def from_openai(
         cls: Model,
         temperature=0,
         model="gpt-3.5-turbo",
         retries=2,
         examples: list[Example] = None,
         **kwargs,
     ) -> Model:
```

### Comparing `struct_gpt-1.0.1/tests/test_models.py` & `struct_gpt-2.0.0/tests/test_models.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,35 +36,35 @@
     """
 
     words_to_sentiment: Mapping[str, SentimentSchema]
     overall_sentiment: SentimentSchema
     narrator: str
 
 def test_SentimentSchema_create():
-    sentiment = SentimentSchema.create(content="I love pizza!", examples=EXAMPLES)
+    sentiment = SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
     assert sentiment.sentiment == "1"
 
 def test_SentimentAnalysis_create():
-    sentiment_analysis = SentimentAnalysis.create(
+    sentiment_analysis = SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting.",
         examples=EXAMPLES
     )
     assert sentiment_analysis.narrator.lower() == "president"
     assert sentiment_analysis.overall_sentiment.sentiment in ["-1", "0", "1"]
     assert all(word in sentiment_analysis.words_to_sentiment for word in ["As", "president,", "I", "loved", "the", "beautiful", "scenery,", "but", "long", "hike", "was", "exhausting."])
 
 
 def test_create_with_no_examples_or_kwargs():
     with pytest.raises(AssertionError):
         # call create without providing examples or kwargs
-        SentimentSchema.create()
+        SentimentSchema.from_openai()
 
 def test_no_docstring_raises_exception():
     with pytest.raises(AssertionError) as e:
-        OpenAiBase.create(content="I love pizza!", examples=EXAMPLES)
+        OpenAiBase.from_openai(content="I love pizza!", examples=EXAMPLES)
         assert "please add a docstring" in str(e)
 
 def test_incorrect_example_format_raises_exception():
     incorrect_examples = [
         {
             "input": "this library is neat!",
             # missing output key
@@ -72,38 +72,38 @@
         {
             # missing input key
             "output": '{"sentiment": "1"}',
         },
     ]
 
     with pytest.raises(KeyError):
-        SentimentSchema.create(content="I love pizza!", examples=incorrect_examples)
+        SentimentSchema.from_openai(content="I love pizza!", examples=incorrect_examples)
 
 @mock.patch("openai.ChatCompletion.create")
 def test_openai_api_failure_raises_exception(mock_chat_completion):
     # Arrange: Mock the OpenAI API to simulate a failure
     class OpenAiError(Exception):
         pass
 
     mock_chat_completion.side_effect = OpenAiError("API request failed")
 
     # Act and Assert: Ensure that the OpenAI error is propagated
     with pytest.raises(OpenAiError):
-        SentimentSchema.create(content="I love pizza!", examples=EXAMPLES)
+        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES)
 
 def test_create_with_invalid_temperature_raises_exception():
     with pytest.raises(AssertionError):
         # temperature should be between 0 and 1
-        SentimentSchema.create(content="I love pizza!", examples=EXAMPLES, temperature=-1)
+        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, temperature=-1)
 
 
 def test_create_with_invalid_retries_raises_exception():
     with pytest.raises(AssertionError):
         # retries should be a non-negative integer
-        SentimentSchema.create(content="I love pizza!", examples=EXAMPLES, retries=-1)
+        SentimentSchema.from_openai(content="I love pizza!", examples=EXAMPLES, retries=-1)
 
 def test_create_with_invalid_json():
     class DummyModel(BaseModel, OpenAiMixin):
         """
         Example model for testing
 
         {content}
@@ -123,8 +123,8 @@
                         })
                     }
                 }
             ]
         }
 
         with pytest.raises(ValidationError):
-            DummyModel.create(content="")
+            DummyModel.from_openai(content="")
```

### Comparing `struct_gpt-1.0.1/PKG-INFO` & `struct_gpt-2.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,10 @@
-Metadata-Version: 2.1
-Name: struct-gpt
-Version: 1.0.1
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
 
+
 [![codecov](https://codecov.io/gh/knowsuchagency/struct-gpt/branch/main/graph/badge.svg?token=TMUQNTCTDI)](https://codecov.io/gh/knowsuchagency/struct-gpt)
 
 ## Features
 
 * Easy creation of custom models using the OpenAI API
 * Integration with Pydantic for model validation and serialization
 * Flexible configuration with retries and temperature settings
@@ -29,24 +17,26 @@
 
 Template variables in the class' docstring are replaced with the keyword arguments passed to `create`.
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
-print(SentimentSchema.create(content="I love pizza!").json())
+
+print(SentimentSchema.from_openai(content="I love pizza!").json())
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
@@ -54,38 +44,40 @@
 Your classes can reference one another. You can also use the `OpenAiMixin` to add functionality to your own classes.
 
 ```python
 from struct_gpt import OpenAiBase, OpenAiMixin
 from pydantic import Field, BaseModel
 from typing import Mapping
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
+
 # you can use the OpenAiMixin to add functionality to your own classes
 class SentimentAnalysis(BaseModel, OpenAiMixin):
     """
     Determine the sentiment of each word in the following: {text}
 
     Also determine the overall sentiment of the text and who the narrator is.
     """
 
     words_to_sentiment: Mapping[str, SentimentSchema]
     overall_sentiment: SentimentSchema
     narrator: str
 
 
 print(
-    SentimentAnalysis.create(
+    SentimentAnalysis.from_openai(
         text="As president, I loved the beautiful scenery, but the long hike was exhausting."
     ).json(indent=2)
 )
 ```
 <details>
 <summary>outputs</summary>
 
@@ -144,35 +136,37 @@
 
 In this example, we are providing the model with examples of positive and negative sentiments:
 
 ```python
 from struct_gpt import OpenAiBase
 from pydantic import Field
 
+
 class SentimentSchema(OpenAiBase):
     """
     Determine the sentiment of the given text:
 
     {content}
     """
 
     sentiment: str = Field(description="Either -1, 0, or 1.")
 
+
 examples = [
     {
         "input": "this library is neat!",
         "output": SentimentSchema(sentiment="1").json(),
     },
     {
         "input": "don't touch that",
         "output": SentimentSchema(sentiment="-1").json(),
     },
 ]
 
-print(SentimentSchema.create(content="I love pizza!", examples=examples).json())
+print(SentimentSchema.from_openai(content="I love pizza!", examples=examples).json())
 ```
 outputs:
 ```json
 {
   "sentiment": "1"
 }
 ```
```

