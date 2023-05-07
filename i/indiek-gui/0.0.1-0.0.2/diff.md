# Comparing `tmp/indiek-gui-0.0.1.tar.gz` & `tmp/indiek-gui-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-3464uv93/indiek-gui-0.0.1.tar", last modified: Fri May  5 01:36:51 2023, max compression
+gzip compressed data, was "/home/adrian_admin/prog/indiek/indiek-gui/dist/.tmp-udfpk_0l/indiek-gui-0.0.2.tar", last modified: Sun May  7 13:36:30 2023, max compression
```

## Comparing `indiek-gui-0.0.1.tar` & `indiek-gui-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-05 01:36:51.554862 indiek-gui-0.0.1/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.1/LICENSE
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-05 01:36:51.554862 indiek-gui-0.0.1/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-05 01:33:55.000000 indiek-gui-0.0.1/README.rst
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-05 01:36:51.550862 indiek-gui-0.0.1/indiek/
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-05 01:36:51.554862 indiek-gui-0.0.1/indiek/gui/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       12 2023-05-05 01:24:51.000000 indiek-gui-0.0.1/indiek/gui/__init__.py
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    11821 2023-05-05 01:29:47.000000 indiek-gui-0.0.1/indiek/gui/app.py
-drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-05 01:36:51.554862 indiek-gui-0.0.1/indiek_gui.egg-info/
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/PKG-INFO
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      284 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/SOURCES.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/dependency_links.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/entry_points.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       77 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/requires.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-05 01:36:51.000000 indiek-gui-0.0.1/indiek_gui.egg-info/top_level.txt
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-05 01:36:51.554862 indiek-gui-0.0.1/setup.cfg
--rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      942 2023-05-05 01:24:51.000000 indiek-gui-0.0.1/setup.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    34523 2023-05-05 01:24:51.000000 indiek-gui-0.0.2/LICENSE
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      555 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/README.rst
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek/
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek/gui/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       34 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/indiek/gui/__init__.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)    17488 2023-05-06 19:51:14.000000 indiek-gui-0.0.2/indiek/gui/app.py
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-06 19:18:51.000000 indiek-gui-0.0.2/indiek/gui/items.py
+drwxrwxr-x   0 adrian_admin  (1001) adrian_admin  (1001)        0 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/indiek_gui.egg-info/
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)     1003 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/PKG-INFO
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      304 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/SOURCES.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        1 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/dependency_links.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       47 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/entry_points.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)       56 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/requires.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)        7 2023-05-07 13:36:30.000000 indiek-gui-0.0.2/indiek_gui.egg-info/top_level.txt
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      147 2023-05-07 13:36:30.306254 indiek-gui-0.0.2/setup.cfg
+-rw-rw-r--   0 adrian_admin  (1001) adrian_admin  (1001)      920 2023-05-07 13:35:40.000000 indiek-gui-0.0.2/setup.py
```

### Comparing `indiek-gui-0.0.1/LICENSE` & `indiek-gui-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.1/PKG-INFO` & `indiek-gui-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.1/README.rst` & `indiek-gui-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `indiek-gui-0.0.1/indiek_gui.egg-info/PKG-INFO` & `indiek-gui-0.0.2/indiek_gui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indiek-gui
-Version: 0.0.1
+Version: 0.0.2
 Summary: Tkinter GUI for IndieK
 Home-page: https://pypi.org/project/indiek-gui/
 Author: Adrian Ernesto Radillo
 Author-email: adrian.radillo@gmail.com
 License: GNU Affero General Public License v3.0
 Project-URL: GitHub, https://github.com/indiek/indiek-gui
 Project-URL: Documentation, https://indiekgui.readthedocs.io/en/latest/
```

### Comparing `indiek-gui-0.0.1/setup.py` & `indiek-gui-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 this_dir = abspath(dirname(__file__))
 with open(join(this_dir, 'README.rst'), encoding='utf-8') as file:
     long_description = file.read()
 
 setup(
     name='indiek-gui',
     python_requires='>=3.8',
-    version='0.0.1',
+    version='0.0.2',
     url='https://pypi.org/project/indiek-gui/',
     description='Tkinter GUI for IndieK',
     long_description=long_description,
     author='Adrian Ernesto Radillo',
     author_email='adrian.radillo@gmail.com',
     license='GNU Affero General Public License v3.0',
     packages=['indiek.gui'],
-    install_requires=['indiek-mockdb==0.1.1', 'indiek-core==0.1.1'],
+    install_requires=['indiek-core == 0.1.2'],
     extras_require={
         'dev': [
             'pytest',
             'pytest-pep8',
             'pytest-cov'
         ]
     },
```

