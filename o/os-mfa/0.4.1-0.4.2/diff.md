# Comparing `tmp/os-mfa-0.4.1.tar.gz` & `tmp/os-mfa-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-mfa-0.4.1.tar", last modified: Sat May  6 02:16:26 2023, max compression
+gzip compressed data, was "os-mfa-0.4.2.tar", last modified: Sun May  7 05:33:33 2023, max compression
```

## Comparing `os-mfa-0.4.1.tar` & `os-mfa-0.4.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-06 02:16:26.311039 os-mfa-0.4.1/
--rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.4.1/LICENSE
--rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-06 02:16:26.311039 os-mfa-0.4.1/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)     7225 2023-05-05 09:49:25.000000 os-mfa-0.4.1/README.md
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-06 02:16:26.311039 os-mfa-0.4.1/os_mfa/
--rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-05-06 02:15:41.000000 os-mfa-0.4.1/os_mfa/__init__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1918 2023-05-05 09:49:25.000000 os-mfa-0.4.1/os_mfa/__main__.py
--rw-r--r--   0 simon     (1000) simon     (1000)     4954 2023-05-06 02:03:12.000000 os-mfa-0.4.1/os_mfa/clouds_configs.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1576 2023-05-06 02:06:52.000000 os-mfa-0.4.1/os_mfa/tokens.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-06 02:16:26.311039 os-mfa-0.4.1/os_mfa.egg-info/
--rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/PKG-INFO
--rw-r--r--   0 simon     (1000) simon     (1000)      375 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/SOURCES.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/dependency_links.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/entry_points.txt
--rw-r--r--   0 simon     (1000) simon     (1000)       80 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/requires.txt
--rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-05-06 02:16:26.000000 os-mfa-0.4.1/os_mfa.egg-info/top_level.txt
--rw-r--r--   0 simon     (1000) simon     (1000)     1215 2023-05-06 02:15:41.000000 os-mfa-0.4.1/pyproject.toml
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-06 02:16:26.311039 os-mfa-0.4.1/setup.cfg
--rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-01 08:59:46.000000 os-mfa-0.4.1/setup.py
-drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-06 02:16:26.311039 os-mfa-0.4.1/tests/
--rw-r--r--   0 simon     (1000) simon     (1000)     1107 2023-05-05 09:49:25.000000 os-mfa-0.4.1/tests/test_create_long_term_config.py
--rw-r--r--   0 simon     (1000) simon     (1000)     1221 2023-05-05 09:49:25.000000 os-mfa-0.4.1/tests/test_create_token_config.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-07 05:33:33.670021 os-mfa-0.4.2/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1060 2023-04-30 09:59:27.000000 os-mfa-0.4.2/LICENSE
+-rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-07 05:33:33.670021 os-mfa-0.4.2/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)     7225 2023-05-05 09:49:25.000000 os-mfa-0.4.2/README.md
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-07 05:33:33.670021 os-mfa-0.4.2/os_mfa/
+-rw-r--r--   0 simon     (1000) simon     (1000)       22 2023-05-07 05:32:09.000000 os-mfa-0.4.2/os_mfa/__init__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1992 2023-05-07 05:28:47.000000 os-mfa-0.4.2/os_mfa/__main__.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     5143 2023-05-07 05:27:08.000000 os-mfa-0.4.2/os_mfa/clouds_configs.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1576 2023-05-07 03:18:49.000000 os-mfa-0.4.2/os_mfa/tokens.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-07 05:33:33.670021 os-mfa-0.4.2/os_mfa.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     7763 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/PKG-INFO
+-rw-r--r--   0 simon     (1000) simon     (1000)      375 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/SOURCES.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        1 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/dependency_links.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       48 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/entry_points.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)       80 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/requires.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)        7 2023-05-07 05:33:33.000000 os-mfa-0.4.2/os_mfa.egg-info/top_level.txt
+-rw-r--r--   0 simon     (1000) simon     (1000)     1215 2023-05-07 05:32:09.000000 os-mfa-0.4.2/pyproject.toml
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-07 05:33:33.670021 os-mfa-0.4.2/setup.cfg
+-rw-r--r--   0 simon     (1000) simon     (1000)       38 2023-05-01 08:59:46.000000 os-mfa-0.4.2/setup.py
+drwxr-xr-x   0 simon     (1000) simon     (1000)        0 2023-05-07 05:33:33.670021 os-mfa-0.4.2/tests/
+-rw-r--r--   0 simon     (1000) simon     (1000)     1107 2023-05-05 09:49:25.000000 os-mfa-0.4.2/tests/test_create_long_term_config.py
+-rw-r--r--   0 simon     (1000) simon     (1000)     1221 2023-05-05 09:49:25.000000 os-mfa-0.4.2/tests/test_create_token_config.py
```

### Comparing `os-mfa-0.4.1/LICENSE` & `os-mfa-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os-mfa-0.4.1/PKG-INFO` & `os-mfa-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os-mfa
-Version: 0.4.1
+Version: 0.4.2
 Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
 Author-email: Simon Merrick <s.m3rrick@gmail.com>
 Project-URL: Homepage, https://github.com/iokiwi/os-mfa
 Keywords: openstack,mfa,auth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `os-mfa-0.4.1/README.md` & `os-mfa-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `os-mfa-0.4.1/os_mfa/__main__.py` & `os-mfa-0.4.2/os_mfa/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,17 @@
 
     # Create a long-term config if it doesn't exist
     if not manager.config_exists(long_term_config_name):
         print("Creating config: {}".format(long_term_config_name))
         default_config = manager.get_config_by_name(os_cloud)
         long_term_config = create_long_term_config(default_config)
         manager.put_config_by_name(long_term_config_name, long_term_config)
+    else:
+        # TODO: Check if current token is expired,
+        pass
 
     # Create token based config from long term config
     long_term_config = manager.get_config_by_name(long_term_config_name)
     token_config = get_token_config(long_term_config)
     print("The '{}' config has been updated.".format(os_cloud))
     manager.put_config_by_name(os_cloud, token_config)
```

### Comparing `os-mfa-0.4.1/os_mfa/clouds_configs.py` & `os-mfa-0.4.2/os_mfa/clouds_configs.py`

 * *Files 9% similar despite different names*

```diff
@@ -81,19 +81,19 @@
 
     if "auth_type" in contents:
         del contents["auth_type"]
 
     if "token" in contents["auth"]:
         del contents["auth"]["token"]
 
-    if "password" in config["auth"]:
-        PASSWORD = config["auth"]["password"]
-        del config["auth"]["password"]
+    if "password" in contents["auth"]:
+        PASSWORD = contents["auth"]["password"]
+        del contents["auth"]["password"]
 
-    return config
+    return contents
 
 
 def create_token_config(long_term_config: dict, token: str) -> dict:
     token_config = copy.deepcopy(long_term_config)
 
     token_config["auth_type"] = "token"
     token_config["auth"]["token"] = token
@@ -101,62 +101,68 @@
     for k in ["username", "password", "user_domain_name"]:
         if k in token_config["auth"]:
             del token_config["auth"][k]
 
     return token_config
 
 
-# TODO: This method has gotten really unweildy
-def get_token_config(config: dict) -> dict:
+def prompt_username(config) -> str:
+    print(
+        "Please enter your username for project '{}'".format(
+            config["auth"]["project_name"]
+        )
+    )
+    username = input("Username: ").strip()
+    config["auth"]["username"] = username
+    print(
+        "Specify a value for auth.username in the long-term configuration to suppress this prompt in the future."
+    )
+
+
+def prompt_user_domain_name(config) -> str:
+    print(
+        "Please provide a user_domain_name for user '{}' in project '{}' or press enter to accept the default.".format(
+            config["auth"].get("username"), config["auth"].get("project_name")
+        )
+    )
+    user_domain_name = input('User Domain Name ["Default"]: ').strip()
+    if user_domain_name == "":
+        print('Using default value for user_domain_name: "Default"')
+        user_domain_name = "Default"
+    print(
+        "Specify a value for auth.user_domain_name in the long-term configuration to suppress this prompt in the future."
+    )
+    return user_domain_name
+
+def prompt_password(config, password=PASSWORD):
+    print(
+        "Authenticating '{}' in project '{}'".format(
+            config["auth"]["username"], config["auth"]["project_name"]
+        )
+    )
+    return getpass(f"Enter Password: ")
+
+# TODO: This method has gotten really unwieldy
+def get_token_config(config: dict, password=PASSWORD) -> dict:
     """takes a long-term-config and generates a token based config"""
 
     config = copy.deepcopy(config)
 
     username = config["auth"].get("username")
     if username is None:
-        print(
-            "Please enter your username for project '{}'".format(
-                config["auth"]["project_name"]
-            )
-        )
-        username = input("Username: ").strip()
-        config["auth"]["username"] = username
-        print(
-            "Specify a value for auth.username in the long-term configuration to suppress this prompt in the future."
-        )
+        username = prompt_username(config)
+    config["auth"]["username"] = username
 
     user_domain_name = config["auth"].get("user_domain_name")
     if user_domain_name is None:
-        print(
-            "Please provide a user_domain_name for user '{}' in project '{}' or press enter to accept the default.".format(
-                username, config["auth"].get("project_name")
-            )
-        )
-        user_domain_name = input('User Domain Name ["Default"]: ').strip()
-
-        if user_domain_name == "":
-            print('Using default value for user_domain_name: "Default"')
-            user_domain_name = "Default"
-
+        user_domain_name = prompt_user_domain_name(config)
         config["auth"]["user_domain_name"] = user_domain_name
-        print(
-            "Specify a value for auth.user_domain_name in the long-term configuration to suppress this prompt in the future."
-        )
-
-    print(
-        "Authenticating '{}' in project '{}'".format(
-            username, config["auth"]["project_name"]
-        )
-    )
 
-    # Prompt for password unless we already have it from converting to long-term config
-    if PASSWORD is None:
-        password = getpass(f"Enter Password: ")
-    else:
-        password = PASSWORD
+    if password is None:
+        password = prompt_password(config)
 
     totp = input("MFA Code (Press enter to skip): ").strip()
     password = password + totp
 
     print("Getting token...")
     token = get_token(config["auth"], password)
```

### Comparing `os-mfa-0.4.1/os_mfa/tokens.py` & `os-mfa-0.4.2/os_mfa/tokens.py`

 * *Files identical despite different names*

### Comparing `os-mfa-0.4.1/os_mfa.egg-info/PKG-INFO` & `os-mfa-0.4.2/os_mfa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: os-mfa
-Version: 0.4.1
+Version: 0.4.2
 Summary: A minimal utility for managing cli authentication with openstack more securely and conveniently
 Author-email: Simon Merrick <s.m3rrick@gmail.com>
 Project-URL: Homepage, https://github.com/iokiwi/os-mfa
 Keywords: openstack,mfa,auth
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `os-mfa-0.4.1/pyproject.toml` & `os-mfa-0.4.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "os-mfa"
-version = "0.4.1"
+version = "0.4.2"
 description = "A minimal utility for managing cli authentication with openstack more securely and conveniently"
 readme = "README.md"
 authors = [{ name = "Simon Merrick", email = "s.m3rrick@gmail.com" }]
 # license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -28,15 +28,15 @@
 [project.urls]
 Homepage = "https://github.com/iokiwi/os-mfa"
 
 [project.scripts]
 os-mfa = "os_mfa.__main__:main"
 
 [tool.bumpver]
-current_version = "0.4.1"
+current_version = "0.4.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `os-mfa-0.4.1/tests/test_create_long_term_config.py` & `os-mfa-0.4.2/tests/test_create_long_term_config.py`

 * *Files identical despite different names*

### Comparing `os-mfa-0.4.1/tests/test_create_token_config.py` & `os-mfa-0.4.2/tests/test_create_token_config.py`

 * *Files identical despite different names*

