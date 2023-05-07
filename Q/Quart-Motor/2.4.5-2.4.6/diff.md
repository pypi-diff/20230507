# Comparing `tmp/Quart-Motor-2.4.5.tar.gz` & `tmp/Quart-Motor-2.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quart-Motor-2.4.5.tar", last modified: Tue May  2 02:27:23 2023, max compression
+gzip compressed data, was "Quart-Motor-2.4.6.tar", last modified: Sun May  7 12:15:38 2023, max compression
```

## Comparing `Quart-Motor-2.4.5.tar` & `Quart-Motor-2.4.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.059043 Quart-Motor-2.4.5/
--rw-r--r--   0 sgp        (501) staff       (20)     1389 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/LICENSE
--rw-r--r--   0 sgp        (501) staff       (20)     7907 2023-05-02 02:27:23.059095 Quart-Motor-2.4.5/PKG-INFO
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058152 Quart-Motor-2.4.5/Quart_Motor.egg-info/
--rw-r--r--   0 sgp        (501) staff       (20)     7907 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/PKG-INFO
--rw-r--r--   0 sgp        (501) staff       (20)      453 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/SOURCES.txt
--rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/dependency_links.txt
--rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/not-zip-safe
--rw-r--r--   0 sgp        (501) staff       (20)       54 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/requires.txt
--rw-r--r--   0 sgp        (501) staff       (20)       18 2023-05-02 02:27:23.000000 Quart-Motor-2.4.5/Quart_Motor.egg-info/top_level.txt
--rw-r--r--   0 sgp        (501) staff       (20)     6940 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/README.md
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058479 Quart-Motor-2.4.5/quart_motor/
--rw-r--r--   0 sgp        (501) staff       (20)     7189 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/__init__.py
--rw-r--r--   0 sgp        (501) staff       (20)     4438 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/helpers.py
--rw-r--r--   0 sgp        (501) staff       (20)     3181 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/quart_motor/wrappers.py
--rw-r--r--   0 sgp        (501) staff       (20)      162 2023-05-02 02:27:23.059263 Quart-Motor-2.4.5/setup.cfg
--rw-r--r--   0 sgp        (501) staff       (20)     2003 2023-05-02 02:25:03.000000 Quart-Motor-2.4.5/setup.py
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058597 Quart-Motor-2.4.5/tests/
--rw-r--r--   0 sgp        (501) staff       (20)      158 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/__init__.py
-drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-02 02:27:23.058933 Quart-Motor-2.4.5/tests/quart_motor_tests/
--rw-r--r--   0 sgp        (501) staff       (20)      144 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/__init__.py
--rw-r--r--   0 sgp        (501) staff       (20)     2866 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/test_connection.py
--rw-r--r--   0 sgp        (501) staff       (20)      915 2023-05-02 02:21:59.000000 Quart-Motor-2.4.5/tests/quart_motor_tests/test_wrappers.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-07 12:15:38.893980 Quart-Motor-2.4.6/
+-rw-r--r--   0 sgp        (501) staff       (20)     1389 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/LICENSE
+-rw-r--r--   0 sgp        (501) staff       (20)     7904 2023-05-07 12:15:38.894036 Quart-Motor-2.4.6/PKG-INFO
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-07 12:15:38.893112 Quart-Motor-2.4.6/Quart_Motor.egg-info/
+-rw-r--r--   0 sgp        (501) staff       (20)     7904 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/PKG-INFO
+-rw-r--r--   0 sgp        (501) staff       (20)      453 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/SOURCES.txt
+-rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/dependency_links.txt
+-rw-r--r--   0 sgp        (501) staff       (20)        1 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/not-zip-safe
+-rw-r--r--   0 sgp        (501) staff       (20)       54 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/requires.txt
+-rw-r--r--   0 sgp        (501) staff       (20)       18 2023-05-07 12:15:38.000000 Quart-Motor-2.4.6/Quart_Motor.egg-info/top_level.txt
+-rw-r--r--   0 sgp        (501) staff       (20)     6937 2023-05-07 12:13:24.000000 Quart-Motor-2.4.6/README.md
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-07 12:15:38.893436 Quart-Motor-2.4.6/quart_motor/
+-rw-r--r--   0 sgp        (501) staff       (20)     7189 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/quart_motor/__init__.py
+-rw-r--r--   0 sgp        (501) staff       (20)     4438 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/quart_motor/helpers.py
+-rw-r--r--   0 sgp        (501) staff       (20)     3208 2023-05-07 12:13:24.000000 Quart-Motor-2.4.6/quart_motor/wrappers.py
+-rw-r--r--   0 sgp        (501) staff       (20)      163 2023-05-07 12:15:38.894225 Quart-Motor-2.4.6/setup.cfg
+-rw-r--r--   0 sgp        (501) staff       (20)     2003 2023-05-07 12:15:34.000000 Quart-Motor-2.4.6/setup.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-07 12:15:38.893547 Quart-Motor-2.4.6/tests/
+-rw-r--r--   0 sgp        (501) staff       (20)      158 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/tests/__init__.py
+drwxr-xr-x   0 sgp        (501) staff       (20)        0 2023-05-07 12:15:38.893872 Quart-Motor-2.4.6/tests/quart_motor_tests/
+-rw-r--r--   0 sgp        (501) staff       (20)      144 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/tests/quart_motor_tests/__init__.py
+-rw-r--r--   0 sgp        (501) staff       (20)     2866 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/tests/quart_motor_tests/test_connection.py
+-rw-r--r--   0 sgp        (501) staff       (20)      915 2023-05-02 02:21:59.000000 Quart-Motor-2.4.6/tests/quart_motor_tests/test_wrappers.py
```

### Comparing `Quart-Motor-2.4.5/LICENSE` & `Quart-Motor-2.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.5/PKG-INFO` & `Quart-Motor-2.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart-Motor
-Version: 2.4.5
+Version: 2.4.6
 Summary: Motor support for Quart applications
 Home-page: https://www.github.com/marirs/quart-motor/
 Download-URL: https://www.github.com/marirs/quart-motor/tags
 Author: Sriram G
 Author-email: marirs@gmail.com
 License: BSD
 Classifier: Environment :: Web Environment
@@ -83,16 +83,16 @@
 work with older versions, but compatibility fixes for older versions will
 not be accepted, and future changes may break compatibility in older
 versions.
 
 Quart-Motor is tested against `supported versions
 <https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
 
-Quart-Motor works very well with 
-- `uvicorn` asgi 
+Quart-Motor works very well with
+- `uvicorn` asgi
 - `hypercorn` asgi
 
 Quart-Motor is tested against `Python 3.7+` versions.
 
 Helpers
 -------
 
@@ -207,15 +207,15 @@
 
 - 2.4.0: Unreleased
 
   - Flask-PyMongo port as released of Flask-PyMongo.
 
 Flask-PyMongo:
 
-- <https://github.com/dcrosta/flask-pymongo> 
+- <https://github.com/dcrosta/flask-pymongo>
 
 
 Contributors of Flask-PyMongo:
 
 - `jeverling <https://github.com/jeverling>`
 - `tang0th <https://github.com/tang0th>`
 - `Fabrice Aneche <https://github.com/akhenakh>`
```

### Comparing `Quart-Motor-2.4.5/Quart_Motor.egg-info/PKG-INFO` & `Quart-Motor-2.4.6/Quart_Motor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quart-Motor
-Version: 2.4.5
+Version: 2.4.6
 Summary: Motor support for Quart applications
 Home-page: https://www.github.com/marirs/quart-motor/
 Download-URL: https://www.github.com/marirs/quart-motor/tags
 Author: Sriram G
 Author-email: marirs@gmail.com
 License: BSD
 Classifier: Environment :: Web Environment
@@ -83,16 +83,16 @@
 work with older versions, but compatibility fixes for older versions will
 not be accepted, and future changes may break compatibility in older
 versions.
 
 Quart-Motor is tested against `supported versions
 <https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
 
-Quart-Motor works very well with 
-- `uvicorn` asgi 
+Quart-Motor works very well with
+- `uvicorn` asgi
 - `hypercorn` asgi
 
 Quart-Motor is tested against `Python 3.7+` versions.
 
 Helpers
 -------
 
@@ -207,15 +207,15 @@
 
 - 2.4.0: Unreleased
 
   - Flask-PyMongo port as released of Flask-PyMongo.
 
 Flask-PyMongo:
 
-- <https://github.com/dcrosta/flask-pymongo> 
+- <https://github.com/dcrosta/flask-pymongo>
 
 
 Contributors of Flask-PyMongo:
 
 - `jeverling <https://github.com/jeverling>`
 - `tang0th <https://github.com/tang0th>`
 - `Fabrice Aneche <https://github.com/akhenakh>`
```

### Comparing `Quart-Motor-2.4.5/README.md` & `Quart-Motor-2.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,16 @@
 work with older versions, but compatibility fixes for older versions will
 not be accepted, and future changes may break compatibility in older
 versions.
 
 Quart-Motor is tested against `supported versions
 <https://www.mongodb.com/support-policy>`_ of MongoDB, 3.5+.
 
-Quart-Motor works very well with 
-- `uvicorn` asgi 
+Quart-Motor works very well with
+- `uvicorn` asgi
 - `hypercorn` asgi
 
 Quart-Motor is tested against `Python 3.7+` versions.
 
 Helpers
 -------
 
@@ -182,15 +182,15 @@
 
 - 2.4.0: Unreleased
 
   - Flask-PyMongo port as released of Flask-PyMongo.
 
 Flask-PyMongo:
 
-- <https://github.com/dcrosta/flask-pymongo> 
+- <https://github.com/dcrosta/flask-pymongo>
 
 
 Contributors of Flask-PyMongo:
 
 - `jeverling <https://github.com/jeverling>`
 - `tang0th <https://github.com/tang0th>`
 - `Fabrice Aneche <https://github.com/akhenakh>`
```

### Comparing `Quart-Motor-2.4.5/quart_motor/__init__.py` & `Quart-Motor-2.4.6/quart_motor/__init__.py`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.5/quart_motor/helpers.py` & `Quart-Motor-2.4.6/quart_motor/helpers.py`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.5/quart_motor/wrappers.py` & `Quart-Motor-2.4.6/quart_motor/wrappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
         if not isinstance(database, db_class):
             raise TypeError(
                 "First argument to MotorCollection must be "
                 "MotorDatabase, not %r" % database
             )
 
-        delegate = _delegate or Collection(
+        delegate = _delegate if _delegate is not None else Collection(
             database.delegate,
             name,
             codec_options=codec_options,
             read_preference=read_preference,
             write_concern=write_concern,
             read_concern=read_concern,
         )
```

### Comparing `Quart-Motor-2.4.5/setup.py` & `Quart-Motor-2.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ]
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name="Quart-Motor",
-    version='2.4.5',
+    version='2.4.6',
     url="https://www.github.com/marirs/quart-motor/",
     download_url="https://www.github.com/marirs/quart-motor/tags",
     license="BSD",
     author="Sriram G",
     author_email="marirs@gmail.com",
     description="Motor support for Quart applications",
     long_description=long_description,
```

### Comparing `Quart-Motor-2.4.5/tests/quart_motor_tests/test_connection.py` & `Quart-Motor-2.4.6/tests/quart_motor_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `Quart-Motor-2.4.5/tests/quart_motor_tests/test_wrappers.py` & `Quart-Motor-2.4.6/tests/quart_motor_tests/test_wrappers.py`

 * *Files identical despite different names*

