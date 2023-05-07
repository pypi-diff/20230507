# Comparing `tmp/uecho-1.0.2.tar.gz` & `tmp/uecho-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uecho-1.0.2.tar", last modified: Thu Jan  5 16:13:21 2023, max compression
+gzip compressed data, was "uecho-1.0.3.tar", last modified: Sun May  7 06:00:49 2023, max compression
```

## Comparing `uecho-1.0.2.tar` & `uecho-1.0.3.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.827590 uecho-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-01-05 16:13:09.000000 uecho-1.0.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-05 16:13:21.827590 uecho-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-01-05 16:13:09.000000 uecho-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-01-05 16:13:21.827590 uecho-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-01-05 16:13:09.000000 uecho-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.819590 uecho-1.0.2/uecho/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     9936 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/esv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.823590 uecho-1.0.2/uecho/frame/
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/multicast_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/frame/unicast_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/local_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.823590 uecho-1.0.2/uecho/log/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/log/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/log/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/manufacturer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/node_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/object.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/option.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.823590 uecho-1.0.2/uecho/protocol/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/esv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/protocol/subject.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/remote_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.827590 uecho-1.0.2/uecho/std/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    18667 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/manufacturers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)   111644 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/objects_mra.py
--rw-r--r--   0 runner    (1001) docker     (123)   115978 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/objects_scsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/std/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/super_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.827590 uecho-1.0.2/uecho/util/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/util/bytes.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-01-05 16:13:09.000000 uecho-1.0.2/uecho/util/hex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-05 16:13:21.819590 uecho-1.0.2/uecho.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-01-05 16:13:21.000000 uecho-1.0.2/uecho.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-01-05 16:13:21.000000 uecho-1.0.2/uecho.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-05 16:13:21.000000 uecho-1.0.2/uecho.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-05 16:13:21.000000 uecho-1.0.2/uecho.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-05 16:13:21.000000 uecho-1.0.2/uecho.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.231910 uecho-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-07 06:00:38.000000 uecho-1.0.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-07 06:00:49.231910 uecho-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-07 06:00:38.000000 uecho-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-07 06:00:49.231910 uecho-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-07 06:00:38.000000 uecho-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.227910 uecho-1.0.3/uecho/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10141 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/esv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.227910 uecho-1.0.3/uecho/frame/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/multicast_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/frame/unicast_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/local_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.227910 uecho-1.0.3/uecho/log/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/log/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/log/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/manufacturer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/node_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15549 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.227910 uecho-1.0.3/uecho/protocol/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/esv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/protocol/subject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/remote_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.231910 uecho-1.0.3/uecho/std/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18839 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/manufacturers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)   114940 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/objects_mra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115978 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/objects_scsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/std/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4251 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/super_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.231910 uecho-1.0.3/uecho/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/util/bytes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-07 06:00:38.000000 uecho-1.0.3/uecho/util/hex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 06:00:49.227910 uecho-1.0.3/uecho.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-07 06:00:49.000000 uecho-1.0.3/uecho.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-07 06:00:49.000000 uecho-1.0.3/uecho.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 06:00:49.000000 uecho-1.0.3/uecho.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-07 06:00:49.000000 uecho-1.0.3/uecho.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 06:00:49.000000 uecho-1.0.3/uecho.egg-info/top_level.txt
```

### Comparing `uecho-1.0.2/COPYING` & `uecho-1.0.3/COPYING`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/PKG-INFO` & `uecho-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uecho
-Version: 1.0.2
+Version: 1.0.3
 Summary: uEcho for Python is a portable development framework for ECHONET Lite developers.
 Home-page: https://github.com/cybergarage/uecho-py.git
 Author: Satoshi Konno
 Author-email: skonno@cybergarage.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `uecho-1.0.2/README.md` & `uecho-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/setup.py` & `uecho-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description=f.read()
 
 setuptools.setup(
     name='uecho',
-    version='1.0.2',
+    version='1.0.3',
     description="uEcho for Python is a portable development framework for ECHONET Lite developers.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Satoshi Konno',
     author_email='skonno@cybergarage.org',
     url='https://github.com/cybergarage/uecho-py.git',
     install_requires=[
```

### Comparing `uecho-1.0.2/uecho/__init__.py` & `uecho-1.0.3/uecho/__init__.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/const.py` & `uecho-1.0.3/uecho/std/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,10 +8,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-ECHONET_LITE_VERSION = 0x010D0100
-DEFAULT_POST_MSG_RERTY = 20
-DEFAULT_POST_MSG_WAIT = 0.1
+from .database import Database
+from .object import StandardObject
+
+__all__ = ['Database', 'StandardObject']
```

### Comparing `uecho-1.0.2/uecho/controller.py` & `uecho-1.0.3/uecho/controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import time
 import abc
 import socket
 from typing import Any, Union, List, Tuple, Optional
+from threading import Condition
 
 from .object import Object
 from .local_node import LocalNode
 from .node_profile import NodeProfile
 from .message import Message
 from .protocol.message import Message as ProtocolMessage
 from .property import Property
 from .remote_node import RemoteNode
 from .node import Node
 from .manufacturer import Manufacture
 from .std import Database
-from .const import DEFAULT_POST_MSG_RERTY, DEFAULT_POST_MSG_WAIT
+from .const import DEFAULT_POST_MSG_TIMEOUT
 from .option import IGNORE_SELF_MESSAGE
 from .messages import SearchMessage
 
 
 class ControleListener(metaclass=abc.ABCMeta):
     """ControleListener is an abstract listener class to listen to response and announce messages for nodes.
     """
@@ -73,21 +74,23 @@
                 return False
             if self.response is not None:
                 return False
             return True
 
     __found_nodes: dict
     __last_post_msg: Any    # Controller.__PostMessage
+    __last_post_cond: Condition
     __database: Database
     __listeners: List[ControleListener]
 
     def __init__(self):
         super().__init__()
         self.__found_nodes = {}
         self.__last_post_msg = Controller.__PostMessage()
+        self.__last_post_cond = Condition()
         self.__database = Database()
         self.__listeners = []
 
     def __del__(self):
         super().__del__()
         self.stop()
 
@@ -191,18 +194,17 @@
         """
         self.__last_post_msg = Controller.__PostMessage()
         self.__last_post_msg.request = msg
 
         if not self.send_message(msg, dest):
             return None
 
-        for i in range(DEFAULT_POST_MSG_RERTY):
-            time.sleep(DEFAULT_POST_MSG_WAIT)
-            if self.__last_post_msg.response is not None:
-                break
+        self.__last_post_cond.acquire()
+        self.__last_post_cond.wait(timeout=DEFAULT_POST_MSG_TIMEOUT)
+        self.__last_post_cond.release()
 
         return self.__last_post_msg.response
 
     def start(self) -> bool:
         """Starts the controller to listen to any multicast and unicast messages from other nodes in the same local network, and executes search() after starting.
         """
         if not super().start():
@@ -292,7 +294,10 @@
 
         if msg.is_notification() or msg.is_read_response():
             self._update_properties(msg)
 
         if self.__last_post_msg.is_waiting():
             if self.__last_post_msg.request.is_response_message(msg):
                 self.__last_post_msg.response = msg
+                self.__last_post_cond.acquire()
+                self.__last_post_cond.notify()
+                self.__last_post_cond.release()
```

### Comparing `uecho-1.0.2/uecho/device.py` & `uecho-1.0.3/uecho/device.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/esv.py` & `uecho-1.0.3/uecho/esv.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/__init__.py` & `uecho-1.0.3/uecho/frame/__init__.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/interface.py` & `uecho-1.0.3/uecho/frame/interface.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/manager.py` & `uecho-1.0.3/uecho/frame/manager.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/multicast_server.py` & `uecho-1.0.3/uecho/frame/multicast_server.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/server.py` & `uecho-1.0.3/uecho/frame/server.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/frame/unicast_server.py` & `uecho-1.0.3/uecho/frame/unicast_server.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/local_node.py` & `uecho-1.0.3/uecho/local_node.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/log/__init__.py` & `uecho-1.0.3/uecho/log/__init__.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/log/constants.py` & `uecho-1.0.3/uecho/log/constants.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/log/logger.py` & `uecho-1.0.3/uecho/log/logger.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/manufacturer.py` & `uecho-1.0.3/uecho/manufacturer.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/message.py` & `uecho-1.0.3/uecho/message.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/messages.py` & `uecho-1.0.3/uecho/messages.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/node.py` & `uecho-1.0.3/uecho/node.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/node_profile.py` & `uecho-1.0.3/uecho/node_profile.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/object.py` & `uecho-1.0.3/uecho/object.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/option.py` & `uecho-1.0.3/uecho/option.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/profile.py` & `uecho-1.0.3/uecho/profile.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/property.py` & `uecho-1.0.3/uecho/property.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/__init__.py` & `uecho-1.0.3/uecho/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/esv.py` & `uecho-1.0.3/uecho/protocol/esv.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/message.py` & `uecho-1.0.3/uecho/protocol/message.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/observer.py` & `uecho-1.0.3/uecho/protocol/observer.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/property.py` & `uecho-1.0.3/uecho/protocol/property.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/protocol/subject.py` & `uecho-1.0.3/uecho/protocol/subject.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/remote_node.py` & `uecho-1.0.3/uecho/remote_node.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/std/__init__.py` & `uecho-1.0.3/uecho/util/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,12 +7,15 @@
 #    http:#www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""
+This module includes general utility classes.
+"""
 
-from .database import Database
-from .object import StandardObject
+from .bytes import Bytes
+from .hex import Hex
 
-__all__ = ['Database', 'StandardObject']
+__all__ = ['Bytes', 'Hex']
```

### Comparing `uecho-1.0.2/uecho/std/database.py` & `uecho-1.0.3/uecho/std/database.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/std/manufacturers.py` & `uecho-1.0.3/uecho/std/manufacturers.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 __std_manufactures[0x00012E] = Manufacture(0x00012E, "Eneres Co.,Ltd.")
 __std_manufactures[0x000041] = Manufacture(0x000041, "ENEGATE CO.,LTD.")
 __std_manufactures[0x00010A] = Manufacture(0x00010A, "ENERGY GAP CORPORATION")
 __std_manufactures[0x0000F3] = Manufacture(0x0000F3, "Energy Gateway, Inc")
 __std_manufactures[0x0000F2] = Manufacture(0x0000F2, "Energy Solutions Inc.")
 __std_manufactures[0x000072] = Manufacture(0x000072, "Eneres Co.,Ltd.")
 __std_manufactures[0x0000DD] = Manufacture(0x0000DD, "EneStone Corporation")
+__std_manufactures[0x000132] = Manufacture(0x000132, "EX4Energy, Inc.")
 __std_manufactures[0x000055] = Manufacture(0x000055, "FAMILYNET JAPAN CORPORATION")
 __std_manufactures[0x0000F6] = Manufacture(0x0000F6, "Field Logic Inc.")
 __std_manufactures[0x00012F] = Manufacture(0x00012F, "FORMOSA BIO AND ENERGY CORP JAPAN")
 __std_manufactures[0x0000CB] = Manufacture(0x0000CB, "Fuji Electric Co.,Ltd")
 __std_manufactures[0x0000FC] = Manufacture(0x0000FC, "FUJI INDUSTRIAL CO.,Ltd.")
 __std_manufactures[0x000051] = Manufacture(0x000051, "Fuji IT Co.,Ltd.")
 __std_manufactures[0x00008A] = Manufacture(0x00008A, "FUJITSU GENERAL LIMITED")
@@ -95,15 +96,15 @@
 __std_manufactures[0x0000BB] = Manufacture(0x0000BB, "Hokuriku Electric Power Transmission & Distribution Company")
 __std_manufactures[0x0000A1] = Manufacture(0x0000A1, "Honda R&D Co., Ltd.")
 __std_manufactures[0x000115] = Manufacture(0x000115, "HUAWEI TECHNOLOGIES JAPAN K.K.")
 __std_manufactures[0x0000AC] = Manufacture(0x0000AC, "IDEC COROPRATION")
 __std_manufactures[0x00004D] = Manufacture(0x00004D, "INABA DENKI SANGYO CO.,LTD.")
 __std_manufactures[0x000056] = Manufacture(0x000056, "iND Co.,Ltd")
 __std_manufactures[0x0000ED] = Manufacture(0x0000ED, "INFINI Co. LTD")
-__std_manufactures[0x0000F2] = Manufacture(0x0000F2, "INTEC Inc.")
+__std_manufactures[0x000124] = Manufacture(0x000124, "INTEC Inc.")
 __std_manufactures[0x0000B1] = Manufacture(0x0000B1, "Internet Initiative Japan Inc.")
 __std_manufactures[0x000087] = Manufacture(0x000087, "I-O DATA DEVICE,INC.")
 __std_manufactures[0x00006B] = Manufacture(0x00006B, "ISB Corporation")
 __std_manufactures[0x00010F] = Manufacture(0x00010F, "Iwatani Corporation")
 __std_manufactures[0x000081] = Manufacture(0x000081, "IWATSU ELECTRIC CO., LTD.")
 __std_manufactures[0x0000C3] = Manufacture(0x0000C3, "Japan Electric Meters Inspection Corporation")
 __std_manufactures[0x0000F7] = Manufacture(0x0000F7, "JCity,Inc.")
@@ -181,14 +182,15 @@
 __std_manufactures[0x00010E] = Manufacture(0x00010E, "SANIX INCORPORATED")
 __std_manufactures[0x0000BA] = Manufacture(0x0000BA, "SankyoTateyama, Inc.")
 __std_manufactures[0x0000C5] = Manufacture(0x0000C5, "SANWA SHUTTER CORPORATION")
 __std_manufactures[0x000093] = Manufacture(0x000093, "SATORI ELECTRIC CO.,LTD.")
 __std_manufactures[0x000107] = Manufacture(0x000107, "SEIKO ELECTRIC CO.,LTD.")
 __std_manufactures[0x00003A] = Manufacture(0x00003A, "SEKISUI HOUSE, LTD.")
 __std_manufactures[0x000005] = Manufacture(0x000005, "Sharp Corp")
+__std_manufactures[0x000131] = Manufacture(0x000131, "Shenzhen Eternalplanet Energy Pingshan Ltd.")
 __std_manufactures[0x0000AE] = Manufacture(0x0000AE, "SHIKOKU ELECTRIC POWER CO.,INC.")
 __std_manufactures[0x00002E] = Manufacture(0x00002E, "SHIKOKU INSTRUMENTATION CO.,LTD")
 __std_manufactures[0x0000CE] = Manufacture(0x0000CE, "SHINDENGEN ELECTRIC MANUFACTURING CO.LTD.")
 __std_manufactures[0x00010D] = Manufacture(0x00010D, "Shizen Energy Inc.")
 __std_manufactures[0x0000A8] = Manufacture(0x0000A8, "Smart Power System. Co,. Ltd.")
 __std_manufactures[0x0000DF] = Manufacture(0x0000DF, "SMA Japan K.K.")
 __std_manufactures[0x000100] = Manufacture(0x000100, "Smart Solar Corporation")
@@ -226,15 +228,15 @@
 __std_manufactures[0x000069] = Manufacture(0x000069, "Toshiba Lifestyle Products & Services Corporation")
 __std_manufactures[0x00001B] = Manufacture(0x00001B, "TOSHIBA LIGHTING & TECHNOLOGY CORPORATION")
 __std_manufactures[0x000035] = Manufacture(0x000035, "Toshiba Toko Meter Systems Co.,Ltd.")
 __std_manufactures[0x000050] = Manufacture(0x000050, "TOTO LTD.")
 __std_manufactures[0x0000EF] = Manufacture(0x0000EF, "TOYOTA INDUSTRIES CORPORATION")
 __std_manufactures[0x000121] = Manufacture(0x000121, "TOYOTA MOTOR CORPORATION")
 __std_manufactures[0x00011F] = Manufacture(0x00011F, "TOYOTA TSUSHO CORPORATION")
-__std_manufactures[0x00005D] = Manufacture(0x00005D, "Tranceboot Co.,Ltd.")
+__std_manufactures[0x00005C] = Manufacture(0x00005C, "Tranceboot Co.,Ltd.")
 __std_manufactures[0x000076] = Manufacture(0x000076, "TSP CO.,Ltd")
 __std_manufactures[0x0000D0] = Manufacture(0x0000D0, "TSUBAKIMOTO CHAIN CO.")
 __std_manufactures[0x0000C1] = Manufacture(0x0000C1, "Tsuken Electric Ind Co., Ltd.")
 __std_manufactures[0x000053] = Manufacture(0x000053, "Ubiquitous AI Corporation")
 __std_manufactures[0x000117] = Manufacture(0x000117, "WWB Corporation")
 __std_manufactures[0x000095] = Manufacture(0x000095, "Yamato Denki Co.,Ltd.")
 __std_manufactures[0x00009E] = Manufacture(0x00009E, "YASKAWA ELECTRIC CORPORATION")
```

### Comparing `uecho-1.0.2/uecho/std/object.py` & `uecho-1.0.3/uecho/std/object.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/std/objects.py` & `uecho-1.0.3/uecho/std/objects.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/std/objects_mra.py` & `uecho-1.0.3/uecho/std/objects_mra.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,29 +31,29 @@
 obj.add_property(Property(0x80, "Operation status", "state", 1, "required", "optional", "required"))
 obj.add_property(Property(0x81, "Installation location", "raw", 0, "required", "required", "required"))
 obj.add_property(Property(0x81, "Installation location", "", 0, "required", "required", "required"))
 obj.add_property(Property(0x82, "Standard version information", "raw", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0x83, "Identification number", "raw", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0x83, "Identification number", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x84, "Measured instantaneous power consumption", "number", 0, "optional", "notApplicable", "optional"))
-obj.add_property(Property(0x85, "Measured cumulative power consumption", "number", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0x85, "Measured cumulative electric energy consumption", "number", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x86, "Manufacturer's fault code", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x87, "Current limit setting", "number", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0x88, "Fault status", "state", 1, "required", "notApplicable", "required"))
 obj.add_property(Property(0x89, "Fault description", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x8A, "Manufacturer code", "raw", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0x8B, "Business facility code", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x8C, "Product code", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x8D, "Production number", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x8E, "Production date", "date", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x8F, "Power-saving operation setting", "state", 1, "optional", "optional", "optional"))
 obj.add_property(Property(0x93, "Location information", "raw", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0x93, "Location information", "raw", 0, "optional", "optional", "required"))
 obj.add_property(Property(0x93, "Remote control setting", "state", 1, "optional", "optional", "optional"))
-obj.add_property(Property(0x93, "Remote controll setting", "state", 1, "optional", "optional", "optional"))
+obj.add_property(Property(0x93, "Remote control setting", "state", 1, "optional", "optional", "optional"))
 obj.add_property(Property(0x97, "Current time setting", "time", 2, "optional", "optional", "optional"))
 obj.add_property(Property(0x98, "Current date setting", "date", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0x99, "Power limit setting", "number", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0x9A, "Cumulative operating time", "object", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0x9D, "Status change announcement property map", "raw", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0x9E, "Set property map", "raw", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0x9F, "Get property map", "raw", 0, "required", "notApplicable", "optional"))
@@ -217,14 +217,15 @@
 obj.add_property(Property(0xDC, "Charging method", "state", 1, "required", "optional", "required"))
 obj.add_property(Property(0xDC, "Charging method", "state", 1, "required", "optional", "required"))
 obj.add_property(Property(0xDD, "Discharging method", "state", 1, "required", "optional", "required"))
 obj.add_property(Property(0xDD, "Discharging method", "state", 1, "required", "optional", "required"))
 obj.add_property(Property(0xDE, "Purchasing electric power setting", "number", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0xDF, "Re-interconnection permission setting", "state", 1, "optional", "optional", "optional"))
 obj.add_property(Property(0xE0, "Charging/Discharging electric power setting", "number", 0, "optional", "optional", "optional"))
+obj.add_property(Property(0xE1, "Working operation status", "state", 1, "optional", "notApplicable", "required"))
 obj.add_property(Property(0xE2, "Remaining stored electricity of vehicle mounted battery1", "number", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0xE3, "Remaining stored electricity of vehicle mounted battery2", "number", 0, "required_c", "notApplicable", "optional"))
 obj.add_property(Property(0xE3, "Remaining stored electricity of vehicle mounted battery2", "number", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE4, "Remaining stored electricity of vehicle mounted battery3", "number", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0xE5, "Maintenance status", "state", 1, "optional", "notApplicable", "required"))
 obj.add_property(Property(0xE6, "Vehicle ID", "object", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0xE7, "Charging amount setting 1", "number", 0, "optional", "optional", "optional"))
@@ -620,14 +621,15 @@
 obj.add_property(Property(0xE0, "Measured cumulative amount of flowing water", "number", 0, "required", "notApplicable", "optional"))
 obj.add_property(Property(0xE1, "Unit for measured Cumulative amounts of flowing water", "numericValue", 1, "required", "notApplicable", "optional"))
 obj.add_property(Property(0xE2, "Historical data of measured cumulative amount of flowing water", "array", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE3, "Detection of abnormal value in metering data", "state", 1, "optional", "notApplicable", "required"))
 obj.add_property(Property(0xE4, "Security data information", "number", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE5, "ID number setting", "raw", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0xE6, "Verification expiration information", "raw", 0, "optional", "optional", "optional"))
+obj.add_property(Property(0xE7, "Historical data 2 of measured cumulative amount of flowing water", "array", 0, "optional", "notApplicable", "optional"))
 __std_mra_objects[(0x02, 0x81)] = obj
 
 # Home air conditioner (0x0130)
 obj = Object("Home air conditioner", 0x01, 0x30)
 obj.add_property(Property(0x80, "Operation status", "state", 1, "required", "required", "required"))
 obj.add_property(Property(0x8F, "Power-saving operation setting", "state", 1, "required", "required", "required"))
 obj.add_property(Property(0x90, "ON timer-based reservation setting", "state", 1, "optional", "optional", "optional"))
@@ -850,19 +852,14 @@
 obj.add_property(Property(0xE6, "Daily timer setting", "state", 1, "optional", "optional", "optional"))
 obj.add_property(Property(0xE7, "Daily timer setting 1", "bitmap", 6, "optional", "optional", "optional"))
 obj.add_property(Property(0xE8, "Daily timer setting 2", "bitmap", 6, "optional", "optional", "optional"))
 obj.add_property(Property(0xE9, "Rated power consumption", "number", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xEA, "Power consumption measurement method", "state", 1, "optional", "notApplicable", "optional"))
 __std_mra_objects[(0x02, 0x7B)] = obj
 
-# Air pressure sensor (0x002D)
-obj = Object("Air pressure sensor", 0x00, 0x2D)
-obj.add_property(Property(0xE0, "Air pressure measurement", "number", 2, "required", "notApplicable", "optional"))
-__std_mra_objects[(0x00, 0x2D)] = obj
-
 # Bath heating status sensor (0x0016)
 obj = Object("Bath heating status sensor", 0x00, 0x16)
 obj.add_property(Property(0xB0, "Detection threshold level", "level", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0xB1, "Bath heating detection status", "state", 1, "required", "notApplicable", "required"))
 __std_mra_objects[(0x00, 0x16)] = obj
 
 # Cold or hot water heat source equipment (0x027A)
@@ -917,14 +914,39 @@
 # Ventilation fan (0x0133)
 obj = Object("Ventilation fan", 0x01, 0x33)
 obj.add_property(Property(0x80, "Operation status", "state", 1, "required", "required", "required"))
 obj.add_property(Property(0xA0, "Set value of ventilation air flow rate", "", 0, "optional", "optional", "optional"))
 obj.add_property(Property(0xBF, "Ventilation Auto setting", "state", 1, "optional", "optional", "optional"))
 __std_mra_objects[(0x01, 0x33)] = obj
 
+# distributed generator's electric energy meter (0x028E)
+obj = Object("distributed generator's electric energy meter", 0x02, 0x8E)
+obj.add_property(Property(0x98, "Current date setting", "date", 0, "required_c", "optional", "optional"))
+obj.add_property(Property(0xD0, "Device type", "raw", 0, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xD1, "Device ID", "raw", 0, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xD2, "Tolerance class", "state", 1, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xD3, "Number of days to retain historical data of measured cumulative amounts of electric energy", "", 0, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xD4, "Unit for cumulative amounts of electric energy", "numericValue", 1, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xD5, "Day on which the historical data of measured cumulative amounts of electric energy is to be retrieved", "", 0, "required_c", "required", "optional"))
+obj.add_property(Property(0xD6, "Identification number of device to be metered", "raw", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xDA, "Current hour, minute, and second setting", "time", 0, "required_c", "optional", "optional"))
+obj.add_property(Property(0xDB, "Time synchronization status", "state", 1, "required", "notApplicable", "optional"))
+obj.add_property(Property(0xE0, "Measured cumulative amounts of electric energy (AC input)", "number", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE1, "Historical data of measured cumulative amounts of electric energy (AC input)", "object", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE2, "Measured cumulative amounts of electric energy (AC output)", "number", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE3, "Historical data of measured cumulative amounts of electric energy (AC output)", "object", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE4, "Measured cumulative amounts of electric energy (output during a power outage)", "", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xE5, "Historical data of measured cumulative amounts of electric energy (output during a power outage )", "object", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xE6, "Cumulative amounts of electric energy measured at fixed time (AC input)", "object", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE7, "Cumulative amounts of electric energy measured at fixed time (AC output)", "object", 0, "required_c", "notApplicable", "optional"))
+obj.add_property(Property(0xE8, "Cumulative amounts of electric energy measured at fixed time (output during a power outage)", "object", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xE9, "Measured instantaneous electric power (AC input/output)", "", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xEA, "Measured instantaneous electric power (output during a power outage)", "", 0, "optional", "notApplicable", "optional"))
+__std_mra_objects[(0x02, 0x8E)] = obj
+
 # Electric lock (0x026F)
 obj = Object("Electric lock", 0x02, 0x6F)
 obj.add_property(Property(0xE0, "Lock setting1", "state", 1, "required", "required", "required"))
 obj.add_property(Property(0xE1, "Lock setting 2", "state", 1, "optional", "optional", "optional"))
 obj.add_property(Property(0xE2, "Lock status of door guard", "state", 1, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE3, "Door open/close status", "state", 1, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE4, "Occupant/ non-occupant status", "state", 1, "optional", "notApplicable", "optional"))
@@ -976,18 +998,18 @@
 obj.add_property(Property(0xC6, "Connection status", "state", 1, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC7, "Business code of the device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC7, "Business code of the device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC8, "Product code of the device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC8, "Product code of the device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC9, "Manufacture date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xC9, "Manufacture date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
-obj.add_property(Property(0xCA, "Registerd information renewal date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
-obj.add_property(Property(0xCA, "Registerd information renewal date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
-obj.add_property(Property(0xCB, "Registerd information renewal version information of the device to be controlled", "number", 0, "optional", "notApplicable", "optional"))
-obj.add_property(Property(0xCB, "Registerd information renewal version information of the device to be controlled", "number", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xCA, "Registered information renewal date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xCA, "Registered information renewal date of the device to be controlled", "date", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xCB, "Registered information renewal version information of the device to be controlled", "number", 0, "optional", "notApplicable", "optional"))
+obj.add_property(Property(0xCB, "Registered information renewal version information of the device to be controlled", "number", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xCC, "Place to install device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xCD, "Fault status of device to be controlled", "state", 1, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xCE, "Set property map for device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xCF, "Get property map for device to be controlled", "raw", 0, "optional", "notApplicable", "optional"))
 obj.add_property(Property(0xE0, "Address of installation location", "raw", 0, "optional", "notApplicable", "optional"))
 __std_mra_objects[(0x05, 0xFF)] = obj
```

### Comparing `uecho-1.0.2/uecho/std/objects_scsl.py` & `uecho-1.0.3/uecho/std/objects_scsl.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/std/reader.py` & `uecho-1.0.3/uecho/std/reader.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/super_object.py` & `uecho-1.0.3/uecho/super_object.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho/util/__init__.py` & `uecho-1.0.3/uecho/util/hex.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,18 @@
 #    http:#www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""
-This module includes general utility classes.
-"""
 
 from .bytes import Bytes
-from .hex import Hex
 
-__all__ = ['Bytes', 'Hex']
+
+class Hex():
+
+    @classmethod
+    def from_string(cls, val: str) -> int:
+        if not isinstance(val, str):
+            return 0
+        return Bytes.to_int(bytes.fromhex(val))
```

### Comparing `uecho-1.0.2/uecho/util/bytes.py` & `uecho-1.0.3/uecho/util/bytes.py`

 * *Files identical despite different names*

### Comparing `uecho-1.0.2/uecho.egg-info/PKG-INFO` & `uecho-1.0.3/uecho.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uecho
-Version: 1.0.2
+Version: 1.0.3
 Summary: uEcho for Python is a portable development framework for ECHONET Lite developers.
 Home-page: https://github.com/cybergarage/uecho-py.git
 Author: Satoshi Konno
 Author-email: skonno@cybergarage.org
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `uecho-1.0.2/uecho.egg-info/SOURCES.txt` & `uecho-1.0.3/uecho.egg-info/SOURCES.txt`

 * *Files identical despite different names*

