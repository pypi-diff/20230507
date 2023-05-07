# Comparing `tmp/pynixconfig-0.1.0.tar.gz` & `tmp/pynixconfig-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynixconfig-0.1.0.tar", last modified: Mon Mar 27 05:02:02 2023, max compression
+gzip compressed data, was "pynixconfig-0.1.1.tar", last modified: Sun May  7 17:25:05 2023, max compression
```

## Comparing `pynixconfig-0.1.0.tar` & `pynixconfig-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,27 @@
-drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-03-27 05:02:02.647870 pynixconfig-0.1.0/
--rw-r--r--   0 sergionahas   (501) staff       (20)      431 2023-03-27 04:54:34.000000 pynixconfig-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 sergionahas   (501) staff       (20)     1069 2023-02-20 00:48:15.000000 pynixconfig-0.1.0/LICENSE
--rw-r--r--   0 sergionahas   (501) staff       (20)      355 2023-03-27 05:01:11.000000 pynixconfig-0.1.0/MANIFEST.in
--rw-r--r--   0 sergionahas   (501) staff       (20)      840 2023-03-27 03:59:08.000000 pynixconfig-0.1.0/Makefile
--rw-r--r--   0 sergionahas   (501) staff       (20)     3146 2023-03-27 05:02:02.647553 pynixconfig-0.1.0/PKG-INFO
--rw-r--r--   0 sergionahas   (501) staff       (20)     1062 2023-03-27 04:54:34.000000 pynixconfig-0.1.0/README.md
-drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-03-27 05:02:02.644106 pynixconfig-0.1.0/pynixconfig/
--rw-r--r--   0 sergionahas   (501) staff       (20)      151 2023-03-27 03:22:19.000000 pynixconfig-0.1.0/pynixconfig/__init__.py
--rw-r--r--   0 sergionahas   (501) staff       (20)     1969 2023-03-27 03:59:35.000000 pynixconfig-0.1.0/pynixconfig/linuxconfig.py
-drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-03-27 05:02:02.646694 pynixconfig-0.1.0/pynixconfig/tests/
--rw-r--r--   0 sergionahas   (501) staff       (20)      760 2023-03-27 03:54:43.000000 pynixconfig-0.1.0/pynixconfig/tests/test_all.py
-drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-03-27 05:02:02.646417 pynixconfig-0.1.0/pynixconfig.egg-info/
--rw-r--r--   0 sergionahas   (501) staff       (20)     3146 2023-03-27 05:02:02.000000 pynixconfig-0.1.0/pynixconfig.egg-info/PKG-INFO
--rw-r--r--   0 sergionahas   (501) staff       (20)      333 2023-03-27 05:02:02.000000 pynixconfig-0.1.0/pynixconfig.egg-info/SOURCES.txt
--rw-r--r--   0 sergionahas   (501) staff       (20)        1 2023-03-27 05:02:02.000000 pynixconfig-0.1.0/pynixconfig.egg-info/dependency_links.txt
--rw-r--r--   0 sergionahas   (501) staff       (20)      156 2023-03-27 05:02:02.000000 pynixconfig-0.1.0/pynixconfig.egg-info/requires.txt
--rw-r--r--   0 sergionahas   (501) staff       (20)       12 2023-03-27 05:02:02.000000 pynixconfig-0.1.0/pynixconfig.egg-info/top_level.txt
--rw-r--r--   0 sergionahas   (501) staff       (20)     2175 2023-03-12 03:42:21.000000 pynixconfig-0.1.0/pyproject.toml
--rw-r--r--   0 sergionahas   (501) staff       (20)       38 2023-03-27 05:02:02.648011 pynixconfig-0.1.0/setup.cfg
--rw-r--r--   0 sergionahas   (501) staff       (20)       38 2023-03-03 00:02:19.000000 pynixconfig-0.1.0/setup.py
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.017592 pynixconfig-0.1.1/
+-rw-r--r--   0 sergionahas   (501) staff       (20)      431 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 sergionahas   (501) staff       (20)     1069 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/LICENSE
+-rw-r--r--   0 sergionahas   (501) staff       (20)      474 2023-05-07 17:17:53.000000 pynixconfig-0.1.1/MANIFEST.in
+-rw-r--r--   0 sergionahas   (501) staff       (20)      840 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/Makefile
+-rw-r--r--   0 sergionahas   (501) staff       (20)     3307 2023-05-07 17:25:05.017090 pynixconfig-0.1.1/PKG-INFO
+-rw-r--r--   0 sergionahas   (501) staff       (20)     1223 2023-05-07 07:29:46.000000 pynixconfig-0.1.1/README.md
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.003884 pynixconfig-0.1.1/docs/
+-rw-r--r--   0 sergionahas   (501) staff       (20)      638 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/docs/Makefile
+-rw-r--r--   0 sergionahas   (501) staff       (20)      804 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/docs/make.bat
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.007751 pynixconfig-0.1.1/docs/source/
+-rw-r--r--   0 sergionahas   (501) staff       (20)     2289 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/docs/source/conf.py
+-rw-r--r--   0 sergionahas   (501) staff       (20)      372 2023-05-07 06:26:28.000000 pynixconfig-0.1.1/docs/source/index.md
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.012406 pynixconfig-0.1.1/pynixconfig/
+-rw-r--r--   0 sergionahas   (501) staff       (20)      167 2023-05-07 07:29:46.000000 pynixconfig-0.1.1/pynixconfig/__init__.py
+-rw-r--r--   0 sergionahas   (501) staff       (20)     2507 2023-05-07 07:29:46.000000 pynixconfig-0.1.1/pynixconfig/linuxconfig.py
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.016185 pynixconfig-0.1.1/pynixconfig/tests/
+-rw-r--r--   0 sergionahas   (501) staff       (20)      887 2023-05-07 07:29:46.000000 pynixconfig-0.1.1/pynixconfig/tests/test_all.py
+drwxr-xr-x   0 sergionahas   (501) staff       (20)        0 2023-05-07 17:25:05.015864 pynixconfig-0.1.1/pynixconfig.egg-info/
+-rw-r--r--   0 sergionahas   (501) staff       (20)     3307 2023-05-07 17:25:04.000000 pynixconfig-0.1.1/pynixconfig.egg-info/PKG-INFO
+-rw-r--r--   0 sergionahas   (501) staff       (20)      402 2023-05-07 17:25:04.000000 pynixconfig-0.1.1/pynixconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 sergionahas   (501) staff       (20)        1 2023-05-07 17:25:04.000000 pynixconfig-0.1.1/pynixconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 sergionahas   (501) staff       (20)      156 2023-05-07 17:25:04.000000 pynixconfig-0.1.1/pynixconfig.egg-info/requires.txt
+-rw-r--r--   0 sergionahas   (501) staff       (20)       12 2023-05-07 17:25:04.000000 pynixconfig-0.1.1/pynixconfig.egg-info/top_level.txt
+-rw-r--r--   0 sergionahas   (501) staff       (20)     2175 2023-05-07 17:24:49.000000 pynixconfig-0.1.1/pyproject.toml
+-rw-r--r--   0 sergionahas   (501) staff       (20)       38 2023-05-07 17:25:05.017859 pynixconfig-0.1.1/setup.cfg
+-rw-r--r--   0 sergionahas   (501) staff       (20)       83 2023-05-07 17:24:09.000000 pynixconfig-0.1.1/setup.py
```

### Comparing `pynixconfig-0.1.0/LICENSE` & `pynixconfig-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynixconfig-0.1.0/Makefile` & `pynixconfig-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pynixconfig-0.1.0/PKG-INFO` & `pynixconfig-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynixconfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple way to config your terminal colors
 Author-email: Sergio Nahas <sn2865@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Sergio Nahas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,31 +49,42 @@
 
 <img src="https://img.shields.io/github/issues/sn2865/pynixconfig" alt="issues"></img>
 
 ![Build Status](https://github.com/sn2865/pynixconfig/actions/workflows/build.yml/badge.svg)
 
 [![codecov](https://codecov.io/gh/sn2865/pynixconfig/branch/main/graph/badge.svg)](https://codecov.io/gh/sn2865/pynixconfig)
 
+[![PyPI](https://img.shields.io/pypi/v/pynixconfig)](https://pypi.org/project/pynixconfig/0.1.0/)
+
+[![Docs](https://img.shields.io/readthedocs/pynixconfig.svg)](https://pynixconfig.readthedocs.io/en/latest/)
+
 # Overview
 
-This library will enable beginners to easily configure their UNIX environment for it to look cool.
-It will allow users to configure anything ranging from environment variables, what their terminal looks like,
-credentials, etc.. using a simple python generated user interface.
+This library allows to easily configure a linux terminal. 
+
+The three configurations developed so far:
+file colors
+shell color
+fonts
+
+# Demo
+
+Watch the Demo here: [Youtube](https://www.youtube.com/watch?v=enuFhW7qoJU)
 
 # Installation
 
 pip install pynixconfig
 
 # Using the Library
 
 1. modify your configs in pynixconfig/linuxconfig.py
 
 2. Run the following command in the root directory of project: $ make run
 
 # Instructions
 
 clone repo on your local
-modify color and font in pynixconfig/linuxconfig.py
+modify color and font and shell in pynixconfig/linuxconfig.py
 
 run command: make run
```

### Comparing `pynixconfig-0.1.0/README.md` & `pynixconfig-0.1.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -6,29 +6,40 @@
 
 <img src="https://img.shields.io/github/issues/sn2865/pynixconfig" alt="issues"></img>
 
 ![Build Status](https://github.com/sn2865/pynixconfig/actions/workflows/build.yml/badge.svg)
 
 [![codecov](https://codecov.io/gh/sn2865/pynixconfig/branch/main/graph/badge.svg)](https://codecov.io/gh/sn2865/pynixconfig)
 
+[![PyPI](https://img.shields.io/pypi/v/pynixconfig)](https://pypi.org/project/pynixconfig/0.1.0/)
+
+[![Docs](https://img.shields.io/readthedocs/pynixconfig.svg)](https://pynixconfig.readthedocs.io/en/latest/)
+
 # Overview
 
-This library will enable beginners to easily configure their UNIX environment for it to look cool.
-It will allow users to configure anything ranging from environment variables, what their terminal looks like,
-credentials, etc.. using a simple python generated user interface.
+This library allows to easily configure a linux terminal. 
+
+The three configurations developed so far:
+file colors
+shell color
+fonts
+
+# Demo
+
+Watch the Demo here: [Youtube](https://www.youtube.com/watch?v=enuFhW7qoJU)
 
 # Installation
 
 pip install pynixconfig
 
 # Using the Library
 
 1. modify your configs in pynixconfig/linuxconfig.py
 
 2. Run the following command in the root directory of project: $ make run
 
 # Instructions
 
 clone repo on your local
-modify color and font in pynixconfig/linuxconfig.py
+modify color and font and shell in pynixconfig/linuxconfig.py
 
 run command: make run
```

### Comparing `pynixconfig-0.1.0/pynixconfig/linuxconfig.py` & `pynixconfig-0.1.1/pynixconfig/linuxconfig.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,20 +40,26 @@
 
 
 def replace_ls_colors(config_string):
     new_line = "LS_COLORS=" + '"{}"'.format(config_string)
     return new_line
 
 
-def main(color, font):
+def bash_shell(color_code):
+    ps1 = r'PS1="\e[0;' + color_code + r'm[\u@\h \W]\$ \e[m "'
+    return ps1
+
+
+def main(color, font, prompt):
     path = "~/.bashrc"
 
     full_path = get_full_path(path)
     color_code = get_color_code(color)
     font_code = get_font_code(font)
+    prompt_code = get_color_code(prompt)
 
     curr_colors = os.popen("echo $LS_COLORS").read()  # make into function?
     print(curr_colors)
     config_string = config(color_code, font_code)
     print(config_string)
 
     bashrc = open(full_path, "r")
@@ -74,15 +80,36 @@
     if exists is False:
         print("does not exist")
         fin_data = add_ls_colors(data, config_string)
         with open(full_path, "w") as file:
             file.write(fin_data)
 
         return fin_data.splitlines()[-1]
+    if prompt != "":
+        with open(full_path, 'a') as file:
+            file.write("\n" + bash_shell(prompt_code))
 
     return replace_ls_colors(config_string)
 
 
 if __name__ == "__main__":
+    '''
+    Possible colors:
+    red
+    green
+    orange
+    blue
+    purple
+    cyan
+    grey
+
+    Possible fonts:
+    bold
+    underlined
+
+    NOTE: To see the changes in the terminal, you will need to restart the terminal
+    '''
+
     color = "cyan"
     font = "bold"
-    main(color, font)
+    prompt = "red"
+    main(color, font, prompt)
```

### Comparing `pynixconfig-0.1.0/pynixconfig/tests/test_all.py` & `pynixconfig-0.1.1/pynixconfig/tests/test_all.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pynixconfig import get_color_code, get_font_code, get_full_path
 from pynixconfig import add_ls_colors, config, main, replace_ls_colors
+from pynixconfig import bash_shell
 import os
 
 
 def test_color_code():
     assert get_color_code("red") == "31"
     assert get_color_code("blue") == "34"
 
@@ -24,9 +25,13 @@
     assert add_ls_colors("", "di=1;31") == '\nLS_COLORS="di=1;31"'
 
 
 def test_replace_ls_colors():
     assert replace_ls_colors("di=1;31") == 'LS_COLORS="di=1;31"'
 
 
+def test_bash_shell():
+    assert bash_shell("32") == r'PS1="\e[0;32m[\u@\h \W]\$ \e[m "'
+
+
 def integration_test():
     assert main("red", "bold") == 'LS_COLORS="di=1;31"'
```

### Comparing `pynixconfig-0.1.0/pynixconfig.egg-info/PKG-INFO` & `pynixconfig-0.1.1/pynixconfig.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynixconfig
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple way to config your terminal colors
 Author-email: Sergio Nahas <sn2865@columbia.edu>
 License: MIT License
         
         Copyright (c) 2023 Sergio Nahas
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -49,31 +49,42 @@
 
 <img src="https://img.shields.io/github/issues/sn2865/pynixconfig" alt="issues"></img>
 
 ![Build Status](https://github.com/sn2865/pynixconfig/actions/workflows/build.yml/badge.svg)
 
 [![codecov](https://codecov.io/gh/sn2865/pynixconfig/branch/main/graph/badge.svg)](https://codecov.io/gh/sn2865/pynixconfig)
 
+[![PyPI](https://img.shields.io/pypi/v/pynixconfig)](https://pypi.org/project/pynixconfig/0.1.0/)
+
+[![Docs](https://img.shields.io/readthedocs/pynixconfig.svg)](https://pynixconfig.readthedocs.io/en/latest/)
+
 # Overview
 
-This library will enable beginners to easily configure their UNIX environment for it to look cool.
-It will allow users to configure anything ranging from environment variables, what their terminal looks like,
-credentials, etc.. using a simple python generated user interface.
+This library allows to easily configure a linux terminal. 
+
+The three configurations developed so far:
+file colors
+shell color
+fonts
+
+# Demo
+
+Watch the Demo here: [Youtube](https://www.youtube.com/watch?v=enuFhW7qoJU)
 
 # Installation
 
 pip install pynixconfig
 
 # Using the Library
 
 1. modify your configs in pynixconfig/linuxconfig.py
 
 2. Run the following command in the root directory of project: $ make run
 
 # Instructions
 
 clone repo on your local
-modify color and font in pynixconfig/linuxconfig.py
+modify color and font and shell in pynixconfig/linuxconfig.py
 
 run command: make run
```

### Comparing `pynixconfig-0.1.0/pyproject.toml` & `pynixconfig-0.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pynixconfig"
 authors = [{name = "Sergio Nahas", email = "sn2865@columbia.edu"}]
 description="Simple way to config your terminal colors"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

