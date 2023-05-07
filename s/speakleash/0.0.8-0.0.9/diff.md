# Comparing `tmp/speakleash-0.0.8.tar.gz` & `tmp/speakleash-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakleash-0.0.8.tar", last modified: Sun Dec 11 23:04:03 2022, max compression
+gzip compressed data, was "speakleash-0.0.9.tar", last modified: Mon Dec 12 22:47:55 2022, max compression
```

## Comparing `speakleash-0.0.8.tar` & `speakleash-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-11 23:04:03.855097 speakleash-0.0.8/
--rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.0.8/LICENSE
--rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-11 23:04:03.854793 speakleash-0.0.8/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)     1391 2022-12-11 23:01:51.000000 speakleash-0.0.8/README.md
--rw-r--r--   0 skondracki   (502) staff       (20)       38 2022-12-11 23:04:03.855189 speakleash-0.0.8/setup.cfg
--rw-r--r--   0 skondracki   (502) staff       (20)      571 2022-12-11 22:32:47.000000 speakleash-0.0.8/setup.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-11 23:04:03.852588 speakleash-0.0.8/speakleash/
--rw-r--r--   0 skondracki   (502) staff       (20)     5006 2022-12-11 22:59:47.000000 speakleash-0.0.8/speakleash/__init__.py
-drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-11 23:04:03.854366 speakleash-0.0.8/speakleash.egg-info/
--rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-11 23:04:03.000000 speakleash-0.0.8/speakleash.egg-info/PKG-INFO
--rw-r--r--   0 skondracki   (502) staff       (20)      218 2022-12-11 23:04:03.000000 speakleash-0.0.8/speakleash.egg-info/SOURCES.txt
--rw-r--r--   0 skondracki   (502) staff       (20)        1 2022-12-11 23:04:03.000000 speakleash-0.0.8/speakleash.egg-info/dependency_links.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       28 2022-12-11 23:04:03.000000 speakleash-0.0.8/speakleash.egg-info/requires.txt
--rw-r--r--   0 skondracki   (502) staff       (20)       11 2022-12-11 23:04:03.000000 speakleash-0.0.8/speakleash.egg-info/top_level.txt
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.473712 speakleash-0.0.9/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1082 2022-11-13 16:50:03.000000 speakleash-0.0.9/LICENSE
+-rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-12 22:47:55.473360 speakleash-0.0.9/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)     1391 2022-12-11 23:01:51.000000 speakleash-0.0.9/README.md
+-rw-r--r--   0 skondracki   (502) staff       (20)       38 2022-12-12 22:47:55.473809 speakleash-0.0.9/setup.cfg
+-rw-r--r--   0 skondracki   (502) staff       (20)      571 2022-12-12 22:45:55.000000 speakleash-0.0.9/setup.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.470436 speakleash-0.0.9/speakleash/
+-rw-r--r--   0 skondracki   (502) staff       (20)     5224 2022-12-12 22:38:04.000000 speakleash-0.0.9/speakleash/__init__.py
+drwxr-xr-x   0 skondracki   (502) staff       (20)        0 2022-12-12 22:47:55.472934 speakleash-0.0.9/speakleash.egg-info/
+-rw-r--r--   0 skondracki   (502) staff       (20)     1689 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/PKG-INFO
+-rw-r--r--   0 skondracki   (502) staff       (20)      218 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/SOURCES.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)        1 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/dependency_links.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       28 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/requires.txt
+-rw-r--r--   0 skondracki   (502) staff       (20)       11 2022-12-12 22:47:55.000000 speakleash-0.0.9/speakleash.egg-info/top_level.txt
```

### Comparing `speakleash-0.0.8/LICENSE` & `speakleash-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `speakleash-0.0.8/PKG-INFO` & `speakleash-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.0.8
+Version: 0.0.9
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `speakleash-0.0.8/README.md` & `speakleash-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `speakleash-0.0.8/setup.py` & `speakleash-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="speakleash",
-    version="0.0.8",
+    version="0.0.9",
     author="SpeakLeash Team",
     author_email="team@speakleash.org",
     description="SpeakLeash agnostic dataset for Polish",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/speakleash/speakleash",
     packages = ["speakleash"],
```

### Comparing `speakleash-0.0.8/speakleash/__init__.py` & `speakleash-0.0.9/speakleash/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
         self.datasets = []
         self.datasets.append(SpeakleashDataset("thesis", "https://zazepa.pl/speakleash/", self.replicate_dir))
         self.datasets.append(SpeakleashDataset("plwiki", "https://zazepa.pl/speakleash/", self.replicate_dir))
         self.datasets.append(SpeakleashDataset("1000_novels_corpus_CLARIN-PL", "https://zazepa.pl/speakleash/", self.replicate_dir))
         self.datasets.append(SpeakleashDataset("wolne_lektury_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
         self.datasets.append(SpeakleashDataset("project_gutenberg_pl_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
         self.datasets.append(SpeakleashDataset("open_subtitles_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
+        self.datasets.append(SpeakleashDataset("biblioteka_nauki_pl_corpus", "https://zazepa.pl/speakleash/", self.replicate_dir))
     def get(self, name):
         for d in self.datasets:
             if d.name == name:
                 return d
         return None
 
 class SpeakleashDataset(object):
@@ -100,14 +101,18 @@
         return self.manifest.get("description","")
 
     @property
     def license(self):
         return self.manifest.get("license","")
 
     @property
+    def category(self):
+        return self.manifest.get("category","")
+
+    @property
     def sources (self):
         return self.manifest.get("sources",{})
 
 
     @property
     def jsonl_zst_file_size(self):
         return self.manifest.get("file_size",0)
```

### Comparing `speakleash-0.0.8/speakleash.egg-info/PKG-INFO` & `speakleash-0.0.9/speakleash.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakleash
-Version: 0.0.8
+Version: 0.0.9
 Summary: SpeakLeash agnostic dataset for Polish
 Home-page: https://github.com/speakleash/speakleash
 Author: SpeakLeash Team
 Author-email: team@speakleash.org
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

