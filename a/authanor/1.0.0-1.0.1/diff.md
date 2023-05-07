# Comparing `tmp/authanor-1.0.0.tar.gz` & `tmp/authanor-1.0.1.tar.gz`

## Comparing `authanor-1.0.0.tar` & `authanor-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.0/CHANGELOG.md
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.0/Makefile
--rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.0/README.md
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.0/_vimrc_local.vim
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.0/config.mk
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.0/requirements.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/README.md
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.0/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/make.bat
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/conf.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/index.rst
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/database.rst
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/modules.rst
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.0/docs/source/api/testing.rst
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/_version.py
--rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/__init__.py
--rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/handler.py
--rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/models.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/database/utils.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/testing/__init__.py
--rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.0/src/authanor/testing/helpers.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_db.py
--rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_handler.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_models.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/database/test_utils.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.0/tests/helpers/test_helpers.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.0/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.0/LICENSE
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 authanor-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 authanor-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 authanor-1.0.1/Makefile
+-rw-r--r--   0        0        0     3686 2020-02-02 00:00:00.000000 authanor-1.0.1/README.md
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 authanor-1.0.1/_vimrc_local.vim
+-rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 authanor-1.0.1/config.mk
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 authanor-1.0.1/requirements.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/README.md
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0    10513 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 authanor-1.0.1/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/make.bat
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/conf.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/index.rst
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/database.rst
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/modules.rst
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 authanor-1.0.1/docs/source/api/testing.rst
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/_version.py
+-rw-r--r--   0        0        0     3988 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18064 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/handler.py
+-rw-r--r--   0        0        0     5546 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/models.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/database/utils.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/testing/__init__.py
+-rw-r--r--   0        0        0    10575 2020-02-02 00:00:00.000000 authanor-1.0.1/src/authanor/testing/helpers.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/conftest.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_db.py
+-rw-r--r--   0        0        0    22059 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_handler.py
+-rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_models.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/database/test_utils.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 authanor-1.0.1/tests/helpers/test_helpers.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 authanor-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-1.0.1/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2270 2020-02-02 00:00:00.000000 authanor-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4730 2020-02-02 00:00:00.000000 authanor-1.0.1/PKG-INFO
```

### Comparing `authanor-1.0.0/Makefile` & `authanor-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/README.md` & `authanor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/config.mk` & `authanor-1.0.1/config.mk`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/.pytest_cache/v/cache/nodeids` & `authanor-1.0.1/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/docs/Makefile` & `authanor-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/docs/make.bat` & `authanor-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/docs/source/conf.py` & `authanor-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/docs/source/api/database.rst` & `authanor-1.0.1/docs/source/api/database.rst`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/src/authanor/database/__init__.py` & `authanor-1.0.1/src/authanor/database/__init__.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/src/authanor/database/handler.py` & `authanor-1.0.1/src/authanor/database/handler.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/src/authanor/database/models.py` & `authanor-1.0.1/src/authanor/database/models.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/src/authanor/database/utils.py` & `authanor-1.0.1/src/authanor/database/utils.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/src/authanor/testing/helpers.py` & `authanor-1.0.1/src/authanor/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/tests/conftest.py` & `authanor-1.0.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/tests/database/test_handler.py` & `authanor-1.0.1/tests/database/test_handler.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/tests/database/test_models.py` & `authanor-1.0.1/tests/database/test_models.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/tests/helpers/test_helpers.py` & `authanor-1.0.1/tests/helpers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/.gitignore` & `authanor-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `authanor-1.0.0/COPYING` & `authanor-1.0.1/COPYING`

 * *Files identical despite different names*

