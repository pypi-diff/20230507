# Comparing `tmp/sicli-cli-0.1.0.tar.gz` & `tmp/sicli-cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sicli-cli-0.1.0.tar", last modified: Fri May  5 09:52:35 2023, max compression
+gzip compressed data, was "sicli-cli-0.2.0.tar", last modified: Sun May  7 08:47:34 2023, max compression
```

## Comparing `sicli-cli-0.1.0.tar` & `sicli-cli-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     3752 2023-04-29 09:39:41.052119 sicli-cli-0.1.0/.gitignore
--rw-r--r--   0        0        0     1075 2023-04-29 09:21:14.580297 sicli-cli-0.1.0/LICENSE
--rw-r--r--   0        0        0     5935 2023-05-05 09:30:04.123618 sicli-cli-0.1.0/README.md
--rw-r--r--   0        0        0      995 2023-05-01 17:28:24.676397 sicli-cli-0.1.0/examples/congrat.py
--rw-r--r--   0        0        0      578 2023-05-05 09:52:19.587208 sicli-cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      128 2023-05-03 17:38:43.511647 sicli-cli-0.1.0/sicli/__init__.py
--rw-r--r--   0        0        0     6119 2023-05-03 19:24:16.633400 sicli-cli-0.1.0/sicli/main.py
--rw-r--r--   0        0        0       67 2023-04-30 08:14:17.530529 sicli-cli-0.1.0/sicli/types.py
--rw-r--r--   0        0        0      639 2023-04-29 18:07:03.719125 sicli-cli-0.1.0/sicli/utils.py
--rw-r--r--   0        0        0     2607 2023-05-03 19:15:51.135860 sicli-cli-0.1.0/tests/test_main.py
--rw-r--r--   0        0        0     6427 1970-01-01 00:00:00.000000 sicli-cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3752 2023-04-29 09:39:41.052119 sicli-cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1075 2023-04-29 09:21:14.580297 sicli-cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5867 2023-05-05 11:19:22.999752 sicli-cli-0.2.0/README.md
+-rw-r--r--   0        0        0      996 2023-05-05 12:19:05.491697 sicli-cli-0.2.0/examples/congrat.py
+-rw-r--r--   0        0        0      578 2023-05-05 09:52:19.587208 sicli-cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      161 2023-05-05 13:54:14.743462 sicli-cli-0.2.0/sicli/__init__.py
+-rw-r--r--   0        0        0     6215 2023-05-05 12:19:05.839704 sicli-cli-0.2.0/sicli/main.py
+-rw-r--r--   0        0        0       67 2023-04-30 08:14:17.530529 sicli-cli-0.2.0/sicli/types.py
+-rw-r--r--   0        0        0      639 2023-05-05 11:00:21.995211 sicli-cli-0.2.0/sicli/utils.py
+-rw-r--r--   0        0        0     2769 2023-05-05 13:49:02.369217 sicli-cli-0.2.0/tests/test_main.py
+-rw-r--r--   0        0        0     6359 1970-01-01 00:00:00.000000 sicli-cli-0.2.0/PKG-INFO
```

### Comparing `sicli-cli-0.1.0/.gitignore` & `sicli-cli-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sicli-cli-0.1.0/LICENSE` & `sicli-cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sicli-cli-0.1.0/README.md` & `sicli-cli-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: sicli-cli
+Version: 0.2.0
+Summary: A package to build simple command line tools in the declarative way.
+Author: immanelg
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Developers
+Requires-Dist: pytest ; extra == "test"
+Project-URL: Documentation, https://github.com/immanelg/sicli
+Project-URL: Source Code, https://github.com/immanelg/sicli
+Provides-Extra: test
+
 # Sicli
 ## Introduction
 `sicli` is a wrapper around standard library module `argparse` that lets you create CLIs in a simple, declarative way.
 It parses the signature of your *type-hinted* function and generates CLI from that.
 
 `sicli` is not intended for big and complex applications, so if you need that, you rather need to use a framework like [Click](https://click.palletsprojects.com/en) or [Typer](https://typer.tiangolo.com/).
 
@@ -135,18 +149,18 @@
 ...     print(numbers[0] / numbers[1])
 ... 
 >>> sicli.run(divide, ["+numbers", "1", "2"], prefix_chars="-+")
 0.5
 
 ```
 
-#### `list[T]`
+#### `list[T], typing.List[T], typing.Sequence[T], typing.Iterable[T]`
 As you saw, `list[T]` lets you pass multiple arguments. `tuple[...]` (for heterogeneous types) is not currently not supported.
 
-#### `typing.Literal[A, B, ...]`
+#### `typing.Literal`
 `Literal[A, B, ...]` (of the same type) lets you restrict values.
 
 #### `enum.Enum`
 It is recommended to use `Literal` instead, but `enum.Enum` can work similarly. To use it, you need to create `__str__` method like that:
 ```python
 class Color(Enum):
     red = "r"
@@ -174,26 +188,22 @@
 #### Limitations
 Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3], {}]]`). Only `Annotated` can wrap other generic types.
 
 ## Requirements
 No dependencies are needed, only pure Python ≥ `3.10`.
 
 ## Installation
-Not available in PyPi for now. Clone the repo and build it yourself.
-```
-git clone git@github.com:immanelg/sicli.git
+Install from PyPI:
 ```
-And then
-```
-flit build
-flit install
+pip install sicli-cli
 ```
 
 ## Motivation
 For fun.
 
 ## Alternatives
 [Click](https://click.palletsprojects.com/en): The greatest CLI toolkit. Use it if you want to have a complex CLI.
 
 [Typer](https://typer.tiangolo.com/): Cool Click wrapper, similar to `sicli`.
 
 [Plac](https://plac.readthedocs.io/en/latest/): Simple wrapper for `argparse`.
+
```

### Comparing `sicli-cli-0.1.0/examples/congrat.py` & `sicli-cli-0.2.0/examples/congrat.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,20 @@
 from typing import Annotated as Ann
 from pathlib import Path
 
 
 def congratulate(
     # positional arguments go here
     reason: str,
-    gift: Ann[str, "What to give them"], # help message
-    language: Literal["en", "fr"] = "en", # choice of values 
-
+    gift: Ann[str, "What to give them"],  # help message
+    language: Literal["en", "fr"] = "en",  # choice of values
     # options go here
     *,
     output: Path = Path("./out.txt"),
-    loud: Ann[bool, "IF ENABLED THEN SCREAM"], # this is a flag
+    loud: Ann[bool, "IF ENABLED THEN SCREAM"],  # this is a flag
     names: list[str] = ["Maria"],
 ) -> None:
     """
     This program congratulates everyone if you haven't guessed.
     By the way, this doctring is the help message for the CLI.
     """
     if language == "fr":
```

### Comparing `sicli-cli-0.1.0/pyproject.toml` & `sicli-cli-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sicli-cli-0.1.0/sicli/main.py` & `sicli-cli-0.2.0/sicli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 from argparse import ArgumentParser
-from collections.abc import Iterable
-from typing import Any, Literal, Annotated, Union
+from collections.abc import Iterable, Sequence
+from typing import Any, Literal, Annotated, Tuple, Union, List
 from enum import Enum
 import inspect
 from .utils import (
     isgeneric,
     unwrap_generic_alias,
     get_signature,
     snake_to_lower_kebab_case,
     lenient_issubclass,
 )
 from sicli.types import AnyCallable
 
 
 class Sicli:
+    """Wrapper for parser that can parse function signatures."""
+
     _parser: ArgumentParser
 
     def __init__(self, **argument_parser_kwargs: Any) -> None:
         self._parser = ArgumentParser(**(argument_parser_kwargs or {}))
 
     def _add_function(self, function: AnyCallable, parser) -> None:
+        """Parses function signature and adding arguments to parser."""
         for param in get_signature(function).parameters.values():
             is_positional = param.kind == param.POSITIONAL_OR_KEYWORD
             is_option = param.kind == param.KEYWORD_ONLY
 
             if not is_option and not is_positional:
                 # just not touch it
                 continue
@@ -31,56 +34,54 @@
             type_annotation = param.annotation
 
             type_annotation, varargs, kwargs = self._unwrap_annotated(type_annotation)
 
             origin, typeargs = unwrap_generic_alias(type_annotation)
 
             if origin is Literal:
-                # case when 'choices'
                 kwargs = {"choices": typeargs, "type": type(typeargs[0])} | kwargs
 
             elif origin is Union:
                 # TODO
                 raise ValueError("Union types are currently not supported")
 
-            # allow only explicit type parameters on generic lists/tuples, so use origin
-            elif lenient_issubclass(origin, list):
-                # TODO handle Sequence, Iterable, ...
+            elif lenient_issubclass(origin, (tuple, Tuple)):
+                # `nargs` do not support heterogeneous types
+                # we can manually implement that but i'm lazy
+                raise ValueError("Tuples are currently unsupported, use `list` instead")
+
+            elif lenient_issubclass(origin, (list, List, Sequence, Iterable)):
                 kwargs = {"nargs": "*", "type": typeargs[0]} | kwargs
                 if isgeneric(typeargs[0]):
-                    raise ValueError("Nested generics for `list` are unsupported")
-
-            elif lenient_issubclass(origin, tuple):
-                # `nargs` do not support heterogeneous types
-                raise ValueError("Tuples are unsupported, use `list` instead")
+                    raise ValueError("Complex generic types are currently unsupported")
 
             elif origin is not None:
-                # Unsupported generic alias
                 raise ValueError(f"Unrecognized generic type {origin}")
 
             elif issubclass(type_annotation, Enum):
                 choices = tuple(c for c in type_annotation)
                 kwargs = {"choices": choices, "type": type_annotation} | kwargs
 
             elif issubclass(type_annotation, bool):
-                # case when boolean flag
                 kwargs = {"action": "store_true"} | kwargs
 
             elif type_annotation is param.empty:
-                # no type is provided
                 pass
 
             else:
                 # case when regular param
                 kwargs = {"type": type_annotation, "action": "store"} | kwargs
 
             if param.default != param.empty:
                 kwargs = {"default": param.default} | kwargs
 
-                if kwargs.get("action") == "store_true" and kwargs.get("default") is True:
+                if (
+                    kwargs.get("action") == "store_true"
+                    and kwargs.get("default") is True
+                ):
                     raise ValueError("Flag default value should be False")
 
             elif is_option and not kwargs.get("action") == "store_true":
                 # if we don't have a default value and it is not a flag, require
                 # the argument instead of passing None
                 # we do it only for options because argparse is raising
                 # `'required' is an invalid argument for positionals`
@@ -88,14 +89,15 @@
 
             if (
                 kwargs.get("default") is not None
                 and kwargs.get("nargs") != "*"
                 and not kwargs.get("action") == "store_true"
             ):
                 # Always respect the existence of default value
+                # (except when flag and when multiple arguments)
                 kwargs = {"nargs": "?"} | kwargs
 
             param_name = param.name
 
             if not varargs:
                 if is_positional:
                     varargs = [snake_to_lower_kebab_case(param_name)]
```

### Comparing `sicli-cli-0.1.0/sicli/utils.py` & `sicli-cli-0.2.0/sicli/utils.py`

 * *Files identical despite different names*

### Comparing `sicli-cli-0.1.0/tests/test_main.py` & `sicli-cli-0.2.0/tests/test_main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Annotated, Literal
+from collections.abc import Iterable, Sequence
+from typing import Annotated, List, Literal
 from sicli import run
 import pytest
 
 
 def test_basic():
     def f(x: str):
         return x
@@ -33,19 +34,21 @@
     def f(x: int, *, y: bool):
         return x, y
 
     assert run(f, ["12", "--y"]) == (12, True)
     assert run(f, ["12"]) == (12, False)
 
 
-def test_list():
-    def f(xs: list[str], *, ys: list[int]):
+@pytest.mark.parametrize("seq", [list, Iterable, List, Sequence])
+def test_list(seq):
+    def f(xs: seq[str], *, ys: seq[int]):
         return xs, ys
 
     assert run(f, ["a", "b", "--ys", "100", "200"]) == (["a", "b"], [100, 200])
+    assert run(f, ["a", "b", "--ys"]) == (["a", "b"], [])
 
 
 def test_list_default_values():
     def f(xs: list[str] = ["a", "b"], *, ys: list[int] = [3, 4]):
         return xs, ys
 
     assert run(f, ["--ys", "100", "200"]) == (["a", "b"], [100, 200])
@@ -90,26 +93,25 @@
         assert run(f, ["--x", "NaN"])
 
 
 def test_annotated_wrapped_type():
     def f(
         x: Annotated[int, "help for x"],
         *,
-        y: Annotated[Literal[3, 4], "help for y", {}] = 3
+        y: Annotated[Literal[3, 4], "help for y", {}] = 3,
     ):
         return x, y
 
     assert run(f, ["1", "--y", "4"]) == (1, 4)
 
+
 def test_annotated_name_override():
-    def f(
-        *, x: Annotated[int, ["-n", "--number"]]
-    ):
+    def f(*, x: Annotated[int, ["-n", "--number"]]):
         return x
-    
+
     assert run(f, ["-n", "34"]) == 34
     assert run(f, ["--number", "34"]) == 34
 
 
 def test_subcommands():
     def sub_1(*, x: int):
         return x
```

### Comparing `sicli-cli-0.1.0/PKG-INFO` & `sicli-cli-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: sicli-cli
-Version: 0.1.0
-Summary: A package to build simple command line tools in the declarative way.
-Author: immanelg
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Developers
-Requires-Dist: pytest ; extra == "test"
-Project-URL: Documentation, https://github.com/immanelg/sicli
-Project-URL: Source Code, https://github.com/immanelg/sicli
-Provides-Extra: test
-
 # Sicli
 ## Introduction
 `sicli` is a wrapper around standard library module `argparse` that lets you create CLIs in a simple, declarative way.
 It parses the signature of your *type-hinted* function and generates CLI from that.
 
 `sicli` is not intended for big and complex applications, so if you need that, you rather need to use a framework like [Click](https://click.palletsprojects.com/en) or [Typer](https://typer.tiangolo.com/).
 
@@ -149,18 +135,18 @@
 ...     print(numbers[0] / numbers[1])
 ... 
 >>> sicli.run(divide, ["+numbers", "1", "2"], prefix_chars="-+")
 0.5
 
 ```
 
-#### `list[T]`
+#### `list[T], typing.List[T], typing.Sequence[T], typing.Iterable[T]`
 As you saw, `list[T]` lets you pass multiple arguments. `tuple[...]` (for heterogeneous types) is not currently not supported.
 
-#### `typing.Literal[A, B, ...]`
+#### `typing.Literal`
 `Literal[A, B, ...]` (of the same type) lets you restrict values.
 
 #### `enum.Enum`
 It is recommended to use `Literal` instead, but `enum.Enum` can work similarly. To use it, you need to create `__str__` method like that:
 ```python
 class Color(Enum):
     red = "r"
@@ -188,27 +174,21 @@
 #### Limitations
 Note that arbitrary nesting of types is not supported (Like in `list[Annotated[Literal[1, 2, 3], {}]]`). Only `Annotated` can wrap other generic types.
 
 ## Requirements
 No dependencies are needed, only pure Python ≥ `3.10`.
 
 ## Installation
-Not available in PyPi for now. Clone the repo and build it yourself.
-```
-git clone git@github.com:immanelg/sicli.git
+Install from PyPI:
 ```
-And then
-```
-flit build
-flit install
+pip install sicli-cli
 ```
 
 ## Motivation
 For fun.
 
 ## Alternatives
 [Click](https://click.palletsprojects.com/en): The greatest CLI toolkit. Use it if you want to have a complex CLI.
 
 [Typer](https://typer.tiangolo.com/): Cool Click wrapper, similar to `sicli`.
 
 [Plac](https://plac.readthedocs.io/en/latest/): Simple wrapper for `argparse`.
-
```

