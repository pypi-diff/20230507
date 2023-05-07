# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.3.26.1679833388.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.3.26.1679833388.tar", last modified: Sun Mar 26 12:23:08 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar", last modified: Sun May  7 10:38:50 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388.tar` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1176 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13467 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    11268 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     6791 2023-03-26 12:22:07.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1176 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-03-26 12:23:08.000000 zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13467 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3326 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     7404 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     1879 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    10693 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    12497 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     6791 2023-05-07 10:37:53.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-07 10:38:50.000000 zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.3.26.1679833388
+Version: 1.0.2023.5.7.1683455929
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/README.md` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/setup.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/BlockDevice.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/protocol.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import json
+
+from typing import List
+
 import requests
 
 import config as cfg
 
 """
 USAGE:
 First you have to init factory with base settings
@@ -126,14 +129,55 @@
             self.api_key = api_key
             self.api_base = api_base
 
         def create(self): return Metrics(stage=self.stage, version=self.version, api_key=self.api_key,
                                          api_base=self.api_base)
 
 
+class MetricsCollection(Request):
+    message: List[dict] = []
+
+    def build_url(self):
+        if self.api_is_private_endpoint:
+            return f'{self.api_base}/bulk-post-metrics'
+        else:
+            return f'{self.api_base}{cfg.bulk_post_metrics_ep}'
+
+    def set_data(self, metrics: dict):
+        self.message.append(metrics)
+
+    def clear(self):
+        self.message = []
+
+    class Response:
+        raw_data: dict = None
+        status_code = None
+
+        def __init__(self, res):
+            self.status_code = res.status_code
+            self.raw_data = res.json()
+            for k, v in self.raw_data.items():
+                setattr(self, str(k), v)
+
+    class Factory:
+        stage = None
+        version = None
+        api_key = None
+        api_base = None
+
+        def __init__(self, stage, version, api_key, api_base: str = DEFAULT_BASE_URL):
+            self.stage = stage
+            self.version = version
+            self.api_key = api_key
+            self.api_base = api_base
+
+        def create(self): return MetricsCollection(stage=self.stage, version=self.version, api_key=self.api_key,
+                                                   api_base=self.api_base)
+
+
 class NotifyException(Request):
     message = {}
 
     def build_url(self):
         if self.api_is_private_endpoint:
             return '{}{}'.format(self.api_base, "/post-notify-exception")
         else:
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.3.26.1679833388
+Version: 1.0.2023.5.7.1683455929
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.3.26.1679833388/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.5.7.1683455929/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

