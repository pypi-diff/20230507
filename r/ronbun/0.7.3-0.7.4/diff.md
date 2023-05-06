# Comparing `tmp/ronbun-0.7.3.tar.gz` & `tmp/ronbun-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ronbun-0.7.3.tar", max compression
+gzip compressed data, was "ronbun-0.7.4.tar", max compression
```

## Comparing `ronbun-0.7.3.tar` & `ronbun-0.7.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-04 23:50:21.644329 ronbun-0.7.3/LICENSE
--rw-r--r--   0        0        0       82 2023-05-04 23:50:21.644329 ronbun-0.7.3/README.md
--rw-r--r--   0        0        0      891 2023-05-04 23:50:21.644329 ronbun-0.7.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-04 23:50:21.644329 ronbun-0.7.3/ronbun/__init__.py
--rw-r--r--   0        0        0     8671 2023-05-04 23:50:21.644329 ronbun-0.7.3/ronbun/readme.py
--rw-r--r--   0        0        0      848 1970-01-01 00:00:00.000000 ronbun-0.7.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 23:22:54.947728 ronbun-0.7.4/LICENSE
+-rw-r--r--   0        0        0       82 2023-05-06 23:22:54.947728 ronbun-0.7.4/README.md
+-rw-r--r--   0        0        0      890 2023-05-06 23:22:54.947728 ronbun-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-06 23:22:54.947728 ronbun-0.7.4/ronbun/__init__.py
+-rw-r--r--   0        0        0     9537 2023-05-06 23:22:54.947728 ronbun-0.7.4/ronbun/readme.py
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 ronbun-0.7.4/PKG-INFO
```

### Comparing `ronbun-0.7.3/LICENSE` & `ronbun-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ronbun-0.7.3/pyproject.toml` & `ronbun-0.7.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Poetry settings
 [tool.poetry]
 name = "ronbun"
 description = "The Sample Programs README Automation Tool"
-version = "0.7.3"
+version = "0.7.4"
 license = "MIT"
 
 authors = [
     "Jeremy Grifski <jeremy.grifski@therenegadecoder.com>"
 ]
 
 readme = "README.md"
@@ -17,15 +17,15 @@
    "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: MIT License"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8"
 snakemd = "^2.2.0b1"
 subete = "^0.16"
 
 [tool.poetry.group.test.dependencies]
 coverage = "^7.2"
 pytest = "^6.2"
 pytest-cov = "^2.12"
```

### Comparing `ronbun-0.7.3/ronbun/readme.py` & `ronbun-0.7.4/ronbun/readme.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 
 
 issue_url_template_base = "https://github.com/TheRenegadeCoder/sample-programs/issues/new"
 issue_url_template_query = "?assignees=&labels=enhancement,{label}&template=code-snippet-request.md&title=Add+{project}+in+{language}"
 
 
 def main():
+    """
+    The main drop in script for the README generation.
+    """
     ssl._create_default_https_context = ssl._create_unverified_context
     args = _get_args()
     numeric_level = getattr(logging, args[1].upper(), None)
     if not isinstance(numeric_level, int):
         raise ValueError(f'Invalid log level: {args[1]}')
     logging.basicConfig(level=numeric_level)
     repo = Repo(sample_programs_repo_dir=args[0])
@@ -27,14 +30,15 @@
         page.dump("README", directory=f"{args[0]}/archive/{language[0]}/{language}")
 
 
 def _get_args() -> tuple:
     """
     A helper function which gets the log level from 
     the command line. Set as warning from default. 
+
     :return: the log level provided by the user
     """
     parser = argparse.ArgumentParser()
     parser.add_argument("path")
     parser.add_argument(
         "-log",
         "--log",
@@ -45,25 +49,32 @@
         ),
     )
     options = parser.parse_args()
     return options.path, options.log
 
 
 def _get_intro_text(language: LanguageCollection) -> Paragraph:
+    """
+    Generates the test for the introduction of the README.
+
+    :param language: the language to generate from the LanguageCollection
+    :return: the introduction paragraph in the README
+    """
     paragraph = Paragraph([f"Welcome to Sample Programs in {language}! "])
     text = Inline("here.", link=language.lang_docs_url())
     if language.has_docs:
         paragraph.add(f"To find documentation related to the {language} code in this repo, look ")
         paragraph.add(text)
     return paragraph
 
 
 def _generate_program_list(language: LanguageCollection) -> list:
     """
     A helper function which generates a list of programs for the README.
+
     :param language: a language collection
     :return: a list of sample programs list items
     """
     list_items = list()
     for program in language:
         program_name = f"{program}"
         program_line = Paragraph([f":white_check_mark: {program_name} [Requirements]"]) \
@@ -72,16 +83,23 @@
         if not program.has_docs():
             program_line.replace(":white_check_mark:", ":warning:") \
                 .replace_link(program.documentation_url(), program.article_issue_query_url())
         list_items.append(program_line)
     return list_items
 
 
-def _generate_missing_program_list(language: LanguageCollection, missing_programs: list[str]):
-    list_items = list()
+def _generate_missing_program_list(language: LanguageCollection, missing_programs: list[str]) -> list[Paragraph]:
+    """
+    Generates the list of programs that are missing in Markdown.
+
+    :param language: the language with missing programs
+    :param missing_programs: the list of programs missing from the language collection
+    :return: the missing programs lines as Markdown strings
+    """
+    list_items: list[Paragraph] = list()
     missing_programs.sort(key=lambda x: x.name())
     for program in missing_programs:
         program: Project
         program_name = program.name()
         program_query = "+".join(program_name.split())
         url = issue_url_template_base + issue_url_template_query.format(
             label=program_query.lower(),
@@ -102,23 +120,30 @@
         Find out how to support this project on Github.
         """
     ])
     p.insert_link("this project", "https://github.com/TheRenegadeCoder/sample-programs-readmes")
     return p
 
 
-def _generate_program_list_header(program_count: int, total_program_count: int):
+def _generate_program_list_header(program_count: int, total_program_count: int) -> str:
+    """
+    Creates the heading test for the programs list.
+
+    :param program_count: the number of programs completed in the language
+    :param total_program_count: the total number of possible programs
+    :return: the heading about the program list
+    """
     i = int(((program_count / total_program_count) * 4))
     emojis = [":disappointed:", ":thinking:", ":relaxed:", ":smile:", ":partying_face:"]
     return f"Sample Programs List - {program_count}/{total_program_count} {emojis[i]}"
 
 
 class ReadMeCatalog:
     """
-    An representation of the collection of READMEs in the Sample Programs repo.
+    A representation of the collection of READMEs in the Sample Programs repo.
     """
 
     def __init__(self, repo: Repo):
         """
         Constructs an instance of a ReadMeCatalog.
         :param repo: a repository instance
         """
```

### Comparing `ronbun-0.7.3/PKG-INFO` & `ronbun-0.7.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 Metadata-Version: 2.1
 Name: ronbun
-Version: 0.7.3
+Version: 0.7.4
 Summary: The Sample Programs README Automation Tool
 Home-page: https://therenegadecoder.com
 License: MIT
 Author: Jeremy Grifski
 Author-email: jeremy.grifski@therenegadecoder.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: snakemd (>=2.2.0b1,<3.0.0)
 Requires-Dist: subete (>=0.16,<0.17)
 Project-URL: Repository, https://github.com/TheRenegadeCoder/sample-programs-readmes
 Description-Content-Type: text/markdown
```

