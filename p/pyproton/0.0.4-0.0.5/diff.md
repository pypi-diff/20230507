# Comparing `tmp/pyproton-0.0.4.tar.gz` & `tmp/pyproton-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproton-0.0.4.tar", last modified: Sat May  6 08:22:52 2023, max compression
+gzip compressed data, was "pyproton-0.0.5.tar", last modified: Sun May  7 07:05:00 2023, max compression
```

## Comparing `pyproton-0.0.4.tar` & `pyproton-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.533567 pyproton-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 08:22:35.000000 pyproton-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-06 08:22:52.533567 pyproton-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-06 08:22:35.000000 pyproton-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.529567 pyproton-0.0.4/pyproton/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-06 08:22:35.000000 pyproton-0.0.4/pyproton/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 08:22:52.533567 pyproton-0.0.4/pyproton.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 08:22:52.000000 pyproton-0.0.4/pyproton.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 08:22:52.533567 pyproton-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-06 08:22:35.000000 pyproton-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:05:00.667771 pyproton-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 07:04:37.000000 pyproton-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-07 07:05:00.667771 pyproton-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-07 07:04:37.000000 pyproton-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-07 07:04:37.000000 pyproton-0.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:05:00.667771 pyproton-0.0.5/pyproton/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-07 07:04:37.000000 pyproton-0.0.5/pyproton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6669 2023-05-07 07:04:37.000000 pyproton-0.0.5/pyproton/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 07:05:00.667771 pyproton-0.0.5/pyproton.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-07 07:05:00.000000 pyproton-0.0.5/pyproton.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-07 07:05:00.000000 pyproton-0.0.5/pyproton.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 07:05:00.000000 pyproton-0.0.5/pyproton.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 07:05:00.000000 pyproton-0.0.5/pyproton.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 07:05:00.671771 pyproton-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-07 07:04:37.000000 pyproton-0.0.5/setup.py
```

### Comparing `pyproton-0.0.4/LICENSE` & `pyproton-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproton-0.0.4/PKG-INFO` & `pyproton-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.4
+Version: 0.0.5
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,18 @@
 
 [![PyPI version](https://badge.fury.io/py/pyproton.svg)](https://badge.fury.io/py/pyproton)
 
 This package is a lightweight minimal wrapper implementation of the linux protonvpn-cli; designed to be an intuitive and simple to use interface for the Proton VPN in python.
 
 ## Getting Started
 
+**Version compatibility:**
+
+`Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)`
+
 ### **Install the CLI:**
 
 [Proton VPN Docs](https://protonvpn.com/support/linux-vpn-tool/)
 
 Debian based distros
 1. [Download the Proton VPN DEB package](https://repo.protonvpn.com/debian/dists/stable/main/binary-all/protonvpn-stable-release_1.0.3_all.deb)
 2. Install the Proton VPN repository
@@ -44,16 +48,16 @@
 ### **Import and use pyproton VPN:**
 
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
-* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
-* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `retries` **optional:** (`default=3`) defines number of retries when a VPN connection attempt times out.
+* `timeout` **optional:** (`default=5`) seconds to wait before timing out a login attempt.
 * `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
@@ -75,11 +79,12 @@
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
 
+* Improve reliability
 * PyTest & Tox testing
 * Sphynx docs
 * Coverage
 * Deepsource scanning
```

### Comparing `pyproton-0.0.4/README.md` & `pyproton-0.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 [![PyPI version](https://badge.fury.io/py/pyproton.svg)](https://badge.fury.io/py/pyproton)
 
 This package is a lightweight minimal wrapper implementation of the linux protonvpn-cli; designed to be an intuitive and simple to use interface for the Proton VPN in python.
 
 ## Getting Started
 
+**Version compatibility:**
+
+`Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)`
+
 ### **Install the CLI:**
 
 [Proton VPN Docs](https://protonvpn.com/support/linux-vpn-tool/)
 
 Debian based distros
 1. [Download the Proton VPN DEB package](https://repo.protonvpn.com/debian/dists/stable/main/binary-all/protonvpn-stable-release_1.0.3_all.deb)
 2. Install the Proton VPN repository
@@ -29,16 +33,16 @@
 ### **Import and use pyproton VPN:**
 
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
-* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
-* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `retries` **optional:** (`default=3`) defines number of retries when a VPN connection attempt times out.
+* `timeout` **optional:** (`default=5`) seconds to wait before timing out a login attempt.
 * `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
@@ -60,11 +64,12 @@
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
 
+* Improve reliability
 * PyTest & Tox testing
 * Sphynx docs
 * Coverage
 * Deepsource scanning
```

### Comparing `pyproton-0.0.4/pyproton/vpn.py` & `pyproton-0.0.5/pyproton/vpn.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,68 +1,66 @@
 import sys
 import random
-import time
 import pexpect
 
 class VPNException(Exception):
     '''exception class for VPN wrapper'''
     def __init__(self, message, status_code):
         self.message = message
         self.status_code = status_code
         super().__init__(f"[{status_code}] - {message}")
 
 
 class VPN():
     '''
     Wrapper for the linux protonvpn-cli
-    
-    Proton version compatibility:
-    Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)
     '''
 
-    def __init__(self, user, pw, verbose=False, retries=3, timeout=20, location='U'):
+    def __init__(self, user, pw, verbose=False, retries=3, timeout=5, location='U'):
         self.user = user
         self.pw = pw
         self.logged_in = False
         self.active = False
         self.verbose = verbose
         self.retries = retries
         self.timeout = timeout
-        if location in ['J','N','U']:
+        if location in ['J', 'N', 'U']:
             self.location = location
         else:
             raise VPNException(f'invalid location {location}', 400)
 
     def login(self):
         '''logs the user into proton vpn'''
+        command = f'protonvpn-cli login {self.user}'
         try:
-            child = pexpect.spawn(f'protonvpn-cli login {self.user}')
+            child = pexpect.spawn(command)
             index = child.expect(['Enter your Proton VPN password:', 'You are already logged in.'], timeout=5)
             if index == 0:
+                child.waitnoecho()
                 child.sendline(self.pw)
-                index = child.expect(['Successful login', 'Incorrect login credentials', 'error occured'], timeout=self.timeout)
-                if index == 0:
+                index = child.expect(['Successful login', ' \r\n', 'Incorrect login credentials', 'error occured'], timeout=self.timeout)
+                if index == 0 or index == 1:
                     child.expect(pexpect.EOF)
                     if self.verbose:
                         sys.stdout.write('successfully logged in\n')
                     self.logged_in = True
                     return
-                elif index == 1:
+                elif index == 2:
                     raise VPNException("invalid credentials", 401)
                 else:
                     raise VPNException("error logging in", 401)
             elif index == 1:
                 try:
                     raise VPNException("already logged in", 409)
                 except VPNException as e:
                     if self.verbose:
                         sys.stderr.write('already logged in skipping step...\n')
                     self.logged_in = True
                     return
-                
+
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
 
     def logout(self):
         '''logs the user out of proton vpn'''
         try:
             child = pexpect.spawn('protonvpn-cli logout')
@@ -83,64 +81,64 @@
                         sys.stdout.write('successfully logged out\n')
                     self.logged_in = False
                     return
                 else:
                     raise VPNException("error logging out", 500)
             else:
                 raise VPNException("error logging out", 500)
-        
+
         except pexpect.ExceptionPexpect as e:
             raise VPNException(str(e), 500)
-
+        
     def connect(self):
         '''
         connects to a random US Proton VPN
-
-        NOTE: less than 1 second sleep intervals resulted in frequent incomplete connections
         '''
         for retry in range(self.retries):
             try:
-                time.sleep(0.1)
                 child = pexpect.spawn('protonvpn-cli c')
-                time.sleep(1)
-                child.sendline(self.location) # select location
-                time.sleep(1)
+                child.waitnoecho(timeout=self.timeout//3)
+                child.sendline(self.location)  # select location
+
+                child.waitnoecho(timeout=self.timeout//3)
                 # randomly select VPN connection
                 for _ in range(random.randint(0, 30)):
                     child.send('+')
-                child.sendline('+') # + 1 and enter VPN selection
-                time.sleep(1)
-                child.sendline('u') # select updb - better speed
-                time.sleep(1)
-                index = child.expect(['Successfully connected'], timeout=10)
+                child.sendline('+')  # + 1 and enter VPN selection
+
+                child.waitnoecho(timeout=self.timeout//3)
+                child.sendline('u')  # select updb - better speed
+
+                index = child.expect(['Successfully connected'], timeout=5)
                 if index == 0:
                     output = child.before.decode().strip().splitlines()[-1]
                     child.expect(pexpect.EOF)
                     if self.verbose:
                         sys.stdout.write(output)
                         sys.stdout.write('\nsuccessfully connected\n')
                     self.active = True
                     return
                 else:
+                    self.logout()
                     raise VPNException('error connecting to vpn', 500)
 
             except pexpect.ExceptionPexpect as e:
-                if retry == self.retries-1:
-                    raise VPNException('maximum retries reached while connecting to VPN', 500)
+                if retry == self.retries - 1:
+                    sys.stderr.write(f'maximum retries reached while connecting to VPN; stopping connection attempt... ({retry + 1}/{self.retries})\n')
+                    return
                 else:
-                    time.sleep(3)
                     if self.verbose:
-                        sys.stderr.write(f'error while connecting to VPN; retrying connection... {retry}\n')
+                        sys.stderr.write(f'error while connecting to VPN; retrying connection... ({retry + 1}/{self.retries})\n')
                     continue
 
     def disconnect(self):
         '''disconnects from VPN connection'''
         try:
             child = pexpect.spawn('protonvpn-cli d')
-            index = child.expect(['Successfully disconnected','No Proton VPN connection was found'], timeout=5)
+            index = child.expect(['Successfully disconnected', 'No Proton VPN connection was found'], timeout=5)
             if index == 0:
                 child.expect(pexpect.EOF)
                 if self.verbose:
                     sys.stdout.write('successfully disconnected\n')
                 self.active = False
             elif index == 1:
                 child.expect(pexpect.EOF)
@@ -169,8 +167,8 @@
         self.login()
         self.connect()
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         '''disconnect and log out of vpn'''
         self.disconnect()
-        self.logout()
+        self.logout()
```

### Comparing `pyproton-0.0.4/pyproton.egg-info/PKG-INFO` & `pyproton-0.0.5/pyproton.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproton
-Version: 0.0.4
+Version: 0.0.5
 Summary: Minimal wrapper implementation of the linux protonvpn-cli
 Home-page: https://github.com/aastopher/pyproton
 Author: Aaron Stopher
 Project-URL: Bug Tracker, https://github.com/aastopher/pyproton/issues
 Keywords: vpn,proton vpn,proton,wrapper,cli
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,14 +17,18 @@
 
 [![PyPI version](https://badge.fury.io/py/pyproton.svg)](https://badge.fury.io/py/pyproton)
 
 This package is a lightweight minimal wrapper implementation of the linux protonvpn-cli; designed to be an intuitive and simple to use interface for the Proton VPN in python.
 
 ## Getting Started
 
+**Version compatibility:**
+
+`Proton VPN CLI v3.13.0 (protonvpn-nm-lib v3.14.0; proton-client v0.7.1)`
+
 ### **Install the CLI:**
 
 [Proton VPN Docs](https://protonvpn.com/support/linux-vpn-tool/)
 
 Debian based distros
 1. [Download the Proton VPN DEB package](https://repo.protonvpn.com/debian/dists/stable/main/binary-all/protonvpn-stable-release_1.0.3_all.deb)
 2. Install the Proton VPN repository
@@ -44,16 +48,16 @@
 ### **Import and use pyproton VPN:**
 
 #### Args
 
 * `user` **required:** user name string
 * `pw` **required:** password string
 * `verbose` **optional:** (`default=False`) turns on/off the stdin output for each step.
-* `retries` **optional:** (`default=3`) defines number of retries when VPN connection times out.
-* `timeout` **optional:** (`default=20`) seconds to wait before timing out a login attempt.
+* `retries` **optional:** (`default=3`) defines number of retries when a VPN connection attempt times out.
+* `timeout` **optional:** (`default=5`) seconds to wait before timing out a login attempt.
 * `location` **optional:** (`default='U'`) location of servers to connect to (free servers only): `{'J':'Japan','N':'Netherlands','U':'United States'}`.
 
 #### Methods
 
 * `vpn.login()` log the user into proton VPN - (context manager): `__enter__`
 * `vpn.logout()` log the user out of proton VPN - (context manager): `__exit__`
 * `vpn.connect()` connect to proton VPN endpoint - (context manager): `__enter__`
@@ -75,11 +79,12 @@
     print('do some stuff')
     vpn.shuffle()
     print('do more stuff')
 ```
 
 ### **TO-DO**
 
+* Improve reliability
 * PyTest & Tox testing
 * Sphynx docs
 * Coverage
 * Deepsource scanning
```

### Comparing `pyproton-0.0.4/setup.py` & `pyproton-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyproton",
-    version="0.0.4",
+    version="0.0.5",
     author="Aaron Stopher",
     packages=setuptools.find_packages(include=["pyproton"]),
     description="Minimal wrapper implementation of the linux protonvpn-cli",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aastopher/pyproton",
     project_urls={
```

