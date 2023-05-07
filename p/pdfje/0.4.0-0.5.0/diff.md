# Comparing `tmp/pdfje-0.4.0.tar.gz` & `tmp/pdfje-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfje-0.4.0.tar", max compression
+gzip compressed data, was "pdfje-0.5.0.tar", max compression
```

## Comparing `pdfje-0.4.0.tar` & `pdfje-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,28 @@
--rw-r--r--   0        0        0     1556 2023-04-10 14:21:01.064991 pdfje-0.4.0/CHANGELOG.rst
--rw-r--r--   0        0        0     4556 2023-04-10 14:21:01.065651 pdfje-0.4.0/README.rst
--rw-r--r--   0        0        0     1458 2023-04-10 14:21:01.069311 pdfje-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2111 2023-04-10 14:21:01.107672 pdfje-0.4.0/src/pdfje/__init__.py
--rw-r--r--   0        0        0     6345 2023-04-10 14:21:01.107957 pdfje-0.4.0/src/pdfje/atoms.py
--rw-r--r--   0        0        0    13623 2023-04-10 14:21:01.108674 pdfje-0.4.0/src/pdfje/common.py
--rw-r--r--   0        0        0    12675 2023-04-10 14:21:01.108836 pdfje-0.4.0/src/pdfje/document.py
--rw-r--r--   0        0        0     8139 2023-04-10 14:21:01.108951 pdfje-0.4.0/src/pdfje/draw.py
--rw-r--r--   0        0        0      155 2023-04-10 14:21:01.109085 pdfje-0.4.0/src/pdfje/fonts/__init__.py
--rw-r--r--   0        0        0   407594 2023-04-10 14:21:01.109836 pdfje-0.4.0/src/pdfje/fonts/builtins.py
--rw-r--r--   0        0        0     5994 2023-04-10 14:21:01.109999 pdfje-0.4.0/src/pdfje/fonts/common.py
--rw-r--r--   0        0        0    13573 2023-04-10 14:21:01.110157 pdfje-0.4.0/src/pdfje/fonts/embed.py
--rw-r--r--   0        0        0     2058 2023-04-10 14:21:01.110267 pdfje-0.4.0/src/pdfje/fonts/registry.py
--rw-r--r--   0        0        0     1789 2023-04-10 14:21:01.110446 pdfje-0.4.0/src/pdfje/layout.py
--rw-r--r--   0        0        0     3275 2023-04-10 14:21:01.110601 pdfje-0.4.0/src/pdfje/ops.py
--rw-r--r--   0        0        0        0 2022-10-26 19:42:23.131874 pdfje-0.4.0/src/pdfje/py.typed
--rw-r--r--   0        0        0     7333 2023-04-10 14:21:01.110776 pdfje-0.4.0/src/pdfje/style.py
--rw-r--r--   0        0        0     5872 2023-04-10 14:21:01.110931 pdfje-0.4.0/src/pdfje/text.py
--rw-r--r--   0        0        0    18193 2023-04-10 14:21:01.111118 pdfje-0.4.0/src/pdfje/typeset.py
--rw-r--r--   0        0        0        0 2023-04-10 14:21:01.111181 pdfje-0.4.0/src/pdfje/vendor/__init__.py
--rw-r--r--   0        0        0    13291 2023-04-10 14:21:01.111371 pdfje-0.4.0/src/pdfje/vendor/get_kerning_pairs.py
--rw-r--r--   0        0        0     5495 1970-01-01 00:00:00.000000 pdfje-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     2014 2023-05-06 09:48:17.480279 pdfje-0.5.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1088 2023-04-10 17:40:34.849969 pdfje-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5274 2023-05-07 11:17:46.799876 pdfje-0.5.0/README.rst
+-rw-r--r--   0        0        0     1524 2023-05-06 09:48:17.486248 pdfje-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      416 2023-05-06 09:48:17.491679 pdfje-0.5.0/src/pdfje/__init__.py
+-rw-r--r--   0        0        0     6446 2023-05-06 09:48:17.492169 pdfje-0.5.0/src/pdfje/atoms.py
+-rw-r--r--   0        0        0    13796 2023-05-06 09:48:17.492624 pdfje-0.5.0/src/pdfje/common.py
+-rw-r--r--   0        0        0    11441 2023-05-06 09:48:17.493043 pdfje-0.5.0/src/pdfje/document.py
+-rw-r--r--   0        0        0    11771 2023-05-06 09:48:17.493430 pdfje-0.5.0/src/pdfje/draw.py
+-rw-r--r--   0        0        0      263 2023-05-06 09:48:17.493801 pdfje-0.5.0/src/pdfje/fonts/__init__.py
+-rw-r--r--   0        0        0   407594 2023-04-13 18:41:37.488082 pdfje-0.5.0/src/pdfje/fonts/builtins.py
+-rw-r--r--   0        0        0     5882 2023-05-06 09:48:17.494173 pdfje-0.5.0/src/pdfje/fonts/common.py
+-rw-r--r--   0        0        0    13635 2023-05-06 09:48:17.494605 pdfje-0.5.0/src/pdfje/fonts/embed.py
+-rw-r--r--   0        0        0     2027 2023-05-06 09:48:17.495048 pdfje-0.5.0/src/pdfje/fonts/registry.py
+-rw-r--r--   0        0        0     9008 2023-05-06 09:48:17.495450 pdfje-0.5.0/src/pdfje/layout.py
+-rw-r--r--   0        0        0        0 2022-10-26 19:42:23.131874 pdfje-0.5.0/src/pdfje/py.typed
+-rw-r--r--   0        0        0    11078 2023-05-06 09:48:17.495830 pdfje-0.5.0/src/pdfje/style.py
+-rw-r--r--   0        0        0        0 2023-05-06 09:48:17.495981 pdfje-0.5.0/src/pdfje/text.py
+-rw-r--r--   0        0        0        0 2023-05-06 09:48:17.496202 pdfje-0.5.0/src/pdfje/typeset/__init__.py
+-rw-r--r--   0        0        0     7663 2023-05-06 09:48:17.496507 pdfje-0.5.0/src/pdfje/typeset/common.py
+-rw-r--r--   0        0        0     1800 2023-05-06 09:48:17.496726 pdfje-0.5.0/src/pdfje/typeset/hyphens.py
+-rw-r--r--   0        0        0     4626 2023-05-06 09:48:17.497064 pdfje-0.5.0/src/pdfje/typeset/lines.py
+-rw-r--r--   0        0        0    13186 2023-05-06 09:48:17.497402 pdfje-0.5.0/src/pdfje/typeset/words.py
+-rw-r--r--   0        0        0     1109 2023-05-06 09:48:17.497690 pdfje-0.5.0/src/pdfje/units.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:21:01.111181 pdfje-0.5.0/src/pdfje/vendor/__init__.py
+-rw-r--r--   0        0        0    13251 2023-05-06 09:48:17.498176 pdfje-0.5.0/src/pdfje/vendor/get_kerning_pairs.py
+-rw-r--r--   0        0        0    35490 2023-05-06 09:48:17.498741 pdfje-0.5.0/src/pdfje/vendor/hyphenate.py
+-rw-r--r--   0        0        0     6291 1970-01-01 00:00:00.000000 pdfje-0.5.0/PKG-INFO
```

### Comparing `pdfje-0.4.0/CHANGELOG.rst` & `pdfje-0.5.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 Changelog
 =========
 
+0.5.0 (2023-??-??)
+------------------
+
+**Breaking**
+
+- 🪆 Expose most classes from submodules instead of root
+  (e.g. ``pdfje.Rect`` becomes ``pdfje.draw.Rect``).
+  The new locations can be found in the API documentation.
+- ``Rule`` ``padding`` attribute renamed to ``margin``.
+
+**Added**
+
+- 📰 Support for horizontal alignment and justification of text.
+- 🫸 Support for indenting the first line of a paragraph.
+- ✂️  Automatic hyphenation of text.
+
 0.4.0 (2023-04-10)
 ------------------
 
 A big release with lots of new features and improvements.
 Most importantly, the page layout engine is now complete and
 can be used to create multi-page/column documents.
 
 **Added**
 
-- ✂️  Automatic layout of multi-style text into lines, columns, and pages
+- 📖 Automatic layout of multi-style text into lines, columns, and pages
 - 🔬 Automatic kerning for supported fonts
 - 🖌️ Support for drawing basic shapes
 - 🎨 Additional text styling options
 - 📦 Make fonttools dependency optional
 - 📏 Horizontal rule element
 
 **Documentation**
```

### Comparing `pdfje-0.4.0/README.rst` & `pdfje-0.5.0/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,87 +1,95 @@
 🌷 pdf'je
 =========
 
-.. image:: https://img.shields.io/pypi/v/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/v/pdfje.svg?style=flat-square&color=blue
    :target: https://pypi.python.org/pypi/pdfje
 
-.. image:: https://img.shields.io/pypi/l/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/pyversions/pdfje.svg?style=flat-square
    :target: https://pypi.python.org/pypi/pdfje
 
-.. image:: https://img.shields.io/pypi/pyversions/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/l/pdfje.svg?style=flat-square&color=blue
    :target: https://pypi.python.org/pypi/pdfje
 
+.. image:: https://img.shields.io/badge/mypy-strict-forestgreen?style=flat-square
+   :target: https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-strict
+
+.. image:: https://img.shields.io/badge/coverage-99%25-forestgreen?style=flat-square
+   :target: https://github.com/ariebovenberg/pdfje
+
+.. image::  https://img.shields.io/github/actions/workflow/status/ariebovenberg/pdfje/tests.yml?branch=main&style=flat-square
+   :target: https://github.com/ariebovenberg/pdfje
+
 .. image:: https://img.shields.io/readthedocs/pdfje.svg?style=flat-square
    :target: http://pdfje.readthedocs.io/
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square
-   :target: https://github.com/psf/black
-
------
+..
 
   **pdf·je** [`🔉 <https://upload.wikimedia.org/wikipedia/commons/a/ac/Nl-pdf%27je.ogg>`_ PDF·yuh] (noun) Dutch for 'small PDF'
 
-Write beautiful PDFs in declarative Python.
+**Write beautiful PDFs in declarative Python.**
 
-Currently in active development. See the roadmap_ for supported features.
-Leave a ⭐️ on GitHub if you're interested how this develops!
+*(Currently in active development. Leave a* ⭐️ *on GitHub if you're interested how this develops!)*
 
-Why?
-----
+Features
+--------
 
-There are many PDF libraries for Python, but none of them
-have these features:
+Pdf'je distinguishes itself with the following combination of features:
 
 🧩 Declarative API
 ~~~~~~~~~~~~~~~~~~
 
-In most PDF writers, you first create various empty objects and
+In most PDF writers, you first create empty objects and
 then mutate them with methods like ``addText()``,
-all while changing the state of the writer with methods like ``setFont()``.
+all while changing the state with methods like ``setFont()``.
 **Pdf'je** is different. You describe the document you want to write,
-and the library takes care of the details. No state to manage, no mutations.
+and it takes care of the details. No state to manage, no mutations.
 This makes your code easier to reuse and reason about.
 
-📐 Polished typography
-~~~~~~~~~~~~~~~~~~~~~~
-
-Legibility counts. And `kerning <https://en.wikipedia.org/wiki/Kerning>`_
-— i.e. adjusting the spacing between letters — is a key part of this.
-Automatic kerning is supported everywhere, from web browsers to word processors.
-However, most PDF writers don't support it.
-By using font metrics to calculate the correct kerning,
-**pdf'je** helps you write documents that look great.
-
-🎈 Small footprint
-~~~~~~~~~~~~~~~~~~
-
-PDF supports many features, but most of the time you only need a few.
-Why install many dependencies — just to write a simple document?
-Not only is **pdf'je** pure-Python, it allows you to
-install only the dependencies you need.
-
-
-Quickstart
-----------
-
-Getting text onto paper is super easy:
-
 .. code-block:: python
 
   from pdfje import Document
   Document("Olá Mundo!").write("hello.pdf")
 
 See `the tutorial <https://pdfje.rtfd.io/en/latest/tutorial.html>`_
 for a complete overview of features, including:
 
 - Styling text including font, size, and color
 - Automatic layout of text into one or more columns
 - Builtin and embedded fonts
 - Drawing basic shapes
 
+See the roadmap_ for supported features.
+
+📖 Decent typography
+~~~~~~~~~~~~~~~~~~~~
+
+Legibility counts — and `kerning <https://en.wikipedia.org/wiki/Kerning>`_
+is a key part of this.
+We've come to expect it everywhere, from web browsers to word processors.
+However, most PDF writers don't support it.
+By using the proper metadata,
+**pdf'je** helps you write documents that look great.
+
+.. image:: https://github.com/ariebovenberg/pdfje/raw/main/sample.png
+   :alt: Sample document with two columns of text
+
+🎈 Small footprint
+~~~~~~~~~~~~~~~~~~
+
+The PDF format supports many features, but most of the time you only need a few.
+Why install many dependencies — just to write a simple document?
+Not only is **pdf'je** pure-Python, it allows you to
+install only the dependencies you need.
+
+.. code-block:: bash
+
+  pip install pdfje                 # no dependencies
+  pip install pdfje[fonts, hyphens] # embedded fonts and improved hyphenation
+
 .. _roadmap:
 
 Roadmap
 -------
 
 **Pdf'je** is still in active development,
 so it is not yet feature-complete.
@@ -91,18 +99,20 @@
 
 ✅ = implemented, 🚧 = planned, ❌ = not planned
 
 - Typesetting
     - ✅ Automatic kerning
     - ✅ Wrapping text into lines, columns, and pages
     - ✅ Page sizes
-    - 🚧 Centering text
-    - 🚧 Justification
-    - 🚧 Hyphenation
-    - 🚧 Avoiding orphaned lines
+    - ✅ Centering text
+    - ✅ Justification
+    - ✅ Hyphenation
+    - 🚧 Avoiding orphaned/widowed lines
+    - 🚧 Tex-style line breaking
+    - 🚧 Broader unicode support in text wrapping
 - Drawing operations
     - ✅ Lines
     - ✅ Rectangles
     - ✅ Circles, ellipses
     - 🚧 Arbitrary paths, fills, and strokes
 - Text styling
     - ✅ Font and size
@@ -111,57 +121,43 @@
     - ✅ Bold, italic
     - 🚧 Underline and strikethrough
     - 🚧 Superscript and subscript
     - ❌ Complex fill patterns
 - 🚧 Images
 - 🚧 Bookmarks and links
 - 🚧 Tables
+- 🚧 Bullet/numbered lists
 - 🚧 Inline markup with Markdown (Commonmark/MyST)
 - ❌ Emoji
 - ❌ Tables of contents
 - ❌ Forms
 - ❌ Annotations
 
-Installation
-------------
-
-It's available on PyPI.
-
-.. code-block:: bash
-
-  pip install pdfje
-
-By default, no additional dependencies are installed.
-If you'd like to use custom fonts, you'll need ``fontTools``,
-which is included in the ``[fonts]`` extras:
-
-.. code-block:: bash
-
-   pip install pdfje[fonts]
-
 License
 -------
 
 This library is licensed under the terms of the MIT license.
 It also includes short scripts from other projects (see ``pdfje/vendor``),
-which are also MIT licensed.
+which are either also MIT licensed, or in the public domain.
 
 Contributing
 ------------
 
 Here are some useful tips for developing in the ``pdfje`` codebase itself:
 
 - Install dependencies with ``poetry install``.
 - To write output files during tests, use ``pytest --output-path=<outpur-dir>``
 - To also run more comprehensive but 'slow' tests, use ``pytest --runslow``
 
-Alternatives
-------------
+Acknowledgements
+----------------
 
-If pdf'je doesn't suit your needs, here are some other options:
+**pdf'je** is inspired by the following projects.
+If you're looking for a PDF writer, you may want to check them out as well:
 
-- PyFPDF
-- ReportLab
-- WeasyPrint
-- borb
-- wkhtmltopdf
-- pydyf
+- `python-typesetting <https://github.com/brandon-rhodes/python-typesetting>`_
+- `fpdf2 <https://pyfpdf.github.io/fpdf2/index.html>`_
+- `ReportLab <https://www.reportlab.com/>`_
+- `WeasyPrint <https://weasyprint.org/>`_
+- `borb <httpsL//github.com/jorisschellekens/borb/>`_
+- `wkhtmltopdf <https://wkhtmltopdf.org/>`_
+- `pydyf <https://github.com/CourtBouillon/pydyf>`_
```

### Comparing `pdfje-0.4.0/pyproject.toml` & `pdfje-0.5.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pdfje"
-version = "0.4.0"
+version = "0.5.0"
 description = "Tiny PDF writer"
 authors = ["Arie Bovenberg <a.c.bovenberg@gmail.com>"]
 license = "MIT"
 classifiers = [
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -18,17 +18,19 @@
 include = ["CHANGELOG.rst", "README.rst"]
 repository = "https://github.com/ariebovenberg/pdfje"
 keywords = ["pdf"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 fonttools = {version="^4.38.0", optional=true}
+pyphen = {version=">=0.13.0", optional=true}
 
 [tool.poetry.extras]
 fonts = ["fonttools"]
+hyphens = ["pyphen"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
 pytest-benchmark = "^4.0.0"
 hypothesis = "^6.68.2"
```

### Comparing `pdfje-0.4.0/src/pdfje/atoms.py` & `pdfje-0.5.0/src/pdfje/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,19 @@
     value: float
 
     def write(self) -> Iterable[bytes]:
         assert isfinite(self.value), "NaN and Inf not supported"
         return (b"%g" % self.value,)
 
 
+# NOTE: this name avoids confusion with typing.LiteralString
 @add_slots
 @dataclass(frozen=True)
-class LiteralString(Atom):
+class LiteralStr(Atom):
+    "See PDF32000-1:2008 (7.3.4.2)"
     value: bytes
 
     # FUTURE: support UTF-16BOM, but in a way that makes it explicit that
     # this does not support usage in text streams.
     # How to prevent accidential UTF-16BOM?
     def write(self) -> Iterable[bytes]:
         return (b"(", _escape(self.value), b")")
@@ -245,15 +247,15 @@
     b"\b": b"\\b",
     b"\f": b"\\f",
     b"(": b"\\(",
     b")": b"\\)",
 }
 
 
-def _replace_with_escape(m: re.Match) -> bytes:
+def _replace_with_escape(m: re.Match[bytes]) -> bytes:
     return _STRING_ESCAPES[m.group()]
 
 
 _escape = partial(
     re.compile(b"(%b)" % b"|".join(map(re.escape, _STRING_ESCAPES))).sub,
     _replace_with_escape,
 )
```

### Comparing `pdfje-0.4.0/src/pdfje/common.py` & `pdfje-0.5.0/src/pdfje/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
+import enum
 from dataclasses import dataclass, fields
-from functools import partial, wraps
-from itertools import chain
-from operator import itemgetter, mul
+from functools import wraps
+from itertools import chain, tee
+from operator import itemgetter
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     Generic,
     Iterable,
     Iterator,
@@ -16,30 +17,21 @@
     Sequence,
     TypeVar,
     final,
     no_type_check,
     overload,
 )
 
-Pt = float
+Pt = float  # not allowed to be inf or nan (math.isfinite)
 Char = str  # 1-character string
 Pos = int  # position within a string (index)
 HexColor = str  # 6-digit hex color, starting with `#`. e.g. #ff0000
+Streamable = Iterable[bytes]  # PDF stream content
 
 flatten = chain.from_iterable
-inch: Callable[[float], Pt] = partial(mul, 72)
-inch.__doc__ = "Convert inches to points"
-cm: Callable[[float], Pt] = partial(mul, 28.346456692913385)
-cm.__doc__ = "Convert centimeters to points"
-mm: Callable[[float], Pt] = partial(mul, 2.8346456692913385)
-mm.__doc__ = "Convert millimeters to points"
-pc: Callable[[float], Pt] = partial(mul, 12)
-pc.__doc__ = "Convert picas to points"
-pt: Callable[[float], Pt] = lambda x: x
-pt.__doc__ = "No-op conversion. Can be used to make units explicit."
 first = itemgetter(0)
 second = itemgetter(1)
 Ordinal = int  # a unicode code point
 NonEmptySequence = Sequence
 NonEmtpyIterator = Iterator
 
 Tclass = TypeVar("Tclass", bound=type)
@@ -54,14 +46,37 @@
 def always(v: T) -> Callable[..., T]:
     return lambda *_, **__: v
 
 
 setattr_frozen = object.__setattr__
 
 
+class BranchableIterator(Iterator[T]):
+    __slots__ = ("_it",)
+
+    def __init__(self, it: Iterable[T]) -> None:
+        self._it = iter(it)
+
+    def __iter__(self) -> BranchableIterator[T]:
+        return self
+
+    def __next__(self) -> T:
+        return next(self._it)
+
+    def branch(self) -> BranchableIterator[T]:
+        # Performance note: as branches are garbage collected,
+        # the tee() objects appear to properly free their memory.
+        self._it, branch = tee(self._it)
+        return BranchableIterator(branch)
+
+    def prepend(self, i: T) -> BranchableIterator[T]:
+        self._it = prepend(i, self._it)
+        return self
+
+
 # adapted from github.com/ericvsmith/dataclasses
 # under its Apache 2.0 license.
 def add_slots(cls: Tclass) -> Tclass:  # pragma: no cover
     if "__slots__" in cls.__dict__:
         raise TypeError(f"{cls.__name__} already specifies __slots__")
     cls_dict = dict(cls.__dict__)
     field_names = tuple(f.name for f in fields(cls))
@@ -178,14 +193,29 @@
         return XY(self.x, self.y + y)
 
     def flip(self) -> XY:
         "Return a new XY with x and y swapped"
         return XY(self.y, self.x)
 
 
+class Align(enum.Enum):
+    """Horizontal alignment of text."""
+
+    LEFT = 0
+    CENTER = 1
+    RIGHT = 2
+    JUSTIFY = 3
+
+    @staticmethod
+    def parse(align: Align | str) -> Align:
+        if isinstance(align, str):
+            return Align[align.upper()]
+        return align
+
+
 @add_slots
 @dataclass(frozen=True)
 class Sides(Sequence[float]):
     """Represents a set of four sides. Used for padding and margins."""
 
     top: Pt = 0
     right: Pt = 0
@@ -238,40 +268,14 @@
 
 
 SidesLike = (
     Sides | tuple[Pt, Pt, Pt, Pt] | tuple[Pt, Pt, Pt] | tuple[Pt, Pt] | Pt
 )
 
 
-A0 = XY(2380, 3368)
-A1 = XY(1684, 2380)
-A2 = XY(1190, 1684)
-A3 = XY(842, 1190)
-A4 = XY(595, 842)
-A5 = XY(420, 595)
-A6 = XY(297, 420)
-A7 = XY(210, 297)
-A8 = XY(148, 210)
-A0_landscape = A0.flip()
-A1_landscape = A1.flip()
-A2_landscape = A2.flip()
-A3_landscape = A3.flip()
-A4_landscape = A4.flip()
-A5_landscape = A5.flip()
-A6_landscape = A6.flip()
-A7_landscape = A7.flip()
-A8_landscape = A8.flip()
-letter = XY(612, 792)
-letter_landscape = letter.flip()
-legal = XY(612, 1008)
-legal_landscape = legal.flip()
-tabloid = XY(792, 1224)
-ledger = tabloid_landscape = tabloid.flip()
-
-
 @final
 @add_slots
 @dataclass(frozen=True, repr=False)
 class RGB(Sequence[float]):
     """Represents a color in RGB space, with values between 0 and 1.
 
     Common colors are available as constants:
@@ -359,29 +363,32 @@
 black = RGB(0, 0, 0)
 white = RGB(1, 1, 1)
 yellow = RGB(1, 1, 0)
 magenta = RGB(1, 0, 1)
 cyan = RGB(0, 1, 1)
 
 
+Tcall = TypeVar("Tcall", bound=Callable[..., Any])
+
+
 # This makes the generator function behave like a "classic coroutine"
 # as described in fluentpython.com/extra/classic-coroutines.
 # Such a coroutine doesn't output anything on the first `yield`.
 # This allows the caller to use the `.send()` method immediately.
-@no_type_check
-def skips_to_first_yield(func: T, /) -> T:
+def skips_to_first_yield(func: Tcall, /) -> Tcall:
     """Decorator which primes a generator func by calling the first next()"""
 
+    @no_type_check
     @wraps(func)
     def primer(*args, **kwargs):
         gen = func(*args, **kwargs)
         next(gen)
         return gen
 
-    return primer
+    return primer  # type: ignore[no-any-return]
 
 
 @add_slots
 @dataclass(frozen=True)
 class dictget(Generic[T, U]):
     _map: Mapping[T, U]
     default: U
@@ -478,23 +485,23 @@
     __f7: Callable[[T7], T8],
 ) -> Callable[[T1], T8]:
     ...
 
 
 @overload  # noqa: F811
 def pipe(
-    __f1: Callable,
-    __f2: Callable,
-    __f3: Callable,
-    __f4: Callable,
-    __f5: Callable,
-    __f6: Callable,
-    __f7: Callable,
-    *__fn: Callable,
-) -> Callable:
+    __f1: Callable[[Any], Any],
+    __f2: Callable[[Any], Any],
+    __f3: Callable[[Any], Any],
+    __f4: Callable[[Any], Any],
+    __f5: Callable[[Any], Any],
+    __f6: Callable[[Any], Any],
+    __f7: Callable[[Any], Any],
+    *__fn: Callable[[Any], Any],
+) -> Callable[[Any], Any]:
     ...
 
 
 def pipe(*__fs: Any) -> Any:  # noqa: F811
     """Create a new callable by piping several in succession
     Example
     -------
```

### Comparing `pdfje-0.4.0/src/pdfje/document.py` & `pdfje-0.5.0/src/pdfje/document.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,85 +9,46 @@
     IO,
     Callable,
     Generator,
     Iterable,
     Iterator,
     Literal,
     Sequence,
+    final,
     overload,
 )
 
-from . import atoms, ops
+from . import atoms
 from .atoms import OBJ_ID_PAGETREE, OBJ_ID_RESOURCES
 from .common import (
-    A4,
-    RGB,
     XY,
-    HexColor,
     Pt,
     Sides,
     SidesLike,
     add_slots,
     always,
-    black,
     flatten,
-    inch,
     setattr_frozen,
     skips_to_first_yield,
 )
 from .draw import Drawing
 from .fonts.registry import Registry
-from .layout import Block, Column, ColumnFill
+from .layout import Block, Column, ColumnFill, Paragraph
 from .style import Style, StyleFull, StyleLike
-from .text import Paragraph
+from .units import A4, inch
 
 _OBJ_ID_FIRST_PAGE: atoms.ObjectID = OBJ_ID_RESOURCES + 1
 _OBJS_PER_PAGE = 2
 
 Rotation = Literal[0, 90, 180, 270]
 
 
 @add_slots
-@dataclass(frozen=True, init=False)
-class Rule(Block):
-    """A :class:`Block` that draws a horizontal line."""
-
-    color: RGB
-    padding: Sides
-
-    def __init__(
-        self,
-        color: RGB | HexColor = black,
-        padding: SidesLike = Sides(6, 0, 6, 0),
-    ) -> None:
-        setattr_frozen(self, "color", RGB.parse(color))
-        setattr_frozen(self, "padding", Sides.parse(padding))
-
-    def layout(
-        self, __: Registry, fill: ColumnFill, ___: StyleFull
-    ) -> Generator[ColumnFill, Column, ColumnFill]:
-        top, right, bottom, left = self.padding
-        if fill.height_free < top + bottom:
-            fill = ColumnFill.new((yield fill))
-
-        y = fill.col.origin.y + fill.height_free - top
-        x = fill.col.origin.x + left
-        return fill.add(
-            ops.DrawLine(
-                XY(x, y),
-                XY(x + fill.col.width - left - right, y),
-                self.color,
-            ),
-            fill.height_free - top - bottom,
-        )
-
-
-@add_slots
 @dataclass(frozen=True)
-class FilledPage:
+class RenderedPage:
     rotate: Rotation
     size: XY
     stream: Iterable[bytes]
 
     def to_atoms(self, i: atoms.ObjectID) -> Iterable[atoms.Object]:
         yield i, atoms.Dictionary(
             (b"Type", atoms.Name(b"Page")),
@@ -96,19 +57,19 @@
             (b"Contents", atoms.Ref(i + 1)),
             (b"Resources", atoms.Ref(OBJ_ID_RESOURCES)),
             (b"Rotate", atoms.Int(self.rotate)),
         )
         yield i + 1, atoms.Stream(self.stream)
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Page:
-    """A single page within a document. Contains any iterable of drawings,
-    which are rendered in the order they are given.
+    """A single page within a document. Contains drawings at given positions.
 
     Example
     -------
 
     .. code-block:: python
 
        from pdfje import Page, Line, Rect, Text, A5
@@ -119,20 +80,21 @@
        ], size=A5)
 
     Parameters
     ----------
     content
         The drawings to render on the page.
     size
-        The size of the page in points.
-        Common page sizes are available as constants:
+        The size of the page in points. Common page sizes are available
+        as constants:
 
         .. code-block:: python
 
-        from pdfje import Page, A4, A5, A6, letter, legal, tabloid
+            from pdfje import Page, A4, A5, A6, letter, legal, tabloid
+
     rotate
         The rotation of the page in degrees.
     margin
         The margin around the page in points, used for layout.
         Can be a single value, or a 2, 3 or 4-tuple following the CSS
         shorthand convention. see https://www.w3schools.com/css/css_margin.asp
     columns
@@ -154,77 +116,73 @@
         rotate: Rotation = 0,
         margin: SidesLike = Sides.parse(inch(1)),
         columns: Sequence[Column] = (),
     ) -> None:
         size = XY.parse(size)
         setattr_frozen(self, "content", content)
         setattr_frozen(self, "rotate", rotate)
-        setattr_frozen(
-            self, "columns", columns or [_column_from_margin(size, margin)]
-        )
+        setattr_frozen(self, "columns", columns or [_column(size, margin)])
         setattr_frozen(self, "size", size)
 
     def add(self, d: Drawing, /) -> Page:
         """Create a new page with the given drawing added
 
         Parameters
         ----------
         d
             The drawing to add to the page
         """
         return Page(
-            [*self.content, d],
-            self.size,
-            self.rotate,
-            columns=self.columns,
+            [*self.content, d], self.size, self.rotate, columns=self.columns
         )
 
     def generate(
         self, f: Registry, s: StyleFull, pnum: int, /
-    ) -> Iterator[FilledPage]:
-        yield FilledPage(
+    ) -> Iterator[RenderedPage]:
+        yield RenderedPage(
             self.rotate,
             self.size,
             flatten(map(methodcaller("render", f, s), self.content)),
         )
 
     def fill(
-        self, f: Registry, s: StyleFull, extra: Iterable[ops.Command]
-    ) -> FilledPage:
-        return FilledPage(
+        self, f: Registry, s: StyleFull, extra: Iterable[bytes]
+    ) -> RenderedPage:
+        return RenderedPage(
             self.rotate,
             self.size,
             chain(
                 flatten(map(methodcaller("render", f, s), self.content)),
-                flatten(map(ops.into_stream, extra)),
+                extra,
             ),
         )
 
 
-def _column_from_margin(page: XY, margin: SidesLike) -> Column:
+def _column(page: XY, margin: SidesLike) -> Column:
     top, right, bottom, left = Sides.parse(margin)
     return Column(
         XY(left, bottom), page.x - left - right, page.y - top - bottom
     )
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class AutoPage:
     """Automatically lays out content on multiple pages.
 
     Parameters
     ----------
     content: ~typing.Iterable[~pdfje.Block | str] | ~pdfje.Block | str
         The content to lay out on the pages. Can be parsed from single string
         or block.
     template: ~pdfje.Page | ~typing.Callable[[int], ~pdfje.Page]
         A page to use as a template for the layout. If a callable is given,
         it is called with the page number as the only argument to generate
-        the page.
+        the page. Defaults to the default :class:`Page`.
 
     """
 
     content: Iterable[str | Block]
     template: Callable[[int], Page]
 
     def __init__(
@@ -240,29 +198,29 @@
 
         if isinstance(template, Page):
             template = always(template)
         setattr_frozen(self, "template", template)
 
     def generate(
         self, fr: Registry, style: StyleFull, pnum: int, /
-    ) -> Iterator[FilledPage]:
+    ) -> Iterator[RenderedPage]:
         gen = self._chained_blocks_layout(fr, style)
         for page in map(self.template, count(pnum)):  # pragma: no branch
             filled_columns = []
             for col in page.columns:
                 try:
                     filled_columns.append(gen.send(col))
                 except StopIteration:
                     break
             else:
-                yield page.fill(fr, style, filled_columns)
+                yield page.fill(fr, style, flatten(filled_columns))
                 continue  # there's still content, so keep on paging
 
             if filled_columns:
-                yield page.fill(fr, style, filled_columns)
+                yield page.fill(fr, style, flatten(filled_columns))
             return
 
     @skips_to_first_yield
     def _chained_blocks_layout(
         self, r: Registry, s: StyleFull, /
     ) -> Generator[ColumnFill, Column, None]:
         fill = ColumnFill.new((yield))  # type: ignore[misc]
@@ -273,25 +231,25 @@
 
 def _as_block(b: str | Block) -> Block:
     if isinstance(b, str):
         return Paragraph(b)
     return b
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Document:
     """a PDF Document
 
     Parameters
     ----------
 
-    content: ~typing.Iterable[Page | AutoPage] | str | Paragraph | None
-        The content of the document. Can be a string, a list of pages,
-        or a list of blocks.
+    content
+        The content of the document.
     style
         Change the default style of the document.
 
     Examples
     --------
 
     Below are some examples of creating documents.
@@ -303,15 +261,15 @@
     ...     AutoPage([LOREM_IPSUM, ZEN_OF_PYTHON]),
     ...     Page(),
     ... ])
 
 
     note
     ----
-       A document must contain at least one page to be valid
+    A document must contain at least one page to be valid
     """
 
     pages: Iterable[Page | AutoPage]
     style: Style
 
     def __init__(
         self,
@@ -329,19 +287,19 @@
         setattr_frozen(self, "style", Style.parse(style))
 
     @overload
     def write(self) -> Iterator[bytes]:
         ...
 
     @overload
-    def write(self, target: os.PathLike | str | IO[bytes]) -> None:
+    def write(self, target: os.PathLike[str] | str | IO[bytes]) -> None:
         ...
 
     def write(  # type: ignore[return]
-        self, target: os.PathLike | str | IO[bytes] | None = None
+        self, target: os.PathLike[str] | str | IO[bytes] | None = None
     ) -> Iterator[bytes] | None:
         """Write the document to a given target. If no target is given,
         outputs the binary PDF content iteratively. See examples below.
 
         Parameters
         ----------
         target: ~os.PathLike | str | ~typing.IO[bytes] | None
```

### Comparing `pdfje-0.4.0/src/pdfje/draw.py` & `pdfje-0.5.0/src/pdfje/draw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,58 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass
-from typing import Iterable
+from operator import attrgetter
+from typing import Callable, Iterable, Iterator, Literal, final
 
-from .common import RGB, XY, HexColor, Pt, add_slots, pipe, setattr_frozen
+from .common import (
+    RGB,
+    XY,
+    Align,
+    HexColor,
+    Pt,
+    Streamable,
+    add_slots,
+    pipe,
+    setattr_frozen,
+)
 from .fonts.registry import Registry
-from .style import StyleFull
+from .style import Span, Style, StyledMixin, StyleFull, StyleLike
+from .typeset.common import Command, State, Stretch, splitlines
+from .typeset.lines import Line as TextLine
+from .typeset.words import parse as parse_words
+
+__all__ = [
+    "Circle",
+    "Ellipse",
+    "Line",
+    "Polyline",
+    "Rect",
+    "Text",
+    "Drawing",
+]
 
 
 class Drawing(abc.ABC):
     """Base class for all drawing operations wich can be put on
     a :class:`~pdfje.Page`."""
 
     __slots__ = ()
 
     @abc.abstractmethod
-    def render(self, f: Registry, s: StyleFull, /) -> Iterable[bytes]:
+    def render(self, f: Registry, s: StyleFull, /) -> Streamable:
         ...
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Line(Drawing):
-    """A :class:`~pdfje.Drawing` of a straight line segment.
+    """A :class:`Drawing` of a straight line segment.
 
     Parameters
     ----------
     start
         The start point of the line. Can be parsed from a 2-tuple.
     end
         The end point of the line. Can be parsed from a 2-tuple.
@@ -46,23 +71,24 @@
         end: XY | tuple[float, float],
         stroke: RGB | HexColor | None = RGB(0, 0, 0),
     ) -> None:
         setattr_frozen(self, "start", XY.parse(start))
         setattr_frozen(self, "end", XY.parse(end))
         setattr_frozen(self, "stroke", stroke and RGB.parse(stroke))
 
-    def render(self, _: Registry, __: StyleFull, /) -> Iterable[bytes]:
+    def render(self, _: Registry, __: StyleFull, /) -> Streamable:
         yield b"%g %g m %g %g l " % (*self.start, *self.end)
         yield from _finish(None, self.stroke, False)
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Rect(Drawing):
-    """A :class:`~pdfje.Drawing` of a rectangle.
+    """A :class:`Drawing` of a rectangle.
 
     Parameters
     ----------
     origin
         The bottom left corner of the rectangle. Can be parsed from a 2-tuple.
     width
         The width of the rectangle.
@@ -91,23 +117,24 @@
     ) -> None:
         setattr_frozen(self, "origin", XY.parse(origin))
         setattr_frozen(self, "width", width)
         setattr_frozen(self, "height", height)
         setattr_frozen(self, "fill", fill and RGB.parse(fill))
         setattr_frozen(self, "stroke", stroke and RGB.parse(stroke))
 
-    def render(self, _: Registry, __: StyleFull, /) -> Iterable[bytes]:
+    def render(self, _: Registry, __: StyleFull, /) -> Streamable:
         yield b"%g %g %g %g re " % (*self.origin, self.width, self.height)
         yield from _finish(self.fill, self.stroke, False)
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Ellipse(Drawing):
-    """A :class:`~pdfje.Drawing` of an ellipse.
+    """A :class:`Drawing` of an ellipse.
 
     Parameters
     ----------
     center
         The center of the ellipse. Can be parsed from a 2-tuple.
     width
         The width of the ellipse.
@@ -136,24 +163,25 @@
     ) -> None:
         setattr_frozen(self, "center", XY.parse(center))
         setattr_frozen(self, "width", width)
         setattr_frozen(self, "height", height)
         setattr_frozen(self, "fill", fill and RGB.parse(fill))
         setattr_frozen(self, "stroke", stroke and RGB.parse(stroke))
 
-    def render(self, _: Registry, __: StyleFull, /) -> Iterable[bytes]:
+    def render(self, _: Registry, __: StyleFull, /) -> Streamable:
         yield from _ellipse(
             self.center, self.width, self.height, self.fill, self.stroke
         )
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Circle(Drawing):
-    """A :class:`~pdfje.Drawing` of a circle.
+    """A :class:`Drawing` of a circle.
 
     Parameters
     ----------
     center
         The center of the circle. Can be parsed from a 2-tuple.
     radius
         The radius of the circle.
@@ -177,22 +205,20 @@
         stroke: RGB | HexColor | None = RGB(0, 0, 0),
     ) -> None:
         setattr_frozen(self, "center", XY.parse(center))
         setattr_frozen(self, "radius", radius)
         setattr_frozen(self, "fill", fill and RGB.parse(fill))
         setattr_frozen(self, "stroke", stroke and RGB.parse(stroke))
 
-    def render(self, _: Registry, __: StyleFull, /) -> Iterable[bytes]:
+    def render(self, _: Registry, __: StyleFull, /) -> Streamable:
         width = self.radius * 2
         yield from _ellipse(self.center, width, width, self.fill, self.stroke)
 
 
-def _finish(
-    fill: RGB | None, stroke: RGB | None, close: bool
-) -> Iterable[bytes]:
+def _finish(fill: RGB | None, stroke: RGB | None, close: bool) -> Streamable:
     if fill and stroke:
         yield b"%g %g %g rg %g %g %g RG " % (*fill, *stroke)
         yield b"b\n" if close else b"B\n"
     elif fill:
         yield b"%g %g %g rg f\n" % fill.astuple()
     elif stroke:
         yield b"%g %g %g RG " % stroke.astuple()
@@ -200,15 +226,15 @@
     else:
         yield b"n\n"
 
 
 # based on https://stackoverflow.com/questions/2172798
 def _ellipse(
     center: XY, w: Pt, h: Pt, fill: RGB | None, stroke: RGB | None
-) -> Iterable[bytes]:
+) -> Streamable:
     x, y = center - (w / 2, h / 2)
     kappa = 0.5522848
     ox = (w / 2) * kappa
     oy = (h / 2) * kappa
     xe = x + w
     ye = y + h
     xm = x + w / 2
@@ -245,18 +271,19 @@
         ym + oy,
         x,
         ym,
     )
     yield from _finish(fill, stroke, False)
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class Polyline(Drawing):
-    """A :class:`~pdfje.Drawing` of a polyline.
+    """A :class:`Drawing` of a polyline.
 
     Parameters
     ----------
     points
         The points of the polyline. Can be parsed from a 2-tuple.
     close
         Whether to close the polyline.
@@ -280,15 +307,132 @@
         stroke: RGB | HexColor | None = RGB(0, 0, 0),
     ) -> None:
         setattr_frozen(self, "points", points)
         setattr_frozen(self, "close", close)
         setattr_frozen(self, "fill", fill and RGB.parse(fill))
         setattr_frozen(self, "stroke", stroke and RGB.parse(stroke))
 
-    def render(self, _: Registry, __: StyleFull, /) -> Iterable[bytes]:
+    def render(self, _: Registry, __: StyleFull, /) -> Streamable:
         it = iter(self.points)
         try:
             yield b"%g %g m " % next(it)
         except StopIteration:
             return
         yield from map(pipe(tuple, b"%g %g l ".__mod__), it)
         yield from _finish(self.fill, self.stroke, self.close)
+
+
+@final
+@add_slots
+@dataclass(frozen=True, init=False)
+class Text(Drawing, StyledMixin):
+    """A :class:`Drawing` of text at the given location (not wrapped)
+
+    Parameters
+    ----------
+    loc
+        The location of the text. Can be parsed from a 2-tuple.
+    content: str | Span | ~typing.Iterable[str | Span]
+        The text to render. Can be a string, or a nested :class:`~pdfje.Span`.
+    style
+        The style to apply to the text.
+    align
+        The horizontal alignment of the text.
+    """
+
+    loc: XY
+    content: Iterable[str | Span]
+    style: Style
+    align: Align
+
+    def __init__(
+        self,
+        loc: XY | tuple[float, float],
+        content: str | Span | Iterable[str | Span],
+        style: StyleLike = Style.EMPTY,
+        align: Align | Literal["left", "center", "right"] = Align.LEFT,
+    ) -> None:
+        if isinstance(content, (str, Span)):
+            content = [content]
+        setattr_frozen(self, "loc", XY.parse(loc))
+        setattr_frozen(self, "content", content)
+        setattr_frozen(self, "style", Style.parse(style))
+        setattr_frozen(self, "align", Align.parse(align))
+        if self.align is Align.JUSTIFY:
+            raise NotImplementedError(
+                "Justified alignment not implemented for explicitly "
+                "positioned text."
+            )
+
+    def render(self, r: Registry, s: StyleFull, /) -> Streamable:
+        state = s.as_state(r)
+        yield b"BT\n%g %g Td\n" % self.loc.astuple()
+        yield from state
+        yield from _pick_renderer(self.align)(
+            into_words(splitlines(self.flatten(r, s)), state), state.lead, 0
+        )
+        yield b"ET\n"
+
+
+def into_words(
+    split: Iterable[Iterable[Stretch]], state: State
+) -> Iterator[tuple[Command, TextLine]]:
+    for s in split:
+        cmd, [*words] = parse_words(s, state)
+        yield (
+            cmd,
+            TextLine(
+                tuple(words),
+                max(w.lead() for w in words),
+                sum(w.width() for w in words),
+                0,
+            ),
+        )
+        state = words[-1].state
+
+
+def _render_left(
+    lines: Iterable[tuple[Command, TextLine]], lead: Pt, _: Pt
+) -> Iterator[bytes]:
+    yield b"%g TL\n" % lead
+    for cmd, ln in lines:
+        yield from cmd
+        if ln.lead == lead:
+            yield b"T*\n"
+        else:
+            yield b"0 %g TD\n" % -ln.lead
+            lead = ln.lead
+        yield from ln
+
+
+def _render_centered(
+    lines: Iterable[tuple[Command, TextLine]], _: Pt, width: Pt
+) -> Iterator[bytes]:
+    for cmd, ln in lines:
+        yield from cmd
+        yield b"%g %g TD\n" % ((width - ln.width) / 2, -ln.lead)
+        yield from ln
+        width = ln.width
+
+
+def _render_right(
+    lines: Iterable[tuple[Command, TextLine]], _: Pt, width: Pt
+) -> Iterator[bytes]:
+    for cmd, ln in lines:
+        yield from cmd
+        yield b"%g %g TD\n" % ((width - ln.width), -ln.lead)
+        yield from ln
+        width = ln.width
+
+
+_pick_renderer: Callable[
+    [Align],
+    Callable[[Iterable[tuple[Command, TextLine]], Pt, Pt], Iterable[bytes]],
+] = pipe(
+    attrgetter("value"),
+    [
+        _render_left,
+        _render_centered,
+        _render_right,
+        _render_left,
+    ].__getitem__,
+)
```

### Comparing `pdfje-0.4.0/src/pdfje/fonts/builtins.py` & `pdfje-0.5.0/src/pdfje/fonts/builtins.py`

 * *Files identical despite different names*

### Comparing `pdfje-0.4.0/src/pdfje/fonts/common.py` & `pdfje-0.5.0/src/pdfje/fonts/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import abc
 from dataclasses import dataclass, field
 from itertools import chain, count, pairwise
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable
+from typing import TYPE_CHECKING, Iterable, final
 
 from .. import atoms
 from ..atoms import ASCII
 from ..common import Char, Func, Pos, Pt, add_slots, setattr_frozen
 
 FontID = bytes  # unique, internal identifier assigned to a font within a PDF
 GlyphPt = float  # length unit in glyph space
@@ -46,34 +46,37 @@
 
     @staticmethod
     @abc.abstractmethod
     def charwidth(c: Char, /) -> GlyphPt:
         ...
 
     @abc.abstractmethod
-    def kern(
-        self, s: str, /, prev: Char | None, offset: int
-    ) -> Iterable[tuple[int, GlyphPt]]:
+    def kern(self, s: str, /, prev: Char | None) -> Iterable[Kern]:
+        ...
+
+    @abc.abstractmethod
+    def charkern(self, a: Char, b: Char, /) -> GlyphPt:
         ...
 
 
 # The abstract properties don't mix well with dataclass inheritance.
 # Deleting properties at runtime fixes the issue. It has no runtime impact.
 # We rely on the type checker to ensure subclasses define the needed methods.
 if not TYPE_CHECKING:  # pragma: no cover
     del Font.id
     del Font.encoding_width
     del Font.charwidth
     del Font.spacewidth
 
 
+@final
 @add_slots
 @dataclass(frozen=True, init=False)
 class TrueType:
-    """A TrueType font which will be embedded in the PDF
+    """A TrueType font to be embedded in a PDF
 
     Parameters
     ----------
     regular
         The regular (i.e. non-bold, non-italic) .ttf file
     bold
         The bold .ttf file
@@ -101,51 +104,47 @@
         setattr_frozen(self, "italic", Path(italic))
         setattr_frozen(self, "bold_italic", Path(bold_italic))
 
     # This method cannot be defined in the class body, as it would cause a
     # circular import. The implementation is patched into the class
     # in the `style` module.
     if TYPE_CHECKING:  # pragma: no cover
-        from ..style import HexColor, Style, StyleLike
+        from ..common import HexColor
+        from ..style import Style, StyleLike
 
         def __or__(self, _: StyleLike, /) -> Style:
             ...
 
         def __ror__(self, _: HexColor, /) -> Style:
             ...
 
     def font(self, bold: bool, italic: bool) -> Path:
         if bold:
             return self.bold_italic if italic else self.bold
         else:
             return self.italic if italic else self.regular
 
 
+@final
 @add_slots
 @dataclass(frozen=True, repr=False)
 class BuiltinTypeface:
-    """A typeface that is built into the PDF renderer.
-    Do not instantiate this class, but import its instances:
-
-    .. code-block:: python
-
-       from pdfje import times_roman, helvetica, courier, symbol, zapf_dingbats
-       isinstance(helvetica, BuiltinTypeface)  # True
-    """
+    """A typeface that is built into the PDF renderer."""
 
     regular: BuiltinFont
     bold: BuiltinFont
     italic: BuiltinFont
     bold_italic: BuiltinFont
 
     # This method cannot be defined in the class body, as it would cause a
     # circular import. The implementation is patched into the class
     # in the `style` module.
     if TYPE_CHECKING:  # pragma: no cover
-        from ..style import HexColor, Style, StyleLike
+        from ..common import HexColor
+        from ..style import Style, StyleLike
 
         def __or__(self, _: StyleLike, /) -> Style:
             ...
 
         def __ror__(self, _: HexColor, /) -> Style:
             ...
 
@@ -158,14 +157,15 @@
         else:
             return self.italic if italic else self.regular
 
 
 Typeface = BuiltinTypeface | TrueType
 
 
+@final
 @add_slots
 @dataclass(frozen=True, eq=False)
 class BuiltinFont(Font):
     name: ASCII
     id: FontID
     charwidth: Func[Char, GlyphPt] = field(repr=False)
     kerning: KerningTable | None = field(repr=False)
@@ -180,18 +180,19 @@
         return sum(map(self.charwidth, s)) / TEXTSPACE_TO_GLYPHSPACE
 
     @staticmethod
     def encode(s: str) -> bytes:
         # FUTURE: normalize unicode to allow better unicode representation
         return s.encode("cp1252", errors="replace")
 
-    def kern(
-        self, s: str, /, prev: Char | None, offset: int
-    ) -> Iterable[tuple[int, GlyphPt]]:
-        return kern(self.kerning, s, 1, prev, offset) if self.kerning else ()
+    def kern(self, s: str, /, prev: Char | None) -> Iterable[Kern]:
+        return kern(self.kerning, s, prev) if self.kerning else ()
+
+    def charkern(self, a: Char, b: Char) -> GlyphPt:
+        return self.kerning((a, b)) if self.kerning else 0
 
     def to_resource(self) -> atoms.Dictionary:
         return atoms.Dictionary(
             (b"Type", atoms.Name(b"Font")),
             (b"Subtype", atoms.Name(b"Type1")),
             (b"BaseFont", atoms.Name(self.name)),
             (b"Encoding", atoms.Name(b"WinAnsiEncoding")),
@@ -201,17 +202,15 @@
 KerningTable = Func[tuple[Char, Char], GlyphPt]
 Kern = tuple[Pos, GlyphPt]
 
 
 def kern(
     table: KerningTable,
     s: str,
-    charsize: int,
     prev: Char | None,
-    offset: int,
 ) -> Iterable[Kern]:
     for i, pair in zip(
-        count(offset + (not prev) * charsize, charsize),
+        count(not prev),
         pairwise(chain(prev, s) if prev else s),
     ):
         if space := table(pair):
             yield (i, space)
```

### Comparing `pdfje-0.4.0/src/pdfje/fonts/embed.py` & `pdfje-0.5.0/src/pdfje/fonts/embed.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
 
 OBJS_PER_EMBEDDED_FONT = 7
 _GlyphName = str  # name uniquely identifying a glyph in a TTF font
 _CID = int  # CharacterID. 16-bit ID uniquely identifying a character in a PDF
 _CID_MAX = 0xFFFF  # character IDs are stored as 16-bit values
 _REPLACEMENT_GLYPH: _GlyphName = ".notdef"
 _CIDSYS_INFO = atoms.Dictionary(
-    (b"Registry", atoms.LiteralString(b"Adobe")),
-    (b"Ordering", atoms.LiteralString(b"UCS")),
+    (b"Registry", atoms.LiteralStr(b"Adobe")),
+    (b"Ordering", atoms.LiteralStr(b"UCS")),
     (b"Supplement", atoms.Int(0)),
 )
 
 
 def _utf16be_hex(c: Ordinal) -> bytes:
     if c <= 0xFFFF:
         return b"%04X" % c
@@ -143,19 +143,20 @@
                 # Encoding by UTF-16BE is a fast way to convert from CIDs
                 # to bytes. Because not all CIDs are valid codepoints,
                 # we use surrogatepass.
                 .encode("utf-16be", errors="surrogatepass")
             )
 
         def kern(
-            self, s: str, /, prev: Char | None, offset: int
+            self, s: str, /, prev: Char | None
         ) -> Iterable[tuple[int, GlyphPt]]:
-            return (
-                kern(self.kerning, s, 2, prev, offset) if self.kerning else ()
-            )
+            return kern(self.kerning, s, prev) if self.kerning else ()
+
+        def charkern(self, a: Char, b: Char, /) -> GlyphPt:
+            return self.kerning((a, b)) if self.kerning else 0
 
         def to_objects(self, obj_id: atoms.ObjectID) -> Iterable[atoms.Object]:
             # PDF only supports 16-bit character/glyph entries,
             # thus there is a theoretical limit to the number of unique
             # characters in a document per font. There are workarounds,
             # but most fonts don't even have this many glyphs and this many
             # different characters seem unlikely to occur in common text.
```

### Comparing `pdfje-0.4.0/src/pdfje/fonts/registry.py` & `pdfje-0.5.0/src/pdfje/fonts/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,14 @@
 
 from .. import atoms
 from ..atoms import ASCII
 from ..common import add_slots
 from .common import BuiltinFont, BuiltinTypeface, Font, TrueType, Typeface
 from .embed import OBJS_PER_EMBEDDED_FONT, Subset
 
-__all__ = [
-    "Registry",
-]
-
 
 @add_slots
 @dataclass(frozen=True, eq=False)
 class Registry:
     """Used to keeps track of fonts as they are used within a document"""
 
     _builtins: dict[tuple[ASCII, bool, bool], BuiltinFont] = field(
```

### Comparing `pdfje-0.4.0/src/pdfje/vendor/get_kerning_pairs.py` & `pdfje-0.5.0/src/pdfje/vendor/get_kerning_pairs.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self.glyphs = []
         self.class2Record = 0
 
 
 def collect_unique_kern_lookup_indexes(featureRecord):
     unique_kern_lookups = []
     for featRecItem in featureRecord:
-        # print(featRecItem.FeatureTag)
         # GPOS feature tags (e.g. kern, mark, mkmk, size) of each ScriptRecord
         if featRecItem.FeatureTag == kKernFeatureTag:
             feature = featRecItem.Feature
 
             for featLookupItem in feature.LookupListIndex:
                 if featLookupItem not in unique_kern_lookups:
                     unique_kern_lookups.append(featLookupItem)
```

### Comparing `pdfje-0.4.0/PKG-INFO` & `pdfje-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfje
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tiny PDF writer
 Home-page: https://github.com/ariebovenberg/pdfje
 License: MIT
 Keywords: pdf
 Author: Arie Bovenberg
 Author-email: a.c.bovenberg@gmail.com
 Requires-Python: >=3.8.1,<4.0
@@ -14,99 +14,109 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: fonts
+Provides-Extra: hyphens
 Requires-Dist: fonttools (>=4.38.0,<5.0.0) ; extra == "fonts"
+Requires-Dist: pyphen (>=0.13.0) ; extra == "hyphens"
 Project-URL: Documentation, https://pdfje.readthedocs.io
 Project-URL: Repository, https://github.com/ariebovenberg/pdfje
 Description-Content-Type: text/x-rst
 
 🌷 pdf'je
 =========
 
-.. image:: https://img.shields.io/pypi/v/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/v/pdfje.svg?style=flat-square&color=blue
    :target: https://pypi.python.org/pypi/pdfje
 
-.. image:: https://img.shields.io/pypi/l/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/pyversions/pdfje.svg?style=flat-square
    :target: https://pypi.python.org/pypi/pdfje
 
-.. image:: https://img.shields.io/pypi/pyversions/pdfje.svg?style=flat-square
+.. image:: https://img.shields.io/pypi/l/pdfje.svg?style=flat-square&color=blue
    :target: https://pypi.python.org/pypi/pdfje
 
+.. image:: https://img.shields.io/badge/mypy-strict-forestgreen?style=flat-square
+   :target: https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-strict
+
+.. image:: https://img.shields.io/badge/coverage-99%25-forestgreen?style=flat-square
+   :target: https://github.com/ariebovenberg/pdfje
+
+.. image::  https://img.shields.io/github/actions/workflow/status/ariebovenberg/pdfje/tests.yml?branch=main&style=flat-square
+   :target: https://github.com/ariebovenberg/pdfje
+
 .. image:: https://img.shields.io/readthedocs/pdfje.svg?style=flat-square
    :target: http://pdfje.readthedocs.io/
 
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square
-   :target: https://github.com/psf/black
-
------
+..
 
   **pdf·je** [`🔉 <https://upload.wikimedia.org/wikipedia/commons/a/ac/Nl-pdf%27je.ogg>`_ PDF·yuh] (noun) Dutch for 'small PDF'
 
-Write beautiful PDFs in declarative Python.
+**Write beautiful PDFs in declarative Python.**
 
-Currently in active development. See the roadmap_ for supported features.
-Leave a ⭐️ on GitHub if you're interested how this develops!
+*(Currently in active development. Leave a* ⭐️ *on GitHub if you're interested how this develops!)*
 
-Why?
-----
+Features
+--------
 
-There are many PDF libraries for Python, but none of them
-have these features:
+Pdf'je distinguishes itself with the following combination of features:
 
 🧩 Declarative API
 ~~~~~~~~~~~~~~~~~~
 
-In most PDF writers, you first create various empty objects and
+In most PDF writers, you first create empty objects and
 then mutate them with methods like ``addText()``,
-all while changing the state of the writer with methods like ``setFont()``.
+all while changing the state with methods like ``setFont()``.
 **Pdf'je** is different. You describe the document you want to write,
-and the library takes care of the details. No state to manage, no mutations.
+and it takes care of the details. No state to manage, no mutations.
 This makes your code easier to reuse and reason about.
 
-📐 Polished typography
-~~~~~~~~~~~~~~~~~~~~~~
-
-Legibility counts. And `kerning <https://en.wikipedia.org/wiki/Kerning>`_
-— i.e. adjusting the spacing between letters — is a key part of this.
-Automatic kerning is supported everywhere, from web browsers to word processors.
-However, most PDF writers don't support it.
-By using font metrics to calculate the correct kerning,
-**pdf'je** helps you write documents that look great.
-
-🎈 Small footprint
-~~~~~~~~~~~~~~~~~~
-
-PDF supports many features, but most of the time you only need a few.
-Why install many dependencies — just to write a simple document?
-Not only is **pdf'je** pure-Python, it allows you to
-install only the dependencies you need.
-
-
-Quickstart
-----------
-
-Getting text onto paper is super easy:
-
 .. code-block:: python
 
   from pdfje import Document
   Document("Olá Mundo!").write("hello.pdf")
 
 See `the tutorial <https://pdfje.rtfd.io/en/latest/tutorial.html>`_
 for a complete overview of features, including:
 
 - Styling text including font, size, and color
 - Automatic layout of text into one or more columns
 - Builtin and embedded fonts
 - Drawing basic shapes
 
+See the roadmap_ for supported features.
+
+📖 Decent typography
+~~~~~~~~~~~~~~~~~~~~
+
+Legibility counts — and `kerning <https://en.wikipedia.org/wiki/Kerning>`_
+is a key part of this.
+We've come to expect it everywhere, from web browsers to word processors.
+However, most PDF writers don't support it.
+By using the proper metadata,
+**pdf'je** helps you write documents that look great.
+
+.. image:: https://github.com/ariebovenberg/pdfje/raw/main/sample.png
+   :alt: Sample document with two columns of text
+
+🎈 Small footprint
+~~~~~~~~~~~~~~~~~~
+
+The PDF format supports many features, but most of the time you only need a few.
+Why install many dependencies — just to write a simple document?
+Not only is **pdf'je** pure-Python, it allows you to
+install only the dependencies you need.
+
+.. code-block:: bash
+
+  pip install pdfje                 # no dependencies
+  pip install pdfje[fonts, hyphens] # embedded fonts and improved hyphenation
+
 .. _roadmap:
 
 Roadmap
 -------
 
 **Pdf'je** is still in active development,
 so it is not yet feature-complete.
@@ -116,18 +126,20 @@
 
 ✅ = implemented, 🚧 = planned, ❌ = not planned
 
 - Typesetting
     - ✅ Automatic kerning
     - ✅ Wrapping text into lines, columns, and pages
     - ✅ Page sizes
-    - 🚧 Centering text
-    - 🚧 Justification
-    - 🚧 Hyphenation
-    - 🚧 Avoiding orphaned lines
+    - ✅ Centering text
+    - ✅ Justification
+    - ✅ Hyphenation
+    - 🚧 Avoiding orphaned/widowed lines
+    - 🚧 Tex-style line breaking
+    - 🚧 Broader unicode support in text wrapping
 - Drawing operations
     - ✅ Lines
     - ✅ Rectangles
     - ✅ Circles, ellipses
     - 🚧 Arbitrary paths, fills, and strokes
 - Text styling
     - ✅ Font and size
@@ -136,58 +148,44 @@
     - ✅ Bold, italic
     - 🚧 Underline and strikethrough
     - 🚧 Superscript and subscript
     - ❌ Complex fill patterns
 - 🚧 Images
 - 🚧 Bookmarks and links
 - 🚧 Tables
+- 🚧 Bullet/numbered lists
 - 🚧 Inline markup with Markdown (Commonmark/MyST)
 - ❌ Emoji
 - ❌ Tables of contents
 - ❌ Forms
 - ❌ Annotations
 
-Installation
-------------
-
-It's available on PyPI.
-
-.. code-block:: bash
-
-  pip install pdfje
-
-By default, no additional dependencies are installed.
-If you'd like to use custom fonts, you'll need ``fontTools``,
-which is included in the ``[fonts]`` extras:
-
-.. code-block:: bash
-
-   pip install pdfje[fonts]
-
 License
 -------
 
 This library is licensed under the terms of the MIT license.
 It also includes short scripts from other projects (see ``pdfje/vendor``),
-which are also MIT licensed.
+which are either also MIT licensed, or in the public domain.
 
 Contributing
 ------------
 
 Here are some useful tips for developing in the ``pdfje`` codebase itself:
 
 - Install dependencies with ``poetry install``.
 - To write output files during tests, use ``pytest --output-path=<outpur-dir>``
 - To also run more comprehensive but 'slow' tests, use ``pytest --runslow``
 
-Alternatives
-------------
+Acknowledgements
+----------------
 
-If pdf'je doesn't suit your needs, here are some other options:
+**pdf'je** is inspired by the following projects.
+If you're looking for a PDF writer, you may want to check them out as well:
 
-- PyFPDF
-- ReportLab
-- WeasyPrint
-- borb
-- wkhtmltopdf
-- pydyf
+- `python-typesetting <https://github.com/brandon-rhodes/python-typesetting>`_
+- `fpdf2 <https://pyfpdf.github.io/fpdf2/index.html>`_
+- `ReportLab <https://www.reportlab.com/>`_
+- `WeasyPrint <https://weasyprint.org/>`_
+- `borb <httpsL//github.com/jorisschellekens/borb/>`_
+- `wkhtmltopdf <https://wkhtmltopdf.org/>`_
+- `pydyf <https://github.com/CourtBouillon/pydyf>`_
```

