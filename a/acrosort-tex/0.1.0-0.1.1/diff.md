# Comparing `tmp/acrosort_tex-0.1.0.tar.gz` & `tmp/acrosort_tex-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acrosort_tex-0.1.0.tar", max compression
+gzip compressed data, was "acrosort_tex-0.1.1.tar", max compression
```

## Comparing `acrosort_tex-0.1.0.tar` & `acrosort_tex-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       23 2023-05-07 18:44:57.123115 acrosort_tex-0.1.0/acrosort_tex/__init__.py
--rw-r--r--   0        0        0     5896 2023-05-07 19:19:21.691427 acrosort_tex-0.1.0/acrosort_tex/sorter.py
--rw-r--r--   0        0        0     1075 2023-05-07 19:13:48.202423 acrosort_tex-0.1.0/LICENSE
--rw-r--r--   0        0        0      885 2023-05-07 19:30:51.216668 acrosort_tex-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1021 2023-05-07 19:31:22.038473 acrosort_tex-0.1.0/README.md
--rw-r--r--   0        0        0     1773 2023-05-07 19:35:24.763573 acrosort_tex-0.1.0/setup.py
--rw-r--r--   0        0        0     1862 2023-05-07 19:35:24.763573 acrosort_tex-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2023-05-07 19:44:22.877485 acrosort_tex-0.1.1/acrosort_tex/__init__.py
+-rw-r--r--   0        0        0     5894 2023-05-07 19:43:08.130277 acrosort_tex-0.1.1/acrosort_tex/sorter.py
+-rw-r--r--   0        0        0     1075 2023-05-07 19:13:48.202423 acrosort_tex-0.1.1/LICENSE
+-rw-r--r--   0        0        0      885 2023-05-07 19:44:35.974039 acrosort_tex-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1021 2023-05-07 19:31:22.038473 acrosort_tex-0.1.1/README.md
+-rw-r--r--   0        0        0     1773 2023-05-07 19:44:58.913328 acrosort_tex-0.1.1/setup.py
+-rw-r--r--   0        0        0     1862 2023-05-07 19:44:58.913328 acrosort_tex-0.1.1/PKG-INFO
```

### Comparing `acrosort_tex-0.1.0/acrosort_tex/sorter.py` & `acrosort_tex-0.1.1/acrosort_tex/sorter.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         longest_shortform_key (str): Longest shortform key to set the width of the shortform column in the acronym block
 
     Returns:
         list: All lines with the new acronym block
     """
     new_acronym_lines = [f"\\begin{{acronym}}[{longest_shortform_key}]\n"]
     for key, (key_in_file, long_form) in sorted_acronyms:
-        new_line = f"\\acro{{{key}}}{{{key_in_file}}}{{{long_form}}}\n"
+        new_line = f"\\acro{{{key}}}[{key_in_file}]{{{long_form}}}\n"
         new_acronym_lines.append(new_line)
     new_acronym_lines.append("\\end{acronym}\n")
 
     tex_lines = (
         tex_lines[:acronym_block_start]
         + new_acronym_lines
         + tex_lines[acronym_block_end + 1 :]
```

### Comparing `acrosort_tex-0.1.0/LICENSE` & `acrosort_tex-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `acrosort_tex-0.1.0/pyproject.toml` & `acrosort_tex-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acrosort_tex"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["baniasbaabe <banias@hotmail.de>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/baniasbaabe/acrosort-tex/tree/main"
 repository = "https://github.com/baniasbaabe/acrosort-tex/tree/main"
 keywords = ["latex", "acronyms", "sorting"]
```

### Comparing `acrosort_tex-0.1.0/README.md` & `acrosort_tex-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `acrosort_tex-0.1.0/setup.py` & `acrosort_tex-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['rich>=13.3.5,<14.0.0']
 
 entry_points = \
 {'console_scripts': ['acrosort = acrosort_tex.sorter:main']}
 
 setup_kwargs = {
     'name': 'acrosort-tex',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': "# acrosort-tex\n\n`acrosort-tex` is a Python Command Line App to sort your acronyms in your `.tex` by their shortform.\n\n## Installation\n\nYou can install acrosort-tex using pip (note the underscore):\n\n```bash\npip install acrosort_tex\n```\n\n## Usage\n\nTo use `acrosort-tex`, you first need to create a `.tex` file with a list of acronyms (see in `examples` for an example file).\n\nIt doesn't matter if there are other TeX commands before or after the `acronym` block.\n\nTo sort the acronyms, run the following command:\n\n```bash\nacrosort <input_file.tex> <output_file.tex>\n```\n\nFor example:\n\n```bash\nacrosort examples/List_Of_Abbreviations.tex acronyms.tex\n```\n\nThis will create a new `.tex` file called `sorted_acronyms.tex` with the sorted acronyms, while everything else isn't touched.\n\nIt will also find the longest key to set the width of the shortform column in the acronym block.\n\n## License\n\n`acrosort_tex` is licensed under the MIT License. See the LICENSE file for more information.\n",
     'author': 'baniasbaabe',
     'author_email': 'banias@hotmail.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/baniasbaabe/acrosort-tex/tree/main',
```

### Comparing `acrosort_tex-0.1.0/PKG-INFO` & `acrosort_tex-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acrosort-tex
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Home-page: https://github.com/baniasbaabe/acrosort-tex/tree/main
 License: MIT
 Keywords: latex,acronyms,sorting
 Author: baniasbaabe
 Author-email: banias@hotmail.de
 Requires-Python: >=3.8,<4.0
```

