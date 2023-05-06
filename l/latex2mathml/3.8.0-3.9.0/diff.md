# Comparing `tmp/latex2mathml-3.8.0.tar.gz` & `tmp/latex2mathml-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latex2mathml-3.8.0.tar", max compression
+gzip compressed data, was "latex2mathml-3.9.0.tar", max compression
```

## Comparing `latex2mathml-3.8.0.tar` & `latex2mathml-3.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1087 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/LICENSE
--rw-r--r--   0        0        0     2646 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/README.md
--rw-r--r--   0        0        0        0 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/__init__.py
--rw-r--r--   0        0        0     3698 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/commands.py
--rw-r--r--   0        0        0    11514 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/converter.py
--rw-r--r--   0        0        0      382 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/exceptions.py
--rw-r--r--   0        0        0     1130 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/symbols_parser.py
--rw-r--r--   0        0        0     6480 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/tokenizer.py
--rw-r--r--   0        0        0   216332 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/unimathsymbols.txt
--rw-r--r--   0        0        0     9148 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/latex2mathml/walker.py
--rw-r--r--   0        0        0     2087 2021-06-05 11:15:09.112440 latex2mathml-3.8.0/pyproject.toml
--rw-r--r--   0        0        0     3527 2021-06-05 11:16:10.136788 latex2mathml-3.8.0/setup.py
--rw-r--r--   0        0        0     3724 2021-06-05 11:16:10.137181 latex2mathml-3.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1087 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/LICENSE
+-rw-r--r--   0        0        0     2646 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/README.md
+-rw-r--r--   0        0        0        0 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/__init__.py
+-rw-r--r--   0        0        0     3734 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/commands.py
+-rw-r--r--   0        0        0    11521 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/converter.py
+-rw-r--r--   0        0        0      382 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/exceptions.py
+-rw-r--r--   0        0        0     1130 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/symbols_parser.py
+-rw-r--r--   0        0        0     6480 2021-06-05 11:41:35.213216 latex2mathml-3.9.0/latex2mathml/tokenizer.py
+-rw-r--r--   0        0        0   216332 2021-06-05 11:41:35.217216 latex2mathml-3.9.0/latex2mathml/unimathsymbols.txt
+-rw-r--r--   0        0        0     9148 2021-06-05 11:41:35.217216 latex2mathml-3.9.0/latex2mathml/walker.py
+-rw-r--r--   0        0        0     2087 2021-06-05 11:41:35.217216 latex2mathml-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3527 2021-06-05 11:42:37.167269 latex2mathml-3.9.0/setup.py
+-rw-r--r--   0        0        0     3724 2021-06-05 11:42:37.167655 latex2mathml-3.9.0/PKG-INFO
```

### Comparing `latex2mathml-3.8.0/LICENSE` & `latex2mathml-3.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/README.md` & `latex2mathml-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/latex2mathml/commands.py` & `latex2mathml-3.9.0/latex2mathml/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 SUMMATION = r"\sum"
 LIMIT = (r"\lim", r"\sup", r"\inf", r"\max", r"\min")
 
 OPERATORNAME = r"\operatorname"
 
 LBRACE = r"\{"
 
-FUNCTIONS = (r"\log", r"\ln", r"\tan", r"\sec", r"\cos", r"\sin", r"\cot", r"\csc")
+FUNCTIONS = (r"\log", r"\ln", r"\tan", r"\sec", r"\cos", r"\sin", r"\cot", r"\csc", r"\arccos", r"\arcsin", r"\arctan")
 
 HLINE = r"\hline"
 
 CASES = r"\cases"
 SUBSTACK = r"\substack"
 MATRICES = (
     r"\matrix",
```

### Comparing `latex2mathml-3.8.0/latex2mathml/converter.py` & `latex2mathml-3.9.0/latex2mathml/converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,18 +235,18 @@
 
 def _convert_symbol(node: Node, parent: Element, is_math_mode: bool = False, font: Optional[str] = None) -> None:
     token = node.token
     symbol = convert_symbol(token)
     if re.match(r"\d+(.\d+)?", token):
         mn = SubElement(parent, "mn")
         mn.text = token
-    elif len(token) and token in "<>&":
+    elif token in ("<", ">", "&", r"\And"):
         mo = SubElement(parent, "mo")
-        mo.text = {"<": "&lt;", ">": "&gt;", "&": "&amp;"}[token]
-    elif len(token) and token in ("+", "-", "*", "/", "(", ")", "=", ",", "?", "[", "]", "|", r"\|", "!"):
+        mo.text = {"<": "&lt;", ">": "&gt;", "&": "&amp;", r"\And": "&amp;"}[token]
+    elif token in ("+", "-", "*", "/", "(", ")", "=", ",", "?", "[", "]", "|", r"\|", "!"):
         mo = SubElement(parent, "mo")
         mo.text = token if symbol is None else "&#x{};".format(symbol)
         if token == r"\|":
             mo.attrib["fence"] = "false"
         if token in ("(", ")", "[", "]", "|", r"\|"):
             mo.attrib["stretchy"] = "false"
     elif (
```

### Comparing `latex2mathml-3.8.0/latex2mathml/symbols_parser.py` & `latex2mathml-3.9.0/latex2mathml/symbols_parser.py`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/latex2mathml/tokenizer.py` & `latex2mathml-3.9.0/latex2mathml/tokenizer.py`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/latex2mathml/unimathsymbols.txt` & `latex2mathml-3.9.0/latex2mathml/unimathsymbols.txt`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/latex2mathml/walker.py` & `latex2mathml-3.9.0/latex2mathml/walker.py`

 * *Files identical despite different names*

### Comparing `latex2mathml-3.8.0/pyproject.toml` & `latex2mathml-3.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latex2mathml"
-version = "3.8.0"
+version = "3.9.0"
 repository = "https://github.com/roniemartinez/latex2mathml"
 description = "Pure Python library for LaTeX to MathML conversion"
 authors = ["Ronie Martinez <ronmarti18@gmail.com>"]
 license = "MIT"
 include = ["latex2mathml/unimathsymbols.txt"]
 readme = "README.md"
 keywords = [
```

### Comparing `latex2mathml-3.8.0/setup.py` & `latex2mathml-3.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 entry_points = \
 {'console_scripts': ['l2m = latex2mathml.converter:main',
                      'latex2mathml = latex2mathml.converter:main']}
 
 setup_kwargs = {
     'name': 'latex2mathml',
-    'version': '3.8.0',
+    'version': '3.9.0',
     'description': 'Pure Python library for LaTeX to MathML conversion',
     'long_description': '# latex2mathml\n\nPure Python library for LaTeX to MathML conversion\n\n<table>\n    <tr>\n        <td>License</td>\n        <td><img src=\'https://img.shields.io/pypi/l/latex2mathml.svg\' alt="License"></td>\n        <td>Version</td>\n        <td><img src=\'https://img.shields.io/pypi/v/latex2mathml.svg\' alt="Version"></td>\n    </tr>\n    <tr>\n        <td>Travis CI</td>\n        <td><img src=\'https://www.travis-ci.com/roniemartinez/latex2mathml.svg?branch=master\' alt="Travis CI"></td>\n        <td>Coverage</td>\n        <td><img src=\'https://codecov.io/gh/roniemartinez/latex2mathml/branch/master/graph/badge.svg\' alt="CodeCov"></td>\n    </tr>\n    <tr>\n        <td>Supported versions</td>\n        <td><img src=\'https://img.shields.io/pypi/pyversions/latex2mathml.svg\' alt="Python Versions"></td>\n        <td>Wheel</td>\n        <td><img src=\'https://img.shields.io/pypi/wheel/latex2mathml.svg\' alt="Wheel"></td>\n    </tr>\n    <tr>\n        <td>Status</td>\n        <td><img src=\'https://img.shields.io/pypi/status/latex2mathml.svg\' alt="Status"></td>\n        <td>Downloads</td>\n        <td><img src=\'https://img.shields.io/pypi/dm/latex2mathml.svg\' alt="Downloads"></td>\n    </tr>\n</table>\n\n## Support\nIf you like `latex2mathml` or if it is useful to you, show your support by buying me a coffee.\n\n<a href="https://www.buymeacoffee.com/roniemartinez" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>\n\n## Installation\n\n```bash\npip install latex2mathml\n```\n\n## Usage\n\n### Python\n\n```python\nimport latex2mathml.converter\n\nlatex_input = "<your_latex_string>"\nmathml_output = latex2mathml.converter.convert(latex_input)\n```\n\n### Command-line\n\n```shell\n% latex2mathml -h\nusage: l2m [-h] [-V] [-b] [-t TEXT | -f FILE]\n\nPure Python library for LaTeX to MathML conversion\n\noptional arguments:\n  -h, --help            show this help message and exit\n  -V, --version         Show version\n  -b, --block           Display block\n\nrequired arguments:\n  -t TEXT, --text TEXT  Text\n  -f FILE, --file FILE  File\n```\n\n## References\n### LaTeX\n\n- https://en.wikibooks.org/wiki/LaTeX/Mathematics\n- http://artofproblemsolving.com/wiki/index.php?title=Main_Page\n- http://milde.users.sourceforge.net/LUCR/Math/\n- https://math-linux.com/latex-26/faq/latex-faq/article/latex-derivatives-limits-sums-products-and-integrals\n- https://www.tutorialspoint.com/tex_commands\n- https://www.giss.nasa.gov/tools/latex/ltx-86.html\n- https://ftp.gwdg.de/pub/ctan/info/l2tabu/english/l2tabuen.pdf\n\n### MathML\n\n- http://www.xmlmind.com/tutorials/MathML/\n\n\n## Author\n- [Ronie Martinez](mailto:ronmarti18@gmail.com)\n',
     'author': 'Ronie Martinez',
     'author_email': 'ronmarti18@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/roniemartinez/latex2mathml',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['latex2mathml'] package_data = \ {'': ['*']} entry_points = \
 {'console_scripts': ['l2m = latex2mathml.converter:main', 'latex2mathml =
 latex2mathml.converter:main']} setup_kwargs = { 'name': 'latex2mathml',
-'version': '3.8.0', 'description': 'Pure Python library for LaTeX to MathML
+'version': '3.9.0', 'description': 'Pure Python library for LaTeX to MathML
 conversion', 'long_description': '# latex2mathml\n\nPure Python library for
 LaTeX to MathML conversion\n\n
 License            [License]         Version   [Version]
 Travis CI          [Travis CI]       Coverage  [CodeCov]
 Supported versions [Python Versions] Wheel     [Wheel]
 Status             [Status]          Downloads [Downloads]
 \n\n## Support\nIf you like `latex2mathml` or if it is useful to you, show your
```

### Comparing `latex2mathml-3.8.0/PKG-INFO` & `latex2mathml-3.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latex2mathml
-Version: 3.8.0
+Version: 3.9.0
 Summary: Pure Python library for LaTeX to MathML conversion
 Home-page: https://github.com/roniemartinez/latex2mathml
 License: MIT
 Keywords: latex,mathml
 Author: Ronie Martinez
 Author-email: ronmarti18@gmail.com
 Requires-Python: >=3.6.2,<4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: latex2mathml Version: 3.8.0 Summary: Pure Python
+Metadata-Version: 2.1 Name: latex2mathml Version: 3.9.0 Summary: Pure Python
 library for LaTeX to MathML conversion Home-page: https://github.com/
 roniemartinez/latex2mathml License: MIT Keywords: latex,mathml Author: Ronie
 Martinez Author-email: ronmarti18@gmail.com Requires-Python: >=3.6.2,<4
 Classifier: Development Status :: 5 - Production/Stable Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
```

