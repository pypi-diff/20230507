# Comparing `tmp/khl-2.0.0.tar.gz` & `tmp/khl-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khl-2.0.0.tar", max compression
+gzip compressed data, was "khl-2.0.1.tar", max compression
```

## Comparing `khl-2.0.0.tar` & `khl-2.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-2.0.0/LICENSE
--rw-r--r--   0        0        0     5409 2023-04-23 14:40:41.764203 khl-2.0.0/README.md
--rw-r--r--   0        0        0     2266 2023-04-23 14:40:56.976257 khl-2.0.0/khl/__init__.py
--rw-r--r--   0        0        0     8710 2023-04-23 14:40:41.764203 khl-2.0.0/khl/preprocess.py
--rw-r--r--   0        0        0     2416 2023-04-23 09:41:56.980021 khl-2.0.0/khl/stop_words.py
--rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-2.0.0/khl/teams_orgs.py
--rw-r--r--   0        0        0    31158 2023-04-23 14:40:41.764203 khl-2.0.0/khl/utils.py
--rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-2.0.0/khl/wrong_lemmas.py
--rw-r--r--   0        0        0     1589 2023-04-23 14:41:12.808314 khl-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6354 1970-01-01 00:00:00.000000 khl-2.0.0/setup.py
--rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 khl-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-05 17:17:58.027493 khl-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5409 2023-04-23 14:40:41.764203 khl-2.0.1/README.md
+-rw-r--r--   0        0        0     2266 2023-05-07 18:36:39.540094 khl-2.0.1/khl/__init__.py
+-rw-r--r--   0        0        0     8710 2023-04-23 14:40:41.764203 khl-2.0.1/khl/preprocess.py
+-rw-r--r--   0        0        0     2404 2023-05-07 18:35:48.387914 khl-2.0.1/khl/stop_words.py
+-rw-r--r--   0        0        0     3274 2023-03-10 16:26:00.431309 khl-2.0.1/khl/teams_orgs.py
+-rw-r--r--   0        0        0    31158 2023-05-07 07:36:57.031042 khl-2.0.1/khl/utils.py
+-rw-r--r--   0        0        0     8346 2023-03-05 17:17:58.031493 khl-2.0.1/khl/wrong_lemmas.py
+-rw-r--r--   0        0        0     1589 2023-05-07 18:36:45.048113 khl-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6354 1970-01-01 00:00:00.000000 khl-2.0.1/setup.py
+-rw-r--r--   0        0        0     6132 1970-01-01 00:00:00.000000 khl-2.0.1/PKG-INFO
```

### Comparing `khl-2.0.0/LICENSE` & `khl-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/README.md` & `khl-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/khl/__init__.py` & `khl-2.0.1/khl/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Подготовка русскоязычных текстов хоккейных новостей для обучения нейронных сетей."""
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 
 from typing import Dict, List, Optional
 
 from khl import preprocess, utils
 from khl.stop_words import stop_words
```

### Comparing `khl-2.0.0/khl/preprocess.py` & `khl-2.0.1/khl/preprocess.py`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/khl/stop_words.py` & `khl-2.0.1/khl/stop_words.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,14 @@
     "красивый",
     "кряду",
     "ли",
     "мало",
     "менее",
     "много",
     "мой",
-    "на",
     "наверно",
     "наверное",
     "наш",
     "немало",
     "немного",
     "неплохой",
     "несколько",
```

### Comparing `khl-2.0.0/khl/teams_orgs.py` & `khl-2.0.1/khl/teams_orgs.py`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/khl/utils.py` & `khl-2.0.1/khl/utils.py`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/khl/wrong_lemmas.py` & `khl-2.0.1/khl/wrong_lemmas.py`

 * *Files identical despite different names*

### Comparing `khl-2.0.0/pyproject.toml` & `khl-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "khl"
-version = "2.0.0"
+version = "2.0.1"
 description = "Preparing russian hockey news for machine learning"
 readme = "README.md"
 license = "MIT"
 authors = ["Rishat Fayzullin <nilluziaf@gmail.com>"]
 repository = "https://github.com/Rishat-F/khl"
 keywords = ["khl", "news", "nlp", "preprocessing", "ml"]
```

### Comparing `khl-2.0.0/setup.py` & `khl-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['natasha==1.4.0']
 
 setup_kwargs = {
     'name': 'khl',
-    'version': '2.0.0',
+    'version': '2.0.1',
     'description': 'Preparing russian hockey news for machine learning',
     'long_description': '![Khl Logo](https://raw.githubusercontent.com/Rishat-F/khl/master/data/logo.png)\n\n<h1 align="center">No Water - Ice Only</h1>\n\nPreparing russian hockey news for machine learning.\n\n**Unify -> Simplify -> Preprocess** text and feed your neural model.\n\n## Installation\n\n*Khl* is available on PyPI:\n\n```console\n$ pip install khl\n```\nIt requires Python 3.8+ to run.\n\n## Usage\n\nTo get started right away with basic usage:\n\n```python\nfrom khl import text_to_codes\n\ncoder = {\n    \'\': 0,     # placeholder\n    \'???\': 1,  # unknown\n    \'.\': 2,\n    \'и\': 3,\n    \'в\': 4,\n    \'-\': 5,\n    \':\': 6,\n    \'матч\': 7,\n    \'за\': 8,\n    \'забить\': 9,\n    \'гол\': 10,\n    \'per\': 11,   # person entity\n    \'org\': 12,   # organization entity\n    \'loc\': 13,   # location entity\n    \'date\': 14,  # date entity\n    \'против\': 15,\n    \'год\': 16,\n    \'pers\': 17,  # few persons entity\n    \'orgs\': 18,  # few organizations entity\n    \'свой\': 19\n}\n\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n\ncodes = text_to_codes(\n    text=text,\n    coder=coder,\n    stop_words_=["за", "и", "свой"],  # stop words to drop\n    replace_ners_=True,               # replace named entities ("Иван Иванов" -> "per", "Спартак" -> "org", "Москва" -> "loc")\n    replace_dates_=True,              # replace dates ("1 апреля 2023 года" -> "date")\n    replace_penalties_=True,          # replace penalties ("5+20" -> "pen")\n    exclude_unknown=True,             # drop lemma that not presented in coder\n    max_len=20,                       # get sequence of codes of length 20\n)\n# codes = [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n```text_to_codes``` is a very high level function. What\'s happens under hood see in [Lower level usage](#lower-level-usage).\n\n## What is `coder`?\n`coder` is just a dictionary where each lemma is represented with unique integer code.\nNote that first two elements are reserved for *placeholder* and *unknown* elements.\n\nIt is possible to get `coder` from frequency dictionary file (see in [Get lemmas coder](#2-get-lemmas-coder)).\nFrequency dictionary file is a **json**-file with dictionary where key is lemma and value is how many times this lemma occurred in your whole dataset.\nPreferably it should be sorted in descending order of values.  \n`example_frequency_dictionary.json`:\n\n```json\n{\n  ".": 1000,\n  "и": 500,\n  "в": 400,\n  "-": 300,\n  ":": 300,\n  "матч": 290,\n  "за": 250,\n  "забить": 240,\n  "гол": 230,\n  "per": 200,\n  "org": 150,\n  "loc": 150,\n  "date": 100,\n  "против": 90,\n  "год": 70,\n  "pers": 40,\n  "orgs": 30,\n  "свой": 20\n}\n```\n\nYou could make and use your own frequency dictionary or download [this dictionary](https://github.com/Rishat-F/khl/blob/master/data/frequency_dictionary.json) created by myself.\n\n## Lower level usage<a id="lower-level-usage"></a>\n\n#### 1. Make imports\n```python\nfrom khl import stop_words\nfrom khl import utils\nfrom khl import preprocess\n```\n\n#### 2. Get lemmas coder<a id="2-get-lemmas-coder"></a>\n```python\ncoder = preprocess.get_coder("example_frequency_dictionary.json")\n```\n\n#### 3. Define text\n```python\ntext = """\n    1 апреля 2023 года в Москве в матче ⅛ финала против „Спартака” Иван Иванов забил свой 100—й гол за карьеру.\n    «Динамо Мск» - «Спартак» 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров.\n"""\n```\n\n#### 4. Unify\n```python\nunified_text = utils.unify(text)\n# "1 апреля 2023 года в Москве в матче 1/8 финала против \'Спартака\' Иван Иванов забил свой 100-й гол за карьеру. \'Динамо Мск\' - \'Спартак\' 2:1 ОТ (1:0 0:1 0:0 1:0) Голы забили: Иванов, Петров и Сидоров."\n```\n\n#### 5. Simplify\n```python\nsimplified_text = utils.simplify(\n    text=unified_text,\n    replace_ners_=True,\n    replace_dates_=True,\n    replace_penalties_=True,\n)\n# \'date в loc в матче финала против org per забил свой гол за карьеру. org org Голы забили: per per per.\'\n```\n\n#### 6. Lemmatize\n```python\nlemmas = preprocess.lemmatize(text=simplified_text, stop_words_=stop_words)\n# [\'date\', \'в\', \'loc\', \'в\', \'матч\', \'финал\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'карьера\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n\n#### 7. Transform to codes\n```python\ncodes = preprocess.lemmas_to_codes(\n    lemmas=lemmas,\n    coder=coder,\n    exclude_unknown=True,\n    max_len=20,\n)\n# [0, 0, 0, 14, 4, 13, 4, 7, 15, 12, 11, 9, 10, 2, 18, 10, 9, 6, 17, 2]\n```\n\n#### 8. Transform to lemmas back (just to look which lemmas are presented in codes sequence)\n```python\nprint(\n    preprocess.codes_to_lemmas(codes=codes, coder=coder)\n)\n# [\'\', \'\', \'\', \'date\', \'в\', \'loc\', \'в\', \'матч\', \'против\', \'org\', \'per\', \'забить\', \'гол\', \'.\', \'orgs\', \'гол\', \'забить\', \':\', \'pers\', \'.\']\n```\n',
     'author': 'Rishat Fayzullin',
     'author_email': 'nilluziaf@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Rishat-F/khl',
```

### Comparing `khl-2.0.0/PKG-INFO` & `khl-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khl
-Version: 2.0.0
+Version: 2.0.1
 Summary: Preparing russian hockey news for machine learning
 Home-page: https://github.com/Rishat-F/khl
 License: MIT
 Keywords: khl,news,nlp,preprocessing,ml
 Author: Rishat Fayzullin
 Author-email: nilluziaf@gmail.com
 Requires-Python: >=3.8,<4.0
```

