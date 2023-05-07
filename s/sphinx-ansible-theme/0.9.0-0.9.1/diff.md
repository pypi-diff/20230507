# Comparing `tmp/sphinx-ansible-theme-0.9.0.tar.gz` & `tmp/sphinx-ansible-theme-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-ansible-theme-0.9.0.tar", last modified: Fri Dec 10 11:26:25 2021, max compression
+gzip compressed data, was "sphinx-ansible-theme-0.9.1.tar", last modified: Wed Jan 26 12:53:36 2022, max compression
```

## Comparing `sphinx-ansible-theme-0.9.0.tar` & `sphinx-ansible-theme-0.9.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.494139 sphinx-ansible-theme-0.9.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)       64 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     7065 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1809 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (121)     1095 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-12-10 11:26:25.494139 sphinx-ansible-theme-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      145 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/_static/css/color-scheme.css
--rw-r--r--   0 runner    (1001) docker     (121)    15406 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/_static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (121)    10320 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/_static/images/logo_invert.png
--rw-r--r--   0 runner    (1001) docker     (121)     4723 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      997 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       23 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      263 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      505 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2011 2021-12-10 11:26:25.498139 sphinx-ansible-theme-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.490139 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/
--rw-r--r--   0 runner    (1001) docker     (121)     2091 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/built_with.html
--rw-r--r--   0 runner    (1001) docker     (121)     1264 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrabody.html
--rw-r--r--   0 runner    (1001) docker     (121)      843 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrafooter.html
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrahead.html
--rw-r--r--   0 runner    (1001) docker     (121)      453 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extranav.html
--rw-r--r--   0 runner    (1001) docker     (121)      347 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/footer.html
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/layout.html
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/rtd-ethical-ads.html
--rw-r--r--   0 runner    (1001) docker     (121)      524 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/searchbox.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.486139 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.494139 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/css/
--rw-r--r--   0 runner    (1001) docker     (121)    11032 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/css/ansible.css
--rw-r--r--   0 runner    (1001) docker     (121)       69 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/css/rtd-ethical-ads.css
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.494139 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/images/
--rw-r--r--   0 runner    (1001) docker     (121)      902 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_Black.svg
--rw-r--r--   0 runner    (1001) docker     (121)      624 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_White.svg
--rw-r--r--   0 runner    (1001) docker     (121)      663 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/theme.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/version_chooser.html
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/versions.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 11:26:25.494139 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       46 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2021-12-10 11:26:25.000000 sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2021-12-10 11:26:09.000000 sphinx-ansible-theme-0.9.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)       64 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     7065 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1809 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (121)     1095 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/_static/css/color-scheme.css
+-rw-r--r--   0 runner    (1001) docker     (121)    15406 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/_static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    10320 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/_static/images/logo_invert.png
+-rw-r--r--   0 runner    (1001) docker     (121)     4723 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      997 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2011 2022-01-26 12:53:36.851916 sphinx-ansible-theme-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/
+-rw-r--r--   0 runner    (1001) docker     (121)     2091 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/built_with.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1264 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrabody.html
+-rw-r--r--   0 runner    (1001) docker     (121)      796 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrafooter.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrahead.html
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extranav.html
+-rw-r--r--   0 runner    (1001) docker     (121)      347 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/footer.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/layout.html
+-rw-r--r--   0 runner    (1001) docker     (121)      321 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/rtd-ethical-ads.html
+-rw-r--r--   0 runner    (1001) docker     (121)      524 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/searchbox.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.843916 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/css/
+-rw-r--r--   0 runner    (1001) docker     (121)    11032 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/css/ansible.css
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/css/rtd-ethical-ads.css
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/images/
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_Black.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      624 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_White.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/version_chooser.html
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/versions.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 12:53:36.847916 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       46 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-01-26 12:53:36.000000 sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-01-26 12:53:19.000000 sphinx-ansible-theme-0.9.1/tox.ini
```

### Comparing `sphinx-ansible-theme-0.9.0/.github/workflows/tox.yml` & `sphinx-ansible-theme-0.9.1/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/.gitignore` & `sphinx-ansible-theme-0.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/.pre-commit-config.yaml` & `sphinx-ansible-theme-0.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/LICENSE` & `sphinx-ansible-theme-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/PKG-INFO` & `sphinx-ansible-theme-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-ansible-theme
-Version: 0.9.0
+Version: 0.9.1
 Summary: Ansible Sphinx Theme
 Home-page: https://github.com/ansible-community/sphinx_ansible_theme
 Author: Ansible by Red Hat
 Author-email: info@ansible.com
 Maintainer: Ansible by Red Hat
 Maintainer-email: info@ansible.com
 License: MIT
```

### Comparing `sphinx-ansible-theme-0.9.0/docs/_static/favicon.ico` & `sphinx-ansible-theme-0.9.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/docs/_static/images/logo_invert.png` & `sphinx-ansible-theme-0.9.1/docs/_static/images/logo_invert.png`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/docs/conf.py` & `sphinx-ansible-theme-0.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/docs/index.rst` & `sphinx-ansible-theme-0.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/setup.cfg` & `sphinx-ansible-theme-0.9.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/setup.py` & `sphinx-ansible-theme-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/__init__.py` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/built_with.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/built_with.html`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrabody.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrabody.html`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrafooter.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrafooter.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-<!-- extra footer elements for Ansible beyond RTD Sphinx Theme --->
+<!-- extra footer elements for Ansible beyond RTD Sphinx Theme -->
 {%- if theme_hubspot_id %}
 <!-- begin analytics -->
-<script type="text/javascript">
+<script>
 var _hsq = _hsq || [];
 _hsq.push(["setContentType", "standard-page"]);
       (function(d,s,i,r) {
       if (d.getElementById(i)){return;}
       var n = d.createElement(s),e = document.getElementsByTagName(s)[0];
       n.id=i;n.src = 'https://js.hs-analytics.net/analytics/'+(Math.ceil(new Date()/r)*r)+'/{{ theme_hubspot_id }}.js';
       e.parentNode.insertBefore(n, e);
       })(document, "script", "hs-analytics",300000);
 </script>
 <!-- end analytics -->
 {%- endif %}
 
 {%- if theme_satellite_tracking | tobool %}
-<script type="text/javascript">
+<script>
 if (("undefined" !== typeof _satellite) && ("function" === typeof _satellite.pageBottom)) {
   _satellite.pageBottom();
 }
 </script>
 {%- endif %}
```

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/extrahead.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/extrahead.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-<!---- extra head elements for Ansible beyond RTD Sphinx Theme --->
+<!-- extra head elements for Ansible beyond RTD Sphinx Theme -->
 {%- if theme_satellite_tracking | tobool %}
-<script type="text/javascript" src="https://www.redhat.com/dtm.js"></script>
+<script src="https://www.redhat.com/dtm.js"></script>
 {%- endif %}
 
 {% if theme_swift_id %}
 <!-- <meta class="swiftype" name="published_at" data-type="date" content="2017-12-13" /> -->
 <meta class="swiftype" name="version" data-type="string" content="{{ version }}">
 {% endif %}
 
@@ -14,15 +14,15 @@
  dataLayer = [];
 </script>
 <!-- End Google Tag Manager Data Layer -->
 {%- endif %}
 
 {% if theme_swift_id %}
 {# Ansible search with Swift - do not remove #}
-<script type="text/javascript">
+<script>
   (function(w,d,t,u,n,s,e){w['SwiftypeObject']=n;w[n]=w[n]||function(){
   (w[n].q=w[n].q||[]).push(arguments);};s=d.createElement(t);
   e=d.getElementsByTagName(t)[0];s.async=1;s.src=u;e.parentNode.insertBefore(s,e);
   })(window,document,'script','https://s.swiftypecdn.com/install/v2/st.js','_st');
 
 _st('install','{{ theme_swift_id }}','2.0.0');
 </script>
```

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/layout.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/layout.html`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/searchbox.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/searchbox.html`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/css/ansible.css` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/css/ansible.css`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_Black.svg` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_Black.svg`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_White.svg` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/static/images/Ansible-Mark-RGB_White.svg`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/theme.conf` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme/version_chooser.html` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme/version_chooser.html`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/PKG-INFO` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-ansible-theme
-Version: 0.9.0
+Version: 0.9.1
 Summary: Ansible Sphinx Theme
 Home-page: https://github.com/ansible-community/sphinx_ansible_theme
 Author: Ansible by Red Hat
 Author-email: info@ansible.com
 Maintainer: Ansible by Red Hat
 Maintainer-email: info@ansible.com
 License: MIT
```

### Comparing `sphinx-ansible-theme-0.9.0/sphinx_ansible_theme.egg-info/SOURCES.txt` & `sphinx-ansible-theme-0.9.1/sphinx_ansible_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sphinx-ansible-theme-0.9.0/tox.ini` & `sphinx-ansible-theme-0.9.1/tox.ini`

 * *Files identical despite different names*

