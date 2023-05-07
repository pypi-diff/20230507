# Comparing `tmp/linkeddeepdict-1.0.0.tar.gz` & `tmp/linkeddeepdict-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkeddeepdict-1.0.0.tar", last modified: Sun Feb 19 14:12:58 2023, max compression
+gzip compressed data, was "linkeddeepdict-1.1.0.tar", last modified: Sun May  7 16:42:32 2023, max compression
```

## Comparing `linkeddeepdict-1.0.0.tar` & `linkeddeepdict-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-02-19 14:12:58.683784 linkeddeepdict-1.0.0/
--rw-rw-rw-   0        0        0     1087 2023-02-19 14:09:58.000000 linkeddeepdict-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      115 2022-08-06 19:28:44.000000 linkeddeepdict-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6356 2023-02-19 14:12:58.683784 linkeddeepdict-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2022-08-14 20:28:26.000000 linkeddeepdict-1.0.0/README.md
--rw-rw-rw-   0        0        0      110 2021-11-30 20:14:54.000000 linkeddeepdict-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       22 2022-08-14 19:25:07.000000 linkeddeepdict-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-02-19 14:12:58.684787 linkeddeepdict-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2264 2023-02-19 14:11:15.000000 linkeddeepdict-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-19 14:12:58.626613 linkeddeepdict-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-02-19 14:12:58.636612 linkeddeepdict-1.0.0/src/linkeddeepdict/
--rw-rw-rw-   0        0        0      184 2023-02-19 14:10:19.000000 linkeddeepdict-1.0.0/src/linkeddeepdict/__init__.py
--rw-rw-rw-   0        0        0    11313 2023-02-19 14:10:30.000000 linkeddeepdict-1.0.0/src/linkeddeepdict/linkeddeepdict.py
-drwxrwxrwx   0        0        0        0 2023-02-19 14:12:58.682784 linkeddeepdict-1.0.0/src/linkeddeepdict/tools/
--rw-rw-rw-   0        0        0       70 2022-08-06 21:12:31.000000 linkeddeepdict-1.0.0/src/linkeddeepdict/tools/__init__.py
--rw-rw-rw-   0        0        0     2585 2022-08-06 21:12:32.000000 linkeddeepdict-1.0.0/src/linkeddeepdict/tools/dtk.py
--rw-rw-rw-   0        0        0     2256 2022-08-06 21:12:32.000000 linkeddeepdict-1.0.0/src/linkeddeepdict/tools/kwargtools.py
-drwxrwxrwx   0        0        0        0 2023-02-19 14:12:58.678816 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/
--rw-rw-rw-   0        0        0     6356 2023-02-19 14:12:58.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-02-19 14:12:58.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-19 14:12:58.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-11 18:08:26.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2023-02-19 14:12:58.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-02-19 14:12:58.000000 linkeddeepdict-1.0.0/src/linkeddeepdict.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.462168 linkeddeepdict-1.1.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5229 2023-05-07 16:42:32.462168 linkeddeepdict-1.1.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       20 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-07 16:42:32.462168 linkeddeepdict-1.1.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.458168 linkeddeepdict-1.1.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.458168 linkeddeepdict-1.1.0/src/linkeddeepdict/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      178 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/src/linkeddeepdict/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/src/linkeddeepdict/linkeddeepdict.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.462168 linkeddeepdict-1.1.0/src/linkeddeepdict/tools/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       68 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/src/linkeddeepdict/tools/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2503 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/src/linkeddeepdict/tools/dtk.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2180 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/src/linkeddeepdict/tools/kwargtools.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.458168 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5229 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-07 16:42:32.000000 linkeddeepdict-1.1.0/src/linkeddeepdict.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:42:32.462168 linkeddeepdict-1.1.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/tests/test_tools.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2189 2023-05-07 16:42:26.000000 linkeddeepdict-1.1.0/tests/test_types.py
```

### Comparing `linkeddeepdict-1.0.0/LICENSE` & `linkeddeepdict-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Dew Loosh
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
+Copyright (c) 2022 Dew Loosh
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

### Comparing `linkeddeepdict-1.0.0/README.md` & `linkeddeepdict-1.1.0/README.md`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/LinkedDeepDict/main?labpath=examples%2Fbasics.ipynb?urlpath=lab)
-[![CircleCI](https://circleci.com/gh/dewloosh/LinkedDeepDict.svg?style=shield)](https://circleci.com/gh/dewloosh/LinkedDeepDict) 
-[![Documentation Status](https://readthedocs.org/projects/LinkedDeepDict/badge/?version=latest)](https://LinkedDeepDict.readthedocs.io/en/latest/?badge=latest) 
-[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![PyPI](https://badge.fury.io/py/LinkedDeepDict.svg)](https://pypi.org/project/LinkedDeepDict) 
- 
-# **LinkedDeepDict**
-
-A Lightweight Python library to manage nested dictionaries with parent-child relationships.
-On top of being a compatible drop-in replcement of the build in ``dict`` class, the self replicating default factory makes the creation of complex nested layouts effortless.
-
-## **Documentation**
-
-Click [here](https://linkeddeepdict.readthedocs.io/en/latest/) to read the documentation.
-
-## **Installation**
-
-This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
-
-```console
->>> python -m venv venv_name
-```
-
-Once the enviroment is created, activate it via typing
-
-```console
->>> .\venv_name\Scripts\activate
-```
-
-The library can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
-
-```console
->>> pip install linkeddeepdict
-```
-
-## **Usage**
-
-In every case where you'd want to use a `dict`, you can use a `LinkedDeepDict` as a drop-in replacement, but on top of what a simple dictionary provides, a `LinkedDeepDict` is more capable, as it provides a machinery to handle nested layouts. It is basically an ordered `defaultdict` with a self replicating default factory. 
-
-```python
->>> from linkeddeepdict import LinkedDeepDict
->>> data = LinkedDeepDict()
-```
-
-A `LinkedDeepDict` is essentially a nested default dictionary. Being nested refers to the fact that you can do this:
-
-```python
->>> data['a']['b']['c']['e'] = 1
->>> data['a']['b']['d'] = 2
-```
-
-Notice that the object carves a way up until the last key, without needing to create each level explicitly. What happens is that every time a key is missing in a `data`, the object creates a new instance, which then is also ready to handle missing keys or data. Accessing nested subdictionaries works in a similar fashion:
-
-```python
->>> data['a']['b']['c']['e']
-1
-```
-To allow for a more Pythonic feel, it also supports array-like indexing, so that the following operations are valid: 
-
-```python
->>> data['a', 'b', 'c', 'e'] = 3
->>> data['a', 'b', 'c', 'e']
-3
-```
-
-Of course, this is something that we can easily replicate using pure Python in one line, without the need for fancy stuff:
-
-```python
->>> data = {'a' : {'b' : {'c' : {'e' : 3}, 'd' : 2}}}    
-```
-
-The key point is that we loop over a pure `dict` instance, we get
-
-```python
->>> [k for k in data.keys()]
-['a']    
-```
-
-But if we use a `LinkedDeepDict` class and the option `deep=True` when accessing
-keys, values or items of dictionaries, the following happens: 
-
-```python
->>> [k for k in LinkedDeepDict(data).keys(deep=True)]
-['e', 'd']    
-```
-
-We can see, that in this case, iteration goes over keys, that actually hold on to some data, and does not return the containers themselves. If we do the same experiment with the values, it shows that the `LinkedDeepDict` only returns the leafs of the data-tree and the behaviour is fundamentally different:
-
-```python
->>> [k for k in data.values()]
-[{'b': {'c': {'e': 3}, 'd': 2}}]    
-```
-
-```python
->>> [k for k in LinkedDeepDict(data).values(deep=True)]
-[3, 2]    
-```
-
-It is important, that the call `obj.values(deep=True)` still returns a generator object, which makes it memory efficient when looping over large datasets.
-
-```python
->>> LinkedDeepDict(data).values(deep=True)
-<generator object OrderedDefaultDict.values at 0x0000028F209D54A0>    
-```
-
-## **Testing**
-
-To run all tests, open up a console in the root directory of the project and type the following
-
-```console
->>> python -m unittest
-```
-
-## **Dependencies**
-
-The only dependency is `six`, to provide basic continuity between major Python versions 2 and 3.
-
-## **License**
-
-This package is licensed under the MIT license.
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/dewloosh/LinkedDeepDict/main?labpath=examples%2Fbasics.ipynb?urlpath=lab)
+[![CircleCI](https://circleci.com/gh/dewloosh/LinkedDeepDict.svg?style=shield)](https://circleci.com/gh/dewloosh/LinkedDeepDict) 
+[![Documentation Status](https://readthedocs.org/projects/LinkedDeepDict/badge/?version=latest)](https://LinkedDeepDict.readthedocs.io/en/latest/?badge=latest) 
+[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI](https://badge.fury.io/py/LinkedDeepDict.svg)](https://pypi.org/project/LinkedDeepDict) 
+ 
+# **LinkedDeepDict**
+
+A Lightweight Python library to manage nested dictionaries with parent-child relationships.
+On top of being a compatible drop-in replcement of the build in ``dict`` class, the self replicating default factory makes the creation of complex nested layouts effortless.
+
+## **Documentation**
+
+Click [here](https://linkeddeepdict.readthedocs.io/en/latest/) to read the documentation.
+
+## **Installation**
+
+This is optional, but we suggest you to create a dedicated virtual enviroment at all times to avoid conflicts with your other projects. Create a folder, open a command shell in that folder and use the following command
+
+```console
+>>> python -m venv venv_name
+```
+
+Once the enviroment is created, activate it via typing
+
+```console
+>>> .\venv_name\Scripts\activate
+```
+
+The library can be installed (either in a virtual enviroment or globally) from PyPI using `pip` on Python >= 3.7:
+
+```console
+>>> pip install linkeddeepdict
+```
+
+## **Usage**
+
+In every case where you'd want to use a `dict`, you can use a `LinkedDeepDict` as a drop-in replacement, but on top of what a simple dictionary provides, a `LinkedDeepDict` is more capable, as it provides a machinery to handle nested layouts. It is basically an ordered `defaultdict` with a self replicating default factory. 
+
+```python
+>>> from linkeddeepdict import LinkedDeepDict
+>>> data = LinkedDeepDict()
+```
+
+A `LinkedDeepDict` is essentially a nested default dictionary. Being nested refers to the fact that you can do this:
+
+```python
+>>> data['a']['b']['c']['e'] = 1
+>>> data['a']['b']['d'] = 2
+```
+
+Notice that the object carves a way up until the last key, without needing to create each level explicitly. What happens is that every time a key is missing in a `data`, the object creates a new instance, which then is also ready to handle missing keys or data. Accessing nested subdictionaries works in a similar fashion:
+
+```python
+>>> data['a']['b']['c']['e']
+1
+```
+To allow for a more Pythonic feel, it also supports array-like indexing, so that the following operations are valid: 
+
+```python
+>>> data['a', 'b', 'c', 'e'] = 3
+>>> data['a', 'b', 'c', 'e']
+3
+```
+
+Of course, this is something that we can easily replicate using pure Python in one line, without the need for fancy stuff:
+
+```python
+>>> data = {'a' : {'b' : {'c' : {'e' : 3}, 'd' : 2}}}    
+```
+
+The key point is that we loop over a pure `dict` instance, we get
+
+```python
+>>> [k for k in data.keys()]
+['a']    
+```
+
+But if we use a `LinkedDeepDict` class and the option `deep=True` when accessing
+keys, values or items of dictionaries, the following happens: 
+
+```python
+>>> [k for k in LinkedDeepDict(data).keys(deep=True)]
+['e', 'd']    
+```
+
+We can see, that in this case, iteration goes over keys, that actually hold on to some data, and does not return the containers themselves. If we do the same experiment with the values, it shows that the `LinkedDeepDict` only returns the leafs of the data-tree and the behaviour is fundamentally different:
+
+```python
+>>> [k for k in data.values()]
+[{'b': {'c': {'e': 3}, 'd': 2}}]    
+```
+
+```python
+>>> [k for k in LinkedDeepDict(data).values(deep=True)]
+[3, 2]    
+```
+
+It is important, that the call `obj.values(deep=True)` still returns a generator object, which makes it memory efficient when looping over large datasets.
+
+```python
+>>> LinkedDeepDict(data).values(deep=True)
+<generator object OrderedDefaultDict.values at 0x0000028F209D54A0>    
+```
+
+## **Testing**
+
+To run all tests, open up a console in the root directory of the project and type the following
+
+```console
+>>> python -m unittest
+```
+
+## **Dependencies**
+
+The only dependency is `six`, to provide basic continuity between major Python versions 2 and 3.
+
+## **License**
+
+This package is licensed under the MIT license.
```

### Comparing `linkeddeepdict-1.0.0/src/linkeddeepdict/linkeddeepdict.py` & `linkeddeepdict-1.1.0/src/linkeddeepdict/linkeddeepdict.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,348 +1,351 @@
-# http://stackoverflow.com/a/6190500/562769
-from typing import Hashable, Union, Tuple, Any
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-import six
-
-from .tools.dtk import dictparser, parseitems, parseaddress, parsedicts
-
-
-__all__ = ['LinkedDeepDict']
-
-
-NoneType = type(None)
-
-
-def issequence(arg) -> bool:
-    """
-    Returns `True` if `arg` is any kind of iterable, but not a string,
-    returns `False` otherwise.
-    
-    Examples
-    --------
-    The formatter to use to print a floating point number with 4 digits:
-    
-    >>> from dewloosh.core.tools import issequence
-    >>> issequence([1, 2])
-    True
-    
-    To print the actual value as a string:
-    
-    >>> issequence('lorem ipsum')
-    False    
-    """
-    return (
-        isinstance(arg, Iterable)
-        and not isinstance(arg, six.string_types)
-    )  
-
-
-class LinkedDeepDict(dict):
-    """
-    An nested dictionary class with a self-replicating default factory. 
-    It can be a drop-in replacement for the bulit-in dictionary type, 
-    but it's more capable as it handles nested layouts.
-    
-    Examples
-    --------
-    Basic usage:
-    
-    >>> from ldd import LinkedDeepDict
-    >>> d = {'a' : {'aa' : {'aaa' : 0}}, 'b' : 1, 'c' : {'cc' : 2}}
-    >>> dd = LinkedDeepDict(d)
-    >>> list(dd.values(deep=True))
-    [0, 1, 2]
-    
-    See the docs for more use cases!
-        
-    """
-    
-    def __init__(self, *args, parent:'LinkedDeepDict'=None, 
-                 root:'LinkedDeepDict'=None, locked:bool=None, 
-                 **kwargs):
-        """
-        Returns a `LinkedDeepDict` instance.
-
-        Parameters
-        ----------
-        *args : tuple, Optional
-            Extra positional arguments are forwarded to the `dict` class.
-
-        parent : `LinkedDeepDict`, Optional
-            Parent `LinkedDeepDict` instance. Default is `None`.
-
-        root : `LinkedDeepDict`, Optional
-            The top-level object. It is automatically set when creating nested
-            layouts, but may be explicitly provided. Default is `None`. 
-
-        locked : bool or NoneType, Optional
-            If the object is locked, it reacts to missing keys as a regular dictionary would.
-            If it is not, a new level and a new child is created (see the examples in the docs).
-            A `None` value means that in terms of locking, the state of the object 
-            is inherited from its parent. Default is `None`.
-
-        **kwargs : tuple, Optional
-            Extra keyword arguments are forwarded to the `dict` class.
-
-        """
-        for k, v in kwargs.items():
-            if isinstance(v, LinkedDeepDict):
-                v.parent = self
-                v._key = k
-        super().__init__(*args, **kwargs)
-        self.parent = parent
-        self._root = root
-        self._locked = locked
-        self._key = None
-        
-    @property
-    def key(self) -> Union[Hashable, NoneType]:
-        """
-        Returns the key of the dictionary in its parent, or `None` if the 
-        object is the root.
-        """
-        return self._key
-           
-    @property
-    def locked(self) -> bool:
-        """
-        Returns `True` if the object is locked. The property is equpped with a setter.
-        """
-        if self.parent is None:
-            return self._locked if isinstance(self._locked, bool) else False
-        else:
-            return self._locked if isinstance(self._locked, bool) else self.parent.locked
-
-    @property
-    def depth(self) -> int:
-        """
-        Retuns the depth of the actual instance in a layout, starting from 0..
-        """
-        if self.parent is None:
-            return 0
-        else:
-            return self.parent.depth + 1
-        
-    @property
-    def address(self) -> Tuple:
-        """Returns the address of an item."""
-        if self.is_root():
-            return []
-        else:
-            r = self.parent.address
-            r.append(self.key)
-            return r
-
-    def lock(self):
-        """
-        Locks the layout of the dictionary. If a `LinkedDeepDict` is locked,
-        missing keys are handled the same way as they would've been handled
-        if it was a ´dict´. Also, setting or deleting items in a locked
-        dictionary and not possible and you will experience an error upon trying.
-        
-        """
-        self._locked = True
-
-    def unlock(self):
-        """
-        Releases the layout of the dictionary. If a `LinkedDeepDict` is not locked,
-        a missing key creates a new level in the layout, also setting and deleting
-        items becomes an option.
-        
-        """
-        self._locked = False
-        
-    def root(self):
-        """
-        Returns the top-level object in a nested layout.
-        """
-        if self.parent is None:
-            return self
-        else:
-            if self._root is not None:
-                return self._root
-            else:
-                return self.parent.root()
-
-    def is_root(self) -> bool:
-        """
-        Returns `True`, if the object is the root.
-        """
-        return self.parent is None
-
-    def containers(self, *args, inclusive:bool=False, deep:bool=True, 
-                   dtype:Any=None, **kwargs):
-        """
-        Returns all the containers in a nested layout. A dictionary in a nested layout
-        is called a container, only if it contains other containers (it is a parent). 
-
-        Parameters
-        ----------
-        inclusive : bool, Optional
-            If `True`, the object the call is made upon also gets returned.
-            This can be important if you make the call on the root object, which most
-            of the time does not hold onto relevant data directly.
-            Default is `False`.
-
-        deep : bool, Optional
-            If `True` the parser goes into nested dictionaries.
-            Default is `True`
-
-        dtype : Any, Optional
-            Constrains the type of the returned objects.
-            Default is `None`, which means no restriction.
-
-        Returns
-        -------
-        generator
-            Returns a generator object.
-
-        Examples
-        --------
-        A simple example:
-
-        >>> from ldd import LinkedDeepDict
-        >>> data = LinkedDeepDict()
-        >>> data['a', 'b', 'c'] = 1
-        >>> [c.key for c in data.containers()]
-        ['a', 'b']
-
-        We can see, that dictionaries 'a' and 'b' are returned as containers, but 'c' 
-        isn't,  because it is not a parent, there are no deeper levels. 
-
-        >>> [c.key for c in data.containers(inclusive=True, deep=True)]
-        [None, 'a', 'b']
-
-        >>> [c.key for c in data.containers(inclusive=True, deep=False)]     
-        [None, 'a']
-
-        >>> [c.key for c in data.containers(inclusive=False, deep=True)]       
-        ['a', 'b']
-
-        >>> [c.key for c in data.containers(inclusive=False, deep=False)]      
-        ['a']
-
-        """
-        dtype = self.__class__ if dtype is None else dtype
-        return parsedicts(self, inclusive=inclusive, dtype=dtype, deep=deep)
-
-    def __getitem__(self, key):
-        try:
-            if issequence(key):
-                return parseaddress(self, key)
-            else:
-                return super().__getitem__(key)
-        except ValueError:
-            return self.__missing__(key)
-        except KeyError:
-            return self.__missing__(key)
-        
-    def __delitem__(self, key):
-        if self.locked:
-            raise RuntimeError("The object is locked!")
-        super().__delitem__(key)
-
-    def __setitem__(self, key, value):
-        if self.locked:
-            raise RuntimeError("The object is locked!")
-        try:
-            if issequence(key):
-                if not key[0] in self:
-                    d = self.__missing__(key[0])
-                else:
-                    d = self[key[0]]
-                if len(key) > 1:
-                    d.__setitem__(key[1:], value)
-                else:
-                    d = self[key[0]]
-                    if isinstance(d, LinkedDeepDict):
-                        d.__leave_parent__()
-                    if value is None:
-                        del self[key[0]]
-                    else:
-                        self[key[0]] = value
-            else:
-                if key in self:
-                    d = self[key]
-                    if isinstance(d, LinkedDeepDict):
-                        d.__leave_parent__()
-                if value is None:
-                    if key in self:
-                        del self[key]
-                else:
-                    if isinstance(value, LinkedDeepDict):
-                        value.__join_parent__(self, key)
-                    return super().__setitem__(key, value)
-        except KeyError:
-            return self.__missing__(key)
-
-    def __missing__(self, key):
-        if self.locked:
-            raise KeyError("Missing key : {}".format(key))
-        if issequence(key):
-            if key[0] not in self:
-                self[key[0]] = value = self.__class__()
-            else:
-                value = self[key[0]]
-            if len(key) > 1:
-                return value.__missing__(key[1:])
-            else:
-                return value
-        else:
-            self[key] = value = self.__class__()
-            return value
-        
-    def __reduce__(self):
-        return self.__class__, tuple(), None, None, self.items()
-    
-    def __repr__(self):
-        frmtstr = self.__class__.__name__ + '(%s)'
-        return frmtstr % (dict.__repr__(self))
-       
-    def __leave_parent__(self):
-        self.parent = None
-        self._root = None
-        self._key = None
-            
-    def __join_parent__(self, parent, key: Hashable = None):
-        self.parent = parent
-        self._root = parent.root()
-        self._key = key
-
-    def items(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, v in dictparser(self):
-                    yield addr, v
-            else:
-                for k, v in parseitems(self):
-                    yield k, v
-        else:
-            for k, v in super().items():
-                yield k, v
-
-    def values(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, v in dictparser(self):
-                    yield addr, v
-            else:
-                for _, v in parseitems(self):
-                    yield v
-        else:
-            for v in super().values():
-                yield v
-
-    def keys(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
-        if deep:
-            if return_address:
-                for addr, _ in dictparser(self):
-                    yield addr
-            else:
-                for k, _ in parseitems(self):
-                    yield k
-        else:
-            for k in super().keys():
-                yield k
+# http://stackoverflow.com/a/6190500/562769
+from typing import Hashable, Union, Tuple, Any
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+import six
+
+from .tools.dtk import dictparser, parseitems, parseaddress, parsedicts
+
+
+__all__ = ['LinkedDeepDict']
+
+
+NoneType = type(None)
+
+
+def issequence(arg) -> bool:
+    return (
+        isinstance(arg, Iterable)
+        and not isinstance(arg, six.string_types)
+    )  
+
+
+class LinkedDeepDict(dict):
+    """
+    An nested dictionary class with a self-replicating default factory. 
+    It can be a drop-in replacement for the bulit-in dictionary type, 
+    but it's more capable as it handles nested layouts.
+    
+    Examples
+    --------
+    Basic usage:
+    
+    >>> from ldd import LinkedDeepDict
+    >>> d = {'a' : {'aa' : {'aaa' : 0}}, 'b' : 1, 'c' : {'cc' : 2}}
+    >>> dd = LinkedDeepDict(d)
+    >>> list(dd.values(deep=True))
+    [0, 1, 2]
+    
+    See the docs for more use cases!
+        
+    """
+    
+    def __init__(self, *args, parent:'LinkedDeepDict'=None, 
+                 root:'LinkedDeepDict'=None, locked:bool=None, 
+                 **kwargs):
+        """
+        Returns a `LinkedDeepDict` instance.
+
+        Parameters
+        ----------
+        *args : tuple, Optional
+            Extra positional arguments are forwarded to the `dict` class.
+
+        parent : `LinkedDeepDict`, Optional
+            Parent `LinkedDeepDict` instance. Default is `None`.
+
+        root : `LinkedDeepDict`, Optional
+            The top-level object. It is automatically set when creating nested
+            layouts, but may be explicitly provided. Default is `None`. 
+
+        locked : bool or NoneType, Optional
+            If the object is locked, it reacts to missing keys as a regular dictionary would.
+            If it is not, a new level and a new child is created (see the examples in the docs).
+            A `None` value means that in terms of locking, the state of the object 
+            is inherited from its parent. Default is `None`.
+
+        **kwargs : tuple, Optional
+            Extra keyword arguments are forwarded to the `dict` class.
+
+        """
+        for k, v in kwargs.items():
+            if isinstance(v, LinkedDeepDict):
+                v.parent = self
+                v._key = k
+        super().__init__(*args, **kwargs)
+        self.parent = parent
+        self._root = root
+        self._locked = locked
+        self._key = None
+        
+    @property
+    def key(self) -> Union[Hashable, NoneType]:
+        """
+        Returns the key of the dictionary in its parent, or `None` if the 
+        object is the root.
+        """
+        return self._key
+           
+    @property
+    def locked(self) -> bool:
+        """
+        Returns `True` if the object is locked. The property is equpped with a setter.
+        """
+        if self.parent is None:
+            return self._locked if isinstance(self._locked, bool) else False
+        else:
+            return self._locked if isinstance(self._locked, bool) else self.parent.locked
+
+    @property
+    def depth(self) -> int:
+        """
+        Retuns the depth of the actual instance in a layout, starting from 0..
+        """
+        if self.parent is None:
+            return 0
+        else:
+            return self.parent.depth + 1
+        
+    @property
+    def address(self) -> Tuple:
+        """Returns the address of an item."""
+        if self.is_root():
+            return []
+        else:
+            r = self.parent.address
+            r.append(self.key)
+            return r
+
+    def lock(self):
+        """
+        Locks the layout of the dictionary. If a `LinkedDeepDict` is locked,
+        missing keys are handled the same way as they would've been handled
+        if it was a ´dict´. Also, setting or deleting items in a locked
+        dictionary and not possible and you will experience an error upon trying.
+        
+        """
+        self._locked = True
+
+    def unlock(self):
+        """
+        Releases the layout of the dictionary. If a `LinkedDeepDict` is not locked,
+        a missing key creates a new level in the layout, also setting and deleting
+        items becomes an option.
+        
+        """
+        self._locked = False
+        
+    def root(self):
+        """
+        Returns the top-level object in a nested layout.
+        """
+        if self.parent is None:
+            return self
+        else:
+            if self._root is not None:
+                return self._root
+            else:
+                return self.parent.root()
+
+    def is_root(self) -> bool:
+        """
+        Returns `True`, if the object is the root.
+        """
+        return self.parent is None
+
+    def containers(self, *args, inclusive:bool=False, deep:bool=True, 
+                   dtype:Any=None, **kwargs):
+        """
+        Returns all the containers in a nested layout. A dictionary in a nested layout
+        is called a container, only if it contains other containers (it is a parent). 
+
+        Parameters
+        ----------
+        inclusive : bool, Optional
+            If `True`, the object the call is made upon also gets returned.
+            This can be important if you make the call on the root object, which most
+            of the time does not hold onto relevant data directly.
+            Default is `False`.
+
+        deep : bool, Optional
+            If `True` the parser goes into nested dictionaries.
+            Default is `True`
+
+        dtype : Any, Optional
+            Constrains the type of the returned objects.
+            Default is `None`, which means no restriction.
+
+        Returns
+        -------
+        generator
+            Returns a generator object.
+
+        Examples
+        --------
+        A simple example:
+
+        >>> from ldd import LinkedDeepDict
+        >>> data = LinkedDeepDict()
+        >>> data['a', 'b', 'c'] = 1
+        >>> [c.key for c in data.containers()]
+        ['a', 'b']
+
+        We can see, that dictionaries 'a' and 'b' are returned as containers, but 'c' 
+        isn't,  because it is not a parent, there are no deeper levels. 
+
+        >>> [c.key for c in data.containers(inclusive=True, deep=True)]
+        [None, 'a', 'b']
+
+        >>> [c.key for c in data.containers(inclusive=True, deep=False)]     
+        [None, 'a']
+
+        >>> [c.key for c in data.containers(inclusive=False, deep=True)]       
+        ['a', 'b']
+
+        >>> [c.key for c in data.containers(inclusive=False, deep=False)]      
+        ['a']
+
+        """
+        dtype = self.__class__ if dtype is None else dtype
+        return parsedicts(self, inclusive=inclusive, dtype=dtype, deep=deep)
+
+    def __getitem__(self, key):
+        try:
+            if issequence(key):
+                return parseaddress(self, key)
+            else:
+                return super().__getitem__(key)
+        except ValueError:
+            return self.__missing__(key)
+        except KeyError:
+            return self.__missing__(key)
+        
+    def __delitem__(self, key):
+        if self.locked:
+            raise RuntimeError("The object is locked!")
+        super().__delitem__(key)
+
+    def __setitem__(self, key, value):
+        if self.locked:
+            raise RuntimeError("The object is locked!")
+        try:
+            if issequence(key):
+                if not key[0] in self:
+                    d = self.__missing__(key[0])
+                else:
+                    d = self[key[0]]
+                if len(key) > 1:
+                    d.__setitem__(key[1:], value)
+                else:
+                    d = self[key[0]]
+                    if isinstance(d, LinkedDeepDict):
+                        d.__leave_parent__()
+                    if value is None:
+                        del self[key[0]]
+                    else:
+                        self[key[0]] = value
+            else:
+                if key in self:
+                    d = self[key]
+                    if isinstance(d, LinkedDeepDict):
+                        d.__leave_parent__()
+                if value is None:
+                    if key in self:
+                        del self[key]
+                else:
+                    if isinstance(value, LinkedDeepDict):
+                        value.__join_parent__(self, key)
+                    return super().__setitem__(key, value)
+        except KeyError:
+            return self.__missing__(key)
+
+    def __missing__(self, key):
+        if self.locked:
+            raise KeyError("Missing key : {}".format(key))
+        if issequence(key):
+            if key[0] not in self:
+                self[key[0]] = value = self.__class__()
+            else:
+                value = self[key[0]]
+            if len(key) > 1:
+                return value.__missing__(key[1:])
+            else:
+                return value
+        else:
+            self[key] = value = self.__class__()
+            return value
+        
+    def __contains__(self, item: Any):
+        if not isinstance(item, Hashable) and issequence(item):
+            if len(item) == 0:
+                raise ValueError(f"{item} has zero length")
+            else:
+                obj = self
+                for subitem in item:
+                    if not isinstance(subitem, Hashable):
+                        raise TypeError(f"{subitem} is not hashable")
+                    else:
+                        if obj.__contains__(subitem):
+                            obj = obj.__getitem__(subitem)
+                        else:
+                            return False
+                return True
+        elif isinstance(item, Hashable):
+            return super().__contains__(item)
+        else:
+            raise TypeError(f"{item} is not hashable")
+        
+    def __reduce__(self):
+        return self.__class__, tuple(), None, None, self.items()
+    
+    def __repr__(self):
+        frmtstr = self.__class__.__name__ + '(%s)'
+        return frmtstr % (dict.__repr__(self))
+       
+    def __leave_parent__(self):
+        self.parent = None
+        self._root = None
+        self._key = None
+            
+    def __join_parent__(self, parent, key: Hashable = None):
+        self.parent = parent
+        self._root = parent.root()
+        self._key = key
+
+    def items(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, v in dictparser(self):
+                    yield addr, v
+            else:
+                for k, v in parseitems(self):
+                    yield k, v
+        else:
+            for k, v in super().items():
+                yield k, v
+
+    def values(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, v in dictparser(self):
+                    yield addr, v
+            else:
+                for _, v in parseitems(self):
+                    yield v
+        else:
+            for v in super().values():
+                yield v
+
+    def keys(self, *args, deep:bool=False, return_address:bool=False, **kwargs):
+        if deep:
+            if return_address:
+                for addr, _ in dictparser(self):
+                    yield addr
+            else:
+                for k, _ in parseitems(self):
+                    yield k
+        else:
+            for k in super().keys():
+                yield k
```

### Comparing `linkeddeepdict-1.0.0/src/linkeddeepdict/tools/kwargtools.py` & `linkeddeepdict-1.1.0/src/linkeddeepdict/tools/kwargtools.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,76 +1,76 @@
-# -*- coding: utf-8 -*-
-try:
-    from collections.abc import Iterable
-except ImportError:
-    from collections import Iterable
-from typing import Callable
-
-
-def isinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return [key in kwargs for key in keys]
-    else:
-        return keys in kwargs
-
-
-def allinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return all([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def anyinkwargs(keys, **kwargs):
-    if isinstance(keys, Iterable) and not isinstance(keys, str):
-        return any([key in kwargs for key in keys])
-    else:
-        return keys in kwargs
-
-
-def getfromkwargs(keys, default=None, astype=None, **kwargs):
-    res = [kwargs.get(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None,
-                **kwargs):
-    res = [d.pop(k, default) for k in keys]
-    if astype is None:
-        return res
-    else:
-        return [astype(p) for p in res]
-
-
-def getallfromkwargs(keys, default=None, **kwargs):
-    params = getfromkwargs(keys, default=default, **kwargs)
-    if None not in params:
-        return params
-    else:
-        missing = list(filter(lambda p: p == default, params))
-        if len(missing) == 1:
-            key = keys[missing[0]]
-            raise RuntimeError("Parameter {} is missing from the definition!"
-                               .format(key))
-        else:
-            missing_keys = [keys[i] for i in missing]
-            raise RuntimeError("Parameters {} is missing from the definition!"
-                               .format(missing_keys))
-
-
-def getasany(keys, default=None, **kwargs):
-    try:
-        condition = [key in kwargs for key in keys]
-        if not any(condition) == True:
-            return default
-        return kwargs[keys[condition.index(True)]]
-    except Exception:
-        return None
-    
-
-def countkwargs(fnc: Callable, **kwargs):
-    assert callable(fnc)
-    return sum(list(map(fnc, kwargs.keys())))
-
+# -*- coding: utf-8 -*-
+try:
+    from collections.abc import Iterable
+except ImportError:
+    from collections import Iterable
+from typing import Callable
+
+
+def isinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return [key in kwargs for key in keys]
+    else:
+        return keys in kwargs
+
+
+def allinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return all([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def anyinkwargs(keys, **kwargs):
+    if isinstance(keys, Iterable) and not isinstance(keys, str):
+        return any([key in kwargs for key in keys])
+    else:
+        return keys in kwargs
+
+
+def getfromkwargs(keys, default=None, astype=None, **kwargs):
+    res = [kwargs.get(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def popfromkwargs(keys, d: dict = None, *args, default=None, astype=None,
+                **kwargs):
+    res = [d.pop(k, default) for k in keys]
+    if astype is None:
+        return res
+    else:
+        return [astype(p) for p in res]
+
+
+def getallfromkwargs(keys, default=None, **kwargs):
+    params = getfromkwargs(keys, default=default, **kwargs)
+    if None not in params:
+        return params
+    else:
+        missing = list(filter(lambda p: p == default, params))
+        if len(missing) == 1:
+            key = keys[missing[0]]
+            raise RuntimeError("Parameter {} is missing from the definition!"
+                               .format(key))
+        else:
+            missing_keys = [keys[i] for i in missing]
+            raise RuntimeError("Parameters {} is missing from the definition!"
+                               .format(missing_keys))
+
+
+def getasany(keys, default=None, **kwargs):
+    try:
+        condition = [key in kwargs for key in keys]
+        if not any(condition) == True:
+            return default
+        return kwargs[keys[condition.index(True)]]
+    except Exception:
+        return None
+    
+
+def countkwargs(fnc: Callable, **kwargs):
+    assert callable(fnc)
+    return sum(list(map(fnc, kwargs.keys())))
+
```

