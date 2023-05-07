# Comparing `tmp/yamdog-0.4.0.14.tar.gz` & `tmp/yamdog-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamdog-0.4.0.14.tar", last modified: Sat Feb  4 09:51:19 2023, max compression
+gzip compressed data, was "yamdog-0.5.0.tar", last modified: Sun May  7 18:40:30 2023, max compression
```

## Comparing `yamdog-0.4.0.14.tar` & `yamdog-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-04 09:51:19.450098 yamdog-0.4.0.14/
--rw-rw-rw-   0        0        0     1085 2022-12-28 18:45:03.000000 yamdog-0.4.0.14/LICENSE.txt
--rw-rw-rw-   0        0        0    21456 2023-02-04 09:51:19.450098 yamdog-0.4.0.14/PKG-INFO
--rw-rw-rw-   0        0        0    20492 2023-02-04 09:51:05.000000 yamdog-0.4.0.14/README.md
--rw-rw-rw-   0        0        0     1250 2023-02-04 09:51:05.000000 yamdog-0.4.0.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-02-04 09:51:19.450098 yamdog-0.4.0.14/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-02-04 09:51:19.418099 yamdog-0.4.0.14/src/
-drwxrwxrwx   0        0        0        0 2023-02-04 09:51:19.448099 yamdog-0.4.0.14/src/YAMDOG.egg-info/
--rw-rw-rw-   0        0        0    21456 2023-02-04 09:51:19.000000 yamdog-0.4.0.14/src/YAMDOG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2023-02-04 09:51:19.000000 yamdog-0.4.0.14/src/YAMDOG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-04 09:51:19.000000 yamdog-0.4.0.14/src/YAMDOG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-02-04 09:51:19.000000 yamdog-0.4.0.14/src/YAMDOG.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-02-04 09:51:19.000000 yamdog-0.4.0.14/src/YAMDOG.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-04 09:51:19.442098 yamdog-0.4.0.14/src/yamdog/
--rw-rw-rw-   0        0        0    39939 2023-02-04 09:43:44.000000 yamdog-0.4.0.14/src/yamdog/API.py
--rw-rw-rw-   0        0        0       41 2023-01-15 12:06:23.000000 yamdog-0.4.0.14/src/yamdog/__init__.py
--rw-rw-rw-   0        0        0        0 2023-01-07 19:42:23.000000 yamdog-0.4.0.14/src/yamdog/__main__.py
--rw-rw-rw-   0        0        0     6656 2023-01-23 17:46:37.000000 yamdog-0.4.0.14/src/yamdog/dataclass_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:40:30.744002 yamdog-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-07 18:39:59.000000 yamdog-0.5.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-05-07 18:40:30.744002 yamdog-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21618 2023-05-07 18:40:27.000000 yamdog-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:39:59.000000 yamdog-0.5.0/dependencies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-07 18:39:59.000000 yamdog-0.5.0/dependencies_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-07 18:40:27.000000 yamdog-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:40:30.744002 yamdog-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:40:30.740002 yamdog-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:40:30.744002 yamdog-0.5.0/src/yamdog/
+-rw-r--r--   0 runner    (1001) docker     (123)    54794 2023-05-07 18:39:59.000000 yamdog-0.5.0/src/yamdog/_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 18:39:59.000000 yamdog-0.5.0/src/yamdog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-07 18:39:59.000000 yamdog-0.5.0/src/yamdog/dataclass_validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:40:30.744002 yamdog-0.5.0/src/yamdog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    22531 2023-05-07 18:40:30.000000 yamdog-0.5.0/src/yamdog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-07 18:40:30.000000 yamdog-0.5.0/src/yamdog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:40:30.000000 yamdog-0.5.0/src/yamdog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-07 18:40:30.000000 yamdog-0.5.0/src/yamdog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 18:40:30.000000 yamdog-0.5.0/src/yamdog.egg-info/top_level.txt
```

### Comparing `yamdog-0.4.0.14/LICENSE.txt` & `yamdog-0.5.0/LICENSE.txt`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Limespy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Limespy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `yamdog-0.4.0.14/PKG-INFO` & `yamdog-0.5.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,815 +1,829 @@
-Metadata-Version: 2.1
-Name: yamdog
-Version: 0.4.0.14
-Summary: Yet Another Markdown Only Generator
-Author: Limespy
-License: MIT License
-Project-URL: Homepage, https://github.com/Limespy/yamdog
-Project-URL: Changelog, https://github.com/Limespy/yamdog/blob/main/README.md#Changelog
-Project-URL: Issue Tracker, https://github.com/Limespy/yamdog/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# Overview of YAMDOG <!-- omit in toc -->
-
-[![PyPI Package latest release](https://img.shields.io/pypi/v/yamdog.svg)][1]
-[![PyPI Wheel](https://img.shields.io/pypi/wheel/yamdog.svg)][1]
-[![Supported versions](https://img.shields.io/pypi/pyversions/yamdog.svg)][1]
-[![Supported implementations](https://img.shields.io/pypi/implementation/yamdog.svg)][1]
-
-Yet Another Markdown Only Generator
-
-## What is YAMDOG? <!-- omit in toc -->
-
-YAMDOG is toolkit for creating Markdown text using Python. Markdown is a light and relatively simple markup language.
-
-### Table of Content <!-- omit in toc -->
-
-- [Quick start guide](#quick-start-guide)
-    - [The first steps](#the-first-steps)
-        - [Install](#install)
-        - [Import](#import)
-    - [Using the package](#using-the-package)
-        - [Making elements](#making-elements)
-            - [Heading](#heading)
-            - [Example heading](#example-heading)
-            - [Paragraph](#paragraph)
-            - [Table](#table)
-            - [Compact table](#compact-table)
-            - [Listing](#listing)
-            - [Checklist](#checklist)
-            - [Link](#link)
-            - [Codeblock](#codeblock)
-            - [Code](#code)
-            - [Address](#address)
-            - [Quote block](#quote-block)
-        - [Combining elements into a document](#combining-elements-into-a-document)
-            - [Example heading](#example-heading1)
-- [Changelog](#changelog)
-- [Further reading](#further-reading)
-- [Annexes](#annexes)
-    - [Annex 1: README Python source](#annex-1-readme-python-source)
-
-# Quick start guide
-
-Here's how you can start automatically generating Markdown documents
-
-## The first steps
-
-
-
-### Install
-
-Install YAMDOG with pip. YAMDOG uses only Python standard library so it has no additional dependencies.
-
-```
-pip install yamdog
-```
-
-### Import
-
-Import name is the same as install name, yamdog.
-
-```python
-import yamdog
-```
-
-Since the package is accessed often, I use abbreviation`md` for MarkDown. The abbreviation is used throughout this document.
-
-```python
-import yamdog as md
-```
-
-## Using the package
-
-There are two main things to building a Markdown document using YAMDOG
-
-1. Making elements
-2. Combining elements into a document
-
-You can call `str` on the element directly to get the markdown source
-
-```python
-markdown_source = str(element)
-```
-
-but most of the time you will compose the elements together into an document
-
-```python
-markdown_source = str(document)
-```
-
-### Making elements
-
-Let's start with an empty document
-
-```python
-document = md.Document()
-```
-
-#### Heading
-
-*Python source*
-
-```python
-heading = md.Heading(4, 'Example heading')
-```
-
-*Markdown source*
-
-```markdown
-#### Example heading
-```
-
-*Rendered result*
-
-#### Example heading
-
----
-
-**bolded text**
-
-*some italiced text*
-
-~~striken text~~
-
-==highlighted text==
-
-==*~~**All styles combined**~~*==
-
-```python
-bold_text = md.Text('bolded text', {md.BOLD})
-italiced_text = md.Text('some italiced text', {md.ITALIC})
-strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
-highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
-all_together = md.Text('All styles combined',
-                               {md.BOLD, md.ITALIC,
-                                md.STRIKETHROUGH, md.HIGHLIGHT})
-```
-
----
-
-#### Paragraph
-
-*Python source*
-
-```python
-paragraph = md.Paragraph(['Example paragraph containing ',
-                          md.Text('bolded text', {md.BOLD})])
-```
-
-*Markdown source*
-
-```markdown
-Example paragraph containing **bolded text**
-```
-
-*Rendered result*
-
-Example paragraph containing **bolded text**
-
----
-
-#### Table
-
-*Python source*
-
-```python
-table = md.Table(['First column', 'Second column', 'Third column'],
-                 [['a', 1, 'Python'],
-                  ['b', 2, 'Markdown']],
-                 [md.RIGHT, md.LEFT, md.CENTER])
-```
-
-*Markdown source*
-
-```markdown
-| First column | Second column | Third column |
-| -----------: | :------------ | :----------: |
-|            a | 1             |    Python    |
-|            b | 2             |   Markdown   |
-```
-
-*Rendered result*
-
-| First column | Second column | Third column |
-| -----------: | :------------ | :----------: |
-|            a | 1             |    Python    |
-|            b | 2             |   Markdown   |
-
----
-
-You can select compact mode at the table object creation
-
-#### Compact table
-
-*Python source*
-
-```python
-table = md.Table(['First column', 'Second column', 'Third column'],
-                 [['a', 1, 'Python'],
-                  ['b', 2, 'Markdown']],
-                 [md.RIGHT, md.LEFT, md.CENTER],
-                 True)
-```
-
-*Markdown source*
-
-```markdown
-First column|Second column|Third column
---:|:--|:-:
-a|1|Python
-b|2|Markdown
-```
-
-*Rendered result*
-
-First column|Second column|Third column
---:|:--|:-:
-a|1|Python
-b|2|Markdown
-
----
-
-or later by changing the attribute `compact`
-
-```python
-table.compact = True
-```
-
-#### Listing
-
-*Python source*
-
-```python
-listing = md.Listing(md.UNORDERED, 
-                     ['Just normal text',
-                      md.Text('some stylised text', {md.ITALIC}),
-                      md.Checkbox(False, 'Listings can include checkboxes'),
-                      md.Checkbox(True, 'Checked and unchecked option available'),
-                      ('Sublist by using a tuple',
-                        md.Listing(md.ORDERED,
-                                  ['first', 'second']))])
-```
-
-*Markdown source*
-
-```markdown
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-```
-
-*Rendered result*
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-
----
-
-#### Checklist
-
-*Python source*
-
-```python
-checklist = md.make_checklist([(False, 'unchecked box'),
-                               (True, 'checked box'),
-                               (True, 'done')])
-```
-
-*Markdown source*
-
-```markdown
-
-```
-
-*Rendered result*
-
-
-
----
-
-#### Link
-
-*Python source*
-
-```python
-link = md.Link('Link to Markdown Guide', 'https://www.markdownguide.org')
-```
-
-*Markdown source*
-
-```markdown
-[Link to Markdown Guide](https://www.markdownguide.org)
-```
-
-*Rendered result*
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
----
-
-#### Codeblock
-
-*Python source*
-
-```python
-codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document()',
-                         'python')
-```
-
-*Markdown source*
-
-````markdown
-```python
-import yamdog as md
-
-doc = md.Document()
-```
-````
-
-*Rendered result*
-
-```python
-import yamdog as md
-
-doc = md.Document()
-```
-
----
-
-#### Code
-
-*Python source*
-
-```python
-code = md.Code('python != markdown')
-```
-
-*Markdown source*
-
-```markdown
-`python != markdown`
-```
-
-*Rendered result*
-
-`python != markdown`
-
----
-
-#### Address
-
-*Python source*
-
-```python
-address = md.Address('https://www.markdownguide.org')
-```
-
-*Markdown source*
-
-```markdown
-<https://www.markdownguide.org>
-```
-
-*Rendered result*
-
-<https://www.markdownguide.org>
-
----
-
-#### Quote block
-
-*Python source*
-
-```python
-quoteblock = md.QuoteBlock('Quote block supports\nmultiple lines')
-```
-
-*Markdown source*
-
-```markdown
-> Quote block supports
-> multiple lines
-```
-
-*Rendered result*
-
-> Quote block supports
-> multiple lines
-
----
-
-### Combining elements into a document
-
-Initialising Document with list of elements
-
-```python
-document = md.Document([heading, link, paragraph, listing])
-```
-
-adding elements into a document
-
-```python
-document = md.Document()
-document += heading
-document += link
-document += paragraph
-document += listing
-```
-
-adding elements together into a document
-
-```python
-document = heading + link + paragraph + listing
-```
-
-Adding two documents together
-
-```python
-document1 = md.Document([heading, link])
-document2 = md.Document([paragraph, listing])
-document = document1 + document2
-```
-
-*Markdown source*
-
-```markdown
-#### Example heading
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
-Example paragraph containing **bolded text**
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-```
-
-*Rendered result*
-
-#### Example heading
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
-Example paragraph containing **bolded text**
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-
-# Changelog
-
-## 0.4.0 2023-01-23 <!-- omit in toc -->
-
-- Much better type validation
-- Some comparisons
-
-## 0.3.1 2023-01-23 <!-- omit in toc -->
-
-- Preliminary type validation
-- Full test coverage
-
-# Further reading
-
-- [basic syntax][2]
-- [extended syntax][2]
-
----
-
-# Annexes
-
-## Annex 1: README Python source
-
-And here the full source code that wrote this README. This can serve as a more advanced example of what this is capable of.
-
-[The python file can also be found here](https://github.com/Limespy/YAMDOG/blob/main/readme.py)
-
-```python
-import yamdog as md
-
-import pathlib
-import re
-
-def make_examples(source: str) -> md.Document:
-    '''Examples are collected via source code introspection'''
-    # First getting the example code blocks
-    pattern = re.compile('\n    #%% ')
-    examples = {}
-    for block in pattern.split(source)[1:]:
-        name, rest = block.split('\n', 1) # from the comment
-        code = rest.split('\n\n', 1)[0].replace('\n    ', '\n').strip()
-        examples[name.strip()] = md.CodeBlock(code, 'python')
-
-    def get_example(title: str, element: md.Element) -> md.Document:
-        return md.Document([md.Heading(4, title.capitalize()),
-                            md.Text('Python source', {md.ITALIC}),
-                            examples[title],
-                            md.Text('Markdown source', {md.ITALIC}),
-                            md.CodeBlock(element, 'markdown'),
-                            md.Text('Rendered result', {md.ITALIC}),
-                            element,
-                            md.HRule()])
-
-    # Starting the actual doc
-    doc = md.Document([
-        md.Heading(3, 'Making elements'),
-
-    ])
-
-    #%% document
-    document = md.Document()
-
-    doc += "Let's start with an empty document"
-    doc += examples['document']
-
-    #%% adding to document
-    # document += 
-
-    #%% heading
-    heading = md.Heading(4, 'Example heading')
-
-    doc += get_example('heading', heading)
-
-    #%% stylised
-    bold_text = md.Text('bolded text', {md.BOLD})
-    italiced_text = md.Text('some italiced text', {md.ITALIC})
-    strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
-    highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
-    all_together = md.Text('All styles combined',
-                                   {md.BOLD, md.ITALIC,
-                                    md.STRIKETHROUGH, md.HIGHLIGHT})
-
-    doc += bold_text
-    doc += italiced_text
-    doc += strikethrough_text
-    doc += highlighted_text
-    doc += all_together
-    doc += examples['stylised']
-    doc += md.HRule()
-
-    #%%  paragraph
-    paragraph = md.Paragraph(['Example paragraph containing ',
-                              md.Text('bolded text', {md.BOLD})])
-
-    doc += get_example('paragraph', paragraph)
-
-    #%% table
-    table = md.Table(['First column', 'Second column', 'Third column'],
-                     [['a', 1, 'Python'],
-                      ['b', 2, 'Markdown']],
-                     [md.RIGHT, md.LEFT, md.CENTER])
-
-    doc += get_example('table', table)
-
-    #%% compact table
-    table = md.Table(['First column', 'Second column', 'Third column'],
-                     [['a', 1, 'Python'],
-                      ['b', 2, 'Markdown']],
-                     [md.RIGHT, md.LEFT, md.CENTER],
-                     True)
-
-    doc += 'You can select compact mode at the table object creation'
-    doc += get_example('compact table', table)
-
-    #%% table compact attribute
-    table.compact = True
-
-    doc += md.Paragraph(['or later by changing the attribute ',
-                         md.Code('compact')])
-    doc += examples['table compact attribute']
-
-    #%% listing
-    listing = md.Listing(md.UNORDERED, 
-                         ['Just normal text',
-                          md.Text('some stylised text', {md.ITALIC}),
-                          md.Checkbox(False, 'Listings can include checkboxes'),
-                          md.Checkbox(True, 'Checked and unchecked option available'),
-                          ('Sublist by using a tuple',
-                            md.Listing(md.ORDERED,
-                                      ['first', 'second']))])
-
-    doc += get_example('listing', listing)
-
-    #%% checklist
-    checklist = md.make_checklist([(False, 'unchecked box'),
-                                   (True, 'checked box'),
-                                   (True, 'done')])
-
-    doc += get_example('checklist', checklist)
-    #%% link
-    link = md.Link('Link to Markdown Guide', 'https://www.markdownguide.org')
-
-    doc += get_example('link', link)
-
-    #%% codeblock
-    codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document()',
-                             'python')
-
-    doc += get_example('codeblock', codeblock)
-
-    #%% code
-    code = md.Code('python != markdown')
-
-    doc += get_example('code', code)
-
-    #%% Image
-    # image = md.Image()
-
-    #%% address
-    address = md.Address('https://www.markdownguide.org')
-
-    doc += get_example('address', address)
-
-    #%% quote block
-    quoteblock = md.QuoteBlock('Quote block supports\nmultiple lines')
-
-    doc += get_example('quote block', quoteblock)
-
-    doc += md.Heading(3, 'Combining elements into a document')
-
-    #%% calling document
-    document = md.Document([heading, link, paragraph, listing])
-
-    doc += 'Initialising Document with list of elements'
-    doc += examples['calling document']
-
-    #%% from empty document
-    document = md.Document()
-    document += heading
-    document += link
-    document += paragraph
-    document += listing
-
-    doc += 'adding elements into a document'
-    doc += examples['from empty document']
-
-    #%% document by adding
-    document = heading + link + paragraph + listing
-
-    doc += 'adding elements together into a document'
-    doc += examples['document by adding']
-
-    #%% document concatenation
-    document1 = md.Document([heading, link])
-    document2 = md.Document([paragraph, listing])
-    document = document1 + document2
-
-    doc += 'Adding two documents together'
-    doc += examples['document concatenation']
-
-    doc += md.Text('Markdown source', {md.ITALIC})
-    doc += md.CodeBlock(document, 'markdown')
-    doc += md.Text('Rendered result', {md.ITALIC})
-    doc += document
-
-    return doc
-
-def make_quick_start_guide(name, pypiname, source):
-    doc = md.Document([
-        md.Heading(1, 'Quick start guide'),
-        "Here's how you can start automatically generating Markdown documents",
-        md.Heading(2, 'The first steps'),
-        '',
-        md.Heading(3, 'Install'),
-        f'''Install {name} with pip.
-        {name} uses only Python standard library so it has no additional dependencies.''',
-        md.CodeBlock(f'pip install {pypiname}'),
-        md.Heading(3, 'Import'),
-        f'''Import name is the same as install name, {pypiname}.''',
-        md.CodeBlock(f'import {pypiname}', 'python'),
-        md.Paragraph(['Since the package is accessed often, I use abbreviation',
-                      md.Code('md'), 
-                      ' for MarkDown. The abbreviation is used throughout this document.']),
-        md.CodeBlock(f'import {pypiname} as md', 'python'),
-        md.Heading(2, 'Using the package'),
-        f'There are two main things to building a Markdown document using {name}',
-        md.Listing(md.ORDERED, ['Making elements',
-                               'Combining elements into a document']),
-        md.Paragraph(['You can call ',
-            md.Code('str'),
-            ' on the element directly to get the markdown source']),
-        md.CodeBlock('markdown_source = str(element)', 'python'),
-        '''but most of the time you will compose the elements together into an
-        document''',
-        md.CodeBlock('markdown_source = str(document)', 'python')
-        ])
-    doc += make_examples(source)
-    return doc
-
-
-def make_changelog():
-    doc = md.Document([md.Heading(1, 'Changelog')])
-
-    changelog = (('0.4.0', '2023-01-23', ['Much better type validation',
-                                          'Some comparisons']),
-                 ('0.3.1', '2023-01-23', ['Preliminary type validation',
-                                          'Full test coverage'])
-                 )
-
-    for version, date, changes in changelog:
-        doc += md.Heading(2, f'{version} {date}', in_TOC = False)
-        doc += md.Listing(md.UNORDERED, changes)
-
-    return doc
-
-def make_further_reading():
-    basic_syntax_link = md.Link('basic syntax',
-                                'https://www.markdownguide.org/basic-syntax/',
-                                '')
-    extended_syntax_link = md.Link('extended syntax',
-                                  'https://www.markdownguide.org/basic-syntax/',
-                                   '')
-
-    doc = md.Document([md.Heading(1, 'Further reading')])
-    doc += md.Listing(md.UNORDERED, [basic_syntax_link, extended_syntax_link])
-    return doc
-
-def make_annexes(source):
-    doc = md.Document([md.Heading(1, 'Annexes')])
-    doc += md.Heading(2, 'Annex 1: README Python source')
-    doc += '''And here the full source code that wrote this README.
-            This can serve as a more advanced example of what this is
-            capable of.'''
-    doc += md.Link('The python file can also be found here',
-                   'https://github.com/Limespy/YAMDOG/blob/main/readme.py')
-    doc += md.CodeBlock(source, 'python')
-    return doc
-
-def make_readme(name, pypiname, source):
-    # Setup for the badges
-    shields_url = 'https://img.shields.io/'
-
-    pypi_project_url = f'https://pypi.org/project/{pypiname}'
-    pypi_badge_info = (('v', 'PyPI Package latest release'),
-                       ('wheel', 'PyPI Wheel'),
-                       ('pyversions', 'Supported versions'),
-                       ('implementation', 'Supported implementations'))
-    pypi_badges = [md.Link(md.Image(f'{shields_url}pypi/{code}/{pypiname}.svg',
-                                    desc), pypi_project_url, '')
-                   for code, desc in pypi_badge_info]
-
-    # Starting the document
-    doc = md.Document([
-        md.Heading(1, f'Overview of {name}', in_TOC = False),
-        md.Paragraph(pypi_badges, '\n'),
-        'Yet Another Markdown Only Generator',
-        md.Heading(2, f'What is {name}?', in_TOC = False),
-        f'''{name} is toolkit for creating Markdown text using Python.
-        Markdown is a light and relatively simple markup language.''',
-        md.Heading(3, 'Table of Content', in_TOC = False),
-        md.TOC()
-        ])
-    doc += make_quick_start_guide(name, pypiname, source)
-    doc += make_changelog()
-    doc += make_further_reading()
-    doc += md.HRule()
-    doc += make_annexes(source)
-    return doc
-
-def main():
-    name = 'YAMDOG'
-    pypiname = 'yamdog'
-
-    source = pathlib.Path(__file__).read_text('utf8')
-
-    doc = make_readme(name, pypiname, source)
-
-    (pathlib.Path(__file__).parent / 'README.md').write_text(str(doc), 'utf8')
-    return doc
-
-if __name__ == '__main__':
-    main()
-```
-
-[1]: <https://pypi.org/project/yamdog> ""
-[2]: <https://www.markdownguide.org/basic-syntax/> ""
+# Overview of YAMDOG <!-- omit in toc -->
+
+[![PyPI Package latest release](https://img.shields.io/pypi/v/yamdog.svg)][1]
+[![PyPI Wheel](https://img.shields.io/pypi/wheel/yamdog.svg)][1]
+[![Supported versions](https://img.shields.io/pypi/pyversions/yamdog.svg)][1]
+[![Supported implementations](https://img.shields.io/pypi/implementation/yamdog.svg)][1]
+
+Yet Another Markdown Only Generator
+
+## What is YAMDOG? <!-- omit in toc -->
+
+YAMDOG is toolkit for creating Markdown text using Python. Markdown is a light and relatively simple markup language.
+
+### Table of Content <!-- omit in toc -->
+
+- [Quick start guide](#quick-start-guide)
+    - [The first steps](#the-first-steps)
+        - [Install](#install)
+        - [Import](#import)
+    - [Using the package](#using-the-package)
+        - [Making elements](#making-elements)
+            - [Heading](#heading)
+            - [Example heading](#example-heading)
+            - [Paragraph](#paragraph)
+            - [Table](#table)
+            - [Compact table](#compact-table)
+            - [Listing](#listing)
+            - [Checklist](#checklist)
+            - [Link](#link)
+            - [Codeblock](#codeblock)
+            - [Code](#code)
+            - [Address](#address)
+            - [Quote block](#quote-block)
+        - [Combining elements into a document](#combining-elements-into-a-document)
+            - [Example heading](#example-heading-1)
+- [Further reading](#further-reading)
+- [Annexes](#annexes)
+    - [Annex 1: README Python source](#annex-1-readme-python-source)
+
+# Quick start guide
+
+Here's how you can start automatically generating Markdown documents
+
+## The first steps
+
+
+
+### Install
+
+Install YAMDOG with pip. YAMDOG uses only Python standard library so it has no additional dependencies.
+
+```
+pip install yamdog
+```
+
+### Import
+
+Import name is the same as install name, yamdog.
+
+```python
+import yamdog
+```
+
+Since the package is accessed often, I use abbreviation`md` for MarkDown. The abbreviation is used throughout this document.
+
+```python
+import yamdog as md
+```
+
+## Using the package
+
+There are two main things to building a Markdown document using YAMDOG
+
+1. Making elements
+2. Combining elements into a document
+
+You can call `str` on the element directly to get the markdown source
+
+```python
+markdown_source = str(element)
+```
+
+but most of the time you will compose the elements together into an document
+
+```python
+markdown_source = str(document)
+```
+
+### Making elements
+
+Let's start with an empty document
+
+```python
+document = md.Document([])
+```
+
+#### Heading
+
+*Python source*
+
+```python
+heading = md.Heading('Example heading', 4)
+```
+
+*Markdown source*
+
+```markdown
+#### Example heading
+```
+
+*Rendered result*
+
+#### Example heading
+
+---
+
+**bolded text**
+
+*some italiced text*
+
+~~striken text~~
+
+==highlighted text==
+
+*~~==**All styles combined**==~~*
+
+```python
+bold_text = md.Text('bolded text', {md.BOLD})
+italiced_text = md.Text('some italiced text', {md.ITALIC})
+strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
+highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
+all_together = md.Text('All styles combined',
+                               {md.BOLD, md.ITALIC,
+                                md.STRIKETHROUGH, md.HIGHLIGHT})
+```
+
+---
+
+#### Paragraph
+
+*Python source*
+
+```python
+paragraph = md.Paragraph(['Example paragraph containing ',
+                          md.Text('bolded text', {md.BOLD})])
+```
+
+*Markdown source*
+
+```markdown
+Example paragraph containing **bolded text**
+```
+
+*Rendered result*
+
+Example paragraph containing **bolded text**
+
+---
+
+#### Table
+
+*Python source*
+
+```python
+table = md.Table([['a', 1, 'Python'],
+                  ['b', 2, 'Markdown']],
+                 ['First column', 'Second column', 'Third column'],
+                 [md.RIGHT, md.LEFT, md.CENTER])
+```
+
+*Markdown source*
+
+```markdown
+| First column | Second column | Third column |
+| -----------: | :------------ | :----------: |
+|            a | 1             |    Python    |
+|            b | 2             |   Markdown   |
+```
+
+*Rendered result*
+
+| First column | Second column | Third column |
+| -----------: | :------------ | :----------: |
+|            a | 1             |    Python    |
+|            b | 2             |   Markdown   |
+
+---
+
+You can select compact mode at the table object creation
+
+#### Compact table
+
+*Python source*
+
+```python
+table = md.Table([['a', 1, 'Python'],
+                  ['b', 2, 'Markdown']],
+                 ['First column', 'Second column', 'Third column'],
+                 [md.RIGHT, md.LEFT, md.CENTER],
+                 True)
+```
+
+*Markdown source*
+
+```markdown
+First column|Second column|Third column
+--:|:--|:-:
+a|1|Python
+b|2|Markdown
+```
+
+*Rendered result*
+
+First column|Second column|Third column
+--:|:--|:-:
+a|1|Python
+b|2|Markdown
+
+---
+
+or later by changing the attribute `compact`
+
+```python
+table.compact = True
+```
+
+#### Listing
+
+*Python source*
+
+```python
+listing = md.Listing(['Just normal text',
+                      md.Text('some stylised text', {md.ITALIC}),
+                      md.Checkbox('Listings can include checkboxes', False),
+                      md.Checkbox('Checked and unchecked option available', True),
+                      ('Sublist by using a tuple',
+                        md.Listing(['first', 'second'], md.ORDERED))],
+                      md.UNORDERED)
+```
+
+*Markdown source*
+
+```markdown
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+```
+
+*Rendered result*
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+
+---
+
+#### Checklist
+
+*Python source*
+
+```python
+checklist = md.make_checklist([('unchecked box', False),
+                               ('checked box', True),
+                               ('done', True)])
+```
+
+*Markdown source*
+
+```markdown
+- [ ] unchecked box
+- [x] checked box
+- [x] done
+```
+
+*Rendered result*
+
+- [ ] unchecked box
+- [x] checked box
+- [x] done
+
+---
+
+#### Link
+
+*Python source*
+
+```python
+link = md.Link('https://www.markdownguide.org', 'Link to Markdown Guide')
+```
+
+*Markdown source*
+
+```markdown
+[Link to Markdown Guide](https://www.markdownguide.org)
+```
+
+*Rendered result*
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+---
+
+#### Codeblock
+
+*Python source*
+
+```python
+codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document([])',
+                         'python')
+```
+
+*Markdown source*
+
+````markdown
+```python
+import yamdog as md
+
+doc = md.Document([])
+```
+````
+
+*Rendered result*
+
+```python
+import yamdog as md
+
+doc = md.Document([])
+```
+
+---
+
+#### Code
+
+*Python source*
+
+```python
+code = md.Code('python != markdown')
+```
+
+*Markdown source*
+
+```markdown
+`python != markdown`
+```
+
+*Rendered result*
+
+`python != markdown`
+
+---
+
+#### Address
+
+*Python source*
+
+```python
+address = md.Link('https://www.markdownguide.org')
+```
+
+*Markdown source*
+
+```markdown
+<https://www.markdownguide.org>
+```
+
+*Rendered result*
+
+<https://www.markdownguide.org>
+
+---
+
+#### Quote block
+
+*Python source*
+
+```python
+quoteblock = md.Quote('Quote block supports\nmultiple lines')
+```
+
+*Markdown source*
+
+```markdown
+> Quote block supports
+> multiple lines
+```
+
+*Rendered result*
+
+> Quote block supports
+> multiple lines
+
+---
+
+### Combining elements into a document
+
+Initialising Document with list of elements
+
+```python
+document = md.Document([heading, link, paragraph, listing])
+```
+
+adding elements into a document
+
+```python
+document = md.Document([])
+document += heading
+document += link
+document += paragraph
+document += listing
+```
+
+adding elements together into a document
+
+```python
+document = heading + link + paragraph + listing
+```
+
+Adding two documents together
+
+```python
+document1 = md.Document([heading, link])
+document2 = md.Document([paragraph, listing])
+document = document1 + document2
+```
+
+*Markdown source*
+
+```markdown
+#### Example heading
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+Example paragraph containing **bolded text**
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+```
+
+*Rendered result*
+
+#### Example heading
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+Example paragraph containing **bolded text**
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+
+# Changelog <!-- omit in toc -->
+
+## 0.5.0 2023-05-07 <!-- omit in toc -->
+
+- Some API changes
+- Added Raw, PDF, Comment
+
+## 0.4.0 2023-01-23 <!-- omit in toc -->
+
+- Much better type validation
+- Some comparisons
+
+## 0.3.1 2023-01-23 <!-- omit in toc -->
+
+- Preliminary type validation
+- Full test coverage
+
+# Further reading
+
+- [basic syntax guide][2]
+- [extended syntax guide][2]
+
+---
+
+# Annexes
+
+## Annex 1: README Python source
+
+And here the full source code that wrote this README. This can serve as a more advanced example of what this is capable of.
+
+[The python file can also be found here](https://github.com/Limespy/YAMDOG/blob/main/readme.py)
+
+```python
+import datetime
+import pathlib
+import re
+
+import yamdog as md
+
+PATH_BASE = pathlib.Path(__file__).parent
+PATH_README = PATH_BASE / 'README.md'
+PATH_CHANGELOG = PATH_BASE / '.changelog.md'
+PATH_PYPROJECT = PATH_BASE / 'pyproject.toml'
+VERSION = md.__version__
+#=======================================================================
+def make_examples(source: str) -> md.Document:
+    '''Examples are collected via source code introspection'''
+    # First getting the example code blocks
+    pattern = re.compile('\n    #%% ')
+    examples = {}
+    for block in pattern.split(source)[1:]:
+        name, rest = block.split('\n', 1) # from the comment
+        code = rest.split('\n\n', 1)[0].replace('\n    ', '\n').strip()
+        examples[name.strip()] = md.CodeBlock(code, 'python')
+
+    def get_example(title: str, element: md.Element) -> md.Document:
+        return md.Document([md.Heading(title.capitalize(), 4),
+                            md.Text('Python source', {md.ITALIC}),
+                            examples[title],
+                            md.Text('Markdown source', {md.ITALIC}),
+                            md.CodeBlock(element, 'markdown'),
+                            md.Text('Rendered result', {md.ITALIC}),
+                            element,
+                            md.HRule()])
+
+    # Starting the actual doc
+    doc = md.Document([
+        md.Heading('Making elements', 3),
+
+    ])
+
+    #%% document
+    document = md.Document([])
+
+    doc += "Let's start with an empty document"
+    doc += examples['document']
+
+    #%% adding to document
+    # document +=
+
+    #%% heading
+    heading = md.Heading('Example heading', 4)
+
+    doc += get_example('heading', heading)
+
+    #%% stylised
+    bold_text = md.Text('bolded text', {md.BOLD})
+    italiced_text = md.Text('some italiced text', {md.ITALIC})
+    strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
+    highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
+    all_together = md.Text('All styles combined',
+                                   {md.BOLD, md.ITALIC,
+                                    md.STRIKETHROUGH, md.HIGHLIGHT})
+
+    doc += bold_text
+    doc += italiced_text
+    doc += strikethrough_text
+    doc += highlighted_text
+    doc += all_together
+    doc += examples['stylised']
+    doc += md.HRule()
+
+    #%%  paragraph
+    paragraph = md.Paragraph(['Example paragraph containing ',
+                              md.Text('bolded text', {md.BOLD})])
+
+    doc += get_example('paragraph', paragraph)
+
+    #%% table
+    table = md.Table([['a', 1, 'Python'],
+                      ['b', 2, 'Markdown']],
+                     ['First column', 'Second column', 'Third column'],
+                     [md.RIGHT, md.LEFT, md.CENTER])
+
+    doc += get_example('table', table)
+
+    #%% compact table
+    table = md.Table([['a', 1, 'Python'],
+                      ['b', 2, 'Markdown']],
+                     ['First column', 'Second column', 'Third column'],
+                     [md.RIGHT, md.LEFT, md.CENTER],
+                     True)
+
+    doc += 'You can select compact mode at the table object creation'
+    doc += get_example('compact table', table)
+
+    #%% table compact attribute
+    table.compact = True
+
+    doc += md.Paragraph(['or later by changing the attribute ',
+                         md.Code('compact')])
+    doc += examples['table compact attribute']
+
+    #%% listing
+    listing = md.Listing(['Just normal text',
+                          md.Text('some stylised text', {md.ITALIC}),
+                          md.Checkbox('Listings can include checkboxes', False),
+                          md.Checkbox('Checked and unchecked option available', True),
+                          ('Sublist by using a tuple',
+                            md.Listing(['first', 'second'], md.ORDERED))],
+                          md.UNORDERED)
+
+    doc += get_example('listing', listing)
+
+    #%% checklist
+    checklist = md.make_checklist([('unchecked box', False),
+                                   ('checked box', True),
+                                   ('done', True)])
+
+    doc += get_example('checklist', checklist)
+    #%% link
+    link = md.Link('https://www.markdownguide.org', 'Link to Markdown Guide')
+
+    doc += get_example('link', link)
+
+    #%% codeblock
+    codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document([])',
+                             'python')
+
+    doc += get_example('codeblock', codeblock)
+
+    #%% code
+    code = md.Code('python != markdown')
+
+    doc += get_example('code', code)
+
+    #%% Image
+    # image = md.Image()
+
+    #%% address
+    address = md.Link('https://www.markdownguide.org')
+
+    doc += get_example('address', address)
+
+    #%% quote block
+    quoteblock = md.Quote('Quote block supports\nmultiple lines')
+
+    doc += get_example('quote block', quoteblock)
+
+    doc += md.Heading('Combining elements into a document', 3)
+
+    #%% calling document
+    document = md.Document([heading, link, paragraph, listing])
+
+    doc += 'Initialising Document with list of elements'
+    doc += examples['calling document']
+
+    #%% from empty document
+    document = md.Document([])
+    document += heading
+    document += link
+    document += paragraph
+    document += listing
+
+    doc += 'adding elements into a document'
+    doc += examples['from empty document']
+
+    #%% document by adding
+    document = heading + link + paragraph + listing
+
+    doc += 'adding elements together into a document'
+    doc += examples['document by adding']
+
+    #%% document concatenation
+    document1 = md.Document([heading, link])
+    document2 = md.Document([paragraph, listing])
+    document = document1 + document2
+
+    doc += 'Adding two documents together'
+    doc += examples['document concatenation']
+
+    doc += md.Text('Markdown source', {md.ITALIC})
+    doc += md.CodeBlock(document, 'markdown')
+    doc += md.Text('Rendered result', {md.ITALIC})
+    doc += document
+
+    return doc
+#=======================================================================
+def make_quick_start_guide(name, pypiname, source):
+    doc = md.Document([
+        md.Heading('Quick start guide', 1),
+        "Here's how you can start automatically generating Markdown documents",
+        md.Heading('The first steps', 2),
+        '',
+        md.Heading('Install', 3),
+        f'''Install {name} with pip.
+        {name} uses only Python standard library so it has no additional dependencies.''',
+        md.CodeBlock(f'pip install {pypiname}'),
+        md.Heading('Import', 3),
+        f'''Import name is the same as install name, {pypiname}.''',
+        md.CodeBlock(f'import {pypiname}', 'python'),
+        md.Paragraph(['Since the package is accessed often, I use abbreviation',
+                      md.Code('md'),
+                      ' for MarkDown. The abbreviation is used throughout this document.']),
+        md.CodeBlock(f'import {pypiname} as md', 'python'),
+        md.Heading('Using the package', 2),
+        f'There are two main things to building a Markdown document using {name}',
+        md.Listing(['Making elements',
+                    'Combining elements into a document'], md.ORDERED),
+        md.Paragraph(['You can call ',
+            md.Code('str'),
+            ' on the element directly to get the markdown source']),
+        md.CodeBlock('markdown_source = str(element)', 'python'),
+        '''but most of the time you will compose the elements together into an
+        document''',
+        md.CodeBlock('markdown_source = str(document)', 'python')
+        ])
+    doc += make_examples(source)
+    return doc
+#=======================================================================
+re_heading = re.compile(r'^#* .*$')
+
+def parse_md_element(text: str):
+    if match := re_heading.match(text):
+        hashes, content = match[0].split(' ', 1)
+        return md.Heading(content, len(hashes))
+    else:
+        return md.Raw(text)
+#-----------------------------------------------------------------------
+def parse_md(text: str):
+    return md.Document([parse_md_element(item.strip())
+                        for item in text.split('\n\n')])
+#-----------------------------------------------------------------------
+def make_changelog(level: int):
+    doc = md.Document([md.Heading('Changelog', level, in_TOC = False)])
+    changelog = parse_md(PATH_CHANGELOG.read_text())
+    if changelog:
+        if (latest := changelog.content[0]).content.split(' ', 1)[0] == VERSION:
+            latest.content = f'{VERSION} {datetime.date.today().isoformat()}'
+        else:
+            raise ValueError('Changelog not up to date')
+
+        PATH_CHANGELOG.write_text(str(changelog) + '\n')
+
+        for item in changelog:
+            if isinstance(item, md.Heading):
+                item.level = level + 1
+                item.in_TOC = False
+
+        doc += changelog
+
+    return doc
+#=======================================================================
+def make_further_reading():
+    basic_syntax_link = md.Link('https://www.markdownguide.org/basic-syntax/',
+                                'basic syntax guide',
+                                '')
+    extended_syntax_link = md.Link('https://www.markdownguide.org/basic-syntax/',
+                                   'extended syntax guide',
+                                   '')
+
+    doc = md.Document([md.Heading('Further reading', 1)])
+    doc += md.Listing([basic_syntax_link, extended_syntax_link], md.UNORDERED)
+    return doc
+#=======================================================================
+def make_annexes(source):
+    doc = md.Document([md.Heading('Annexes', 1)])
+    doc += md.Heading('Annex 1: README Python source', 2)
+    doc += '''And here the full source code that wrote this README.
+            This can serve as a more advanced example of what this is
+            capable of.'''
+    doc += md.Link('https://github.com/Limespy/YAMDOG/blob/main/readme.py',
+                   'The python file can also be found here')
+    doc += md.CodeBlock(source, 'python')
+    return doc
+#=======================================================================
+def make(name, pypiname, source):
+    # Setup for the badges
+    shields_url = 'https://img.shields.io/'
+
+    pypi_project_url = f'https://pypi.org/project/{pypiname}'
+    pypi_badge_info = (('v', 'PyPI Package latest release'),
+                       ('wheel', 'PyPI Wheel'),
+                       ('pyversions', 'Supported versions'),
+                       ('implementation', 'Supported implementations'))
+    pypi_badges = [md.Link(pypi_project_url,
+                           md.Image(f'{shields_url}pypi/{code}/{pypiname}.svg',
+                                    desc), '')
+                   for code, desc in pypi_badge_info]
+
+    # Starting the document
+    doc = md.Document([
+        md.Heading(f'Overview of {name}', 1, in_TOC = False),
+        md.Paragraph(pypi_badges, '\n'),
+        'Yet Another Markdown Only Generator',
+        md.Heading(f'What is {name}?', 2, in_TOC = False),
+        f'''{name} is toolkit for creating Markdown text using Python.
+        Markdown is a light and relatively simple markup language.''',
+        md.Heading('Table of Content', 3, in_TOC = False),
+        md.TOC()
+        ])
+    source = pathlib.Path(__file__).read_text('utf8')
+    doc += make_quick_start_guide(name, pypiname, source)
+    doc += make_changelog(level = 1)
+    doc += make_further_reading()
+    doc += md.HRule()
+    doc += make_annexes(source)
+    return doc
+#=======================================================================
+def main():
+    try:
+        import tomllib
+    except ModuleNotFoundError:
+        import tomli as tomllib # type: ignore
+
+    pyproject = tomllib.loads(PATH_PYPROJECT.read_text())
+    master_info = pyproject['master-info']
+    package_name = master_info["package_name"]
+    full_name = master_info.get("full_name",
+                                package_name.replace('-', ' ').capitalize())
+    description = master_info['description']
+
+    doc = make(full_name, package_name, description)
+    PATH_README.write_text(str(doc) + '\n')
+#=======================================================================
+if __name__ == '__main__':
+    main()
+
+```
+
+[1]: <https://pypi.org/project/yamdog> ""
+[2]: <https://www.markdownguide.org/basic-syntax/> ""
```

### Comparing `yamdog-0.4.0.14/src/YAMDOG.egg-info/PKG-INFO` & `yamdog-0.5.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,815 +1,852 @@
-Metadata-Version: 2.1
-Name: yamdog
-Version: 0.4.0.14
-Summary: Yet Another Markdown Only Generator
-Author: Limespy
-License: MIT License
-Project-URL: Homepage, https://github.com/Limespy/yamdog
-Project-URL: Changelog, https://github.com/Limespy/yamdog/blob/main/README.md#Changelog
-Project-URL: Issue Tracker, https://github.com/Limespy/yamdog/issues
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Unix
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.txt
-
-# Overview of YAMDOG <!-- omit in toc -->
-
-[![PyPI Package latest release](https://img.shields.io/pypi/v/yamdog.svg)][1]
-[![PyPI Wheel](https://img.shields.io/pypi/wheel/yamdog.svg)][1]
-[![Supported versions](https://img.shields.io/pypi/pyversions/yamdog.svg)][1]
-[![Supported implementations](https://img.shields.io/pypi/implementation/yamdog.svg)][1]
-
-Yet Another Markdown Only Generator
-
-## What is YAMDOG? <!-- omit in toc -->
-
-YAMDOG is toolkit for creating Markdown text using Python. Markdown is a light and relatively simple markup language.
-
-### Table of Content <!-- omit in toc -->
-
-- [Quick start guide](#quick-start-guide)
-    - [The first steps](#the-first-steps)
-        - [Install](#install)
-        - [Import](#import)
-    - [Using the package](#using-the-package)
-        - [Making elements](#making-elements)
-            - [Heading](#heading)
-            - [Example heading](#example-heading)
-            - [Paragraph](#paragraph)
-            - [Table](#table)
-            - [Compact table](#compact-table)
-            - [Listing](#listing)
-            - [Checklist](#checklist)
-            - [Link](#link)
-            - [Codeblock](#codeblock)
-            - [Code](#code)
-            - [Address](#address)
-            - [Quote block](#quote-block)
-        - [Combining elements into a document](#combining-elements-into-a-document)
-            - [Example heading](#example-heading1)
-- [Changelog](#changelog)
-- [Further reading](#further-reading)
-- [Annexes](#annexes)
-    - [Annex 1: README Python source](#annex-1-readme-python-source)
-
-# Quick start guide
-
-Here's how you can start automatically generating Markdown documents
-
-## The first steps
-
-
-
-### Install
-
-Install YAMDOG with pip. YAMDOG uses only Python standard library so it has no additional dependencies.
-
-```
-pip install yamdog
-```
-
-### Import
-
-Import name is the same as install name, yamdog.
-
-```python
-import yamdog
-```
-
-Since the package is accessed often, I use abbreviation`md` for MarkDown. The abbreviation is used throughout this document.
-
-```python
-import yamdog as md
-```
-
-## Using the package
-
-There are two main things to building a Markdown document using YAMDOG
-
-1. Making elements
-2. Combining elements into a document
-
-You can call `str` on the element directly to get the markdown source
-
-```python
-markdown_source = str(element)
-```
-
-but most of the time you will compose the elements together into an document
-
-```python
-markdown_source = str(document)
-```
-
-### Making elements
-
-Let's start with an empty document
-
-```python
-document = md.Document()
-```
-
-#### Heading
-
-*Python source*
-
-```python
-heading = md.Heading(4, 'Example heading')
-```
-
-*Markdown source*
-
-```markdown
-#### Example heading
-```
-
-*Rendered result*
-
-#### Example heading
-
----
-
-**bolded text**
-
-*some italiced text*
-
-~~striken text~~
-
-==highlighted text==
-
-==*~~**All styles combined**~~*==
-
-```python
-bold_text = md.Text('bolded text', {md.BOLD})
-italiced_text = md.Text('some italiced text', {md.ITALIC})
-strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
-highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
-all_together = md.Text('All styles combined',
-                               {md.BOLD, md.ITALIC,
-                                md.STRIKETHROUGH, md.HIGHLIGHT})
-```
-
----
-
-#### Paragraph
-
-*Python source*
-
-```python
-paragraph = md.Paragraph(['Example paragraph containing ',
-                          md.Text('bolded text', {md.BOLD})])
-```
-
-*Markdown source*
-
-```markdown
-Example paragraph containing **bolded text**
-```
-
-*Rendered result*
-
-Example paragraph containing **bolded text**
-
----
-
-#### Table
-
-*Python source*
-
-```python
-table = md.Table(['First column', 'Second column', 'Third column'],
-                 [['a', 1, 'Python'],
-                  ['b', 2, 'Markdown']],
-                 [md.RIGHT, md.LEFT, md.CENTER])
-```
-
-*Markdown source*
-
-```markdown
-| First column | Second column | Third column |
-| -----------: | :------------ | :----------: |
-|            a | 1             |    Python    |
-|            b | 2             |   Markdown   |
-```
-
-*Rendered result*
-
-| First column | Second column | Third column |
-| -----------: | :------------ | :----------: |
-|            a | 1             |    Python    |
-|            b | 2             |   Markdown   |
-
----
-
-You can select compact mode at the table object creation
-
-#### Compact table
-
-*Python source*
-
-```python
-table = md.Table(['First column', 'Second column', 'Third column'],
-                 [['a', 1, 'Python'],
-                  ['b', 2, 'Markdown']],
-                 [md.RIGHT, md.LEFT, md.CENTER],
-                 True)
-```
-
-*Markdown source*
-
-```markdown
-First column|Second column|Third column
---:|:--|:-:
-a|1|Python
-b|2|Markdown
-```
-
-*Rendered result*
-
-First column|Second column|Third column
---:|:--|:-:
-a|1|Python
-b|2|Markdown
-
----
-
-or later by changing the attribute `compact`
-
-```python
-table.compact = True
-```
-
-#### Listing
-
-*Python source*
-
-```python
-listing = md.Listing(md.UNORDERED, 
-                     ['Just normal text',
-                      md.Text('some stylised text', {md.ITALIC}),
-                      md.Checkbox(False, 'Listings can include checkboxes'),
-                      md.Checkbox(True, 'Checked and unchecked option available'),
-                      ('Sublist by using a tuple',
-                        md.Listing(md.ORDERED,
-                                  ['first', 'second']))])
-```
-
-*Markdown source*
-
-```markdown
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-```
-
-*Rendered result*
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-
----
-
-#### Checklist
-
-*Python source*
-
-```python
-checklist = md.make_checklist([(False, 'unchecked box'),
-                               (True, 'checked box'),
-                               (True, 'done')])
-```
-
-*Markdown source*
-
-```markdown
-
-```
-
-*Rendered result*
-
-
-
----
-
-#### Link
-
-*Python source*
-
-```python
-link = md.Link('Link to Markdown Guide', 'https://www.markdownguide.org')
-```
-
-*Markdown source*
-
-```markdown
-[Link to Markdown Guide](https://www.markdownguide.org)
-```
-
-*Rendered result*
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
----
-
-#### Codeblock
-
-*Python source*
-
-```python
-codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document()',
-                         'python')
-```
-
-*Markdown source*
-
-````markdown
-```python
-import yamdog as md
-
-doc = md.Document()
-```
-````
-
-*Rendered result*
-
-```python
-import yamdog as md
-
-doc = md.Document()
-```
-
----
-
-#### Code
-
-*Python source*
-
-```python
-code = md.Code('python != markdown')
-```
-
-*Markdown source*
-
-```markdown
-`python != markdown`
-```
-
-*Rendered result*
-
-`python != markdown`
-
----
-
-#### Address
-
-*Python source*
-
-```python
-address = md.Address('https://www.markdownguide.org')
-```
-
-*Markdown source*
-
-```markdown
-<https://www.markdownguide.org>
-```
-
-*Rendered result*
-
-<https://www.markdownguide.org>
-
----
-
-#### Quote block
-
-*Python source*
-
-```python
-quoteblock = md.QuoteBlock('Quote block supports\nmultiple lines')
-```
-
-*Markdown source*
-
-```markdown
-> Quote block supports
-> multiple lines
-```
-
-*Rendered result*
-
-> Quote block supports
-> multiple lines
-
----
-
-### Combining elements into a document
-
-Initialising Document with list of elements
-
-```python
-document = md.Document([heading, link, paragraph, listing])
-```
-
-adding elements into a document
-
-```python
-document = md.Document()
-document += heading
-document += link
-document += paragraph
-document += listing
-```
-
-adding elements together into a document
-
-```python
-document = heading + link + paragraph + listing
-```
-
-Adding two documents together
-
-```python
-document1 = md.Document([heading, link])
-document2 = md.Document([paragraph, listing])
-document = document1 + document2
-```
-
-*Markdown source*
-
-```markdown
-#### Example heading
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
-Example paragraph containing **bolded text**
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-```
-
-*Rendered result*
-
-#### Example heading
-
-[Link to Markdown Guide](https://www.markdownguide.org)
-
-Example paragraph containing **bolded text**
-
-- Just normal text
-- *some stylised text*
-- [ ] Listings can include checkboxes
-- [x] Checked and unchecked option available
-- Sublist by using a tuple
-    1. first
-    2. second
-
-# Changelog
-
-## 0.4.0 2023-01-23 <!-- omit in toc -->
-
-- Much better type validation
-- Some comparisons
-
-## 0.3.1 2023-01-23 <!-- omit in toc -->
-
-- Preliminary type validation
-- Full test coverage
-
-# Further reading
-
-- [basic syntax][2]
-- [extended syntax][2]
-
----
-
-# Annexes
-
-## Annex 1: README Python source
-
-And here the full source code that wrote this README. This can serve as a more advanced example of what this is capable of.
-
-[The python file can also be found here](https://github.com/Limespy/YAMDOG/blob/main/readme.py)
-
-```python
-import yamdog as md
-
-import pathlib
-import re
-
-def make_examples(source: str) -> md.Document:
-    '''Examples are collected via source code introspection'''
-    # First getting the example code blocks
-    pattern = re.compile('\n    #%% ')
-    examples = {}
-    for block in pattern.split(source)[1:]:
-        name, rest = block.split('\n', 1) # from the comment
-        code = rest.split('\n\n', 1)[0].replace('\n    ', '\n').strip()
-        examples[name.strip()] = md.CodeBlock(code, 'python')
-
-    def get_example(title: str, element: md.Element) -> md.Document:
-        return md.Document([md.Heading(4, title.capitalize()),
-                            md.Text('Python source', {md.ITALIC}),
-                            examples[title],
-                            md.Text('Markdown source', {md.ITALIC}),
-                            md.CodeBlock(element, 'markdown'),
-                            md.Text('Rendered result', {md.ITALIC}),
-                            element,
-                            md.HRule()])
-
-    # Starting the actual doc
-    doc = md.Document([
-        md.Heading(3, 'Making elements'),
-
-    ])
-
-    #%% document
-    document = md.Document()
-
-    doc += "Let's start with an empty document"
-    doc += examples['document']
-
-    #%% adding to document
-    # document += 
-
-    #%% heading
-    heading = md.Heading(4, 'Example heading')
-
-    doc += get_example('heading', heading)
-
-    #%% stylised
-    bold_text = md.Text('bolded text', {md.BOLD})
-    italiced_text = md.Text('some italiced text', {md.ITALIC})
-    strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
-    highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
-    all_together = md.Text('All styles combined',
-                                   {md.BOLD, md.ITALIC,
-                                    md.STRIKETHROUGH, md.HIGHLIGHT})
-
-    doc += bold_text
-    doc += italiced_text
-    doc += strikethrough_text
-    doc += highlighted_text
-    doc += all_together
-    doc += examples['stylised']
-    doc += md.HRule()
-
-    #%%  paragraph
-    paragraph = md.Paragraph(['Example paragraph containing ',
-                              md.Text('bolded text', {md.BOLD})])
-
-    doc += get_example('paragraph', paragraph)
-
-    #%% table
-    table = md.Table(['First column', 'Second column', 'Third column'],
-                     [['a', 1, 'Python'],
-                      ['b', 2, 'Markdown']],
-                     [md.RIGHT, md.LEFT, md.CENTER])
-
-    doc += get_example('table', table)
-
-    #%% compact table
-    table = md.Table(['First column', 'Second column', 'Third column'],
-                     [['a', 1, 'Python'],
-                      ['b', 2, 'Markdown']],
-                     [md.RIGHT, md.LEFT, md.CENTER],
-                     True)
-
-    doc += 'You can select compact mode at the table object creation'
-    doc += get_example('compact table', table)
-
-    #%% table compact attribute
-    table.compact = True
-
-    doc += md.Paragraph(['or later by changing the attribute ',
-                         md.Code('compact')])
-    doc += examples['table compact attribute']
-
-    #%% listing
-    listing = md.Listing(md.UNORDERED, 
-                         ['Just normal text',
-                          md.Text('some stylised text', {md.ITALIC}),
-                          md.Checkbox(False, 'Listings can include checkboxes'),
-                          md.Checkbox(True, 'Checked and unchecked option available'),
-                          ('Sublist by using a tuple',
-                            md.Listing(md.ORDERED,
-                                      ['first', 'second']))])
-
-    doc += get_example('listing', listing)
-
-    #%% checklist
-    checklist = md.make_checklist([(False, 'unchecked box'),
-                                   (True, 'checked box'),
-                                   (True, 'done')])
-
-    doc += get_example('checklist', checklist)
-    #%% link
-    link = md.Link('Link to Markdown Guide', 'https://www.markdownguide.org')
-
-    doc += get_example('link', link)
-
-    #%% codeblock
-    codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document()',
-                             'python')
-
-    doc += get_example('codeblock', codeblock)
-
-    #%% code
-    code = md.Code('python != markdown')
-
-    doc += get_example('code', code)
-
-    #%% Image
-    # image = md.Image()
-
-    #%% address
-    address = md.Address('https://www.markdownguide.org')
-
-    doc += get_example('address', address)
-
-    #%% quote block
-    quoteblock = md.QuoteBlock('Quote block supports\nmultiple lines')
-
-    doc += get_example('quote block', quoteblock)
-
-    doc += md.Heading(3, 'Combining elements into a document')
-
-    #%% calling document
-    document = md.Document([heading, link, paragraph, listing])
-
-    doc += 'Initialising Document with list of elements'
-    doc += examples['calling document']
-
-    #%% from empty document
-    document = md.Document()
-    document += heading
-    document += link
-    document += paragraph
-    document += listing
-
-    doc += 'adding elements into a document'
-    doc += examples['from empty document']
-
-    #%% document by adding
-    document = heading + link + paragraph + listing
-
-    doc += 'adding elements together into a document'
-    doc += examples['document by adding']
-
-    #%% document concatenation
-    document1 = md.Document([heading, link])
-    document2 = md.Document([paragraph, listing])
-    document = document1 + document2
-
-    doc += 'Adding two documents together'
-    doc += examples['document concatenation']
-
-    doc += md.Text('Markdown source', {md.ITALIC})
-    doc += md.CodeBlock(document, 'markdown')
-    doc += md.Text('Rendered result', {md.ITALIC})
-    doc += document
-
-    return doc
-
-def make_quick_start_guide(name, pypiname, source):
-    doc = md.Document([
-        md.Heading(1, 'Quick start guide'),
-        "Here's how you can start automatically generating Markdown documents",
-        md.Heading(2, 'The first steps'),
-        '',
-        md.Heading(3, 'Install'),
-        f'''Install {name} with pip.
-        {name} uses only Python standard library so it has no additional dependencies.''',
-        md.CodeBlock(f'pip install {pypiname}'),
-        md.Heading(3, 'Import'),
-        f'''Import name is the same as install name, {pypiname}.''',
-        md.CodeBlock(f'import {pypiname}', 'python'),
-        md.Paragraph(['Since the package is accessed often, I use abbreviation',
-                      md.Code('md'), 
-                      ' for MarkDown. The abbreviation is used throughout this document.']),
-        md.CodeBlock(f'import {pypiname} as md', 'python'),
-        md.Heading(2, 'Using the package'),
-        f'There are two main things to building a Markdown document using {name}',
-        md.Listing(md.ORDERED, ['Making elements',
-                               'Combining elements into a document']),
-        md.Paragraph(['You can call ',
-            md.Code('str'),
-            ' on the element directly to get the markdown source']),
-        md.CodeBlock('markdown_source = str(element)', 'python'),
-        '''but most of the time you will compose the elements together into an
-        document''',
-        md.CodeBlock('markdown_source = str(document)', 'python')
-        ])
-    doc += make_examples(source)
-    return doc
-
-
-def make_changelog():
-    doc = md.Document([md.Heading(1, 'Changelog')])
-
-    changelog = (('0.4.0', '2023-01-23', ['Much better type validation',
-                                          'Some comparisons']),
-                 ('0.3.1', '2023-01-23', ['Preliminary type validation',
-                                          'Full test coverage'])
-                 )
-
-    for version, date, changes in changelog:
-        doc += md.Heading(2, f'{version} {date}', in_TOC = False)
-        doc += md.Listing(md.UNORDERED, changes)
-
-    return doc
-
-def make_further_reading():
-    basic_syntax_link = md.Link('basic syntax',
-                                'https://www.markdownguide.org/basic-syntax/',
-                                '')
-    extended_syntax_link = md.Link('extended syntax',
-                                  'https://www.markdownguide.org/basic-syntax/',
-                                   '')
-
-    doc = md.Document([md.Heading(1, 'Further reading')])
-    doc += md.Listing(md.UNORDERED, [basic_syntax_link, extended_syntax_link])
-    return doc
-
-def make_annexes(source):
-    doc = md.Document([md.Heading(1, 'Annexes')])
-    doc += md.Heading(2, 'Annex 1: README Python source')
-    doc += '''And here the full source code that wrote this README.
-            This can serve as a more advanced example of what this is
-            capable of.'''
-    doc += md.Link('The python file can also be found here',
-                   'https://github.com/Limespy/YAMDOG/blob/main/readme.py')
-    doc += md.CodeBlock(source, 'python')
-    return doc
-
-def make_readme(name, pypiname, source):
-    # Setup for the badges
-    shields_url = 'https://img.shields.io/'
-
-    pypi_project_url = f'https://pypi.org/project/{pypiname}'
-    pypi_badge_info = (('v', 'PyPI Package latest release'),
-                       ('wheel', 'PyPI Wheel'),
-                       ('pyversions', 'Supported versions'),
-                       ('implementation', 'Supported implementations'))
-    pypi_badges = [md.Link(md.Image(f'{shields_url}pypi/{code}/{pypiname}.svg',
-                                    desc), pypi_project_url, '')
-                   for code, desc in pypi_badge_info]
-
-    # Starting the document
-    doc = md.Document([
-        md.Heading(1, f'Overview of {name}', in_TOC = False),
-        md.Paragraph(pypi_badges, '\n'),
-        'Yet Another Markdown Only Generator',
-        md.Heading(2, f'What is {name}?', in_TOC = False),
-        f'''{name} is toolkit for creating Markdown text using Python.
-        Markdown is a light and relatively simple markup language.''',
-        md.Heading(3, 'Table of Content', in_TOC = False),
-        md.TOC()
-        ])
-    doc += make_quick_start_guide(name, pypiname, source)
-    doc += make_changelog()
-    doc += make_further_reading()
-    doc += md.HRule()
-    doc += make_annexes(source)
-    return doc
-
-def main():
-    name = 'YAMDOG'
-    pypiname = 'yamdog'
-
-    source = pathlib.Path(__file__).read_text('utf8')
-
-    doc = make_readme(name, pypiname, source)
-
-    (pathlib.Path(__file__).parent / 'README.md').write_text(str(doc), 'utf8')
-    return doc
-
-if __name__ == '__main__':
-    main()
-```
-
-[1]: <https://pypi.org/project/yamdog> ""
-[2]: <https://www.markdownguide.org/basic-syntax/> ""
+Metadata-Version: 2.1
+Name: yamdog
+Version: 0.5.0
+Summary: Yet Another Markdown Only Generator
+Author: Limespy
+Project-URL: Homepage, https://github.com/Limespy/yamdog
+Project-URL: Changelog, https://github.com/Limespy/yamdog/blob/main/README.md#Changelog
+Project-URL: Issue Tracker, https://github.com/Limespy/yamdog/issues
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE.txt
+
+# Overview of YAMDOG <!-- omit in toc -->
+
+[![PyPI Package latest release](https://img.shields.io/pypi/v/yamdog.svg)][1]
+[![PyPI Wheel](https://img.shields.io/pypi/wheel/yamdog.svg)][1]
+[![Supported versions](https://img.shields.io/pypi/pyversions/yamdog.svg)][1]
+[![Supported implementations](https://img.shields.io/pypi/implementation/yamdog.svg)][1]
+
+Yet Another Markdown Only Generator
+
+## What is YAMDOG? <!-- omit in toc -->
+
+YAMDOG is toolkit for creating Markdown text using Python. Markdown is a light and relatively simple markup language.
+
+### Table of Content <!-- omit in toc -->
+
+- [Quick start guide](#quick-start-guide)
+    - [The first steps](#the-first-steps)
+        - [Install](#install)
+        - [Import](#import)
+    - [Using the package](#using-the-package)
+        - [Making elements](#making-elements)
+            - [Heading](#heading)
+            - [Example heading](#example-heading)
+            - [Paragraph](#paragraph)
+            - [Table](#table)
+            - [Compact table](#compact-table)
+            - [Listing](#listing)
+            - [Checklist](#checklist)
+            - [Link](#link)
+            - [Codeblock](#codeblock)
+            - [Code](#code)
+            - [Address](#address)
+            - [Quote block](#quote-block)
+        - [Combining elements into a document](#combining-elements-into-a-document)
+            - [Example heading](#example-heading-1)
+- [Further reading](#further-reading)
+- [Annexes](#annexes)
+    - [Annex 1: README Python source](#annex-1-readme-python-source)
+
+# Quick start guide
+
+Here's how you can start automatically generating Markdown documents
+
+## The first steps
+
+
+
+### Install
+
+Install YAMDOG with pip. YAMDOG uses only Python standard library so it has no additional dependencies.
+
+```
+pip install yamdog
+```
+
+### Import
+
+Import name is the same as install name, yamdog.
+
+```python
+import yamdog
+```
+
+Since the package is accessed often, I use abbreviation`md` for MarkDown. The abbreviation is used throughout this document.
+
+```python
+import yamdog as md
+```
+
+## Using the package
+
+There are two main things to building a Markdown document using YAMDOG
+
+1. Making elements
+2. Combining elements into a document
+
+You can call `str` on the element directly to get the markdown source
+
+```python
+markdown_source = str(element)
+```
+
+but most of the time you will compose the elements together into an document
+
+```python
+markdown_source = str(document)
+```
+
+### Making elements
+
+Let's start with an empty document
+
+```python
+document = md.Document([])
+```
+
+#### Heading
+
+*Python source*
+
+```python
+heading = md.Heading('Example heading', 4)
+```
+
+*Markdown source*
+
+```markdown
+#### Example heading
+```
+
+*Rendered result*
+
+#### Example heading
+
+---
+
+**bolded text**
+
+*some italiced text*
+
+~~striken text~~
+
+==highlighted text==
+
+*~~==**All styles combined**==~~*
+
+```python
+bold_text = md.Text('bolded text', {md.BOLD})
+italiced_text = md.Text('some italiced text', {md.ITALIC})
+strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
+highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
+all_together = md.Text('All styles combined',
+                               {md.BOLD, md.ITALIC,
+                                md.STRIKETHROUGH, md.HIGHLIGHT})
+```
+
+---
+
+#### Paragraph
+
+*Python source*
+
+```python
+paragraph = md.Paragraph(['Example paragraph containing ',
+                          md.Text('bolded text', {md.BOLD})])
+```
+
+*Markdown source*
+
+```markdown
+Example paragraph containing **bolded text**
+```
+
+*Rendered result*
+
+Example paragraph containing **bolded text**
+
+---
+
+#### Table
+
+*Python source*
+
+```python
+table = md.Table([['a', 1, 'Python'],
+                  ['b', 2, 'Markdown']],
+                 ['First column', 'Second column', 'Third column'],
+                 [md.RIGHT, md.LEFT, md.CENTER])
+```
+
+*Markdown source*
+
+```markdown
+| First column | Second column | Third column |
+| -----------: | :------------ | :----------: |
+|            a | 1             |    Python    |
+|            b | 2             |   Markdown   |
+```
+
+*Rendered result*
+
+| First column | Second column | Third column |
+| -----------: | :------------ | :----------: |
+|            a | 1             |    Python    |
+|            b | 2             |   Markdown   |
+
+---
+
+You can select compact mode at the table object creation
+
+#### Compact table
+
+*Python source*
+
+```python
+table = md.Table([['a', 1, 'Python'],
+                  ['b', 2, 'Markdown']],
+                 ['First column', 'Second column', 'Third column'],
+                 [md.RIGHT, md.LEFT, md.CENTER],
+                 True)
+```
+
+*Markdown source*
+
+```markdown
+First column|Second column|Third column
+--:|:--|:-:
+a|1|Python
+b|2|Markdown
+```
+
+*Rendered result*
+
+First column|Second column|Third column
+--:|:--|:-:
+a|1|Python
+b|2|Markdown
+
+---
+
+or later by changing the attribute `compact`
+
+```python
+table.compact = True
+```
+
+#### Listing
+
+*Python source*
+
+```python
+listing = md.Listing(['Just normal text',
+                      md.Text('some stylised text', {md.ITALIC}),
+                      md.Checkbox('Listings can include checkboxes', False),
+                      md.Checkbox('Checked and unchecked option available', True),
+                      ('Sublist by using a tuple',
+                        md.Listing(['first', 'second'], md.ORDERED))],
+                      md.UNORDERED)
+```
+
+*Markdown source*
+
+```markdown
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+```
+
+*Rendered result*
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+
+---
+
+#### Checklist
+
+*Python source*
+
+```python
+checklist = md.make_checklist([('unchecked box', False),
+                               ('checked box', True),
+                               ('done', True)])
+```
+
+*Markdown source*
+
+```markdown
+- [ ] unchecked box
+- [x] checked box
+- [x] done
+```
+
+*Rendered result*
+
+- [ ] unchecked box
+- [x] checked box
+- [x] done
+
+---
+
+#### Link
+
+*Python source*
+
+```python
+link = md.Link('https://www.markdownguide.org', 'Link to Markdown Guide')
+```
+
+*Markdown source*
+
+```markdown
+[Link to Markdown Guide](https://www.markdownguide.org)
+```
+
+*Rendered result*
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+---
+
+#### Codeblock
+
+*Python source*
+
+```python
+codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document([])',
+                         'python')
+```
+
+*Markdown source*
+
+````markdown
+```python
+import yamdog as md
+
+doc = md.Document([])
+```
+````
+
+*Rendered result*
+
+```python
+import yamdog as md
+
+doc = md.Document([])
+```
+
+---
+
+#### Code
+
+*Python source*
+
+```python
+code = md.Code('python != markdown')
+```
+
+*Markdown source*
+
+```markdown
+`python != markdown`
+```
+
+*Rendered result*
+
+`python != markdown`
+
+---
+
+#### Address
+
+*Python source*
+
+```python
+address = md.Link('https://www.markdownguide.org')
+```
+
+*Markdown source*
+
+```markdown
+<https://www.markdownguide.org>
+```
+
+*Rendered result*
+
+<https://www.markdownguide.org>
+
+---
+
+#### Quote block
+
+*Python source*
+
+```python
+quoteblock = md.Quote('Quote block supports\nmultiple lines')
+```
+
+*Markdown source*
+
+```markdown
+> Quote block supports
+> multiple lines
+```
+
+*Rendered result*
+
+> Quote block supports
+> multiple lines
+
+---
+
+### Combining elements into a document
+
+Initialising Document with list of elements
+
+```python
+document = md.Document([heading, link, paragraph, listing])
+```
+
+adding elements into a document
+
+```python
+document = md.Document([])
+document += heading
+document += link
+document += paragraph
+document += listing
+```
+
+adding elements together into a document
+
+```python
+document = heading + link + paragraph + listing
+```
+
+Adding two documents together
+
+```python
+document1 = md.Document([heading, link])
+document2 = md.Document([paragraph, listing])
+document = document1 + document2
+```
+
+*Markdown source*
+
+```markdown
+#### Example heading
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+Example paragraph containing **bolded text**
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+```
+
+*Rendered result*
+
+#### Example heading
+
+[Link to Markdown Guide](https://www.markdownguide.org)
+
+Example paragraph containing **bolded text**
+
+- Just normal text
+- *some stylised text*
+- [ ] Listings can include checkboxes
+- [x] Checked and unchecked option available
+- Sublist by using a tuple
+    1. first
+    2. second
+
+# Changelog <!-- omit in toc -->
+
+## 0.5.0 2023-05-07 <!-- omit in toc -->
+
+- Some API changes
+- Added Raw, PDF, Comment
+
+## 0.4.0 2023-01-23 <!-- omit in toc -->
+
+- Much better type validation
+- Some comparisons
+
+## 0.3.1 2023-01-23 <!-- omit in toc -->
+
+- Preliminary type validation
+- Full test coverage
+
+# Further reading
+
+- [basic syntax guide][2]
+- [extended syntax guide][2]
+
+---
+
+# Annexes
+
+## Annex 1: README Python source
+
+And here the full source code that wrote this README. This can serve as a more advanced example of what this is capable of.
+
+[The python file can also be found here](https://github.com/Limespy/YAMDOG/blob/main/readme.py)
+
+```python
+import datetime
+import pathlib
+import re
+
+import yamdog as md
+
+PATH_BASE = pathlib.Path(__file__).parent
+PATH_README = PATH_BASE / 'README.md'
+PATH_CHANGELOG = PATH_BASE / '.changelog.md'
+PATH_PYPROJECT = PATH_BASE / 'pyproject.toml'
+VERSION = md.__version__
+#=======================================================================
+def make_examples(source: str) -> md.Document:
+    '''Examples are collected via source code introspection'''
+    # First getting the example code blocks
+    pattern = re.compile('\n    #%% ')
+    examples = {}
+    for block in pattern.split(source)[1:]:
+        name, rest = block.split('\n', 1) # from the comment
+        code = rest.split('\n\n', 1)[0].replace('\n    ', '\n').strip()
+        examples[name.strip()] = md.CodeBlock(code, 'python')
+
+    def get_example(title: str, element: md.Element) -> md.Document:
+        return md.Document([md.Heading(title.capitalize(), 4),
+                            md.Text('Python source', {md.ITALIC}),
+                            examples[title],
+                            md.Text('Markdown source', {md.ITALIC}),
+                            md.CodeBlock(element, 'markdown'),
+                            md.Text('Rendered result', {md.ITALIC}),
+                            element,
+                            md.HRule()])
+
+    # Starting the actual doc
+    doc = md.Document([
+        md.Heading('Making elements', 3),
+
+    ])
+
+    #%% document
+    document = md.Document([])
+
+    doc += "Let's start with an empty document"
+    doc += examples['document']
+
+    #%% adding to document
+    # document +=
+
+    #%% heading
+    heading = md.Heading('Example heading', 4)
+
+    doc += get_example('heading', heading)
+
+    #%% stylised
+    bold_text = md.Text('bolded text', {md.BOLD})
+    italiced_text = md.Text('some italiced text', {md.ITALIC})
+    strikethrough_text = md.Text('striken text', {md.STRIKETHROUGH})
+    highlighted_text = md.Text('highlighted text', {md.HIGHLIGHT})
+    all_together = md.Text('All styles combined',
+                                   {md.BOLD, md.ITALIC,
+                                    md.STRIKETHROUGH, md.HIGHLIGHT})
+
+    doc += bold_text
+    doc += italiced_text
+    doc += strikethrough_text
+    doc += highlighted_text
+    doc += all_together
+    doc += examples['stylised']
+    doc += md.HRule()
+
+    #%%  paragraph
+    paragraph = md.Paragraph(['Example paragraph containing ',
+                              md.Text('bolded text', {md.BOLD})])
+
+    doc += get_example('paragraph', paragraph)
+
+    #%% table
+    table = md.Table([['a', 1, 'Python'],
+                      ['b', 2, 'Markdown']],
+                     ['First column', 'Second column', 'Third column'],
+                     [md.RIGHT, md.LEFT, md.CENTER])
+
+    doc += get_example('table', table)
+
+    #%% compact table
+    table = md.Table([['a', 1, 'Python'],
+                      ['b', 2, 'Markdown']],
+                     ['First column', 'Second column', 'Third column'],
+                     [md.RIGHT, md.LEFT, md.CENTER],
+                     True)
+
+    doc += 'You can select compact mode at the table object creation'
+    doc += get_example('compact table', table)
+
+    #%% table compact attribute
+    table.compact = True
+
+    doc += md.Paragraph(['or later by changing the attribute ',
+                         md.Code('compact')])
+    doc += examples['table compact attribute']
+
+    #%% listing
+    listing = md.Listing(['Just normal text',
+                          md.Text('some stylised text', {md.ITALIC}),
+                          md.Checkbox('Listings can include checkboxes', False),
+                          md.Checkbox('Checked and unchecked option available', True),
+                          ('Sublist by using a tuple',
+                            md.Listing(['first', 'second'], md.ORDERED))],
+                          md.UNORDERED)
+
+    doc += get_example('listing', listing)
+
+    #%% checklist
+    checklist = md.make_checklist([('unchecked box', False),
+                                   ('checked box', True),
+                                   ('done', True)])
+
+    doc += get_example('checklist', checklist)
+    #%% link
+    link = md.Link('https://www.markdownguide.org', 'Link to Markdown Guide')
+
+    doc += get_example('link', link)
+
+    #%% codeblock
+    codeblock = md.CodeBlock('import yamdog as md\n\ndoc = md.Document([])',
+                             'python')
+
+    doc += get_example('codeblock', codeblock)
+
+    #%% code
+    code = md.Code('python != markdown')
+
+    doc += get_example('code', code)
+
+    #%% Image
+    # image = md.Image()
+
+    #%% address
+    address = md.Link('https://www.markdownguide.org')
+
+    doc += get_example('address', address)
+
+    #%% quote block
+    quoteblock = md.Quote('Quote block supports\nmultiple lines')
+
+    doc += get_example('quote block', quoteblock)
+
+    doc += md.Heading('Combining elements into a document', 3)
+
+    #%% calling document
+    document = md.Document([heading, link, paragraph, listing])
+
+    doc += 'Initialising Document with list of elements'
+    doc += examples['calling document']
+
+    #%% from empty document
+    document = md.Document([])
+    document += heading
+    document += link
+    document += paragraph
+    document += listing
+
+    doc += 'adding elements into a document'
+    doc += examples['from empty document']
+
+    #%% document by adding
+    document = heading + link + paragraph + listing
+
+    doc += 'adding elements together into a document'
+    doc += examples['document by adding']
+
+    #%% document concatenation
+    document1 = md.Document([heading, link])
+    document2 = md.Document([paragraph, listing])
+    document = document1 + document2
+
+    doc += 'Adding two documents together'
+    doc += examples['document concatenation']
+
+    doc += md.Text('Markdown source', {md.ITALIC})
+    doc += md.CodeBlock(document, 'markdown')
+    doc += md.Text('Rendered result', {md.ITALIC})
+    doc += document
+
+    return doc
+#=======================================================================
+def make_quick_start_guide(name, pypiname, source):
+    doc = md.Document([
+        md.Heading('Quick start guide', 1),
+        "Here's how you can start automatically generating Markdown documents",
+        md.Heading('The first steps', 2),
+        '',
+        md.Heading('Install', 3),
+        f'''Install {name} with pip.
+        {name} uses only Python standard library so it has no additional dependencies.''',
+        md.CodeBlock(f'pip install {pypiname}'),
+        md.Heading('Import', 3),
+        f'''Import name is the same as install name, {pypiname}.''',
+        md.CodeBlock(f'import {pypiname}', 'python'),
+        md.Paragraph(['Since the package is accessed often, I use abbreviation',
+                      md.Code('md'),
+                      ' for MarkDown. The abbreviation is used throughout this document.']),
+        md.CodeBlock(f'import {pypiname} as md', 'python'),
+        md.Heading('Using the package', 2),
+        f'There are two main things to building a Markdown document using {name}',
+        md.Listing(['Making elements',
+                    'Combining elements into a document'], md.ORDERED),
+        md.Paragraph(['You can call ',
+            md.Code('str'),
+            ' on the element directly to get the markdown source']),
+        md.CodeBlock('markdown_source = str(element)', 'python'),
+        '''but most of the time you will compose the elements together into an
+        document''',
+        md.CodeBlock('markdown_source = str(document)', 'python')
+        ])
+    doc += make_examples(source)
+    return doc
+#=======================================================================
+re_heading = re.compile(r'^#* .*$')
+
+def parse_md_element(text: str):
+    if match := re_heading.match(text):
+        hashes, content = match[0].split(' ', 1)
+        return md.Heading(content, len(hashes))
+    else:
+        return md.Raw(text)
+#-----------------------------------------------------------------------
+def parse_md(text: str):
+    return md.Document([parse_md_element(item.strip())
+                        for item in text.split('\n\n')])
+#-----------------------------------------------------------------------
+def make_changelog(level: int):
+    doc = md.Document([md.Heading('Changelog', level, in_TOC = False)])
+    changelog = parse_md(PATH_CHANGELOG.read_text())
+    if changelog:
+        if (latest := changelog.content[0]).content.split(' ', 1)[0] == VERSION:
+            latest.content = f'{VERSION} {datetime.date.today().isoformat()}'
+        else:
+            raise ValueError('Changelog not up to date')
+
+        PATH_CHANGELOG.write_text(str(changelog) + '\n')
+
+        for item in changelog:
+            if isinstance(item, md.Heading):
+                item.level = level + 1
+                item.in_TOC = False
+
+        doc += changelog
+
+    return doc
+#=======================================================================
+def make_further_reading():
+    basic_syntax_link = md.Link('https://www.markdownguide.org/basic-syntax/',
+                                'basic syntax guide',
+                                '')
+    extended_syntax_link = md.Link('https://www.markdownguide.org/basic-syntax/',
+                                   'extended syntax guide',
+                                   '')
+
+    doc = md.Document([md.Heading('Further reading', 1)])
+    doc += md.Listing([basic_syntax_link, extended_syntax_link], md.UNORDERED)
+    return doc
+#=======================================================================
+def make_annexes(source):
+    doc = md.Document([md.Heading('Annexes', 1)])
+    doc += md.Heading('Annex 1: README Python source', 2)
+    doc += '''And here the full source code that wrote this README.
+            This can serve as a more advanced example of what this is
+            capable of.'''
+    doc += md.Link('https://github.com/Limespy/YAMDOG/blob/main/readme.py',
+                   'The python file can also be found here')
+    doc += md.CodeBlock(source, 'python')
+    return doc
+#=======================================================================
+def make(name, pypiname, source):
+    # Setup for the badges
+    shields_url = 'https://img.shields.io/'
+
+    pypi_project_url = f'https://pypi.org/project/{pypiname}'
+    pypi_badge_info = (('v', 'PyPI Package latest release'),
+                       ('wheel', 'PyPI Wheel'),
+                       ('pyversions', 'Supported versions'),
+                       ('implementation', 'Supported implementations'))
+    pypi_badges = [md.Link(pypi_project_url,
+                           md.Image(f'{shields_url}pypi/{code}/{pypiname}.svg',
+                                    desc), '')
+                   for code, desc in pypi_badge_info]
+
+    # Starting the document
+    doc = md.Document([
+        md.Heading(f'Overview of {name}', 1, in_TOC = False),
+        md.Paragraph(pypi_badges, '\n'),
+        'Yet Another Markdown Only Generator',
+        md.Heading(f'What is {name}?', 2, in_TOC = False),
+        f'''{name} is toolkit for creating Markdown text using Python.
+        Markdown is a light and relatively simple markup language.''',
+        md.Heading('Table of Content', 3, in_TOC = False),
+        md.TOC()
+        ])
+    source = pathlib.Path(__file__).read_text('utf8')
+    doc += make_quick_start_guide(name, pypiname, source)
+    doc += make_changelog(level = 1)
+    doc += make_further_reading()
+    doc += md.HRule()
+    doc += make_annexes(source)
+    return doc
+#=======================================================================
+def main():
+    try:
+        import tomllib
+    except ModuleNotFoundError:
+        import tomli as tomllib # type: ignore
+
+    pyproject = tomllib.loads(PATH_PYPROJECT.read_text())
+    master_info = pyproject['master-info']
+    package_name = master_info["package_name"]
+    full_name = master_info.get("full_name",
+                                package_name.replace('-', ' ').capitalize())
+    description = master_info['description']
+
+    doc = make(full_name, package_name, description)
+    PATH_README.write_text(str(doc) + '\n')
+#=======================================================================
+if __name__ == '__main__':
+    main()
+
+```
+
+[1]: <https://pypi.org/project/yamdog> ""
+[2]: <https://www.markdownguide.org/basic-syntax/> ""
```

### Comparing `yamdog-0.4.0.14/src/yamdog/dataclass_validate.py` & `yamdog-0.5.0/src/yamdog/dataclass_validate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,103 +1,124 @@
-
-from dataclasses import *
-_dataclass_std = dataclass
-del dataclass
-import typing as _typing
-
-def _basic(fieldtype, value: str) -> list[str]:
-    return ([] if isinstance(value, fieldtype) else 
-            [f"{value!r} is type '{type(value).__qualname__}',"
-             f" not '{fieldtype.__qualname__}'"])
-#──────────────────────────────────────────────────────────────────────────────
-def _tuple(fieldtypes, values: str) -> list[str]:
-    if not fieldtypes and not values:
-        return []
-    if len(fieldtypes) == 2 and fieldtypes[-1] is Ellipsis:
-        return _iterate(fieldtypes[0], values)
-    if len(fieldtypes) != len(values):
-        return [f'Length of the tuple {values!r} not {len(fieldtypes)}']
-    errormessages = []
-    for _type, subvalue in zip(fieldtypes, values):
-        errormessages += _validate(_type, subvalue)
-    return errormessages
-#──────────────────────────────────────────────────────────────────────────────
-def _iterate(fieldtype, values: str) -> list[str]:
-    errormessages = []
-    for item in values:
-        errormessages += _validate(fieldtype, item)
-    return errormessages
-#──────────────────────────────────────────────────────────────────────────────
-def _dict(fieldtypes, values) -> list[str]:
-    return (_iterate(fieldtypes[0], values.keys())
-            + _iterate(fieldtypes[1], values.values()))
-#──────────────────────────────────────────────────────────────────────────────
-def _generic_alias(fieldtype, value: str) -> list[str]:
-    basetype = fieldtype.__origin__
-    if errormessage := _basic(basetype, value):
-        return errormessage
-    if basetype is tuple:
-        return _tuple(fieldtype.__args__, value)
-    if (basetype is set or basetype is list) and value:
-        return _iterate(fieldtype.__args__[0], value)
-    if basetype is dict and value:
-        return _dict(fieldtype.__args__, value)
-    return []
-#──────────────────────────────────────────────────────────────────────────────
-def _union(fieldtypes: tuple[type, ...], value: str) -> list[str]:
-    errormessages = []
-    for _type in fieldtypes:
-        if not (errormessage := _validate(_type, value)):
-            return []
-        errormessages += errormessage
-    return errormessages
-#──────────────────────────────────────────────────────────────────────────────
-def _validate(fieldtype, value: str) -> list[str]:
-    if fieldtype == _typing.Any:
-        return []
-    if isinstance(fieldtype, _typing._UnionGenericAlias): # type: ignore
-        return _union(fieldtype.__args__, value)
-    if isinstance(fieldtype, _typing.GenericAlias): # type: ignore
-        return _generic_alias(fieldtype, value)
-    return _basic(fieldtype, value)
-#──────────────────────────────────────────────────────────────────────────────
-def _validate_fields(obj, ExceptionType = TypeError) -> None:
-    '''Checks types of the attributes of the class
-    '''
-    errormessages = []
-    for name, field in obj.__dataclass_fields__.items():
-        if messages := _validate(field.type, getattr(obj, name)):
-            errormessages.append(f'{name}: {" ".join(messages)}')
-    if errormessages:
-        errormessages.insert(0, f'{obj.__class__.__qualname__} parameters not matching types')
-        raise ExceptionType('\n    - '.join(errormessages))
-#──────────────────────────────────────────────────────────────────────────────
-def dataclass(cls=None, /, *, validate: _typing.Optional[str] = None, **kwargs): # type: ignore
-    '''Validate after 'init', 'post_init' or not at all (`None`)
-    '''
-
-    if validate is None:
-        return _dataclass_std(cls, **kwargs)
-    if not (validate == 'middle' or validate == 'last'):
-        raise ValueError(f'validate was {repr(validate)}, not "middle", or "last"')
-    # cls is None
-    dataclass_wrapper = _dataclass_std(cls, **kwargs)
-    #─────────────────────────────────────────────────────────────────────────
-    # Creating a new wrapper to wrap the original dataclass wrapper
-    # to wrap init or post_init 
-    def decoratorwrap(cls):
-        cls = dataclass_wrapper(cls)
-        method_name = ('__post_init__'
-                       if validate == 'last' and hasattr(cls, '__post_init__')
-                       else '__init__')
-
-        original_method = getattr(cls, method_name)
-        #─────────────────────────────────────────────────────────────────────
-        def validation_wrap(self, *args, **kwargs) -> None:
-            original_method(self, *args, **kwargs)
-            _validate_fields(self)
-        #─────────────────────────────────────────────────────────────────────
-        setattr(cls, method_name, validation_wrap)
-
-        return cls
-    #─────────────────────────────────────────────────────────────────────────
-    return decoratorwrap
+from collections.abc import Collection as _Collection
+from collections.abc import Mapping as _Mapping
+from dataclasses import *
+from dataclasses import dataclass as _dataclass_std
+from functools import wraps
+from typing import _UnionGenericAlias # type: ignore
+from typing import Any as _Any
+from typing import Callable as _Callable
+from typing import GenericAlias as _GenericAlias # type: ignore
+from typing import Iterable as _Iterable
+from typing import Protocol as _Protocol
+del dataclass # type: ignore
+#──────────────────────────────────────────────────────────────────────────────
+class _DataclassWrapped(_Protocol):
+    __dataclass_fields__: dict[str, Field]
+#──────────────────────────────────────────────────────────────────────────────
+def _basic(fieldtype, value: _Any) -> list[str]:
+    return ([] if isinstance(value, fieldtype) else
+            [f"{value!r} is type '{type(value).__qualname__}',"
+             f" not '{fieldtype.__qualname__}'"])
+#──────────────────────────────────────────────────────────────────────────────
+def _tuple(fieldtypes, values: _Any) -> list[str]:
+    if not fieldtypes and not values:
+        return []
+    if len(fieldtypes) == 2 and fieldtypes[-1] is Ellipsis:
+        return _iterate(fieldtypes[0], values)
+    if len(fieldtypes) != len(values):
+        return [f'Length of the tuple {values!r} not {len(fieldtypes)}']
+    errormessages = []
+    for fieldtype, subvalue in zip(fieldtypes, values):
+        errormessages.extend(_validate(fieldtype, subvalue))
+    return errormessages
+#──────────────────────────────────────────────────────────────────────────────
+def _iterate(fieldtype: type, values: _Iterable[_Any]) -> list[str]:
+    errormessages = []
+    for item in values:
+        errormessages.extend(_validate(fieldtype, item))
+    return errormessages
+#──────────────────────────────────────────────────────────────────────────────
+def _generic_alias(fieldtype, value: _Any) -> list[str]:
+    basetype = fieldtype.__origin__
+    if errormessage := _basic(basetype, value):
+        return errormessage
+    if issubclass(basetype, tuple):
+        return _tuple(fieldtype.__args__, value)
+    if issubclass(basetype, dict) and value:
+        keytype, valuetype = fieldtype.__args__
+        return (_iterate(keytype, value.keys())
+                + _iterate(valuetype, value.values()))
+    if issubclass(basetype, _Collection) and value:
+        return _iterate(fieldtype.__args__[0], value)
+    return []
+#──────────────────────────────────────────────────────────────────────────────
+def _union(fieldtypes: tuple[type, ...], value: _Any) -> list[str]:
+    '''If one of the types in the union matches'''
+    errormessages = []
+    for _type in fieldtypes:
+        if not (errormessage := _validate(_type, value)):
+            return []
+        errormessages.extend(errormessage)
+    return errormessages
+#──────────────────────────────────────────────────────────────────────────────
+def _validate(fieldtype: type, value: _Any) -> list[str]:
+    if fieldtype == _Any:
+        return []
+    if isinstance(fieldtype, _UnionGenericAlias):
+        return _union(fieldtype.__args__, value)
+    if isinstance(fieldtype, _GenericAlias):
+        return _generic_alias(fieldtype, value)
+    return _basic(fieldtype, value)
+#──────────────────────────────────────────────────────────────────────────────
+def _validate_fields(obj: _DataclassWrapped) -> None:
+    '''Checks types of the attributes of the class
+    '''
+    errormessages = []
+    for name, field in obj.__dataclass_fields__.items():
+        try:
+            attribute = getattr(obj, name)
+        except AttributeError:
+            continue
+        if messages := _validate(field.type, attribute):
+            errormessages.append(f'{name}: {" ".join(messages)}')
+    if errormessages:
+        errormessages.insert(0,
+                             f'{obj.__class__.__qualname__} '
+                             'parameters not matching types')
+        raise TypeError('\n    '.join(errormessages))
+#──────────────────────────────────────────────────────────────────────────────
+def validate(cls: type):
+    '''Validate after 'init', 'post_init' or not at all (`None`)
+    '''
+    #─────────────────────────────────────────────────────────────────────────
+    # Creating a new wrapper to wrap the original dataclass wrapper
+    # to wrap init or post_init
+
+    if hasattr(cls, '__post_init__'):
+        method_name = '__post_init__'
+        original_method = getattr(cls, method_name)
+        @wraps(original_method)
+        def validation_wrap(self, *args, **kwargs) -> None:
+            _validate_fields(self)
+            original_method(self, *args, **kwargs)
+    else:
+        method_name = '__init__'
+        original_method = getattr(cls, method_name)
+        @wraps(original_method)
+        def validation_wrap(self, *args, **kwargs) -> None:
+            original_method(self, *args, **kwargs)
+            _validate_fields(self)
+    #─────────────────────────────────────────────────────────────────────
+    setattr(cls, method_name, validation_wrap)
+    return cls
+_validation_function = validate
+#──────────────────────────────────────────────────────────────────────────────
+def dataclass(cls = None, /, *, validate: bool = False, **kwargs # type: ignore
+              ) -> _Callable:
+    '''Validate after 'init', 'post_init' or not at all (`None`)
+    '''
+    if not validate:
+        return _dataclass_std(cls, **kwargs)
+    # cls is None
+    dataclass_wrapper = _dataclass_std(cls, **kwargs)
+
+    return lambda cls: _validation_function(dataclass_wrapper(cls))
```

