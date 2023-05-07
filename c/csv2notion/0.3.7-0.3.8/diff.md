# Comparing `tmp/csv2notion-0.3.7.tar.gz` & `tmp/csv2notion-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv2notion-0.3.7.tar", max compression
+gzip compressed data, was "csv2notion-0.3.8.tar", max compression
```

## Comparing `csv2notion-0.3.7.tar` & `csv2notion-0.3.8.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     7398 2022-12-06 11:31:37.806873 csv2notion-0.3.7/CHANGELOG.md
--rw-r--r--   0        0        0     1065 2022-12-06 11:31:37.806873 csv2notion-0.3.7/LICENSE
--rw-r--r--   0        0        0    17750 2022-12-06 11:31:37.806873 csv2notion-0.3.7/README.md
--rw-r--r--   0        0        0        0 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/__init__.py
--rw-r--r--   0        0        0       91 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/__main__.py
--rw-r--r--   0        0        0     2352 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/cli.py
--rw-r--r--   0        0        0    10761 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/cli_args.py
--rw-r--r--   0        0        0     2283 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/cli_steps.py
--rw-r--r--   0        0        0     3781 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/csv_data.py
--rw-r--r--   0        0        0    10710 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/notion_convert.py
--rw-r--r--   0        0        0     1867 2022-12-06 11:31:37.806873 csv2notion-0.3.7/csv2notion/notion_convert_map.py
--rw-r--r--   0        0        0     6572 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_db.py
--rw-r--r--   0        0        0     1929 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_db_client.py
--rw-r--r--   0        0        0     3089 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_db_collection.py
--rw-r--r--   0        0        0     9165 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_preparator.py
--rw-r--r--   0        0        0     8500 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_row.py
--rw-r--r--   0        0        0     3478 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_row_image_block.py
--rw-r--r--   0        0        0     2569 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_row_upload_file.py
--rw-r--r--   0        0        0      947 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_type_guess.py
--rw-r--r--   0        0        0     1527 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/notion_uploader.py
--rw-r--r--   0        0        0     1276 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_db.py
--rw-r--r--   0        0        0      305 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_exceptions.py
--rw-r--r--   0        0        0      331 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_file.py
--rw-r--r--   0        0        0      679 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_rand_id.py
--rw-r--r--   0        0        0     1712 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_static.py
--rw-r--r--   0        0        0      136 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_str.py
--rw-r--r--   0        0        0     1375 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/utils_threading.py
--rw-r--r--   0        0        0       22 2022-12-06 11:31:37.810873 csv2notion-0.3.7/csv2notion/version.py
--rw-r--r--   0        0        0     4878 2022-12-06 11:31:37.814874 csv2notion-0.3.7/pyproject.toml
--rw-r--r--   0        0        0    18997 1970-01-01 00:00:00.000000 csv2notion-0.3.7/setup.py
--rw-r--r--   0        0        0    19274 1970-01-01 00:00:00.000000 csv2notion-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     7643 2023-05-07 06:55:25.705304 csv2notion-0.3.8/CHANGELOG.md
+-rw-r--r--   0        0        0     1065 2023-05-07 06:55:25.705304 csv2notion-0.3.8/LICENSE
+-rw-r--r--   0        0        0    17750 2023-05-07 06:55:25.705304 csv2notion-0.3.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/__init__.py
+-rw-r--r--   0        0        0       91 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/__main__.py
+-rw-r--r--   0        0        0     2352 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/cli.py
+-rw-r--r--   0        0        0    10761 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/cli_args.py
+-rw-r--r--   0        0        0     2283 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/cli_steps.py
+-rw-r--r--   0        0        0     3781 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/csv_data.py
+-rw-r--r--   0        0        0    10710 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_convert.py
+-rw-r--r--   0        0        0     1867 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_convert_map.py
+-rw-r--r--   0        0        0     6572 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_db.py
+-rw-r--r--   0        0        0     1929 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_db_client.py
+-rw-r--r--   0        0        0     3089 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_db_collection.py
+-rw-r--r--   0        0        0     9165 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_preparator.py
+-rw-r--r--   0        0        0     8500 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_row.py
+-rw-r--r--   0        0        0     3478 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_row_image_block.py
+-rw-r--r--   0        0        0     2569 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_row_upload_file.py
+-rw-r--r--   0        0        0      947 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_type_guess.py
+-rw-r--r--   0        0        0     1527 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/notion_uploader.py
+-rw-r--r--   0        0        0     1276 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_db.py
+-rw-r--r--   0        0        0      305 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_exceptions.py
+-rw-r--r--   0        0        0      331 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_file.py
+-rw-r--r--   0        0        0      679 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_rand_id.py
+-rw-r--r--   0        0        0     1712 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_static.py
+-rw-r--r--   0        0        0      136 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_str.py
+-rw-r--r--   0        0        0     1375 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/utils_threading.py
+-rw-r--r--   0        0        0       22 2023-05-07 06:55:25.705304 csv2notion-0.3.8/csv2notion/version.py
+-rw-r--r--   0        0        0     4906 2023-05-07 06:55:25.713304 csv2notion-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0    19315 1970-01-01 00:00:00.000000 csv2notion-0.3.8/PKG-INFO
```

### Comparing `csv2notion-0.3.7/CHANGELOG.md` & `csv2notion-0.3.8/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+### [0.3.8](https://github.com/vzhd1701/csv2notion/compare/v0.3.7...v0.3.8) (2023-05-07)
+
+### Bug Fixes
+
+- update Notion SDK to avoid 403 error ([da15829](https://github.com/vzhd1701/csv2notion/commit/da158292c4bb01668615a2fb309966d76a6df690))
+
 ### [0.3.7](https://github.com/vzhd1701/csv2notion/compare/v0.3.6...v0.3.7) (2022-12-06)
 
 ### Bug Fixes
 
 - improve URL permission check ([c74b759](https://github.com/vzhd1701/csv2notion/commit/c74b759b895100bd6c62362eee22895ddf6b1cdc))
 - update notion SDK ([94d5d60](https://github.com/vzhd1701/csv2notion/commit/94d5d60782b5ea6b939a4b2c79d0353448595c3f))
```

### Comparing `csv2notion-0.3.7/LICENSE` & `csv2notion-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/README.md` & `csv2notion-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/cli.py` & `csv2notion-0.3.8/csv2notion/cli.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/cli_args.py` & `csv2notion-0.3.8/csv2notion/cli_args.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/cli_steps.py` & `csv2notion-0.3.8/csv2notion/cli_steps.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/csv_data.py` & `csv2notion-0.3.8/csv2notion/csv_data.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_convert.py` & `csv2notion-0.3.8/csv2notion/notion_convert.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_convert_map.py` & `csv2notion-0.3.8/csv2notion/notion_convert_map.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_db.py` & `csv2notion-0.3.8/csv2notion/notion_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_db_client.py` & `csv2notion-0.3.8/csv2notion/notion_db_client.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_db_collection.py` & `csv2notion-0.3.8/csv2notion/notion_db_collection.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_preparator.py` & `csv2notion-0.3.8/csv2notion/notion_preparator.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_row.py` & `csv2notion-0.3.8/csv2notion/notion_row.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_row_image_block.py` & `csv2notion-0.3.8/csv2notion/notion_row_image_block.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_row_upload_file.py` & `csv2notion-0.3.8/csv2notion/notion_row_upload_file.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_type_guess.py` & `csv2notion-0.3.8/csv2notion/notion_type_guess.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/notion_uploader.py` & `csv2notion-0.3.8/csv2notion/notion_uploader.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/utils_db.py` & `csv2notion-0.3.8/csv2notion/utils_db.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/utils_rand_id.py` & `csv2notion-0.3.8/csv2notion/utils_rand_id.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/utils_static.py` & `csv2notion-0.3.8/csv2notion/utils_static.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/csv2notion/utils_threading.py` & `csv2notion-0.3.8/csv2notion/utils_threading.py`

 * *Files identical despite different names*

### Comparing `csv2notion-0.3.7/pyproject.toml` & `csv2notion-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "csv2notion"
-version = "0.3.7"
+version = "0.3.8"
 description = "Import/Merge CSV files into Notion database"
 authors = ["vzhd1701 <vzhd1701@gmail.com>"]
 readme = "README.md"
 include = ["CHANGELOG.md"]
 license = "MIT"
 repository = "https://github.com/vzhd1701/csv2notion"
 keywords = ["csv", "notion", "import", "merge"]
@@ -32,15 +32,16 @@
 csv2notion = "csv2notion.cli:main"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 python-dateutil = "^2.8.2"
 tqdm = "^4.64.0"
 emoji = "^2.0.0"
-notion-vzhd1701-fork = "0.0.36"
+notion-vzhd1701-fork = "0.0.37"
+requests = ">=2.27.1,<2.29"
 types-requests = "^2.27.27"
 types-python-dateutil = "^2.8.16"
 types-emoji = "^1.2.8"
 
 [tool.poetry.group.dev.dependencies]
 mdformat = "0.7.7"
 pytest = "^7.1.2"
```

### Comparing `csv2notion-0.3.7/setup.py` & `csv2notion-0.3.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,304 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: csv2notion
+Version: 0.3.8
+Summary: Import/Merge CSV files into Notion database
+Home-page: https://github.com/vzhd1701/csv2notion
+License: MIT
+Keywords: csv,notion,import,merge
+Author: vzhd1701
+Author-email: vzhd1701@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft
+Classifier: Operating System :: Unix
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Terminals
+Classifier: Topic :: Utilities
+Requires-Dist: emoji (>=2.0.0,<3.0.0)
+Requires-Dist: notion-vzhd1701-fork (==0.0.37)
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
+Requires-Dist: requests (>=2.27.1,<2.29)
+Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Requires-Dist: types-emoji (>=1.2.8,<2.0.0)
+Requires-Dist: types-python-dateutil (>=2.8.16,<3.0.0)
+Requires-Dist: types-requests (>=2.27.27,<3.0.0)
+Project-URL: Changelog, https://github.com/vzhd1701/csv2notion/blob/master/CHANGELOG.md
+Project-URL: Repository, https://github.com/vzhd1701/csv2notion
+Description-Content-Type: text/markdown
 
-packages = \
-['csv2notion']
+# csv2notion
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://img.shields.io/pypi/v/csv2notion?label=version)](https://pypi.python.org/pypi/csv2notion)
+[![Python Version](https://img.shields.io/pypi/pyversions/csv2notion.svg)](https://pypi.org/project/csv2notion/)
+[![tests](https://github.com/vzhd1701/csv2notion/actions/workflows/test.yml/badge.svg)](https://github.com/vzhd1701/csv2notion/actions/workflows/test.yml)
+[![codecov](https://codecov.io/gh/vzhd1701/csv2notion/branch/master/graph/badge.svg)](https://codecov.io/gh/vzhd1701/csv2notion)
 
-install_requires = \
-['emoji>=2.0.0,<3.0.0',
- 'notion-vzhd1701-fork==0.0.36',
- 'python-dateutil>=2.8.2,<3.0.0',
- 'tqdm>=4.64.0,<5.0.0',
- 'types-emoji>=1.2.8,<2.0.0',
- 'types-python-dateutil>=2.8.16,<3.0.0',
- 'types-requests>=2.27.27,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['csv2notion = csv2notion.cli:main']}
-
-setup_kwargs = {
-    'name': 'csv2notion',
-    'version': '0.3.7',
-    'description': 'Import/Merge CSV files into Notion database',
-    'long_description': '# csv2notion\n\n[![PyPI version](https://img.shields.io/pypi/v/csv2notion?label=version)](https://pypi.python.org/pypi/csv2notion)\n[![Python Version](https://img.shields.io/pypi/pyversions/csv2notion.svg)](https://pypi.org/project/csv2notion/)\n[![tests](https://github.com/vzhd1701/csv2notion/actions/workflows/test.yml/badge.svg)](https://github.com/vzhd1701/csv2notion/actions/workflows/test.yml)\n[![codecov](https://codecov.io/gh/vzhd1701/csv2notion/branch/master/graph/badge.svg)](https://codecov.io/gh/vzhd1701/csv2notion)\n\nAn alternative way to import `*.csv` files to [Notion.so](https://notion.so).\n\nDue to current limitations of the official Notion SDK this tool is using the unofficial SDK by **Jamie Alexandre** [notion-py](https://github.com/jamalex/notion-py).\n\nOriginal idea belongs to [Vigneswaran Rajkumar](https://vigneswaranrajkumar.com/).\n\n### Advantages over native import\n\n- Actually merge CSV with existing database rows (not just add new ones), first column will be used as a key\n- Manually set column types instead of relying on autodetection\n- Automatically link or create new entries in relation columns based on their value\n- Upload files into "Files & media" column\n- Set icon for each row\n- Set cover or embed image for each row\n- Upload image file used for cover or icon\n- Options for validation of input data\n\n### Disadvantages over native import\n\n- Slower speed, since every row is imported separately\n  - this is mitigated by multithreaded upload\n\n## Installation\n\n### Using portable binary\n\n[**Download the latest binary release**](https://github.com/vzhd1701/csv2notion/releases/latest) for your OS.\n\n### With [Homebrew](https://brew.sh/) (Recommended for macOS)\n\n```bash\n$ brew install vzhd1701/tap/csv2notion\n```\n\n### With [PIPX](https://github.com/pypa/pipx) (Recommended for Linux & Windows)\n\n```shell\n$ pipx install csv2notion\n```\n\n### With PIP\n\n```bash\n$ pip install --user csv2notion\n```\n\n**Python 3.7 or later required.**\n\n### From source\n\nThis project uses [poetry](https://python-poetry.org/) for dependency management and packaging. You will have to install it first. See [poetry official documentation](https://python-poetry.org/docs/) for instructions.\n\n```shell\n$ git clone https://github.com/vzhd1701/csv2notion.git\n$ cd csv2notion/\n$ poetry install --no-dev\n$ poetry run csv2notion\n```\n\n## Usage\n\n```plain\n$ csv2notion --help\nusage: csv2notion [-h] --token TOKEN [--url URL] [OPTION]... FILE\n\nImport/Merge CSV file into Notion database\n\npositional arguments:\n  FILE                               CSV file to upload\n\ngeneral options:\n  --token TOKEN                      Notion token, stored in token_v2 cookie for notion.so\n  --url URL                          Notion database URL; if none is provided, will create a new database\n  --max-threads NUMBER               upload threads (default: 5)\n  --log FILE                         file to store program log\n  --verbose                          output debug information\n  --version                          show program\'s version number and exit\n  -h, --help                         show this help message and exit\n\ncolumn options:\n  --column-types TYPES               comma-separated list of column types to use for non-key columns;\n                                     if none is provided, types will be guessed from CSV values\n                                     (can also be used with --add-missing-columns flag)\n  --add-missing-columns              if columns are present in CSV but not in Notion DB, add them to Notion DB\n  --randomize-select-colors          randomize colors for added options in select and multi select columns\n\nmerge options:\n  --merge                            merge CSV with existing Notion DB rows, first column will be used as a key\n  --merge-only-column COLUMN         CSV column that should be updated on merge;\n                                     when provided, other columns will be ignored\n                                     (use multiple times for multiple columns)\n  --merge-skip-new                   skip new rows in CSV that are not already in Notion DB during merge\n\nrelations options:\n  --add-missing-relations            add missing entries into linked Notion DB\n\npage cover options:\n  --image-column COLUMN              CSV column that points to URL or image file that will be embedded for that row\n  --image-column-keep                keep image CSV column as a Notion DB column\n  --image-column-mode {cover,block}  upload image as [cover] or insert it as [block] (default: block)\n  --image-caption-column COLUMN      CSV column that points to text caption that will be added to the image block\n                                     if --image-column-mode is set to \'block\'\n  --image-caption-column-keep        keep image caption CSV column as a Notion DB column\n\npage icon options:\n  --icon-column COLUMN               CSV column that points to emoji, URL or image file\n                                     that will be used as page icon for that row\n  --icon-column-keep                 keep icon CSV column as a Notion DB column\n  --default-icon ICON                Emoji, URL or image file that will be used as page icon for every row by default\n\nvalidation options:\n  --mandatory-column COLUMN          CSV column that cannot be empty (use multiple times for multiple columns)\n  --fail-on-relation-duplicates      fail if any linked DBs in relation columns have duplicate entries;\n                                     otherwise, first entry in alphabetical order\n                                     will be treated as unique when looking up relations\n  --fail-on-duplicates               fail if Notion DB or CSV has duplicates in key column,\n                                     useful when sanitizing before merge to avoid ambiguous mapping\n  --fail-on-duplicate-csv-columns    fail if CSV has duplicate columns;\n                                     otherwise last column will be used\n  --fail-on-conversion-error         fail if any column type conversion error occurs;\n                                     otherwise errors will be replaced with empty strings\n  --fail-on-inaccessible-relations   fail if any relation column points to a Notion DB that\n                                     is not accessible to the current user;\n                                     otherwise those columns will be ignored\n  --fail-on-missing-columns          fail if columns are present in CSV but not in Notion DB;\n                                     otherwise those columns will be ignored\n  --fail-on-unsettable-columns       fail if DB has columns that don\'t support assigning value to them;\n                                     otherwise those columns will be ignored\n                                     (columns with type created_by, last_edited_by, rollup or formula)\n  --fail-on-wrong-status-values      fail if values for \'status\' columns don\'t have matching option in DB;\n                                     otherwise those values will be replaced with default status\n```\n\n### Input\n\nYou must pass a single `*.csv` file for upload. The CSV file must contain at least 2 rows. The first row will be used as a header.\n\nOptionally you can provide a URL to an existing Notion database with the `--url` option; if not provided, the tool will create a new database named after the CSV file. The URL must link [to a database view](https://github.com/vzhd1701/csv2notion/raw/master/examples/db_link.png), not a page.\n\nThe tool also requires you to provide a `token_v2` cookie for the Notion website through `--token` option. For information on how to get it, see [this article](https://vzhd1701.notion.site/Find-Your-Notion-Token-5f57951434c1414d84ac72f88226eede).\n\n**Important notice**. `token_v2` cookie provides complete access to your Notion account. Handle it with caution.\n\n### Upload speed\n\nDue to API limitations, the upload is performed one row at a time. To speed things up, this tool uses multiple parallel threads. Use the `--max-threads` option to control how fast it will go. Try not to set it too high to avoid rate limiting by the Notion server.\n\n### Duplicate CSV columns\n\nNotion does not allow the database to have multiple columns with the same name. Therefore CSV columns will be treated as unique. Only the **last** column will be used if CSV has multiple columns with the same name. If you want the program to stop if it finds duplicate columns, use the `--fail-on-duplicate-csv-columns` flag.\n\n### Missing columns\n\nIf a CSV file has columns absent from Notion DB, they will be ignored by default. Use the `--add-missing-columns` flag if you want the tool to add missing columns into Notion DB. Use the `--fail-on-missing-columns` flag if you want the program to stop if it finds a column mismatch.\n\n### Column types\n\nBy default, the tool will try to guess column types based on their content. Alternatively, you can provide a comma-separated list of column types with the `--column-types` option when creating a new database or adding new columns with the `--add-missing-columns` flag. Since the first column in Notion DB is always text, the tool will use the list to set types for the rest of the columns.\n\nBy default, new options for `select` and `multi_select` columns are added with default (gray) color. If you want the tool to randomize colors for new options, use the `--randomize-select-colors` flag.\n\nSome column types do not support assigning value to them because the database generates their content automatically. Currently these types include `created_by`, `last_edited_by`, `rollup` and `formula`. If you want the program to stop if it finds such columns in the database, use the `--fail-on-unsettable-columns` flag.\n\nIf the tool cannot convert the column value type properly, it will replace it with an empty string. If you want to make sure all values are correctly converted, use the `--fail-on-conversion-error` flag, which will stop execution in case of a conversion error.\n\nThe table below describes available codes for `--column-types` and what values are supported by each column type:\n\n<details><summary>Show table</summary>\n<p>\n\n| Column Type<br />Name   | Column Type<br />Code   | Supported Values | Multiple Values<br />(Comma Separated) |\n| ----------------------- | ----------------------- | ---------------- | -------------------------------------- |\n| **Basic**               |                         |                  |                                        |\n| Text                    | `text`                  | string           | ❌                                     |\n| Number                  | `number`                | numerical        | ❌                                     |\n| Select                  | `select`                | string           | ❌                                     |\n| Multi-select            | `multi_select`          | string           | ✔️                                     |\n| Status                  | `status`                | string           | ❌                                     |\n| Date                    | `date`                  | any date format  | ✔️ (range)                             |\n| Person                  | `person`                | username, email  | ✔️                                     |\n| Files & media           | `file`                  | file name, URL   | ✔️                                     |\n| Checkbox                | `checkbox`              | `true`, `false`  | ❌                                     |\n| URL                     | `url`                   | string           | ❌                                     |\n| Email                   | `email`                 | string           | ❌                                     |\n| Phone                   | `phone_number`          | string           | ❌                                     |\n| **Advanced**            |                         |                  |                                        |\n| Formula                 | `formula`               | `---`            | `---`                                  |\n| Relation                | `---`                   | key, Notion URL  | ✔️                                     |\n| Rollup                  | `rollup`                | `---`            | `---`                                  |\n| Created time            | `created_time`          | any date format  | ❌                                     |\n| Created by              | `created_by`            | `---`            | `---`                                  |\n| Last edited time        | `last_edited_time`      | any date format  | ❌                                     |\n| Last edited by          | `last_edited_by`        | `---`            | `---`                                  |\n\n</p>\n</details>\n\n### Merging\n\nBy default, the tool will add rows to the existing Notion DB. To merge CSV rows with the Notion database, use the `--merge` flag. The first column of CSV and Notion DB will be used as a key to update existing rows with new values. CSV rows that didn\'t have a match in Notion DB will be added as new.\n\nSince the tool treats rows as unique during merge based on the key column, it will use first found rows with a unique key. To avoid this ambiguity, you might want to validate duplicate row keys with the `--fail-on-duplicates` flag. It will check both CSV and target Notion DB before the merge.\n\nIf you want only select columns to be updated, use the `--merge-only-column` option.\n\nIf you don\'t want the tool to add any new rows not already present in the Notion DB during merge, use the `--merge-skip-new` flag.\n\n### Relation columns\n\nNotion database has a `relation` column type, which allows you to link together entries from different databases. The tool will try to match column data with keys from a linked database.\n\nBy default, it will match with the first found row; it will add nothing if it cannot find the match. Use the `--add-missing-relations` flag if you want the tool to create new entries in the linked DB if no match is found. Use the `--fail-on-conversion-error` flag if you want the program to stop if no match is found.\n\nYou can also use Notion URLs in columns of this type, and they must belong to the linked DB. The tool will not be able to add missing entries for URLs if you use the `--add-missing-columns` flag.\n\nSince the tool treats rows in the linked DB as unique you can prevent ambiguous matching with the `--fail-on-relation-duplicates` flag. It will check linked DB for duplicate keys and stop the executions if it finds any.\n\nIf linked DB is not accessible (linked DB is deleted or your account doesn\'t have access to it), columns that point to it will be ignored. If you prefer the program to stop in this case, use the `--fail-on-inaccessible-relations` flag.\n\n### Cover image / Embedded image\n\nThe tool allows you to add an image to each row with the `--image-column` option. It will use one column from CSV as a data source for the image. It can be either a URL or a file name. The file name must be either an absolute path or a path relative to the CSV file. The tool will upload the file to the Notion server.\n\nBy default, the tool will embed an image inside the row page. If you want it to use the image as a page cover, then set the `--image-column-mode` option to `cover`.\n\nColumn specified with the `--image-column` option will not be treated as a regular column by default. If you want it to appear in Notion DB, use the `--image-column-keep` flag.\n\nTo add custom caption to image block uploaded with `--image-column-mode` set to `block`, use `--image-caption-column` option. To also keep the caption as a Notion DB column, use `--image-caption-column-keep` flag.\n\n### Icon\n\nThe tool allows you to add an icon to each row with the `--icon-column` option. The behavior is the same as with `--image-column`; the only difference is that you can use URL, file name, or single emoji.\n\nTo also treat `--icon-column` as a regular column, use `--icon-column-keep` flag, similar to `--image-column-keep`.\n\nIf you want to set the same icon for each row, use the `--default-icon` option. If both `--icon-column` and `--default-icon` are present, the default icon is used if the row doesn\'t have anything in the icon column.\n\n### Mandatory columns\n\nIf you want to ensure that specific columns always have value and are not allowed to be empty, then use the `--mandatory-column` option. The program execution will stop if validation fails.\n\n## Examples\n\n- [Importing CSV into new DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/new_db.png)\n- [Using custom column types](https://github.com/vzhd1701/csv2notion/raw/master/examples/new_db_types.png)\n- [Importing CSV into existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/add_new.png)\n- [Merging CSV with existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/merge.png)\n- [Merging CSV with select columns in existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/merge_only.png)\n- [Importing rows with images](https://github.com/vzhd1701/csv2notion/raw/master/examples/image_column.png)\n- [Importing rows with emoji icons](https://github.com/vzhd1701/csv2notion/raw/master/examples/icon_column.png)\n- [Updating emoji icon only for all rows](https://github.com/vzhd1701/csv2notion/raw/master/examples/default_icon_only.png)\n\n## Getting help\n\nIf you found a bug or have a feature request, please [open a new issue](https://github.com/vzhd1701/csv2notion/issues/new/choose).\n\nIf you have a question about the program or have difficulty using it, you are welcome to [the discussions page](https://github.com/vzhd1701/csv2notion/discussions). You can also mail me directly, I\'m always happy to help.\n',
-    'author': 'vzhd1701',
-    'author_email': 'vzhd1701@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/vzhd1701/csv2notion',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
+An alternative way to import `*.csv` files to [Notion.so](https://notion.so).
 
+Due to current limitations of the official Notion SDK this tool is using the unofficial SDK by **Jamie Alexandre** [notion-py](https://github.com/jamalex/notion-py).
+
+Original idea belongs to [Vigneswaran Rajkumar](https://vigneswaranrajkumar.com/).
+
+### Advantages over native import
+
+- Actually merge CSV with existing database rows (not just add new ones), first column will be used as a key
+- Manually set column types instead of relying on autodetection
+- Automatically link or create new entries in relation columns based on their value
+- Upload files into "Files & media" column
+- Set icon for each row
+- Set cover or embed image for each row
+- Upload image file used for cover or icon
+- Options for validation of input data
+
+### Disadvantages over native import
+
+- Slower speed, since every row is imported separately
+  - this is mitigated by multithreaded upload
+
+## Installation
+
+### Using portable binary
+
+[**Download the latest binary release**](https://github.com/vzhd1701/csv2notion/releases/latest) for your OS.
+
+### With [Homebrew](https://brew.sh/) (Recommended for macOS)
+
+```bash
+$ brew install vzhd1701/tap/csv2notion
+```
+
+### With [PIPX](https://github.com/pypa/pipx) (Recommended for Linux & Windows)
+
+```shell
+$ pipx install csv2notion
+```
+
+### With PIP
+
+```bash
+$ pip install --user csv2notion
+```
+
+**Python 3.7 or later required.**
+
+### From source
+
+This project uses [poetry](https://python-poetry.org/) for dependency management and packaging. You will have to install it first. See [poetry official documentation](https://python-poetry.org/docs/) for instructions.
+
+```shell
+$ git clone https://github.com/vzhd1701/csv2notion.git
+$ cd csv2notion/
+$ poetry install --no-dev
+$ poetry run csv2notion
+```
+
+## Usage
+
+```plain
+$ csv2notion --help
+usage: csv2notion [-h] --token TOKEN [--url URL] [OPTION]... FILE
+
+Import/Merge CSV file into Notion database
+
+positional arguments:
+  FILE                               CSV file to upload
+
+general options:
+  --token TOKEN                      Notion token, stored in token_v2 cookie for notion.so
+  --url URL                          Notion database URL; if none is provided, will create a new database
+  --max-threads NUMBER               upload threads (default: 5)
+  --log FILE                         file to store program log
+  --verbose                          output debug information
+  --version                          show program's version number and exit
+  -h, --help                         show this help message and exit
+
+column options:
+  --column-types TYPES               comma-separated list of column types to use for non-key columns;
+                                     if none is provided, types will be guessed from CSV values
+                                     (can also be used with --add-missing-columns flag)
+  --add-missing-columns              if columns are present in CSV but not in Notion DB, add them to Notion DB
+  --randomize-select-colors          randomize colors for added options in select and multi select columns
+
+merge options:
+  --merge                            merge CSV with existing Notion DB rows, first column will be used as a key
+  --merge-only-column COLUMN         CSV column that should be updated on merge;
+                                     when provided, other columns will be ignored
+                                     (use multiple times for multiple columns)
+  --merge-skip-new                   skip new rows in CSV that are not already in Notion DB during merge
+
+relations options:
+  --add-missing-relations            add missing entries into linked Notion DB
+
+page cover options:
+  --image-column COLUMN              CSV column that points to URL or image file that will be embedded for that row
+  --image-column-keep                keep image CSV column as a Notion DB column
+  --image-column-mode {cover,block}  upload image as [cover] or insert it as [block] (default: block)
+  --image-caption-column COLUMN      CSV column that points to text caption that will be added to the image block
+                                     if --image-column-mode is set to 'block'
+  --image-caption-column-keep        keep image caption CSV column as a Notion DB column
+
+page icon options:
+  --icon-column COLUMN               CSV column that points to emoji, URL or image file
+                                     that will be used as page icon for that row
+  --icon-column-keep                 keep icon CSV column as a Notion DB column
+  --default-icon ICON                Emoji, URL or image file that will be used as page icon for every row by default
+
+validation options:
+  --mandatory-column COLUMN          CSV column that cannot be empty (use multiple times for multiple columns)
+  --fail-on-relation-duplicates      fail if any linked DBs in relation columns have duplicate entries;
+                                     otherwise, first entry in alphabetical order
+                                     will be treated as unique when looking up relations
+  --fail-on-duplicates               fail if Notion DB or CSV has duplicates in key column,
+                                     useful when sanitizing before merge to avoid ambiguous mapping
+  --fail-on-duplicate-csv-columns    fail if CSV has duplicate columns;
+                                     otherwise last column will be used
+  --fail-on-conversion-error         fail if any column type conversion error occurs;
+                                     otherwise errors will be replaced with empty strings
+  --fail-on-inaccessible-relations   fail if any relation column points to a Notion DB that
+                                     is not accessible to the current user;
+                                     otherwise those columns will be ignored
+  --fail-on-missing-columns          fail if columns are present in CSV but not in Notion DB;
+                                     otherwise those columns will be ignored
+  --fail-on-unsettable-columns       fail if DB has columns that don't support assigning value to them;
+                                     otherwise those columns will be ignored
+                                     (columns with type created_by, last_edited_by, rollup or formula)
+  --fail-on-wrong-status-values      fail if values for 'status' columns don't have matching option in DB;
+                                     otherwise those values will be replaced with default status
+```
+
+### Input
+
+You must pass a single `*.csv` file for upload. The CSV file must contain at least 2 rows. The first row will be used as a header.
+
+Optionally you can provide a URL to an existing Notion database with the `--url` option; if not provided, the tool will create a new database named after the CSV file. The URL must link [to a database view](https://github.com/vzhd1701/csv2notion/raw/master/examples/db_link.png), not a page.
+
+The tool also requires you to provide a `token_v2` cookie for the Notion website through `--token` option. For information on how to get it, see [this article](https://vzhd1701.notion.site/Find-Your-Notion-Token-5f57951434c1414d84ac72f88226eede).
+
+**Important notice**. `token_v2` cookie provides complete access to your Notion account. Handle it with caution.
+
+### Upload speed
+
+Due to API limitations, the upload is performed one row at a time. To speed things up, this tool uses multiple parallel threads. Use the `--max-threads` option to control how fast it will go. Try not to set it too high to avoid rate limiting by the Notion server.
+
+### Duplicate CSV columns
+
+Notion does not allow the database to have multiple columns with the same name. Therefore CSV columns will be treated as unique. Only the **last** column will be used if CSV has multiple columns with the same name. If you want the program to stop if it finds duplicate columns, use the `--fail-on-duplicate-csv-columns` flag.
+
+### Missing columns
+
+If a CSV file has columns absent from Notion DB, they will be ignored by default. Use the `--add-missing-columns` flag if you want the tool to add missing columns into Notion DB. Use the `--fail-on-missing-columns` flag if you want the program to stop if it finds a column mismatch.
+
+### Column types
+
+By default, the tool will try to guess column types based on their content. Alternatively, you can provide a comma-separated list of column types with the `--column-types` option when creating a new database or adding new columns with the `--add-missing-columns` flag. Since the first column in Notion DB is always text, the tool will use the list to set types for the rest of the columns.
+
+By default, new options for `select` and `multi_select` columns are added with default (gray) color. If you want the tool to randomize colors for new options, use the `--randomize-select-colors` flag.
+
+Some column types do not support assigning value to them because the database generates their content automatically. Currently these types include `created_by`, `last_edited_by`, `rollup` and `formula`. If you want the program to stop if it finds such columns in the database, use the `--fail-on-unsettable-columns` flag.
+
+If the tool cannot convert the column value type properly, it will replace it with an empty string. If you want to make sure all values are correctly converted, use the `--fail-on-conversion-error` flag, which will stop execution in case of a conversion error.
+
+The table below describes available codes for `--column-types` and what values are supported by each column type:
+
+<details><summary>Show table</summary>
+<p>
+
+| Column Type<br />Name   | Column Type<br />Code   | Supported Values | Multiple Values<br />(Comma Separated) |
+| ----------------------- | ----------------------- | ---------------- | -------------------------------------- |
+| **Basic**               |                         |                  |                                        |
+| Text                    | `text`                  | string           | ❌                                     |
+| Number                  | `number`                | numerical        | ❌                                     |
+| Select                  | `select`                | string           | ❌                                     |
+| Multi-select            | `multi_select`          | string           | ✔️                                     |
+| Status                  | `status`                | string           | ❌                                     |
+| Date                    | `date`                  | any date format  | ✔️ (range)                             |
+| Person                  | `person`                | username, email  | ✔️                                     |
+| Files & media           | `file`                  | file name, URL   | ✔️                                     |
+| Checkbox                | `checkbox`              | `true`, `false`  | ❌                                     |
+| URL                     | `url`                   | string           | ❌                                     |
+| Email                   | `email`                 | string           | ❌                                     |
+| Phone                   | `phone_number`          | string           | ❌                                     |
+| **Advanced**            |                         |                  |                                        |
+| Formula                 | `formula`               | `---`            | `---`                                  |
+| Relation                | `---`                   | key, Notion URL  | ✔️                                     |
+| Rollup                  | `rollup`                | `---`            | `---`                                  |
+| Created time            | `created_time`          | any date format  | ❌                                     |
+| Created by              | `created_by`            | `---`            | `---`                                  |
+| Last edited time        | `last_edited_time`      | any date format  | ❌                                     |
+| Last edited by          | `last_edited_by`        | `---`            | `---`                                  |
+
+</p>
+</details>
+
+### Merging
+
+By default, the tool will add rows to the existing Notion DB. To merge CSV rows with the Notion database, use the `--merge` flag. The first column of CSV and Notion DB will be used as a key to update existing rows with new values. CSV rows that didn't have a match in Notion DB will be added as new.
+
+Since the tool treats rows as unique during merge based on the key column, it will use first found rows with a unique key. To avoid this ambiguity, you might want to validate duplicate row keys with the `--fail-on-duplicates` flag. It will check both CSV and target Notion DB before the merge.
+
+If you want only select columns to be updated, use the `--merge-only-column` option.
+
+If you don't want the tool to add any new rows not already present in the Notion DB during merge, use the `--merge-skip-new` flag.
+
+### Relation columns
+
+Notion database has a `relation` column type, which allows you to link together entries from different databases. The tool will try to match column data with keys from a linked database.
+
+By default, it will match with the first found row; it will add nothing if it cannot find the match. Use the `--add-missing-relations` flag if you want the tool to create new entries in the linked DB if no match is found. Use the `--fail-on-conversion-error` flag if you want the program to stop if no match is found.
+
+You can also use Notion URLs in columns of this type, and they must belong to the linked DB. The tool will not be able to add missing entries for URLs if you use the `--add-missing-columns` flag.
+
+Since the tool treats rows in the linked DB as unique you can prevent ambiguous matching with the `--fail-on-relation-duplicates` flag. It will check linked DB for duplicate keys and stop the executions if it finds any.
+
+If linked DB is not accessible (linked DB is deleted or your account doesn't have access to it), columns that point to it will be ignored. If you prefer the program to stop in this case, use the `--fail-on-inaccessible-relations` flag.
+
+### Cover image / Embedded image
+
+The tool allows you to add an image to each row with the `--image-column` option. It will use one column from CSV as a data source for the image. It can be either a URL or a file name. The file name must be either an absolute path or a path relative to the CSV file. The tool will upload the file to the Notion server.
+
+By default, the tool will embed an image inside the row page. If you want it to use the image as a page cover, then set the `--image-column-mode` option to `cover`.
+
+Column specified with the `--image-column` option will not be treated as a regular column by default. If you want it to appear in Notion DB, use the `--image-column-keep` flag.
+
+To add custom caption to image block uploaded with `--image-column-mode` set to `block`, use `--image-caption-column` option. To also keep the caption as a Notion DB column, use `--image-caption-column-keep` flag.
+
+### Icon
+
+The tool allows you to add an icon to each row with the `--icon-column` option. The behavior is the same as with `--image-column`; the only difference is that you can use URL, file name, or single emoji.
+
+To also treat `--icon-column` as a regular column, use `--icon-column-keep` flag, similar to `--image-column-keep`.
+
+If you want to set the same icon for each row, use the `--default-icon` option. If both `--icon-column` and `--default-icon` are present, the default icon is used if the row doesn't have anything in the icon column.
+
+### Mandatory columns
+
+If you want to ensure that specific columns always have value and are not allowed to be empty, then use the `--mandatory-column` option. The program execution will stop if validation fails.
+
+## Examples
+
+- [Importing CSV into new DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/new_db.png)
+- [Using custom column types](https://github.com/vzhd1701/csv2notion/raw/master/examples/new_db_types.png)
+- [Importing CSV into existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/add_new.png)
+- [Merging CSV with existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/merge.png)
+- [Merging CSV with select columns in existing DB](https://github.com/vzhd1701/csv2notion/raw/master/examples/merge_only.png)
+- [Importing rows with images](https://github.com/vzhd1701/csv2notion/raw/master/examples/image_column.png)
+- [Importing rows with emoji icons](https://github.com/vzhd1701/csv2notion/raw/master/examples/icon_column.png)
+- [Updating emoji icon only for all rows](https://github.com/vzhd1701/csv2notion/raw/master/examples/default_icon_only.png)
+
+## Getting help
+
+If you found a bug or have a feature request, please [open a new issue](https://github.com/vzhd1701/csv2notion/issues/new/choose).
+
+If you have a question about the program or have difficulty using it, you are welcome to [the discussions page](https://github.com/vzhd1701/csv2notion/discussions). You can also mail me directly, I'm always happy to help.
 
-setup(**setup_kwargs)
```

