# Comparing `tmp/queenbee-local-0.5.2.tar.gz` & `tmp/queenbee-local-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/queenbee-local-0.5.2.tar", last modified: Thu Mar 30 17:30:16 2023, max compression
+gzip compressed data, was "dist/queenbee-local-0.5.3.tar", last modified: Sat May  6 23:16:11 2023, max compression
```

## Comparing `queenbee-local-0.5.2.tar` & `queenbee-local-0.5.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/_build/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local/
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/queenbee_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/queenbee_local/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3759 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/queenbee_local/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/queenbee_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-30 17:30:16.000000 queenbee-local-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-03-30 17:29:17.000000 queenbee-local-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2850 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/_build/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local/
+-rw-r--r--   0 runner    (1001) docker     (123)    17037 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/queenbee_local/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/queenbee_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 23:16:10.000000 queenbee-local-0.5.3/queenbee_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 23:16:11.000000 queenbee-local-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-06 23:15:01.000000 queenbee-local-0.5.3/setup.py
```

### Comparing `queenbee-local-0.5.2/.github/workflows/ci.yaml` & `queenbee-local-0.5.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.2/LICENSE` & `queenbee-local-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.2/PKG-INFO` & `queenbee-local-0.5.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.2
+Version: 0.5.3
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.2/docs/conf.py` & `queenbee-local-0.5.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.2/queenbee_local/__init__.py` & `queenbee-local-0.5.3/queenbee_local/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -393,20 +393,21 @@
             data['meta']['resources_duration']['cpu'] += cpu_seconds
             progress = data['meta']['progress']
             if started:
                 progress['running'] += 1
                 progress['total'] += 1
             else:
                 # task finished
+                progress['running'] -= 1
+                progress['completed'] += 1
                 if progress['running'] < 0:
                     # apparently this can happen is complicated workflows.
                     # I can spend hours to replicate and fix this issue but it is not
                     # really critical. This small fix will make it look reasonable.
                     progress['running'] = 0
-                progress['completed'] += 1
 
             # write the json file
             logger.info(
                 f'[{progress["completed"]}/{progress["total"]}] completed. '
                 f'{progress["running"]} running.'
             )
             inf.write_text(json.dumps(data))
```

### Comparing `queenbee-local-0.5.2/queenbee_local/cli.py` & `queenbee-local-0.5.3/queenbee_local/cli.py`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.2/queenbee_local/helper.py` & `queenbee-local-0.5.3/queenbee_local/helper.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,25 @@
     return ('\t' * indent + string).replace('\t', '    ')
 
 
 def to_camel_case(name: str):
     return ''.join(n.capitalize() for n in name.split('-'))
 
 
-def to_snake_case(name: str):
-    return ''.join(n.lower() for n in name.replace('-', '_'))
+def to_snake_case(name: str, lowercase: bool = False):
+    """Return a snake_case string.
+
+    NOTE: To be able to handle recipe inputs with capital letters this method doesn't
+    change the letters to lowercase by default.
+
+    """
+    if lowercase:
+        return ''.join(n.lower() for n in name.replace('-', '_'))
+    else:
+        return name.replace('-', '_')
 
 
 def parse_input_args(args):
     """Parse input arguments for a recipe module."""
     user_values = {}
     if not 2 <= len(args) <= 4:
         raise ValueError(f'Number of arguments must be between 2-4 not {len(args)}.\n')
```

### Comparing `queenbee-local-0.5.2/queenbee_local.egg-info/PKG-INFO` & `queenbee-local-0.5.3/queenbee_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: queenbee-local
-Version: 0.5.2
+Version: 0.5.3
 Summary: Queenbee local provides a helper module for running queenbee recipes on desktop
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
```

### Comparing `queenbee-local-0.5.2/queenbee_local.egg-info/SOURCES.txt` & `queenbee-local-0.5.3/queenbee_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `queenbee-local-0.5.2/setup.py` & `queenbee-local-0.5.3/setup.py`

 * *Files identical despite different names*

