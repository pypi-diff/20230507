# Comparing `tmp/mdsplit-0.3.2.tar.gz` & `tmp/mdsplit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdsplit-0.3.2.tar", max compression
+gzip compressed data, was "mdsplit-0.4.0.tar", max compression
```

## Comparing `mdsplit-0.3.2.tar` & `mdsplit-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1070 2022-06-07 07:27:36.620744 mdsplit-0.3.2/LICENSE
--rw-r--r--   0        0        0     4154 2022-07-26 11:40:17.575114 mdsplit-0.3.2/README.md
--rwxr-xr-x   0        0        0    10478 2022-07-26 11:36:19.763789 mdsplit-0.3.2/mdsplit.py
--rw-r--r--   0        0        0      678 2022-07-26 12:12:54.018999 mdsplit-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     4864 2022-07-26 12:13:27.826875 mdsplit-0.3.2/setup.py
--rw-r--r--   0        0        0     4763 2022-07-26 12:13:27.827174 mdsplit-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-03-18 19:39:47.189090 mdsplit-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4226 2023-05-07 18:53:22.736680 mdsplit-0.4.0/README.md
+-rwxr-xr-x   0        0        0    11816 2023-05-07 18:52:01.241047 mdsplit-0.4.0/mdsplit.py
+-rw-r--r--   0        0        0      663 2023-05-07 19:03:00.946162 mdsplit-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 mdsplit-0.4.0/PKG-INFO
```

### Comparing `mdsplit-0.3.2/LICENSE` & `mdsplit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdsplit-0.3.2/README.md` & `mdsplit-0.4.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 `mdsplit` is a python command line tool to
 **split markdown files** into chapters
 **at a given [heading level](https://spec.commonmark.org/0.30/#atx-headings)**.
 
 Each chapter (or subchapter) is written to its own file,
 which is named after the heading title.
 These files are written to subdirectories representing the document's structure.
+Optionally a table of contents (`toc.md`) can be created for each input file.
 
 **Note:**
 - *Code blocks* (`` ``` ``)are detected (and headers inside ignored)
 - The output is *guaranteed to be identical* with the input
   (except for the separation into multiple files of course)
     - This means: no touching of whitespace or changing `-` to `*` of your lists
       like some viusual markdown editors tend to do
@@ -35,14 +36,20 @@
 
 Or simply download [mdsplit.py](mdsplit.py) and run it (it does not use any dependencies but python itself):
 
     python3 mdsplit.py
 
 ## Usage
 
+**Show documentation and supported arguments**:
+
+```bash
+mdsplit --help
+```
+
 **Split a file at level 1 headings**, e.g. `# This Heading`, and write results to an output folder based on the input name:
 
 ```bash
 mdsplit in.md
 ```
 
 ```mermaid
@@ -104,32 +111,33 @@
 ```
 
 ## Development (Ubuntu 22.04)
 
 Add the [deadsnakes PPA](https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa)
 and install additional python versions for testing
 
-    sudo add-apt-repository ppa:deadsnakes/ppa
-    sudo apt install python3.7 python3.7-distutils
-    sudo apt install python3.8 python3.8-distutils
-    sudo apt install python3.9 python3.9-distutils
+```bash
+sudo add-apt-repository ppa:deadsnakes/ppa
+sudo apt install python3.7 python3.7-distutils
+...
+```
 
 Install [poetry](https://python-poetry.org)
 
 Prepare virtual environment and download dependencies
 
     poetry install
 
 Run tests (for the default python version)
 
     poetry run pytest
 
 Run tests for all supported python versions
 
-    tox
+    poetry run tox
 
 Release new version
 
     poetry build
     poetry publish
 
 [Download statistics](https://pypistats.org/packages/mdsplit)
```

### Comparing `mdsplit-0.3.2/mdsplit.py` & `mdsplit-0.4.0/mdsplit.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 - The output is *guaranteed to be identical* with the input
     (except for the separation into multiple files of course).
     - This means: no touching of whitespace or changing `-` to `*` of your lists
         like some viusual markdown editors tend to do.
 - Text before the first heading is written to a file with the same name as the markdown file.
 - Chapters with the same heading name are written to the same file.
 - Only ATX headings (such as # Heading 1) are supported.
+- Optionally a table of contents (toc.md) can be created.
 """
 
 from abc import ABC, abstractmethod
 from collections import namedtuple
 from dataclasses import dataclass
 from pathlib import Path
 import argparse
@@ -28,16 +29,17 @@
 MAX_HEADING_LEVEL = 6
 DIR_SUFFIX = "_split"
 
 Chapter = namedtuple("Chapter", "parent_headings, heading, text")
 
 
 class Splitter(ABC):
-    def __init__(self, level, force, verbose):
+    def __init__(self, level, toc, force, verbose):
         self.level = level
+        self.toc = toc
         self.force = force
         self.verbose = verbose
         self.stats = Stats()
 
     @abstractmethod
     def process(self):
         pass
@@ -46,14 +48,15 @@
     def print_stats(self):
         pass
 
     def process_stream(self, in_stream, fallback_out_file_name, out_path):
         if self.verbose:
             print(f"Create output folder '{out_path}'")
 
+        toc = "# Table of Contents\n"
         self.stats.in_files += 1
         chapters = split_by_heading(in_stream, self.level)
         for chapter in chapters:
             self.stats.chapters += 1
             chapter_dir = out_path
             for parent in chapter.parent_headings:
                 chapter_dir = chapter_dir / get_valid_filename(parent)
@@ -65,25 +68,48 @@
                 else get_valid_filename(chapter.heading.heading_title) + ".md"
             )
 
             chapter_path = chapter_dir / chapter_filename
             if self.verbose:
                 print(f"Write {len(chapter.text)} lines to '{chapter_path}'")
             if not chapter_path.exists():
+                # the first time a chapter file is written
+                # (can happen multiple times for duplicate headings)
                 self.stats.new_out_files += 1
+                if self.toc:
+                    indent = len(chapter.parent_headings) * "  "
+                    title = (
+                        Splitter.remove_md_suffix(fallback_out_file_name)
+                        if chapter.heading is None
+                        else chapter.heading.heading_title
+                    )
+                    toc += f"\n{indent}- [{title}](<./{chapter_path.relative_to(out_path)}>)"
             with open(chapter_path, mode="a") as file:
                 for line in chapter.text:
                     file.write(line)
 
+        if self.toc:
+            self.stats.new_out_files += 1
+            with open(out_path / "toc.md", mode="w") as file:
+                if self.verbose:
+                    print(f"Write table of contents to {out_path / 'toc.md'}")
+                file.write(toc)
+
+    @staticmethod
+    def remove_md_suffix(filename):
+        if filename.endswith(".md"):
+            return filename[:-3]
+        return filename
+
 
 class StdinSplitter(Splitter):
     """Split content from stdin"""
 
-    def __init__(self, level, out_path, force, verbose):
-        super().__init__(level, force, verbose)
+    def __init__(self, level, toc, out_path, force, verbose):
+        super().__init__(level, toc, force, verbose)
         self.out_path = Path(DIR_SUFFIX) if out_path is None else Path(out_path)
         if self.out_path.exists():
             if self.force:
                 print(f"Warning: writing output to existing directory '{self.out_path}'")
             else:
                 raise MdSplitError(f"Output directory '{self.out_path}' already exists. Exiting..")
 
@@ -95,16 +121,16 @@
         print(f"- {self.stats.chapters} extracted chapter(s)")
         print(f"- {self.stats.new_out_files} new output file(s) ({self.out_path})")
 
 
 class PathBasedSplitter(Splitter):
     """Split a specific file or all .md files found in a directory (recursively)"""
 
-    def __init__(self, in_path, level, out_path, force, verbose):
-        super().__init__(level, force, verbose)
+    def __init__(self, in_path, level, toc, out_path, force, verbose):
+        super().__init__(level, toc, force, verbose)
         self.in_path = Path(in_path)
         if not self.in_path.exists():
             raise MdSplitError(f"Input file/directory '{self.in_path}' does not exist. Exiting..")
         elif self.in_path.is_file():
             self.out_path = Path(self.in_path.stem) if out_path is None else Path(out_path)
         else:
             self.out_path = (
@@ -270,28 +296,35 @@
         "--max-level",
         type=int,
         choices=range(1, MAX_HEADING_LEVEL + 1),
         help="maximum heading level to split, default: %(default)s",
         default=1,
     )
     parser.add_argument(
+        "-t",
+        "--table-of-contents",
+        action="store_true",
+        help="Generate a table of contents (one 'toc.md' per input file)",
+    )
+    parser.add_argument(
         "-o", "--output", default=None, help="path to output folder (must not exist)"
     )
     parser.add_argument(
         "-f",
         "--force",
         action="store_true",
         help="write into output folder even if it already exists",
     )
     parser.add_argument("-v", "--verbose", action="store_true")
     args = parser.parse_args()
 
     try:
         splitter_args = {
             "level": args.max_level,
+            "toc": args.table_of_contents,
             "out_path": args.output,
             "force": args.force,
             "verbose": args.verbose,
         }
         splitter = (
             StdinSplitter(**splitter_args)
             if args.input == "-"
```

### Comparing `mdsplit-0.3.2/pyproject.toml` & `mdsplit-0.4.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 [tool.poetry]
 name = "mdsplit"
-version = "0.3.2"
+version = "0.4.0"
 description = "Split markdown files at headings"
 readme = "README.md"
 authors = ["Markus Straub"]
 license = "MIT"
 repository = "https://github.com/markusstraub/mdsplit"
 
 [tool.poetry.scripts]
 mdsplit = "mdsplit:main"
 
 [tool.poetry.dependencies]
-python = ">=3.7"
+python = "^3.7"
 
 [tool.poetry.dev-dependencies]
-pytest = ">=7"
-pytest-console-scripts = ">=1.3"
-tox = ">=^3.25"
+pytest = "^7"
+pytest-console-scripts = "^1.3"
+tox = "^4"
 black = "*"
 flake8 = "*"
 ipykernel = "*"
 
 [tool.pytest.ini_options]
 addopts = ["-ra", "-W error"]
 testpaths = ["tests"]
 
 [tool.black]
 line-length = 100
 target-version = ['py310']
 
 [build-system]
-requires = ["poetry-core>=1.0.0"]
+requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mdsplit-0.3.2/setup.py` & `mdsplit-0.4.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,162 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mdsplit
+Version: 0.4.0
+Summary: Split markdown files at headings
+Home-page: https://github.com/markusstraub/mdsplit
+License: MIT
+Author: Markus Straub
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Repository, https://github.com/markusstraub/mdsplit
+Description-Content-Type: text/markdown
 
-modules = \
-['mdsplit']
-entry_points = \
-{'console_scripts': ['mdsplit = mdsplit:main']}
-
-setup_kwargs = {
-    'name': 'mdsplit',
-    'version': '0.3.2',
-    'description': 'Split markdown files at headings',
-    'long_description': "# mdsplit\n\n`mdsplit` is a python command line tool to\n**split markdown files** into chapters\n**at a given [heading level](https://spec.commonmark.org/0.30/#atx-headings)**.\n\nEach chapter (or subchapter) is written to its own file,\nwhich is named after the heading title.\nThese files are written to subdirectories representing the document's structure.\n\n**Note:**\n- *Code blocks* (`` ``` ``)are detected (and headers inside ignored)\n- The output is *guaranteed to be identical* with the input\n  (except for the separation into multiple files of course)\n    - This means: no touching of whitespace or changing `-` to `*` of your lists\n      like some viusual markdown editors tend to do\n- Text before the first heading is written to a file with the same name as the markdown file\n- Chapters with the same heading name are written to the same file.\n- Reading from `stdin` is supported\n- Can easily handle large files,\n  e.g. a 1 GB file is split into 30k files in 35 seconds on my 2015 Thinkpad (with an SSD)\n\n**Limitations:**\n- Only [ATX headings](https://spec.commonmark.org/0.30/#atx-headings) \n  such as `# Heading 1` are supported.\n  [Setext headings](https://spec.commonmark.org/0.30/#setext-headings)\n  (underlined headings) are not recognised.\n\n## Installation\n\nEither use pip:\n\n    pip install mdsplit\n    mdsplit\n\nOr simply download [mdsplit.py](mdsplit.py) and run it (it does not use any dependencies but python itself):\n\n    python3 mdsplit.py\n\n## Usage\n\n**Split a file at level 1 headings**, e.g. `# This Heading`, and write results to an output folder based on the input name:\n\n```bash\nmdsplit in.md\n```\n\n```mermaid\n%%{init: {'themeVariables': { 'fontFamily': 'Monospace', 'text-align': 'left'}}}%%\nflowchart LR\n    subgraph in.md\n        SRC[# Heading 1<br>lorem ipsum<br><br># HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]\n    end\n    SRC --> MDSPLIT(mdsplit in.md)\n    MDSPLIT --> SPLIT_A\n    MDSPLIT --> SPLIT_B\n    subgraph in/HeadingTwo.md\n        SPLIT_B[# HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]\n    end\n    subgraph in/Heading 1.md\n        SPLIT_A[# Heading 1<br>lorem ipsum<br><br>]\n    end\n    style SRC text-align:left\n    style SPLIT_A text-align:left\n    style SPLIT_B text-align:left\n    style MDSPLIT fill:#000,color:#0F0\n```\n\n**Split a file at level 2 headings** and higher, e.g. `# This Heading` and `## That Heading`, and write to a specific output directory:\n\n```bash\nmdsplit in.md --max-level 2 --output out\n```\n\n```mermaid\n%%{init: {'themeVariables': { 'fontFamily': 'Monospace', 'text-align': 'left'}}}%%\nflowchart LR\n    subgraph in.md\n        SRC[# Heading 1<br>lorem ipsum<br><br># HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]\n    end\n    SRC --> MDSPLIT(mdsplit in.md -l 2 -o out)\n    subgraph out/HeadingTwo/Heading 2.1.md\n        SPLIT_C[## Heading 2.1<br>consetetur sadipscing elitr]\n    end\n    subgraph out/HeadingTwo.md\n        SPLIT_B[# HeadingTwo<br>dolor sit amet<br><br>]\n    end\n    subgraph out/Heading 1.md\n        SPLIT_A[# Heading 1<br>lorem ipsum<br><br>]\n    end\n    MDSPLIT --> SPLIT_A\n    MDSPLIT --> SPLIT_B\n    MDSPLIT --> SPLIT_C\n    style SRC text-align:left\n    style SPLIT_A text-align:left\n    style SPLIT_B text-align:left\n    style MDSPLIT fill:#000,color:#0F0\n```\n\n**Split markdown from stdin**:\n\n```bash\ncat in.md | mdsplit --output out\n```\n\n## Development (Ubuntu 22.04)\n\nAdd the [deadsnakes PPA](https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa)\nand install additional python versions for testing\n\n    sudo add-apt-repository ppa:deadsnakes/ppa\n    sudo apt install python3.7 python3.7-distutils\n    sudo apt install python3.8 python3.8-distutils\n    sudo apt install python3.9 python3.9-distutils\n\nInstall [poetry](https://python-poetry.org)\n\nPrepare virtual environment and download dependencies\n\n    poetry install\n\nRun tests (for the default python version)\n\n    poetry run pytest\n\nRun tests for all supported python versions\n\n    tox\n\nRelease new version\n\n    poetry build\n    poetry publish\n\n[Download statistics](https://pypistats.org/packages/mdsplit)\n",
-    'author': 'Markus Straub',
-    'author_email': None,
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/markusstraub/mdsplit',
-    'py_modules': modules,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7',
-}
+# mdsplit
 
+`mdsplit` is a python command line tool to
+**split markdown files** into chapters
+**at a given [heading level](https://spec.commonmark.org/0.30/#atx-headings)**.
+
+Each chapter (or subchapter) is written to its own file,
+which is named after the heading title.
+These files are written to subdirectories representing the document's structure.
+Optionally a table of contents (`toc.md`) can be created for each input file.
+
+**Note:**
+- *Code blocks* (`` ``` ``)are detected (and headers inside ignored)
+- The output is *guaranteed to be identical* with the input
+  (except for the separation into multiple files of course)
+    - This means: no touching of whitespace or changing `-` to `*` of your lists
+      like some viusual markdown editors tend to do
+- Text before the first heading is written to a file with the same name as the markdown file
+- Chapters with the same heading name are written to the same file.
+- Reading from `stdin` is supported
+- Can easily handle large files,
+  e.g. a 1 GB file is split into 30k files in 35 seconds on my 2015 Thinkpad (with an SSD)
+
+**Limitations:**
+- Only [ATX headings](https://spec.commonmark.org/0.30/#atx-headings) 
+  such as `# Heading 1` are supported.
+  [Setext headings](https://spec.commonmark.org/0.30/#setext-headings)
+  (underlined headings) are not recognised.
+
+## Installation
+
+Either use pip:
+
+    pip install mdsplit
+    mdsplit
+
+Or simply download [mdsplit.py](mdsplit.py) and run it (it does not use any dependencies but python itself):
+
+    python3 mdsplit.py
+
+## Usage
+
+**Show documentation and supported arguments**:
+
+```bash
+mdsplit --help
+```
+
+**Split a file at level 1 headings**, e.g. `# This Heading`, and write results to an output folder based on the input name:
+
+```bash
+mdsplit in.md
+```
+
+```mermaid
+%%{init: {'themeVariables': { 'fontFamily': 'Monospace', 'text-align': 'left'}}}%%
+flowchart LR
+    subgraph in.md
+        SRC[# Heading 1<br>lorem ipsum<br><br># HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]
+    end
+    SRC --> MDSPLIT(mdsplit in.md)
+    MDSPLIT --> SPLIT_A
+    MDSPLIT --> SPLIT_B
+    subgraph in/HeadingTwo.md
+        SPLIT_B[# HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]
+    end
+    subgraph in/Heading 1.md
+        SPLIT_A[# Heading 1<br>lorem ipsum<br><br>]
+    end
+    style SRC text-align:left
+    style SPLIT_A text-align:left
+    style SPLIT_B text-align:left
+    style MDSPLIT fill:#000,color:#0F0
+```
+
+**Split a file at level 2 headings** and higher, e.g. `# This Heading` and `## That Heading`, and write to a specific output directory:
+
+```bash
+mdsplit in.md --max-level 2 --output out
+```
+
+```mermaid
+%%{init: {'themeVariables': { 'fontFamily': 'Monospace', 'text-align': 'left'}}}%%
+flowchart LR
+    subgraph in.md
+        SRC[# Heading 1<br>lorem ipsum<br><br># HeadingTwo<br>dolor sit amet<br><br>## Heading 2.1<br>consetetur sadipscing elitr]
+    end
+    SRC --> MDSPLIT(mdsplit in.md -l 2 -o out)
+    subgraph out/HeadingTwo/Heading 2.1.md
+        SPLIT_C[## Heading 2.1<br>consetetur sadipscing elitr]
+    end
+    subgraph out/HeadingTwo.md
+        SPLIT_B[# HeadingTwo<br>dolor sit amet<br><br>]
+    end
+    subgraph out/Heading 1.md
+        SPLIT_A[# Heading 1<br>lorem ipsum<br><br>]
+    end
+    MDSPLIT --> SPLIT_A
+    MDSPLIT --> SPLIT_B
+    MDSPLIT --> SPLIT_C
+    style SRC text-align:left
+    style SPLIT_A text-align:left
+    style SPLIT_B text-align:left
+    style MDSPLIT fill:#000,color:#0F0
+```
+
+**Split markdown from stdin**:
+
+```bash
+cat in.md | mdsplit --output out
+```
+
+## Development (Ubuntu 22.04)
+
+Add the [deadsnakes PPA](https://launchpad.net/~deadsnakes/+archive/ubuntu/ppa)
+and install additional python versions for testing
+
+```bash
+sudo add-apt-repository ppa:deadsnakes/ppa
+sudo apt install python3.7 python3.7-distutils
+...
+```
+
+Install [poetry](https://python-poetry.org)
+
+Prepare virtual environment and download dependencies
+
+    poetry install
+
+Run tests (for the default python version)
+
+    poetry run pytest
+
+Run tests for all supported python versions
+
+    poetry run tox
+
+Release new version
+
+    poetry build
+    poetry publish
+
+[Download statistics](https://pypistats.org/packages/mdsplit)
 
-setup(**setup_kwargs)
```

