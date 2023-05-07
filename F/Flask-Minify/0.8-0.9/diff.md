# Comparing `tmp/Flask-Minify-0.8.tar.gz` & `tmp/Flask-Minify-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-Minify-0.8.tar", last modified: Sat Jun 30 16:45:49 2018, max compression
+gzip compressed data, was "dist/Flask-Minify-0.9.tar", last modified: Tue Aug 14 15:49:58 2018, max compression
```

## Comparing `Flask-Minify-0.8.tar` & `Flask-Minify-0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-06-30 16:45:49.000000 Flask-Minify-0.8/
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)      950 2018-06-30 16:45:49.000000 Flask-Minify-0.8/PKG-INFO
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)     2159 2018-06-29 01:49:09.000000 Flask-Minify-0.8/README.md
-drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)      950 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/PKG-INFO
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)       28 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/requires.txt
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)        1 2018-06-30 16:45:43.000000 Flask-Minify-0.8/Flask_Minify.egg-info/not-zip-safe
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)      267 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/SOURCES.txt
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)       20 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/top_level.txt
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)        1 2018-06-30 16:45:49.000000 Flask-Minify-0.8/Flask_Minify.egg-info/dependency_links.txt
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)      190 2018-06-30 16:45:49.000000 Flask-Minify-0.8/setup.cfg
-drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-06-30 16:45:49.000000 Flask-Minify-0.8/flask_minify/
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)     2745 2018-06-10 04:57:13.000000 Flask-Minify-0.8/flask_minify/__init__.py
--rw-r--r--   0 mrf3      (1000) mrf3      (1001)     1330 2018-06-30 16:45:04.000000 Flask-Minify-0.8/setup.py
+drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-08-14 15:49:58.000000 Flask-Minify-0.9/
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)      950 2018-08-14 15:49:58.000000 Flask-Minify-0.9/PKG-INFO
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)     2254 2018-08-14 15:43:18.000000 Flask-Minify-0.9/README.md
+drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)      950 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/PKG-INFO
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)       28 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/requires.txt
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)        1 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/not-zip-safe
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)      267 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/SOURCES.txt
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)       20 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/top_level.txt
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)        1 2018-08-14 15:49:58.000000 Flask-Minify-0.9/Flask_Minify.egg-info/dependency_links.txt
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)      190 2018-08-14 15:49:58.000000 Flask-Minify-0.9/setup.cfg
+drwxr-xr-x   0 mrf3      (1000) mrf3      (1001)        0 2018-08-14 15:49:58.000000 Flask-Minify-0.9/flask_minify/
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)     3246 2018-08-14 15:43:03.000000 Flask-Minify-0.9/flask_minify/__init__.py
+-rw-r--r--   0 mrf3      (1000) mrf3      (1001)     1330 2018-08-14 15:18:12.000000 Flask-Minify-0.9/setup.py
```

### Comparing `Flask-Minify-0.8/PKG-INFO` & `Flask-Minify-0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Flask-Minify
-Version: 0.8
+Version: 0.9
 Summary: flask extension to minify html, css, js and less
 Home-page: https://github.com/mrf345/flask_minify/
 Author: Mohamed Feddad
 Author-email: mrf345@gmail.com
 License: MIT
-Download-URL: https://github.com/mrf345/flask_minify/archive/0.7.tar.gz
+Download-URL: https://github.com/mrf345/flask_minify/archive/0.8.tar.gz
 Description: 
         Flask-Minify
         -------------
         
         A Flask extension to minify flask response for html,
         javascript, css and less compilation as well.
```

### Comparing `Flask-Minify-0.8/README.md` & `Flask-Minify-0.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -54,22 +54,24 @@
 ## Options:
 ```python
 def __init__(self,
   app=None,
   html=True,
   js=False,
   cssless=True,
-  cache=True):
+  cache=True,
+  fail_safe=True):
   """
     A Flask extension to minify flask response for html,
     javascript, css and less.
     @param: app Flask app instance to be passed (default:None).
     @param: js To minify the css output (default:False).
     @param: cssless To minify spaces in css (default:True).
     @param: cache To cache minifed response with hash (default: True).
+    @param: fail_safe to avoid raising error while minifying (default True).
   """
 ```
 
 ## Credit:
 > - [htmlmin][1322354e]: HTML python minifier.
 > - [lesscpy][1322353e]: Python less compiler and css minifier.
 > - [jsmin][1322355e]: JavaScript python minifier.
```

### Comparing `Flask-Minify-0.8/Flask_Minify.egg-info/PKG-INFO` & `Flask-Minify-0.9/Flask_Minify.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: Flask-Minify
-Version: 0.8
+Version: 0.9
 Summary: flask extension to minify html, css, js and less
 Home-page: https://github.com/mrf345/flask_minify/
 Author: Mohamed Feddad
 Author-email: mrf345@gmail.com
 License: MIT
-Download-URL: https://github.com/mrf345/flask_minify/archive/0.7.tar.gz
+Download-URL: https://github.com/mrf345/flask_minify/archive/0.8.tar.gz
 Description: 
         Flask-Minify
         -------------
         
         A Flask extension to minify flask response for html,
         javascript, css and less compilation as well.
```

### Comparing `Flask-Minify-0.8/flask_minify/__init__.py` & `Flask-Minify-0.9/flask_minify/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,31 @@
 from htmlmin import minify as minifyHtml
 from hashlib import md5
 
 
 class minify(object):
     def __init__(self, app=None,
         html=True, js=False,
-        cssless=True, cache=True):
+        cssless=True, cache=True,
+        fail_safe=True):
         """
         A Flask extension to minify flask response for html,
         javascript, css and less.
         @param: app Flask app instance to be passed (default:None).
         @param: js To minify the css output (default:False).
         @param: cssless To minify spaces in css (default:True).
         @param: cache To cache minifed response with hash (default: True).
+        @param: fail_safe to avoid raising error while minifying (default True).
         """
         self.app = app
         self.html = html
         self.js = js
         self.cssless = cssless
         self.cache = cache
+        self.fail_safe = fail_safe
         self.history = {} # where cache hash and compiled response stored 
         if self.app is None:
             raise(AttributeError("minify(app=) requires Flask app instance"))
         for arg in ['cssless', 'js', 'html', 'cache']:
             if not isinstance(eval(arg), bool):
                 raise(TypeError("minify(" + arg + "=) requires True or False"))
         self.app.after_request(self.toLoopTag)
@@ -48,19 +51,27 @@
                         toReplace = text.split(
                             '<' + tag, i
                         )[i].split(
                             '</' + tag + '>'
                         )[0].split(
                             '>', 1
                         )[1]
-                        text = text.replace(
-                            toReplace,
-                            compile(StringIO(toReplace),
-                            minify=True, xminify=True
-                            ) if tag == 'style' else jsmin(toReplace
-                            ).replace('\n', ';')
-                        ) if len(toReplace) > 2 else text
+                        result = None
+                        try:
+                            result = text.replace(
+                                toReplace,
+                                compile(StringIO(toReplace),
+                                minify=True, xminify=True
+                                ) if tag == 'style' else jsmin(toReplace
+                                ).replace('\n', ';')
+                            ) if len(toReplace) > 2 else text
+                            text = result
+                        except Exception as e:
+                            if self.fail_safe:
+                                text = result or text
+                            else:
+                                raise e
             finalResp = minifyHtml(text) if self.html else text
             response.set_data(finalResp)
             if self.cache:
                 self.history[forHash] = finalResp
         return response
```

### Comparing `Flask-Minify-0.8/setup.py` & `Flask-Minify-0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 javascript, css and less compilation as well.
 
 """
 from setuptools import setup
 
 setup(
     name='Flask-Minify',
-    version='0.8',
+    version='0.9',
     url='https://github.com/mrf345/flask_minify/',
-    download_url='https://github.com/mrf345/flask_minify/archive/0.7.tar.gz',
+    download_url='https://github.com/mrf345/flask_minify/archive/0.8.tar.gz',
     license='MIT',
     author='Mohamed Feddad',
     author_email='mrf345@gmail.com',
     description='flask extension to minify html, css, js and less',
     long_description=__doc__,
     py_modules=['minify'],
     packages=['flask_minify'],
```

