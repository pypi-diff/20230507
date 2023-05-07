# Comparing `tmp/queenbee-local-0.5.3.tar.gz` & `tmp/queenbee-local-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/queenbee-local-0.5.3.tar", last modified: Sat May  6 23:16:11 2023, max compression
+gzip compressed data, was "dist/queenbee-local-0.5.4.tar", last modified: Sun May  7 02:10:30 2023, max compression
```

## Comparing `queenbee-local-0.5.3.tar` & `queenbee-local-0.5.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local/
--rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/_build/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local/
+-rw-r--r--   0 runner    (1001) docker     (123)    17839 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/queenbee_local/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/queenbee_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 02:10:30.000000 queenbee-local-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-07 02:09:21.000000 queenbee-local-0.5.4/setup.py
```

### Comparing `queenbee-local-0.5.3/.github/workflows/ci.yaml` & `queenbee-local-0.5.4/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/LICENSE` & `queenbee-local-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/PKG-INFO` & `queenbee-local-0.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.3
+Version: 0.5.4
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.3/docs/conf.py` & `queenbee-local-0.5.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/queenbee_local/__init__.py` & `queenbee-local-0.5.4/queenbee_local/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 import logging
 import logging.config
 import subprocess
 import socket
 import pathlib
 import os
+import time
 import shutil
 import tempfile
 import platform
 import json
 import warnings
 from datetime import datetime, timedelta
 
@@ -368,53 +369,73 @@
         warnings.warn(
             'load_input_param classmethod is deprecated. Update your code to use the '
             'function directly instead.',
             category=DeprecationWarning, stacklevel=2
         )
         return load_input_param(input_param)
 
-    def _update_status(self, logger, started=True, cpu_seconds=0):
-        """Update run status."""
-        if not hasattr(self, '_status_lock'):
-            warnings.warn(
-                'This recipe is generated by an older version of queenbee luigi. '
-                'Update the recipe to get the run status.'
+    def _try_update_status(self, logger, started, cpu_seconds, sleep=0):
+        if sleep:
+            logger.info(
+                f'Re-trying to read and update the status after {sleep} seconds.'
             )
-            return
+            time.sleep(sleep)
+
         with self._status_lock:
             # open JSON file
             inf = self.status_file()
             # update values
             try:
                 data = json.loads(inf.read_text())
             except json.JSONDecodeError:
                 # this should not happen unless user directly interacts with the status
                 # file and blocks the status update
-                return
-            data['meta']['resources_duration']['cpu'] += cpu_seconds
-            progress = data['meta']['progress']
-            if started:
-                progress['running'] += 1
-                progress['total'] += 1
+                logger.info('Failed to read the status file.')
+                # create a copy for debugging.
+                shutil.copy(inf.as_posix(), inf.parent.joinpath(inf.name + 'bak'))
+                return False
             else:
-                # task finished
-                progress['running'] -= 1
-                progress['completed'] += 1
-                if progress['running'] < 0:
-                    # apparently this can happen is complicated workflows.
-                    # I can spend hours to replicate and fix this issue but it is not
-                    # really critical. This small fix will make it look reasonable.
-                    progress['running'] = 0
+                data['meta']['resources_duration']['cpu'] += cpu_seconds
+                progress = data['meta']['progress']
+                if started:
+                    progress['running'] += 1
+                    progress['total'] += 1
+                else:
+                    # task finished
+                    progress['running'] -= 1
+                    progress['completed'] += 1
+                    if progress['running'] < 0:
+                        # apparently this can happen is complicated workflows.
+                        # I can spend hours to replicate and fix this issue but it is not
+                        # really critical. This small fix will make it look reasonable.
+                        progress['running'] = 0
+
+                # write the json file
+                logger.info(
+                    f'[{progress["completed"]}/{progress["total"]}] completed. '
+                    f'{progress["running"]} running.'
+                )
+                inf.write_text(json.dumps(data))
+                return True
 
-            # write the json file
-            logger.info(
-                f'[{progress["completed"]}/{progress["total"]}] completed. '
-                f'{progress["running"]} running.'
+    def _update_status(self, logger, started=True, cpu_seconds=0):
+        """Update run status."""
+        if not hasattr(self, '_status_lock'):
+            warnings.warn(
+                'This recipe is generated by an older version of queenbee luigi. '
+                'Update the recipe to get the run status.'
             )
-            inf.write_text(json.dumps(data))
+            return
+
+        for i in range(3):
+            success = self._try_update_status(
+                logger=logger, started=started, cpu_seconds=cpu_seconds, sleep=i * 3
+            )
+            if success:
+                return
 
 
 def load_input_param(input_param):
     """This function tries to import the values from a file as a Task input
         parameter.
 
     It first tries to import the content as a dictionary assuming the input file is
```

### Comparing `queenbee-local-0.5.3/queenbee_local/cli.py` & `queenbee-local-0.5.4/queenbee_local/cli.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/queenbee_local/helper.py` & `queenbee-local-0.5.4/queenbee_local/helper.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/queenbee_local.egg-info/PKG-INFO` & `queenbee-local-0.5.4/queenbee_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.3
+Version: 0.5.4
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.3/queenbee_local.egg-info/SOURCES.txt` & `queenbee-local-0.5.4/queenbee_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.3/setup.py` & `queenbee-local-0.5.4/setup.py`

 * *Files identical despite different names*

