# Comparing `tmp/saltext.bitwarden-0.0.1b8.tar.gz` & `tmp/saltext.bitwarden-0.0.1b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.bitwarden-0.0.1b8.tar", last modified: Sat Jan 21 05:48:06 2023, max compression
+gzip compressed data, was "saltext.bitwarden-0.0.1b9.tar", last modified: Sun Jan 22 10:38:13 2023, max compression
```

## Comparing `saltext.bitwarden-0.0.1b8.tar` & `saltext.bitwarden-0.0.1b9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.351390 saltext.bitwarden-0.0.1b8/
--rw-r--r--   0 root         (0) root         (0)    11344 2023-01-07 23:35:43.000000 saltext.bitwarden-0.0.1b8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)    12015 2023-01-21 05:48:15.353387 saltext.bitwarden-0.0.1b8/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)    10729 2023-01-15 06:49:11.000000 saltext.bitwarden-0.0.1b8/README.md
--rwxr--r--   0 root         (0) root         (0)      169 2023-01-06 07:49:09.000000 saltext.bitwarden-0.0.1b8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)     1950 2023-01-21 05:48:15.365917 saltext.bitwarden-0.0.1b8/setup.cfg
--rwxr--r--   0 root         (0) root         (0)      547 2023-01-08 06:50:17.000000 saltext.bitwarden-0.0.1b8/setup.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:14.542950 saltext.bitwarden-0.0.1b8/src/
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:14.545957 saltext.bitwarden-0.0.1b8/src/saltext/
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:14.998793 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/
--rwxr--r--   0 root         (0) root         (0)      863 2023-01-04 22:56:05.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/__init__.py
--rwxr--r--   0 root         (0) root         (0)      801 2023-01-07 07:25:50.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/loader.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.054134 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/modules/
--rw-r--r--   0 root         (0) root         (0)     5694 2023-01-21 05:42:06.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/modules/bitwarden_mod.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.113585 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/runners/
--rw-r--r--   0 root         (0) root         (0)     5681 2023-01-21 05:41:45.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/runners/bitwarden_mod.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.170386 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/sdb/
--rw-rw-r--   0 root         (0) root         (0)     9727 2023-01-21 05:41:56.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/sdb/bitwarden_mod.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.232649 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/states/
--rw-rw-r--   0 root         (0) root         (0)     5942 2023-01-21 05:41:29.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/states/bitwarden_mod.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:15.295868 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/utils/
--rw-rw-r--   0 root         (0) root         (0)    21026 2023-01-21 05:25:08.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/utils/bitwarden_mod.py
--rw-rw-r--   0 root         (0) root         (0)       24 2023-01-21 05:44:07.000000 saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/version.py
-drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-21 05:48:14.881863 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/
--rwxr--r--   0 root         (0) root         (0)    12015 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/PKG-INFO
--rwxr--r--   0 root         (0) root         (0)      694 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/SOURCES.txt
--rwxr--r--   0 root         (0) root         (0)        1 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/dependency_links.txt
--rwxr--r--   0 root         (0) root         (0)       52 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/entry_points.txt
--rwxr--r--   0 root         (0) root         (0)        1 2023-01-04 23:17:02.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/not-zip-safe
--rwxr--r--   0 root         (0) root         (0)      353 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/requires.txt
--rwxr--r--   0 root         (0) root         (0)        8 2023-01-21 05:48:14.000000 saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/top_level.txt
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:22.175439 saltext.bitwarden-0.0.1b9/
+-rw-r--r--   0 root         (0) root         (0)    11344 2023-01-07 23:35:43.000000 saltext.bitwarden-0.0.1b9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)    12015 2023-01-22 10:38:22.176440 saltext.bitwarden-0.0.1b9/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)    10729 2023-01-15 06:49:11.000000 saltext.bitwarden-0.0.1b9/README.md
+-rwxr--r--   0 root         (0) root         (0)      169 2023-01-06 07:49:09.000000 saltext.bitwarden-0.0.1b9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-01-22 10:38:22.185443 saltext.bitwarden-0.0.1b9/setup.cfg
+-rwxr--r--   0 root         (0) root         (0)      547 2023-01-08 06:50:17.000000 saltext.bitwarden-0.0.1b9/setup.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.439686 saltext.bitwarden-0.0.1b9/src/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.442689 saltext.bitwarden-0.0.1b9/src/saltext/
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.908132 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/
+-rwxr--r--   0 root         (0) root         (0)      863 2023-01-04 22:56:05.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/__init__.py
+-rwxr--r--   0 root         (0) root         (0)      801 2023-01-07 07:25:50.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/loader.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.947911 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/modules/
+-rw-rw-r--   0 root         (0) root         (0)     9004 2023-01-22 10:10:25.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/modules/bitwarden_mod.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.991333 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/runners/
+-rw-rw-r--   0 root         (0) root         (0)     8989 2023-01-22 10:10:32.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/runners/bitwarden_mod.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:22.040096 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/sdb/
+-rw-rw-r--   0 root         (0) root         (0)     9727 2023-01-21 05:41:56.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/sdb/bitwarden_mod.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:22.086352 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/states/
+-rw-rw-r--   0 root         (0) root         (0)     5942 2023-01-21 05:41:29.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/states/bitwarden_mod.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:22.132900 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/utils/
+-rw-rw-r--   0 root         (0) root         (0)    31564 2023-01-22 10:17:01.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/utils/bitwarden_mod.py
+-rw-rw-r--   0 root         (0) root         (0)       24 2023-01-22 10:25:46.000000 saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/version.py
+drwxrwxr-x   0 root         (0) root         (0)        0 2023-01-22 10:38:21.781867 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/
+-rwxr--r--   0 root         (0) root         (0)    12015 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/PKG-INFO
+-rwxr--r--   0 root         (0) root         (0)      694 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/SOURCES.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/dependency_links.txt
+-rwxr--r--   0 root         (0) root         (0)       52 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/entry_points.txt
+-rwxr--r--   0 root         (0) root         (0)        1 2023-01-04 23:17:02.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/not-zip-safe
+-rwxr--r--   0 root         (0) root         (0)      353 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/requires.txt
+-rwxr--r--   0 root         (0) root         (0)        8 2023-01-22 10:38:21.000000 saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/top_level.txt
```

### Comparing `saltext.bitwarden-0.0.1b8/LICENSE` & `saltext.bitwarden-0.0.1b9/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/PKG-INFO` & `saltext.bitwarden-0.0.1b9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.bitwarden
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Salt Extension Modules for Bitwarden
 Home-page: https://gitlab.com/ggiesen/salt-ext-bitwarden
 Author: Gary T. Giesen
 Author-email: ggiesen@giesen.me
 License: Apache Software License
 Project-URL: Source, https://gitlab.com/ggiesen/salt-ext-bitwarden
 Project-URL: Tracker, https://gitlab.com/ggiesen/salt-ext-bitwarden/-/issues
```

### Comparing `saltext.bitwarden-0.0.1b8/README.md` & `saltext.bitwarden-0.0.1b9/README.md`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/setup.cfg` & `saltext.bitwarden-0.0.1b9/setup.cfg`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/setup.py` & `saltext.bitwarden-0.0.1b9/setup.py`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/__init__.py` & `saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/loader.py` & `saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/loader.py`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/modules/bitwarden_mod.py` & `saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/states/bitwarden_mod.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
-Bitwarden execution module
+Bitwarden state module
 
 This module allows access to a Bitwarden vault.
 
 :depends: pyhumps, validators
 
 This module requires the ``bw`` Bitwarden CLI utility to be installed.
 Installation instructions are available
 `here <https://bitwarden.com/help/cli/#download-and-install>`_.
 
 This module primarily relies on the `Bitwarden Vault Management API
 <https://bitwarden.com/help/vault-management-api/>`_ running locally on the minion
 using the ``bw serve`` feature of the Bitwarden CLI utility, as well as the
 `Bitwarden Public (Organization Management) API
 <https://bitwarden.com/help/api/>`_ for its functionality. A
-small number of functions also rely on executing the ``bw`` client directly
+small number of functions also rely on executing the `bw` client directly
 (mostly for login/logout since those methods are not exposed through any other
 API).
 
 .. warning::
     The Bitwarden Vault Management API running on the minion, once the vault is
     unlocked, has no authentication or other protection. All traffic is
     unencrypted. Any users who can access the HTTP server or observe traffic to
@@ -26,15 +26,15 @@
 
     Please ensure you take adequate measures to protect the HTTP server, such as
     ensuring it only binds to localhost, using firewall rules to limit access to
     the port to specific users (where possible), and limiting which users have
     access to any system on which it is running.
 
 This module also requires a configuration profile to be configured in either the
-minion configuration file.
+minion or master configuration file.
 
 Configuration example:
 
 .. code-block:: yaml
 
     my-bitwarden-vault:
       driver: bitwarden
@@ -47,22 +47,22 @@
       public_api_url: https://api.bitwarden.com
       client_id: user.25fa6fc6-deeb-4b42-a279-5e680b51aa58
       client_secret: AofieD0oexiex1mie3eigi9oojooF3
       org_client_id: organization.d0e19db4-38aa-4284-be3d-e80cff306e6c
       org_client_secret: aWMk2MBf4NWXfaevrKyxa3uqNXYVQy
 
 The ``driver`` refers to the Bitwarden module, and must be set to ``bitwarden``
-in order to use this driver.
+in order to use this module.
 
 Other configuration options:
 
 cli_path: ``None``
     The path to the bitwarden cli binary on the local system. If set to ``None``
     the module will use ``bw`` (Unix-like) or ``bw.exe`` (Windows) from the Salt
-    user's ``PATH``.
+    user's `PATH`.
 
 cli_conf_dir: ``None``
     The path specifying a folder where the Bitwarden CLI will store configuration
     data.
 
 vault_url: ``https://bitwarden.com``
     The URL for the Bitwarden vault.
@@ -94,20 +94,23 @@
 """
 import logging
 
 import saltext.bitwarden.utils.bitwarden_mod as utils
 
 log = logging.getLogger(__name__)
 
+# Prefix that is appended to all log entries
+LOG_PREFIX = "bitwarden:"
+
 __virtualname__ = "bitwarden"
 
 
 def __virtual__():
     # To force a module not to load return something like:
-    #   return (False, "The bitwarden execution module is not implemented yet")
+    #   return (False, "The bitwarden state module is not implemented yet")
     return __virtualname__
 
 
 def _get_config(profile=None):  # pylint: disable=C0116
     config = {}
     if profile:
         config = __salt__["config.get"](profile)
@@ -119,100 +122,64 @@
     if not config:
         log.debug("The config is not set")
         return {}
 
     return config
 
 
-def login(profile=None):
+def logged_in(name=None, use_cli=False, profile=None):
     """
-    Login to Bitwarden vault
-
-    profile
-        Profile to use (optional)
-
-    CLI Example:
-
-    .. code-block:: bash
+    Ensure the vault is logged in.
 
-        salt '*' bitwarden.login
-
-    Returns ``True`` if successful or a dictionary containing an error if unsuccessful
-    """
-    opts = _get_config(profile=profile)
-    return utils.login(opts=opts)
-
-
-def logout(profile=None):
-    """
-    Logout of Bitwarden vault
+    name
+        Placeholder name, not used (string)
 
-    profile
-        Profile to use (optional)
-
-    CLI Example:
-
-    .. code-block:: bash
-
-        salt '*' bitwarden.logout
-
-    Returns ``True`` if successful or ``False`` if unsuccessful
-    """
-    opts = _get_config(profile=profile)
-    return utils.logout(opts=opts)
-
-
-def lock(profile=None):
-    """
-    Lock the Bitwarden vault
+    use_cli
+        Use CLI to get status instead of REST API (boolean)
 
     profile
         Profile to use (optional)
 
     CLI Example:
 
-    .. code-block:: bash
+    .. code-block:: yaml
 
-        salt '*' bitwarden.lock
+        Login to Bitwarden vault:
+          bitwarden.logged_in:
+            - name: logged_in
+            - use_cli: True
 
-    Returns ``True`` if successful or ``False`` if unsuccessful
     """
     opts = _get_config(profile=profile)
-    return utils.lock(opts=opts)
+    if name and not isinstance(name, str):
+        log.error('%s Value for "name" must be a string.', LOG_PREFIX)
+        return {"Error": 'Value for "name" must be a string.'}
+    if not isinstance(use_cli, bool):
+        log.error('%s Value for "use_cli" must be a boolean.', LOG_PREFIX)
+        return {"Error": 'Value for "use_cli" must be a boolean.'}
 
+    if use_cli:
+        status = utils.get_status_cli(opts)
+    else:
+        status = utils.get_status(opts)
 
-def unlock(profile=None):
-    """
-    Unlock the Bitwarden vault
-
-    profile
-        Profile to use (optional)
-
-    CLI Example:
-
-    .. code-block:: bash
-
-        salt '*' bitwarden.unlock
-
-    Returns ``True`` if successful or ``False`` if unsuccessful
-    """
-    opts = _get_config(profile=profile)
-    return utils.unlock(opts=opts)
-
-
-def sync(profile=None):
-    """
-    Sync Bitwarden vault
-
-    profile
-        Profile to use (optional)
-
-    CLI Example:
-
-    .. code-block:: bash
-
-        salt '*' bitwarden.sync
+    ret = {"name": name, "changes": {}, "result": False, "comment": ""}
+    if status.get("status"):
+        if status["status"] not in ["locked", "unlocked"]:
+            log.debug("%s not logged in.", LOG_PREFIX)
+            if utils.login(opts):
+                ret["result"] = True
+                ret["changes"]["old"] = status["status"]
+                if use_cli:
+                    ret["changes"]["new"] = utils.get_status_cli(opts)["status"]
+                else:
+                    ret["changes"]["new"] = utils.get_status(opts)["status"]
+                ret["comment"] = "bitwarden logged in succesfully."
+            else:
+                ret["result"] = False
+                ret["comment"] = "bitwarden unable to log in."
+        else:
+            log.debug("%s already logged in.", LOG_PREFIX)
+            ret["result"] = True
+            ret["comment"] = "bitwarden already logged in."
 
-    Returns ``True`` if successful or ``False`` if unsuccessful
-    """
-    opts = _get_config(profile=profile)
-    return utils.sync(opts=opts)
+    return ret
```

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/sdb/bitwarden_mod.py` & `saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/sdb/bitwarden_mod.py`

 * *Files identical despite different names*

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext/bitwarden/utils/bitwarden_mod.py` & `saltext.bitwarden-0.0.1b9/src/saltext/bitwarden/utils/bitwarden_mod.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Bitwarden util module
 """
 import json
 import logging
 import os
 import subprocess
+import urllib.parse
 
 import humps
 import pyotp
 import salt.utils.files
 import salt.utils.http
 import salt.utils.url
 import validators
@@ -556,14 +557,326 @@
 
     if result["success"]:
         return humps.decamelize(result["data"]["template"])
 
     return False
 
 
+def generate_password(
+    opts=None, uppercase=None, lowercase=None, numeric=None, special=None, length=None
+):
+    """
+    Generate a passphrase
+
+    opts
+        Dictionary containing the following keys:
+
+        vault_api_url: ``http://localhost:8087``
+            The URL for the Bitwarden Vault Management API.
+
+    uppercase
+        Include uppercase characters in the password (boolean)
+
+    lowercase
+        Include lowercase characters in the password (boolean)
+
+    numeric
+        Include numbers in the password (boolean)
+
+    special
+        Include special characters in the password (boolean)
+
+    length
+        Number of characters in the password (integer >= 5)
+
+    Returns a string containing the generated password if successful or ``False`` if unsuccessful
+    """
+    config = _validate_opts(opts=opts, opts_list=["vault_api_url"])
+    if not config:
+        log.error("%s Invalid configuration supplied", LOG_PREFIX)
+        return {"Error": "Invalid configuration supplied"}
+    elif config.get("Error"):
+        log.error("%s %s", LOG_PREFIX, config["Error"])
+        return {"Error": config["Error"]}
+    params = {}
+    if uppercase is not None:
+        if not isinstance(uppercase, bool):
+            log.error('%s Value for "uppercase" must be a boolean.', LOG_PREFIX)
+            return False
+        elif uppercase:
+            params["uppercase"] = "true"
+    if lowercase is not None:
+        if not isinstance(lowercase, bool):
+            log.error('%s Value for "lowercase" must be a boolean.', LOG_PREFIX)
+            return False
+        elif lowercase:
+            params["lowercase"] = "true"
+    if numeric is not None:
+        if not isinstance(numeric, bool):
+            log.error('%s Value for "numeric" must be a boolean.', LOG_PREFIX)
+            return False
+        elif numeric:
+            params["number"] = "true"
+    if special is not None:
+        if not isinstance(special, bool):
+            log.error('%s Value for "special" must be a boolean.', LOG_PREFIX)
+            return False
+        elif special:
+            params["special"] = "true"
+    if length is not None:
+        if not isinstance(length, int):
+            log.error('%s Value for "length" must be an integer.', LOG_PREFIX)
+            return False
+        elif length:
+            params["length"] = str(length)
+        if length < 5:
+            log.error("%s Password length must be at least 5 characters.", LOG_PREFIX)
+            return False
+    if params:
+        params = urllib.parse.urlencode(params)
+        params = "?" + params
+    else:
+        params = ""
+    headers = _get_headers()
+    vault_api_url = config["vault_api_url"]
+    generate_url = f"{vault_api_url}/generate{params}"
+    generate_results = {}
+    generate_ret = salt.utils.http.query(
+        generate_url, method="GET", header_dict=headers, decode=True
+    )
+    # Check status code for API call
+    if "error" in generate_ret:
+        log.error(
+            '%s API query failed for "generate_password", status code: %s, error %s',
+            LOG_PREFIX,
+            generate_ret["status"],
+            generate_ret["error"],
+        )
+        return False
+    else:
+        generate_results = json.loads(generate_ret["body"])
+        if generate_results.get("success"):
+            return generate_results["data"]["data"]
+
+    return False
+
+
+def generate_passphrase(
+    opts=None, words=None, separator=None, capitalize=None, number=None
+):  # pylint: disable=C0116
+    """
+    Generate a passphrase
+
+    opts
+        Dictionary containing the following keys:
+
+        vault_api_url: ``http://localhost:8087``
+            The URL for the Bitwarden Vault Management API.
+
+    words
+        Number of words in the passphrase (integer >= 3)
+
+    separator
+        Separator character in the passphrase
+
+    capitalize
+        Title-case the passphrase (boolean)
+
+    number
+        Include numbers in the passphrase (boolean)
+
+    Returns a string containing the generated passphrase if successful or ``False`` if unsuccessful
+    """
+    config = _validate_opts(opts=opts, opts_list=["vault_api_url"])
+    if not config:
+        log.error("%s Invalid configuration supplied", LOG_PREFIX)
+        return {"Error": "Invalid configuration supplied"}
+    elif config.get("Error"):
+        log.error("%s %s", LOG_PREFIX, config["Error"])
+        return {"Error": config["Error"]}
+    params = {"passphrase": "true"}
+    if words is not None:
+        if not isinstance(words, int):
+            log.error('%s Value for "words" must be an integer.', LOG_PREFIX)
+            return False
+        else:
+            params["words"] = str(words)
+        if words < 3:
+            log.error("%s Passphrase length must be at least 3 words.", LOG_PREFIX)
+            return False
+    if separator is not None:
+        if not isinstance(separator, str):
+            log.error('%s Value for "separator" must be a string.', LOG_PREFIX)
+            return False
+        else:
+            params["separator"] = separator
+        if len(separator) != 1:
+            log.error("%s Separator must be a single character.", LOG_PREFIX)
+            return False
+    if capitalize is not None:
+        if not isinstance(capitalize, bool):
+            log.error('%s Value for "capitalize" must be a boolean.', LOG_PREFIX)
+            return False
+        elif capitalize:
+            params["capitalize"] = "true"
+    if number is not None:
+        if not isinstance(number, bool):
+            log.error('%s Value for "number" must be a boolean.', LOG_PREFIX)
+            return False
+        elif number:
+            params["includeNumber"] = "true"
+    if params:
+        params = urllib.parse.urlencode(params)
+        params = "?" + params
+    else:
+        params = ""
+    headers = _get_headers()
+    vault_api_url = config["vault_api_url"]
+    generate_url = f"{vault_api_url}/generate{params}"
+    generate_results = {}
+    generate_ret = salt.utils.http.query(
+        generate_url, method="GET", header_dict=headers, decode=True
+    )
+    # Check status code for API call
+    if "error" in generate_ret:
+        log.error(
+            '%s API query failed for "generate_passphrase", status code: %s, error %s',
+            LOG_PREFIX,
+            generate_ret["status"],
+            generate_ret["error"],
+        )
+        return False
+    else:
+        generate_results = json.loads(generate_ret["body"])
+        if generate_results.get("success"):
+            return generate_results["data"]["data"]
+
+    return False
+
+
+def get_template(opts=None, template_type=None):  # pylint: disable=C0116
+    """
+    Get a template
+
+    opts
+        Dictionary containing the following keys:
+
+        vault_api_url: ``http://localhost:8087``
+            The URL for the Bitwarden Vault Management API.
+
+    template_type
+        Type of template to retrieve. (One of: "item", "item.field", "item.login.url", "item.card",
+        item.identity", item.securenote, "folder", "collection", "item-collections", "org-collection")
+
+    profile
+        Profile to use (optional)
+
+    Returns a dictionary containing the template if successful or ``False`` if unsuccessful
+    """
+    config = _validate_opts(opts=opts, opts_list=["vault_api_url"])
+    if not config:
+        log.error("%s Invalid configuration supplied", LOG_PREFIX)
+        return {"Error": "Invalid configuration supplied"}
+    elif config.get("Error"):
+        log.error("%s %s", LOG_PREFIX, config["Error"])
+        return {"Error": config["Error"]}
+    if template_type not in (
+        "item",
+        "item.field",
+        "item.login.url",
+        "item.card",
+        "item.identity",
+        "item.securenote",
+        "folder",
+        "collection",
+        "item-collections",
+        "org-collection",
+    ):
+        log.error(
+            '%s Value for "template_type" must be one of:  %s, %s, %s, %s, %s, %s, %s, %s, %s, %s.',
+            LOG_PREFIX,
+            "item",
+            "item.field",
+            "item.login.url",
+            "item.card",
+            "item.identity",
+            "item.securenote",
+            "folder",
+            "collection",
+            "item-collections",
+            "org-collection",
+        )
+        return False
+    headers = _get_headers()
+    vault_api_url = config["vault_api_url"]
+    template_url = f"{vault_api_url}/object/template/{template_type}"
+    template_results = {}
+    template_ret = salt.utils.http.query(
+        template_url, method="GET", header_dict=headers, decode=True
+    )
+    # Check status code for API call
+    if "error" in template_ret:
+        log.error(
+            '%s API query failed for "get_template", status code: %s, error %s',
+            LOG_PREFIX,
+            template_ret["status"],
+            template_ret["error"],
+        )
+        return False
+    else:
+        template_results = json.loads(template_ret["body"])
+        if template_results.get("success"):
+            return humps.decamelize(template_results["data"]["template"])
+
+    return False
+
+
+def get_fingerprint(opts=None):  # pylint: disable=C0116
+    """
+    Display user fingerprint
+
+    opts
+        Dictionary containing the following keys:
+
+        vault_api_url: ``http://localhost:8087``
+            The URL for the Bitwarden Vault Management API.
+
+    Returns a string containing the fingerprint if successful or ``False`` if unsuccessful
+    """
+    config = _validate_opts(opts=opts, opts_list=["vault_api_url"])
+    if not config:
+        log.error("%s Invalid configuration supplied", LOG_PREFIX)
+        return {"Error": "Invalid configuration supplied"}
+    elif config.get("Error"):
+        log.error("%s %s", LOG_PREFIX, config["Error"])
+        return {"Error": config["Error"]}
+    headers = _get_headers()
+    vault_api_url = config["vault_api_url"]
+    fingerprint_url = f"{vault_api_url}/object/fingerprint/me"
+    fingerprint_results = {}
+    fingerprint_ret = salt.utils.http.query(
+        fingerprint_url, method="GET", header_dict=headers, decode=True
+    )
+    # Check status code for API call
+    if "error" in fingerprint_ret:
+        log.error(
+            '%s API query failed for "get_fingerprint", status code: %s, error %s',
+            LOG_PREFIX,
+            fingerprint_ret["status"],
+            fingerprint_ret["error"],
+        )
+        return False
+    else:
+        fingerprint_results = json.loads(fingerprint_ret["body"])
+        if fingerprint_results.get("success"):
+            return humps.decamelize(fingerprint_results["data"]["data"])
+
+    return False
+
+
 def get_totp(seed=None):
     """
     Get the current TOTP value
 
     seed
         TOTP seed
```

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/PKG-INFO` & `saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saltext.bitwarden
-Version: 0.0.1b8
+Version: 0.0.1b9
 Summary: Salt Extension Modules for Bitwarden
 Home-page: https://gitlab.com/ggiesen/salt-ext-bitwarden
 Author: Gary T. Giesen
 Author-email: ggiesen@giesen.me
 License: Apache Software License
 Project-URL: Source, https://gitlab.com/ggiesen/salt-ext-bitwarden
 Project-URL: Tracker, https://gitlab.com/ggiesen/salt-ext-bitwarden/-/issues
```

### Comparing `saltext.bitwarden-0.0.1b8/src/saltext.bitwarden.egg-info/SOURCES.txt` & `saltext.bitwarden-0.0.1b9/src/saltext.bitwarden.egg-info/SOURCES.txt`

 * *Files identical despite different names*

