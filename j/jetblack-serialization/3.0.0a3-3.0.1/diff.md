# Comparing `tmp/jetblack-serialization-3.0.0a3.tar.gz` & `tmp/jetblack-serialization-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jetblack-serialization-3.0.0a3.tar", max compression
+gzip compressed data, was "jetblack-serialization-3.0.1.tar", max compression
```

## Comparing `jetblack-serialization-3.0.0a3.tar` & `jetblack-serialization-3.0.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2022-04-27 09:50:02.686185 jetblack-serialization-3.0.0a3/LICENSE
--rw-r--r--   0        0        0     5284 2022-04-27 09:50:02.686350 jetblack-serialization-3.0.0a3/README.md
--rw-r--r--   0        0        0      161 2022-09-24 06:31:30.080154 jetblack-serialization-3.0.0a3/jetblack_serialization/__init__.py
--rw-r--r--   0        0        0     1623 2022-09-24 08:24:38.781842 jetblack-serialization-3.0.0a3/jetblack_serialization/config.py
--rw-r--r--   0        0        0     2651 2022-09-24 06:31:30.080822 jetblack-serialization-3.0.0a3/jetblack_serialization/custom_annotations.py
--rw-r--r--   0        0        0      578 2022-09-24 08:24:38.781967 jetblack-serialization-3.0.0a3/jetblack_serialization/json/__init__.py
--rw-r--r--   0        0        0     2040 2022-04-27 09:50:02.688358 jetblack-serialization-3.0.0a3/jetblack_serialization/json/annotations.py
--rw-r--r--   0        0        0     1824 2022-09-24 08:24:38.782145 jetblack-serialization-3.0.0a3/jetblack_serialization/json/serialization.py
--rw-r--r--   0        0        0     7414 2022-09-24 08:24:38.782348 jetblack-serialization-3.0.0a3/jetblack_serialization/json/typed_deserializer.py
--rw-r--r--   0        0        0     6066 2022-09-24 08:24:38.782525 jetblack-serialization-3.0.0a3/jetblack_serialization/json/typed_serializer.py
--rw-r--r--   0        0        0     1551 2022-09-24 08:24:38.782648 jetblack-serialization-3.0.0a3/jetblack_serialization/json/untyped_deserializer.py
--rw-r--r--   0        0        0     1338 2022-09-24 08:24:38.782776 jetblack-serialization-3.0.0a3/jetblack_serialization/json/untyped_serializer.py
--rw-r--r--   0        0        0       10 2022-04-27 09:50:02.689256 jetblack-serialization-3.0.0a3/jetblack_serialization/py.typed
--rw-r--r--   0        0        0       77 2022-04-27 09:50:02.689362 jetblack-serialization-3.0.0a3/jetblack_serialization/types.py
--rw-r--r--   0        0        0     3103 2022-09-24 06:31:30.082399 jetblack-serialization-3.0.0a3/jetblack_serialization/typing_inspect_ex.py
--rw-r--r--   0        0        0     1405 2022-09-24 08:24:38.782891 jetblack-serialization-3.0.0a3/jetblack_serialization/utils.py
--rw-r--r--   0        0        0      528 2022-09-24 08:24:38.783012 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/__init__.py
--rw-r--r--   0        0        0     2047 2022-09-24 08:24:38.783127 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/annotations.py
--rw-r--r--   0        0        0     1822 2022-09-24 08:24:38.783197 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/serialization.py
--rw-r--r--   0        0        0     8148 2022-09-24 08:29:33.303404 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/typed_deserializer.py
--rw-r--r--   0        0        0     7356 2022-09-24 08:24:38.783494 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/typed_serializer.py
--rw-r--r--   0        0        0     3101 2022-09-24 08:24:38.783613 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/untyped_deserializer.py
--rw-r--r--   0        0        0     2725 2022-09-24 08:24:38.783726 jetblack-serialization-3.0.0a3/jetblack_serialization/xml/untyped_serializer.py
--rw-r--r--   0        0        0      881 2022-09-24 08:25:58.833081 jetblack-serialization-3.0.0a3/pyproject.toml
--rw-r--r--   0        0        0     6412 2022-09-24 08:32:23.519205 jetblack-serialization-3.0.0a3/setup.py
--rw-r--r--   0        0        0     6231 2022-09-24 08:32:23.519517 jetblack-serialization-3.0.0a3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-04-27 09:50:02.686185 jetblack-serialization-3.0.1/LICENSE
+-rw-r--r--   0        0        0     5284 2022-04-27 09:50:02.686350 jetblack-serialization-3.0.1/README.md
+-rw-r--r--   0        0        0      161 2022-09-24 06:31:30.080154 jetblack-serialization-3.0.1/jetblack_serialization/__init__.py
+-rw-r--r--   0        0        0     1623 2022-09-24 08:24:38.781842 jetblack-serialization-3.0.1/jetblack_serialization/config.py
+-rw-r--r--   0        0        0     2651 2022-09-24 06:31:30.080822 jetblack-serialization-3.0.1/jetblack_serialization/custom_annotations.py
+-rw-r--r--   0        0        0      578 2022-09-24 08:24:38.781967 jetblack-serialization-3.0.1/jetblack_serialization/json/__init__.py
+-rw-r--r--   0        0        0     2040 2022-04-27 09:50:02.688358 jetblack-serialization-3.0.1/jetblack_serialization/json/annotations.py
+-rw-r--r--   0        0        0     1824 2022-09-24 08:24:38.782145 jetblack-serialization-3.0.1/jetblack_serialization/json/serialization.py
+-rw-r--r--   0        0        0     7414 2022-09-24 08:24:38.782348 jetblack-serialization-3.0.1/jetblack_serialization/json/typed_deserializer.py
+-rw-r--r--   0        0        0     6066 2022-09-24 08:24:38.782525 jetblack-serialization-3.0.1/jetblack_serialization/json/typed_serializer.py
+-rw-r--r--   0        0        0     1551 2022-09-24 08:24:38.782648 jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_deserializer.py
+-rw-r--r--   0        0        0     1338 2022-09-24 08:24:38.782776 jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_serializer.py
+-rw-r--r--   0        0        0       10 2022-04-27 09:50:02.689256 jetblack-serialization-3.0.1/jetblack_serialization/py.typed
+-rw-r--r--   0        0        0       77 2022-04-27 09:50:02.689362 jetblack-serialization-3.0.1/jetblack_serialization/types.py
+-rw-r--r--   0        0        0     3235 2023-05-07 15:09:34.077443 jetblack-serialization-3.0.1/jetblack_serialization/typing_inspect_ex.py
+-rw-r--r--   0        0        0     1405 2022-09-24 08:24:38.782891 jetblack-serialization-3.0.1/jetblack_serialization/utils.py
+-rw-r--r--   0        0        0      528 2022-09-24 08:24:38.783012 jetblack-serialization-3.0.1/jetblack_serialization/xml/__init__.py
+-rw-r--r--   0        0        0     2047 2022-09-24 08:24:38.783127 jetblack-serialization-3.0.1/jetblack_serialization/xml/annotations.py
+-rw-r--r--   0        0        0     1822 2022-09-24 08:24:38.783197 jetblack-serialization-3.0.1/jetblack_serialization/xml/serialization.py
+-rw-r--r--   0        0        0     8148 2022-09-24 08:29:33.303404 jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_deserializer.py
+-rw-r--r--   0        0        0     7356 2022-09-24 08:24:38.783494 jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_serializer.py
+-rw-r--r--   0        0        0     3101 2022-09-24 08:24:38.783613 jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_deserializer.py
+-rw-r--r--   0        0        0     2725 2022-09-24 08:24:38.783726 jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_serializer.py
+-rw-r--r--   0        0        0      873 2023-05-07 15:05:34.350734 jetblack-serialization-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6410 2023-05-07 15:10:25.552501 jetblack-serialization-3.0.1/setup.py
+-rw-r--r--   0        0        0     6229 2023-05-07 15:10:25.552819 jetblack-serialization-3.0.1/PKG-INFO
```

### Comparing `jetblack-serialization-3.0.0a3/LICENSE` & `jetblack-serialization-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/README.md` & `jetblack-serialization-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/config.py` & `jetblack-serialization-3.0.1/jetblack_serialization/config.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/custom_annotations.py` & `jetblack-serialization-3.0.1/jetblack_serialization/custom_annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/__init__.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/__init__.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/annotations.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/serialization.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/serialization.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/typed_deserializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/typed_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/typed_serializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/typed_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/untyped_deserializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/json/untyped_serializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/json/untyped_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/typing_inspect_ex.py` & `jetblack-serialization-3.0.1/jetblack_serialization/typing_inspect_ex.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 
 try:
     # Python3.8
     from typing import _TypedDictMeta  # type: ignore
 except:  # pylint: disable=bare-except
     # Python3.7
     from typing_extensions import _TypedDictMeta  # type: ignore
-# type: ignore# pylint: disable=unused-import
+
+# type: ignore
 from typing_extensions import _AnnotatedAlias
+
+# pylint: disable=unused-import
 from typing_inspect import (
     get_args,
     get_bound,
     get_constraints,
     get_generic_bases,
     get_generic_type,
     get_last_args,
@@ -109,7 +112,14 @@
         return True
     elif is_union_type(tp):
         return any(is_optional_type(tt) for tt in get_args(tp, evaluate=True))
     elif is_annotated_type(tp):
         return is_optional_type(get_unannotated_type(tp))
     else:
         return False
+
+
+def is_optional_list_type(tp):
+    return (
+        is_optional_type(tp)
+        and is_list_type(get_optional_type(tp))
+    )
```

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/utils.py` & `jetblack-serialization-3.0.1/jetblack_serialization/utils.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/__init__.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/annotations.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/annotations.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/serialization.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/serialization.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/typed_deserializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/typed_serializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/typed_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/untyped_deserializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_deserializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/jetblack_serialization/xml/untyped_serializer.py` & `jetblack-serialization-3.0.1/jetblack_serialization/xml/untyped_serializer.py`

 * *Files identical despite different names*

### Comparing `jetblack-serialization-3.0.0a3/pyproject.toml` & `jetblack-serialization-3.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jetblack-serialization"
-version = "3.0.0-alpha.3"
+version = "3.0.1"
 description = "Serialization for JSON and XML using typing"
 repository = "https://github.com/rob-blackbourn/jetblack-serialization"
 authors = ["Rob Blackbourn <rob.blackbourn@gmail.com>"]
 keywords = ['serialization', 'jetblack', 'json', 'xml', 'typing']
 license = "Apache-2.0"
 readme = "README.md"
 packages = [
```

### Comparing `jetblack-serialization-3.0.0a3/setup.py` & `jetblack-serialization-3.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ['jetblack-iso8601>=1.0,<2.0',
  'lxml>=4.9,<5.0',
  'typing-extensions>=4,<5',
  'typing_inspect>=0.8,<0.9']
 
 setup_kwargs = {
     'name': 'jetblack-serialization',
-    'version': '3.0.0a3',
+    'version': '3.0.1',
     'description': 'Serialization for JSON and XML using typing',
     'long_description': '# jetblack-serialization\n\nSerialization for JSON and XML in Python using typing annotations\n(read the [docs](https://rob-blackbourn.github.io/jetblack-serialization/)).\n\n## Status\n\nIt has been tested with Python 3.7 used the `typing_extensions`\npackage for `TypedDict` and `Annotated`. In Python 3.8 the `TypedDict`\nclass is available in the standard `typing` package.\n\n## Installation\n\nThe package can be installed with pip.\n\n```bash\npip install jetblack-serialization\n```\n\n## Overview\n\nThe package adds support for type annotations when serializing or deserializing\nJSON or XML.\n\n\n### JSON\n\nGiven a typed dictionary:\n\n```python\nfrom datetime import datetime\nfrom typing import List, Optional, TypedDict, Union\n\nclass Book(TypedDict, total=False):\n    book_id: int\n    title: str\n    author: str\n    publication_date: datetime\n    keywords: List[str]\n    phrases: List[str]\n    age: Optional[Union[datetime, int]]\n    pages: Optional[int]\n```\n\n#### Serializing\n\nThis could be serialized to JSON as:\n\n```python\nfrom stringcase import camelcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.json import serialize\n\nobj: Book = {\n    \'author\': \'Chairman Mao\',\n    \'book_id\': 42,\n    \'title\': \'Little Red Book\',\n    \'publication_date\': datetime(1973, 1, 1, 21, 52, 13),\n    \'keywords\': [\'Revolution\', \'Communism\'],\n    \'phrases\': [\n        \'Revolutionary wars are inevitable in class society\',\n        \'War is the continuation of politics\'\n    ],\n    \'age\': 24,\n}\ntext = serialize(\n    obj,\n    Book,\n    SerializerConfig(camelcase, snakecase, pretty_print=True)\n)\nprint(text)\n```\n\ngiving:\n\n```json\n{\n    "bookId": 42,\n    "title": "Little Red Book",\n    "author": "Chairman Mao",\n    "publicationDate": "1973-01-01T21:52:13.00Z",\n    "keywords": ["Revolution", "Communism"],\n    "phrases": ["Revolutionary wars are inevitable in class society", "War is the continuation of politics"],\n    "age": 24,\n    "pages": null\n}\n```\n\nNote the fields have been camel cased, and the publication date has been turned\ninto an ISO 8601 date.\n\n#### Deserializing\n\nWe can deserialize the data as follows:\n\n```python\nfrom stringcase import camelcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.json import deserialize\n\ndct = deserialize(\n    text,\n    Annotated[Book, JSONValue()],\n    SerializerConfig(camelcase, snakecase)\n)\n```\n\n### XML\n\nThe XML version of the typed dictionary might look like this:\n\n```python\nfrom datetime import datetime\nfrom typing import List, Optional, TypedDict, Union\nfrom typing_extensions import Annotated\nfrom jetblack_serialization.xml import XMLEntity, XMLAttribute\n\nclass Book(TypedDict, total=False):\n    book_id: Annotated[int, XMLAttribute("bookId")]\n    title: str\n    author: str\n    publication_date: datetime\n    keywords: Annotated[List[Annotated[str, XMLEntity("Keyword")]], XMLEntity("Keywords")]\n    phrases: List[str]\n    age: Optional[Union[datetime, int]]\n    pages: Optional[int]\n```\n\nNote we have introduced some annotations to control the serialization.\nFor XML we have used pascal-case to serialized the keys and snake-case\nfor deserialization.\n\n#### Serializing\n\nTo serialize we need to provide the containing tag `Book`:\n\n```python\nfrom stringcase import pascalcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.xml import serialize\n\nbook: Book = {\n    \'author\': \'Chairman Mao\',\n    \'book_id\': 42,\n    \'title\': \'Little Red Book\',\n    \'publication_date\': datetime(1973, 1, 1, 21, 52, 13),\n    \'keywords\': [\'Revolution\', \'Communism\'],\n    \'phrases\': [\n        \'Revolutionary wars are inevitable in class society\',\n        \'War is the continuation of politics\'\n    ],\n    \'age\': 24,\n    \'pages\': None\n}\ntext = serialize(\n    book,\n    Annotated[Book, XMLEntity("Book")],\n    SerializerConfig(pascalcase, snakecase)\n)\nprint(text)\n```\n\nProducing:\n\n```xml\n<Book bookId="42">\n    <Title>Little Red Book</Title>\n    <Author>Chairman Mao</Author>\n    <PublicationDate>1973-01-01T21:52:13.00Z</PublicationDate>\n    <Keywords>\n        <Keyword>Revolution</Keyword>\n        <Keyword>Communism</Keyword>\n    </Keywords>\n    <Phrase>Revolutionary wars are inevitable in class society</Phrase>\n    <Phrase>War is the continuation of politics</Phrase>\n    <Age>24</Age>\n</Book>\'\n```\n\nThe annotations are more elaborate here. However, much of the typed dictionary\nrequires no annotation.\n\nFirst we needed the outer document wrapper `XMLEntity("Book")`.\n\nNext we annotated the `book_id` to be an `XMLAttribute`.\n\nFinally we annotated the two lists differently. The `keywords` list used\na nested structure, which we indicated by giving the list a different\n`XMLEntity` tag to the list items. For the phrases we used the default\nin-line behaviour.\n\n#### Deserializing\n\nWe can deserialize the XML as follows:\n\n```python\nfrom stringcase import pascalcase, snakecase\nfrom jetblack_serialization import SerializerConfig\nfrom jetblack_serialization.xml import deserialize\n\ndct = deserialize(\n    text,\n    Annotated[Book, XMLEntity("Book")],\n    SerializerConfig(pascalcase, snakecase)\n)\n```\n\n## Attributes\n\nFor JSON, attributes are typically not required. However\n`JSONProperty(tag: str)` and `JSONValue()` are provided for\ncompleteness.',
     'author': 'Rob Blackbourn',
     'author_email': 'rob.blackbourn@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/rob-blackbourn/jetblack-serialization',
```

### Comparing `jetblack-serialization-3.0.0a3/PKG-INFO` & `jetblack-serialization-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jetblack-serialization
-Version: 3.0.0a3
+Version: 3.0.1
 Summary: Serialization for JSON and XML using typing
 Home-page: https://github.com/rob-blackbourn/jetblack-serialization
 License: Apache-2.0
 Keywords: serialization,jetblack,json,xml,typing
 Author: Rob Blackbourn
 Author-email: rob.blackbourn@gmail.com
 Requires-Python: >=3.7,<4.0
```

