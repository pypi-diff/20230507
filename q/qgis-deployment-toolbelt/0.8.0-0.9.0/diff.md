# Comparing `tmp/qgis-deployment-toolbelt-0.8.0.tar.gz` & `tmp/qgis-deployment-toolbelt-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qgis-deployment-toolbelt-0.8.0.tar", last modified: Mon May 16 21:38:43 2022, max compression
+gzip compressed data, was "qgis-deployment-toolbelt-0.9.0.tar", last modified: Wed May 18 13:05:10 2022, max compression
```

## Comparing `qgis-deployment-toolbelt-0.8.0.tar` & `qgis-deployment-toolbelt-0.9.0.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.405453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/
--rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/cli_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/cli_clean.py
--rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3926 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (121)    10339 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_profiles_synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     9177 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_shortcuts.py
--rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/orchestrator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/remote_git_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)     9618 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/scenarios/
--rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/scenarios/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/scenarios/scenario_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/bouncer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/journalizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/slugger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-16 21:38:43.409453 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-05-16 21:38:42.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1370 2022-05-16 21:38:43.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-16 21:38:42.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-16 21:38:43.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-16 21:38:43.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-16 21:38:43.000000 qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-16 21:38:43.413453 qgis-deployment-toolbelt-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-05-16 21:38:25.000000 qgis-deployment-toolbelt-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     7652 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1950 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.083280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/
+-rw-r--r--   0 runner    (1001) docker     (121)     1366 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7400 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.083280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/cli_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4070 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/cli_clean.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2832 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4767 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10339 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_profiles_synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9177 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_shortcuts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2889 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/orchestrator.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3630 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/remote_git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11250 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/scenarios/
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/scenarios/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6017 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/scenarios/scenario_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)       89 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2493 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/bouncer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4644 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/journalizer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2878 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/slugger.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/str2bool.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2046 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/win32utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-18 13:05:10.083280 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-05-18 13:05:09.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-05-18 13:05:10.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-18 13:05:09.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-05-18 13:05:09.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-05-18 13:05:09.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-18 13:05:09.000000 qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-05-18 13:05:10.087280 qgis-deployment-toolbelt-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2414 2022-05-18 13:04:51.000000 qgis-deployment-toolbelt-0.9.0/setup.py
```

### Comparing `qgis-deployment-toolbelt-0.8.0/LICENSE` & `qgis-deployment-toolbelt-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/PKG-INFO` & `qgis-deployment-toolbelt-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-deployment-toolbelt
-Version: 0.8.0
+Version: 0.9.0
 Summary: QGIS deployment toolbelt is a CLI (Command Line Interface) to perform redundant operations after a QGIS deployment.
 Home-page: https://github.com/Guts/qgis-deployment-cli/
 Author: Julien Moura (Oslandia)
 Author-email: qgis@oslandia.com
 Keywords: cli, QGIS, deployment, profiles
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

### Comparing `qgis-deployment-toolbelt-0.8.0/README.md` & `qgis-deployment-toolbelt-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/__about__.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,14 @@
 __title__ = "QGIS Deployment Toolbelt"
 __title_clean__ = "".join(e for e in __title__ if e.isalnum())
 __uri_homepage__ = "https://guts.github.io/qgis-deployment-cli/"
 __uri_repository__ = "https://github.com/Guts/qgis-deployment-cli/"
 __uri_tracker__ = "https://github.com/Guts/qgis-deployment-cli/issues/"
 __uri__ = __uri_repository__
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 __version_info__ = tuple(
     [
         int(num) if num.isdigit() else num
         for num in __version__.replace("-", ".", 1).split(".")
     ]
 )
```

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/cli.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/cli.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/cli_check.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/cli_check.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/commands/cli_clean.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/commands/cli_clean.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/constants.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/constants.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_environment_variables.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_environment_variables.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 
 # #############################################################################
 # ########## Libraries #############
 # ##################################
 
 # Standard library
 import logging
+from os.path import expanduser, expandvars
+from pathlib import Path
 from sys import platform as opersys
 from typing import List
 
 # Imports depending on operating system
 if opersys == "win32":
     """windows"""
     import win32gui
@@ -56,29 +58,52 @@
     def run(self) -> None:
         """Apply environment variables from dictionary to the system."""
         if opersys == "win32":
             for env_var in self.options:
                 if env_var.get("action") == "add":
                     setenv(
                         name=env_var.get("name"),
-                        value=env_var.get("value"),
+                        value=self.prepare_value(env_var.get("value")),
                         user=env_var.get("scope") == "user",
                         suppress_echo=True,
                     )
             # force Windows to refresh the environment
             self.win_refresh_environment()
 
         # TODO: for linux, edit ~/.profile or add a .env file and source it from ~./profile
         else:
             logger.debug(
                 f"Setting persistent environment variables is not supported on {opersys}"
             )
 
         logger.debug(f"Job {self.ID} ran successfully.")
 
+    def prepare_value(self, value: str) -> str:
+        """Prepare value to be used in the environment variable.
+
+        :param str value: value to prepare.
+        :return str: prepared value.
+        """
+        try:
+            # test if value is a path
+            value_as_path = Path(expanduser(expandvars(value)))
+            if not value_as_path.exists():
+                logger.warning(
+                    f"{value} seems to be a valid path but does not exist (yet)."
+                )
+
+            return str(value_as_path.resolve())
+        except Exception as err:
+            logger.debug(f"Value {value} is not a valid path: {err}")
+
+        if opersys == "win32":
+            return value
+        else:
+            return f'"{value}"'
+
     def validate_options(self, options: List[dict]) -> List[dict]:
         """Validate options.
 
         :param List[dict] options: options to validate.
         :return List[dict]: options if they are valid.
         """
         if not isinstance(options, list):
```

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_profiles_synchronizer.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_profiles_synchronizer.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/job_shortcuts.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/job_shortcuts.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/jobs/orchestrator.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/jobs/orchestrator.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/remote_git_handler.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/remote_git_handler.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/profiles/shortcuts.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/profiles/shortcuts.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # ########## Libraries #############
 # ##################################
 # standard
 import logging
 import os
 from pathlib import Path
 from sys import platform as opersys
-from typing import Tuple, Union
+from typing import Iterable, Tuple, Union
 
 # Imports depending on operating system
 if opersys == "win32":
     """windows"""
     import win32com.client
     from win32comext.shell import shell, shellcon
 else:
@@ -40,28 +40,27 @@
 # ########## Classes ###############
 # ##################################
 class ApplicationShortcut:
     def __init__(
         self,
         name: str,
         exec_path: Union[str, Path],
-        exec_arguments: Tuple[str] = None,
+        exec_arguments: Iterable[str] = None,
         description: str = None,
         icon_path: Union[str, Path] = None,
         work_dir: Union[str, Path] = None,
     ):
         """Initialize a shortcut object.
 
         :param str name: name of the shortcut that will be created
         :param Union[str, Path] exec_path: path to the executable (which should exist)
-        :param Tuple[str] exec_arguments: list of arguments and options to pass to the executable, defaults to None
+        :param Iterable[str] exec_arguments: list of arguments and options to pass to the executable, defaults to None
         :param str description: shortcut description, defaults to None
-        :param Union[str, Path] icon_path: path to icon .ico, defaults to None
+        :param Union[str, Path] icon_path: path to icon file, defaults to None
         :param Union[str, Path] work_dir: current folder where to start the executable, defaults to None
-
         """
         # retrieve operating system specific configuration
         if opersys not in OS_CONFIG:
             raise OSError(
                 f"Your operating system {opersys} is not supported. "
                 f"Supported platforms: {','.join(OS_CONFIG.keys())}."
             )
@@ -82,43 +81,34 @@
                 logger.warning(f"Executable does not exist: {self.exec_path}")
         else:
             raise TypeError(
                 f"exec_path must be a string or pathlib.Path, not {type(exec_path)}"
             )
 
         # optional
-        if not description or isinstance(description, str):
-            self.description = description
+        if isinstance(exec_arguments, (tuple, list, type(None))):
+            self.exec_arguments = self.check_exec_arguments(exec_arguments)
         else:
             raise TypeError(
-                f"If defined, description must be a string, not {type(description)}"
+                f"If defined, exec_arguments must be a tuple or list, not {type(exec_arguments)}"
             )
-
-        if not exec_arguments or isinstance(exec_arguments, (tuple, list)):
-            self.exec_arguments = " ".join(exec_arguments)
+        if isinstance(description, (str, type(None))):
+            self.description = description
         else:
             raise TypeError(
-                f"If defined, exec_arguments must be a tuple or list, not {type(exec_arguments)}"
+                f"If defined, description must be a string, not {type(description)}"
             )
-        if isinstance(icon_path, (str, Path)):
-            self.icon_path = Path(icon_path)
-            if not self.icon_path.exists():
-                logger.warning(f"Icon does not exist: {self.exec_path}")
-        elif icon_path is None:
-            self.icon_path = icon_path
+        if isinstance(icon_path, (str, Path, type(None))):
+            self.icon_path = self.check_icon_path(icon_path)
         else:
             raise TypeError(
                 f"If defined, icon_path must be a string or pathlib.Path, not {type(icon_path)}"
             )
-        if isinstance(work_dir, (str, Path)):
-            self.work_dir = Path(work_dir)
-            if not self.work_dir.exists():
-                logger.warning(f"Work folder does not exist: {self.work_dir}")
-        elif work_dir is None:
-            self.work_dir = work_dir
+        if isinstance(work_dir, (str, Path, type(None))):
+            self.work_dir = self.check_work_dir(work_dir)
         else:
             raise TypeError(
                 f"If defined, work_dir must be a string or pathlib.Path, not {type(work_dir)}"
             )
 
     def create(
         self,
@@ -140,30 +130,83 @@
             self.start_menu = start_menu
         else:
             raise TypeError(f"start_menu must be a boolean, not {type(start_menu)}")
 
         if opersys == "win32":
             return self.win32_create()
 
+    def check_exec_arguments(
+        self, exec_arguments: Union[Iterable[str], None]
+    ) -> Union[Tuple[str], None]:
+        """Check if exec_arguments are valid.
+
+        :param Union[Iterable[str], None] exec_arguments: input executable arguments to check
+
+        :return Union[Tuple[str], None]: tuple of arguments
+        """
+        if not exec_arguments:
+            return None
+        # store as path
+        return " ".join(exec_arguments)
+
+    def check_icon_path(self, icon_path: Union[str, Path, None]) -> Union[Path, None]:
+        """Check icon path and return full path if it exists.
+
+        :param Union[str, Path] icon_path: input icon path to check
+
+        :return Union[Path, None]: icon path as Path if str or Path, else None
+        """
+        if not icon_path:
+            return None
+        # store as path
+        icon_path = Path(icon_path)
+        # checks
+        if icon_path.exists():
+            return icon_path.resolve()
+        else:
+
+            logger.warning(f"Icon does not exist: {icon_path}")
+            return None
+
+    def check_work_dir(self, work_dir: Union[str, Path, None]) -> Union[Path, None]:
+        """Check work dir and return full path if it exists.
+
+        :param Union[str, Path] work_dir: input work dir to check
+
+        :return Union[Path, None]: work dir as Path if str or Path, else None
+        """
+        if not work_dir:
+            return None
+        # store as path
+        work_dir = Path(work_dir)
+        # checks
+        if work_dir.is_dir():
+            return work_dir.resolve()
+        else:
+            logger.warning(f"Work folder does not exist: {work_dir}")
+            return None
+
     # -- PROPERTIES --------------------------------------------------------------
     @property
     def desktop_path(self) -> Path:
         """Return the user Desktop folder.
 
         :return Path: path to the Desktop folder
         """
         if opersys == "win32":
             return Path(shell.SHGetFolderPath(0, shellcon.CSIDL_DESKTOP, None, 0))
 
     @property
     def homedir_path(self) -> Path:
         """Return home directory.
 
-        For Windows, note that we return CSIDL_PROFILE, not CSIDL_APPDATA,
-        CSIDL_LOCAL_APPDATA or CSIDL_COMMON_APPDATA.
+        For Windows, note that we return `CSIDL_PROFILE`, not `CSIDL_APPDATA`,
+        `CSIDL_LOCAL_APPDATA` or `CSIDL_COMMON_APPDATA`.
+        See: https://www.nirsoft.net/articles/find_special_folder_location.html
+        TODO: evaluate use of platformdirs
 
         :return Path: path to the user home
         """
         if opersys == "win32":
             return Path(shell.SHGetFolderPath(0, shellcon.CSIDL_PROFILE, 0, 0))
         elif opersys == "linux":
             home = None
@@ -183,15 +226,15 @@
             logger.error(f"Unrecognized operating system: {opersys}.")
             return None
 
     @property
     def startmenu_path(self) -> Path:
         """Return user Start Menu Programs folder.
 
-        For Windows, note that we return CSIDL_PROGRAMS not CSIDL_COMMON_PROGRAMS.
+        For Windows, note that we return `CSIDL_PROGRAMS` not `CSIDL_COMMON_PROGRAMS`.
 
         :return Path: path to the Start Menu Programs folder
         """
         if opersys == "win32":
             return Path(shell.SHGetFolderPath(0, shellcon.CSIDL_PROGRAMS, None, 0))
         elif opersys == "linux":
             return self.homedir_path / ".local/share/applications"
@@ -243,15 +286,18 @@
             wscript = _WSHELL.CreateShortCut(str(shortcut_start_menu_path.resolve()))
             if self.exec_arguments:
                 wscript.Arguments = self.exec_arguments
             wscript.Targetpath = str(self.exec_path.resolve())
             if self.work_dir is not None:
                 wscript.WorkingDirectory = str(self.work_dir.resolve())
             wscript.WindowStyle = 0
-            wscript.Description = self.description
+            if self.description:
+                wscript.Description = self.description
+            else:
+                wscript.Description = f"Created by {__title__} {__version__}"
             if self.icon_path is not None:
                 wscript.IconLocation = str(self.icon_path.resolve())
             wscript.save()
         else:
             shortcut_start_menu_path = None
 
         return (shortcut_desktop_path, shortcut_start_menu_path)
```

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/scenarios/scenario_reader.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/scenarios/scenario_reader.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/bouncer.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/bouncer.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/journalizer.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/journalizer.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/logger.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/logger.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/proxies.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/proxies.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt/utils/slugger.py` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt/utils/slugger.py`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/PKG-INFO` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qgis-deployment-toolbelt
-Version: 0.8.0
+Version: 0.9.0
 Summary: QGIS deployment toolbelt is a CLI (Command Line Interface) to perform redundant operations after a QGIS deployment.
 Home-page: https://github.com/Guts/qgis-deployment-cli/
 Author: Julien Moura (Oslandia)
 Author-email: qgis@oslandia.com
 Keywords: cli, QGIS, deployment, profiles
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
```

### Comparing `qgis-deployment-toolbelt-0.8.0/qgis_deployment_toolbelt.egg-info/SOURCES.txt` & `qgis-deployment-toolbelt-0.9.0/qgis_deployment_toolbelt.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -26,8 +26,10 @@
 qgis_deployment_toolbelt/scenarios/__init__.py
 qgis_deployment_toolbelt/scenarios/scenario_reader.py
 qgis_deployment_toolbelt/utils/__init__.py
 qgis_deployment_toolbelt/utils/bouncer.py
 qgis_deployment_toolbelt/utils/journalizer.py
 qgis_deployment_toolbelt/utils/logger.py
 qgis_deployment_toolbelt/utils/proxies.py
-qgis_deployment_toolbelt/utils/slugger.py
+qgis_deployment_toolbelt/utils/slugger.py
+qgis_deployment_toolbelt/utils/str2bool.py
+qgis_deployment_toolbelt/utils/win32utils.py
```

### Comparing `qgis-deployment-toolbelt-0.8.0/setup.cfg` & `qgis-deployment-toolbelt-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `qgis-deployment-toolbelt-0.8.0/setup.py` & `qgis-deployment-toolbelt-0.9.0/setup.py`

 * *Files identical despite different names*

