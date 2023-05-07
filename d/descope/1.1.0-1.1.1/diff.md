# Comparing `tmp/descope-1.1.0.tar.gz` & `tmp/descope-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "descope-1.1.0.tar", max compression
+gzip compressed data, was "descope-1.1.1.tar", max compression
```

## Comparing `descope-1.1.0.tar` & `descope-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1064 2023-04-04 08:44:21.303425 descope-1.1.0/LICENSE
--rw-r--r--   0        0        0    28342 2023-04-04 08:44:21.307425 descope-1.1.0/README.md
--rw-r--r--   0        0        0      531 2023-04-04 08:44:21.307425 descope-1.1.0/descope/__init__.py
--rw-r--r--   0        0        0    20073 2023-04-04 08:44:21.307425 descope-1.1.0/descope/auth.py
--rw-r--r--   0        0        0        0 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/__init__.py
--rw-r--r--   0        0        0     4956 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/enchantedlink.py
--rw-r--r--   0        0        0     5451 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/magiclink.py
--rw-r--r--   0        0        0     1588 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/oauth.py
--rw-r--r--   0        0        0    10008 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/otp.py
--rw-r--r--   0        0        0     8200 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/password.py
--rw-r--r--   0        0        0     1541 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/saml.py
--rw-r--r--   0        0        0     5181 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/totp.py
--rw-r--r--   0        0        0     6759 2023-04-04 08:44:21.307425 descope-1.1.0/descope/authmethod/webauthn.py
--rw-r--r--   0        0        0     4360 2023-04-04 08:44:21.307425 descope-1.1.0/descope/common.py
--rw-r--r--   0        0        0    11188 2023-04-04 08:44:21.307425 descope-1.1.0/descope/descope_client.py
--rw-r--r--   0        0        0     1353 2023-04-04 08:44:21.307425 descope-1.1.0/descope/exceptions.py
--rw-r--r--   0        0        0     5661 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/access_key.py
--rw-r--r--   0        0        0     3426 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/common.py
--rw-r--r--   0        0        0     3911 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/group.py
--rw-r--r--   0        0        0     1019 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/jwt.py
--rw-r--r--   0        0        0     2591 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/permission.py
--rw-r--r--   0        0        0     2989 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/role.py
--rw-r--r--   0        0        0     5200 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/sso_settings.py
--rw-r--r--   0        0        0     3477 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/tenant.py
--rw-r--r--   0        0        0    23454 2023-04-04 08:44:21.307425 descope-1.1.0/descope/management/user.py
--rw-r--r--   0        0        0     1408 2023-04-04 08:44:21.307425 descope-1.1.0/descope/mgmt.py
--rw-r--r--   0        0        0     1125 2023-04-04 08:44:49.783311 descope-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    29435 1970-01-01 00:00:00.000000 descope-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-20 15:32:22.171015 descope-1.1.1/LICENSE
+-rw-r--r--   0        0        0    28342 2023-04-20 15:32:22.171015 descope-1.1.1/README.md
+-rw-r--r--   0        0        0      531 2023-04-20 15:32:22.171015 descope-1.1.1/descope/__init__.py
+-rw-r--r--   0        0        0    20073 2023-04-20 15:32:22.171015 descope-1.1.1/descope/auth.py
+-rw-r--r--   0        0        0        0 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/__init__.py
+-rw-r--r--   0        0        0     4956 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/enchantedlink.py
+-rw-r--r--   0        0        0     5451 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/magiclink.py
+-rw-r--r--   0        0        0     1588 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/oauth.py
+-rw-r--r--   0        0        0    10008 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/otp.py
+-rw-r--r--   0        0        0     8200 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/password.py
+-rw-r--r--   0        0        0     1541 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/saml.py
+-rw-r--r--   0        0        0     5181 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/totp.py
+-rw-r--r--   0        0        0     6759 2023-04-20 15:32:22.171015 descope-1.1.1/descope/authmethod/webauthn.py
+-rw-r--r--   0        0        0     4267 2023-04-20 15:32:22.171015 descope-1.1.1/descope/common.py
+-rw-r--r--   0        0        0    11188 2023-04-20 15:32:22.171015 descope-1.1.1/descope/descope_client.py
+-rw-r--r--   0        0        0     1353 2023-04-20 15:32:22.171015 descope-1.1.1/descope/exceptions.py
+-rw-r--r--   0        0        0     5661 2023-04-20 15:32:22.171015 descope-1.1.1/descope/management/access_key.py
+-rw-r--r--   0        0        0     3426 2023-04-20 15:32:22.171015 descope-1.1.1/descope/management/common.py
+-rw-r--r--   0        0        0     3911 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/group.py
+-rw-r--r--   0        0        0     1019 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/jwt.py
+-rw-r--r--   0        0        0     2591 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/permission.py
+-rw-r--r--   0        0        0     2989 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/role.py
+-rw-r--r--   0        0        0     5200 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/sso_settings.py
+-rw-r--r--   0        0        0     3477 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/tenant.py
+-rw-r--r--   0        0        0    23454 2023-04-20 15:32:22.175015 descope-1.1.1/descope/management/user.py
+-rw-r--r--   0        0        0     1408 2023-04-20 15:32:22.175015 descope-1.1.1/descope/mgmt.py
+-rw-r--r--   0        0        0     1125 2023-04-20 15:32:46.674681 descope-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    29435 1970-01-01 00:00:00.000000 descope-1.1.1/PKG-INFO
```

### Comparing `descope-1.1.0/LICENSE` & `descope-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/README.md` & `descope-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/__init__.py` & `descope-1.1.1/descope/__init__.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/auth.py` & `descope-1.1.1/descope/auth.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/enchantedlink.py` & `descope-1.1.1/descope/authmethod/enchantedlink.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/magiclink.py` & `descope-1.1.1/descope/authmethod/magiclink.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/oauth.py` & `descope-1.1.1/descope/authmethod/oauth.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/otp.py` & `descope-1.1.1/descope/authmethod/otp.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/password.py` & `descope-1.1.1/descope/authmethod/password.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/saml.py` & `descope-1.1.1/descope/authmethod/saml.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/totp.py` & `descope-1.1.1/descope/authmethod/totp.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/authmethod/webauthn.py` & `descope-1.1.1/descope/authmethod/webauthn.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/common.py` & `descope-1.1.1/descope/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-import sys
 from enum import Enum
 
 from descope.exceptions import ERROR_TYPE_INVALID_ARGUMENT, AuthException
 
-if "unittest" in sys.modules:
-    DEFAULT_BASE_URL = "http://127.0.0.1"
-else:
-    DEFAULT_BASE_URL = "https://api.descope.com"  # pragma: no cover
+DEFAULT_BASE_URL = "https://api.descope.com"  # pragma: no cover
 
 PHONE_REGEX = """^(?:(?:\\(?(?:00|\\+)([1-4]\\d\\d|[1-9]\\d?)\\)?)?[\\-\\.\\ \\\\/]?)?((?:\\(?\\d{1,}\\)?[\\-\\.\\ \\\\/]?){0,})(?:[\\-\\.\\ \\\\/]?(?:#|ext\\.?|extension|x)[\\-\\.\\ \\\\/]?(\\d+))?$"""
 
 SESSION_COOKIE_NAME = "DS"
 REFRESH_SESSION_COOKIE_NAME = "DSR"
 
 SESSION_TOKEN_NAME = "sessionToken"
```

### Comparing `descope-1.1.0/descope/descope_client.py` & `descope-1.1.1/descope/descope_client.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/exceptions.py` & `descope-1.1.1/descope/exceptions.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/access_key.py` & `descope-1.1.1/descope/management/access_key.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/common.py` & `descope-1.1.1/descope/management/common.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/group.py` & `descope-1.1.1/descope/management/group.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/jwt.py` & `descope-1.1.1/descope/management/jwt.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/permission.py` & `descope-1.1.1/descope/management/permission.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/role.py` & `descope-1.1.1/descope/management/role.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/sso_settings.py` & `descope-1.1.1/descope/management/sso_settings.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/tenant.py` & `descope-1.1.1/descope/management/tenant.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/management/user.py` & `descope-1.1.1/descope/management/user.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/descope/mgmt.py` & `descope-1.1.1/descope/mgmt.py`

 * *Files identical despite different names*

### Comparing `descope-1.1.0/pyproject.toml` & `descope-1.1.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "descope"
-version = "1.1.0"
+version = "1.1.1"
 description = "Descope Python SDK"
 authors = ["Descope <info@descope.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://descope.com/"
 repository = "https://github.com/descope/python-sdk"
 documentation = "https://docs.descope.com"
@@ -23,25 +23,25 @@
 "Bug Tracker" = "https://github.com/descope/python-sdk/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 requests = "2.28.2"
 PyJWT = "==2.6.0"
-cryptography = "==39.0.2"
+cryptography = "==40.0.1"
 email-validator = "==1.3.1"
 
 [tool.poetry.group.dev.dependencies]
 mock = "5.0.1"
 pre-commit = "2.21.0"
 Flask = "2.2.3"
 flake8 = "5.0.4"
 pytest-cov = "4.0.0"
 pytest = "7.2.2"
-black = "23.1.0"
+black = "23.3.0"
 liccheck = "0.8.3"
 isort = "5.11.4"
 pep8-naming = "0.13.3"
 
 [build-system]
 requires = ["poetry-core>=1.1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `descope-1.1.0/PKG-INFO` & `descope-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: descope
-Version: 1.1.0
+Version: 1.1.1
 Summary: Descope Python SDK
 Home-page: https://descope.com/
 License: MIT
 Author: Descope
 Author-email: info@descope.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: PyJWT (==2.6.0)
-Requires-Dist: cryptography (==39.0.2)
+Requires-Dist: cryptography (==40.0.1)
 Requires-Dist: email-validator (==1.3.1)
 Requires-Dist: requests (==2.28.2)
 Project-URL: Bug Tracker, https://github.com/descope/python-sdk/issues
 Project-URL: Documentation, https://docs.descope.com
 Project-URL: Repository, https://github.com/descope/python-sdk
 Description-Content-Type: text/markdown
```

