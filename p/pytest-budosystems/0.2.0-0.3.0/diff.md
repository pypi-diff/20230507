# Comparing `tmp/pytest-budosystems-0.2.0.tar.gz` & `tmp/pytest-budosystems-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-budosystems-0.2.0.tar", last modified: Tue Feb 14 03:40:13 2023, max compression
+gzip compressed data, was "pytest-budosystems-0.3.0.tar", last modified: Sun May  7 00:59:13 2023, max compression
```

## Comparing `pytest-budosystems-0.2.0.tar` & `pytest-budosystems-0.3.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.219337 pytest-budosystems-0.2.0/
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)    11347 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/LICENCE.txt
--rw-rw-rw-   0 root         (0) root         (0)      272 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6156 2023-02-14 03:40:13.218336 pytest-budosystems-0.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5044 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.209336 pytest-budosystems-0.2.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      638 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      764 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.211336 pytest-budosystems-0.2.0/docs/source/
--rw-rw-rw-   0 root         (0) root         (0)       42 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/CommitLog.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.211336 pytest-budosystems-0.2.0/docs/source/_static/
--rw-rw-rw-   0 root         (0) root         (0)     1145 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/_static/budosystems.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.203336 pytest-budosystems-0.2.0/docs/source/_templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.213336 pytest-budosystems-0.2.0/docs/source/_templates/autosummary/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/_templates/autosummary/base.rst
--rw-rw-rw-   0 root         (0) root         (0)     1052 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/_templates/autosummary/class.rst
--rw-rw-rw-   0 root         (0) root         (0)     1485 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/_templates/autosummary/module.rst
--rw-rw-rw-   0 root         (0) root         (0)      195 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/api.rst
--rw-rw-rw-   0 root         (0) root         (0)     6142 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      496 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/docs/source/index.rst
--rw-rw-rw-   0 root         (0) root         (0)    53661 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     9613 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/logo.svg
--rw-rw-rw-   0 root         (0) root         (0)      785 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/mypy.ini
--rw-rw-rw-   0 root         (0) root         (0)    16322 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/pylintrc
--rw-rw-rw-   0 root         (0) root         (0)     2856 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-14 03:40:13.219337 pytest-budosystems-0.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.205336 pytest-budosystems-0.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.204336 pytest-budosystems-0.2.0/src/budosystems/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.204336 pytest-budosystems-0.2.0/src/budosystems/xtra/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.214336 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/
--rw-rw-rw-   0 root         (0) root         (0)      594 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/_version.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.215336 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/
--rw-rw-rw-   0 root         (0) root         (0)      700 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15518 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/abstract_test_repository.py
--rw-rw-rw-   0 root         (0) root         (0)     3228 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.217337 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6156 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1071 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-14 03:40:12.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      190 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-02-14 03:40:13.000000 pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-14 03:40:13.218336 pytest-budosystems-0.2.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)      263 2023-02-14 03:39:52.000000 pytest-budosystems-0.2.0/tests/test_subproject.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.488526 pytest-budosystems-0.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)      272 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6156 2023-05-07 00:59:13.488526 pytest-budosystems-0.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5044 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.478525 pytest-budosystems-0.3.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      764 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.480525 pytest-budosystems-0.3.0/docs/source/
+-rw-rw-rw-   0 root         (0) root         (0)       42 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/CommitLog.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.480525 pytest-budosystems-0.3.0/docs/source/_static/
+-rw-rw-rw-   0 root         (0) root         (0)     1145 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/_static/budosystems.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.472525 pytest-budosystems-0.3.0/docs/source/_templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.481525 pytest-budosystems-0.3.0/docs/source/_templates/autosummary/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/_templates/autosummary/base.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1052 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/_templates/autosummary/class.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1485 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/_templates/autosummary/module.rst
+-rw-rw-rw-   0 root         (0) root         (0)      195 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/api.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6142 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      496 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/docs/source/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)    53661 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     9613 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/logo.svg
+-rw-rw-rw-   0 root         (0) root         (0)      785 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/mypy.ini
+-rw-rw-rw-   0 root         (0) root         (0)    16322 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/pylintrc
+-rw-rw-rw-   0 root         (0) root         (0)     2856 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 00:59:13.488526 pytest-budosystems-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.473525 pytest-budosystems-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.472525 pytest-budosystems-0.3.0/src/budosystems/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.473525 pytest-budosystems-0.3.0/src/budosystems/xtra/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.482525 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/
+-rw-rw-rw-   0 root         (0) root         (0)      594 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.484526 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/
+-rw-rw-rw-   0 root         (0) root         (0)      700 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20321 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/abstract_test_repository.py
+-rw-rw-rw-   0 root         (0) root         (0)     5114 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.486526 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6156 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 00:59:12.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      190 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-07 00:59:13.000000 pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 00:59:13.487526 pytest-budosystems-0.3.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)      263 2023-05-07 00:58:51.000000 pytest-budosystems-0.3.0/tests/test_subproject.py
```

### Comparing `pytest-budosystems-0.2.0/LICENCE.txt` & `pytest-budosystems-0.3.0/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/PKG-INFO` & `pytest-budosystems-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-budosystems
-Version: 0.2.0
+Version: 0.3.0
 Summary:         Budo Systems is a martial arts school management system. This module is the Budo Systems Pytest Plugin.
 Author-email: Joël Larose <joel.larose@budo.systems>
 Project-URL: Repository, https://gitlab.com/budosystems/pytest-budosystems
 Project-URL: Issue Tracker, https://gitlab.com/budosystems/pytest-budosystems/-/issues
 Keywords: Budo Systems,test,pytest
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pytest-budosystems-0.2.0/README.rst` & `pytest-budosystems-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/Makefile` & `pytest-budosystems-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/make.bat` & `pytest-budosystems-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/source/_static/budosystems.css` & `pytest-budosystems-0.3.0/docs/source/_static/budosystems.css`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/source/_templates/autosummary/class.rst` & `pytest-budosystems-0.3.0/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/source/_templates/autosummary/module.rst` & `pytest-budosystems-0.3.0/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/docs/source/conf.py` & `pytest-budosystems-0.3.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/logo.png` & `pytest-budosystems-0.3.0/logo.png`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/logo.svg` & `pytest-budosystems-0.3.0/logo.svg`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/mypy.ini` & `pytest-budosystems-0.3.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/pylintrc` & `pytest-budosystems-0.3.0/pylintrc`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/pyproject.toml` & `pytest-budosystems-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/__init__.py` & `pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/__init__.py` & `pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/src/budosystems/xtra/pytest_suite/repository/abstract_test_repository.py` & `pytest-budosystems-0.3.0/src/budosystems/xtra/pytest_suite/repository/abstract_test_repository.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 #
 """Minimal test suite for all implementations of `Repository`."""
 
-from typing import Any
+from typing import Any, Optional, Union
 from abc import ABC, abstractmethod
 from collections.abc import Generator
 # from uuid import UUID
 
 import pytest
 from pytest import fixture
 
@@ -30,16 +30,21 @@
     EntitySaveFailed, EntityNotFound, EntityAlreadyExists,
     EntityReadFailed, EntityDeleteFailed,
     RepositoryNotAccessible,  # RepositoryError
 )
 
 from .conftest import (
     OneIntFieldEntity as _1IFE,
-    # OneRefFieldEntity as _1RFE,
+    OneRefFieldEntity as _1RFE,
     OneComplexFieldEntity as _1CFE,
+    SimpleUnionFieldEntity as _SUFE,
+    OptionalFieldEntity as _OFE,
+    MappingFieldEntity as _MFE,
+    SequenceFieldEntity as _SFE,
+    KitchenSinkEntity as _KSE,
 )
 
 # pylint: disable=too-many-public-methods
 class AbstractTestRepository(ABC):
     """Standard test suite for implementations of `Repository`."""
 
     @abstractmethod
@@ -50,19 +55,20 @@
     @fixture(scope="class")
     def repo_args(self) -> dict[str, Any]:
         """Returns implementation specific arguments to instantiate the implementation of
         `Repository` being tested."""
         return {}
 
     @fixture(scope="class")
-    def repo_inaccessible(self, repo_class: type[Repository]) -> Repository:
+    def repo_inaccessible(self, repo_class: type[Repository]) -> Optional[Repository]:
         """
         Returns an instance of the implementation of `Repository` with improper connection.
         """
         pytest.skip(f"No 'inaccessible' implementation of {str(repo_class)}")
+        return None
 
     @fixture(scope="class")
     def repository(self,
                    repo_class: type[Repository],
                    repo_args: dict[str, Any],
                    init_data: list[Entity]
                    ) -> Generator[Repository, None, None]:
@@ -221,14 +227,26 @@
         val = 109j
         ent = one_complex_ent(name=ns, slug=ns, c_var=val)
         with pytest.raises(EntityReadFailed) as e:
             _db_ent = repository.load(entity_type=one_complex_ent, entity_id=ent.entity_id)
         assert e.type == EntityReadFailed
         assert isinstance(e.value.reason, TypeError)
 
+    def test_load_wrong_type(self, repository: Repository,
+                             one_int_ent: type[_1IFE],
+                             one_ref_ent: type[_1RFE]) -> None:
+        """Test: Load valid record but with wrong type."""
+        ns = "int_9"
+        val = 9
+        ent = one_int_ent(name=ns, slug=ns, i_var=val)
+        with pytest.raises(EntityReadFailed) as e:
+            _db_ent = repository.load(one_ref_ent, ent.entity_id)
+        assert e.type == EntityReadFailed
+        assert isinstance(e.value.reason, (TypeError, EntityNotFound))
+
     def test_load_repo_not_accessible(self, repo_inaccessible: Repository,
                                       one_int_ent: type[_1IFE]) -> None:
         """Test: Load while repository is not accessible."""
         ns = "int_10"
         val = 10
         ent = one_int_ent(name=ns, slug=ns, i_var=val)
         with pytest.raises(EntityReadFailed) as e:
@@ -329,7 +347,106 @@
         ns = "int_19"
         val = 19
         ent = one_int_ent(name=ns, slug=ns, i_var=val)
         with pytest.raises(EntityDeleteFailed) as e:
             repo_inaccessible.delete(entity_type=one_int_ent, entity_id=ent.entity_id)
         assert e.type == EntityDeleteFailed
         assert isinstance(e.value.reason, RepositoryNotAccessible)
+
+    def test_insert_union_with_value_for_first_type(self, repository: Repository,
+                                                    simple_union_ent: type[_SUFE]) -> None:
+        """Test: Insert with value from first type"""
+        ns = "su_int_20"
+        val = 20
+        ent = simple_union_ent(name=ns, slug=ns, u_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(simple_union_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_union_with_value_for_second_type(self, repository: Repository,
+                                                     simple_union_ent: type[_SUFE]) -> None:
+        """Test: Insert with value from second type"""
+        ns = "su_str_test21"
+        val = "test21"
+        ent = simple_union_ent(name=ns, slug=ns, u_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(simple_union_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_optional_with_none(self, repository: Repository,
+                                       opt_f_ent: type[_OFE]) -> None:
+        """Test: Insert Entity with None in optional value."""
+        ns = "opt_none"
+        val = None
+        ent = opt_f_ent(name=ns, slug=ns, opt_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(opt_f_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_optional_with_value(self, repository: Repository,
+                                        opt_f_ent: type[_OFE]) -> None:
+        """Test: Insert with non-None in optional value."""
+        ns = "opt_value"
+        val = 2.4
+        ent = opt_f_ent(name=ns, slug=ns, opt_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(opt_f_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_mapping(self, repository: Repository,
+                            map_ent: type[_MFE]) -> None:
+        """Test: Insert with mapping."""
+        ns = "mapping"
+        val = {"x": 25, "y": 42}
+        ent = map_ent(name=ns, slug=ns, map_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(map_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_sequence(self, repository: Repository,
+                             seq_ent: type[_SFE]) -> None:
+        """Test: Insert with sequence."""
+        ns = "sequence"
+        val = [3, 4, 26, -2]
+        ent = seq_ent(name=ns, slug=ns, seq_var=val)
+        repository.save(entity=ent)
+        by_slug = repository.match(seq_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
+
+    def test_insert_kitchen_sink(self, repository: Repository,
+                                 kitchen_sink_ent: type[_KSE]) -> None:
+        """Test: Insert entity that features a wide variety of types."""
+        ns = "kitchen_sink_1"
+        vals = {
+                "name": ns,
+                "slug": ns,
+                "s_var": "hello",
+                "i_var": 30,
+                "f_var": 4.2,
+                "c_var": 1+5.9j,
+                "ent_var": _1IFE(name="int_18", slug="int_18", i_var=18),
+                "u_var": 100,
+                "opt_var": None,
+                "map_var": {"a": 0, "b": 4},
+                "seq_var": [-9, 2, -5],
+                "none_var": None,
+                "b_var": False,
+                "opt_num_var": 8j,
+        }
+        ent = kitchen_sink_ent(**vals)
+        repository.save(entity=ent)
+        by_slug = repository.match(kitchen_sink_ent, {"slug": ns})
+        assert len(by_slug) == 1
+        assert by_slug[0] == ent
+        assert by_slug[0] is not ent
```

### Comparing `pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/PKG-INFO` & `pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-budosystems
-Version: 0.2.0
+Version: 0.3.0
 Summary:         Budo Systems is a martial arts school management system. This module is the Budo Systems Pytest Plugin.
 Author-email: Joël Larose <joel.larose@budo.systems>
 Project-URL: Repository, https://gitlab.com/budosystems/pytest-budosystems
 Project-URL: Issue Tracker, https://gitlab.com/budosystems/pytest-budosystems/-/issues
 Keywords: Budo Systems,test,pytest
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pytest-budosystems-0.2.0/src/pytest_budosystems.egg-info/SOURCES.txt` & `pytest-budosystems-0.3.0/src/pytest_budosystems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-budosystems-0.2.0/tests/conftest.py` & `pytest-budosystems-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

