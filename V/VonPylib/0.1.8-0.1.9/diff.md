# Comparing `tmp/VonPylib-0.1.8.tar.gz` & `tmp/VonPylib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VonPylib-0.1.8.tar", last modified: Fri Nov 18 07:52:12 2022, max compression
+gzip compressed data, was "VonPylib-0.1.9.tar", last modified: Fri Nov 18 11:12:37 2022, max compression
```

## Comparing `VonPylib-0.1.8.tar` & `VonPylib-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2022-11-18 07:52:12.901506 VonPylib-0.1.8/
--rw-rw-rw-   0        0        0     1089 2022-11-18 00:44:24.000000 VonPylib-0.1.8/LICENSE
--rw-rw-rw-   0        0        0      571 2022-11-18 07:52:12.902505 VonPylib-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0       67 2022-11-18 00:44:24.000000 VonPylib-0.1.8/README.md
--rw-rw-rw-   0        0        0      108 2022-11-18 00:44:24.000000 VonPylib-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0      643 2022-11-18 07:52:12.904536 VonPylib-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-11-18 07:52:12.838386 VonPylib-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-11-18 07:52:12.872538 VonPylib-0.1.8/src/VonPylib.egg-info/
--rw-rw-rw-   0        0        0      571 2022-11-18 07:52:12.000000 VonPylib-0.1.8/src/VonPylib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      455 2022-11-18 07:52:12.000000 VonPylib-0.1.8/src/VonPylib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-18 07:52:12.000000 VonPylib-0.1.8/src/VonPylib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2022-11-18 07:52:12.000000 VonPylib-0.1.8/src/VonPylib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-11-18 07:52:12.876537 VonPylib-0.1.8/src/example_package/
--rw-rw-rw-   0        0        0        0 2022-11-18 06:54:15.000000 VonPylib-0.1.8/src/example_package/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-18 06:54:28.000000 VonPylib-0.1.8/src/example_package/example.py
-drwxrwxrwx   0        0        0        0 2022-11-18 07:52:12.900507 VonPylib-0.1.8/src/von/
--rw-rw-rw-   0        0        0        0 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/__init__.py
--rw-rw-rw-   0        0        0     1256 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/devices_helper.py
--rw-rw-rw-   0        0        0     3236 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/future_features.py
--rw-rw-rw-   0        0        0     2236 2022-11-18 01:12:02.000000 VonPylib-0.1.8/src/von/log.py
--rw-rw-rw-   0        0        0     3913 2022-11-18 06:38:54.000000 VonPylib-0.1.8/src/von/mqtt_agent.py
--rw-rw-rw-   0        0        0     2466 2022-11-18 07:50:40.000000 VonPylib-0.1.8/src/von/mqtt_auto_syncer.py
--rw-rw-rw-   0        0        0     5488 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/reprap_arm.py
--rw-rw-rw-   0        0        0      618 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/singleton.py
--rw-rw-rw-   0        0        0     1633 2022-11-18 00:44:24.000000 VonPylib-0.1.8/src/von/terminal_font.py
+drwxrwxrwx   0        0        0        0 2022-11-18 11:12:37.599093 VonPylib-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2022-11-18 00:44:24.000000 VonPylib-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0      571 2022-11-18 11:12:37.601079 VonPylib-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0       67 2022-11-18 00:44:24.000000 VonPylib-0.1.9/README.md
+-rw-rw-rw-   0        0        0      108 2022-11-18 00:44:24.000000 VonPylib-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0      643 2022-11-18 11:12:37.609071 VonPylib-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-18 11:12:37.468150 VonPylib-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-18 11:12:37.532128 VonPylib-0.1.9/src/VonPylib.egg-info/
+-rw-rw-rw-   0        0        0      571 2022-11-18 11:12:37.000000 VonPylib-0.1.9/src/VonPylib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2022-11-18 11:12:37.000000 VonPylib-0.1.9/src/VonPylib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-18 11:12:37.000000 VonPylib-0.1.9/src/VonPylib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2022-11-18 11:12:37.000000 VonPylib-0.1.9/src/VonPylib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-18 11:12:37.550110 VonPylib-0.1.9/src/example_package/
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:54:15.000000 VonPylib-0.1.9/src/example_package/__init__.py
+-rw-rw-rw-   0        0        0        0 2022-11-18 06:54:28.000000 VonPylib-0.1.9/src/example_package/example.py
+drwxrwxrwx   0        0        0        0 2022-11-18 11:12:37.595079 VonPylib-0.1.9/src/von/
+-rw-rw-rw-   0        0        0        0 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/__init__.py
+-rw-rw-rw-   0        0        0     1256 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/devices_helper.py
+-rw-rw-rw-   0        0        0     3236 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/future_features.py
+-rw-rw-rw-   0        0        0     2236 2022-11-18 01:12:02.000000 VonPylib-0.1.9/src/von/log.py
+-rw-rw-rw-   0        0        0     3913 2022-11-18 06:38:54.000000 VonPylib-0.1.9/src/von/mqtt_agent.py
+-rw-rw-rw-   0        0        0     2466 2022-11-18 07:50:40.000000 VonPylib-0.1.9/src/von/mqtt_auto_syncer.py
+-rw-rw-rw-   0        0        0     5035 2022-11-18 11:06:49.000000 VonPylib-0.1.9/src/von/rabbitmq_agent.py
+-rw-rw-rw-   0        0        0     5488 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/reprap_arm.py
+-rw-rw-rw-   0        0        0      618 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/singleton.py
+-rw-rw-rw-   0        0        0     1633 2022-11-18 00:44:24.000000 VonPylib-0.1.9/src/von/terminal_font.py
```

### Comparing `VonPylib-0.1.8/LICENSE` & `VonPylib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/PKG-INFO` & `VonPylib-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VonPylib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A small example package
 Home-page: https://github.com/voicevon/VonPylib
 Author: Xuming Feng
 Author-email: voicevon@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VonPylib-0.1.8/setup.cfg` & `VonPylib-0.1.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2056 6f6e 5079 6c69 620d 0a76 6572   = VonPylib..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e38 0d0a 6175  sion = 0.1.8..au
+00000020: 7369 6f6e 203d 2030 2e31 2e39 0d0a 6175  sion = 0.1.9..au
 00000030: 7468 6f72 203d 2058 756d 696e 6720 4665  thor = Xuming Fe
 00000040: 6e67 0d0a 6175 7468 6f72 5f65 6d61 696c  ng..author_email
 00000050: 203d 2076 6f69 6365 766f 6e40 676d 6169   = voicevon@gmai
 00000060: 6c2e 636f 6d0d 0a64 6573 6372 6970 7469  l.com..descripti
 00000070: 6f6e 203d 2041 2073 6d61 6c6c 2065 7861  on = A small exa
 00000080: 6d70 6c65 2070 6163 6b61 6765 0d0a 6c6f  mple package..lo
 00000090: 6e67 5f64 6573 6372 6970 7469 6f6e 203d  ng_description =
```

### Comparing `VonPylib-0.1.8/src/VonPylib.egg-info/PKG-INFO` & `VonPylib-0.1.9/src/VonPylib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VonPylib
-Version: 0.1.8
+Version: 0.1.9
 Summary: A small example package
 Home-page: https://github.com/voicevon/VonPylib
 Author: Xuming Feng
 Author-email: voicevon@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `VonPylib-0.1.8/src/von/devices_helper.py` & `VonPylib-0.1.9/src/von/devices_helper.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/future_features.py` & `VonPylib-0.1.9/src/von/future_features.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/log.py` & `VonPylib-0.1.9/src/von/log.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/mqtt_agent.py` & `VonPylib-0.1.9/src/von/mqtt_agent.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/mqtt_auto_syncer.py` & `VonPylib-0.1.9/src/von/mqtt_auto_syncer.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/reprap_arm.py` & `VonPylib-0.1.9/src/von/reprap_arm.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/singleton.py` & `VonPylib-0.1.9/src/von/singleton.py`

 * *Files identical despite different names*

### Comparing `VonPylib-0.1.8/src/von/terminal_font.py` & `VonPylib-0.1.9/src/von/terminal_font.py`

 * *Files identical despite different names*

