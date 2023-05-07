# Comparing `tmp/configgy-0.1.0.tar.gz` & `tmp/configgy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configgy-0.1.0.tar", max compression
+gzip compressed data, was "configgy-0.1.1.tar", max compression
```

## Comparing `configgy-0.1.0.tar` & `configgy-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2023-05-07 10:04:30.256725 configgy-0.1.0/configgy/__init__.py
--rw-r--r--   0        0        0     1685 2023-05-07 10:19:07.217993 configgy-0.1.0/configgy/loader.py
--rw-r--r--   0        0        0      895 2023-05-07 10:22:30.411095 configgy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      685 2023-05-07 10:28:15.110504 configgy-0.1.0/README.md
--rw-r--r--   0        0        0     1365 2023-05-07 10:29:12.897231 configgy-0.1.0/setup.py
--rw-r--r--   0        0        0     1585 2023-05-07 10:29:12.897231 configgy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-07 10:49:47.657638 configgy-0.1.1/configgy/__init__.py
+-rw-r--r--   0        0        0     1785 2023-05-07 10:41:29.594277 configgy-0.1.1/configgy/loader.py
+-rw-r--r--   0        0        0      888 2023-05-07 10:49:30.101181 configgy-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      685 2023-05-07 10:41:27.361147 configgy-0.1.1/README.md
+-rw-r--r--   0        0        0     1386 2023-05-07 10:49:52.237457 configgy-0.1.1/setup.py
+-rw-r--r--   0        0        0     1650 2023-05-07 10:49:52.237457 configgy-0.1.1/PKG-INFO
```

### Comparing `configgy-0.1.0/configgy/loader.py` & `configgy-0.1.1/configgy/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 import configparser
 import json
 from typing import Dict, Protocol
 
 import toml
 import yaml
 
+from configgy import __version__
+
+
+def test_version():
+    assert __version__ == '0.1.0'
+    
 
 class Loader(Protocol):
     def load(self, f) -> Dict:
         pass
 
 
 class ConfigLoader:
```

### Comparing `configgy-0.1.0/pyproject.toml` & `configgy-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,32 @@
 [tool.poetry]
 name = "configgy"
-version = "0.1.0"
-description = "Load popular config file formats into a python dict"
+version = "0.1.1"
+description = "A subtle config loader for python"
 authors = ["baniasbaabe <banias@hotmail.de>"]
 license = "MIT"
 readme = "README.md"
-homepage = ""
-repository = ""
-keywords = ["config", "ini", "yaml", "toml", "json"]
+homepage = "https://github.com/baniasbaabe/configgy"
+repository = "https://github.com/baniasbaabe/configgy"
+keywords = ["´config", "yaml", "json", "toml", "ini"]
 classifiers = [
-    "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Documentation",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Quality Assurance",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 PyYAML = "^6.0"
-configparser = "^5.3.0"
 toml = "^0.10.2"
+configparser = "^5.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
-black = "^23.3.0"
-isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `configgy-0.1.0/README.md` & `configgy-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `configgy-0.1.0/setup.py` & `configgy-0.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0,<7.0', 'configparser>=5.3.0,<6.0.0', 'toml>=0.10.2,<0.11.0']
 
 setup_kwargs = {
     'name': 'configgy',
-    'version': '0.1.0',
-    'description': 'Load popular config file formats into a python dict',
+    'version': '0.1.1',
+    'description': 'A subtle config loader for python',
     'long_description': '# Configgy\n\nA subtle Python package for loading configuration files without having to specify the file type.\n\n## Installation\n\nYou can install the package from PyPI using pip:\n\n```bash\npip install configgy\n```\n\n## Usage\n\nHere\'s an example of how to use the package to load a configuration file:\n\n```python\nfrom configgy.loader import ConfigLoader\n\ndata = ConfigLoader().load_config_file("file.json")\n```\n\nThe `load_config` function takes a single argument, the path to the configuration file. It will automatically detect the file type and use the appropriate loader.\n\nCurrently, the package supports the following file types:\n\n- INI\n- YAML\n- TOML\n- JSON\n',
     'author': 'baniasbaabe',
     'author_email': 'banias@hotmail.de',
     'maintainer': None,
     'maintainer_email': None,
-    'url': '',
+    'url': 'https://github.com/baniasbaabe/configgy',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8,<4.0',
 }
```

### Comparing `configgy-0.1.0/PKG-INFO` & `configgy-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: configgy
-Version: 0.1.0
-Summary: Load popular config file formats into a python dict
+Version: 0.1.1
+Summary: A subtle config loader for python
+Home-page: https://github.com/baniasbaabe/configgy
 License: MIT
-Keywords: config,ini,yaml,toml,json
+Keywords: ´config,yaml,json,toml,ini
 Author: baniasbaabe
 Author-email: banias@hotmail.de
 Requires-Python: >=3.8,<4.0
-Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Quality Assurance
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: configparser (>=5.3.0,<6.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
+Project-URL: Repository, https://github.com/baniasbaabe/configgy
 Description-Content-Type: text/markdown
 
 # Configgy
 
 A subtle Python package for loading configuration files without having to specify the file type.
 
 ## Installation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

