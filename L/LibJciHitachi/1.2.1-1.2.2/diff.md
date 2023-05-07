# Comparing `tmp/LibJciHitachi-1.2.1.tar.gz` & `tmp/LibJciHitachi-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibJciHitachi-1.2.1.tar", last modified: Fri May  5 07:22:10 2023, max compression
+gzip compressed data, was "LibJciHitachi-1.2.2.tar", last modified: Sun May  7 16:37:32 2023, max compression
```

## Comparing `LibJciHitachi-1.2.1.tar` & `LibJciHitachi-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/JciHitachi/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35711 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/aws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/JciHitachi/cert/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/AmazonRootCA1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/mqtt_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_aws_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/JciHitachi/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40937 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36190 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/aws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/JciHitachi/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/AmazonRootCA1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/mqtt_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/JciHitachi/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.640206 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 16:37:32.000000 LibJciHitachi-1.2.2/LibJciHitachi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:37:32.644206 LibJciHitachi-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_aws_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-07 16:37:18.000000 LibJciHitachi-1.2.2/tests/test_status.py
```

### Comparing `LibJciHitachi-1.2.1/JciHitachi/api.py` & `LibJciHitachi-1.2.2/JciHitachi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1290,15 +1290,15 @@
                 },
             },
             status_name: status_value,
             "TaskID": self.task_id,
             "Timestamp": time.time(),
         })
 
-        _, _, _, control_results = self._mqtt.execute()
+        _, _, _, control_results = self._mqtt.execute(control=True)
 
         if thing.thing_name in control_results:
             device_control = self._mqtt.mqtt_events.device_control.get(thing.thing_name)
             if device_control.get(status_name) == status_value:
                 thing.status_code.set_new_status(status_name, status_value)
                 return True
         return False
```

### Comparing `LibJciHitachi-1.2.1/JciHitachi/aws_connection.py` & `LibJciHitachi-1.2.2/JciHitachi/aws_connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -885,41 +885,54 @@
                         ),
                         qos=QOS
                     )
             publish_future.result()
             self._mqtt_events.device_shadow_event[thing_name].wait()
         self._execution_pools.shadow_execution_pool.append(self._wrap_async(thing_name, fn, timeout))
     
-    def execute(self) -> list[list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]]]:
+    def execute(self, control: bool = False) -> list[list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]]]:
         """Execute publish commands in the execution pools.
         
+        Parameters
+        ----------
+        control : bool
+            If True, commands in the `control_execution_pool` will be executed; otherwise, commands in other execution pools will be executed.
+
         Returns
         -------
         list
             Execution results of support, shadow, status, control, respectively.
             Each result is a list containing thing names if the execution was successful or BaseException(s) if an error occurred during execution.
         """
 
         async def runner():
             a, b, c, d = None, None, None, None
-            try:
-                self._execution_lock.acquire()
+            if control and len(self._execution_pools.control_execution_pool) != 0:
+                d = await asyncio.gather(*self._execution_pools.control_execution_pool, return_exceptions=True)
+                self._execution_pools.control_execution_pool.clear()
+            else:
                 if len(self._execution_pools.support_execution_pool) != 0:
                     a = await asyncio.gather(*self._execution_pools.support_execution_pool, return_exceptions=True)
                     self._execution_pools.support_execution_pool.clear()
                 if len(self._execution_pools.shadow_execution_pool) != 0:
                     b = await asyncio.gather(*self._execution_pools.shadow_execution_pool, return_exceptions=True)
                     self._execution_pools.shadow_execution_pool.clear()
                 if len(self._execution_pools.status_execution_pool) != 0:
                     c = await asyncio.gather(*self._execution_pools.status_execution_pool, return_exceptions=True)
                     self._execution_pools.status_execution_pool.clear()
-                if len(self._execution_pools.control_execution_pool) != 0:
-                    d = await asyncio.gather(*self._execution_pools.control_execution_pool, return_exceptions=True)
-                    self._execution_pools.control_execution_pool.clear()
-            finally:
-                self._execution_lock.release()
+            
             return a, b, c, d
+        
+        locked = self._execution_lock.locked()
 
-        results = asyncio.run(runner())
+        try:
+            if locked:
+                _LOGGER.debug("Other execution in progress, waiting for a lock.")
+            self._execution_lock.acquire()
+            if locked:
+                _LOGGER.debug("Lock acquired.")
+            results = asyncio.run(runner())
+        finally:
+            self._execution_lock.release()
         
         return results
```

### Comparing `LibJciHitachi-1.2.1/JciHitachi/cert/AmazonRootCA1.pem` & `LibJciHitachi-1.2.2/JciHitachi/cert/AmazonRootCA1.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.2/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.2/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/connection.py` & `LibJciHitachi-1.2.2/JciHitachi/connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/model.py` & `LibJciHitachi-1.2.2/JciHitachi/model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/mqtt_connection.py` & `LibJciHitachi-1.2.2/JciHitachi/mqtt_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/status.py` & `LibJciHitachi-1.2.2/JciHitachi/status.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/JciHitachi/utility.py` & `LibJciHitachi-1.2.2/JciHitachi/utility.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/LICENSE` & `LibJciHitachi-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/LibJciHitachi.egg-info/PKG-INFO` & `LibJciHitachi-1.2.2/LibJciHitachi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.1/LibJciHitachi.egg-info/SOURCES.txt` & `LibJciHitachi-1.2.2/LibJciHitachi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/PKG-INFO` & `LibJciHitachi-1.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.1
+Version: 1.2.2
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.1/README.md` & `LibJciHitachi-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/setup.py` & `LibJciHitachi-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_api.py` & `LibJciHitachi-1.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_aws_connection.py` & `LibJciHitachi-1.2.2/tests/test_aws_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_integration.py` & `LibJciHitachi-1.2.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_model.py` & `LibJciHitachi-1.2.2/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_sanity.py` & `LibJciHitachi-1.2.2/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.1/tests/test_status.py` & `LibJciHitachi-1.2.2/tests/test_status.py`

 * *Files identical despite different names*

