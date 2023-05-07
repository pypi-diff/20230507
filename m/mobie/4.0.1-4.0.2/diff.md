# Comparing `tmp/mobie-4.0.1.tar.gz` & `tmp/mobie-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobie-4.0.1.tar", last modified: Fri May  5 12:25:21 2023, max compression
+gzip compressed data, was "mobie-4.0.2.tar", last modified: Sun May  7 13:58:16 2023, max compression
```

## Comparing `mobie-4.0.1.tar` & `mobie-4.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.672637 mobie-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-05 12:25:19.000000 mobie-4.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:25:21.672637 mobie-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-05 12:25:19.000000 mobie-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.668637 mobie-4.0.1/mobie/
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 12:25:19.000000 mobie-4.0.1/mobie/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.672637 mobie-4.0.1/mobie.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:25:21.672637 mobie-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-05 12:25:19.000000 mobie-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-07 13:58:14.000000 mobie-4.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 13:58:16.579856 mobie-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-07 13:58:14.000000 mobie-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/mobie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-07 13:58:14.000000 mobie-4.0.2/mobie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 13:58:16.579856 mobie-4.0.2/mobie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 13:58:16.000000 mobie-4.0.2/mobie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 13:58:16.579856 mobie-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-07 13:58:14.000000 mobie-4.0.2/setup.py
```

### Comparing `mobie-4.0.1/LICENSE.txt` & `mobie-4.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mobie-4.0.1/README.md` & `mobie-4.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 ## Development
 
 ### Install mamba
 
 Download mamba-forge
 
-### Manage pypi packages
+### Manage pypi package
 
-- https://pypi.org/
+- https://pypi.org/project/mobie/
+
+### Check versions on conda
+
+- https://anaconda.org/conda-forge/mobie
 
 ### Create mobie-dev env
 
 ```
 mamba create -y -n mobie-dev -c conda-forge openjdk=8 jgo pip maven blosc
 ```
 
@@ -26,23 +30,21 @@
 2. hardcode this version in `__init__.py`: e.g., 
    `_artifactVersion         = '3.2.0-SNAPSHOT' #version("mobie")` 
    
 continue as in [test locally](#test-locally)
 
 ### Release a new version
 
-This is not needed for local testing.
-
-Example for version `3.0.11`:
+Example for version `3.0.10`:
 
 #### mobie-viewer-fiji repo
 
-Within the mobie Java code change the versions here:
+Within the mobie Java code update the versions in all command line tools, e.g.:
 ```java
-@CommandLine.Command(name = "mobie", mixinStandardHelpOptions = true, version = "3.0.11", description = "Visualise multi-modal big image data, see https://mobie.github.io/")
+@CommandLine.Command(name = "mobie", mixinStandardHelpOptions = true, version = "3.0.10", description = "Visualise multi-modal big image data, see https://mobie.github.io/")
 ```
 
 Use the below lines to make a maven release:
 
 ```
 mamba activate mobie-dev # this activates java 8!
 ./install.sh  # test the line of code suggested by the script!
@@ -58,31 +60,37 @@
 
 ```
 git add setup.py
 git commit -m "Version bump 3.0.10"
 ```
 
 
-##### test locally
+#### test locally
 
 ```
 mamba activate mobie-dev
 pip install -e .
 mobie --help
 mobie project -p "https://github.com/mobie/platybrowser-project"
 mobie files -r "/Users/tischer/Documents/mobie/src/test/resources/input/skimage-2d-tiff/" -i "image.tif" -l "segmentation.tif" -t "table.tsv"
 ```
 
-##### deploy
+#### deploy to pypi
 
 ```
 git tag 3.0.10
 git push --tags
 ```
 
+Pushing a tag triggers build and deploy to pypi via github actions that are configured in the mobie-cmd repo.
+
+#### release on conda-forge
+
+deploying to pypi (s.a.) automatically triggers a PR in https://github.com/conda-forge/mobie-feedstock
+
 
 #### Troubleshooting
 
 Remove a tag (remote and local):
 
 ```
 git push origin --delete 3.0.10
```

### Comparing `mobie-4.0.1/mobie/__init__.py` & `mobie-4.0.2/mobie/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from importlib.metadata import version
 from functools import partial
 
 _picocli_autocomplete = "picocli.AutoComplete"
 _mobie_main_class = "org.embl.mobie.cmd.MoBIECmd"
 _groupId = "org.embl.mobie"
 _artifactId = "mobie-viewer-fiji"
-_artifactVersion = "3.2.0-SNAPSHOT"  # version("mobie")
+_artifactVersion = version("mobie")
 
 
 def launch_mobie(main_class, mobie_options):
     return jgo.util.main_from_endpoint(
         argv=mobie_options,
         primary_endpoint=f"{_groupId}:{_artifactId}",
         primary_endpoint_main_class=main_class,
```

### Comparing `mobie-4.0.1/setup.py` & `mobie-4.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 entry_points = {
     "console_scripts": [
         "mobie=mobie:main",
     ]
 }
 
-version = "4.0.1"
+version = "4.0.2"
 
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python :: 3 :: Only",
 ]
 
 package_urls = {
```

