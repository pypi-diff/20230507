# Comparing `tmp/edc-dx-0.1.8.tar.gz` & `tmp/edc-dx-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-dx-0.1.8.tar", last modified: Thu Aug 11 23:24:27 2022, max compression
+gzip compressed data, was "edc-dx-0.1.9.tar", last modified: Fri Aug 12 12:29:41 2022, max compression
```

## Comparing `edc-dx-0.1.8.tar` & `edc-dx-0.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.844859 edc-dx-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-05-25 02:35:41.000000 edc-dx-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 02:35:41.000000 edc-dx-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.838304 edc-dx-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.841006 edc-dx-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-11 23:24:19.000000 edc-dx-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-25 02:35:41.000000 edc-dx-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-11 23:24:19.000000 edc-dx-0.1.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:24:19.000000 edc-dx-0.1.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-25 02:35:41.000000 edc-dx-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-07 03:33:10.000000 edc-dx-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 02:35:41.000000 edc-dx-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1928 2022-08-11 23:24:27.844947 edc-dx-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      926 2022-05-25 02:35:41.000000 edc-dx-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-11 23:24:19.000000 edc-dx-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:24:19.000000 edc-dx-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.841801 edc-dx-0.1.8/edc_dx/
--rw-r--r--   0 erikvw     (501) staff       (20)      156 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)     9163 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/diagnoses.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1961 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/form_validators.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.843259 edc-dx-0.1.8/edc_dx/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.844295 edc-dx-0.1.8/edc_dx/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/etc/user-salt-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)      543 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/holidays.csv
--rw-r--r--   0 erikvw     (501) staff       (20)     3055 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/test_case_mixin.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.844740 edc-dx-0.1.8/edc_dx/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     8145 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/tests/test_diagnoses.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1569 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/tests/test_forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      566 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/tests/test_labels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      252 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2409 2022-05-25 02:35:41.000000 edc-dx-0.1.8/edc_dx/tests/visit_schedule.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1915 2022-05-31 21:04:46.000000 edc-dx-0.1.8/edc_dx/utils.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-11 23:24:27.842574 edc-dx-0.1.8/edc_dx.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1928 2022-08-11 23:24:27.000000 edc-dx-0.1.8/edc_dx.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1078 2022-08-11 23:24:27.000000 edc-dx-0.1.8/edc_dx.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-11 23:24:27.000000 edc-dx-0.1.8/edc_dx.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:39.000000 edc-dx-0.1.8/edc_dx.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)        7 2022-08-11 23:24:27.000000 edc-dx-0.1.8/edc_dx.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1715 2022-08-11 23:24:19.000000 edc-dx-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2717 2022-05-25 02:35:41.000000 edc-dx-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1260 2022-08-11 23:24:27.845241 edc-dx-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.887814 edc-dx-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       78 2022-05-25 02:35:41.000000 edc-dx-0.1.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-25 02:35:41.000000 edc-dx-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.879598 edc-dx-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.882981 edc-dx-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-11 23:24:19.000000 edc-dx-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1843 2022-05-25 02:35:41.000000 edc-dx-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-11 23:24:19.000000 edc-dx-0.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-11 23:24:19.000000 edc-dx-0.1.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2022-05-25 02:35:41.000000 edc-dx-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-07-07 03:33:10.000000 edc-dx-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-25 02:35:41.000000 edc-dx-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1928 2022-08-12 12:29:41.887927 edc-dx-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      926 2022-05-25 02:35:41.000000 edc-dx-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-12 12:29:33.000000 edc-dx-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-11 23:24:19.000000 edc-dx-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.884350 edc-dx-0.1.9/edc_dx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      156 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      109 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     9163 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/diagnoses.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1961 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/form_validators.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.886137 edc-dx-0.1.9/edc_dx/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.887197 edc-dx-0.1.9/edc_dx/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1674 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/etc/user-salt-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      543 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      508 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/holidays.csv
+-rw-r--r--   0 erikvw     (501) staff       (20)     3055 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/test_case_mixin.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.887686 edc-dx-0.1.9/edc_dx/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     8145 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/tests/test_diagnoses.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1569 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/tests/test_forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      566 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/tests/test_labels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      252 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2409 2022-05-25 02:35:41.000000 edc-dx-0.1.9/edc_dx/tests/visit_schedule.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1915 2022-05-31 21:04:46.000000 edc-dx-0.1.9/edc_dx/utils.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-12 12:29:41.885276 edc-dx-0.1.9/edc_dx.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1928 2022-08-12 12:29:41.000000 edc-dx-0.1.9/edc_dx.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1078 2022-08-12 12:29:41.000000 edc-dx-0.1.9/edc_dx.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-12 12:29:41.000000 edc-dx-0.1.9/edc_dx.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-07-09 17:35:39.000000 edc-dx-0.1.9/edc_dx.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)        7 2022-08-12 12:29:41.000000 edc-dx-0.1.9/edc_dx.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1730 2022-08-12 12:29:33.000000 edc-dx-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2717 2022-05-25 02:35:41.000000 edc-dx-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1260 2022-08-12 12:29:41.888251 edc-dx-0.1.9/setup.cfg
```

### Comparing `edc-dx-0.1.8/.github/workflows/build.yml` & `edc-dx-0.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/.gitignore` & `edc-dx-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/.pre-commit-config.yaml` & `edc-dx-0.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/LICENSE` & `edc-dx-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/PKG-INFO` & `edc-dx-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc diagnosis,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-0.1.8/README.rst` & `edc-dx-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/diagnoses.py` & `edc-dx-0.1.9/edc_dx/diagnoses.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/form_validators.py` & `edc-dx-0.1.9/edc_dx/form_validators.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-local-private.pem` & `edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/etc/user-rsa-restricted-private.pem` & `edc-dx-0.1.9/edc_dx/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/forms.py` & `edc-dx-0.1.9/edc_dx/tests/forms.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/test_case_mixin.py` & `edc-dx-0.1.9/edc_dx/tests/test_case_mixin.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/tests/test_diagnoses.py` & `edc-dx-0.1.9/edc_dx/tests/tests/test_diagnoses.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/tests/test_forms.py` & `edc-dx-0.1.9/edc_dx/tests/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/tests/test_labels.py` & `edc-dx-0.1.9/edc_dx/tests/tests/test_labels.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/tests/visit_schedule.py` & `edc-dx-0.1.9/edc_dx/tests/visit_schedule.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx/utils.py` & `edc-dx-0.1.9/edc_dx/utils.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/edc_dx.egg-info/PKG-INFO` & `edc-dx-0.1.9/edc_dx.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-dx
-Version: 0.1.8
+Version: 0.1.9
 Summary: Classes to manage review of HIV, DM and HTN diagnoses for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-dx
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc diagnosis,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-dx-0.1.8/edc_dx.egg-info/SOURCES.txt` & `edc-dx-0.1.9/edc_dx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/pyproject.toml` & `edc-dx-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
     dj40: Django>=4.0,<4.1
     dj41: Django>=4.1,<4.2
     djdev: https://github.com/django/django/tarball/main
 
 commands =
-    pip install -U pip
+    pip install -U pip coverage[toml]
     pip --version
     pip freeze
     coverage run -a runtests.py
     coverage report
 
 [testenv:lint]
 deps = -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/lint.txt
```

### Comparing `edc-dx-0.1.8/runtests.py` & `edc-dx-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-dx-0.1.8/setup.cfg` & `edc-dx-0.1.9/setup.cfg`

 * *Files identical despite different names*

