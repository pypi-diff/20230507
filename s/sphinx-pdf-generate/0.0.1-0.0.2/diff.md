# Comparing `tmp/sphinx_pdf_generate-0.0.1.tar.gz` & `tmp/sphinx_pdf_generate-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_pdf_generate-0.0.1.tar", max compression
+gzip compressed data, was "sphinx_pdf_generate-0.0.2.tar", max compression
```

## Comparing `sphinx_pdf_generate-0.0.1.tar` & `sphinx_pdf_generate-0.0.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1068 2023-05-07 00:28:22.091127 sphinx_pdf_generate-0.0.1/LICENSE.md
--rw-r--r--   0        0        0     4486 2023-05-07 00:28:22.091127 sphinx_pdf_generate-0.0.1/README.rst
--rw-r--r--   0        0        0     3311 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/__init__.py
--rw-r--r--   0        0        0      115 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/__main__.py
--rw-r--r--   0        0        0     1897 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/build.py
--rw-r--r--   0        0        0     5364 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/cli.py
--rw-r--r--   0        0        0     2437 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/cover.py
--rw-r--r--   0        0        0     3029 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/generate_txt.py
--rw-r--r--   0        0        0      171 2023-05-07 00:28:22.095127 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/logging.py
--rw-r--r--   0        0        0     3860 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/options.py
--rw-r--r--   0        0        0     9834 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/pdf_generate.py
--rw-r--r--   0        0        0       58 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/__init__.py
--rw-r--r--   0        0        0       67 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/content/__init__.py
--rw-r--r--   0        0        0      837 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/content/tabbed_block.py
--rw-r--r--   0        0        0       67 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/links/__init__.py
--rw-r--r--   0        0        0     1970 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/links/util.py
--rw-r--r--   0        0        0     2286 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/prep.py
--rw-r--r--   0        0        0     6168 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/renderer.py
--rw-r--r--   0        0        0     3135 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/__init__.py
--rw-r--r--   0        0        0     1294 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/_paging.css
--rw-r--r--   0        0        0     1777 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/cover.css
--rw-r--r--   0        0        0     1659 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/toc.css
--rw-r--r--   0        0        0        0 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/__init__.py
--rw-r--r--   0        0        0     1272 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/default_cover.html.j2
--rw-r--r--   0        0        0      437 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/filters/__init__.py
--rw-r--r--   0        0        0      184 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/filters/datetime.py
--rw-r--r--   0        0        0      924 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/filters/url.py
--rw-r--r--   0        0        0     5038 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/template.py
--rw-r--r--   0        0        0        0 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/__init__.py
--rw-r--r--   0        0        0     3701 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/alabaster.py
--rw-r--r--   0        0        0      458 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/generic.py
--rw-r--r--   0        0        0    11433 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/immaterial_styles.css
--rw-r--r--   0        0        0     1852 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/material_styles.css
--rw-r--r--   0        0        0     4270 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/sphinx_immaterial.py
--rw-r--r--   0        0        0     4273 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/sphinx_material.py
--rw-r--r--   0        0        0     5796 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/toc.py
--rw-r--r--   0        0        0     3780 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/utils.py
--rw-r--r--   0        0        0       22 2023-05-07 00:28:22.099128 sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/version.py
--rw-r--r--   0        0        0     6309 1970-01-01 00:00:00.000000 sphinx_pdf_generate-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-07 01:56:49.720092 sphinx_pdf_generate-0.0.2/LICENSE.md
+-rw-r--r--   0        0        0     5646 2023-05-07 01:56:49.720092 sphinx_pdf_generate-0.0.2/README.rst
+-rw-r--r--   0        0        0     3311 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/__init__.py
+-rw-r--r--   0        0        0      115 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/__main__.py
+-rw-r--r--   0        0        0     1897 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/build.py
+-rw-r--r--   0        0        0     5288 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cli.py
+-rw-r--r--   0        0        0     2437 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cover.py
+-rw-r--r--   0        0        0     3029 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/generate_txt.py
+-rw-r--r--   0        0        0      171 2023-05-07 01:56:49.724092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/logging.py
+-rw-r--r--   0        0        0     3860 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/options.py
+-rw-r--r--   0        0        0     9834 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/pdf_generate.py
+-rw-r--r--   0        0        0       58 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/__init__.py
+-rw-r--r--   0        0        0       67 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/__init__.py
+-rw-r--r--   0        0        0      837 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/tabbed_block.py
+-rw-r--r--   0        0        0       67 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/__init__.py
+-rw-r--r--   0        0        0     1970 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/util.py
+-rw-r--r--   0        0        0     2482 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/prep.py
+-rw-r--r--   0        0        0     6169 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/renderer.py
+-rw-r--r--   0        0        0     3135 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/__init__.py
+-rw-r--r--   0        0        0     1294 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/_paging.css
+-rw-r--r--   0        0        0     1777 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/cover.css
+-rw-r--r--   0        0        0     1659 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/toc.css
+-rw-r--r--   0        0        0        0 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/__init__.py
+-rw-r--r--   0        0        0     1272 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/default_cover.html.j2
+-rw-r--r--   0        0        0      437 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/__init__.py
+-rw-r--r--   0        0        0      184 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/datetime.py
+-rw-r--r--   0        0        0      924 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/url.py
+-rw-r--r--   0        0        0     5038 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/template.py
+-rw-r--r--   0        0        0        0 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/__init__.py
+-rw-r--r--   0        0        0     3689 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/alabaster.py
+-rw-r--r--   0        0        0      456 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/generic.py
+-rw-r--r--   0        0        0    11433 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/immaterial_styles.css
+-rw-r--r--   0        0        0     1852 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/material_styles.css
+-rw-r--r--   0        0        0     4270 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_immaterial.py
+-rw-r--r--   0        0        0     4273 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_material.py
+-rw-r--r--   0        0        0     5841 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/toc.py
+-rw-r--r--   0        0        0     3780 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/utils.py
+-rw-r--r--   0        0        0       22 2023-05-07 01:56:49.728092 sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/version.py
+-rw-r--r--   0        0        0     7469 1970-01-01 00:00:00.000000 sphinx_pdf_generate-0.0.2/PKG-INFO
```

### Comparing `sphinx_pdf_generate-0.0.1/LICENSE.md` & `sphinx_pdf_generate-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/README.rst` & `sphinx_pdf_generate-0.0.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -22,14 +22,36 @@
 
 .. |sphinx-immaterial| replace:: Sphinx-Immaterial
 
 .. _contributing: https://isolveit.github.io/sphinx-pdf-generate/contribute.html
 
 .. |contributing| replace:: Contribution Guidelines
 
+.. image:: https://img.shields.io/pypi/dm/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: Downloads
+.. image:: https://img.shields.io/pypi/l/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: License
+.. image:: https://img.shields.io/pypi/pyversions/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: Supported versions
+.. image:: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/main.yaml
+   :alt: GitHub Docs CI Action status
+.. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/ci.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions
+   :alt: GitHub CI Action status
+.. image:: https://img.shields.io/pypi/v/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: PyPI Package latest release
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: black code style
+
 Sphinx PDF Generate
 ===================
 
 *A Sphinx extension to generate individual PDF files for each documentation page.*
 
 Sphinx-PDF-Generate extension generates separate PDF files from each HTML page derived from your Sphinx RST files page
 in your Sphinx documentation using `WeasyPrint <http://weasyprint.org/>`_.
```

### Comparing `sphinx_pdf_generate-0.0.1/pyproject.toml` & `sphinx_pdf_generate-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sphinx-pdf-generate"
 
 # !! Don't miss updates in __init__.py, and changelog.rst!!!
-version = "0.0.1"
+version = "0.0.2"
 
 description = "A Sphinx extension to generate individual PDF files for each documentation page."
 authors = ["Duodu Randy <duodurandy19@gmail.com>"]
 license = "MIT"
 maintainers = [
     "Duodu Randy <duodurandy19@gmail.com>",
 ]
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/build.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/build.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/cli.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import os
 from pathlib import Path
 from typing import Dict
 
 import colorama
 
 from .build import SPHINX_BUILD_OPTIONS, get_builder, show
-from .logging import get_logger
 from .pdf_generate import PdfGeneratePlugin
 from .version import __version__
 
 GLOBAL_OPTIONS = {}.update(
     verbose=False,
     site_url="http://127.0.0.1:8000",
     debug=False,
@@ -97,15 +96,14 @@
     parser.add_argument("outdir", help="output directory for built documentation")
     return parser
 
 
 def main() -> None:
     """Actual application logic."""
     colorama.init()
-    log = get_logger("sphinx-pdf-generate")
 
     parser = get_parser()
     args = parser.parse_args()
 
     show(context="Starting PDF Build Process")
 
     srcdir = os.path.realpath(args.sourcedir)
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/cover.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/cover.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/generate_txt.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/generate_txt.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/options.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/options.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/pdf_generate.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/pdf_generate.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/content/tabbed_block.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/content/tabbed_block.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/links/util.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/links/util.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/preprocessor/prep.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/preprocessor/prep.py`

 * *Files 11% similar despite different names*

```diff
@@ -29,15 +29,19 @@
     """
     Function to restructure HTML content by removing all unwanted parts and leaving only the content that will be
     used in converting the PDF.
 
     :param soup: HTML content
     :return: Restructured HTML content
     """
+    # support for sphinx-material & sphinx-immaterial theme
     content = soup.find("article", attrs={"class": "md-content__inner"})
+    if content is None:
+        # support for all sphinx themes
+        content = soup.find(["div", "article"], attrs={"role": "main"})
     new_content = [content]
     soup.body.clear()
     soup.body.extend(new_content)
     # Check image alignment
     all_images = soup.find_all("img", attrs={"align": re.compile(r"left|right")})
     for img in all_images:
         # Modify <img> tags
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/renderer.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import re
 import sys
 from importlib import import_module
-from importlib.util import spec_from_file_location, module_from_spec
+from importlib.util import module_from_spec, spec_from_file_location
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from bs4 import BeautifulSoup, Tag
 from weasyprint import HTML
 
 from . import cover, toc
@@ -131,15 +131,15 @@
                 )
                 pass
         try:
             return import_module(module_name, "sphinx_pdf_generate.themes")
         except ImportError as e:
             self.logger.error(
                 f"Could not load theme handler {theme} because it is not a supported theme by default: {e}",
-                file=sys.stderr
+                file=sys.stderr,
             )
             return generic_theme
 
     def _load_user_plugin_handler(self):
         custom_plugin_handler_path = self._options.user_plugin_handler_path
         module_name = ".user_plugin"
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/__init__.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/_paging.css` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/_paging.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/cover.css` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/cover.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/styles/toc.css` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/styles/toc.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/default_cover.html.j2` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/default_cover.html.j2`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/filters/url.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/filters/url.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/templates/template.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/templates/template.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/alabaster.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/alabaster.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional
 
 
 def get_stylesheet() -> Optional[str]:
-    return None
+    return ""
 
 
 def modify_html(html: str, href: str) -> str:
     svg_tag = """<svg version="1.1" xmlns="http://www.w3.org/2000/svg" style="width:40px;height:40px;" viewBox="0 0 56 
     56"> <g><path style="fill:#E9E9E0;" d="M36.985,0H7.963C7.155,0,6.5,0.655,6.5,1.926V55c0,0.345,0.655,1,1.463,
     1h40.074 c0.808,0,1.463-0.655,1.463-1V12.978c0-0.696-0.093-0.92-0.257-1.085L37.607,0.257C37.442,0.093,37.218,0,
     36.985,0z"/> <polygon style="fill:#D9D7CA;" points="37.5,0.151 37.5,12 49.349,12 	"/> <path 
@@ -34,13 +34,13 @@
     0.187-0.875,0.219C28.222,52.984,28.026,53,27.898,53h-3.814V42.924h3.035 c0.848,0,1.593,0.135,2.235,0.403s1.176,
     0.627,1.6,1.073s0.74,0.955,0.95,1.524C32.114,46.494,32.219,47.08,32.219,47.682z M27.352,51.797c1.112,0,
     1.914-0.355,2.406-1.066s0.738-1.741,0.738-3.09c0-0.419-0.05-0.834-0.15-1.244 
     c-0.101-0.41-0.294-0.781-0.581-1.114s-0.677-0.602-1.169-0.807s-1.13-0.308-1.914-0.308h-0.957v7.629H27.352z"/> 
     <path style="fill:#FFFFFF;" d="M36.266,44.168v3.172h4.211v1.121h-4.211V53h-1.668V42.924H40.9v1.244H36.266z"/> 
     </g></g> </svg>"""  # noqa: W291
 
-    a_tag = '<a style="margin:0;" href="{}" download title="Download PDF">{}</a>'.format(href, svg_tag)
+    a_tag = f'<a style="margin:0;" href="{href}" download title="Download PDF">{svg_tag}</a>'
 
     # insert into HTML
     insert_point = '<div class="document">'
     html = html.replace(insert_point, insert_point + a_tag)
     return html
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/immaterial_styles.css` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/immaterial_styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/material_styles.css` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/material_styles.css`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/sphinx_immaterial.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_immaterial.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/themes/sphinx_material.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/themes/sphinx_material.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/toc.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/toc.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from bs4 import NavigableString, Tag, BeautifulSoup, PageElement
+from bs4 import BeautifulSoup, NavigableString, PageElement, Tag
 
 from .options import Options
 
 
 def make_toc(soup: BeautifulSoup, options: Options):
     """Generate a toc tree.
 
@@ -36,17 +36,17 @@
 
     h1li = None
     h2ul = h2li = h3ul = h3li = h4ul = h4li = h5ul = h5li = h6ul = None
     # exclude_lv2 = exclude_lv3 = False
 
     def makelink(heading: PageElement) -> PageElement:
         li = soup.new_tag("li")
-        # if h.name == "h1":
-        #     return li
         ref = heading.get("id", "")
+        if ref == "":
+            ref = heading.parent.get("id")  # support for all sphinx themes
         prefix = heading.get("data-numbering", None)
         a = (
             soup.new_tag("a", href=f"#{ref}", attrs={"data-numbering": prefix})
             if prefix is not None
             else soup.new_tag("a", href=f"#{ref}")
         )
         for el in heading.contents:
```

### Comparing `sphinx_pdf_generate-0.0.1/sphinx_pdf_generate/utils.py` & `sphinx_pdf_generate-0.0.2/sphinx_pdf_generate/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_pdf_generate-0.0.1/PKG-INFO` & `sphinx_pdf_generate-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-pdf-generate
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Sphinx extension to generate individual PDF files for each documentation page.
 Home-page: https://github.com/iSOLveIT/sphinx-pdf-generate
 License: MIT
 Author: Duodu Randy
 Author-email: duodurandy19@gmail.com
 Maintainer: Duodu Randy
 Maintainer-email: duodurandy19@gmail.com
@@ -66,14 +66,36 @@
 
 .. |sphinx-immaterial| replace:: Sphinx-Immaterial
 
 .. _contributing: https://isolveit.github.io/sphinx-pdf-generate/contribute.html
 
 .. |contributing| replace:: Contribution Guidelines
 
+.. image:: https://img.shields.io/pypi/dm/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: Downloads
+.. image:: https://img.shields.io/pypi/l/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: License
+.. image:: https://img.shields.io/pypi/pyversions/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: Supported versions
+.. image:: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/workflows/main.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphnx-pdf-generate/actions/main.yaml
+   :alt: GitHub Docs CI Action status
+.. image:: https://github.com/iSOLveIT/sphinx-pdf-generate/actions/workflows/ci.yaml/badge.svg
+   :target: https://github.com/iSOLveIT/sphinx-pdf-generate/actions
+   :alt: GitHub CI Action status
+.. image:: https://img.shields.io/pypi/v/sphinx-pdf-generate.svg
+   :target: https://pypi.python.org/pypi/sphinx-pdf-generate
+   :alt: PyPI Package latest release
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+   :target: https://github.com/psf/black
+   :alt: black code style
+
 Sphinx PDF Generate
 ===================
 
 *A Sphinx extension to generate individual PDF files for each documentation page.*
 
 Sphinx-PDF-Generate extension generates separate PDF files from each HTML page derived from your Sphinx RST files page
 in your Sphinx documentation using `WeasyPrint <http://weasyprint.org/>`_.
```

