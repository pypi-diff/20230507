# Comparing `tmp/password-generator-lib-0.1.0.tar.gz` & `tmp/password-generator-lib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\password-generator-lib-0.1.0.tar", last modified: Sun May  7 12:24:46 2023, max compression
+gzip compressed data, was "dist\password-generator-lib-1.0.0.tar", last modified: Sun May  7 12:33:01 2023, max compression
```

## Comparing `password-generator-lib-0.1.0.tar` & `password-generator-lib-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 12:24:46.212558 password-generator-lib-0.1.0/
--rw-rw-rw-   0        0        0      262 2023-05-07 12:24:46.211548 password-generator-lib-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1861 2023-05-07 12:18:48.000000 password-generator-lib-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-07 12:24:46.209546 password-generator-lib-0.1.0/password_generator_lib.egg-info/
--rw-rw-rw-   0        0        0      262 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      157 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 12:24:46.000000 password-generator-lib-0.1.0/password_generator_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-07 12:24:46.213551 password-generator-lib-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      817 2023-05-07 12:23:36.000000 password-generator-lib-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:33:01.689641 password-generator-lib-1.0.0/
+-rw-rw-rw-   0        0        0     2853 2023-05-07 12:33:01.688632 password-generator-lib-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1861 2023-05-07 12:18:48.000000 password-generator-lib-1.0.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 12:33:01.659629 password-generator-lib-1.0.0/password_generator/
+-rw-rw-rw-   0        0        0        0 2023-05-07 12:32:47.000000 password-generator-lib-1.0.0/password_generator/__init__.py
+-rw-rw-rw-   0        0        0     7803 2023-05-07 12:12:47.000000 password-generator-lib-1.0.0/password_generator/generator.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:33:01.685651 password-generator-lib-1.0.0/password_generator_lib.egg-info/
+-rw-rw-rw-   0        0        0     2853 2023-05-07 12:33:01.000000 password-generator-lib-1.0.0/password_generator_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-05-07 12:33:01.000000 password-generator-lib-1.0.0/password_generator_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:33:01.000000 password-generator-lib-1.0.0/password_generator_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      157 2023-05-07 12:33:01.000000 password-generator-lib-1.0.0/password_generator_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-07 12:33:01.000000 password-generator-lib-1.0.0/password_generator_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 12:33:01.689641 password-generator-lib-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1004 2023-05-07 12:32:59.000000 password-generator-lib-1.0.0/setup.py
```

### Comparing `password-generator-lib-0.1.0/README.md` & `password-generator-lib-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `password-generator-lib-0.1.0/setup.py` & `password-generator-lib-1.0.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 
-setup(
-    name='password-generator-lib',
-    version='0.1.0',
-    description='A library for generating secure passwords',
-    author='Mahammad Salimov',
-    author_email='salimovm.7@gmail.com',
-    packages=find_packages(),
-    install_requires=["black==23.3.0",
-                      "click==8.1.3",
-                      "colorama==0.4.6",
-                      "mypy-extensions==1.0.0",
-                      "packaging==23.1",
-                      "pathspec==0.11.1",
-                      "platformdirs==3.5.0",
-                      "tomli==2.0.1",
-                      "typing-extensions==4.5.0",
-                      ],
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
 
-    entry_points={
-        'console_scripts': [
-            'password-generator=generator:main'
-        ]
-    }
+setup(
+    name="password-generator-lib",
+    version="1.0.0",
+    description="A library for generating secure passwords",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="https://github.com/salimovm/password-generator",
+    author="Mahammad Salimov",
+    author_email="salimovm.7@gmail.com",
+    license="MIT",
+    packages=["password_generator"],
+    install_requires=[
+        "black==23.3.0",
+        "click==8.1.3",
+        "colorama==0.4.6",
+        "mypy-extensions==1.0.0",
+        "packaging==23.1",
+        "pathspec==0.11.1",
+        "platformdirs==3.5.0",
+        "tomli==2.0.1",
+        "typing-extensions==4.5.0",
+    ],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
 )
```

