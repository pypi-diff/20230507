# Comparing `tmp/padacioso-0.2.0.tar.gz` & `tmp/padacioso-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "padacioso-0.2.0.tar", last modified: Fri May  5 21:51:18 2023, max compression
+gzip compressed data, was "padacioso-0.2.1a1.tar", last modified: Sat May  6 22:28:10 2023, max compression
```

## Comparing `padacioso-0.2.0.tar` & `padacioso-0.2.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:51:18.262656 padacioso-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 21:51:12.000000 padacioso-0.2.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 21:51:18.262656 padacioso-0.2.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:51:18.262656 padacioso-0.2.0/padacioso/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-05 21:51:12.000000 padacioso-0.2.0/padacioso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-05 21:51:12.000000 padacioso-0.2.0/padacioso/bracket_expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 21:51:12.000000 padacioso-0.2.0/padacioso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:51:18.262656 padacioso-0.2.0/padacioso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 21:51:18.000000 padacioso-0.2.0/padacioso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 21:51:18.000000 padacioso-0.2.0/padacioso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:51:18.000000 padacioso-0.2.0/padacioso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 21:51:18.000000 padacioso-0.2.0/padacioso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:51:18.000000 padacioso-0.2.0/padacioso.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:51:18.262656 padacioso-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 21:51:12.000000 padacioso-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:51:18.262656 padacioso-0.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-05 21:51:12.000000 padacioso-0.2.0/test/test_padacioso.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/padacioso/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/padacioso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/padacioso/bracket_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/padacioso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/padacioso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-06 22:28:10.000000 padacioso-0.2.1a1/padacioso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-06 22:28:10.000000 padacioso-0.2.1a1/padacioso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:28:10.000000 padacioso-0.2.1a1/padacioso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 22:28:10.000000 padacioso-0.2.1a1/padacioso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 22:28:10.000000 padacioso-0.2.1a1/padacioso.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:10.200299 padacioso-0.2.1a1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7133 2023-05-06 22:28:09.000000 padacioso-0.2.1a1/test/test_padacioso.py
```

### Comparing `padacioso-0.2.0/LICENSE.md` & `padacioso-0.2.1a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.0/padacioso/__init__.py` & `padacioso-0.2.1a1/padacioso/__init__.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.0/padacioso/bracket_expansion.py` & `padacioso-0.2.1a1/padacioso/bracket_expansion.py`

 * *Files identical despite different names*

### Comparing `padacioso-0.2.0/setup.py` & `padacioso-0.2.1a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,15 @@
         return [pkg for pkg in requirements
                 if pkg.strip() and not pkg.startswith("#")]
 
 setup(
     name='padacioso',
     version=get_version(),
     packages=['padacioso'],
+    package_data={'': package_files('padacioso')},
     url='https://github.com/OpenVoiceOS/padacioso',
     license='apache-2.0',
     author='jarbasai',
     author_email='jarbasai@mailfence.com',
     install_requires=required("requirements.txt"),
     description='dead simple intent parser'
 )
```

### Comparing `padacioso-0.2.0/test/test_padacioso.py` & `padacioso-0.2.1a1/test/test_padacioso.py`

 * *Files identical despite different names*

