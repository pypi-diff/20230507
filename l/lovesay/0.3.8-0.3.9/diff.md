# Comparing `tmp/lovesay-0.3.8.tar.gz` & `tmp/lovesay-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lovesay-0.3.8.tar", max compression
+gzip compressed data, was "lovesay-0.3.9.tar", max compression
```

## Comparing `lovesay-0.3.8.tar` & `lovesay-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2022-10-14 21:56:01.688970 lovesay-0.3.8/LICENSE
--rw-r--r--   0        0        0     3895 2022-11-07 03:54:53.406370 lovesay-0.3.8/README.md
--rw-r--r--   0        0        0        0 2022-10-14 21:56:01.689292 lovesay-0.3.8/lovesay/__init__.py
--rw-r--r--   0        0        0      850 2022-11-07 03:52:32.853630 lovesay-0.3.8/lovesay/cli.py
--rw-r--r--   0        0        0     5240 2022-11-07 03:53:23.124867 lovesay-0.3.8/lovesay/love.py
--rw-r--r--   0        0        0      448 2022-11-07 03:53:46.860913 lovesay-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     4741 1970-01-01 00:00:00.000000 lovesay-0.3.8/setup.py
--rw-r--r--   0        0        0     4408 1970-01-01 00:00:00.000000 lovesay-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-12-05 18:54:08.638254 lovesay-0.3.9/LICENSE
+-rw-r--r--   0        0        0     3854 2022-12-05 18:49:16.823752 lovesay-0.3.9/README.md
+-rw-r--r--   0        0        0        0 2022-10-14 21:56:01.689292 lovesay-0.3.9/lovesay/__init__.py
+-rw-r--r--   0        0        0      850 2022-11-07 03:52:32.853630 lovesay-0.3.9/lovesay/cli.py
+-rw-r--r--   0        0        0     5210 2022-11-07 03:55:51.057839 lovesay-0.3.9/lovesay/love.py
+-rw-r--r--   0        0        0      449 2022-12-05 18:48:56.741894 lovesay-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     4701 1970-01-01 00:00:00.000000 lovesay-0.3.9/setup.py
+-rw-r--r--   0        0        0     4368 1970-01-01 00:00:00.000000 lovesay-0.3.9/PKG-INFO
```

### Comparing `lovesay-0.3.8/LICENSE` & `lovesay-0.3.9/LICENSE`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 ZenithDS
+Copyright (c) 2021 dotzenith
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `lovesay-0.3.8/README.md` & `lovesay-0.3.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -27,33 +27,33 @@
 ---
 
 ### ❖ Requirements
 
 Note: These requirements only apply if using you're using lovesay to print a different quote for each day of the month.  
 
 - A quotes file stored in `$HOME/.config/lovesay/`
-- Each quote must be on a new line, see the example quotes file in `.config/lovesay/quotes`
+- Each quote must be on a new line, see the example quotes file in `.example/quotes`
 - (optional) A partner to write you 31 lines full of love, one for each day of the month
 
 ---
 
 ### ❖ Installation
 
 > Install from pip
 ```sh
 pip3 install lovesay
 ```
 
 > Install from source
 - First, install [poetry](https://python-poetry.org/)
 ```sh
-git clone https://github.com/ZenithDS/lovesay.git
+git clone https://github.com/dotzenith/lovesay.git
 cd lovesay
 poetry build
-pip3 install ./dist/lovesay-0.3.8.tar.gz
+pip3 install ./dist/lovesay-0.3.9.tar.gz
 ```
 
 ### ❖ Usage 
 
 lovesay can be used in a similar fashion to cowsay
 
 ```sh
@@ -107,15 +107,15 @@
 Seeing words full of love from my partner is a lot better than any other command I could possibly run. It makes my terminal feel cozy, welcoming, and as is the case with most things my partner touches, it makes my terminal feel like home. 
 
 I hope that someone else finds a use for this little script as well. Love is a wonderful thing, and we could all use a little bit more of it in our lives (especially arch linux users)
 
 ---
 
 ### ❖ What's New? 
-0.3.8 - Black is now used for formatting alongside isort
+0.3.9 - Change author
 
 ---
 
 <div align="center">
 
    <img src="https://img.shields.io/static/v1.svg?label=License&message=MIT&color=F5E0DC&labelColor=302D41&style=for-the-badge">
```

### Comparing `lovesay-0.3.8/lovesay/cli.py` & `lovesay-0.3.9/lovesay/cli.py`

 * *Files identical despite different names*

### Comparing `lovesay-0.3.8/lovesay/love.py` & `lovesay-0.3.9/lovesay/love.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 # Dotzenith
 # Lovesay: A script to display a quote from a loved one based on the day of the month
 
 import textwrap as tr
 from datetime import date
 
-# Imports to make life easier
 from os import getenv
 from os.path import exists, expanduser
 from typing import Optional
 
 from kolorz.kolor import get_all_colorschemes, make_kolorz
```

### Comparing `lovesay-0.3.8/setup.py` & `lovesay-0.3.9/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 ['kolorz>=0.2.1,<0.3.0', 'typer>=0.4.0,<0.5.0']
 
 entry_points = \
 {'console_scripts': ['lovesay = lovesay.cli:main']}
 
 setup_kwargs = {
     'name': 'lovesay',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'Cowsay, but full of love',
-    'long_description': '<h2 align="center"> ━━━━━━  ❖  ━━━━━━ </h2>\n\n<!-- BADGES -->\n<div align="center">\n   <p></p>\n   \n   <img src="https://img.shields.io/github/stars/dotzenith/lovesay?color=F8BD96&labelColor=302D41&style=for-the-badge">   \n\n   <img src="https://img.shields.io/github/forks/dotzenith/lovesay?color=DDB6F2&labelColor=302D41&style=for-the-badge">   \n\n   <img src="https://img.shields.io/github/repo-size/dotzenith/lovesay?color=ABE9B3&labelColor=302D41&style=for-the-badge">\n   \n   <img src="https://img.shields.io/github/commit-activity/y/dotzenith/lovesay?color=96CDFB&labelColor=302D41&style=for-the-badge&label=COMMITS"/>\n   <br>\n</div>\n\n<p/>\n\n---\n\n### ❖ Information \n\n  lovesay is a simple python script that displays a quote from a loved one based on the day of the month or a quote passed in through the cli arguments. \n\n  <img src="https://github.com/dotzenith/dotzenith/blob/main/assets/lovesay/lovesay.gif" alt="lovesay gif">\n\n---\n\n### ❖ Requirements\n\nNote: These requirements only apply if using you\'re using lovesay to print a different quote for each day of the month.  \n\n- A quotes file stored in `$HOME/.config/lovesay/`\n- Each quote must be on a new line, see the example quotes file in `.config/lovesay/quotes`\n- (optional) A partner to write you 31 lines full of love, one for each day of the month\n\n---\n\n### ❖ Installation\n\n> Install from pip\n```sh\npip3 install lovesay\n```\n\n> Install from source\n- First, install [poetry](https://python-poetry.org/)\n```sh\ngit clone https://github.com/ZenithDS/lovesay.git\ncd lovesay\npoetry build\npip3 install ./dist/lovesay-0.3.8.tar.gz\n```\n\n### ❖ Usage \n\nlovesay can be used in a similar fashion to cowsay\n\n```sh\nlovesay "Hello World"\n```\n\nif there\'s a `quotes` file in `$HOME/.config/lovesay/`, lovesay can be used without any arguments\n\n```sh\nlovesay\n```\n\nif you\'d like to use a quotes stored somewhere other than the path above, the `LOVESAY_PATH` env variable can be used as such\n\n```sh\nexport LOVESAY_PATH="~/path/to/file"\n```\n\nlovesay can also be used with a variety of different color schemes.\n\n> lovesay uses [catppuccin](https://github.com/catppuccin)(mocha) as it\'s default color scheme, but a different one can be specified using the `--color` option. \n\nFor example:\n```sh\nlovesay # uses catppuccin\n```\n  \n```sh\nlovesay -c nord # uses nord \n```\n\nSupported color schemes as of now: \n- [catppuccin](https://github.com/catppuccin) - latte, frappe, macchiato, mocha\n- [nord](https://github.com/arcticicestudio/nord)\n- [dracula](https://github.com/dracula/dracula-theme)\n- [gruvbox](https://github.com/morhetz/gruvbox)\n- [onedark](https://github.com/joshdick/onedark.vim)\n- [tokyonight](https://github.com/folke/tokyonight.nvim)\n- [ayu](https://github.com/ayu-theme)\n- [palenight](https://github.com/drewtempelmeyer/palenight.vim)\n- [gogh](https://github.com/Mayccoll/Gogh)\n\nby default, lovesay checks for the quotes file at `$HOME/.config/lovesay/quotes` if there is nothing there and no quote is given using the cli args, it will just print out a heart with no quote\n\n---\n\n### ❖ About lovesay\n\nI wrote lovesay because I got tired of seeing neofetch or pfetch every time I opened my terminal. I wanted something more personal. \n\nSeeing words full of love from my partner is a lot better than any other command I could possibly run. It makes my terminal feel cozy, welcoming, and as is the case with most things my partner touches, it makes my terminal feel like home. \n\nI hope that someone else finds a use for this little script as well. Love is a wonderful thing, and we could all use a little bit more of it in our lives (especially arch linux users)\n\n---\n\n### ❖ What\'s New? \n0.3.8 - Black is now used for formatting alongside isort\n\n---\n\n<div align="center">\n\n   <img src="https://img.shields.io/static/v1.svg?label=License&message=MIT&color=F5E0DC&labelColor=302D41&style=for-the-badge">\n\n</div>\n',
-    'author': 'ZenithDS',
+    'long_description': '<h2 align="center"> ━━━━━━  ❖  ━━━━━━ </h2>\n\n<!-- BADGES -->\n<div align="center">\n   <p></p>\n   \n   <img src="https://img.shields.io/github/stars/dotzenith/lovesay?color=F8BD96&labelColor=302D41&style=for-the-badge">   \n\n   <img src="https://img.shields.io/github/forks/dotzenith/lovesay?color=DDB6F2&labelColor=302D41&style=for-the-badge">   \n\n   <img src="https://img.shields.io/github/repo-size/dotzenith/lovesay?color=ABE9B3&labelColor=302D41&style=for-the-badge">\n   \n   <img src="https://img.shields.io/github/commit-activity/y/dotzenith/lovesay?color=96CDFB&labelColor=302D41&style=for-the-badge&label=COMMITS"/>\n   <br>\n</div>\n\n<p/>\n\n---\n\n### ❖ Information \n\n  lovesay is a simple python script that displays a quote from a loved one based on the day of the month or a quote passed in through the cli arguments. \n\n  <img src="https://github.com/dotzenith/dotzenith/blob/main/assets/lovesay/lovesay.gif" alt="lovesay gif">\n\n---\n\n### ❖ Requirements\n\nNote: These requirements only apply if using you\'re using lovesay to print a different quote for each day of the month.  \n\n- A quotes file stored in `$HOME/.config/lovesay/`\n- Each quote must be on a new line, see the example quotes file in `.example/quotes`\n- (optional) A partner to write you 31 lines full of love, one for each day of the month\n\n---\n\n### ❖ Installation\n\n> Install from pip\n```sh\npip3 install lovesay\n```\n\n> Install from source\n- First, install [poetry](https://python-poetry.org/)\n```sh\ngit clone https://github.com/dotzenith/lovesay.git\ncd lovesay\npoetry build\npip3 install ./dist/lovesay-0.3.9.tar.gz\n```\n\n### ❖ Usage \n\nlovesay can be used in a similar fashion to cowsay\n\n```sh\nlovesay "Hello World"\n```\n\nif there\'s a `quotes` file in `$HOME/.config/lovesay/`, lovesay can be used without any arguments\n\n```sh\nlovesay\n```\n\nif you\'d like to use a quotes stored somewhere other than the path above, the `LOVESAY_PATH` env variable can be used as such\n\n```sh\nexport LOVESAY_PATH="~/path/to/file"\n```\n\nlovesay can also be used with a variety of different color schemes.\n\n> lovesay uses [catppuccin](https://github.com/catppuccin)(mocha) as it\'s default color scheme, but a different one can be specified using the `--color` option. \n\nFor example:\n```sh\nlovesay # uses catppuccin\n```\n  \n```sh\nlovesay -c nord # uses nord \n```\n\nSupported color schemes as of now: \n- [catppuccin](https://github.com/catppuccin) - latte, frappe, macchiato, mocha\n- [nord](https://github.com/arcticicestudio/nord)\n- [dracula](https://github.com/dracula/dracula-theme)\n- [gruvbox](https://github.com/morhetz/gruvbox)\n- [onedark](https://github.com/joshdick/onedark.vim)\n- [tokyonight](https://github.com/folke/tokyonight.nvim)\n- [ayu](https://github.com/ayu-theme)\n- [palenight](https://github.com/drewtempelmeyer/palenight.vim)\n- [gogh](https://github.com/Mayccoll/Gogh)\n\nby default, lovesay checks for the quotes file at `$HOME/.config/lovesay/quotes` if there is nothing there and no quote is given using the cli args, it will just print out a heart with no quote\n\n---\n\n### ❖ About lovesay\n\nI wrote lovesay because I got tired of seeing neofetch or pfetch every time I opened my terminal. I wanted something more personal. \n\nSeeing words full of love from my partner is a lot better than any other command I could possibly run. It makes my terminal feel cozy, welcoming, and as is the case with most things my partner touches, it makes my terminal feel like home. \n\nI hope that someone else finds a use for this little script as well. Love is a wonderful thing, and we could all use a little bit more of it in our lives (especially arch linux users)\n\n---\n\n### ❖ What\'s New? \n0.3.9 - Change author\n\n---\n\n<div align="center">\n\n   <img src="https://img.shields.io/static/v1.svg?label=License&message=MIT&color=F5E0DC&labelColor=302D41&style=for-the-badge">\n\n</div>\n',
+    'author': 'dotzenith',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
```

### Comparing `lovesay-0.3.8/PKG-INFO` & `lovesay-0.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lovesay
-Version: 0.3.8
+Version: 0.3.9
 Summary: Cowsay, but full of love
 License: MIT
-Author: ZenithDS
+Author: dotzenith
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: kolorz (>=0.2.1,<0.3.0)
@@ -43,33 +43,33 @@
 ---
 
 ### ❖ Requirements
 
 Note: These requirements only apply if using you're using lovesay to print a different quote for each day of the month.  
 
 - A quotes file stored in `$HOME/.config/lovesay/`
-- Each quote must be on a new line, see the example quotes file in `.config/lovesay/quotes`
+- Each quote must be on a new line, see the example quotes file in `.example/quotes`
 - (optional) A partner to write you 31 lines full of love, one for each day of the month
 
 ---
 
 ### ❖ Installation
 
 > Install from pip
 ```sh
 pip3 install lovesay
 ```
 
 > Install from source
 - First, install [poetry](https://python-poetry.org/)
 ```sh
-git clone https://github.com/ZenithDS/lovesay.git
+git clone https://github.com/dotzenith/lovesay.git
 cd lovesay
 poetry build
-pip3 install ./dist/lovesay-0.3.8.tar.gz
+pip3 install ./dist/lovesay-0.3.9.tar.gz
 ```
 
 ### ❖ Usage 
 
 lovesay can be used in a similar fashion to cowsay
 
 ```sh
@@ -123,15 +123,15 @@
 Seeing words full of love from my partner is a lot better than any other command I could possibly run. It makes my terminal feel cozy, welcoming, and as is the case with most things my partner touches, it makes my terminal feel like home. 
 
 I hope that someone else finds a use for this little script as well. Love is a wonderful thing, and we could all use a little bit more of it in our lives (especially arch linux users)
 
 ---
 
 ### ❖ What's New? 
-0.3.8 - Black is now used for formatting alongside isort
+0.3.9 - Change author
 
 ---
 
 <div align="center">
 
    <img src="https://img.shields.io/static/v1.svg?label=License&message=MIT&color=F5E0DC&labelColor=302D41&style=for-the-badge">
```

