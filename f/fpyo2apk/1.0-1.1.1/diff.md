# Comparing `tmp/fpyo2apk-1.0.tar.gz` & `tmp/fpyo2apk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpyo2apk-1.0.tar", last modified: Sun May  7 21:07:59 2023, max compression
+gzip compressed data, was "fpyo2apk-1.1.1.tar", last modified: Sun May  7 21:22:53 2023, max compression
```

## Comparing `fpyo2apk-1.0.tar` & `fpyo2apk-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.193226 fpyo2apk-1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:07:47.000000 fpyo2apk-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 21:07:47.000000 fpyo2apk-1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-07 21:07:59.193226 fpyo2apk-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:47.000000 fpyo2apk-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.189226 fpyo2apk-1.0/fpyo2apk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.193226 fpyo2apk-1.0/fpyo2apk/Tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/Tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/Tools/check_system.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/Tools/check_venv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/Tools/unzip_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.193226 fpyo2apk-1.0/fpyo2apk/assets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/assets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/assets/fpyo2apkdist.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.193226 fpyo2apk-1.0/fpyo2apk/beeware_tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/beeware_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/beeware_tools/edit_beeware_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/beeware_tools/the_app_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/beeware_tools/the_localhost_py.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 21:07:47.000000 fpyo2apk-1.0/fpyo2apk/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:07:59.189226 fpyo2apk-1.0/fpyo2apk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-07 21:07:59.000000 fpyo2apk-1.0/fpyo2apk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-07 21:07:59.000000 fpyo2apk-1.0/fpyo2apk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:07:59.000000 fpyo2apk-1.0/fpyo2apk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:07:59.000000 fpyo2apk-1.0/fpyo2apk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 21:07:59.000000 fpyo2apk-1.0/fpyo2apk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 21:07:47.000000 fpyo2apk-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:07:59.193226 fpyo2apk-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-07 21:07:47.000000 fpyo2apk-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/Tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/check_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/check_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/Tools/unzip_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/assets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   495603 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/assets/fpyo2apkdist.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/edit_beeware_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_app_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_localhost_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/fpyo2apk/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/fpyo2apk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-07 21:22:53.000000 fpyo2apk-1.1.1/fpyo2apk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 21:22:53.270157 fpyo2apk-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-07 21:22:42.000000 fpyo2apk-1.1.1/setup.py
```

### Comparing `fpyo2apk-1.0/LICENSE` & `fpyo2apk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk/Tools/unzip_assets.py` & `fpyo2apk-1.1.1/fpyo2apk/Tools/unzip_assets.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk/assets/fpyo2apkdist.zip` & `fpyo2apk-1.1.1/fpyo2apk/assets/fpyo2apkdist.zip`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk/beeware_tools/edit_beeware_project.py` & `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/edit_beeware_project.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     project_name = "fpyo2apkdist"
     if not os.path.isdir(project_name):
         raise FileNotFoundError(f"There is no folder with path '{project_name}'.")
     
     if not os.path.isdir(f"{project_name}/src"):
         raise FileNotFoundError(f"There is no folder with path '{project_name}/src'.")
     
-    if not os.path.isdir(f"{project_name}/src/fpyo2apkdist/assets"):
-        os.mkdir(f"{project_name}/src/fpyo2apkdist/assets")
+    if not os.path.isdir(f"{project_name}/src/fpyo2apk/assets"):
+        os.mkdir(f"{project_name}/src/fpyo2apk/assets")
     
     if not os.path.isdir("dist"):
         raise FileNotFoundError("There must be a flet-pyodide folder called `dist` to start.")
     
     print("editing the dist..")
     if '  <base href="/basedurlhere/">' in open("dist/index.html", encoding="utf-8").read():
         pass
@@ -31,23 +31,23 @@
         sys.exit("Exit with Error: The base/href url of the dist must be '/'.")
     
     the_index_file = open("dist/index.html", encoding="utf-8").read()
     the_index_file = str(the_index_file).replace('  <base href="/">', '  <base href="/basedurlhere/">')
     open("dist/index.html", "w+", encoding="utf-8").write(the_index_file)
 
     print("copy the dist..")
-    if os.path.isdir(f"{project_name}/src/fpyo2apkdist/assets/dist"):
-        shutil.rmtree(f"{project_name}/src/fpyo2apkdist/assets/dist")
-    shutil.copytree("dist", f"{project_name}/src/fpyo2apkdist/assets/dist")
+    if os.path.isdir(f"{project_name}/src/fpyo2apk/assets/dist"):
+        shutil.rmtree(f"{project_name}/src/fpyo2apk/assets/dist")
+    shutil.copytree("dist", f"{project_name}/src/fpyo2apk/assets/dist")
 
     print("start edit the 'app.py' file")
-    open(f"{project_name}/src/fpyo2apkdist/app.py", "w+", encoding="utf-8").write(The_app_py_script)
+    open(f"{project_name}/src/fpyo2apk/app.py", "w+", encoding="utf-8").write(The_app_py_script)
 
     print("start creating/editing the 'localhost.py' file")
-    open(f"{project_name}/src/fpyo2apkdist/localhost.py", "w+", encoding="utf-8").write(The_localhost_py_script)
+    open(f"{project_name}/src/fpyo2apk/localhost.py", "w+", encoding="utf-8").write(The_localhost_py_script)
 
     print("Your app is being built and then opened on the iOS simulator..\nThis Usually take two minutes to finish, please wait..")
     process = subprocess.Popen(["cd fpyo2apkdist\nbriefcase create Android\nbriefcase build Android\n"], stdin=subprocess.PIPE, stdout=subprocess.PIPE, shell=True)
     output, error = process.communicate()
     if error != None:
         sys.exit(f"\nExit with Error: {error}")
```

### Comparing `fpyo2apk-1.0/fpyo2apk/beeware_tools/the_app_py.py` & `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_app_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk/beeware_tools/the_localhost_py.py` & `fpyo2apk-1.1.1/fpyo2apk/beeware_tools/the_localhost_py.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk/build.py` & `fpyo2apk-1.1.1/fpyo2apk/build.py`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/fpyo2apk.egg-info/SOURCES.txt` & `fpyo2apk-1.1.1/fpyo2apk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fpyo2apk-1.0/setup.py` & `fpyo2apk-1.1.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fpyo2apk',
-    version='1.0',
+    version='1.1.1',
     author='SKbarbon',
     description='A package tool that allow you to built a python Android apps with flet-pyodide dist.',
     long_description="https://github.com/SKbarbon/fpyo2apk",
     url='https://github.com/SKbarbon/fpyo2apk',
     install_requires=["briefcase==0.3.14"],
     include_package_data=True,
     packages=find_packages(),
```

