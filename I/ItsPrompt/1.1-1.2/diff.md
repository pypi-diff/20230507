# Comparing `tmp/ItsPrompt-1.1.tar.gz` & `tmp/ItsPrompt-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ItsPrompt-1.1.tar", last modified: Wed Mar  8 19:00:09 2023, max compression
+gzip compressed data, was "ItsPrompt-1.2.tar", last modified: Sun May  7 11:29:09 2023, max compression
```

## Comparing `ItsPrompt-1.1.tar` & `ItsPrompt-1.2.tar`

### file list

```diff
@@ -1,28 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:09.200900 ItsPrompt-1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:09.196900 ItsPrompt-1.1/ItsPrompt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:09.196900 ItsPrompt-1.1/ItsPrompt/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/data/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/data/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/data/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/data/style.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/data/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/keyboard_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18060 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:09.200900 ItsPrompt-1.1/ItsPrompt/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/checkbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/confirm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/expand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/raw_select.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-03-08 18:59:58.000000 ItsPrompt-1.1/ItsPrompt/prompts/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-08 19:00:09.196900 ItsPrompt-1.1/ItsPrompt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-03-08 19:00:09.000000 ItsPrompt-1.1/ItsPrompt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-03-08 19:00:09.000000 ItsPrompt-1.1/ItsPrompt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-08 19:00:09.000000 ItsPrompt-1.1/ItsPrompt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-08 19:00:09.000000 ItsPrompt-1.1/ItsPrompt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-08 19:00:09.000000 ItsPrompt-1.1/ItsPrompt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-08 18:59:58.000000 ItsPrompt-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13184 2023-03-08 19:00:09.200900 ItsPrompt-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-03-08 18:59:58.000000 ItsPrompt-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-08 18:59:58.000000 ItsPrompt-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-08 19:00:09.200900 ItsPrompt-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.441138 ItsPrompt-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.433138 ItsPrompt-1.2/ItsPrompt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/data/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/keyboard_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20427 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     4951 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/checkbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/confirm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3721 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/expand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6353 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/raw_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-07 11:28:58.000000 ItsPrompt-1.2/ItsPrompt/prompts/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 11:29:09.437138 ItsPrompt-1.2/ItsPrompt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-07 11:29:09.000000 ItsPrompt-1.2/ItsPrompt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-07 11:28:58.000000 ItsPrompt-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16526 2023-05-07 11:29:09.441138 ItsPrompt-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14719 2023-05-07 11:28:58.000000 ItsPrompt-1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-07 11:28:58.000000 ItsPrompt-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 11:29:09.441138 ItsPrompt-1.2/setup.cfg
```

### Comparing `ItsPrompt-1.1/ItsPrompt/data/checkbox.py` & `ItsPrompt-1.2/ItsPrompt/data/checkbox.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/data/expand.py` & `ItsPrompt-1.2/ItsPrompt/data/expand.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/data/select.py` & `ItsPrompt-1.2/ItsPrompt/data/select.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/data/style.py` & `ItsPrompt-1.2/ItsPrompt/data/style.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/prompt.py` & `ItsPrompt-1.2/ItsPrompt/prompt.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,33 +5,35 @@
 
 :copyright: (c) 2023-present ItsNameless
 :license: MIT, see LICENSE for more details.
 '''
 
 from typing import Callable
 
+from pandas import DataFrame
 from prompt_toolkit import HTML
 from prompt_toolkit.buffer import Buffer
 from prompt_toolkit.completion import Completer
 from prompt_toolkit.layout.containers import (Float, FloatContainer, HSplit,
                                               VSplit, Window)
 from prompt_toolkit.layout.controls import BufferControl, FormattedTextControl
 from prompt_toolkit.layout.layout import Layout
 from prompt_toolkit.layout.menus import (CompletionsMenu,
                                          MultiColumnCompletionsMenu)
 
 from .data.style import PromptStyle, convert_style, default_style
 from .data.type import CompletionDict
-from .keyboard_handler import kb
+from .keyboard_handler import generate_key_bindings
 from .prompts.checkbox import CheckboxPrompt
 from .prompts.confirm import ConfirmPrompt
 from .prompts.expand import ExpandPrompt
 from .prompts.input import InputPrompt
 from .prompts.raw_select import RawSelectPrompt
 from .prompts.select import SelectPrompt
+from .prompts.table import TablePrompt
 
 
 class Prompt:
     '''
     # Modern python prompter
     
     This tool is used to ask the user questions, the fancy way.
@@ -78,15 +80,15 @@
                     Window(FormattedTextControl(), always_hide_cursor=True),
                     Window(FormattedTextControl(
                         HTML('Use UP, DOWN to select, ENTER to submit')),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
-            key_bindings=kb,
+            key_bindings=generate_key_bindings(SelectPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
@@ -134,15 +136,15 @@
                         HTML(
                             'Type the INDEX of your selection, ENTER to submit'
                         )),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
-            key_bindings=kb,
+            key_bindings=generate_key_bindings(RawSelectPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
@@ -192,15 +194,15 @@
                         HTML(
                             'Type the KEY for your selection, ENTER to submit (use h to show all options)'
                         )),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
-            key_bindings=kb,
+            key_bindings=generate_key_bindings(ExpandPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
@@ -253,15 +255,15 @@
                         HTML(
                             'Use UP, DOWN to change selection, SPACE to select, ENTER to submit'
                         )),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
-            key_bindings=kb,
+            key_bindings=generate_key_bindings(CheckboxPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
@@ -305,15 +307,15 @@
                         HTML(
                             'Press Y or N, ENTER if default value is available'
                         )),
                            char=' ',
                            style='class:tooltip',
                            height=1)
                 ])),
-            key_bindings=kb,
+            key_bindings=generate_key_bindings(ConfirmPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
 
         ans = app.prompt()
         if ans == None:
@@ -378,16 +380,16 @@
             VSplit([
                 Window(
                     FormattedTextControl(),
                     always_hide_cursor=True,
                     dont_extend_width=True,
                 ),
                 Window(
-                    BufferControl(
-                        Buffer(complete_while_typing=True))), # the completer will be passed in the Application class
+                    BufferControl(Buffer(complete_while_typing=True))
+                ),  # the completer will be passed in the Application class
             ]),
             Window(
                 FormattedTextControl(
                     HTML(
                         f'Type your answer, {"ALT+ENTER" if multiline else "ENTER"} to submit'
                     )),
                 char=' ',
@@ -401,25 +403,76 @@
             default,
             multiline,
             show_symbol,
             validate,
             completions,
             completer,
             layout=Layout(
-                FloatContainer(content=body,
-                               floats=[
-                                   Float(
-                                       MultiColumnCompletionsMenu(show_meta=False) if completion_show_multicolumn else CompletionsMenu(),
-                                       xcursor=True,
-                                       ycursor=True,
-                                   )
-                               ])),
-            key_bindings=kb,
+                FloatContainer(
+                    content=body,
+                    floats=[
+                        Float(
+                            MultiColumnCompletionsMenu(show_meta=False) if
+                            completion_show_multicolumn else CompletionsMenu(),
+                            xcursor=True,
+                            ycursor=True,
+                        )
+                    ])),
+            key_bindings=generate_key_bindings(InputPrompt),
             erase_when_done=True,
             style=convert_style(style)
             if style else convert_style(default_style),
         )
 
         ans = app.prompt()
         if ans == None:
             raise KeyboardInterrupt()
         return ans
+
+    @classmethod
+    def table(
+        cls,
+        question: str,
+        data: DataFrame,
+        style: PromptStyle | None = None,
+    ) -> DataFrame:
+        '''
+        Ask the user for filling out the displayed table.
+
+        This method shows the question alongside a table, which the user may navigate with the arrow keys. The user has the ability to use the up, down and enter keys to navigate between the options and change the text in each cell.
+
+        The `data` is a pandas DataFrame, where the values will be input in the cells by default.
+
+        # TODO
+        :param question: The question to display
+        :type question: str
+        :param options: A list of possible options
+        :type options: tuple[str  |  tuple[str, str], ...]
+        :param default: The id of the default option to select (empty or None if the first should be default), defaults to None
+        :type default: str | None, optional
+        :param style: A separate style to style the prompt (empty or None for default style), defaults to None
+        :type style: PromptStyle | None, optional
+        :raises KeyboardInterrupt: When the user presses ctrl-c, `KeyboardInterrupt` will be raised
+        :return: The id of the selected option
+        :rtype: str
+        '''
+        app = TablePrompt(
+            question,
+            data,
+            layout=Layout(
+                HSplit([
+                    Window(FormattedTextControl()),
+                    Window(FormattedTextControl(
+                        HTML('Use UP, DOWN, LEFT, RIGHT to select a cell, TYPE to add char, BACKSPACE to delete char, ENTER to submit')),
+                           char=' ',
+                           style='class:tooltip',
+                           height=1)
+                ])),
+            key_bindings=generate_key_bindings(TablePrompt),
+            erase_when_done=True,
+            style=convert_style(style)
+            if style else convert_style(default_style),
+        )
+        ans = app.prompt()
+        if type(ans) != DataFrame and ans == None:
+            raise KeyboardInterrupt()
+        return ans
```

### Comparing `ItsPrompt-1.1/ItsPrompt/prompts/checkbox.py` & `ItsPrompt-1.2/ItsPrompt/prompts/checkbox.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/prompts/confirm.py` & `ItsPrompt-1.2/ItsPrompt/prompts/confirm.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/prompts/expand.py` & `ItsPrompt-1.2/ItsPrompt/prompts/expand.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/prompts/raw_select.py` & `ItsPrompt-1.2/ItsPrompt/prompts/raw_select.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt/prompts/select.py` & `ItsPrompt-1.2/ItsPrompt/prompts/select.py`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/ItsPrompt.egg-info/PKG-INFO` & `ItsPrompt-1.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,7 @@
-Metadata-Version: 2.1
-Name: ItsPrompt
-Version: 1.1
-Summary: Prompting - the fancy way
-Author: ItsNameless
-License: MIT License
-        
-        Copyright (c) 2023-present ItsNameless
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-        
-Project-URL: Homepage, https://github.com/TheItsProjects/ItsPrompt
-Project-URL: Repository, https://github.com/TheItsProjects/ItsPrompt
-Project-URL: Issue Tracker, https://github.com/TheItsProjects/ItsPrompt/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI version](https://badge.fury.io/py/ItsPrompt.svg)](https://badge.fury.io/py/ItsPrompt)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ItsPrompt)](https://pypi.org/project/ItsPrompt/)
 [![GitHub issues](https://img.shields.io/github/issues/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/issues)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/stargazers)
 [![GitHub](https://img.shields.io/github/license/TheitsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/1082381448624996514)](https://discord.gg/rP9Qke2jDs)
 
@@ -54,37 +17,62 @@
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
 **ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
 
+# TOC
+
+- [ItsPrompt](#itsprompt)
+- [TOC](#toc)
+    - [A small, thankful note](#a-small-thankful-note)
+  - [Features](#features)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Prompt types](#prompt-types)
+    - [`select`](#select)
+    - [`raw_select`](#raw_select)
+    - [`expand`](#expand)
+    - [`checkbox`](#checkbox)
+    - [`confirm`](#confirm)
+    - [`input`](#input)
+    - [`table`](#table)
+  - [Additional Features and Tips](#additional-features-and-tips)
+    - [Options](#options)
+    - [Data](#data)
+    - [Styling](#styling)
+    - [Prompt Validation](#prompt-validation)
+    - [Prompt Completion](#prompt-completion)
+    - [Further Information](#further-information)
+
 ---
 
 ### A small, thankful note
 
 This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
 
 On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without every looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
 
 On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
     - raw_select
     - expand
     - checkbox
     - confirm
     - input
+    - table
 - big feature set
 - simple, pythonic syntax
 - a helpful toolbar with error messages
 - customizable style with `prompt-toolkit`
 
 ---
 
@@ -216,14 +204,28 @@
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
+### `table`
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
+
+```py
+Prompt.table(
+    question='something',
+    data=DataFrame(['something']),
+    style=my_style,
+)
+```
+
+*additional information on the function arguments can be found in the docstring*
+
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
 The `options` is always a `tuple` containing `str` and `tuple` objects. 
@@ -234,20 +236,69 @@
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
+### Data
+
+The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
+
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+
+---
+
 ### Styling
 
 **ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
 
 You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+
+```py
+# examples for the different styling class components
+Prompt.raw_select(
+    question='question',
+    options=(
+        'option',
+        'selected_option',
+    )
+)
+
+Prompt.input(
+    question='question',
+    default='grayout',
+    validate=lambda x: 'error',
+)
+```
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
+
+| ID  |    styling tag    |             default style             |
+| --- | ----------------- | ------------------------------------- |
+| 1   | `question_mark`   | `fg:ansigreen`                        |
+| 2   | `question`        | *                                     |
+| 3   | `option`          | *                                     |
+| 4   | `selected_option` | `fg:ansicyan`                         |
+| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6   | `text`            | *                                     |
+| 7   | `grayout`          | `fg:ansibrightblack`                  |
+| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+
+*\*These values are not changed from the default `prompt-toolkit` values.*
+
+
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -267,15 +318,15 @@
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. If you want this to be the case, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
@@ -393,12 +444,14 @@
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
-If you got any other questions, or want to give an idea on how to improve **ItsPrompt**, join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
+If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+- visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
+- join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.1/ItsPrompt.egg-info/SOURCES.txt` & `ItsPrompt-1.2/ItsPrompt.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 ItsPrompt.egg-info/dependency_links.txt
 ItsPrompt.egg-info/requires.txt
 ItsPrompt.egg-info/top_level.txt
 ItsPrompt/data/checkbox.py
 ItsPrompt/data/expand.py
 ItsPrompt/data/select.py
 ItsPrompt/data/style.py
+ItsPrompt/data/table.py
 ItsPrompt/data/type.py
 ItsPrompt/prompts/checkbox.py
 ItsPrompt/prompts/confirm.py
 ItsPrompt/prompts/expand.py
 ItsPrompt/prompts/input.py
 ItsPrompt/prompts/raw_select.py
-ItsPrompt/prompts/select.py
+ItsPrompt/prompts/select.py
+ItsPrompt/prompts/table.py
```

### Comparing `ItsPrompt-1.1/LICENSE` & `ItsPrompt-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ItsPrompt-1.1/PKG-INFO` & `ItsPrompt-1.2/ItsPrompt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ItsPrompt
-Version: 1.1
+Version: 1.2
 Summary: Prompting - the fancy way
 Author: ItsNameless
 License: MIT License
         
         Copyright (c) 2023-present ItsNameless
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -54,37 +54,62 @@
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
 **ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
 
+# TOC
+
+- [ItsPrompt](#itsprompt)
+- [TOC](#toc)
+    - [A small, thankful note](#a-small-thankful-note)
+  - [Features](#features)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Prompt types](#prompt-types)
+    - [`select`](#select)
+    - [`raw_select`](#raw_select)
+    - [`expand`](#expand)
+    - [`checkbox`](#checkbox)
+    - [`confirm`](#confirm)
+    - [`input`](#input)
+    - [`table`](#table)
+  - [Additional Features and Tips](#additional-features-and-tips)
+    - [Options](#options)
+    - [Data](#data)
+    - [Styling](#styling)
+    - [Prompt Validation](#prompt-validation)
+    - [Prompt Completion](#prompt-completion)
+    - [Further Information](#further-information)
+
 ---
 
 ### A small, thankful note
 
 This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
 
 On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without every looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
 
 On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
     - raw_select
     - expand
     - checkbox
     - confirm
     - input
+    - table
 - big feature set
 - simple, pythonic syntax
 - a helpful toolbar with error messages
 - customizable style with `prompt-toolkit`
 
 ---
 
@@ -216,14 +241,28 @@
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
+### `table`
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
+
+```py
+Prompt.table(
+    question='something',
+    data=DataFrame(['something']),
+    style=my_style,
+)
+```
+
+*additional information on the function arguments can be found in the docstring*
+
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
 The `options` is always a `tuple` containing `str` and `tuple` objects. 
@@ -234,20 +273,69 @@
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
+### Data
+
+The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
+
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+
+---
+
 ### Styling
 
 **ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
 
 You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+
+```py
+# examples for the different styling class components
+Prompt.raw_select(
+    question='question',
+    options=(
+        'option',
+        'selected_option',
+    )
+)
+
+Prompt.input(
+    question='question',
+    default='grayout',
+    validate=lambda x: 'error',
+)
+```
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
+
+| ID  |    styling tag    |             default style             |
+| --- | ----------------- | ------------------------------------- |
+| 1   | `question_mark`   | `fg:ansigreen`                        |
+| 2   | `question`        | *                                     |
+| 3   | `option`          | *                                     |
+| 4   | `selected_option` | `fg:ansicyan`                         |
+| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6   | `text`            | *                                     |
+| 7   | `grayout`          | `fg:ansibrightblack`                  |
+| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+
+*\*These values are not changed from the default `prompt-toolkit` values.*
+
+
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -267,15 +355,15 @@
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. If you want this to be the case, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
@@ -393,12 +481,14 @@
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
-If you got any other questions, or want to give an idea on how to improve **ItsPrompt**, join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
+If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+- visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
+- join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.1/README.md` & `ItsPrompt-1.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,44 @@
+Metadata-Version: 2.1
+Name: ItsPrompt
+Version: 1.2
+Summary: Prompting - the fancy way
+Author: ItsNameless
+License: MIT License
+        
+        Copyright (c) 2023-present ItsNameless
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/TheItsProjects/ItsPrompt
+Project-URL: Repository, https://github.com/TheItsProjects/ItsPrompt
+Project-URL: Issue Tracker, https://github.com/TheItsProjects/ItsPrompt/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI version](https://badge.fury.io/py/ItsPrompt.svg)](https://badge.fury.io/py/ItsPrompt)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ItsPrompt)](https://pypi.org/project/ItsPrompt/)
 [![GitHub issues](https://img.shields.io/github/issues/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/issues)
 [![GitHub Repo stars](https://img.shields.io/github/stars/TheItsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/stargazers)
 [![GitHub](https://img.shields.io/github/license/TheitsProjects/ItsPrompt)](https://github.com/TheItsProjects/ItsPrompt/blob/main/LICENSE)
 [![Discord](https://img.shields.io/discord/1082381448624996514)](https://discord.gg/rP9Qke2jDs)
 
@@ -17,37 +54,62 @@
 
 And do you think all of this should be done easily, without caring to much how it all works?
 
 Then you are right here! **ItsPrompt** gives you the ability to ask the user for input, the *fancy* way.
 
 **ItsPrompt** tries to be an easy-to-use module for managing prompts for the user. You task is to create a great program, not how to ask the user for input. That is why **ItsPrompt** is there to take care of this problem, so you can focus on the important things!
 
+# TOC
+
+- [ItsPrompt](#itsprompt)
+- [TOC](#toc)
+    - [A small, thankful note](#a-small-thankful-note)
+  - [Features](#features)
+  - [Installation](#installation)
+  - [Usage](#usage)
+  - [Prompt types](#prompt-types)
+    - [`select`](#select)
+    - [`raw_select`](#raw_select)
+    - [`expand`](#expand)
+    - [`checkbox`](#checkbox)
+    - [`confirm`](#confirm)
+    - [`input`](#input)
+    - [`table`](#table)
+  - [Additional Features and Tips](#additional-features-and-tips)
+    - [Options](#options)
+    - [Data](#data)
+    - [Styling](#styling)
+    - [Prompt Validation](#prompt-validation)
+    - [Prompt Completion](#prompt-completion)
+    - [Further Information](#further-information)
+
 ---
 
 ### A small, thankful note
 
 This project is not the first to accomplish the above mentioned tasks. There is another package, `PyInquirer`, which inspired me to build **ItsPrompt**.
 
 On my way to create a small program I came to a point were I needed a simple GUI, and I tried `PyInquirer`. Unfortunately, at the current time it is not actively maintained and a bit outdated. I thought of updating it, but then I thought "*Isn't it easier to just create my own version?*" - And so I did!
 
-**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without every looking deep into the source code of `PyInquirer`.
+**ItsPrompt** is not a copy or a fork of `PyInquirer`. I built this module from the ground up, without ever looking deep into the source code of `PyInquirer`.
 
 On my way to build this package, I learned a lot about `prompt-toolkit`, and all of this just because of `PyInquirer`! Thanks!
 
 ---
 
 ## Features
 
 - many prompt types (more details below):
     - select
     - raw_select
     - expand
     - checkbox
     - confirm
     - input
+    - table
 - big feature set
 - simple, pythonic syntax
 - a helpful toolbar with error messages
 - customizable style with `prompt-toolkit`
 
 ---
 
@@ -179,14 +241,28 @@
     completion_show_multicolumn=True,
     style=my_style,
 )
 ```
 
 *additional information on the function arguments can be found in the docstring*
 
+### `table`
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/table.png)
+
+```py
+Prompt.table(
+    question='something',
+    data=DataFrame(['something']),
+    style=my_style,
+)
+```
+
+*additional information on the function arguments can be found in the docstring*
+
 ---
 
 ## Additional Features and Tips
 
 ### Options
 
 The `options` is always a `tuple` containing `str` and `tuple` objects. 
@@ -197,20 +273,69 @@
 
 If an option is given as a `tuple`, the first value will be the options name, the second value the options id to return.
 
 *In case of `expand`, the first value will be the key, the second value the name and the third value the id.*
 
 ---
 
+### Data
+
+The `table` prompt takes a mandatory `data` argument, which needs to be a `pandas.DataFrame`.
+
+This `DataFrame` is used as the content of the table. The user may change the fields of the table. The output of the `table` prompt is a `pandas.DataFrame` with the user given values.
+
+Currently, the output will convert all input values to a `str`, so `int`, `bool`, ... will be converted to strings. This is a current limitation of the way the table is displayed, but may later be updated.
+
+Another limitation of the `table` prompt is the use of styling in the `DataFrame` fields. All styling tags will be displayed as-is, so a `<u>...</u>` will not be underlined, but rather displayed as its shown.
+
+---
+
 ### Styling
 
 **ItsPrompt** uses `prompt-toolkit` for its prompts. This module not only provides an easy way to interact with the command line, but also a full set of styling features.
 
 You can learn more about the available styling features in the documentation of `prompt-toolkit`: [Styling](https://python-prompt-toolkit.readthedocs.io/en/master/pages/printing_text.html#formatted-text).
 
+**ItsPrompt** makes it a bit easier for you to style each component of a prompt. For every component, we give a separate attribute in the `PromptStyle` class, which you can style with valid `prompt-toolkit` styling:
+
+```py
+# examples for the different styling class components
+Prompt.raw_select(
+    question='question',
+    options=(
+        'option',
+        'selected_option',
+    )
+)
+
+Prompt.input(
+    question='question',
+    default='grayout',
+    validate=lambda x: 'error',
+)
+```
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_raw_select_annotated.png)
+
+![](https://raw.githubusercontent.com/TheItsProjects/ItsPrompt/main/media/styling_input_annotated.png)
+
+| ID  |    styling tag    |             default style             |
+| --- | ----------------- | ------------------------------------- |
+| 1   | `question_mark`   | `fg:ansigreen`                        |
+| 2   | `question`        | *                                     |
+| 3   | `option`          | *                                     |
+| 4   | `selected_option` | `fg:ansicyan`                         |
+| 5   | `tooltip`         | `fg:ansibrightblue bg:ansiwhite bold` |
+| 6   | `text`            | *                                     |
+| 7   | `grayout`          | `fg:ansibrightblack`                  |
+| 8   | `error`           | `fg:ansiwhite bg:ansired bold`        |
+
+*\*These values are not changed from the default `prompt-toolkit` values.*
+
+
 To create your own style, there are two ways:
 
 ***Changing the default style***
 
 To change the default style, you need to import the `default_style` and change its values:
 
 ```py
@@ -230,15 +355,15 @@
 
 my_style = PromptStyle(
     question_mark='fg:ansiblue',
     error='fg:ansired bg:ansiwhite',
 )
 ```
 
-All styles which are not given, **will not** be the same as the default style. If you want this to be the case, then copy the `default_style` and change your values, instead of directly creating your own style:
+All styles which are not given, **will not** be the same as the default style. Instead they will use the styling given by `prompt-toolkit`. If you want to change our default styles, then copy the `default_style` and change your values, instead of directly creating your own style:
 
 ```py
 from ItsPrompt.data.style import create_from_default
 
 my_style = create_from_default()
 
 my_style.error = 'fg:ansired bg:ansiwhite'
@@ -356,12 +481,14 @@
 
 ### Further Information
 
 If you need some easy examples, refer to [example.py](example.py)!
 
 If you want to contribute, check out the projects repository: [ItsPrompt](https://github.com/TheItsProjects/ItsPrompt)!
 
-If you got any other questions, or want to give an idea on how to improve **ItsPrompt**, join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
+If you got any other questions, or want to give an idea on how to improve **ItsPrompt**:
+- visit our discussions: [ItsPrompt Discussions](https://github.com/TheItsProjects/ItsPrompt/discussions)!
+- join our discord: [TheItsProjects](https://discord.gg/rP9Qke2jDs)!
 
 ---
 
 Puh, that was so much to read... But now, lets have fun with **ItsPrompt**!
```

### Comparing `ItsPrompt-1.1/pyproject.toml` & `ItsPrompt-1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ItsPrompt"
-version = "1.1"
+version = "1.2"
 authors = [
     {name = "ItsNameless"}
 ]
 description = "Prompting - the fancy way"
 readme = "README.md"
 requires-python = ">=3.8"
 dependencies = [
```

