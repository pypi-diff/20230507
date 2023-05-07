# Comparing `tmp/blinkpdf-1.5.tar.gz` & `tmp/blinkpdf-1.6.tar.gz`

## Comparing `blinkpdf-1.5.tar` & `blinkpdf-1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 blinkpdf-1.5/blinkpdf/__init__.py
--rwxr-xr-x   0        0        0     4311 2020-02-02 00:00:00.000000 blinkpdf-1.5/blinkpdf/__main__.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blinkpdf-1.5/.gitignore
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 blinkpdf-1.5/LICENSE
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 blinkpdf-1.5/README.md
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 blinkpdf-1.5/pyproject.toml
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 blinkpdf-1.5/PKG-INFO
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 blinkpdf-1.6/blinkpdf/__init__.py
+-rwxr-xr-x   0        0        0     4258 2020-02-02 00:00:00.000000 blinkpdf-1.6/blinkpdf/__main__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blinkpdf-1.6/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 blinkpdf-1.6/LICENSE
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 blinkpdf-1.6/README.md
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 blinkpdf-1.6/pyproject.toml
+-rw-r--r--   0        0        0     1530 2020-02-02 00:00:00.000000 blinkpdf-1.6/PKG-INFO
```

### Comparing `blinkpdf-1.5/blinkpdf/__main__.py` & `blinkpdf-1.6/blinkpdf/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,22 +7,22 @@
 
 from argparse import ArgumentParser
 from contextlib import contextmanager
 import os
 import subprocess
 import sys
 
-from PyQt5.QtWebEngineWidgets import QWebEnginePage, QWebEngineProfile
-from PyQt5.QtNetwork import QNetworkCookie
-from PyQt5.QtWidgets import (
+from PyQt6.QtNetwork import QNetworkCookie
+from PyQt6.QtWidgets import (
     QApplication,
 )
-from PyQt5.QtWebEngine import QtWebEngine
-from PyQt5.QtWebEngineCore import QWebEngineHttpRequest
-from PyQt5.QtCore import (
+from PyQt6.QtWebEngineCore import (
+    QWebEngineHttpRequest, QWebEnginePage, QWebEngineProfile,
+)
+from PyQt6.QtCore import (
     QUrl, QEventLoop,
 )
 
 
 __all__ = (
     'init',
     'convert',
@@ -38,15 +38,15 @@
 def prepare_loop(sig=None):
     loop = QEventLoop()
     if sig is not None:
         sig.connect(loop.quit)
 
     yield loop
 
-    loop.exec_()
+    loop.exec()
 
 
 class HeadlessPage(QWebEnginePage):
     def javaScriptAlert(self, url, msg):
         pass
 
     def javaScriptConfirm(self, url, msg):
@@ -73,18 +73,19 @@
 
 def convert(args):
     profile = QWebEngineProfile()
     # explicitly pass None 'parent' to use the 2-params ctor
     page = HeadlessPage(profile, None)
 
     settings = page.settings()
-    settings.setAttribute(settings.JavascriptCanOpenWindows, False)
-    settings.setAttribute(settings.WebGLEnabled, False)
-    settings.setAttribute(settings.AutoLoadIconsForPage, False)
-    settings.setAttribute(settings.ShowScrollBars, False)
+    attributes = settings.WebAttribute
+    settings.setAttribute(attributes.JavascriptCanOpenWindows, False)
+    settings.setAttribute(attributes.WebGLEnabled, False)
+    settings.setAttribute(attributes.AutoLoadIconsForPage, False)
+    settings.setAttribute(attributes.ShowScrollBars, False)
 
     qurl = QUrl(args['url'])
     req = QWebEngineHttpRequest(qurl)
 
     for name, value in args.get('headers', ()):
         req.setHeader(name.encode('utf-8'), value.encode('utf-8'))
 
@@ -110,16 +111,14 @@
 
 def init(create_app=True):
     global APP
 
     if QApplication.instance() is None and create_app:
         APP = QApplication(["blinkpdf", "--headless"])
 
-    QtWebEngine.initialize()
-
 
 def parse_cookies(cookiestr):
     name, _, value = cookiestr.partition('=')
     return (name, value)
 
 
 def run_main(args, prepend=None):
```

### Comparing `blinkpdf-1.5/LICENSE` & `blinkpdf-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `blinkpdf-1.5/pyproject.toml` & `blinkpdf-1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Printing",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "PyQt5",
-    "PyQtWebEngine",
+    "PyQt6",
+    "PyQt6-WebEngine",
 ]
 
 [project.scripts]
 blinkpdf = "blinkpdf.__main__:main"
 
 [project.urls]
 Homepage = "https://gitlab.com/hydrargyrum/blinkpdf"
```

### Comparing `blinkpdf-1.5/PKG-INFO` & `blinkpdf-1.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blinkpdf
-Version: 1.5
+Version: 1.6
 Summary: Blink-based webpage-to-pdf converter
 Project-URL: Homepage, https://gitlab.com/hydrargyrum/blinkpdf
 Author-email: Hg <dev@indigo.re>
 License-Expression: Unlicense
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -16,19 +16,27 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Printing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.5
-Requires-Dist: pyqt5
-Requires-Dist: pyqtwebengine
+Requires-Dist: pyqt6
+Requires-Dist: pyqt6-webengine
 Description-Content-Type: text/markdown
 
-BlinkPDF is yet another webpage-to-pdf converter.
+# BlinkPDF is yet another webpage-to-pdf converter
 
-It uses PyQt5 and QtWebEngine (with Blink engine) to do so.
+It uses PyQt6 and QtWebEngine (with Blink engine) to do so.
 
 Pass an URL and an output filename, the page will be retrieved and converted
 to PDF. Additionally, it can be given custom cookies and headers and also
 some javascript code to execute (if needing to perform custom tweaks to
 the page).
+
+## Usage
+
+`blinkpdf [--cookie NAME=VALUE] [--header NAME=VALUE] [--run-script JS_SNIPPET] https://pypi.org/project/blinkpdf/ output.pdf`
+
+## Install
+
+[`pip install blinkpdf`](https://pypi.org/project/blinkpdf/)
```

