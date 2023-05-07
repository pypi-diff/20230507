# Comparing `tmp/arvan_dns-1.0.2.tar.gz` & `tmp/arvan_dns-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arvan_dns-1.0.2.tar", last modified: Sun May  7 13:07:29 2023, max compression
+gzip compressed data, was "arvan_dns-1.0.5.tar", last modified: Sun May  7 21:27:51 2023, max compression
```

## Comparing `arvan_dns-1.0.2.tar` & `arvan_dns-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-07 13:07:29.423051 arvan_dns-1.0.2/
--rw-r--r--   0 seyed      (501) staff       (20)       55 2023-05-06 20:01:14.000000 arvan_dns-1.0.2/.gitignore
--rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-07 13:07:29.422872 arvan_dns-1.0.2/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      588 2023-05-07 13:06:38.000000 arvan_dns-1.0.2/README.md
--rw-r--r--   0 seyed      (501) staff       (20)        0 2023-05-06 19:41:19.000000 arvan_dns-1.0.2/__init__.py
-drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-07 13:07:29.422653 arvan_dns-1.0.2/arvan_dns.egg-info/
--rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/PKG-INFO
--rw-r--r--   0 seyed      (501) staff       (20)      254 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/SOURCES.txt
--rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/dependency_links.txt
--rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/entry_points.txt
--rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/requires.txt
--rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-07 13:07:29.000000 arvan_dns-1.0.2/arvan_dns.egg-info/top_level.txt
--rw-r--r--   0 seyed      (501) staff       (20)     3992 2023-05-07 13:06:11.000000 arvan_dns-1.0.2/arvan_dns.py
--rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-07 13:07:29.423200 arvan_dns-1.0.2/setup.cfg
--rw-r--r--   0 seyed      (501) staff       (20)      533 2023-05-07 13:06:57.000000 arvan_dns-1.0.2/setup.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-07 21:27:51.495991 arvan_dns-1.0.5/
+-rw-r--r--   0 seyed      (501) staff       (20)       55 2023-05-06 20:01:14.000000 arvan_dns-1.0.5/.gitignore
+-rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-07 21:27:51.495831 arvan_dns-1.0.5/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      588 2023-05-07 13:06:38.000000 arvan_dns-1.0.5/README.md
+-rw-r--r--   0 seyed      (501) staff       (20)        0 2023-05-06 19:41:19.000000 arvan_dns-1.0.5/__init__.py
+drwxr-xr-x   0 seyed      (501) staff       (20)        0 2023-05-07 21:27:51.495596 arvan_dns-1.0.5/arvan_dns.egg-info/
+-rw-r--r--   0 seyed      (501) staff       (20)      841 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/PKG-INFO
+-rw-r--r--   0 seyed      (501) staff       (20)      254 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/SOURCES.txt
+-rw-r--r--   0 seyed      (501) staff       (20)        1 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/dependency_links.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       45 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/entry_points.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       18 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/requires.txt
+-rw-r--r--   0 seyed      (501) staff       (20)       10 2023-05-07 21:27:51.000000 arvan_dns-1.0.5/arvan_dns.egg-info/top_level.txt
+-rw-r--r--   0 seyed      (501) staff       (20)     3714 2023-05-07 21:26:17.000000 arvan_dns-1.0.5/arvan_dns.py
+-rw-r--r--   0 seyed      (501) staff       (20)       38 2023-05-07 21:27:51.496036 arvan_dns-1.0.5/setup.cfg
+-rw-r--r--   0 seyed      (501) staff       (20)      533 2023-05-07 21:27:43.000000 arvan_dns-1.0.5/setup.py
```

### Comparing `arvan_dns-1.0.2/PKG-INFO` & `arvan_dns-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arvan_dns
-Version: 1.0.2
+Version: 1.0.5
 Summary: Arvan DNS updater
 Home-page: https://github.com/seyed-dev/arvan-dns
 Author: SeYeD.DeV
 Author-email: me@seyed.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `arvan_dns-1.0.2/README.md` & `arvan_dns-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `arvan_dns-1.0.2/arvan_dns.egg-info/PKG-INFO` & `arvan_dns-1.0.5/arvan_dns.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arvan-dns
-Version: 1.0.2
+Version: 1.0.5
 Summary: Arvan DNS updater
 Home-page: https://github.com/seyed-dev/arvan-dns
 Author: SeYeD.DeV
 Author-email: me@seyed.dev
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `arvan_dns-1.0.2/arvan_dns.py` & `arvan_dns-1.0.5/arvan_dns.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 DOMAINS_FILE = args.domains_file
 PORT = args.port
 
 headers = {
         'authority': 'napi.arvancloud.ir',
         'accept': 'application/json, text/plain, */*',
         'accept-language': 'fa',
-        'authorization': f'Bearer DwVZf8ZpyZgP5eoGVP5KUMxeLAAJziAxUBu7Cu2Vf0s6e0jRKoqzsVAbYiGDiWZ6d973Lb5xQlhzzcy2qd6CrD0Q7aCsMQ4KSQlMqjOkDy1R74HfMdSK0gG5Jwdonqe2K4LJWmL1xXRrzdzlmPr5pDmYxLkaaYAbNQYEdttFOFJK6PgJs5FS9HMXTgy27Ip7EzvRGrV6Jb0PQx4npsk2lKjXSWWnclS7SboLUs6gE7mslR92oH3e2Cku5VB9bxX.d8e200a4-1307-441e-a920-9cccf7f4b23d',
+        'authorization': f'Bearer {BEARER_TOKEN}',
         'content-type': 'application/json',
         'origin': 'https://panel.arvancloud.ir',
         'referer': 'https://panel.arvancloud.ir/',
         'sec-ch-ua': '"Google Chrome";v="113", "Chromium";v="113", "Not-A.Brand";v="24"',
         'sec-ch-ua-mobile': '?0',
         'sec-ch-ua-platform': '"macOS"',
         'sec-fetch-dest': 'empty',
```

### Comparing `arvan_dns-1.0.2/setup.py` & `arvan_dns-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='arvan_dns',
-    version='1.0.2',
+    version='1.0.5',
     description='Arvan DNS updater',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     py_modules=['arvan_dns'],
     install_requires=[
         'requests',
         'argparse'
```

