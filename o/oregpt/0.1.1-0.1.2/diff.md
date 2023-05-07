# Comparing `tmp/oregpt-0.1.1.tar.gz` & `tmp/oregpt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oregpt-0.1.1.tar", max compression
+gzip compressed data, was "oregpt-0.1.2.tar", max compression
```

## Comparing `oregpt-0.1.1.tar` & `oregpt-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0     1076 2023-05-02 02:51:46.385578 oregpt-0.1.1/LICENSE
--rw-r--r--   0        0        0     2037 2023-05-06 07:13:10.385157 oregpt-0.1.1/README.md
--rw-r--r--   0        0        0     2302 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/chat_bot.py
--rw-r--r--   0        0        0     2072 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/main.py
--rw-r--r--   0        0        0     2232 2023-05-06 07:12:20.995157 oregpt-0.1.1/oregpt/stdinout.py
--rw-r--r--   0        0        0     1819 2023-05-06 07:12:43.525157 oregpt-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 oregpt-0.1.1/setup.py
--rw-r--r--   0        0        0     2899 1970-01-01 00:00:00.000000 oregpt-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 04:09:40.942289 oregpt-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2051 2023-05-07 08:54:28.160734 oregpt-0.1.2/README.md
+-rw-r--r--   0        0        0     2274 2023-05-07 08:41:56.348454 oregpt-0.1.2/oregpt/chat_bot.py
+-rw-r--r--   0        0        0     2136 2023-05-07 08:41:56.348614 oregpt-0.1.2/oregpt/main.py
+-rw-r--r--   0        0        0      304 2023-05-07 08:41:56.348724 oregpt-0.1.2/oregpt/resources/config.yml
+-rw-r--r--   0        0        0     2188 2023-05-07 08:41:56.348886 oregpt-0.1.2/oregpt/stdinout.py
+-rw-r--r--   0        0        0     1907 2023-05-07 08:54:28.160930 oregpt-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-07 04:09:40.943569 oregpt-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-07 08:41:56.349839 oregpt-0.1.2/tests/test_chat_bot.py
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 oregpt-0.1.2/PKG-INFO
```

### Comparing `oregpt-0.1.1/LICENSE` & `oregpt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oregpt-0.1.1/README.md` & `oregpt-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 ```
 
 ## Configuration
 You can specify the place of conversation `log`,
 [style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
 and
 [the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
-in `~/.oregpt/config.yml`
+in `~/.config/oregpt/config.yml`
 ```yaml
-❯ cat ~/.oregpt/config.yml
+❯ cat ~/.config/oregpt/config.yml
 log: /tmp/oregpt/
 openai:
     model: gpt-3.5-turbo
 # You can also specify OpenAI's API key here
 #     api_key: <your-api-key>
 character:
     user:
```

### Comparing `oregpt-0.1.1/oregpt/chat_bot.py` & `oregpt-0.1.2/oregpt/chat_bot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 import pathlib
 from datetime import datetime
-from typing import Callable
 
 import openai
 
 from oregpt.stdinout import StdInOut
 
 
 class ChatBot:
```

### Comparing `oregpt-0.1.1/oregpt/main.py` & `oregpt-0.1.2/oregpt/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import os
+import pathlib
 import shutil
 from typing import Any
 
 import openai
 import yaml
-from prompt_toolkit.styles import Style
 
 from oregpt.chat_bot import ChatBot
 from oregpt.stdinout import StdInOut
 
 
 def load_config() -> dict[str, Any]:
     # TODO: Find more sophisticated way to do this...
-    config_file = os.path.join(os.path.expanduser("~"), ".oregpt/config.yml")
+    config_file = os.path.join(os.path.expanduser("~"), ".config/oregpt/config.yml")
     if not os.path.exists(config_file):
         os.makedirs(os.path.dirname(config_file), exist_ok=True)
-        shutil.copyfile("config.yml", config_file)
+        directory = pathlib.Path(__file__).parent.resolve()
+        shutil.copyfile(directory / "resources/config.yml", config_file)
     with open(config_file, "r") as file:
         config: dict[str, Any] = yaml.load(file, Loader=yaml.FullLoader)
     return config
 
 
 def initialize_open_ai_key(config: dict[str, Any]) -> None:
     if "api_key" in config:
```

### Comparing `oregpt-0.1.1/oregpt/stdinout.py` & `oregpt-0.1.2/oregpt/stdinout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import contextlib
-import copy
 import sys
 from dataclasses import dataclass
-from typing import Any, Callable, ContextManager, Iterator, Optional
+from typing import Any, Iterator, Optional
 
-from prompt_toolkit import HTML, print_formatted_text, prompt
+from prompt_toolkit import print_formatted_text, prompt
 from prompt_toolkit.formatted_text import AnyFormattedText, FormattedText
 from prompt_toolkit.styles import Style
 
 
 @dataclass
 class Character:
     name: str
```

### Comparing `oregpt-0.1.1/pyproject.toml` & `oregpt-0.1.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 [tool.poetry]
 name = "oregpt"
-version = "0.1.1"
+version = "0.1.2"
 description = "A tiny GPT CLI tool"
 authors = ["Shinichi Takayanagi <shinichi.takayanagi@gmail.com>"]
 homepage = "https://github.com/shinichi-takayanagi/oregpt"
 repository = "https://github.com/shinichi-takayanagi/oregpt"
 license = "MIT"
 readme = "README.md"
 keywords = ["gpt-chatbot", "gpt-cli", "openai-cli"]
 classifiers = [
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
   "Topic :: Utilities",
 ]
+packages = [
+    { include = "oregpt"}
+]
 include = [
-    "LICENSE",
+    { path = "tests", format = "sdist" }
 ]
 
 [tool.poetry.scripts]
 oregpt = "oregpt.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -32,14 +35,15 @@
 pytest = "^7.3.1"
 
 
 [tool.poetry.group.lint.dependencies]
 black = "^23.3.0"
 isort = "^5.12.0"
 mypy = "^1.2.0"
+autoflake = "^2.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 # === Black ===
```

### Comparing `oregpt-0.1.1/setup.py` & `oregpt-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: oregpt
+Version: 0.1.2
+Summary: A tiny GPT CLI tool
+Home-page: https://github.com/shinichi-takayanagi/oregpt
+License: MIT
+Keywords: gpt-chatbot,gpt-cli,openai-cli
+Author: Shinichi Takayanagi
+Author-email: shinichi.takayanagi@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Requires-Dist: openai (>=0.27.6,<0.28.0)
+Requires-Dist: prompt-toolkit (>=3.0.38,<4.0.0)
+Requires-Dist: pyyaml (>=6.0,<7.0)
+Project-URL: Repository, https://github.com/shinichi-takayanagi/oregpt
+Description-Content-Type: text/markdown
+
+# oregpt
+![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)
+[![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)
+[![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)
+[![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)
+[![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)
+
+A tiny GPT CLI tool.
+You can chat with the GPT model developped by OpenAI and save the conversation as json.
+
+![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)
+
+## Installation
+### Get your own OpenAI API Key
+Assuming you have an environment variable with key named `OPENAI_API_KEY`.
+If you don't have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable
+
+```bash
+export OPENAI_API_KEY=<YOUR-OPENAI-API-KEY>
+
+```
+
+### Instal from PyPI
+You can install the package using pip:
+
+```bash
+$ pip install oregpt
+```
+
+## Usage
+Once you have installed oregpt, you can run it by typing:
+```bash
+$ oregpt
+```
+
+## Configuration
+You can specify the place of conversation `log`,
+[style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)
+and
+[the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)
+in `~/.config/oregpt/config.yml`
+```yaml
+❯ cat ~/.config/oregpt/config.yml
+log: /tmp/oregpt/
+openai:
+    model: gpt-3.5-turbo
+# You can also specify OpenAI's API key here
+#     api_key: <your-api-key>
+character:
+    user:
+        name: Me
+        style: "#00BEFE"
+    assistant:
+        name: AI
+        style: "#87CEEB"
+    system:
+        name: System
+        style: "#cc0000"
+```
 
-packages = \
-['oregpt']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['openai>=0.27.6,<0.28.0', 'prompt-toolkit>=3.0.38,<4.0.0', 'pyyaml>=6.0,<7.0']
-
-entry_points = \
-{'console_scripts': ['oregpt = oregpt.main:main']}
-
-setup_kwargs = {
-    'name': 'oregpt',
-    'version': '0.1.1',
-    'description': 'A tiny GPT CLI tool',
-    'long_description': '# oregpt\n![workflow](https://github.com/shinichi-takayanagi/oregpt/actions/workflows/main.yml/badge.svg)\n[![license](https://img.shields.io/github/license/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/blob/master/LICENSE)\n[![release](https://img.shields.io/github/release/shinichi-takayanagi/oregpt.svg)](https://github.com/shinichi-takayanagi/oregpt/releases/latest)\n[![python-version](https://img.shields.io/pypi/pyversions/oregpt.svg)](https://pypi.org/project/oregpt/)\n[![pypi](https://img.shields.io/pypi/v/oregpt?color=%2334D058&label=pypi%20package)](https://pypi.org/project/oregpt)\n\nA tiny GPT CLI tool.\nYou can chat with the GPT model developped by OpenAI and save the conversation as json.\n\n![oregpt](https://user-images.githubusercontent.com/24406372/236609166-0f2385b1-fd9e-4810-b80d-c19c44d13411.gif)\n\n## Installation\n### Get your own OpenAI API Key\nAssuming you have an environment variable with key named `OPENAI_API_KEY`.\nIf you don\'t have a OpenAI API key [visit here](https://platform.openai.com/account/api-keys), generate one and add it as an environment variable\n\n```bash\nexport OPENAI_API_KEY=<YOUR-OPENAI-API-KEY>\n\n```\n\n### Instal from PyPI\nYou can install the package using pip:\n\n```bash\n$ pip install oregpt\n```\n\n## Usage\nOnce you have installed oregpt, you can run it by typing:\n```bash\n$ oregpt\n```\n\n## Configuration\nYou can specify the place of conversation `log`,\n[style (color etc)](https://python-prompt-toolkit.readthedocs.io/en/master/pages/advanced_topics/styling.html)\nand\n[the model supported in /v1/chat/completions endpoint provided by OpenAI](https://platform.openai.com/docs/models/overview)\nin `~/.oregpt/config.yml`\n```yaml\n❯ cat ~/.oregpt/config.yml\nlog: /tmp/oregpt/\nopenai:\n    model: gpt-3.5-turbo\n# You can also specify OpenAI\'s API key here\n#     api_key: <your-api-key>\ncharacter:\n    user:\n        name: Me\n        style: "#00BEFE"\n    assistant:\n        name: AI\n        style: "#87CEEB"\n    system:\n        name: System\n        style: "#cc0000"\n```\n',
-    'author': 'Shinichi Takayanagi',
-    'author_email': 'shinichi.takayanagi@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/shinichi-takayanagi/oregpt',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

