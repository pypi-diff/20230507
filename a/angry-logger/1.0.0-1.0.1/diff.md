# Comparing `tmp/angry_logger-1.0.0.tar.gz` & `tmp/angry_logger-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angry_logger-1.0.0.tar", max compression
+gzip compressed data, was "angry_logger-1.0.1.tar", max compression
```

## Comparing `angry_logger-1.0.0.tar` & `angry_logger-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1576 2023-05-06 06:29:17.463215 angry_logger-1.0.0/README.md
--rw-r--r--   0        0        0       50 2023-05-06 06:22:52.569107 angry_logger-1.0.0/angry_logger/__init__.py
--rw-r--r--   0        0        0     1502 2023-05-06 06:19:33.244907 angry_logger-1.0.0/angry_logger/_const.py
--rw-r--r--   0        0        0     1796 2023-05-06 06:22:52.576459 angry_logger-1.0.0/angry_logger/logging.py
--rw-r--r--   0        0        0      551 2023-05-06 06:29:17.463324 angry_logger-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2237 1970-01-01 00:00:00.000000 angry_logger-1.0.0/setup.py
--rw-r--r--   0        0        0     2309 1970-01-01 00:00:00.000000 angry_logger-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1595 2023-05-07 08:02:23.949049 angry_logger-1.0.1/README.md
+-rw-r--r--   0        0        0       50 2023-05-06 06:22:52.569107 angry_logger-1.0.1/angry_logger/__init__.py
+-rw-r--r--   0        0        0     1502 2023-05-06 06:19:33.244907 angry_logger-1.0.1/angry_logger/_const.py
+-rw-r--r--   0        0        0     1796 2023-05-06 06:22:52.576459 angry_logger-1.0.1/angry_logger/logging.py
+-rw-r--r--   0        0        0      551 2023-05-07 08:03:40.409055 angry_logger-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2257 1970-01-01 00:00:00.000000 angry_logger-1.0.1/setup.py
+-rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 angry_logger-1.0.1/PKG-INFO
```

### Comparing `angry_logger-1.0.0/README.md` & `angry_logger-1.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-[![https://img.shields.io/pypi/v/angry-logger]](https://pypi.org/project/angry-logger/)
-[![https://img.shields.io/pypi/l/angry-logger]](https://github.com/GitToby/angry-logger)
+
+[![version](https://img.shields.io/pypi/v/angry-logger)](https://pypi.org/project/angry-logger/)
+[![licence](https://img.shields.io/pypi/l/angry-logger)](https://github.com/GitToby/angry-logger)
 
 # Angry Logging Made Easy
 
 Do you want to show your logger to be more passive aggressive? maybe just actual aggressive? This is the library for
 you.
 
 ## Installation
```

### Comparing `angry_logger-1.0.0/angry_logger/_const.py` & `angry_logger-1.0.1/angry_logger/_const.py`

 * *Files identical despite different names*

### Comparing `angry_logger-1.0.0/angry_logger/logging.py` & `angry_logger-1.0.1/angry_logger/logging.py`

 * *Files identical despite different names*

### Comparing `angry_logger-1.0.0/pyproject.toml` & `angry_logger-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "angry-logger"
-version = "1.0.0"
+version = "1.0.1"
 description = "Make your logging more passive agressive. Or just agressive agressive."
 readme = 'README.md'
 homepage = 'https://github.com/GitToby/angry-logger'
 authors = ["Toby Devlin <toby@tobydevlin.com>"]
 license = 'MIT'
 
 [tool.poetry.urls]
```

### Comparing `angry_logger-1.0.0/setup.py` & `angry_logger-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['angry_logger']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'angry-logger',
-    'version': '1.0.0',
+    'version': '1.0.1',
     'description': 'Make your logging more passive agressive. Or just agressive agressive.',
-    'long_description': '[![https://img.shields.io/pypi/v/angry-logger]](https://pypi.org/project/angry-logger/)\n[![https://img.shields.io/pypi/l/angry-logger]](https://github.com/GitToby/angry-logger)\n\n# Angry Logging Made Easy\n\nDo you want to show your logger to be more passive aggressive? maybe just actual aggressive? This is the library for\nyou.\n\n## Installation\nYou can install via pip!\n```shell\npip install angry-logger\n```\n\n## Usage\nWhen deciding your project needs more aggression, all you have to do is tell the Angry Logger to go to town. Like so.\n```python\nimport angry_logger\nangry_logger.start()\n```\nIf you\'re not a fan of naughty words, you can tell the angry logger to be less of a potty mouth.\n```python\nimport angry_logger\nangry_logger.start(potty_mouth=False)\n```\n\nFrom here, use your logging as you normally would.\n```python\nimport angry_logger\nimport logging\n\nangry_logger.start(potty_mouth=False)\nlogging.basicConfig(level=logging.DEBUG)\n\ntest_logger = logging.getLogger("test_logger")\n\ntest_logger.debug("this is a test debug message")\ntest_logger.info("this is a test info message")\ntest_logger.warning("this is a test warning message")\ntest_logger.error("this is a test error message")\n```\n\nThis will output your new normal, information hidden behind abuse.\n```\nDEBUG:test_logger:Can I go home now? this is a test debug message\nINFO:test_logger:this is a test info message. But what do you mean by that?\nWARNING:test_logger:Did you do something stupid? Look: this is a test warning message\nERROR:test_logger:this is a test error message????? Are you *****ING kidding me??\n```',
+    'long_description': '\n[![version](https://img.shields.io/pypi/v/angry-logger)](https://pypi.org/project/angry-logger/)\n[![licence](https://img.shields.io/pypi/l/angry-logger)](https://github.com/GitToby/angry-logger)\n\n# Angry Logging Made Easy\n\nDo you want to show your logger to be more passive aggressive? maybe just actual aggressive? This is the library for\nyou.\n\n## Installation\nYou can install via pip!\n```shell\npip install angry-logger\n```\n\n## Usage\nWhen deciding your project needs more aggression, all you have to do is tell the Angry Logger to go to town. Like so.\n```python\nimport angry_logger\nangry_logger.start()\n```\nIf you\'re not a fan of naughty words, you can tell the angry logger to be less of a potty mouth.\n```python\nimport angry_logger\nangry_logger.start(potty_mouth=False)\n```\n\nFrom here, use your logging as you normally would.\n```python\nimport angry_logger\nimport logging\n\nangry_logger.start(potty_mouth=False)\nlogging.basicConfig(level=logging.DEBUG)\n\ntest_logger = logging.getLogger("test_logger")\n\ntest_logger.debug("this is a test debug message")\ntest_logger.info("this is a test info message")\ntest_logger.warning("this is a test warning message")\ntest_logger.error("this is a test error message")\n```\n\nThis will output your new normal, information hidden behind abuse.\n```\nDEBUG:test_logger:Can I go home now? this is a test debug message\nINFO:test_logger:this is a test info message. But what do you mean by that?\nWARNING:test_logger:Did you do something stupid? Look: this is a test warning message\nERROR:test_logger:this is a test error message????? Are you *****ING kidding me??\n```',
     'author': 'Toby Devlin',
     'author_email': 'toby@tobydevlin.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/GitToby/angry-logger',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `angry_logger-1.0.0/PKG-INFO` & `angry_logger-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angry-logger
-Version: 1.0.0
+Version: 1.0.1
 Summary: Make your logging more passive agressive. Or just agressive agressive.
 Home-page: https://github.com/GitToby/angry-logger
 License: MIT
 Author: Toby Devlin
 Author-email: toby@tobydevlin.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,16 +13,17 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: PyPi, https://pypi.org/project/angry-logger/
 Description-Content-Type: text/markdown
 
-[![https://img.shields.io/pypi/v/angry-logger]](https://pypi.org/project/angry-logger/)
-[![https://img.shields.io/pypi/l/angry-logger]](https://github.com/GitToby/angry-logger)
+
+[![version](https://img.shields.io/pypi/v/angry-logger)](https://pypi.org/project/angry-logger/)
+[![licence](https://img.shields.io/pypi/l/angry-logger)](https://github.com/GitToby/angry-logger)
 
 # Angry Logging Made Easy
 
 Do you want to show your logger to be more passive aggressive? maybe just actual aggressive? This is the library for
 you.
 
 ## Installation
```

