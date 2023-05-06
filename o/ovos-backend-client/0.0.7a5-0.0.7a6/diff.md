# Comparing `tmp/ovos-backend-client-0.0.7a5.tar.gz` & `tmp/ovos-backend-client-0.0.7a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a5.tar", last modified: Tue Apr 25 14:59:56 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.0.7a6.tar", last modified: Sat May  6 22:28:01 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a5.tar` & `ovos-backend-client-0.0.7a6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.819379 ovos-backend-client-0.0.7a5/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/backends/selene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 14:59:46.000000 ovos-backend-client-0.0.7a5/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-25 14:59:56.000000 ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 14:59:56.823380 ovos-backend-client-0.0.7a5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-04-25 14:59:40.000000 ovos-backend-client-0.0.7a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.170351 ovos-backend-client-0.0.7a6/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22979 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/ovos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/backends/selene.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 22:27:51.000000 ovos-backend-client-0.0.7a6/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-06 22:28:01.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 22:28:00.000000 ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 22:28:01.174351 ovos-backend-client-0.0.7a6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-06 22:27:45.000000 ovos-backend-client-0.0.7a6/setup.py
```

### Comparing `ovos-backend-client-0.0.7a5/README.md` & `ovos-backend-client-0.0.7a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/api.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/api.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/base.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/offline.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/ovos.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/ovos.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/backends/selene.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/backends/selene.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/cloud.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/config.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/database.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/identity.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/pairing.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client/settings.py` & `ovos-backend-client-0.0.7a6/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.0.7a6/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a5/setup.py` & `ovos-backend-client-0.0.7a6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
                 if pkg.strip() and not pkg.startswith("#")]
 
 
 setup(
     name='ovos-backend-client',
     version=get_version(),
     packages=['ovos_backend_client', 'ovos_backend_client.backends'],
+    package_data={'': package_files('ovos_backend_client')},
     url='https://github.com/OpenVoiceOS/ovos-backend-client',
     license='Apache2',
     author='jarbasai',
     install_requires=required("requirements/requirements.txt"),
     extras_require={
         'offline': required('requirements/offline.txt')
     },
```

