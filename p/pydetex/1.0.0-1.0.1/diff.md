# Comparing `tmp/pydetex-1.0.0.tar.gz` & `tmp/pydetex-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydetex-1.0.0.tar", last modified: Mon May  1 22:29:35 2023, max compression
+gzip compressed data, was "pydetex-1.0.1.tar", last modified: Sun May  7 20:52:57 2023, max compression
```

## Comparing `pydetex-1.0.0.tar` & `pydetex-1.0.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.060000 pydetex-1.0.0/
--rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5567 2023-05-01 22:29:36.000000 pydetex-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4370 2023-03-08 22:09:00.000000 pydetex-1.0.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.080000 pydetex-1.0.0/pydetex/
--rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-1.0.0/pydetex/__init__.py
--rw-rw-rw-   0        0        0     1314 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/_fonts.py
--rw-rw-rw-   0        0        0    24925 2022-12-05 13:17:22.000000 pydetex-1.0.0/pydetex/_gui_settings.py
--rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-1.0.0/pydetex/_gui_utils.py
--rw-rw-rw-   0        0        0    23415 2022-05-13 22:07:20.000000 pydetex-1.0.0/pydetex/_symbols.py
--rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/_utils_lang.py
--rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/_utils_tex.py
--rw-rw-rw-   0        0        0    30942 2022-05-13 22:07:20.000000 pydetex-1.0.0/pydetex/gui.py
--rw-rw-rw-   0        0        0    46650 2023-03-08 21:59:08.000000 pydetex-1.0.0/pydetex/parsers.py
--rw-rw-rw-   0        0        0     2941 2023-02-15 12:36:20.000000 pydetex-1.0.0/pydetex/pipelines.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.120000 pydetex-1.0.0/pydetex/res/
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.0/pydetex/res/cog.ico
--rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:18.000000 pydetex-1.0.0/pydetex/res/dictionary.ico
--rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-1.0.0/pydetex/res/icon.gif
--rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.0/pydetex/res/icon.ico
--rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/res/placeholder_en.tex
--rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-1.0.0/pydetex/res/placeholder_es.tex
--rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-1.0.0/pydetex/res/stopwords.json
--rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_subscripts.txt
--rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_superscripts.txt
--rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_symbols.txt
--rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textbb.txt
--rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textbf.txt
--rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textcal.txt
--rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textfrak.txt
--rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textit.txt
--rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-1.0.0/pydetex/res/u_textmono.txt
--rw-rw-rw-   0        0        0     8357 2022-12-05 13:17:22.000000 pydetex-1.0.0/pydetex/utils.py
--rw-rw-rw-   0        0        0      789 2023-05-01 22:29:30.000000 pydetex-1.0.0/pydetex/version.py
-drwxrwxrwx   0        0        0        0 2023-05-01 22:29:35.100000 pydetex-1.0.0/pydetex.egg-info/
--rw-rw-rw-   0        0        0     5567 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      870 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      284 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-01 22:29:36.000000 pydetex-1.0.0/pydetex.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      173 2023-05-01 22:26:04.000000 pydetex-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 22:29:36.000000 pydetex-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1872 2023-04-13 16:52:48.000000 pydetex-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.820000 pydetex-1.0.1/
+-rw-rw-rw-   0        0        0     1073 2021-10-03 21:53:42.000000 pydetex-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      406 2021-11-01 21:25:22.000000 pydetex-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     5567 2023-05-07 20:52:58.000000 pydetex-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4370 2023-03-08 22:09:00.000000 pydetex-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.880000 pydetex-1.0.1/pydetex/
+-rw-rw-rw-   0        0        0      721 2022-02-03 13:19:14.000000 pydetex-1.0.1/pydetex/__init__.py
+-rw-rw-rw-   0        0        0     1314 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/_fonts.py
+-rw-rw-rw-   0        0        0    25324 2023-05-07 18:03:40.000000 pydetex-1.0.1/pydetex/_gui_settings.py
+-rw-rw-rw-   0        0        0    45460 2023-02-15 12:36:58.000000 pydetex-1.0.1/pydetex/_gui_utils.py
+-rw-rw-rw-   0        0        0    23466 2023-05-07 20:24:00.000000 pydetex-1.0.1/pydetex/_symbols.py
+-rw-rw-rw-   0        0        0     9705 2023-02-15 12:36:20.000000 pydetex-1.0.1/pydetex/_utils_lang.py
+-rw-rw-rw-   0        0        0    23887 2023-02-15 12:36:20.000000 pydetex-1.0.1/pydetex/_utils_tex.py
+-rw-rw-rw-   0        0        0    30942 2022-05-13 22:07:20.000000 pydetex-1.0.1/pydetex/gui.py
+-rw-rw-rw-   0        0        0    45728 2023-05-07 20:39:50.000000 pydetex-1.0.1/pydetex/parsers.py
+-rw-rw-rw-   0        0        0     3887 2023-05-07 20:26:56.000000 pydetex-1.0.1/pydetex/pipelines.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.990000 pydetex-1.0.1/pydetex/res/
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.1/pydetex/res/cog.ico
+-rw-rw-rw-   0        0        0     4286 2021-10-18 04:07:18.000000 pydetex-1.0.1/pydetex/res/dictionary.ico
+-rw-rw-rw-   0        0        0    13224 2021-09-14 16:31:46.000000 pydetex-1.0.1/pydetex/res/icon.gif
+-rw-rw-rw-   0        0        0     4286 2021-10-13 18:08:22.000000 pydetex-1.0.1/pydetex/res/icon.ico
+-rw-rw-rw-   0        0        0      554 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/res/placeholder_en.tex
+-rw-rw-rw-   0        0        0      605 2021-11-14 20:58:54.000000 pydetex-1.0.1/pydetex/res/placeholder_es.tex
+-rw-rw-rw-   0        0        0   184280 2021-10-16 20:19:00.000000 pydetex-1.0.1/pydetex/res/stopwords.json
+-rw-rw-rw-   0        0        0      227 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_subscripts.txt
+-rw-rw-rw-   0        0        0      416 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_superscripts.txt
+-rw-rw-rw-   0        0        0     4861 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_symbols.txt
+-rw-rw-rw-   0        0        0      427 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textbb.txt
+-rw-rw-rw-   0        0        0      900 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textbf.txt
+-rw-rw-rw-   0        0        0      364 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textcal.txt
+-rw-rw-rw-   0        0        0      359 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textfrak.txt
+-rw-rw-rw-   0        0        0      829 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textit.txt
+-rw-rw-rw-   0        0        0      434 2020-02-26 08:23:30.000000 pydetex-1.0.1/pydetex/res/u_textmono.txt
+-rw-rw-rw-   0        0        0     8362 2023-05-07 20:35:20.000000 pydetex-1.0.1/pydetex/utils.py
+-rw-rw-rw-   0        0        0      789 2023-05-07 20:13:54.000000 pydetex-1.0.1/pydetex/version.py
+drwxrwxrwx   0        0        0        0 2023-05-07 20:52:54.930000 pydetex-1.0.1/pydetex.egg-info/
+-rw-rw-rw-   0        0        0     5567 2023-05-07 20:52:54.000000 pydetex-1.0.1/pydetex.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      870 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      284 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-07 20:52:56.000000 pydetex-1.0.1/pydetex.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      173 2023-05-01 22:26:04.000000 pydetex-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 20:52:58.000000 pydetex-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1872 2023-04-13 16:52:48.000000 pydetex-1.0.1/setup.py
```

### Comparing `pydetex-1.0.0/LICENSE` & `pydetex-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/PKG-INFO` & `pydetex-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydetex
-Version: 1.0.0
+Version: 1.0.1
 Summary: An application that transforms LaTeX code to plain text
 Home-page: https://pydetex.readthedocs.io
 Author: Pablo Pizarro R.
 Author-email: pablo@ppizarror.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
 Project-URL: Documentation, https://pydetex.readthedocs.io
```

### Comparing `pydetex-1.0.0/README.rst` & `pydetex-1.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/__init__.py` & `pydetex-1.0.1/pydetex/__init__.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/_fonts.py` & `pydetex-1.0.1/pydetex/_fonts.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/_gui_settings.py` & `pydetex-1.0.1/pydetex/_gui_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,16 @@
 
 _SETTINGS_FILE = [os.path.join(ut.get_local_path(), '.pydetex.cfg')]
 _SETTINGS_TEST = os.path.join(ut.RESOURCES_PATH, '.pydetex.cfg')
 
 # Store the pipelines
 _PIPELINES = {
     'pipeline_simple': pip.simple,
-    'pipeline_strict': pip.strict
+    'pipeline_strict': pip.strict,
+    'pipeline_strict_eqn': pip.strict_eqn
 }
 
 # Store the window sizes (w, h, height_richtext, margin_between_richtext, button_margin)
 _WINDOW_SIZE = {
     'window_size_small': [720, 480, 175, 3, 6],
     'window_size_medium': [960, 540, 200, 5, 10],
     'window_size_large': [1280, 720, 285, 5, 15],
@@ -115,15 +116,17 @@
                 'menu_paste': 'Paste',
                 'open_file': 'Open file',
                 'open_file_latex_file': 'LaTeX file',
                 'open_file_select': 'Select a LaTeX file',
                 'pipeline_simple': 'Simple',
                 'pipeline_simple_description': 'Removes common Tex commands, replaces cites and references',
                 'pipeline_strict': 'Strict',
-                'pipeline_strict_description': 'An extension of the Simple pipeline which removes all Tex commands and environments',
+                'pipeline_strict_description': 'An extension of the simple pipeline which removes all Tex commands and environments',
+                'pipeline_strict_eqn': 'Strict + equation',
+                'pipeline_strict_eqn_description': 'An extension of the strict pipeline which converts also the equations',
                 'placeholder': ut.open_file(ut.RESOURCES_PATH + 'placeholder_en.tex'),
                 'process': 'Process',
                 'process_clip': 'Process from clipboard',
                 'process_copy': 'Copy to clipboard',
                 'process_error': 'An error has occured while processing the text.\nPlease create a new issue in the GitHub '
                                  'page ({0}) with full defails and minimal working example.\n\nError traceback:\n{1}\n',
                 'reload_message_message': 'To apply these changes, the app must be reloaded',
@@ -224,14 +227,16 @@
                 'open_file': 'Abrir archivo',
                 'open_file_latex_file': 'Archivo LaTeX',
                 'open_file_select': 'Selecciona un archivo LaTeX',
                 'pipeline_simple': 'Simple',
                 'pipeline_simple_description': 'Elimina comandos Tex comunes, remplaza citas y referencias',
                 'pipeline_strict': 'Estricto',
                 'pipeline_strict_description': 'Una extensión del pipeline simple que elimina todos los entornos y comandos',
+                'pipeline_strict_eqn': 'Estricto + ecuación',
+                'pipeline_strict_eqn_description': 'Pipeline estricto que además reemplaza las ecuaciones',
                 'placeholder': ut.open_file(ut.RESOURCES_PATH + 'placeholder_es.tex'),
                 'process': 'Procesar',
                 'process_clip': 'Procesar desde portapapeles',
                 'process_copy': 'Copiar al portapapeles',
                 'process_error': 'Un error ha ocurrido mientras se procesaba el texto.\nPor favor crea un nuevo issue en'
                                  ' la página de GitHub ({0}) con los detalles completos y un ejemplo mínimo para probar'
                                  ' las soluciones.\n\nDetalles del error:\n{1}\n',
```

### Comparing `pydetex-1.0.0/pydetex/_gui_utils.py` & `pydetex-1.0.1/pydetex/_gui_utils.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/_symbols.py` & `pydetex-1.0.1/pydetex/_symbols.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,14 +131,15 @@
     ('\\asymp', '≍'),
     ('\\backepsilon', '϶'),
     ('\\backprime', '‵'),
     ('\\backsim', '∽'),
     ('\\backsimeq', '⋍'),
     ('\\barwedge', '⊼'),
     ('\\because', '∵'),
+    ('\\beginsmallmatrix', ''),
     ('\\beta', 'β'),
     ('\\beth', 'ℶ'),
     ('\\between', '≬'),
     ('\\bigcap', '⋂'),
     ('\\bigcup', '⋃'),
     ('\\bigodot', '⨀'),
     ('\\bigoplus', '⨁'),
@@ -285,15 +286,15 @@
     ('\\Koppa', 'Ϟ'),
     ('\\koppa', 'ϟ'),
     ('\\Lambda', 'Λ'),
     ('\\lambda', 'λ'),
     ('\\langle', '〈'),
     ('\\lceil', '⌈'),
     ('\\ldots', '…'),
-    ('\\le', '≤'),
+    ('\\left', ''),
     ('\\leftarrow', '←'),
     ('\\Leftarrow', '⇐'),
     ('\\LeftArrowBar', '⇤'),
     ('\\leftarrowtail', '↢'),
     ('\\leftarrowtriangle', '⇽'),
     ('\\leftharpoondown', '↽'),
     ('\\leftharpoonup', '↼'),
@@ -788,14 +789,15 @@
     ('\\sum', '∑'),
     ('\\supset', '⊃'),
     ('\\Supset', '⋑'),
     ('\\supseteq', '⊇'),
     ('\\supsetneq', '⊋'),
     ('\\swarrow', '↙'),
     ('\\tau', 'τ'),
+    ('\\text', ''),
     ('\\textasciimacron', '¯'),
     ('\\textbardbl', '‖'),
     ('\\textbrokenbar', '¦'),
     ('\\textcent', '¢'),
     ('\\textcurrency', '¤'),
     ('\\textdiscount', '⁒'),
     ('\\textestimated', '℮'),
```

### Comparing `pydetex-1.0.0/pydetex/_utils_lang.py` & `pydetex-1.0.1/pydetex/_utils_lang.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/_utils_tex.py` & `pydetex-1.0.1/pydetex/_utils_tex.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/gui.py` & `pydetex-1.0.1/pydetex/gui.py`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/parsers.py` & `pydetex-1.0.1/pydetex/parsers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1393 +1,1403 @@
-"""
-PyDetex
-https://github.com/ppizarror/PyDetex
-
-PARSERS
-Defines parsers, which perform a single task for removal LaTex things.
-"""
-
-__all__ = [
-    'find_str',
-    'FONT_FORMAT_SETTINGS',
-    'process_begin_document',
-    'process_chars_equations',
-    'process_cite',
-    'process_citeauthor',
-    'process_def',
-    'process_inputs',
-    'process_items',
-    'process_labels',
-    'process_ref',
-    'remove_commands_char',
-    'remove_commands_param',
-    'remove_commands_param_noargv',
-    'remove_comments',
-    'remove_common_tags',
-    'remove_environments',
-    'remove_equations',
-    'remove_tag',
-    'replace_pydetex_tags',
-    'simple_replace',
-    'strip_punctuation',
-    'unicode_chars_equations'
-]
-
-import os
-import pydetex.utils as ut
-
-from pydetex._symbols import *
-from typing import List, Tuple, Union, Optional, Callable
-
-# Files
-_LAST_NOT_FOUND_FILES_PATH = [os.getcwd()]
-_NOT_FOUND_FILES = []
-_PRINT_LOCATION = False
-
-# Tags
-_TAG_BRACE_CLOSE = '⇱BRACE_CLOSE⇲'
-_TAG_BRACE_OPEN = '⇱BRACE_OPEN⇲'
-_TAG_CLOSE_CITE = '⇱CLOSE_CITE⇲'
-_TAG_DOLLAR_SYMBOL = '⇱DOLLAR_SYMBOL⇲'
-_TAG_FILE_ERROR = '⇱FILE_ERROR⇲'
-_TAG_ITEM_SPACE = '⇱ITEM_SPACE⇲'
-_TAG_NEW_LINE = '⇱NEW_LINE⇲'
-_TAG_OPEN_CITE = '⇱OPEN_CITE⇲'
-_TAG_PERCENTAGE_SYMBOL = '⇱COMMENT_PERCENTAGE_SYMBOL⇲'
-
-# Others
-_ROMAN_DIGITS = [
-    (1000, 'M'),
-    (900, 'CM'),
-    (500, 'D'),
-    (400, 'CD'),
-    (100, 'C'),
-    (90, 'XC'),
-    (50, 'L'),
-    (40, 'XL'),
-    (10, 'X'),
-    (9, 'IX'),
-    (5, 'V'),
-    (4, 'IV'),
-    (1, 'I')
-]
-
-# Stores the learned definitions
-_DEFS = {}
-
-# Parser font format. This dict stores the font of some tex elements to be represented
-# in the GUI text editor. The values are the same of _fonts.FONT_TAGS. By default,
-# they are empty, and are updated in the PyDetexGUI._process() method
-FONT_FORMAT_SETTINGS = {
-    'bold': '',
-    'cite': '',
-    'equation': '',
-    'italic': '',
-    'normal': '',
-    'ref': '',
-    'tex_text_tag': '',
-    'tex_text_tag_content': ''
-}
-
-LANG_TT_TAGS = ut.LangTexTextTags()
-
-
-def _find_str(s: str, char: str) -> int:
-    """
-    Finds a sequence within a string, and returns the position. If not exists, returns ``-1``.
-
-    :param s: Latex string code
-    :param char: Sequence
-    :return: Position
-    """
-    index = 0
-
-    if char in s:
-        c = char[0]
-        for ch in s:
-            if ch == c:
-                if s[index:index + len(char)] == char:
-                    return index
-
-            index += 1
-
-    return -1
-
-
-def _os_listfolder() -> List[str]:
-    """
-    Returns the folders from the current path.
-
-    :return: Folder list
-    """
-    dirs = os.listdir('./')
-    folders = []
-    for k in dirs:
-        if os.path.isdir(k):
-            folders.append(k + '/')
-    return folders
-
-
-def _load_file(f: str, path: str) -> str:
-    """
-    Try to load a file.
-
-    :param f: Filename
-    :param path: Path to look from
-    :return: File contents
-    """
-    try:
-        return ut.open_file(path + f)
-    except FileNotFoundError:
-        return _TAG_FILE_ERROR
-
-
-def find_str(s: str, char: Union[str, List[str], Tuple[str, ...]]) -> int:
-    """
-    Finds a sequence within a string, and returns the position. If not exists, returns ``-1``.
-
-    :param s: Latex string code
-    :param char: Sequence or List of sequences
-    :return: Position
-    """
-    if isinstance(char, str):
-        return _find_str(s, char)
-    else:
-        for ch in char:
-            j = _find_str(s, ch)
-            if j != -1:
-                return j
-    return -1
-
-
-def remove_tag(s: str, tagname: str) -> str:
-    """
-    Removes a latex tag code.
-
-    :param s: Latex string code
-    :param tagname: Tag code
-    :return: String without tags
-    """
-    tagname = '\\' + tagname
-    tagadd = 1
-    if '{' not in tagname:
-        tagname += '{'
-        tagadd = 0
-    while True:
-        k = find_str(s, tagname)
-        if k == -1:  # No more tags, return
-            return s
-        deep = 0
-        f = False
-        for j in range(len(s)):
-            if s[k + j] == '{':
-                deep += 1
-                f = True
-                continue
-            if s[k + j] == '}':
-                deep -= 1
-            if deep == 0 and f:
-                # update s
-                s = s[:k] + s[k + len(tagname) + tagadd:k + j] + s[k + j + 1:]
-                break
-
-
-def remove_common_tags(
-    s: str,
-    replace_tags: Optional[List] = None,
-    **kwargs
-) -> str:
-    """
-    Remove common tags from string.
-
-    :param s: Latex string code
-    :param replace_tags: List to replace. If ``None``, default will be used
-    :return: Text without tags
-    """
-    if replace_tags is None:
-        replace_tags = [
-            'chapter',
-            'emph',
-            'emph',
-            'hl',
-            'section',
-            'subsection',
-            'subsubsection',
-            'subsubsubsection',
-            'textbf',
-            'textit',
-            'textsuperscript',
-            'texttt'
-        ]
-
-    for tag in replace_tags:
-        s = remove_tag(s, tag)
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing common tags')
-    return s
-
-
-def process_cite(
-    s: str,
-    sort_cites: bool = True,
-    compress_cite: bool = True,
-    cite_separator: str = ', ',
-    **kwargs
-) -> str:
-    """
-    Transforms all cites to a text-based with numbers. For example:
-    ``'This is from \cite{Pizarro}'`` to ``'This is from [1]'``.
-
-    :param s: Latex string code
-    :param sort_cites: Sort the cite numbers
-    :param compress_cite: Compress the cite numbers, ex ``[1, 2, 3, 10]`` to ``[1-3, 10]``
-    :param cite_separator: Separator of cites, for example ``[1{sep}2{sep}3]``
-    :return: Latex with cite as numbers
-    """
-    assert isinstance(cite_separator, str)
-    cites = {}
-    look = ['\\cite*{', '\\citet*{', '\\citep*{', '\\cite{', '\\citet{', '\\citep{', '\\newcite{', '\\newcite*{']
-    k = -1
-    while True:
-        run_j = ''
-        for j in look.copy():
-            k = find_str(s, j)
-            if k == -1:
-                look.remove(j)
-            else:
-                run_j = j
-                break
-        if k == -1:
-            if kwargs.get('pb'):  # Update progressbar
-                kwargs.get('pb').update('Processing cites')
-            return s
-        for j in range(len(s)):
-            if s[k + j] == '}':
-                c = s[k + len(run_j):k + j]
-
-                # Create the number of the cites
-                cite_nums: List[int] = []
-                for w in c.split(','):
-                    w = w.strip()
-                    if w not in cites.keys():
-                        cites[w] = len(cites.keys()) + 1
-                    cite_nums.append(cites[w])
-                    c = c.replace(w, str(cites[w]))
-
-                # Sort the cites
-                if sort_cites:
-                    cite_nums.sort()
-
-                new_cites: List[str] = []
-
-                # Compress
-                if compress_cite:
-                    cont = False  # Cite number continues
-                    prev_c = -1  # Previous cite
-                    compr_range = -1  # First compress
-                    for w in cite_nums:
-                        if w - prev_c != 1 or w == cite_nums[-1]:
-                            if cont:
-                                # Find if the first is present in the list
-                                for m in range(len(new_cites)):
-                                    if new_cites[m] == str(compr_range):
-                                        new_cites.pop(m)
-                                        break
-                                new_cites.append(f'{compr_range}-{w}')
-                            else:
-                                new_cites.append(str(w))
-                            cont = False
-                            compr_range = w
-                        else:
-                            cont = True
-                        prev_c = w
-
-                else:
-                    for w in cite_nums:
-                        new_cites.append(str(w))
-
-                c = cite_separator.join(new_cites)
-                s = s[:k] + FONT_FORMAT_SETTINGS['cite'] + _TAG_OPEN_CITE + c + \
-                    _TAG_CLOSE_CITE + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
-                break
-
-
-def process_citeauthor(
-    s: str,
-    lang: str,
-    **kwargs
-) -> str:
-    """
-    Transforms all citeauthor to [cite]. For example:
-    ``'This is from \citeauthor{Pizarro}, and that is from \citeauthor{cite1, cite2}'`` to
-    ``'This is from [author], and that is from [authors]'``.
-
-    :param s: Latex string code
-    :param lang: Language tag of the code
-    :return: Latex with replaced cites
-    """
-    look = ['\\citeauthor{']
-    k = -1
-    while True:
-        run_j = ''
-        for j in look.copy():
-            k = find_str(s, j)
-            if k == -1:
-                look.remove(j)
-            else:
-                run_j = j
-                break
-        if k == -1:
-            if kwargs.get('pb'):  # Update progressbar
-                kwargs.get('pb').update('Processing citeauthor')
-            return s
-        for j in range(len(s)):
-            if s[k + j] == '}':
-                c = s[k + len(run_j):k + j].split(',')
-
-                # Count the number of cites
-                c = LANG_TT_TAGS.get(lang, 'citeauthor_single' if len(c) == 1 else 'citeauthor_multiple')
-
-                # Write cite
-                s = s[:k] + FONT_FORMAT_SETTINGS['cite'] + _TAG_OPEN_CITE + c + \
-                    _TAG_CLOSE_CITE + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
-                break
-
-
-def replace_pydetex_tags(
-    s: str,
-    cite_format: Tuple[str, str] = ('[', ']'),
-    **kwargs
-) -> str:
-    """
-    Replaces tags to text.
-
-    :param s: Latex string code
-    :param cite_format: Cite format
-    :return: String with no cites
-    """
-    assert len(cite_format) == 2
-    s = s.replace(_TAG_OPEN_CITE, (cite_format[0]))
-    s = s.replace(_TAG_CLOSE_CITE, (cite_format[1]))
-    s = s.replace(_TAG_ITEM_SPACE, ' ')
-    s = s.replace(_TAG_PERCENTAGE_SYMBOL, '%')
-    s = s.replace(_TAG_BRACE_OPEN, '{')
-    s = s.replace(_TAG_BRACE_CLOSE, '}')
-    s = s.replace(_TAG_NEW_LINE, '\n')
-    if kwargs.get('replace_pydetex_tag_dollar_symbol', True):
-        s = s.replace(_TAG_DOLLAR_SYMBOL, '$')
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Replacing pydetex tags')
-    return s
-
-
-def process_labels(s: str, **kwargs) -> str:
-    """
-    Removes labels.
-
-    :param s: Latex string code
-    :return: String with no labels
-    """
-    while True:
-        k = find_str(s, '\\label{')
-        if k == -1:
-            if kwargs.get('pb'):  # Update progressbar
-                kwargs.get('pb').update('Processing labels')
-            return s
-        for j in range(len(s)):
-            if s[k + j] == '}':
-                s = s[:k] + s[k + j + 1:]
-                break
-
-
-def process_ref(s: str, **kwargs) -> str:
-    """
-    Process references, same as cites, replaces by numbers.
-
-    :param s: Latex string code
-    :return: String with numbers instead of references.
-    """
-    look = ['\\ref{', '\\ref*{', '\\autoref{']
-    refs = []
-    k = -1
-    while True:
-        run_j = ''
-        for j in look.copy():
-            k = find_str(s, j)
-            if k == -1:
-                look.remove(j)
-            else:
-                run_j = j
-                break
-        if k == -1:
-            if kwargs.get('pb'):  # Update progressbar
-                kwargs.get('pb').update('Processing references')
-            return s
-        for j in range(len(s)):
-            if s[k + j] == '}':
-                ref_label = s[k + len(run_j):k + j].strip()
-                if ref_label not in refs:
-                    refs.append(ref_label)
-                ref_idx = refs.index(ref_label) + 1
-                s = s[:k] + FONT_FORMAT_SETTINGS['ref'] + str(ref_idx) + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
-                break
-
-
-def remove_comments(s: str, **kwargs) -> str:
-    """
-    Remove comments from text.
-
-    :param s: Latex string code
-    :return: String without comments
-    """
-    newline_symbol = '⇱NEWLINE_SYMBOL_REMOVE_COMMENTS⇲'
-    s = s.replace('  ', ' ')
-    s = s.replace('\\\\', newline_symbol)
-    s = s.replace('\\%', _TAG_PERCENTAGE_SYMBOL)
-    s = s.replace('\\\n', '\n')
-    k = s.split('\n')
-
-    for r in range(len(k)):
-        k[r] = k[r].strip()  # Strips all text
-    line_merge: List[bool] = []
-    for r in range(len(k)):
-        sp = k[r].split('%')
-        k[r] = sp[0]  # Removes all comments from list
-        line_merge.append(len(sp) > 1)
-    line_merge.append(False)
-    line_merge2: List[bool] = line_merge.copy()
-    k.append('')
-    for r in range(len(k)):
-        if line_merge[r] and not line_merge[r + 1] and k[r + 1] != '':
-            line_merge2[r + 1] = True
-    for r in range(len(k)):
-        line_merge[r] = line_merge[r] or line_merge2[r]
-    new_k = []
-    j = 0
-    merged_str = ''
-
-    while True:  # Merge comment lines
-        if not line_merge[j]:
-            if merged_str != '':  # Add current merged str
-                new_k.append(merged_str)
-                merged_str = ''
-            new_k.append(k[j])
-        else:
-            merged_str += k[j]
-        if j == len(k) - 1:
-            break
-        j += 1
-    if merged_str != '':
-        new_k.append(merged_str)
-    k = new_k
-
-    w = []  # Remove duplicates '' lines to single ''
-    last = ''
-    for j in k:
-        if j == '' and j == last:
-            pass
-        else:
-            w.append(j)
-        last = j
-
-    if len(w) > 0 and w[-1] == '':  # Removes last space
-        w.pop()
-    s = '\n'.join(w).strip()
-    s = s.replace(newline_symbol, '\\\\')
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing comments')
-    return s
-
-
-def simple_replace(s: str, **kwargs) -> str:
-    """
-    Replace simple tokens.
-
-    :param s: Latex string code
-    :return: String with replaced items
-    """
-    for w in REPLACE_SYMBOLS_LIBRARY:
-        s = s.replace(w[0], w[1])
-
-    # Replace unique symbols
-    s += ' '
-    invalid_tag = '⇱SYMBOL_REPLACE_TAG_TOKEN⇲'
-    for w in REPLACE_TEX_COMMANDS_LIBRARY:
-        word, repl = w
-        while True:
-            k = s.find(word)
-            if k == -1:
-                break
-            if s[k + len(word)] not in ut.TEX_COMMAND_CHARS:
-                s = s[0:k] + repl + s[k + len(word):]
-            else:
-                s = s[0:k + 1] + invalid_tag + s[k + 1:]  # format ...\\INVALID_TAG...
-    s = s[0:len(s) - 1].replace(invalid_tag, '')
-
-    # Replace equation symbols
-    s = s.replace('\$', _TAG_DOLLAR_SYMBOL)
-    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
-    new_s = ''
-    k = 0  # Moves through tags
-    added_s = False
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][1]:
-                new_s += s[i]
-            elif tex_tags[k][1] <= i < tex_tags[k][2] and not added_s or tex_tags[k][1] == i == tex_tags[k][2]:
-                if not added_s:
-                    k_s: str = s[tex_tags[k][1]:tex_tags[k][2] + 1]
-                    # Replace
-                    for j in REPLACE_EQUATION_SYMBOLS_LIBRARY:
-                        k_s = k_s.replace(j[0], j[1])
-                    new_s += k_s
-                added_s = True
-            elif tex_tags[k][2] < i < tex_tags[k][3]:
-                new_s += s[i]
-            elif i == tex_tags[k][3]:  # Advance to other tag
-                new_s += s[i]
-                k += 1
-                added_s = False
-        else:
-            new_s += s[i]
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Replacing simple tokens')
-    return new_s
-
-
-def _load_file_search(tex_file: str, print_error: bool = False) -> str:
-    """
-    Search and load a file.
-
-    :param tex_file: Name of the file
-    :param print_error: Prints if file not found
-    :return: Loaded file or tag error
-    """
-    tx = _TAG_FILE_ERROR
-    folders = _os_listfolder()
-    folders.insert(0, '../')
-    folders.insert(0, './')
-    for f in folders:
-        tx = _load_file(tex_file, f)
-        if tx == _TAG_FILE_ERROR:
-            if print_error:
-                print(f'\tFile not found in {f}')
-        else:
-            break
-    return tx
-
-
-def process_inputs(
-    s: str,
-    clear_not_found_files: bool = False,
-    **kwargs
-) -> str:
-    """
-    Process inputs, which find the input files and retrieve its contents.
-
-    :param s: Latex string code with inputs
-    :param clear_not_found_files: Clear the not found files. Used when changing the path
-    :return: Text copied with data from inputs
-    """
-    global _PRINT_LOCATION, _NOT_FOUND_FILES
-    if os.getcwd() != _LAST_NOT_FOUND_FILES_PATH[0] or clear_not_found_files:
-        _LAST_NOT_FOUND_FILES_PATH[0] = os.getcwd()
-        _NOT_FOUND_FILES.clear()
-        _PRINT_LOCATION = False
-    print_ = kwargs.get('print', True)
-    symbol = '⇱INPUT_FILE_TAG⇲'
-    s = remove_comments(s)
-    while True:
-        k = find_str(s, '\\input{')
-        if k == -1:
-            if kwargs.get('pb'):  # Update progressbar
-                kwargs.get('pb').update('Processing \\input')
-            return s.replace(symbol, '\\input{')
-        m = 0
-        for j in range(len(s)):
-            if s[k + j] == '{':
-                m = j
-            if s[k + j] == '}':
-                tex_file = s[k + m + 1:k + j]
-                if '.tex' not in tex_file:
-                    tex_file += '.tex'
-                if tex_file not in _NOT_FOUND_FILES and '\jobname' not in tex_file:
-                    if not _PRINT_LOCATION:
-                        if print_:
-                            print(f'Current path location:\n\t{os.getcwd()}')
-                        _PRINT_LOCATION = True
-                    if print_:
-                        print(f'Detected file {tex_file}:')
-                    tx = _load_file_search(tex_file, print_error=print_)
-                    if tx == _TAG_FILE_ERROR:
-                        _NOT_FOUND_FILES.append(tex_file)
-                        s = s[:k] + symbol + s[k + m + 1:]
-                    else:
-                        if print_:
-                            print('\tFile found and loaded')
-                        tx = '\n'.join(tx.splitlines())
-                        tx = remove_comments(tx)
-                        s = s[:k] + tx + s[k + j + 1:]
-                else:
-                    s = s[:k] + symbol + s[k + m + 1:]
-                break
-
-
-def remove_commands_char(s: str, chars: List[Tuple[str, str, bool]]) -> str:
-    """
-    Remove all char commands.
-
-    :param s: Latex string code
-    :param chars: Char that define equations [(initial, final, ignore escape), ...]
-    :return: Code with removed chars
-    """
-    tex_tags = ut.find_tex_command_char(s, symbols_char=chars)
-    if len(tex_tags) == 0:
-        return s
-    new_s = ''
-    k = 0  # Moves through tags
-
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][0]:
-                new_s += s[i]
-            # elif tex_tags[k][0] <= i < tex_tags[k][3]:
-            #     pass
-            elif i == tex_tags[k][3]:  # Advance to other tag
-                k += 1
-        else:
-            new_s += s[i]
-
-    return new_s
-
-
-def remove_equations(s: str, **kwargs) -> str:
-    """
-    Remove all equations from a string.
-
-    :param s: Latex string code
-    :return: Latex without equation
-    """
-    s = remove_commands_char(s, chars=ut.TEX_EQUATION_CHARS)
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing equations')
-    return s
-
-
-def output_text_for_some_commands(
-    s: str,
-    lang: str
-) -> str:
-    """
-    Replaces the command for a particular text.
-
-    :param s: Latex string code
-    :param lang: Language tag of the code
-    :return: Text string or empty if error
-    """
-    # Stores the commands to be transformed
-    # (
-    #   command name,
-    #   [(argument number, argument is optional), ...],
-    #   tag to be replaced,
-    #   total commands,
-    #   font_tag ('tex_text_tag' if None),
-    #   font_content ('tex_text_tag_content' if None),
-    #   add new line (before, after)
-    # )
-    # The font format is like .... [font tag]YOUR TAG {[font content]YOUR CONTENT} ...[font normal]. In that case, tag to be
-    # relaced is 'YOUR TAG {0}, {1}
-    # All *arguments will be formatted using the tag
-    commands: List[Tuple[str, List[Tuple[int, bool]], Union[str, Callable[[str, ...], str]], int, Optional[str], Optional[str], Tuple[bool, bool]]] = [
-        ('ac', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
-        ('acf', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
-        ('acl', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
-        ('acs', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
-        ('caption', [(1, False)], LANG_TT_TAGS.get(lang, 'caption'), 1, None, None, (False, True)),
-        ('chapter', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('chapter*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('doublequotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
-        ('em', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
-        ('emph', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
-        ('enquote', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
-        ('href', [(2, False)], LANG_TT_TAGS.get(lang, 'link'), 2, None, None, (False, False)),
-        ('insertimage', [(3, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 3, None, None, (False, True)),  # (Template) Informe
-        ('insertimage', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, False)),  # (Template) Informe
-        ('insertimageboxed', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, True)),  # (Template) Informe
-        ('insertimageboxed', [(5, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 5, None, None, (False, True)),  # (Template) Informe
-        ('institutionentry', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
-        ('institutionentryshort', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
-        ('lowercase', [(1, False)], lambda t: t.lower(), 1, 'normal', 'normal', (False, False)),
-        ('MakeLowercase', [(1, False)], lambda t: t.lower(), 1, 'normal', 'normal', (False, False)),
-        ('MakeUppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False)),
-        ('otherentry', [(1, False), (2, False)], '{0} {1}', 2, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
-        ('paragraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('quotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
-        ('section', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('section*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subfloat', [(1, True)], LANG_TT_TAGS.get(lang, 'sub_figure_title'), 1, None, None, (False, True)),
-        ('subparagraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsubsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('subsubsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
-        ('textbf', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
-        ('textit', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
-        ('texttt', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),
-        ('uppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False))
-    ]
-    new_s = ''
-
-    # Get the commands
-    cmd_args = ut.get_tex_commands_args(s)
-    for c in cmd_args:
-        for cmd in commands:
-            if c[0] == cmd[0]:
-                _, cmd_args, cmd_tag, total_commands, font_tag, font_content, cmd_newline = cmd
-                if font_tag is None:
-                    font_tag = 'tex_text_tag'
-                if font_content is None:
-                    font_content = 'tex_text_tag_content'
-                if len(c) - 1 == total_commands:
-                    args = []
-                    for j in cmd_args:
-                        cmd_argnum, cmd_is_optional = j
-                        if len(c) - 1 >= j[0] >= 0 and c[cmd_argnum][1] == cmd_is_optional:
-                            argv = c[cmd_argnum][0].replace('\n', ' ')  # Command's argument to process
-                            argv = remove_commands_param(argv, lang)  # Remove commands within the argument
-                            argv = argv.strip()
-                            if argv != '':
-                                args.append(argv)
-                    if len(args) == len(cmd_args):
-                        # Add format text
-                        for a in range(len(args)):
-                            args[a] = FONT_FORMAT_SETTINGS[font_content] + args[a] + FONT_FORMAT_SETTINGS[font_tag]
-                        if callable(cmd_tag):
-                            text = cmd_tag(*args)
-                        else:
-                            try:
-                                text = cmd_tag.format(*args)
-                            except IndexError:
-                                text = cmd_tag
-                        text = FONT_FORMAT_SETTINGS[font_tag] + text + FONT_FORMAT_SETTINGS['normal']
-                        if cmd_newline[0]:
-                            text = _TAG_NEW_LINE + text
-                        new_s += text
-                        if cmd_newline[1]:
-                            new_s += _TAG_NEW_LINE
-                        break
-
-    return new_s.strip()
-
-
-def remove_environments(
-    s: str,
-    env_list: Optional[List[str]] = None,
-    **kwargs
-) -> str:
-    """
-    Remove a selection of environments.
-
-    :param s: Latex code
-    :param env_list: Environment list, if not defined, use the default from PyDetex
-    :return: Code without given environments
-    """
-    if not env_list:
-        env_list = [
-            'lstlisting',
-            'references',
-            'minted',
-            'sourcecode',
-            'tabular',
-            'thebibiliography',
-            'tikzpicture',
-            'verbatim'
-        ]
-    tex_tags = ut.find_tex_environments(s)
-    if len(tex_tags) == 0 or len(env_list) == 0:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No environment found in code')
-        return s
-    new_s = ''
-
-    new_tex_tags = []
-    # Remove all the environments not in env_list
-    for t in tex_tags:
-        is_removed = False
-        for j in env_list:
-            if j in t[0]:
-                is_removed = True
-                break
-        if is_removed:
-            new_tex_tags.append(t)
-
-    # If tex tags is empty
-    if len(new_tex_tags) == 0:
-        return s
-
-    def is_in_tags(v: int) -> bool:
-        """
-        Check if a position is within tags.
-
-        :param v: Position
-        :return: True if in tags range
-        """
-        for j_ in new_tex_tags:
-            if j_[1] <= v <= j_[4] + 1:
-                return True
-        return False
-
-    for i in range(len(s)):
-        if not is_in_tags(i):
-            new_s += s[i]
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing environments')
-    return new_s
-
-
-def remove_commands_param(
-    s: str,
-    lang: str,
-    invalid_commands: Optional[List[str]] = None,
-    **kwargs
-) -> str:
-    """
-    Remove all commands with params.
-
-    :param s: Latex string code
-    :param lang: Language tag of the code
-    :param invalid_commands: Invalid commands that will not call output_text_for_some_commands. If ``None`` use defaults
-    :return: Code with removed chars
-    """
-    tex_tags = ut.find_tex_commands(s)
-    if len(tex_tags) == 0:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No parameter commands found in code')
-        return s
-    new_s = ''
-    k = 0  # Moves through tags
-
-    # invalid commands that will not call output_text_for_some_commands
-    if not invalid_commands:
-        invalid_commands = [
-            'DeclareUnicodeCharacter',
-            'ifthenelse',
-            'newcommand',
-            'newenvironment',
-            'usepackage'
-        ]
-
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][0]:
-                new_s += s[i]
-            elif i < tex_tags[k][3] + 1:
-                pass
-            else:  # Advance to other tag
-                sub_s = s[tex_tags[k][0]:tex_tags[k][3] + 2]
-
-                # If the command does not continue, write the text for such
-                # command, if this does not continue (for example, that happens
-                # when calling for \mycommand{1}{2}{3}). In that case, only tex_tags
-                # [\mycommand .... {3}] will be called, thus, sub_s will contain
-                # all the parameters of the command ({1}{2}{3})
-                if not tex_tags[k][4]:
-                    cmd_name = s[tex_tags[k][0]:tex_tags[k][1] + 1].strip()
-
-                    # Check if the invalid_commands are not within command name
-                    is_invalid = False
-                    for c in invalid_commands:
-                        if c in cmd_name:
-                            is_invalid = True
-                            break
-
-                    # If not invalid, call the analysis for its commands, check that
-                    # it can be recursive
-                    if not is_invalid:
-                        new_s += output_text_for_some_commands(sub_s, lang)
-                k += 1
-        else:
-            new_s += s[i]
-
-    # Replace all command symbols
-    parenthesis_open_symbol = '⇱PARENTHESIS_OPEN_SYMBOL⇲'
-    parenthesis_close_symbol = '⇱PARENTHESIS_CLOSE_SYMBOL⇲'
-    parenthesis_sq_open_symbol = '⇱PARENTHESIS_SQ_OPEN_SYMBOL⇲'
-    parenthesis_sq_close_symbol = '⇱PARENTHESIS_SQ_CLOSE_SYMBOL⇲'
-    new_s = new_s.replace('\\{', parenthesis_open_symbol)
-    new_s = new_s.replace('\\}', parenthesis_close_symbol)
-    new_s = new_s.replace('\\[', parenthesis_sq_open_symbol)
-    new_s = new_s.replace('\\]', parenthesis_sq_close_symbol)
-    new_s = new_s.replace('{', '').replace('}', '')  # .replace('[', '').replace(']', '')
-    new_s = new_s.replace(parenthesis_open_symbol, '\\{')
-    new_s = new_s.replace(parenthesis_close_symbol, '\\}')
-    new_s = new_s.replace(parenthesis_sq_open_symbol, '\\[')
-    new_s = new_s.replace(parenthesis_sq_close_symbol, '\\]')
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing command with parameters')
-    return new_s
-
-
-def remove_commands_param_noargv(s: str, **kwargs) -> str:
-    """
-    Remove all commands without arguments.
-
-    :param s: Latex string code
-    :return: Code with removed chars
-    """
-    tex_tags = ut.find_tex_commands_noargv(s)
-    if len(tex_tags) == 0:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No command without arguments were found in code')
-        return s
-    new_s = ''
-    k = 0  # Moves through tags
-
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][0]:
-                new_s += s[i]
-            elif i < tex_tags[k][1]:
-                pass
-            else:  # Advance to other tag
-                k += 1
-        else:
-            new_s += s[i]
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Removing command without arguments')
-    return new_s
-
-
-def unicode_chars_equations(s: str, **kwargs) -> str:
-    """
-    Converts all equations to unicode.
-
-    :param s: Latex string code
-    :return: Latex with unicode converted
-    """
-    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
-    new_s = ''
-    k = 0  # Moves through tags
-    added_s = False
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][1]:
-                new_s += s[i]
-            elif tex_tags[k][1] <= i < tex_tags[k][2] and not added_s or tex_tags[k][1] == i == tex_tags[k][2]:
-                if not added_s:
-                    k_s: str = s[tex_tags[k][1]:tex_tags[k][2] + 1]
-                    k_s_tex = ut.tex_to_unicode(k_s)
-                    k_s_tex = k_s_tex.replace('\{', _TAG_BRACE_OPEN).replace('\}', _TAG_BRACE_CLOSE)
-                    new_s += k_s_tex
-                added_s = True
-            elif tex_tags[k][2] < i < tex_tags[k][3]:
-                new_s += s[i]
-            elif i == tex_tags[k][3]:  # Advance to other tag
-                new_s += s[i]
-                k += 1
-                added_s = False
-        else:
-            new_s += s[i]
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Processing unicode equations')
-    return new_s
-
-
-def process_chars_equations(
-    s: str,
-    lang: str,
-    single_only: bool,
-    **kwargs
-) -> str:
-    """
-    Process single char equations, removing the symbols.
-
-    :param s: Latex string code
-    :param lang: Language tag of the code
-    :param single_only: Only process single char equations. If False, replaces the equation by a text-label
-    :return: Code without symbols
-    """
-    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
-    if len(tex_tags) == 0:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No char equtions found')
-        return s
-
-    new_s = ''
-    k = 0  # Moves through tags
-    eqn_number = 0
-    added_equ = False
-
-    for i in range(len(s)):
-        if k < len(tex_tags):
-            if i < tex_tags[k][0]:
-                new_s += s[i]
-            # elif tex_tags[k][0] <= i < tex_tags[k][1]:
-            #     continue
-            elif tex_tags[k][1] <= i <= tex_tags[k][2] and not added_equ:
-                equ = s[tex_tags[k][1]:tex_tags[k][2] + 1]
-                if len(equ) == 1:
-                    new_s += FONT_FORMAT_SETTINGS['equation'] + s[i] + FONT_FORMAT_SETTINGS['normal']
-                else:
-                    equ = s[tex_tags[k][0]:tex_tags[k][3] + 1]
-                    if not single_only:
-                        new_s += FONT_FORMAT_SETTINGS['equation'] + \
-                                 LANG_TT_TAGS.get(lang, 'multi_char_equ').format(eqn_number) + \
-                                 FONT_FORMAT_SETTINGS['normal']
-                        eqn_number += 1
-                    else:
-                        new_s += equ
-                added_equ = True
-            # elif tex_tags[k][2] < i < tex_tags[k][3]:
-            #     continue
-            elif tex_tags[k][3] == i:
-                k += 1
-                added_equ = False
-                continue
-        else:
-            new_s += s[i]
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Processing char equations')
-    return new_s
-
-
-def strip_punctuation(s: str, **kwargs) -> str:
-    """
-    Strips punctuation. For example, ``'mycode :'`` to ``'mycode:'``.
-
-    :param s: Latex string code
-    :return: Stripped punctuation
-    """
-    for j in [',', ':', '=', ';', '!', '?', '.']:  # Before
-        s = s.replace(f' {j}', j)
-    s = s.replace('\n\n\n', '\n\n')
-    s = s.strip()
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Stripping punctuation')
-    return s
-
-
-def process_def(
-    s: str,
-    clear_learned: bool = True,
-    replace: bool = False,
-    **kwargs
-) -> str:
-    """
-    Process \defs. Store the definition, among others.
-
-    :param s: Latex with definitions
-    :param clear_learned: Clear the last learned definitions
-    :param replace: Replace instances of learned defs
-    :return: Latex without definitions
-    """
-    if '\\def' not in s:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No definitions found in code')
-        return s
-    if clear_learned:
-        _DEFS.clear()
-    s += '    '
-    new_s = ''
-    found_def = False
-    a, b, c, depth = 0, 0, -1, -1  # Def positions (a\def      b{ .... c}
-    def_ranges = []
-    for i in range(len(s) - 4):
-        # After finding a def, check the first and last parenthesis
-        if s[i:i + 4] == '\\def' and s[i + 4] not in ut.TEX_COMMAND_CHARS:
-            a, b, depth = i, -1, 0
-            found_def = True
-            continue
-        elif found_def:
-            if found_def and s[i] == '{' and s[i - 1] != '\\':
-                if depth == 0:
-                    b = i
-                depth += 1
-            if found_def and s[i] == '}' and s[i - 1] != '\\':
-                depth -= 1
-                if depth == 0:
-                    c = i
-                    def_ranges.append((a, c))
-
-                    # Check the name, if not a command, store
-                    def_name = s[a + 4:b].strip()
-                    if '#' not in def_name:
-                        _DEFS[def_name] = remove_common_tags(s[b + 1:c])
-                    found_def = False
-            continue
-
-        else:
-            new_s += s[i]
-
-    # Now, if replace defs is enabled, check all non-arg commands and replace if
-    # known
-    if replace:
-        new_s_def = ''
-        st = ut.find_tex_commands_noargv(new_s)
-        w = 0  # Iterates through st
-        k = 0
-        if len(st) > 0:
-            for _ in range(len(new_s)):
-                if k < len(new_s):
-                    if k < st[w][0]:
-                        new_s_def += new_s[k]
-                    else:
-                        a, b = st[w]
-                        def_n = new_s[a:b + 1]
-                        if def_n in _DEFS.keys():
-                            new_s_def += _DEFS[def_n]
-                        else:
-                            new_s_def += new_s[a:b + 1]
-                        k += b - a
-                        w += 1
-                        if w == len(st):
-                            new_s_def += new_s[k + 1:]
-                            break
-                k += 1
-            new_s = new_s_def
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Processing definitions')
-
-    return new_s
-
-
-def process_items(s: str, lang: str, **kwargs) -> str:
-    """
-    Process itemize and enumerate.
-
-    :param s: Latex string code
-    :param lang: Language tag
-    :return: Processed items
-    """
-    if not ('itemize' in s or 'enumerate' in s or 'tablenotes' in s):
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No item found')
-        return s
-
-    def _get_name(e: str) -> str:
-        """
-        Get the environment name.
-
-        :param e: Environment name
-        :return: New name
-        """
-        # This is due to itemize can contain other symbols or spaces, thus,
-        # itemize*    .. is converted to itemize
-        if 'itemize' in e:
-            return 'itemize'
-        if 'enumerate' in e:
-            return 'enumerate'
-        if 'tablenotes' in e:
-            return 'tablenotes'
-        return ''
-
-    def _are_item(e: str) -> bool:
-        """
-        Return true if both are enumerated. Used to check recursive enumerates.
-
-        :param e: Environment name
-        :return: True if item
-        """
-        return e == 'itemize' or e == 'enumerate' or e == 'tablenotes'
-
-    # First, process the nested ones
-    while True:
-        equal = False
-        envs = ut.find_tex_environments(s)
-        for tag in envs:
-            t, a, b, c, d, t2, _, item_depth = tag
-            t, t2 = _get_name(t), _get_name(t2)
-            if t == '' or t2 == '':
-                continue
-            if t == t2 or _are_item(t) and _are_item(t2):
-                s = s[0:a] + _process_item(s[b:c].strip(), t, item_depth) + s[d + 2:]
-                equal = True
-                break
-        if not equal:
-            break
-
-    # Not nested
-    while True:
-        conv = False
-        envs = ut.find_tex_environments(s)
-        for tag in envs:
-            t, a, b, c, d, _, _, _ = tag
-            t = _get_name(t)
-            if t == '':
-                continue
-            s = s[0:a] + remove_commands_param(_process_item(s[b:c].strip(), t), lang) + s[d + 2:]
-            conv = True
-            break
-        if not conv:
-            break
-
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Processing item/enumerate environments')
-    return s
-
-
-def _process_item(s: str, t: str, depth: int = 0) -> str:
-    """
-    Process the items.
-
-    :param s: Latex string code
-    :param t: Type (enumerate, itemize)
-    :param depth: Depth
-    :return: Processed items
-    """
-    if len(s) == 0:
-        return ''
-    line = '\n' + _TAG_ITEM_SPACE * (3 * depth)
-
-    def _num(x: int) -> str:
-        """
-        Get number based on the depth.
-
-        :param x: Number
-        :return: Number format by depth
-        """
-        if depth % 5 == 0:
-            return f'{line}{x}. '
-        elif depth % 5 == 1:
-            x = _int_to_alph(x).lower()
-            return f'{line}{x}) '
-        elif depth % 5 == 2:
-            x = _int_to_roman(x).lower()
-            return f'{line}{x}. '
-        elif depth % 5 == 3:
-            x = _int_to_alph(x).upper()
-            return f'{line}{x}) '
-        elif depth % 5 == 4:
-            x = _int_to_roman(x).upper()
-            return f'{line}{x}. '
-
-    def _itm() -> str:
-        """
-        :return: The item string based on depth.
-        """
-        char = ['-', '•', '◦', '■', '*']
-        x = char[depth % 5]
-        return f'{line}{x} '
-
-    # Remove optional arguments list
-    if s[0] == '[':
-        sqd = 1
-        for j in range(1, len(s)):
-            if s[j] == '[':
-                sqd += 1
-            elif s[j] == ']':
-                sqd -= 1
-            if sqd == 0:
-                s = s[j + 1:len(s)].strip()
-                break
-
-    # Remove invalid newlines
-    s_ = []
-    for v in s.split('\n'):
-        v = v.strip()
-        if v != '':
-            s_.append(v)
-    s_ = '\n'.join(s_)
-    s = s_
-
-    if t == 'enumerate':
-        s += ' ' * 5
-        new_s = ''
-        k = 1
-        j = -1
-        while True:
-            j += 1
-            if s[j:j + 5] == '\\item':
-                new_s += _num(k)
-                j += 5
-                k += 1
-            else:
-                new_s += s[j]
-            if j == len(s) - 5:
-                break
-    else:
-        new_s = s.replace('\\item', _itm())
-
-    # Last operations
-    new_s = new_s.replace('\n\n', '\n').strip(' ')
-    return new_s
-
-
-def _int_to_roman(number: int) -> str:
-    """
-    Convert an arabic integer number to a roman.
-
-    :param number: Number
-    :return: Number in roman
-    """
-    result = ''
-    for (arabic, roman) in _ROMAN_DIGITS:
-        (factor, number) = divmod(number, arabic)
-        result += roman * factor
-    return result
-
-
-def _int_to_alph(n: int) -> str:
-    """
-    Integer to a..z.
-
-    :param n: Number
-    :return: Number in AABB..
-    """
-    string = ''
-    while n > 0:
-        n, remainder = divmod(n - 1, 26)
-        string = chr(65 + remainder) + string
-    return string
-
-
-def process_begin_document(s: str, **kwargs) -> str:
-    """
-    Removes all code outside begin document, if found.
-
-    :param s: Latex code
-    :return: Removes all data outside the document
-    """
-    if '{document}' not in s:
-        if kwargs.get('pb'):  # Update progressbar
-            kwargs.get('pb').update('No document environment found')
-        return s
-
-    s += '          '
-    is_env = False
-    is_end = False
-    is_document_begin = False
-    i, j, w = -1, -1, -1  # Init and start of "begin document", w indicates the start of \end
-    # Find if begin document exists
-    for k in range(len(s) - 10):
-        if s[k:k + 6] == '\\begin':
-            is_env = True
-        elif s[k] == '{' and s[k - 1] != '\\' and is_env and not is_document_begin:
-            if s[k:k + 10] == '{document}':
-                is_document_begin = True
-                i = k + 10
-            else:
-                is_env = False
-        elif is_document_begin and s[k:k + 4] == '\\end':
-            is_end = True
-            w = k
-        elif is_document_begin and is_end and s[k] == '{' and s[k - 1] != '\\':
-            if s[k:k + 10] == '{document}':
-                break
-
-    # If document has been found
-    if kwargs.get('pb'):  # Update progressbar
-        kwargs.get('pb').update('Processing {document} environment')
-    if -1 < i <= w:
-        return s[i:w]
-    return s[0:len(s) - 10]
+"""
+PyDetex
+https://github.com/ppizarror/PyDetex
+
+PARSERS
+Defines parsers, which perform a single task for removal LaTex things.
+"""
+
+__all__ = [
+    'find_str',
+    'FONT_FORMAT_SETTINGS',
+    'process_begin_document',
+    'process_chars_equations',
+    'process_cite',
+    'process_citeauthor',
+    'process_def',
+    'process_inputs',
+    'process_items',
+    'process_labels',
+    'process_ref',
+    'remove_commands_char',
+    'remove_commands_param',
+    'remove_commands_param_noargv',
+    'remove_comments',
+    'remove_common_tags',
+    'remove_environments',
+    'remove_equations',
+    'remove_tag',
+    'replace_pydetex_tags',
+    'simple_replace',
+    'strip_punctuation',
+    'unicode_chars_equations'
+]
+
+import os
+import pydetex.utils as ut
+
+from pydetex._symbols import *
+from typing import List, Tuple, Union, Optional, Callable
+
+# Files
+_LAST_NOT_FOUND_FILES_PATH = [os.getcwd()]
+_NOT_FOUND_FILES = []
+_PRINT_LOCATION = False
+
+# Tags
+_TAG_BRACE_CLOSE = '⇱BRACE_CLOSE⇲'
+_TAG_BRACE_OPEN = '⇱BRACE_OPEN⇲'
+_TAG_CLOSE_CITE = '⇱CLOSE_CITE⇲'
+_TAG_CLOSE_CITE_EQN = '⇱CLOSE_CITE_EQN⇲'
+_TAG_DOLLAR_SYMBOL = '⇱DOLLAR_SYMBOL⇲'
+_TAG_FILE_ERROR = '⇱FILE_ERROR⇲'
+_TAG_ITEM_SPACE = '⇱ITEM_SPACE⇲'
+_TAG_NEW_LINE = '⇱NEW_LINE⇲'
+_TAG_OPEN_CITE = '⇱OPEN_CITE⇲'
+_TAG_OPEN_CITE_EQN = '⇱OPEN_CITE_EQN⇲'
+_TAG_PERCENTAGE_SYMBOL = '⇱COMMENT_PERCENTAGE_SYMBOL⇲'
+
+# Others
+_ROMAN_DIGITS = [
+    (1000, 'M'),
+    (900, 'CM'),
+    (500, 'D'),
+    (400, 'CD'),
+    (100, 'C'),
+    (90, 'XC'),
+    (50, 'L'),
+    (40, 'XL'),
+    (10, 'X'),
+    (9, 'IX'),
+    (5, 'V'),
+    (4, 'IV'),
+    (1, 'I')
+]
+
+# Stores the learned definitions
+_DEFS = {}
+
+# Parser font format. This dict stores the font of some tex elements to be represented
+# in the GUI text editor. The values are the same of _fonts.FONT_TAGS. By default,
+# they are empty, and are updated in the PyDetexGUI._process() method
+FONT_FORMAT_SETTINGS = {
+    'bold': '',
+    'cite': '',
+    'equation': '',
+    'italic': '',
+    'normal': '',
+    'ref': '',
+    'tex_text_tag': '',
+    'tex_text_tag_content': ''
+}
+
+LANG_TT_TAGS = ut.LangTexTextTags()
+
+
+def _find_str(s: str, char: str) -> int:
+    """
+    Finds a sequence within a string, and returns the position. If not exists, returns ``-1``.
+
+    :param s: Latex string code
+    :param char: Sequence
+    :return: Position
+    """
+    index = 0
+
+    if char in s:
+        c = char[0]
+        for ch in s:
+            if ch == c:
+                if s[index:index + len(char)] == char:
+                    return index
+
+            index += 1
+
+    return -1
+
+
+def _os_listfolder() -> List[str]:
+    """
+    Returns the folders from the current path.
+
+    :return: Folder list
+    """
+    dirs = os.listdir('./')
+    folders = []
+    for k in dirs:
+        if os.path.isdir(k):
+            folders.append(k + '/')
+    return folders
+
+
+def _load_file(f: str, path: str) -> str:
+    """
+    Try to load a file.
+
+    :param f: Filename
+    :param path: Path to look from
+    :return: File contents
+    """
+    try:
+        return ut.open_file(path + f)
+    except FileNotFoundError:
+        return _TAG_FILE_ERROR
+
+
+def find_str(s: str, char: Union[str, List[str], Tuple[str, ...]]) -> int:
+    """
+    Finds a sequence within a string, and returns the position. If not exists, returns ``-1``.
+
+    :param s: Latex string code
+    :param char: Sequence or List of sequences
+    :return: Position
+    """
+    if isinstance(char, str):
+        return _find_str(s, char)
+    else:
+        for ch in char:
+            j = _find_str(s, ch)
+            if j != -1:
+                return j
+    return -1
+
+
+def remove_tag(s: str, tagname: str) -> str:
+    """
+    Removes a latex tag code.
+
+    :param s: Latex string code
+    :param tagname: Tag code
+    :return: String without tags
+    """
+    tagname = '\\' + tagname
+    tagadd = 1
+    if '{' not in tagname:
+        tagname += '{'
+        tagadd = 0
+    while True:
+        k = find_str(s, tagname)
+        if k == -1:  # No more tags, return
+            return s
+        deep = 0
+        f = False
+        for j in range(len(s)):
+            if s[k + j] == '{':
+                deep += 1
+                f = True
+                continue
+            if s[k + j] == '}':
+                deep -= 1
+            if deep == 0 and f:
+                # update s
+                s = s[:k] + s[k + len(tagname) + tagadd:k + j] + s[k + j + 1:]
+                break
+
+
+def remove_common_tags(
+    s: str,
+    replace_tags: Optional[List] = None,
+    **kwargs
+) -> str:
+    """
+    Remove common tags from string.
+
+    :param s: Latex string code
+    :param replace_tags: List to replace. If ``None``, default will be used
+    :return: Text without tags
+    """
+    if replace_tags is None:
+        replace_tags = [
+            'chapter',
+            'emph',
+            'emph',
+            'hl',
+            'section',
+            'subsection',
+            'subsubsection',
+            'subsubsubsection',
+            'textbf',
+            'textit',
+            'textsuperscript',
+            'texttt'
+        ]
+
+    for tag in replace_tags:
+        s = remove_tag(s, tag)
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing common tags')
+    return s
+
+
+def process_cite(
+    s: str,
+    sort_cites: bool = True,
+    compress_cite: bool = True,
+    cite_separator: str = ', ',
+    **kwargs
+) -> str:
+    """
+    Transforms all cites to a text-based with numbers. For example:
+    ``'This is from \cite{Pizarro}'`` to ``'This is from [1]'``.
+
+    :param s: Latex string code
+    :param sort_cites: Sort the cite numbers
+    :param compress_cite: Compress the cite numbers, ex ``[1, 2, 3, 10]`` to ``[1-3, 10]``
+    :param cite_separator: Separator of cites, for example ``[1{sep}2{sep}3]``
+    :return: Latex with cite as numbers
+    """
+    assert isinstance(cite_separator, str)
+    cites = {}
+    look = ['\\cite*{', '\\citet*{', '\\citep*{', '\\cite{', '\\citet{', '\\citep{',
+            '\\newcite{', '\\newcite*{']
+    look_eqn = ['\\eqref{']
+    look += look_eqn
+    k = -1
+    while True:
+        run_j = ''
+        for j in look.copy():
+            k = find_str(s, j)
+            if k == -1:
+                look.remove(j)
+            else:
+                run_j = j
+                break
+        if k == -1:
+            if kwargs.get('pb'):  # Update progressbar
+                kwargs.get('pb').update('Processing cites')
+            return s
+        for j in range(len(s)):
+            if s[k + j] == '}':
+                c = s[k + len(run_j):k + j]
+
+                # Create the number of the cites
+                cite_nums: List[int] = []
+                for w in c.split(','):
+                    w = w.strip()
+                    if w not in cites.keys():
+                        cites[w] = len(cites.keys()) + 1
+                    cite_nums.append(cites[w])
+                    c = c.replace(w, str(cites[w]))
+
+                # Sort the cites
+                if sort_cites:
+                    cite_nums.sort()
+
+                new_cites: List[str] = []
+
+                # Compress
+                if compress_cite:
+                    cont = False  # Cite number continues
+                    prev_c = -1  # Previous cite
+                    compr_range = -1  # First compress
+                    for w in cite_nums:
+                        if w - prev_c != 1 or w == cite_nums[-1]:
+                            if cont:
+                                # Find if the first is present in the list
+                                for m in range(len(new_cites)):
+                                    if new_cites[m] == str(compr_range):
+                                        new_cites.pop(m)
+                                        break
+                                new_cites.append(f'{compr_range}-{w}')
+                            else:
+                                new_cites.append(str(w))
+                            cont = False
+                            compr_range = w
+                        else:
+                            cont = True
+                        prev_c = w
+
+                else:
+                    for w in cite_nums:
+                        new_cites.append(str(w))
+
+                c = cite_separator.join(new_cites)
+                eqn_mode = run_j in look_eqn
+                open_cite = _TAG_OPEN_CITE if not eqn_mode else _TAG_OPEN_CITE_EQN
+                close_cite = _TAG_CLOSE_CITE if not eqn_mode else _TAG_CLOSE_CITE_EQN
+                s = s[:k] + FONT_FORMAT_SETTINGS['cite'] + open_cite + c + \
+                    close_cite + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
+                break
+
+
+def process_citeauthor(
+    s: str,
+    lang: str,
+    **kwargs
+) -> str:
+    """
+    Transforms all citeauthor to [cite]. For example:
+    ``'This is from \citeauthor{Pizarro}, and that is from \citeauthor{cite1, cite2}'`` to
+    ``'This is from [author], and that is from [authors]'``.
+
+    :param s: Latex string code
+    :param lang: Language tag of the code
+    :return: Latex with replaced cites
+    """
+    look = ['\\citeauthor{']
+    k = -1
+    while True:
+        run_j = ''
+        for j in look.copy():
+            k = find_str(s, j)
+            if k == -1:
+                look.remove(j)
+            else:
+                run_j = j
+                break
+        if k == -1:
+            if kwargs.get('pb'):  # Update progressbar
+                kwargs.get('pb').update('Processing citeauthor')
+            return s
+        for j in range(len(s)):
+            if s[k + j] == '}':
+                c = s[k + len(run_j):k + j].split(',')
+
+                # Count the number of cites
+                c = LANG_TT_TAGS.get(lang, 'citeauthor_single' if len(c) == 1 else 'citeauthor_multiple')
+
+                # Write cite
+                s = s[:k] + FONT_FORMAT_SETTINGS['cite'] + _TAG_OPEN_CITE + c + \
+                    _TAG_CLOSE_CITE + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
+                break
+
+
+def replace_pydetex_tags(
+    s: str,
+    cite_format: Tuple[str, str] = ('[', ']'),
+    **kwargs
+) -> str:
+    """
+    Replaces tags to text.
+
+    :param s: Latex string code
+    :param cite_format: Cite format
+    :return: String with no cites
+    """
+    assert len(cite_format) == 2
+    s = s.replace(_TAG_OPEN_CITE, (cite_format[0]))
+    s = s.replace(_TAG_OPEN_CITE_EQN, '(')
+    s = s.replace(_TAG_CLOSE_CITE, (cite_format[1]))
+    s = s.replace(_TAG_CLOSE_CITE_EQN, ')')
+    s = s.replace(_TAG_ITEM_SPACE, ' ')
+    s = s.replace(_TAG_PERCENTAGE_SYMBOL, '%')
+    s = s.replace(_TAG_BRACE_OPEN, '{')
+    s = s.replace(_TAG_BRACE_CLOSE, '}')
+    s = s.replace(_TAG_NEW_LINE, '\n')
+    if kwargs.get('replace_pydetex_tag_dollar_symbol', True):
+        s = s.replace(_TAG_DOLLAR_SYMBOL, '$')
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Replacing pydetex tags')
+    return s
+
+
+def process_labels(s: str, **kwargs) -> str:
+    """
+    Removes labels.
+
+    :param s: Latex string code
+    :return: String with no labels
+    """
+    while True:
+        k = find_str(s, '\\label{')
+        if k == -1:
+            if kwargs.get('pb'):  # Update progressbar
+                kwargs.get('pb').update('Processing labels')
+            return s
+        for j in range(len(s)):
+            if s[k + j] == '}':
+                s = s[:k] + s[k + j + 1:]
+                break
+
+
+def process_ref(s: str, **kwargs) -> str:
+    """
+    Process references, same as cites, replaces by numbers.
+
+    :param s: Latex string code
+    :return: String with numbers instead of references.
+    """
+    look = ['\\ref{', '\\ref*{', '\\autoref{']
+    refs = []
+    k = -1
+    while True:
+        run_j = ''
+        for j in look.copy():
+            k = find_str(s, j)
+            if k == -1:
+                look.remove(j)
+            else:
+                run_j = j
+                break
+        if k == -1:
+            if kwargs.get('pb'):  # Update progressbar
+                kwargs.get('pb').update('Processing references')
+            return s
+        for j in range(len(s)):
+            if s[k + j] == '}':
+                ref_label = s[k + len(run_j):k + j].strip()
+                if ref_label not in refs:
+                    refs.append(ref_label)
+                ref_idx = refs.index(ref_label) + 1
+                s = s[:k] + FONT_FORMAT_SETTINGS['ref'] + str(ref_idx) + FONT_FORMAT_SETTINGS['normal'] + s[k + j + 1:]
+                break
+
+
+def remove_comments(s: str, **kwargs) -> str:
+    """
+    Remove comments from text.
+
+    :param s: Latex string code
+    :return: String without comments
+    """
+    newline_symbol = '⇱NEWLINE_SYMBOL_REMOVE_COMMENTS⇲'
+    s = s.replace('  ', ' ')
+    s = s.replace('\\\\', newline_symbol)
+    s = s.replace('\\%', _TAG_PERCENTAGE_SYMBOL)
+    s = s.replace('\\\n', '\n')
+    k = s.split('\n')
+
+    for r in range(len(k)):
+        k[r] = k[r].strip()  # Strips all text
+    line_merge: List[bool] = []
+    for r in range(len(k)):
+        sp = k[r].split('%')
+        k[r] = sp[0]  # Removes all comments from list
+        line_merge.append(len(sp) > 1)
+    line_merge.append(False)
+    line_merge2: List[bool] = line_merge.copy()
+    k.append('')
+    for r in range(len(k)):
+        if line_merge[r] and not line_merge[r + 1] and k[r + 1] != '':
+            line_merge2[r + 1] = True
+    for r in range(len(k)):
+        line_merge[r] = line_merge[r] or line_merge2[r]
+    new_k = []
+    j = 0
+    merged_str = ''
+
+    while True:  # Merge comment lines
+        if not line_merge[j]:
+            if merged_str != '':  # Add current merged str
+                new_k.append(merged_str)
+                merged_str = ''
+            new_k.append(k[j])
+        else:
+            merged_str += k[j]
+        if j == len(k) - 1:
+            break
+        j += 1
+    if merged_str != '':
+        new_k.append(merged_str)
+    k = new_k
+
+    w = []  # Remove duplicates '' lines to single ''
+    last = ''
+    for j in k:
+        if j == '' and j == last:
+            pass
+        else:
+            w.append(j)
+        last = j
+
+    if len(w) > 0 and w[-1] == '':  # Removes last space
+        w.pop()
+    s = '\n'.join(w).strip()
+    s = s.replace(newline_symbol, '\\\\')
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing comments')
+    return s
+
+
+def simple_replace(s: str, **kwargs) -> str:
+    """
+    Replace simple tokens.
+
+    :param s: Latex string code
+    :return: String with replaced items
+    """
+    for w in REPLACE_SYMBOLS_LIBRARY:
+        s = s.replace(w[0], w[1])
+
+    # Replace unique symbols
+    s += ' '
+    invalid_tag = '⇱SYMBOL_REPLACE_TAG_TOKEN⇲'
+    for w in REPLACE_TEX_COMMANDS_LIBRARY:
+        word, repl = w
+        while True:
+            k = s.find(word)
+            if k == -1:
+                break
+            if s[k + len(word)] not in ut.TEX_COMMAND_CHARS:
+                s = s[0:k] + repl + s[k + len(word):]
+            else:
+                s = s[0:k + 1] + invalid_tag + s[k + 1:]  # format ...\\INVALID_TAG...
+    s = s[0:len(s) - 1].replace(invalid_tag, '')
+
+    # Replace equation symbols
+    s = s.replace('\$', _TAG_DOLLAR_SYMBOL)
+    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
+    new_s = ''
+    k = 0  # Moves through tags
+    added_s = False
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][1]:
+                new_s += s[i]
+            elif tex_tags[k][1] <= i < tex_tags[k][2] and not added_s or tex_tags[k][1] == i == tex_tags[k][2]:
+                if not added_s:
+                    k_s: str = s[tex_tags[k][1]:tex_tags[k][2] + 1]
+                    # Replace
+                    for j in REPLACE_EQUATION_SYMBOLS_LIBRARY:
+                        k_s = k_s.replace(j[0], j[1])
+                    new_s += k_s
+                added_s = True
+            elif tex_tags[k][2] < i < tex_tags[k][3]:
+                new_s += s[i]
+            elif i == tex_tags[k][3]:  # Advance to other tag
+                new_s += s[i]
+                k += 1
+                added_s = False
+        else:
+            new_s += s[i]
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Replacing simple tokens')
+    return new_s
+
+
+def _load_file_search(tex_file: str, print_error: bool = False) -> str:
+    """
+    Search and load a file.
+
+    :param tex_file: Name of the file
+    :param print_error: Prints if file not found
+    :return: Loaded file or tag error
+    """
+    tx = _TAG_FILE_ERROR
+    folders = _os_listfolder()
+    folders.insert(0, '../')
+    folders.insert(0, './')
+    for f in folders:
+        tx = _load_file(tex_file, f)
+        if tx == _TAG_FILE_ERROR:
+            if print_error:
+                print(f'\tFile not found in {f}')
+        else:
+            break
+    return tx
+
+
+def process_inputs(
+    s: str,
+    clear_not_found_files: bool = False,
+    **kwargs
+) -> str:
+    """
+    Process inputs, which find the input files and retrieve its contents.
+
+    :param s: Latex string code with inputs
+    :param clear_not_found_files: Clear the not found files. Used when changing the path
+    :return: Text copied with data from inputs
+    """
+    global _PRINT_LOCATION, _NOT_FOUND_FILES
+    if os.getcwd() != _LAST_NOT_FOUND_FILES_PATH[0] or clear_not_found_files:
+        _LAST_NOT_FOUND_FILES_PATH[0] = os.getcwd()
+        _NOT_FOUND_FILES.clear()
+        _PRINT_LOCATION = False
+    print_ = kwargs.get('print', True)
+    symbol = '⇱INPUT_FILE_TAG⇲'
+    s = remove_comments(s)
+    while True:
+        k = find_str(s, '\\input{')
+        if k == -1:
+            if kwargs.get('pb'):  # Update progressbar
+                kwargs.get('pb').update('Processing \\input')
+            return s.replace(symbol, '\\input{')
+        m = 0
+        for j in range(len(s)):
+            if s[k + j] == '{':
+                m = j
+            if s[k + j] == '}':
+                tex_file = s[k + m + 1:k + j]
+                if '.tex' not in tex_file:
+                    tex_file += '.tex'
+                if tex_file not in _NOT_FOUND_FILES and '\jobname' not in tex_file:
+                    if not _PRINT_LOCATION:
+                        if print_:
+                            print(f'Current path location:\n\t{os.getcwd()}')
+                        _PRINT_LOCATION = True
+                    if print_:
+                        print(f'Detected file {tex_file}:')
+                    tx = _load_file_search(tex_file, print_error=print_)
+                    if tx == _TAG_FILE_ERROR:
+                        _NOT_FOUND_FILES.append(tex_file)
+                        s = s[:k] + symbol + s[k + m + 1:]
+                    else:
+                        if print_:
+                            print('\tFile found and loaded')
+                        tx = '\n'.join(tx.splitlines())
+                        tx = remove_comments(tx)
+                        s = s[:k] + tx + s[k + j + 1:]
+                else:
+                    s = s[:k] + symbol + s[k + m + 1:]
+                break
+
+
+def remove_commands_char(s: str, chars: List[Tuple[str, str, bool]]) -> str:
+    """
+    Remove all char commands.
+
+    :param s: Latex string code
+    :param chars: Char that define equations [(initial, final, ignore escape), ...]
+    :return: Code with removed chars
+    """
+    tex_tags = ut.find_tex_command_char(s, symbols_char=chars)
+    if len(tex_tags) == 0:
+        return s
+    new_s = ''
+    k = 0  # Moves through tags
+
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][0]:
+                new_s += s[i]
+            # elif tex_tags[k][0] <= i < tex_tags[k][3]:
+            #     pass
+            elif i == tex_tags[k][3]:  # Advance to other tag
+                k += 1
+        else:
+            new_s += s[i]
+
+    return new_s
+
+
+def remove_equations(s: str, **kwargs) -> str:
+    """
+    Remove all equations from a string.
+
+    :param s: Latex string code
+    :return: Latex without equation
+    """
+    s = remove_commands_char(s, chars=ut.TEX_EQUATION_CHARS)
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing equations')
+    return s
+
+
+def output_text_for_some_commands(
+    s: str,
+    lang: str
+) -> str:
+    """
+    Replaces the command for a particular text.
+
+    :param s: Latex string code
+    :param lang: Language tag of the code
+    :return: Text string or empty if error
+    """
+    # Stores the commands to be transformed
+    # (
+    #   command name,
+    #   [(argument number, argument is optional), ...],
+    #   tag to be replaced,
+    #   total commands,
+    #   font_tag ('tex_text_tag' if None),
+    #   font_content ('tex_text_tag_content' if None),
+    #   add new line (before, after)
+    # )
+    # The font format is like .... [font tag]YOUR TAG {[font content]YOUR CONTENT} ...[font normal]. In that case, tag to be
+    # relaced is 'YOUR TAG {0}, {1}
+    # All *arguments will be formatted using the tag
+    commands: List[Tuple[str, List[Tuple[int, bool]], Union[str, Callable[[str, ...], str]], int, Optional[str], Optional[str], Tuple[bool, bool]]] = [
+        ('ac', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
+        ('acf', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
+        ('acl', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
+        ('acs', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),  # Acronym
+        ('caption', [(1, False)], LANG_TT_TAGS.get(lang, 'caption'), 1, None, None, (False, True)),
+        ('chapter', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('chapter*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('doublequotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
+        ('em', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
+        ('emph', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
+        ('enquote', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
+        ('frac', [(1, False), (2, False)], '{0}/{1}', 2, 'normal', 'normal', (False, False)),
+        ('href', [(2, False)], LANG_TT_TAGS.get(lang, 'link'), 2, None, None, (False, False)),
+        ('insertimage', [(3, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 3, None, None, (False, True)),  # (Template) Informe
+        ('insertimage', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, False)),  # (Template) Informe
+        ('insertimageboxed', [(4, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 4, None, None, (False, True)),  # (Template) Informe
+        ('insertimageboxed', [(5, False)], LANG_TT_TAGS.get(lang, 'figure_caption'), 5, None, None, (False, True)),  # (Template) Informe
+        ('institutionentry', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
+        ('institutionentryshort', [(1, False), (2, False), (3, False), (4, False)], '{0} ({1}-{2}). {3}', 4, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
+        ('lowercase', [(1, False)], lambda t: t.lower(), 1, 'normal', 'normal', (False, False)),
+        ('MakeLowercase', [(1, False)], lambda t: t.lower(), 1, 'normal', 'normal', (False, False)),
+        ('MakeUppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False)),
+        ('otherentry', [(1, False), (2, False)], '{0} {1}', 2, 'normal', 'normal', (False, False)),  # (Template) Professional-CV
+        ('paragraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('quotes', [(1, False)], lambda t: '"{0}"'.format(t), 1, 'normal', 'normal', (False, False)),
+        ('section', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('section*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subfloat', [(1, True)], LANG_TT_TAGS.get(lang, 'sub_figure_title'), 1, None, None, (False, True)),
+        ('subparagraph', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsubsubsection', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('subsubsubsection*', [(1, False)], '{0}', 1, 'normal', 'bold', (True, True)),
+        ('textbf', [(1, False)], '{0}', 1, 'normal', 'bold', (False, False)),
+        ('textit', [(1, False)], '{0}', 1, 'normal', 'italic', (False, False)),
+        ('texttt', [(1, False)], '{0}', 1, 'normal', 'normal', (False, False)),
+        ('uppercase', [(1, False)], lambda t: t.upper(), 1, 'normal', 'normal', (False, False))
+    ]
+    new_s = ''
+
+    # Get the commands
+    cmd_args = ut.get_tex_commands_args(s)
+    for c in cmd_args:
+        for cmd in commands:
+            if c[0] == cmd[0]:
+                _, cmd_args, cmd_tag, total_commands, font_tag, font_content, cmd_newline = cmd
+                if font_tag is None:
+                    font_tag = 'tex_text_tag'
+                if font_content is None:
+                    font_content = 'tex_text_tag_content'
+                if len(c) - 1 == total_commands:
+                    args = []
+                    for j in cmd_args:
+                        cmd_argnum, cmd_is_optional = j
+                        if len(c) - 1 >= j[0] >= 0 and c[cmd_argnum][1] == cmd_is_optional:
+                            argv = c[cmd_argnum][0].replace('\n', ' ')  # Command's argument to process
+                            argv = remove_commands_param(argv, lang)  # Remove commands within the argument
+                            argv = argv.strip()
+                            if argv != '':
+                                args.append(argv)
+                    if len(args) == len(cmd_args):
+                        # Add format text
+                        for a in range(len(args)):
+                            args[a] = FONT_FORMAT_SETTINGS[font_content] + args[a] + FONT_FORMAT_SETTINGS[font_tag]
+                        if callable(cmd_tag):
+                            text = cmd_tag(*args)
+                        else:
+                            try:
+                                text = cmd_tag.format(*args)
+                            except IndexError:
+                                text = cmd_tag
+                        text = FONT_FORMAT_SETTINGS[font_tag] + text + FONT_FORMAT_SETTINGS['normal']
+                        if cmd_newline[0]:
+                            text = _TAG_NEW_LINE + text
+                        new_s += text
+                        if cmd_newline[1]:
+                            new_s += _TAG_NEW_LINE
+                        break
+
+    return new_s.strip()
+
+
+def remove_environments(
+    s: str,
+    env_list: Optional[List[str]] = None,
+    **kwargs
+) -> str:
+    """
+    Remove a selection of environments.
+
+    :param s: Latex code
+    :param env_list: Environment list, if not defined, use the default from PyDetex
+    :return: Code without given environments
+    """
+    if not env_list:
+        env_list = [
+            'lstlisting',
+            'references',
+            'minted',
+            'sourcecode',
+            'tabular',
+            'thebibiliography',
+            'tikzpicture',
+            'verbatim'
+        ]
+    tex_tags = ut.find_tex_environments(s)
+    if len(tex_tags) == 0 or len(env_list) == 0:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No environment found in code')
+        return s
+    new_s = ''
+
+    new_tex_tags = []
+    # Remove all the environments not in env_list
+    for t in tex_tags:
+        is_removed = False
+        for j in env_list:
+            if j in t[0]:
+                is_removed = True
+                break
+        if is_removed:
+            new_tex_tags.append(t)
+
+    # If tex tags is empty
+    if len(new_tex_tags) == 0:
+        return s
+
+    def is_in_tags(v: int) -> bool:
+        """
+        Check if a position is within tags.
+
+        :param v: Position
+        :return: True if in tags range
+        """
+        for j_ in new_tex_tags:
+            if j_[1] <= v <= j_[4] + 1:
+                return True
+        return False
+
+    for i in range(len(s)):
+        if not is_in_tags(i):
+            new_s += s[i]
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing environments')
+    return new_s
+
+
+def remove_commands_param(
+    s: str,
+    lang: str,
+    invalid_commands: Optional[List[str]] = None,
+    **kwargs
+) -> str:
+    """
+    Remove all commands with params.
+
+    :param s: Latex string code
+    :param lang: Language tag of the code
+    :param invalid_commands: Invalid commands that will not call output_text_for_some_commands. If ``None`` use defaults
+    :return: Code with removed chars
+    """
+    tex_tags = ut.find_tex_commands(s)
+    if len(tex_tags) == 0:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No parameter commands found in code')
+        return s
+    new_s = ''
+    k = 0  # Moves through tags
+
+    # invalid commands that will not call output_text_for_some_commands
+    if not invalid_commands:
+        invalid_commands = [
+            'DeclareUnicodeCharacter',
+            'ifthenelse',
+            'newcommand',
+            'newenvironment',
+            'usepackage'
+        ]
+
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][0]:
+                new_s += s[i]
+            elif i < tex_tags[k][3] + 1:
+                pass
+            else:  # Advance to other tag
+                sub_s = s[tex_tags[k][0]:tex_tags[k][3] + 2]
+
+                # If the command does not continue, write the text for such
+                # command, if this does not continue (for example, that happens
+                # when calling for \mycommand{1}{2}{3}). In that case, only tex_tags
+                # [\mycommand .... {3}] will be called, thus, sub_s will contain
+                # all the parameters of the command ({1}{2}{3})
+                if not tex_tags[k][4]:
+                    cmd_name = s[tex_tags[k][0]:tex_tags[k][1] + 1].strip()
+
+                    # Check if the invalid_commands are not within command name
+                    is_invalid = False
+                    for c in invalid_commands:
+                        if c in cmd_name:
+                            is_invalid = True
+                            break
+
+                    # If not invalid, call the analysis for its commands, check that
+                    # it can be recursive
+                    if not is_invalid:
+                        new_s += output_text_for_some_commands(sub_s, lang)
+                k += 1
+        else:
+            new_s += s[i]
+
+    # Replace all command symbols
+    parenthesis_open_symbol = '⇱PARENTHESIS_OPEN_SYMBOL⇲'
+    parenthesis_close_symbol = '⇱PARENTHESIS_CLOSE_SYMBOL⇲'
+    parenthesis_sq_open_symbol = '⇱PARENTHESIS_SQ_OPEN_SYMBOL⇲'
+    parenthesis_sq_close_symbol = '⇱PARENTHESIS_SQ_CLOSE_SYMBOL⇲'
+    new_s = new_s.replace('\\{', parenthesis_open_symbol)
+    new_s = new_s.replace('\\}', parenthesis_close_symbol)
+    new_s = new_s.replace('\\[', parenthesis_sq_open_symbol)
+    new_s = new_s.replace('\\]', parenthesis_sq_close_symbol)
+    new_s = new_s.replace('{', '').replace('}', '')  # .replace('[', '').replace(']', '')
+    new_s = new_s.replace(parenthesis_open_symbol, '\\{')
+    new_s = new_s.replace(parenthesis_close_symbol, '\\}')
+    new_s = new_s.replace(parenthesis_sq_open_symbol, '\\[')
+    new_s = new_s.replace(parenthesis_sq_close_symbol, '\\]')
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing command with parameters')
+    return new_s
+
+
+def remove_commands_param_noargv(s: str, **kwargs) -> str:
+    """
+    Remove all commands without arguments.
+
+    :param s: Latex string code
+    :return: Code with removed chars
+    """
+    tex_tags = ut.find_tex_commands_noargv(s)
+    if len(tex_tags) == 0:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No command without arguments were found in code')
+        return s
+    new_s = ''
+    k = 0  # Moves through tags
+
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][0]:
+                new_s += s[i]
+            elif i < tex_tags[k][1]:
+                pass
+            else:  # Advance to other tag
+                k += 1
+        else:
+            new_s += s[i]
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Removing command without arguments')
+    return new_s
+
+
+def unicode_chars_equations(s: str, **kwargs) -> str:
+    """
+    Converts all equations to unicode.
+
+    :param s: Latex string code
+    :return: Latex with unicode converted
+    """
+    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
+    new_s = ''
+    k = 0  # Moves through tags
+    added_s = False
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][1]:
+                new_s += s[i]
+            elif tex_tags[k][1] <= i < tex_tags[k][2] and not added_s or tex_tags[k][1] == i == tex_tags[k][2]:
+                if not added_s:
+                    k_s: str = s[tex_tags[k][1]:tex_tags[k][2] + 1]
+                    k_s_tex = ut.tex_to_unicode(k_s)
+                    k_s_tex = k_s_tex.replace('\{', _TAG_BRACE_OPEN).replace('\}', _TAG_BRACE_CLOSE)
+                    new_s += k_s_tex
+                added_s = True
+            elif tex_tags[k][2] < i < tex_tags[k][3]:
+                new_s += s[i]
+            elif i == tex_tags[k][3]:  # Advance to other tag
+                new_s += s[i]
+                k += 1
+                added_s = False
+        else:
+            new_s += s[i]
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Processing unicode equations')
+    return new_s
+
+
+def process_chars_equations(
+    s: str,
+    lang: str,
+    single_only: bool,
+    **kwargs
+) -> str:
+    """
+    Process single char equations, removing the symbols.
+
+    :param s: Latex string code
+    :param lang: Language tag of the code
+    :param single_only: Only process single char equations. If False, replaces the equation by a text-label
+    :return: Code without symbols
+    """
+    tex_tags = ut.find_tex_command_char(s, ut.TEX_EQUATION_CHARS)
+    if len(tex_tags) == 0:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No char equtions found')
+        return s
+
+    new_s = ''
+    k = 0  # Moves through tags
+    eqn_number = 0
+    added_equ = False
+
+    for i in range(len(s)):
+        if k < len(tex_tags):
+            if i < tex_tags[k][0]:
+                new_s += s[i]
+            # elif tex_tags[k][0] <= i < tex_tags[k][1]:
+            #     continue
+            elif tex_tags[k][1] <= i <= tex_tags[k][2] and not added_equ:
+                equ = s[tex_tags[k][1]:tex_tags[k][2] + 1]
+                if len(equ) == 1:
+                    new_s += FONT_FORMAT_SETTINGS['equation'] + s[i] + FONT_FORMAT_SETTINGS['normal']
+                else:
+                    if not single_only:
+                        new_s += FONT_FORMAT_SETTINGS['equation'] + \
+                                 LANG_TT_TAGS.get(lang, 'multi_char_equ').format(eqn_number) + \
+                                 FONT_FORMAT_SETTINGS['normal']
+                        eqn_number += 1
+                    else:
+                        new_s += equ
+                added_equ = True
+            # elif tex_tags[k][2] < i < tex_tags[k][3]:
+            #     continue
+            elif tex_tags[k][3] == i:
+                k += 1
+                added_equ = False
+                continue
+        else:
+            new_s += s[i]
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Processing char equations')
+    return new_s
+
+
+def strip_punctuation(s: str, **kwargs) -> str:
+    """
+    Strips punctuation. For example, ``'mycode :'`` to ``'mycode:'``.
+
+    :param s: Latex string code
+    :return: Stripped punctuation
+    """
+    for j in [',', ':', '=', ';', '!', '?', '.']:  # Before
+        s = s.replace(f' {j}', j)
+    s = s.replace('\n\n\n', '\n\n')
+    s = s.strip()
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Stripping punctuation')
+    return s
+
+
+def process_def(
+    s: str,
+    clear_learned: bool = True,
+    replace: bool = False,
+    **kwargs
+) -> str:
+    """
+    Process \defs. Store the definition, among others.
+
+    :param s: Latex with definitions
+    :param clear_learned: Clear the last learned definitions
+    :param replace: Replace instances of learned defs
+    :return: Latex without definitions
+    """
+    if '\\def' not in s:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No definitions found in code')
+        return s
+    if clear_learned:
+        _DEFS.clear()
+    s += '    '
+    new_s = ''
+    found_def = False
+    a, b, c, depth = 0, 0, -1, -1  # Def positions (a\def      b{ .... c}
+    def_ranges = []
+    for i in range(len(s) - 4):
+        # After finding a def, check the first and last parenthesis
+        if s[i:i + 4] == '\\def' and s[i + 4] not in ut.TEX_COMMAND_CHARS:
+            a, b, depth = i, -1, 0
+            found_def = True
+            continue
+        elif found_def:
+            if found_def and s[i] == '{' and s[i - 1] != '\\':
+                if depth == 0:
+                    b = i
+                depth += 1
+            if found_def and s[i] == '}' and s[i - 1] != '\\':
+                depth -= 1
+                if depth == 0:
+                    c = i
+                    def_ranges.append((a, c))
+
+                    # Check the name, if not a command, store
+                    def_name = s[a + 4:b].strip()
+                    if '#' not in def_name:
+                        _DEFS[def_name] = remove_common_tags(s[b + 1:c])
+                    found_def = False
+            continue
+
+        else:
+            new_s += s[i]
+
+    # Now, if replace defs is enabled, check all non-arg commands and replace if
+    # known
+    if replace:
+        new_s_def = ''
+        st = ut.find_tex_commands_noargv(new_s)
+        w = 0  # Iterates through st
+        k = 0
+        if len(st) > 0:
+            for _ in range(len(new_s)):
+                if k < len(new_s):
+                    if k < st[w][0]:
+                        new_s_def += new_s[k]
+                    else:
+                        a, b = st[w]
+                        def_n = new_s[a:b + 1]
+                        if def_n in _DEFS.keys():
+                            new_s_def += _DEFS[def_n]
+                        else:
+                            new_s_def += new_s[a:b + 1]
+                        k += b - a
+                        w += 1
+                        if w == len(st):
+                            new_s_def += new_s[k + 1:]
+                            break
+                k += 1
+            new_s = new_s_def
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Processing definitions')
+
+    return new_s
+
+
+def process_items(s: str, lang: str, **kwargs) -> str:
+    """
+    Process itemize and enumerate.
+
+    :param s: Latex string code
+    :param lang: Language tag
+    :return: Processed items
+    """
+    if not ('itemize' in s or 'enumerate' in s or 'tablenotes' in s):
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No item found')
+        return s
+
+    def _get_name(e: str) -> str:
+        """
+        Get the environment name.
+
+        :param e: Environment name
+        :return: New name
+        """
+        # This is due to itemize can contain other symbols or spaces, thus,
+        # itemize*    .. is converted to itemize
+        if 'itemize' in e:
+            return 'itemize'
+        if 'enumerate' in e:
+            return 'enumerate'
+        if 'tablenotes' in e:
+            return 'tablenotes'
+        return ''
+
+    def _are_item(e: str) -> bool:
+        """
+        Return true if both are enumerated. Used to check recursive enumerates.
+
+        :param e: Environment name
+        :return: True if item
+        """
+        return e == 'itemize' or e == 'enumerate' or e == 'tablenotes'
+
+    # First, process the nested ones
+    while True:
+        equal = False
+        envs = ut.find_tex_environments(s)
+        for tag in envs:
+            t, a, b, c, d, t2, _, item_depth = tag
+            t, t2 = _get_name(t), _get_name(t2)
+            if t == '' or t2 == '':
+                continue
+            if t == t2 or _are_item(t) and _are_item(t2):
+                s = s[0:a] + _process_item(s[b:c].strip(), t, item_depth) + s[d + 2:]
+                equal = True
+                break
+        if not equal:
+            break
+
+    # Not nested
+    while True:
+        conv = False
+        envs = ut.find_tex_environments(s)
+        for tag in envs:
+            t, a, b, c, d, _, _, _ = tag
+            t = _get_name(t)
+            if t == '':
+                continue
+            s = s[0:a] + remove_commands_param(_process_item(s[b:c].strip(), t), lang) + s[d + 2:]
+            conv = True
+            break
+        if not conv:
+            break
+
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Processing item/enumerate environments')
+    return s
+
+
+def _process_item(s: str, t: str, depth: int = 0) -> str:
+    """
+    Process the items.
+
+    :param s: Latex string code
+    :param t: Type (enumerate, itemize)
+    :param depth: Depth
+    :return: Processed items
+    """
+    if len(s) == 0:
+        return ''
+    line = '\n' + _TAG_ITEM_SPACE * (3 * depth)
+
+    def _num(x: int) -> str:
+        """
+        Get number based on the depth.
+
+        :param x: Number
+        :return: Number format by depth
+        """
+        if depth % 5 == 0:
+            return f'{line}{x}. '
+        elif depth % 5 == 1:
+            x = _int_to_alph(x).lower()
+            return f'{line}{x}) '
+        elif depth % 5 == 2:
+            x = _int_to_roman(x).lower()
+            return f'{line}{x}. '
+        elif depth % 5 == 3:
+            x = _int_to_alph(x).upper()
+            return f'{line}{x}) '
+        elif depth % 5 == 4:
+            x = _int_to_roman(x).upper()
+            return f'{line}{x}. '
+
+    def _itm() -> str:
+        """
+        :return: The item string based on depth.
+        """
+        char = ['-', '•', '◦', '■', '*']
+        x = char[depth % 5]
+        return f'{line}{x} '
+
+    # Remove optional arguments list
+    if s[0] == '[':
+        sqd = 1
+        for j in range(1, len(s)):
+            if s[j] == '[':
+                sqd += 1
+            elif s[j] == ']':
+                sqd -= 1
+            if sqd == 0:
+                s = s[j + 1:len(s)].strip()
+                break
+
+    # Remove invalid newlines
+    s_ = []
+    for v in s.split('\n'):
+        v = v.strip()
+        if v != '':
+            s_.append(v)
+    s_ = '\n'.join(s_)
+    s = s_
+
+    if t == 'enumerate':
+        s += ' ' * 5
+        new_s = ''
+        k = 1
+        j = -1
+        while True:
+            j += 1
+            if s[j:j + 5] == '\\item':
+                new_s += _num(k)
+                j += 5
+                k += 1
+            else:
+                new_s += s[j]
+            if j == len(s) - 5:
+                break
+    else:
+        new_s = s.replace('\\item', _itm())
+
+    # Last operations
+    new_s = new_s.replace('\n\n', '\n').strip(' ')
+    return new_s
+
+
+def _int_to_roman(number: int) -> str:
+    """
+    Convert an arabic integer number to a roman.
+
+    :param number: Number
+    :return: Number in roman
+    """
+    result = ''
+    for (arabic, roman) in _ROMAN_DIGITS:
+        (factor, number) = divmod(number, arabic)
+        result += roman * factor
+    return result
+
+
+def _int_to_alph(n: int) -> str:
+    """
+    Integer to a..z.
+
+    :param n: Number
+    :return: Number in AABB..
+    """
+    string = ''
+    while n > 0:
+        n, remainder = divmod(n - 1, 26)
+        string = chr(65 + remainder) + string
+    return string
+
+
+def process_begin_document(s: str, **kwargs) -> str:
+    """
+    Removes all code outside begin document, if found.
+
+    :param s: Latex code
+    :return: Removes all data outside the document
+    """
+    if '{document}' not in s:
+        if kwargs.get('pb'):  # Update progressbar
+            kwargs.get('pb').update('No document environment found')
+        return s
+
+    s += '          '
+    is_env = False
+    is_end = False
+    is_document_begin = False
+    i, j, w = -1, -1, -1  # Init and start of "begin document", w indicates the start of \end
+    # Find if begin document exists
+    for k in range(len(s) - 10):
+        if s[k:k + 6] == '\\begin':
+            is_env = True
+        elif s[k] == '{' and s[k - 1] != '\\' and is_env and not is_document_begin:
+            if s[k:k + 10] == '{document}':
+                is_document_begin = True
+                i = k + 10
+            else:
+                is_env = False
+        elif is_document_begin and s[k:k + 4] == '\\end':
+            is_end = True
+            w = k
+        elif is_document_begin and is_end and s[k] == '{' and s[k - 1] != '\\':
+            if s[k:k + 10] == '{document}':
+                break
+
+    # If document has been found
+    if kwargs.get('pb'):  # Update progressbar
+        kwargs.get('pb').update('Processing {document} environment')
+    if -1 < i <= w:
+        return s[i:w]
+    return s[0:len(s) - 10]
```

### Comparing `pydetex-1.0.0/pydetex/pipelines.py` & `pydetex-1.0.1/pydetex/pipelines.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 PIPELINES
 Defines the pipelines which apply parsers.
 """
 
 __all__ = [
     'simple',
     'strict',
+    'strict_eqn',
     'PipelineType'
 ]
 
 import pydetex.parsers as par
 from pydetex.utils import ProgressBar
 from typing import Callable
 
@@ -21,75 +22,104 @@
 
 def simple(
     s: str,
     lang: str = 'en',
     show_progress: bool = False,
     replace_pydetex_tags: bool = True,
     remove_common_tags: bool = True,
+    replace_single_chars_eqn: bool = True,
     **kwargs
 ) -> str:
     """
     The most simple pipeline ever.
 
     :param s: String latex
     :param lang: Language tag of the code
     :param show_progress: Show progress bar
     :param replace_pydetex_tags: Replace pydetex tags like symbols, cites
     :param remove_common_tags: Call ``remove_common_tags`` parser
+    :param replace_single_chars_eqn: Replaces all single char equations
     :return: String with no latex!
     """
     if len(s) == 0:
         return s
-    pb = kwargs.get('progressbar', ProgressBar(steps=16 if replace_pydetex_tags else 15)) if show_progress else None
+    steps = 17
+    if not replace_pydetex_tags:
+        steps -= 1
+    if not replace_single_chars_eqn:
+        steps -= 1
+    pb = kwargs.get('progressbar', ProgressBar(steps)) if show_progress else None
     s = '\n'.join(s.splitlines())  # Removes \r\n
     s = par.process_inputs(s, pb=pb)
     s = par.remove_comments(s, pb=pb)
     s = par.process_begin_document(s, pb=pb)
     s = par.simple_replace(s, pb=pb)
     s = par.process_def(s, pb=pb, replace=kwargs.get('replace_defs', False))
     if remove_common_tags:
         s = par.remove_common_tags(s, pb=pb)
     s = par.process_cite(s, pb=pb, compress_cite=kwargs.get('compress_cite', True))
     s = par.process_citeauthor(s, lang, pb=pb)
     s = par.process_ref(s, pb=pb)
     s = par.process_labels(s, pb=pb)
     s = par.process_items(s, lang, pb=pb)
-    s = par.process_chars_equations(s, lang, single_only=True, pb=pb)
+    if replace_single_chars_eqn:
+        s = par.process_chars_equations(s, lang, single_only=True, pb=pb)
     s = par.unicode_chars_equations(s, pb=pb)
     s = par.remove_comments(s, pb=pb)  # comments, replace tags, strip
     if replace_pydetex_tags:
         s = par.replace_pydetex_tags(s, pb=pb, **kwargs)
     s = par.strip_punctuation(s, pb=pb)
+    s = par.simple_replace(s, pb=pb)
     if s[-1] == '\\':
         s = s[0:len(s) - 1]
     return s
 
 
 def strict(
     s: str,
     lang: str = 'en',
     show_progress: bool = False,
+    eqn_simple: bool = True,
     **kwargs
 ) -> str:
     """
     Apply simple + removes all commands.
 
     :param s: String latex
     :param lang: Language tag of the code
     :param show_progress: Show progress bar
+    :param eqn_simple: If true, replace equations with a label, else, attempt to write it as-is
     :return: String with no latex!
     """
-    pb = ProgressBar(steps=21) if show_progress else None
+    pb = ProgressBar(steps=24) if show_progress else None
     if 'progressbar' not in kwargs.keys():
         # noinspection PyTypeChecker
         kwargs['progressbar'] = pb
     s = simple(s, lang, replace_pydetex_tags=False, remove_common_tags=False,
-               show_progress=show_progress, **kwargs)
-    s = par.process_chars_equations(s, lang, False, pb=pb)
+               show_progress=show_progress, replace_single_chars_eqn=False, **kwargs)  # 15 steps
+    s = par.process_chars_equations(s, lang, single_only=not eqn_simple, pb=pb)
     s = par.remove_equations(s, pb=pb)
     s = par.remove_environments(s, pb=pb)
     s = par.remove_commands_param(s, lang, pb=pb)
     s = par.remove_commands_param_noargv(s, pb=pb)
     s = par.remove_comments(s, pb=pb)
     s = par.replace_pydetex_tags(s, pb=pb, **kwargs)
     s = par.strip_punctuation(s, pb=pb)
+    s = par.simple_replace(s, pb=pb)
     return s
+
+
+def strict_eqn(
+    s: str,
+    lang: str = 'en',
+    show_progress: bool = False,
+    **kwargs
+) -> str:
+    """
+    Same as strict, but replaces the equations with their string representation.
+
+    :param s: String latex
+    :param lang: Language tag of the code
+    :param show_progress: Show progress bar
+    :return: String with no latex!
+    """
+    return strict(s, lang, show_progress, eqn_simple=False, **kwargs)
```

### Comparing `pydetex-1.0.0/pydetex/res/cog.ico` & `pydetex-1.0.1/pydetex/res/cog.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/dictionary.ico` & `pydetex-1.0.1/pydetex/res/dictionary.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/icon.gif` & `pydetex-1.0.1/pydetex/res/icon.gif`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/icon.ico` & `pydetex-1.0.1/pydetex/res/icon.ico`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/placeholder_en.tex` & `pydetex-1.0.1/pydetex/res/placeholder_en.tex`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/placeholder_es.tex` & `pydetex-1.0.1/pydetex/res/placeholder_es.tex`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/stopwords.json` & `pydetex-1.0.1/pydetex/res/stopwords.json`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/u_symbols.txt` & `pydetex-1.0.1/pydetex/res/u_symbols.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/u_textbf.txt` & `pydetex-1.0.1/pydetex/res/u_textbf.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/res/u_textit.txt` & `pydetex-1.0.1/pydetex/res/u_textit.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/pydetex/utils.py` & `pydetex-1.0.1/pydetex/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     """
     Split a string based on tags, each line is then tagged.
 
     String format:
     [TAG1]new line[TAG2]this is[TAG1]very epic
 
     Output:
-    [('TAG1', 'newline'), ('TAG', 'this is), ('TAG1', 'very epic')]
+    [('TAG1', 'newline'), ('TAG', 'this is), ('TAG1', 'very epic') ... ]
 
     :param s: String
     :param tags: Tag list
     :return: Split tags
     """
     assert len(tags) > 0
     tagged_lines: List[Tuple[str, str]] = []
```

### Comparing `pydetex-1.0.0/pydetex/version.py` & `pydetex-1.0.1/pydetex/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,10 +28,10 @@
         return '{}.{}.{}'.format(*self)
 
     major = property(lambda self: self[0])
     minor = property(lambda self: self[1])
     patch = property(lambda self: self[2])
 
 
-vernum = Version(1, 0, 0)
+vernum = Version(1, 0, 1)
 ver = str(vernum)
 rev = ''
```

### Comparing `pydetex-1.0.0/pydetex.egg-info/PKG-INFO` & `pydetex-1.0.1/pydetex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydetex
-Version: 1.0.0
+Version: 1.0.1
 Summary: An application that transforms LaTeX code to plain text
 Home-page: https://pydetex.readthedocs.io
 Author: Pablo Pizarro R.
 Author-email: pablo@ppizarror.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/ppizarror/PyDetex/issues
 Project-URL: Documentation, https://pydetex.readthedocs.io
```

### Comparing `pydetex-1.0.0/pydetex.egg-info/SOURCES.txt` & `pydetex-1.0.1/pydetex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydetex-1.0.0/setup.py` & `pydetex-1.0.1/setup.py`

 * *Files identical despite different names*

