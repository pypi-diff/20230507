# Comparing `tmp/slashml-0.1.tar.gz` & `tmp/slashml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-3b8dsknu/slashml-0.1.tar", last modified: Mon Apr 24 08:22:28 2023, max compression
+gzip compressed data, was "/Users/faizank/workspace/experiments/live_projects/slashml/sdk_tests/slashml/dist/.tmp-gkluihqa/slashml-0.1.1.tar", last modified: Sat May  6 22:11:49 2023, max compression
```

## Comparing `slashml-0.1.tar` & `slashml-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-04-24 08:22:28.720764 slashml-0.1/
--rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1/LICENSE.txt
--rw-r--r--   0 faizank    (501) staff       (20)      277 2023-04-24 08:22:28.720589 slashml-0.1/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)     6847 2023-04-24 07:51:41.000000 slashml-0.1/README.md
--rw-r--r--   0 faizank    (501) staff       (20)       38 2023-04-24 08:22:28.720815 slashml-0.1/setup.cfg
--rw-r--r--   0 faizank    (501) staff       (20)      728 2023-04-24 08:22:15.000000 slashml-0.1/setup.py
-drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-04-24 08:22:28.720388 slashml-0.1/slashml.egg-info/
--rw-r--r--   0 faizank    (501) staff       (20)      277 2023-04-24 08:22:28.000000 slashml-0.1/slashml.egg-info/PKG-INFO
--rw-r--r--   0 faizank    (501) staff       (20)      184 2023-04-24 08:22:28.000000 slashml-0.1/slashml.egg-info/SOURCES.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-04-24 08:22:28.000000 slashml-0.1/slashml.egg-info/dependency_links.txt
--rw-r--r--   0 faizank    (501) staff       (20)       17 2023-04-24 08:22:28.000000 slashml-0.1/slashml.egg-info/requires.txt
--rw-r--r--   0 faizank    (501) staff       (20)        1 2023-04-24 08:22:28.000000 slashml-0.1/slashml.egg-info/top_level.txt
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-06 22:11:49.718359 slashml-0.1.1/
+-rw-r--r--   0 faizank    (501) staff       (20)     1064 2023-04-24 05:35:14.000000 slashml-0.1.1/LICENSE.txt
+-rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-06 22:11:49.718192 slashml-0.1.1/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)     6847 2023-04-24 07:51:41.000000 slashml-0.1.1/README.md
+-rw-r--r--   0 faizank    (501) staff       (20)       38 2023-05-06 22:11:49.718410 slashml-0.1.1/setup.cfg
+-rw-r--r--   0 faizank    (501) staff       (20)      730 2023-05-06 22:11:38.000000 slashml-0.1.1/setup.py
+drwxr-xr-x   0 faizank    (501) staff       (20)        0 2023-05-06 22:11:49.717994 slashml-0.1.1/slashml.egg-info/
+-rw-r--r--   0 faizank    (501) staff       (20)      279 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/PKG-INFO
+-rw-r--r--   0 faizank    (501) staff       (20)      184 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/SOURCES.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/dependency_links.txt
+-rw-r--r--   0 faizank    (501) staff       (20)       17 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/requires.txt
+-rw-r--r--   0 faizank    (501) staff       (20)        1 2023-05-06 22:11:49.000000 slashml-0.1.1/slashml.egg-info/top_level.txt
```

### Comparing `slashml-0.1/LICENSE.txt` & `slashml-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `slashml-0.1/README.md` & `slashml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `slashml-0.1/setup.py` & `slashml-0.1.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     with open(f"{SLASHML_DIR}requires-{req_type}.txt") as fp:  # pylint: disable=W1514
         requires = (line.strip() for line in fp)
         return [req for req in requires if req and not req.startswith("#")]
 
 
 setup(
     name="slashml",
-    version="0.1",
+    version="0.1.1",
     url="https://slashml.com/",
     author="eff-kay",
     author_email="faiizan14@gmail.com",
     description=(
         "A Python client for interacting with SlashML services" "Developed by SlashML."
     ),
     packages=find_packages("slashml"),
```

