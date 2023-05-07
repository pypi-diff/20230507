# Comparing `tmp/arxiv-post-0.6.4.tar.gz` & `tmp/arxiv_post-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv-post-0.6.4.tar", max compression
+gzip compressed data, was "arxiv_post-0.7.0.tar", max compression
```

## Comparing `arxiv-post-0.6.4.tar` & `arxiv_post-0.7.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1071 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/LICENSE
--rw-r--r--   0        0        0     2417 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/README.md
--rw-r--r--   0        0        0      170 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/__init__.py
--rw-r--r--   0        0        0       50 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/apps/__init__.py
--rw-r--r--   0        0        0     2050 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/apps/slack.py
--rw-r--r--   0        0        0     1907 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/article.py
--rw-r--r--   0        0        0     1679 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/arxiv.py
--rw-r--r--   0        0        0     3017 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/cli.py
--rw-r--r--   0        0        0      534 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/consts.py
--rw-r--r--   0        0        0     6029 2022-07-29 11:24:33.699239 arxiv-post-0.6.4/arxiv_post/deepl.py
--rw-r--r--   0        0        0      915 2022-07-29 11:24:33.719239 arxiv-post-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3486 2022-07-29 11:24:44.577538 arxiv-post-0.6.4/setup.py
--rw-r--r--   0        0        0     3445 2022-07-29 11:24:44.577844 arxiv-post-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-07 15:10:57.622303 arxiv_post-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2429 2023-05-07 15:10:57.622303 arxiv_post-0.7.0/README.md
+-rw-r--r--   0        0        0      249 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/__init__.py
+-rw-r--r--   0        0        0       50 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/apps/__init__.py
+-rw-r--r--   0        0        0     2050 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/apps/slack.py
+-rw-r--r--   0        0        0     1907 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/article.py
+-rw-r--r--   0        0        0     1679 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/arxiv.py
+-rw-r--r--   0        0        0     3017 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/cli.py
+-rw-r--r--   0        0        0      534 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/consts.py
+-rw-r--r--   0        0        0     6302 2023-05-07 15:10:57.626303 arxiv_post-0.7.0/arxiv_post/deepl.py
+-rw-r--r--   0        0        0      952 2023-05-07 15:10:57.642303 arxiv_post-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 arxiv_post-0.7.0/PKG-INFO
```

### Comparing `arxiv-post-0.6.4/LICENSE` & `arxiv_post-0.7.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 Akio Taniguchi
+Copyright (c) 2020-2023 Akio Taniguchi
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `arxiv-post-0.6.4/README.md` & `arxiv_post-0.7.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # arxiv-post
 
 [![Release](https://img.shields.io/pypi/v/arxiv-post?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)
 [![Python](https://img.shields.io/pypi/pyversions/arxiv-post?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)
 [![Downloads](https://img.shields.io/pypi/dm/arxiv-post?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/arxiv-post)
-[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.6127352-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.6127352)
-[![Tests](https://img.shields.io/github/workflow/status/astropenguin/arxiv-post/Tests?label=Tests&style=flat-square)](https://github.com/astropenguin/arxiv-post/actions)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5633924-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.5633924)
+[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/arxiv-post/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/arxiv-post/actions)
 
 Translate and post arXiv articles to Slack and various apps
 
 ## Installation
 
 ```shell
 $ pip install arxiv-post
```

### Comparing `arxiv-post-0.6.4/arxiv_post/apps/slack.py` & `arxiv_post-0.7.0/arxiv_post/apps/slack.py`

 * *Files identical despite different names*

### Comparing `arxiv-post-0.6.4/arxiv_post/article.py` & `arxiv_post-0.7.0/arxiv_post/article.py`

 * *Files identical despite different names*

### Comparing `arxiv-post-0.6.4/arxiv_post/arxiv.py` & `arxiv_post-0.7.0/arxiv_post/arxiv.py`

 * *Files identical despite different names*

### Comparing `arxiv-post-0.6.4/arxiv_post/cli.py` & `arxiv_post-0.7.0/arxiv_post/cli.py`

 * *Files identical despite different names*

### Comparing `arxiv-post-0.6.4/arxiv_post/consts.py` & `arxiv_post-0.7.0/arxiv_post/consts.py`

 * *Files identical despite different names*

### Comparing `arxiv-post-0.6.4/arxiv_post/deepl.py` & `arxiv_post-0.7.0/arxiv_post/deepl.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 __all__ = ["translate"]
 
 
 # standard library
+import re
 from asyncio import gather, sleep, run
 from logging import getLogger
 from textwrap import shorten
 from typing import Iterable, List, Sequence, Protocol, TypeVar, cast
 
 
 # dependencies
@@ -22,16 +23,18 @@
     N_CONCURRENT,
     TIMEOUT,
     DeepLMode,
 )
 
 
 # constants
-DEEPL_INPUT = "textarea.lmt__source_textarea"
-DEEPL_OUTPUT = "#target-dummydiv"
+DEEPL_SOURCE_DIV = "data-testid=translator-source-input"
+DEEPL_SOURCE_BOX = "role=textbox"
+DEEPL_TARGET_DIV = "data-testid=translator-target-input"
+DEEPL_TARGET_BOX = "role=textbox"
 DEEPL_TRANSLATOR = "https://deepl.com/translator"
 
 
 # logger
 logger = getLogger(__name__)
 
 
@@ -157,35 +160,40 @@
                 await browser.close()
 
     return run(main())
 
 
 async def _translate(translatable: TL, page: Page, timeout: float) -> TL:
     """Translate an object in a page of a browser."""
-    if not (original := str(translatable)):
+    if not (source := str(translatable)):
         return translatable
 
-    await page.fill(DEEPL_INPUT, "")
-    await page.fill(DEEPL_INPUT, original)
+    source_box = page.locator(DEEPL_SOURCE_DIV).locator(DEEPL_SOURCE_BOX)
+    target_box = page.locator(DEEPL_TARGET_DIV).locator(DEEPL_TARGET_BOX)
+
+    await source_box.fill("")
+    await source_box.fill(source)
 
     for _ in range(int(timeout / 0.5)):
         await sleep(0.5)
 
-        if (content := await page.text_content(DEEPL_OUTPUT)) is None:
+        if (target := await target_box.inner_text()) is None:
             continue
 
-        if not (content := content.strip()):
+        if not (target := target.strip()):
             continue
 
+        target = re.sub("\n+", "\n", target)
+
         try:
-            return translatable.replace(original, content)
+            return translatable.replace(source, target)
         except ValueError:
             break
 
-    logger.warn(f"Failed to translate: {shorten(original, 50)!r}")
+    logger.warn(f"Failed to translate: {shorten(source, 50)!r}")
     return translatable
 
 
 def parse_language(lang: str) -> str:
     """Parse and format a language string."""
     if (lang := lang.lower()) in vars(Language).values():
         return lang
```

### Comparing `arxiv-post-0.6.4/setup.py` & `arxiv_post-0.7.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: arxiv-post
+Version: 0.7.0
+Summary: Translate and post arXiv articles to Slack and various apps
+Home-page: https://github.com/astropenguin/arxiv-post/
+License: MIT
+Keywords: arxiv,deepl,slack,translation
+Author: Akio Taniguchi
+Author-email: taniguchi@a.phys.nagoya-u.ac.jp
+Requires-Python: >=3.8,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: arxiv (>=1.4,<2.0)
+Requires-Dist: dateparser (>=1.1,<2.0)
+Requires-Dist: deepl (>=1.12,<2.0)
+Requires-Dist: fire (>=0.5,<0.6)
+Requires-Dist: more-itertools (>=9.0,<10.0)
+Requires-Dist: playwright (>=1.30,<2.0)
+Requires-Dist: pylatexenc (>=2.10,<3.0)
+Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: tomli (>=2.0,<3.0)
+Project-URL: Documentation, https://astropenguin.github.io/arxiv-post/
+Description-Content-Type: text/markdown
+
+# arxiv-post
+
+[![Release](https://img.shields.io/pypi/v/arxiv-post?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)
+[![Python](https://img.shields.io/pypi/pyversions/arxiv-post?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)
+[![Downloads](https://img.shields.io/pypi/dm/arxiv-post?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/arxiv-post)
+[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.5633924-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.5633924)
+[![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/arxiv-post/tests.yml?label=Tests&style=flat-square)](https://github.com/astropenguin/arxiv-post/actions)
+
+Translate and post arXiv articles to Slack and various apps
+
+## Installation
+
+```shell
+$ pip install arxiv-post
+$ playwright install chromium
+```
+
+## Usage
+
+Command line interface `arxiv-post` is available after installation, with which you can translate and post arXiv articles to various apps.
+Note that only `slack` app is currently available.
+You need to [create a custom Slack app to get an URL of incoming webhook](https://slack.com/help/articles/115005265063-Incoming-webhooks-for-Slack).
+
+```shell
+$ arxiv-post slack --keywords deshima \
+                   --categories astro-ph.IM \
+                   --target_lang ja \
+                   --slack_webhook_url <Slack webhook URL>
+```
+
+The posted article looks like this.
+
+![arxiv-post-slack.png](https://raw.githubusercontent.com/astropenguin/arxiv-post/master/docs/_static/arxiv-post-slack.png)
+
+For detailed information, see the built-in help by the following command.
+
+```shell
+$ arxiv-post slack --help
+```
+
+## Example
 
-packages = \
-['arxiv_post', 'arxiv_post.apps']
+It would be nice to regularly run the command by some automation tools such as GitHub Actions.
+Here is a live example where daily arXiv articles in [astro-ph.GA](https://arxiv.org/list/astro-ph.GA/new), [astro-ph.IM](https://arxiv.org/list/astro-ph.IM/new), and [astro-ph.HE](https://arxiv.org/list/astro-ph.HE/new) are posted to different channels of a Slack workspace.
 
-package_data = \
-{'': ['*']}
+- [a-lab-nagoya/astro-ph-slack: Translate and post arXiv articles to Slack](https://github.com/a-lab-nagoya/astro-ph-slack)
 
-install_requires = \
-['arxiv>=1.4,<2.0',
- 'dateparser>=1.1,<2.0',
- 'deepl>=1.4,<2.0',
- 'fire>=0.4,<0.5',
- 'more-itertools>=8.13,<9.0',
- 'playwright>=1.18,<2.0',
- 'pylatexenc>=2.10,<3.0',
- 'requests>=2.27,<3.0',
- 'tomli>=2.0,<3.0']
-
-entry_points = \
-{'console_scripts': ['arxiv-post = arxiv_post.cli:main']}
-
-setup_kwargs = {
-    'name': 'arxiv-post',
-    'version': '0.6.4',
-    'description': 'Translate and post arXiv articles to Slack and various apps',
-    'long_description': '# arxiv-post\n\n[![Release](https://img.shields.io/pypi/v/arxiv-post?label=Release&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)\n[![Python](https://img.shields.io/pypi/pyversions/arxiv-post?label=Python&color=cornflowerblue&style=flat-square)](https://pypi.org/project/arxiv-post/)\n[![Downloads](https://img.shields.io/pypi/dm/arxiv-post?label=Downloads&color=cornflowerblue&style=flat-square)](https://pepy.tech/project/arxiv-post)\n[![DOI](https://img.shields.io/badge/DOI-10.5281/zenodo.6127352-cornflowerblue?style=flat-square)](https://doi.org/10.5281/zenodo.6127352)\n[![Tests](https://img.shields.io/github/workflow/status/astropenguin/arxiv-post/Tests?label=Tests&style=flat-square)](https://github.com/astropenguin/arxiv-post/actions)\n\nTranslate and post arXiv articles to Slack and various apps\n\n## Installation\n\n```shell\n$ pip install arxiv-post\n$ playwright install chromium\n```\n\n## Usage\n\nCommand line interface `arxiv-post` is available after installation, with which you can translate and post arXiv articles to various apps.\nNote that only `slack` app is currently available.\nYou need to [create a custom Slack app to get an URL of incoming webhook](https://slack.com/help/articles/115005265063-Incoming-webhooks-for-Slack).\n\n```shell\n$ arxiv-post slack --keywords deshima \\\n                   --categories astro-ph.IM \\\n                   --target_lang ja \\\n                   --slack_webhook_url <Slack webhook URL>\n```\n\nThe posted article looks like this.\n\n![arxiv-post-slack.png](https://raw.githubusercontent.com/astropenguin/arxiv-post/master/docs/_static/arxiv-post-slack.png)\n\nFor detailed information, see the built-in help by the following command.\n\n```shell\n$ arxiv-post slack --help\n```\n\n## Example\n\nIt would be nice to regularly run the command by some automation tools such as GitHub Actions.\nHere is a live example where daily arXiv articles in [astro-ph.GA](https://arxiv.org/list/astro-ph.GA/new), [astro-ph.IM](https://arxiv.org/list/astro-ph.IM/new), and [astro-ph.HE](https://arxiv.org/list/astro-ph.HE/new) are posted to different channels of a Slack workspace.\n\n- [a-lab-nagoya/astro-ph-slack: Translate and post arXiv articles to Slack](https://github.com/a-lab-nagoya/astro-ph-slack)\n\n## References\n\n- [fkubota/Carrier-Owl: arxiv--> DeepL --> Slack](https://github.com/fkubota/Carrier-Owl): The arxiv-post package is highly inspired by their work.\n',
-    'author': 'Akio Taniguchi',
-    'author_email': 'taniguchi@a.phys.nagoya-u.ac.jp',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/astropenguin/arxiv-post/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.11',
-}
+## References
 
+- [fkubota/Carrier-Owl: arxiv--> DeepL --> Slack](https://github.com/fkubota/Carrier-Owl): The arxiv-post package is highly inspired by their work.
 
-setup(**setup_kwargs)
```

