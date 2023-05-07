# Comparing `tmp/vmilog-py-0.9.0.tar.gz` & `tmp/vmilog-py-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vmilog-py-0.9.0.tar", last modified: Sat May  6 14:38:14 2023, max compression
+gzip compressed data, was "vmilog-py-1.0.0.tar", last modified: Sun May  7 05:41:31 2023, max compression
```

## Comparing `vmilog-py-0.9.0.tar` & `vmilog-py-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 14:38:14.886163 vmilog-py-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmi485tousb/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmi485tousb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmi485tousb/_uartChannel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmiiputil/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmiiputil/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmiiputil/_iputil.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmilog/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmilog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmilog/_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmilog_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-06 14:38:14.000000 vmilog-py-0.9.0/src/vmilog_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-06 14:38:14.000000 vmilog-py-0.9.0/src/vmilog_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 14:38:14.000000 vmilog-py-0.9.0/src/vmilog_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 14:38:14.000000 vmilog-py-0.9.0/src/vmilog_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-06 14:38:14.000000 vmilog-py-0.9.0/src/vmilog_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmimpeg/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmimpeg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmimpeg/_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 14:38:14.882162 vmilog-py-0.9.0/src/vmimqtt/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmimqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-06 14:37:58.000000 vmilog-py-0.9.0/src/vmimqtt/_mqttchannel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.470600 vmilog-py-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 05:41:31.470600 vmilog-py-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:41:31.470600 vmilog-py-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/vmi485tousb/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmi485tousb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1619 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmi485tousb/_uartChannel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/vmiconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmiconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmiconfig/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/vmiiputil/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmiiputil/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmiiputil/_iputil.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/vmilog/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmilog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmilog/_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.466600 vmilog-py-1.0.0/src/vmilog_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-07 05:41:31.000000 vmilog-py-1.0.0/src/vmilog_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-07 05:41:31.000000 vmilog-py-1.0.0/src/vmilog_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:41:31.000000 vmilog-py-1.0.0/src/vmilog_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 05:41:31.000000 vmilog-py-1.0.0/src/vmilog_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-07 05:41:31.000000 vmilog-py-1.0.0/src/vmilog_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.470600 vmilog-py-1.0.0/src/vmimpeg/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmimpeg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmimpeg/_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:41:31.470600 vmilog-py-1.0.0/src/vmimqtt/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmimqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-07 05:41:15.000000 vmilog-py-1.0.0/src/vmimqtt/_mqttchannel.py
```

### Comparing `vmilog-py-0.9.0/LICENSE` & `vmilog-py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.9.0/PKG-INFO` & `vmilog-py-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmilog-py
-Version: 0.9.0
+Version: 1.0.0
 Summary: log library for vmilabs
 Home-page: https://github.com/openvmi/vmilog-py
 Author: vmilabs
 Author-email: zeekzhou@163.com
 License: Apache-2.0
 Keywords: vmilabs log sdk
 Requires-Python: >=3.6
```

### Comparing `vmilog-py-0.9.0/setup.py` & `vmilog-py-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.9.0"
+VERSION = "1.0.0"
 
 install_requires = [
     'netifaces==0.11.0',
     'pyserial',
     'paho-mqtt'
 ]
```

### Comparing `vmilog-py-0.9.0/src/vmi485tousb/_uartChannel.py` & `vmilog-py-1.0.0/src/vmi485tousb/_uartChannel.py`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.9.0/src/vmilog/_logging.py` & `vmilog-py-1.0.0/src/vmilog/_logging.py`

 * *Files identical despite different names*

### Comparing `vmilog-py-0.9.0/src/vmilog_py.egg-info/PKG-INFO` & `vmilog-py-1.0.0/src/vmilog_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vmilog-py
-Version: 0.9.0
+Version: 1.0.0
 Summary: log library for vmilabs
 Home-page: https://github.com/openvmi/vmilog-py
 Author: vmilabs
 Author-email: zeekzhou@163.com
 License: Apache-2.0
 Keywords: vmilabs log sdk
 Requires-Python: >=3.6
```

### Comparing `vmilog-py-0.9.0/src/vmimqtt/_mqttchannel.py` & `vmilog-py-1.0.0/src/vmimqtt/_mqttchannel.py`

 * *Files identical despite different names*

