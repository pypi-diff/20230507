# Comparing `tmp/dt-authentication-ente-1.0.1.tar.gz` & `tmp/dt-authentication-ente-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-authentication-ente-1.0.1.tar", last modified: Thu Mar 23 17:28:51 2023, max compression
+gzip compressed data, was "dt-authentication-ente-2.0.0.tar", last modified: Sun May  7 18:41:25 2023, max compression
```

## Comparing `dt-authentication-ente-1.0.1.tar` & `dt-authentication-ente-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,21 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-03-23 17:28:51.780348 dt-authentication-ente-1.0.1/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-03-23 17:18:14.000000 dt-authentication-ente-1.0.1/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      484 2023-03-23 17:28:51.780348 dt-authentication-ente-1.0.1/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-03-22 22:05:56.000000 dt-authentication-ente-1.0.1/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-03-23 17:28:51.780348 dt-authentication-ente-1.0.1/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2169 2023-03-23 17:18:14.000000 dt-authentication-ente-1.0.1/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-03-23 17:28:51.776348 dt-authentication-ente-1.0.1/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-03-23 17:28:51.780348 dt-authentication-ente-1.0.1/src/dt_authentication/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      152 2023-03-23 17:28:49.000000 dt-authentication-ente-1.0.1/src/dt_authentication/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      108 2023-03-23 17:18:14.000000 dt-authentication-ente-1.0.1/src/dt_authentication/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4132 2023-03-23 17:26:04.000000 dt-authentication-ente-1.0.1/src/dt_authentication/token.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-03-23 17:28:51.780348 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      484 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      433 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       20 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/entry_points.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-03-23 17:28:51.000000 dt-authentication-ente-1.0.1/src/dt_authentication_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       34 2023-04-19 19:49:17.000000 dt-authentication-ente-2.0.0/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      400 2023-04-19 19:49:17.000000 dt-authentication-ente-2.0.0/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2299 2023-05-07 18:37:07.000000 dt-authentication-ente-2.0.0/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/src/dt_authentication/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      153 2023-05-07 18:40:59.000000 dt-authentication-ente-2.0.0/src/dt_authentication/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2545 2023-05-07 18:36:38.000000 dt-authentication-ente-2.0.0/src/dt_authentication/cli.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      218 2023-05-07 18:35:09.000000 dt-authentication-ente-2.0.0/src/dt_authentication/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2194 2023-05-07 07:05:57.000000 dt-authentication-ente-2.0.0/src/dt_authentication/scope.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8445 2023-05-07 18:36:14.000000 dt-authentication-ente-2.0.0/src/dt_authentication/token.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1415 2023-05-07 07:29:27.000000 dt-authentication-ente-2.0.0/src/dt_authentication/utils.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-05-07 18:41:25.002045 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      490 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      524 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      127 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/entry_points.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       13 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-05-07 18:41:24.000000 dt-authentication-ente-2.0.0/src/dt_authentication_ente.egg-info/top_level.txt
```

### Comparing `dt-authentication-ente-1.0.1/setup.py` & `dt-authentication-ente-2.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # :==> Fill in your project data here
 # The package name is the name on PyPI
 # it is not the python module names.
 distro = 'ente'
 package_name = 'dt-authentication-{}'.format(distro)
 library_webpage = 'http://github.com/duckietown/lib-dt-authentication'
 maintainer = 'Andrea F. Daniele'
-maintainer_email = 'afdaniele@ttic.edu'
+maintainer_email = 'afdaniele@duckietown.com'
 short_description = 'Authentication client library used to decode Duckietown Tokens'
 full_description = """
 Authentication client library used to decode Duckietown Tokens.
 """
 
 
 # Read version from the __init__ file
@@ -51,15 +51,19 @@
 description = """
 {name}: {short}
 {underline}
 
 {long}
 """.format(name=package_name, short=short_description, long=full_description, underline=underline)
 
-console_scripts = []
+console_scripts = [
+    "dt-tokens-generate = dt_authentication.cli:cli_generate",
+    "dt-tokens-verify = dt_authentication.cli:cli_verify",
+]
+
 # setup package
 setup(
     name=package_name,
     author=maintainer,
     author_email=maintainer_email,
     url=library_webpage,
     tests_require=tests_require,
```

