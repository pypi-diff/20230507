# Comparing `tmp/punctfix-0.0.9.tar.gz` & `tmp/punctfix-0.10.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "punctfix-0.0.9.tar", last modified: Tue Jun 28 10:03:35 2022, max compression
+gzip compressed data, was "punctfix-0.10.0.tar", last modified: Sun May  7 09:11:21 2023, max compression
```

## Comparing `punctfix-0.0.9.tar` & `punctfix-0.10.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 mcni      (1000) mcni      (1000)        0 2022-06-28 10:03:35.262392 punctfix-0.0.9/
--rw-rw-r--   0 mcni      (1000) mcni      (1000)    11358 2022-06-28 09:29:10.000000 punctfix-0.0.9/LICENCE.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       63 2022-06-28 09:29:10.000000 punctfix-0.0.9/MANIFEST.in
--rw-rw-r--   0 mcni      (1000) mcni      (1000)     2411 2022-06-28 10:03:35.262392 punctfix-0.0.9/PKG-INFO
--rw-rw-r--   0 mcni      (1000) mcni      (1000)     1951 2022-06-28 09:29:10.000000 punctfix-0.0.9/README.md
-drwxrwxr-x   0 mcni      (1000) mcni      (1000)        0 2022-06-28 10:03:35.262392 punctfix-0.0.9/punctfix/
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       34 2022-06-28 09:29:10.000000 punctfix-0.0.9/punctfix/__init__.py
--rw-rw-r--   0 mcni      (1000) mcni      (1000)     8204 2022-06-28 09:33:10.000000 punctfix-0.0.9/punctfix/inference.py
--rw-rw-r--   0 mcni      (1000) mcni      (1000)     1753 2022-06-28 09:29:10.000000 punctfix-0.0.9/punctfix/models.py
-drwxrwxr-x   0 mcni      (1000) mcni      (1000)        0 2022-06-28 10:03:35.262392 punctfix-0.0.9/punctfix.egg-info/
--rw-rw-r--   0 mcni      (1000) mcni      (1000)     2411 2022-06-28 10:03:34.000000 punctfix-0.0.9/punctfix.egg-info/PKG-INFO
--rw-rw-r--   0 mcni      (1000) mcni      (1000)      324 2022-06-28 10:03:35.000000 punctfix-0.0.9/punctfix.egg-info/SOURCES.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)        1 2022-06-28 10:03:34.000000 punctfix-0.0.9/punctfix.egg-info/dependency_links.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       44 2022-06-28 10:03:35.000000 punctfix-0.0.9/punctfix.egg-info/requires.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       15 2022-06-28 10:03:35.000000 punctfix-0.0.9/punctfix.egg-info/top_level.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       48 2022-06-28 09:29:10.000000 punctfix-0.0.9/requirements.txt
--rw-rw-r--   0 mcni      (1000) mcni      (1000)       38 2022-06-28 10:03:35.262392 punctfix-0.0.9/setup.cfg
--rw-rw-r--   0 mcni      (1000) mcni      (1000)      846 2022-06-28 09:50:19.000000 punctfix-0.0.9/setup.py
-drwxrwxr-x   0 mcni      (1000) mcni      (1000)        0 2022-06-28 10:03:35.262392 punctfix-0.0.9/tests/
--rw-rw-r--   0 mcni      (1000) mcni      (1000)        0 2022-06-28 09:29:10.000000 punctfix-0.0.9/tests/__init__.py
--rw-rw-r--   0 mcni      (1000) mcni      (1000)    10250 2022-06-28 09:45:30.000000 punctfix-0.0.9/tests/test_punctuation.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.688915 punctfix-0.10.0/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    11358 2023-05-06 18:27:41.000000 punctfix-0.10.0/LICENCE.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       63 2023-05-06 18:27:41.000000 punctfix-0.10.0/MANIFEST.in
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2403 2023-05-07 09:11:21.688915 punctfix-0.10.0/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1979 2023-05-06 18:27:41.000000 punctfix-0.10.0/README.md
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.685582 punctfix-0.10.0/punctfix/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       34 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/__init__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    10211 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/inference.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     1905 2023-05-06 18:27:41.000000 punctfix-0.10.0/punctfix/models.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.685582 punctfix-0.10.0/punctfix.egg-info/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)     2403 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/PKG-INFO
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      324 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/SOURCES.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        1 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/dependency_links.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       44 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/requires.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       15 2023-05-07 09:11:21.000000 punctfix-0.10.0/punctfix.egg-info/top_level.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       48 2023-05-06 18:27:41.000000 punctfix-0.10.0/requirements.txt
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)       38 2023-05-07 09:11:21.688915 punctfix-0.10.0/setup.cfg
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)      847 2023-05-06 18:28:03.000000 punctfix-0.10.0/setup.py
+drwxr-xr-x   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-07 09:11:21.688915 punctfix-0.10.0/tests/
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)        0 2023-05-06 18:27:41.000000 punctfix-0.10.0/tests/__init__.py
+-rw-r--r--   0 sorenmulli  (1000) sorenmulli  (1000)    12449 2023-05-06 18:27:41.000000 punctfix-0.10.0/tests/test_punctuation.py
```

### Comparing `punctfix-0.0.9/LICENCE.txt` & `punctfix-0.10.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `punctfix-0.0.9/PKG-INFO` & `punctfix-0.10.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: punctfix
-Version: 0.0.9
+Version: 0.10.0
 Summary: Punctuation restoration library
 Home-page: https://github.com/danspeech/punctfix
 Author: Martin Carsten Nielsen
 Author-email: martin@alvenir.ai
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Punctuation restoration 
-Adds punctuation and capitalization for a given text.
+Adds punctuation and capitalization for a given text without punctuation.
 
 Works on Danish, German and English. 
 
-Models hosted on huggingface! <3 
+Models hosted on huggingface! ❤️  🤗
 
 ## Status with python 3.8
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/run_tests.yml/badge.svg)
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/pylint.yml/badge.svg)
 
 ## Installation
 ```
@@ -30,18 +28,18 @@
 ```
 
 ## Usage
 Its quite simple to use! 
 
 ```python
 >>> from punctfix import PunctFixer
->>> model = PunctFixer(language="da")
+>>> fixer = PunctFixer(language="da")
 
 >>> example_text = "mit navn det er rasmus og jeg kommer fra firmaet alvenir det er mig som har trænet denne lækre model"
->>> print(model.punctuate(example_text))
+>>> print(fixer.punctuate(example_text))
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
@@ -53,12 +51,10 @@
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
 
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
-then a PR that fixes the issue! ;-) 
+then a PR that fixes the issue! ;-)
 
 Happy punctuating!
-
-
```

### Comparing `punctfix-0.0.9/README.md` & `punctfix-0.10.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Punctuation restoration 
-Adds punctuation and capitalization for a given text.
+Adds punctuation and capitalization for a given text without punctuation.
 
 Works on Danish, German and English. 
 
-Models hosted on huggingface! <3 
+Models hosted on huggingface! ❤️  🤗
 
 ## Status with python 3.8
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/run_tests.yml/badge.svg)
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/pylint.yml/badge.svg)
 
 ## Installation
 ```
@@ -15,18 +15,18 @@
 ```
 
 ## Usage
 Its quite simple to use! 
 
 ```python
 >>> from punctfix import PunctFixer
->>> model = PunctFixer(language="da")
+>>> fixer = PunctFixer(language="da")
 
 >>> example_text = "mit navn det er rasmus og jeg kommer fra firmaet alvenir det er mig som har trænet denne lækre model"
->>> print(model.punctuate(example_text))
+>>> print(fixer.punctuate(example_text))
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
@@ -38,10 +38,10 @@
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
 
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
-then a PR that fixes the issue! ;-) 
+then a PR that fixes the issue! ;-)
 
 Happy punctuating!
```

### Comparing `punctfix-0.0.9/punctfix/inference.py` & `punctfix-0.10.0/punctfix/inference.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,32 @@
 from collections import Counter
 from dataclasses import dataclass
-from typing import Tuple, Dict, List
+from typing import Tuple, Dict, List, Union, Optional
+import warnings
+import re
 
 import torch
 from transformers import TokenClassificationPipeline
 
 from punctfix.models import get_custom_model_and_tokenizer, get_english_model_and_tokenizer, \
     get_danish_model_and_tokenizer, get_german_model_and_tokenizer
 
 
+WORD_NORMALIZATION_PATTERN = re.compile(r"[\W_]+")
+
 class NoLanguageOrModelSelect(Exception):
     """
     Exception raised if you fail to specify either a language or custom model path.
     """
 
+class NonNormalizedTextWarning(RuntimeWarning):
+    """
+    Warning given when the input text does not follow the normalization used
+    during training.
+    """
 
 @dataclass
 class WordPrediction:
     """
     Dataclass to hold word and labels for inference.
     """
     word: str
@@ -36,36 +45,43 @@
 class PunctFixer:
     """
     PunctFixer used to punctuate a given text.
     """
 
     def __init__(self, language: str = "da",
                  custom_model_path: str = None,
+                 use_auth_token: Optional[Union[bool, str]] = None,
                  word_overlap: int = 70,
                  word_chunk_size: int = 100,
-                 device: str = "cpu"):
+                 device: str = "cpu",
+                 skip_normalization=False,
+                 warn_on_normalization=False,):
         """
         :param language: Valid options are "da", "de", "en", for Danish, German and English, respectively.
         :param custom_model_path: If you have a trained model yourself. If parsed, then language param will be ignored.
         :param word_overlap: How many words should overlap in case text is too long. Defaults to 70.
         :param word_chunk_size: How many words should a single pass consist of. Defaults to 100.
         :param device: "cpu" or "cuda" to indicate where to run inference. Defaults to "cpu".
+        :param skip_normalization: Don't check input text and don't normalize it.
+        :param warn_on_normalization: Warn the user if the input text was normalized.
         """
 
         self.word_overlap = word_overlap
         self.word_chunk_size = word_chunk_size
+        self.skip_normalization = skip_normalization
+        self.warn_on_normalization = warn_on_normalization
 
         self.supported_languages = {
             "de": "German",
             "da": "Danish",
             "en": "English"
         }
 
         if custom_model_path:
-            self.model, self.tokenizer = get_custom_model_and_tokenizer(custom_model_path)
+            self.model, self.tokenizer = get_custom_model_and_tokenizer(custom_model_path, use_auth_token)
         elif language == "en":
             self.model, self.tokenizer = get_english_model_and_tokenizer()
         elif language == "da":
             self.model, self.tokenizer = get_danish_model_and_tokenizer()
         elif language == "de":
             self.model, self.tokenizer = get_german_model_and_tokenizer()
         else:
@@ -117,15 +133,15 @@
                 words_in_text = text.split(" ")
 
                 for word in words_in_text:
                     current_index = i * self.word_chunk_size + word_counter - (i * self.word_overlap)
 
                     # Sanity check
                     assert word_prediction_list[current_index].word == word, \
-                        f"Something went wrong due to handling of a long text... " \
+                        f"Something went wrong while matching word list ... " \
                         f"Tried matching the word: {word} with {word_prediction_list[current_index].word}"
                     word_prediction_list[current_index].labels.append(label)
                     word_counter += 1
 
         return word_prediction_list
 
     def combine_word_predictions_into_final_text(self, word_prediction_list: List[WordPrediction]):
@@ -158,30 +174,61 @@
                 range(0, len(words), self.word_chunk_size - self.word_overlap)]
 
     def punctuate(self, text: str) -> str:
         """
         Punctuates given text.
 
         :param text: A lowercase text with no punctuation.
+            If it has punctuatation, it will be removed.
         :return: A punctuated text.
         """
-        words = text.split(" ")
+        words = self._split_input_text(text)
 
         # If we have a long sequence of text (measured by words), we split it into chunks
         chunks = []
         if len(words) >= self.word_chunk_size:
             chunks = self.split_words_into_chunks(words)
         else:
             chunks.append(words)
 
         # We create a word prediction list and then combine the predictions to to final text
         word_prediction_list = self.init_word_prediction_list(words)
         word_prediction_list = self.populate_word_prediction_with_labels(chunks, word_prediction_list)
         return self.combine_word_predictions_into_final_text(word_prediction_list)
 
+    def _split_input_text(self, text: str) -> List[str]:
+        words = text.split(" ")
+        if self.skip_normalization:
+            return words
+
+        normalized_words = []
+        to_warn = []
+        for word in words:
+            if not word:
+                to_warn.append("Additional whitespace was removed.")
+            norm_word = WORD_NORMALIZATION_PATTERN.sub("", word)
+            if not word:
+                continue
+            if len(norm_word) < len(word):
+                to_warn.append(r"Non-word (r'\W') characters were removed.")
+            if not norm_word.islower():
+                norm_word = norm_word.lower()
+                to_warn.append("Text was lowercased.")
+            normalized_words.append(norm_word)
+
+        # Warn once for each type of normalization
+        if self.warn_on_normalization and to_warn:
+            warnings.warn(
+                "The input text was modified to follow model normalization: " +
+                " ".join(sorted(set(to_warn))) +
+                " To avoid seeing this, set suppress_normalization_warning=True. "\
+                "To entirely circumvent normalization, set skip_normalization=True. ",
+                NonNormalizedTextWarning)
+        return normalized_words
+
     @staticmethod
     def _combine_label_and_word(label: str, word: str, auto_uppercase: bool = False) -> Tuple[str, bool]:
         """
         Combines label and word into a single string by looking at the label to see what should be changed.
 
         :param label: Punctuation label from the model
         :param word: Word to handle
@@ -195,11 +242,11 @@
 
         if label[0] != "O":
             word += label[0]
 
         if auto_uppercase:
             word = word.capitalize()
 
-        if label[0] != "0" and label[0] in [".", "!", "?"]:
+        if label[0] in {".", "!", "?"}:
             next_auto_uppercase = True
 
         return word, next_auto_uppercase
```

### Comparing `punctfix-0.0.9/punctfix/models.py` & `punctfix-0.10.0/punctfix/models.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple
+from typing import Tuple, Optional, Union
 
 from transformers import AutoTokenizer, AutoModelForTokenClassification, BertTokenizerFast
 
 
 def get_english_model_and_tokenizer() -> Tuple[AutoModelForTokenClassification, AutoTokenizer]:
     """
     Gets English transformer model and tokenizer
@@ -32,15 +32,18 @@
     """
     model_id = "Alvenir/bert-punct-restoration-de"
     tokenizer = BertTokenizerFast.from_pretrained(model_id)
     model = AutoModelForTokenClassification.from_pretrained(model_id)
     return model, tokenizer
 
 
-def get_custom_model_and_tokenizer(model_path: str) -> Tuple[AutoModelForTokenClassification, AutoTokenizer]:
+def get_custom_model_and_tokenizer(
+        model_path: str,
+        use_auth_token: Optional[Union[bool, str]] = None
+    ) -> Tuple[AutoModelForTokenClassification, AutoTokenizer]:
     """
     Gets local transformer model and tokenizer
     :return: Tuple with (model, tokenizer)
     """
-    model = AutoModelForTokenClassification.from_pretrained(model_path)
-    tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True)
+    model = AutoModelForTokenClassification.from_pretrained(model_path, use_auth_token=use_auth_token)
+    tokenizer = AutoTokenizer.from_pretrained(model_path, use_fast=True, use_auth_token=use_auth_token)
     return model, tokenizer
```

### Comparing `punctfix-0.0.9/punctfix.egg-info/PKG-INFO` & `punctfix-0.10.0/punctfix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 Metadata-Version: 2.1
 Name: punctfix
-Version: 0.0.9
+Version: 0.10.0
 Summary: Punctuation restoration library
 Home-page: https://github.com/danspeech/punctfix
 Author: Martin Carsten Nielsen
 Author-email: martin@alvenir.ai
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Punctuation restoration 
-Adds punctuation and capitalization for a given text.
+Adds punctuation and capitalization for a given text without punctuation.
 
 Works on Danish, German and English. 
 
-Models hosted on huggingface! <3 
+Models hosted on huggingface! ❤️  🤗
 
 ## Status with python 3.8
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/run_tests.yml/badge.svg)
 ![example workflow](https://github.com/danspeech/punctfix/actions/workflows/pylint.yml/badge.svg)
 
 ## Installation
 ```
@@ -30,18 +28,18 @@
 ```
 
 ## Usage
 Its quite simple to use! 
 
 ```python
 >>> from punctfix import PunctFixer
->>> model = PunctFixer(language="da")
+>>> fixer = PunctFixer(language="da")
 
 >>> example_text = "mit navn det er rasmus og jeg kommer fra firmaet alvenir det er mig som har trænet denne lækre model"
->>> print(model.punctuate(example_text))
+>>> print(fixer.punctuate(example_text))
 'Mit navn det er Rasmus og jeg kommer fra firmaet Alvenir. Det er mig som har trænet denne lækre model.'
 
 >>> example_text = "en dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning det fungerer da meget godt ikke"
 >>> print(fixer.punctuate(example_text)) 
 'En dag bliver vi sku glade for, at vi nu kan sætte punktummer og kommaer i en sætning. Det fungerer da meget godt, ikke?' 
 ```
 
@@ -53,12 +51,10 @@
 default values `word_chunk_size=100`, `word_overlap=70` which makes it run a bit slow. The default parameters
 will be updated when we have some results on variations. 
 * Supported languages are "en" for English, "da" for Danish and "de" for German. Default is `language="da"`.
 
 
 ## Contribute
 If you encounter issues, feel free to open issues in the repo and then we will fix. Even better, create issue and 
-then a PR that fixes the issue! ;-) 
+then a PR that fixes the issue! ;-)
 
 Happy punctuating!
-
-
```

### Comparing `punctfix-0.0.9/setup.py` & `punctfix-0.10.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', encoding="utf-8") as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="punctfix",
-    version="0.0.9",
+    version="0.10.0",
     author="Martin Carsten Nielsen",
     author_email="martin@alvenir.ai",
     description="Punctuation restoration library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

### Comparing `punctfix-0.0.9/tests/test_punctuation.py` & `punctfix-0.10.0/tests/test_punctuation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import unittest
 from unittest.mock import patch, MagicMock, ANY
 
 from punctfix import PunctFixer
+from punctfix.inference import NonNormalizedTextWarning
 
 class CleanupDisableTest(unittest.TestCase):
 
     def setUp(self) -> None:
         super().setUp()
         self.model = PunctFixer(language="en")
 
@@ -184,10 +185,53 @@
                                                                         ignore_labels=ANY)
 
     def tearDown(self) -> None:
         super().tearDown()
         self.torch_cuda_patch.stop()
         self.token_classification_pipeline_patch.stop()
 
+class NormalizationTest(unittest.TestCase):
+
+    def setUp(self) -> None:
+        super().setUp()
+        self.model = PunctFixer(language="da")
+
+    def tearDown(self) -> None:
+        super().tearDown()
+        self.model = None
+
+    def test_do_normalize(self):
+        self.model.warn_on_normalization = False
+        expected_output = ["hejsa", "mand"]
+        for model_input in ("hejsa, mand", " hejsa mand", "hejsa mand",
+                "Hejsa mand", "hejsa  mand", "  hejsa mand", "  hejsa, Mand"):
+            actual_output = self.model._split_input_text(model_input)
+            self.assertEqual(actual_output, expected_output)
+
+    def test_warnings(self):
+        self.model.warn_on_normalization = True
+        with self.assertWarns(NonNormalizedTextWarning):
+            model_input = "hejsa, mand"
+            self.model._split_input_text(model_input)
+
+        with self.assertWarns(NonNormalizedTextWarning):
+            model_input = "hejsa  mand"
+            self.model._split_input_text(model_input)
+
+        with self.assertWarns(NonNormalizedTextWarning):
+            model_input = "hejsa  Mand"
+            self.model._split_input_text(model_input)
+
+    def test_do_not_normalize(self):
+        model_input = "det der sker over de tre dage fra præsident huden tav ankommer til københavn det er at der " \
+                      "sådan en bliver spillet sådan et form for tom og jerry kispus mellem københavns politi og " \
+                      "så de har danske demonstranter for tibet og fåfalungongsom meget gerne vil vise deres " \
+                      "utilfredshed med det kinesiske regime og det de opfatter som undertrykkelse af de her " \
+                      "mindretal i kine og lige nu står støttekomiteen for ti bedet bag en demonstration på" \
+                      " højbro plads i københavn lisbeth davidsen hvor mange er der kommet det er ikke " \
+                      "de store folkemasser der er mødt op her på"
+        expected_output = model_input.split(" ")
+        actual_output = self.model._split_input_text(model_input)
+        self.assertEqual(actual_output, expected_output)
 
 if __name__ == '__main__':
     unittest.main()
```

