# Comparing `tmp/colony_print-0.1.4.tar.gz` & `tmp/colony-print-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/colony_print-0.1.4.tar", last modified: Tue May 16 19:34:26 2017, max compression
+gzip compressed data, was "dist/colony-print-0.2.0.tar", last modified: Sun May  7 15:55:20 2023, max compression
```

## Comparing `colony_print-0.1.4.tar` & `colony-print-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/controllers/
--rw-r--r--   0 travis    (1000) travis    (1000)      285 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/controllers/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      115 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/controllers/base.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2781 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/controllers/document.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2689 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/controllers/node.py
--rw-r--r--   0 travis    (1000) travis    (1000)      779 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/controllers/printer.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/printing/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/printing/binie/
--rw-r--r--   0 travis    (1000) travis    (1000)      263 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/binie/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      866 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/binie/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)      879 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/binie/system.py
--rw-r--r--   0 travis    (1000) travis    (1000)    20630 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/binie/visitor.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/printing/common/
--rw-r--r--   0 travis    (1000) travis    (1000)      111 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/common/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2695 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/common/base.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/printing/manager/
--rw-r--r--   0 travis    (1000) travis    (1000)      448 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2274 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/ast.py
--rw-r--r--   0 travis    (1000) travis    (1000)      870 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)     7540 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/parser.py
--rw-r--r--   0 travis    (1000) travis    (1000)     4300 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/system.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2768 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/manager/visitor.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/printing/pdf/
--rw-r--r--   0 travis    (1000) travis    (1000)      272 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/pdf/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)     1456 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/pdf/exceptions.py
--rw-r--r--   0 travis    (1000) travis    (1000)      973 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/pdf/system.py
--rw-r--r--   0 travis    (1000) travis    (1000)    33542 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/pdf/visitor.py
--rw-r--r--   0 travis    (1000) travis    (1000)      222 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/printing/__init__.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/static/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/static/example/
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/static/example/js/
--rw-r--r--   0 travis    (1000) travis    (1000)     3554 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/static/example/js/main.js
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print/static/example/xml/
--rw-r--r--   0 travis    (1000) travis    (1000)      251 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/static/example/xml/hello.xml
--rw-r--r--   0 travis    (1000) travis    (1000)    26876 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/static/example/xml/money_sale_slip.xml
--rw-r--r--   0 travis    (1000) travis    (1000)      594 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/static/example/print.html
--rw-r--r--   0 travis    (1000) travis    (1000)      206 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/__init__.py
--rw-r--r--   0 travis    (1000) travis    (1000)      534 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/main.py
--rw-r--r--   0 travis    (1000) travis    (1000)     2478 2017-05-16 19:33:41.000000 colony_print-0.1.4/src/colony_print/node.py
-drwxr-xr-x   0 travis    (1000) travis    (1000)        0 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/
--rw-r--r--   0 travis    (1000) travis    (1000)      991 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)     1524 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/SOURCES.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/dependency_links.txt
--rw-r--r--   0 travis    (1000) travis    (1000)        1 2017-05-16 19:34:22.000000 colony_print-0.1.4/src/colony_print.egg-info/not-zip-safe
--rw-r--r--   0 travis    (1000) travis    (1000)       45 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/requires.txt
--rw-r--r--   0 travis    (1000) travis    (1000)       13 2017-05-16 19:34:26.000000 colony_print-0.1.4/src/colony_print.egg-info/top_level.txt
--rw-r--r--   0 travis    (1000) travis    (1000)     1850 2017-05-16 19:33:41.000000 colony_print-0.1.4/setup.py
--rw-r--r--   0 travis    (1000) travis    (1000)      991 2017-05-16 19:34:26.000000 colony_print-0.1.4/PKG-INFO
--rw-r--r--   0 travis    (1000) travis    (1000)       88 2017-05-16 19:34:26.000000 colony_print-0.1.4/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-07 15:55:20.000000 colony-print-0.2.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/js/
+-rw-r--r--   0 root         (0) root         (0)     3555 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/js/main.js
+-rw-r--r--   0 root         (0) root         (0)      594 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/print.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/static/example/xml/
+-rw-r--r--   0 root         (0) root         (0)    26876 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/xml/money_sale_slip.xml
+-rw-r--r--   0 root         (0) root         (0)      251 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/static/example/xml/hello.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/pdf/
+-rw-r--r--   0 root         (0) root         (0)      973 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/system.py
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33615 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/pdf/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/manager/
+-rw-r--r--   0 root         (0) root         (0)     4300 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/system.py
+-rw-r--r--   0 root         (0) root         (0)      870 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2274 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/ast.py
+-rw-r--r--   0 root         (0) root         (0)      448 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/visitor.py
+-rw-r--r--   0 root         (0) root         (0)     7540 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/manager/parser.py
+-rw-r--r--   0 root         (0) root         (0)      222 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/binie/
+-rw-r--r--   0 root         (0) root         (0)      879 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/system.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      263 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20628 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/binie/visitor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/printing/common/
+-rw-r--r--   0 root         (0) root         (0)     2695 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/common/base.py
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/printing/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print/controllers/
+-rw-r--r--   0 root         (0) root         (0)      115 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/base.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/printer.py
+-rw-r--r--   0 root         (0) root         (0)     2794 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/document.py
+-rw-r--r--   0 root         (0) root         (0)      285 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4965 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/controllers/node.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/main.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2474 2023-05-07 15:54:48.000000 colony-print-0.2.0/src/colony_print/node.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:55:20.000000 colony-print-0.2.0/src/colony_print.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 15:55:15.000000 colony-print-0.2.0/src/colony_print.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     2067 2023-05-07 15:54:48.000000 colony-print-0.2.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)     1945 2023-05-07 15:54:48.000000 colony-print-0.2.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     3515 2023-05-07 15:55:20.000000 colony-print-0.2.0/PKG-INFO
```

### Comparing `colony_print-0.1.4/src/colony_print/controllers/document.py` & `colony-print-0.2.0/src/colony_print/controllers/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
 EXAMPLE = "<?xml version=\"1.0\" encoding=\"UTF-8\"?>\
     <printing_document name=\"hello_world\" font=\"Calibri\" font_size=\"9\">\
         <paragraph text_align=\"center\">\
             <line><text>Hello World</text></line>\
         </paragraph>\
     </printing_document>"
-""" Example xml string that should display an hello world
-message using the xml printing language """
+""" Example XML string that should display an hello world
+message using the XML printing language """
 
 class DocumentController(appier.Controller):
 
     def __init__(self, owner, *args, **kwargs):
         appier.Controller.__init__(self, owner, *args, **kwargs)
         self.manager = None
 
@@ -32,25 +32,25 @@
     def example(self, format):
         return self.send_print(EXAMPLE, format)
 
     @appier.route("/documents.<format>", "POST")
     def convert(self, format):
         # retrieves the current request reference and then
         # uses it to retrieve its "raw" data, that should
-        # contain the xml string for the generation of the
+        # contain the XML string for the generation of the
         # of binie result and then sends the value for print
         request = self.get_request()
         data = request.get_data()
         return self.send_print(data, format = format)
 
     def send_print(self, data, format = "binie"):
         # retrieves the various optional fields for printing
         # and then parses them creating the composite values
         # (should include the size tuple)
-        b64 = self.field("base64", False)
+        b64 = self.field("base64", False, cast = bool)
         width = self.field("width", 0.0, cast = float)
         height = self.field("height", 0.0, cast = float)
         has_size = width > 0.0 and width > 0.0
 
         mime = self.get_mime(format, b64 = base64)
         manager = self.get_manager()
```

### Comparing `colony_print-0.1.4/src/colony_print/controllers/printer.py` & `colony-print-0.2.0/src/colony_print/controllers/printer.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,20 @@
         return self.npcolony.get_devices()
 
     @appier.route("/printers/hello", "GET", json = True)
     @appier.ensure(token = "admin")
     def hello(self):
         self.npcolony.print_hello()
 
+    @appier.route("/printers/print", "GET", json = True)
+    @appier.ensure(token = "admin")
+    def print_document_f(self):
+        printer = self.field("printer")
+        return self.print_document(printer)
+
     @appier.route("/printers/<str:printer>/print", ("GET", "POST"), json = True)
     @appier.ensure(token = "admin")
     def print_document(self, printer):
         data_b64 = self.field("data_b64")
         self.npcolony.print_printer_base64(printer, data_b64)
 
     @property
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/binie/exceptions.py` & `colony-print-0.2.0/src/colony_print/printing/binie/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     The invalid context information name class.
     """
 
     def __init__(self, message):
         """
         Constructor of the class.
 
-        @type message: String
-        @param message: The message to be printed.
+        :type message: String
+        :param message: The message to be printed.
         """
 
         PrintingBinieException.__init__(self)
         self.message = message
 
     def __str__(self):
         """
         Returns the string representation of the class.
 
-        @rtype: String
-        @return: The string representation of the class.
+        :rtype: String
+        :return: The string representation of the class.
         """
 
         return "Invalid context information name - %s" % self.message
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/binie/system.py` & `colony-print-0.2.0/src/colony_print/printing/binie/system.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     def print_test(self, options = {}):
         pass
 
     def print_test_image(self, image_path, options = {}):
         pass
 
     def print_language(self, printing_document, options = {}):
-        # creates the pdf printing visitor then sets the
+        # creates the PDF printing visitor then sets the
         # provided printing options in the visitor
         _visitor = visitor.Visitor()
         _visitor.set_options(options)
 
         # accepts the visitor in the printing document,
         # using double visiting mode
         printing_document.accept_double(_visitor)
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/binie/visitor.py` & `colony-print-0.2.0/src/colony_print/printing/binie/visitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,38 +103,38 @@
 
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
-            # an ast node class reference must continue the loop
+            # an AST node class reference must continue the loop
             if not hasattr(self_class_real_element, "ast_node_class"): continue
 
-            # retrieves the ast node class from the current class real element
+            # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     def get_options(self):
         """
         Retrieves the printing options.
 
-        @rtype: Dictionary
-        @return: The printing options.
+        :rtype: Dictionary
+        :return: The printing options.
         """
 
         return self.options
 
     def set_options(self, options):
         """
         Sets the printing options.
 
-        @type options: Dictionary.
-        @param options: The printing options.
+        :type options: Dictionary.
+        :param options: The printing options.
         """
 
         self.options = options
 
     @dispatch_visit()
     def visit(self, node):
         print("unrecognized element node of type " + node.__class__.__name__)
@@ -390,15 +390,15 @@
                 # decodes the image source from the default base 64
                 # encoding to be used for the loading
                 image_source_decoded = base64.b64decode(image_source)
 
                 # creates the image buffer then writes the decoded
                 # image into it and opens the file object with the
                 # created buffer (image loading into structure)
-                image_source_buffer = appier.legacy.StringIO()
+                image_source_buffer = appier.legacy.BytesIO()
                 image_source_buffer.write(image_source_decoded)
                 image_source_buffer.seek(0)
                 bitmap_image = PIL.Image.open(image_source_buffer)
 
             # retrieves the bitmap image width and height
             bitmap_image_width, bitmap_image_height = bitmap_image.size
 
@@ -421,15 +421,15 @@
             elif text_align == "center": text_align_int = 3
 
             # sets the real bitmap image height as the bitmap
             # image height (value copy)
             real_bitmap_image_height = bitmap_image_height
 
             # creates a new string buffer for the image
-            string_buffer = appier.legacy.StringIO()
+            string_buffer = appier.legacy.BytesIO()
 
             # saves the new image into the string buffer and then
             # retrieve the buffer data
             other_image.save(string_buffer, "bmp")
             buffer = string_buffer.getvalue()
 
             # packs the element image element structure containing all the meta
@@ -457,16 +457,16 @@
             self.remove_context(node)
 
     def get_current_position_context(self):
         """
         Retrieves the current position based on the current
         context information.
 
-        @rtype: Tuple
-        @return: The current position base on the current context information
+        :rtype: Tuple
+        :return: The current position base on the current context information
         and applied with the font scale factor.
         """
 
         # retrieves the current position in x and y
         current_position_x, current_position_y = self.current_position
 
         # converts the current position to context
@@ -522,19 +522,19 @@
         return self.context_map[context_name][-1]
 
     def put_context(self, context_name, context_value):
         """
         Puts the given context information in the context
         information map.
 
-        @type context_name: String
-        @param context_name: The name of the context information
+        :type context_name: String
+        :param context_name: The name of the context information
         to be put in the context information map.
-        @type context_value: Object
-        @param context_value: The value of the context information to be put
+        :type context_value: Object
+        :param context_value: The value of the context information to be put
         in the context information map.
         """
 
         if not context_name in self.context_map:
             raise exceptions.InvalidContextInformationName(
                 "the context information name: " + context_name + " is invalid"
             )
@@ -542,19 +542,19 @@
         self.context_map[context_name][-1] = context_value
 
     def has_context(self, context_name):
         """
         Tests if the given context information name exists
         in the current context information map.
 
-        @type context_name: String
-        @param context_name: The context information name
+        :type context_name: String
+        :param context_name: The context information name
         to be tested against the current context information map.
-        @rtype: bool
-        @return: If the context information name exists in the
+        :rtype: bool
+        :return: If the context information name exists in the
         current context information map (and is valid).
         """
 
         # in case the context information name exists in the
         # context information map and is not invalid
         if context_name in self.context_map and\
             self.context_map[context_name]: return True
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/common/base.py` & `colony-print-0.2.0/src/colony_print/printing/common/base.py`

 * *Files identical despite different names*

### Comparing `colony_print-0.1.4/src/colony_print/printing/manager/ast.py` & `colony-print-0.2.0/src/colony_print/printing/manager/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 class AstNode(object):
     """
-    The ast node class, that represents a generic node
-    to be percolated as part of the ast (abstract syntax tree).
+    The AST node class, that represents a generic node
+    to be percolated as part of the AST (abstract syntax tree).
     """
 
     value = None
     """ The value """
 
     indent = False
     """ The indentation level """
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/manager/exceptions.py` & `colony-print-0.2.0/src/colony_print/printing/pdf/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,62 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-class PrintingManagerException(Exception):
+class PrintingPdfException(Exception):
     """
-    The printing manager exception class.
+    The printing PDF exception class.
     """
 
     message = None
     """ The exception's message """
 
-class PrintingPluginNotAvailable(PrintingManagerException):
+class InvalidContextInformationName(PrintingPdfException):
     """
-    The printing plugin not available name class.
+    The invalid context information name class.
     """
 
     def __init__(self, message):
         """
         Constructor of the class.
 
-        @type message: String
-        @param message: The message to be printed.
+        :type message: String
+        :param message: The message to be printed.
         """
 
-        PrintingManagerException.__init__(self)
+        PrintingPdfException.__init__(self)
         self.message = message
 
     def __str__(self):
         """
         Returns the string representation of the class.
 
-        @rtype: String
-        @return: The string representation of the class.
+        :rtype: String
+        :return: The string representation of the class.
         """
 
-        return "Printing plugin not available - %s" % self.message
+        return "Invalid context information name - %s" % self.message
+
+class InvalidFont(PrintingPdfException):
+    """
+    The invalid font class.
+    """
+
+    def __init__(self, message):
+        """
+        Constructor of the class.
+
+        :type message: String
+        :param message: The message to be printed.
+        """
+
+        PrintingPdfException.__init__(self)
+        self.message = message
+
+    def __str__(self):
+        """
+        Returns the string representation of the class.
+
+        :rtype: String
+        :return: The string representation of the class.
+        """
+
+        return "Invalid font - %s" % self.message
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/manager/parser.py` & `colony-print-0.2.0/src/colony_print/printing/manager/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 
         pass
 
     def get_value(self):
         """
         Retrieves the result of the parse
 
-        @rtype: Object
-        @return: The result of the parse
+        :rtype: Object
+        :return: The result of the parse
         """
 
         pass
 
     def parse_element_attributes(self, node, element):
         attributes = node.attributes
 
@@ -76,21 +76,21 @@
     def get_value(self):
         return self.printing_document
 
     def get_build_automation(self):
         return self.printing_document
 
     def load_printing_language_file(self, file):
-        # creates the xml document DOM object
+        # creates the XML document DOM object
         xml_document = xml.dom.minidom.parse(file)
 
         self.load_printing_language(xml_document)
 
     def load_printing_language_string(self, string):
-        # creates the xml document DOM object, the provided
+        # creates the XML document DOM object, the provided
         # string is encoded to avoid possible parsing problems
         string = type(string) == appier.legacy.UNICODE and string.encode(DEFAULT_CHARSET) or string
         xml_document = xml.dom.minidom.parseString(string)
 
         self.load_printing_language(xml_document)
 
     def load_printing_language(self, xml_document):
@@ -217,18 +217,18 @@
 
         return image_structure
 
 def valid_node(node):
     """
     Gets if a node is valid or not for parsing.
 
-    @type node: Node
-    @param node: The Xml node to be validated.
-    @rtype: bool
-    @return: The valid or not valid value.
+    :type node: Node
+    :param node: The Xml node to be validated.
+    :rtype: bool
+    :return: The valid or not valid value.
     """
 
     # in case the node is of type element
     if node.nodeType == xml.dom.minidom.Node.ELEMENT_NODE:
         # returns true (valid)
         return True
     # otherwise
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/manager/system.py` & `colony-print-0.2.0/src/colony_print/printing/manager/system.py`

 * *Files identical despite different names*

### Comparing `colony_print-0.1.4/src/colony_print/printing/manager/visitor.py` & `colony-print-0.2.0/src/colony_print/printing/manager/visitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
-            # an ast node class reference must continue the loop
+            # an AST node class reference must continue the loop
             if not hasattr(self_class_real_element, "ast_node_class"): continue
 
-            # retrieves the ast node class from the current class real element
+            # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     @dispatch_visit()
     def visit(self, node):
         print("unrecognized element node of type " + node.__class__.__name__)
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/pdf/exceptions.py` & `colony-print-0.2.0/src/colony_print/printing/manager/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,36 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
-class PrintingPdfException(Exception):
+class PrintingManagerException(Exception):
     """
-    The printing pdf exception class.
+    The printing manager exception class.
     """
 
     message = None
     """ The exception's message """
 
-class InvalidContextInformationName(PrintingPdfException):
+class PrintingPluginNotAvailable(PrintingManagerException):
     """
-    The invalid context information name class.
+    The printing plugin not available name class.
     """
 
     def __init__(self, message):
         """
         Constructor of the class.
 
-        @type message: String
-        @param message: The message to be printed.
+        :type message: String
+        :param message: The message to be printed.
         """
 
-        PrintingPdfException.__init__(self)
+        PrintingManagerException.__init__(self)
         self.message = message
 
     def __str__(self):
         """
         Returns the string representation of the class.
 
-        @rtype: String
-        @return: The string representation of the class.
+        :rtype: String
+        :return: The string representation of the class.
         """
 
-        return "Invalid context information name - %s" % self.message
-
-class InvalidFont(PrintingPdfException):
-    """
-    The invalid font class.
-    """
-
-    def __init__(self, message):
-        """
-        Constructor of the class.
-
-        @type message: String
-        @param message: The message to be printed.
-        """
-
-        PrintingPdfException.__init__(self)
-        self.message = message
-
-    def __str__(self):
-        """
-        Returns the string representation of the class.
-
-        @rtype: String
-        @return: The string representation of the class.
-        """
-
-        return "Invalid font - %s" % self.message
+        return "Printing plugin not available - %s" % self.message
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/pdf/system.py` & `colony-print-0.2.0/src/colony_print/printing/pdf/system.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 from . import visitor
 
 PRINTING_NAME = "pdf"
-""" The printing name, for the current pdf
+""" The printing name, for the current PDF
 infra-structure (as defined in spec) """
 
 class PrintingPDF(object):
     """
-    The printing pdf class, that is responsible for
-    the handling of the logic for the printing of pdf
-    files based on the xml template language.
+    The printing PDF class, that is responsible for
+    the handling of the logic for the printing of PDF
+    files based on the XML template language.
     """
 
     def get_name(self):
         return PRINTING_NAME
 
     def print_test(self, options = {}):
         pass
 
     def print_test_image(self, image_path, options = {}):
         pass
 
     def print_language(self, printing_document, options = {}):
-        # creates the pdf printing visitor then sets the
+        # creates the PDF printing visitor then sets the
         # provided printing options in the visitor
         _visitor = visitor.Visitor()
         _visitor.set_options(options)
 
         # accepts the visitor in the printing document,
         # using double visiting mode
         printing_document.accept_double(_visitor)
```

### Comparing `colony_print-0.1.4/src/colony_print/printing/pdf/visitor.py` & `colony-print-0.2.0/src/colony_print/printing/pdf/visitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from . import exceptions
 
 from ..common.base import *
 from ..manager.ast import *
 
 try:
     import reportlab.lib.units
-except:
+except ImportError:
     INCH = 72.0
     CM = INCH / 2.54
 else:
     INCH = reportlab.lib.units.inch
     CM = reportlab.lib.units.cm
 
 FONT_SCALE_FACTOR = 1
@@ -70,15 +70,15 @@
 to created the full font name """
 
 DEFAULT_ENCODER = "utf-8"
 """ The default encoder """
 
 SCALE = CM
 """ The scale value to be used in the conversion
-of the centimeter value into the pdf point """
+of the centimeter value into the PDF point """
 
 TWIP_SCALE = 0.001763889
 """ The scale factor to convert a twip value into
 a centimeter base value """
 
 A4_PAPER = (21.0 * SCALE, 29.7 * SCALE)
 """ The default size (dimensions) for an a4 paper
@@ -96,16 +96,16 @@
 
 FONT_PATHS = ("", "~/.fonts/", "/usr/share/fonts/truetype/")
 """ The set of base paths to be used for searching
 for fonts on the current system """
 
 class Visitor(object):
     """
-    The visitor class for the pdf printing infra-structure
-    this visitor should be able to generate a pdf file
+    The visitor class for the PDF printing infra-structure
+    this visitor should be able to generate a PDF file
     using the reportlab library as basics.
     """
 
     node_method_map = {}
     """ The node method map """
 
     visit_childs = True
@@ -118,36 +118,36 @@
     """ The visit index, for multiple visits """
 
     options = {}
     """ The printing options """
 
     canvas = None
     """ The reference to the canvas object to be used
-    for manipulating the various pdf elements """
+    for manipulating the various PDF elements """
 
     size = None
     """ The size of the document to be printed, this
-    is the width and height measured in pdf points """
+    is the width and height measured in PDF points """
 
     width = None
     """ The width of the document to be printed, this
-    is the width measured in pdf points """
+    is the width measured in PDF points """
 
     height = None
     """ The height of the document to be printed, this
-    is the height measured in pdf points """
+    is the height measured in PDF points """
 
     single = False
     """ If the document to be parsed is considered to be
     single page only or multi page, this is relevant for
     the fixed/absolute positioning using blocks  """
 
     current_position = None
     """ The current position in the document measured
-    as pdf points """
+    as PDF points """
 
     fonts = {}
     """ The map containing the various loaded fonts
     to avoid multiple loading of fonts (redundancy is
     removed to avoid errors) """
 
     context_map = {}
@@ -178,38 +178,38 @@
 
         # iterates over all the name of the elements
         for self_class_element in self_class_elements:
             # retrieves the real element value
             self_class_real_element = getattr(self_class, self_class_element)
 
             # in case the current class real element does not contain
-            # an ast node class reference must continue the loop
+            # an AST node class reference must continue the loop
             if not hasattr(self_class_real_element, "ast_node_class"): continue
 
-            # retrieves the ast node class from the current class real element
+            # retrieves the AST node class from the current class real element
             # and sets it in the node method map
             ast_node_class = getattr(self_class_real_element, "ast_node_class")
             self.node_method_map[ast_node_class] = self_class_real_element
 
     def get_options(self):
         """
         Retrieves the printing options.
 
-        @rtype: Dictionary
-        @return: The printing options.
+        :rtype: Dictionary
+        :return: The printing options.
         """
 
         return self.options
 
     def set_options(self, options):
         """
         Sets the printing options.
 
-        @type options: Dictionary.
-        @param options: The printing options.
+        :type options: Dictionary.
+        :param options: The printing options.
         """
 
         self.options = options
 
     @dispatch_visit()
     def visit(self, node):
         print("unrecognized element node of type " + node.__class__.__name__)
@@ -235,15 +235,15 @@
 
         # in case it's the first visit
         if self.visit_index == 0:
             # adds the node as the context information
             self.add_context(node)
 
             # retrieves both the file (buffer) to be used for the output
-            # of the pdf file contents and the expected size for the pdf
+            # of the PDF file contents and the expected size for the PDF
             # document, in case no size is provided a default one is used
             file = self.options["file"]
             size = self.options.get("size", PAPER_SIZE)
 
             # tries to retrieve the document width and height values and
             # converts them into the proper integer values, these values
             # are mostly available for single page operations
@@ -263,15 +263,15 @@
             # unpacks the size tuple into the width and height
             # components and sets the tuple containing both values
             # as the size to be used for the document
             self.width, self.height = size
             self.size = (self.width, self.height)
 
             # creates the canvas object to be used as the primary
-            # entry point for operation on the pdf
+            # entry point for operation on the PDF
             self.canvas = reportlab.pdfgen.canvas.Canvas(
                 file,
                 pagesize = self.size
             )
 
             # sets the initial position so that the "virtual" cursor
             # position is situated at the top left corner of the page
@@ -279,15 +279,15 @@
                 0, self.height
             )
 
         # in case it's the second visit
         elif self.visit_index == 1:
             # saves the final canvas structure flushing the data to
             # the associated file object, this is considered the final
-            # operation for the creation of the pdf file
+            # operation for the creation of the PDF file
             self.canvas.save()
 
             # removes the context information
             self.remove_context(node)
 
     @visited(Block)
     def visit_block(self, node):
@@ -364,15 +364,15 @@
             margin_right = int(self.get_context("margin_right", "0"))
             position_x = int(self.get_context("x", "0"))
             position_y = int(self.get_context("y", "0"))
             block_width = int(self.get_context("width", "0"))
             block_height = int(self.get_context("height", "0"))
 
             # converts the various block related values from their original
-            # twip based value into the pdf point value to be used in print
+            # twip based value into the PDF point value to be used in print
             position_x = int(position_x * TWIP_SCALE * SCALE)
             position_y = int(position_y * TWIP_SCALE * SCALE)
             block_width = int(block_width * TWIP_SCALE * SCALE)
             block_height = int(block_height * TWIP_SCALE * SCALE)
 
             # verifies if the current context is of type block, so that
             # the proper absolute positions are going to be used instead
@@ -398,15 +398,15 @@
             # according to the printing language specification, the value
             # is rounded to one decimal place so that no major visual
             # rounding problems occur
             font_size_r = round(font_size / 1.2, 1)
 
             # retrieves the proper suffix for the requested font style
             # and uses it to create the complete font name ensuring that
-            # it's currently loaded in the pdf context
+            # it's currently loaded in the PDF context
             suffix = FONT_SUFFIX_MAP.get(font_style, "")
             font_name_c = font_name + suffix
             self.ensure_font(font_name_c)
 
             # sets the complete computed font in the current canvas context
             # note that the leading value is overriden to avoid font sizing
             # problems in accordance with the printing language specification,
@@ -505,15 +505,15 @@
             text_align = self.get_context("text_align")
             position_x = int(self.get_context("x", "0"))
             position_y = int(self.get_context("y", "0"))
             block_width = int(self.get_context("width", "0"))
             block_height = int(self.get_context("height", "0"))
 
             # converts the various block related values from their original
-            # twip based value into the pdf point value to be used in print
+            # twip based value into the PDF point value to be used in print
             position_x = int(position_x * TWIP_SCALE * SCALE)
             position_y = int(position_y * TWIP_SCALE * SCALE)
             block_width = int(block_width * TWIP_SCALE * SCALE)
             block_height = int(block_height * TWIP_SCALE * SCALE)
 
             # verifies if the current context is of type block, so that
             # the proper absolute positions are going to be used instead
@@ -548,15 +548,15 @@
                 # decodes the image source from the default base 64
                 # encoding to be used for the loading
                 image_source_decoded = base64.b64decode(image_source)
 
                 # creates the image buffer then writes the decoded
                 # image into it and opens the file object with the
                 # created buffer (image loading into structure)
-                image_source_buffer = appier.legacy.StringIO()
+                image_source_buffer = appier.legacy.BytesIO()
                 image_source_buffer.write(image_source_decoded)
                 image_source_buffer.seek(0)
                 bitmap_image = PIL.Image.open(image_source_buffer)
 
             # retrieves the bitmap image width and height
             bitmap_image_width, bitmap_image_height = bitmap_image.size
 
@@ -617,22 +617,22 @@
         Ensures that the provided vertical position is valid for
         the current page (no overflow) in case it's not a new page
         is created and the returned position is the new one.
 
         The calculation of the new vertical position takes into
         account the provided offset value.
 
-        @type y_position: float
-        @param y_position: The vertical position as a pdf point value
+        :type y_position: float
+        :param y_position: The vertical position as a PDF point value
         to be validated against the current page metrics.
-        @type offset: float
-        @param offset: The vertical offset to be applied to the new's
+        :type offset: float
+        :param offset: The vertical offset to be applied to the new's
         page vertical value in case a new page is created.
-        @rtype: float
-        @return: The resulting vertical position taking into account
+        :rtype: float
+        :return: The resulting vertical position taking into account
         creation of new pages.
         """
 
         # in case the current document in parsing has been marked
         # as single page oriented (absolute positioning), there's
         # no need to verify for new page creation
         if self.single: return y_position
@@ -661,26 +661,26 @@
         # caller method
         self.canvas.showPage()
         return y_position
 
     def ensure_font(self, font_name, file_path = None):
         """
         Ensures that the font is present in the current
-        canvas object, loading it into the pdf context
+        canvas object, loading it into the PDF context
         in case it's required.
 
         The provided file path may be an absolute path
         or a relative (file name) to the system's default
         font directory.
 
-        @type font_name: String
-        @param font_name: The name of the font to be ensured
+        :type font_name: String
+        :param font_name: The name of the font to be ensured
         to be loaded in the current context.
-        @type file_path: String
-        @param file_path: The path to the true type font file
+        :type file_path: String
+        :param file_path: The path to the true type font file
         that should be loaded for the font (may be a relative
         or absolute path)
         """
 
         import reportlab.pdfbase.ttfonts
         import reportlab.pdfbase.pdfmetrics
 
@@ -696,15 +696,15 @@
         file_path = file_path or font_name_l + ".ttf"
 
         # sets the error flag as true by default the loading of
         # the font is not possible in case one of the steps
         # completes the error flag is unset
         error = True
 
-        # iterate over all the font path trying to find a path
+        # iterates over all the font paths trying to find a path
         # that can correctly load the requested font
         for font_path in FONT_PATHS:
             try:
                 # creates the complete font path with the current
                 # base path in iteration and the font name in case
                 # the font path is empty the default system wide
                 # search will be used (varies from system to system)
@@ -712,16 +712,19 @@
                 file_path_f = os.path.expanduser(file_path_f)
 
                 # creates the font structure for the font name and path
                 # and the registers it in the the current report lab
                 # metrics (to be used in further operations)
                 font = reportlab.pdfbase.ttfonts.TTFont(font_name, file_path_f)
                 reportlab.pdfbase.pdfmetrics.registerFont(font)
-            except: continue
-            else: error = False; break
+            except Exception:
+                continue
+            else:
+                error = False
+                break
 
         # in case the error flag is set raises the invalid font
         # exception, indicating that it was not possible to load
         # the associated font file
         if error: raise exceptions.InvalidFont(
             "not possible to load '%s' - '%s'" % (font_name, file_path)
         )
@@ -732,16 +735,16 @@
         self.fonts[font_name] = file_path
 
     def get_current_position_context(self):
         """
         Retrieves the current position based on the current
         context information.
 
-        @rtype: Tuple
-        @return: The current position base on the current context information
+        :rtype: Tuple
+        :return: The current position base on the current context information
         and applied with the font scale factor.
         """
 
         # retrieves the current position in x and y
         current_position_x, current_position_y = self.current_position
 
         # converts the current position to context
@@ -759,21 +762,21 @@
             raise exceptions.InvalidContextInformationName(
                 "the context information name: " + context_name + " is invalid"
             )
 
         return self.peek_context(context_name)
 
     def add_context(self, node):
-        valid_attributes = [(value, getattr(node, value)) for value in dir(node) if value not in EXCLUSION_LIST]
+        valid_attributes = [(value, getattr(node, value)) for value in dir(node) if not value in EXCLUSION_LIST]
 
         for valid_attribute_name, valid_attribute_value in valid_attributes:
             self.push_context(valid_attribute_name, valid_attribute_value)
 
     def remove_context(self, node):
-        valid_attribute_names = [value for value in dir(node) if value not in EXCLUSION_LIST]
+        valid_attribute_names = [value for value in dir(node) if not value in EXCLUSION_LIST]
 
         for valid_attribute_name in valid_attribute_names:
             self.pop_context(valid_attribute_name)
 
     def push_context(self, context_name, context_value):
         if not context_name in self.context_map:
             self.context_map[context_name] = []
@@ -797,19 +800,19 @@
         return self.context_map[context_name][-1]
 
     def put_context(self, context_name, context_value):
         """
         Puts the given context information in the context
         information map.
 
-        @type context_name: String
-        @param context_name: The name of the context information
+        :type context_name: String
+        :param context_name: The name of the context information
         to be put in the context information map.
-        @type context_value: Object
-        @param context_value: The value of the context information to be put
+        :type context_value: Object
+        :param context_value: The value of the context information to be put
         in the context information map.
         """
 
         if not context_name in self.context_map:
             raise exceptions.InvalidContextInformationName(
                 "the context information name: " + context_name + " is invalid"
             )
@@ -817,19 +820,19 @@
         self.context_map[context_name][-1] = context_value
 
     def has_context(self, context_name):
         """
         Tests if the given context information name exists
         in the current context information map.
 
-        @type context_name: String
-        @param context_name: The context information name
+        :type context_name: String
+        :param context_name: The context information name
         to be tested against the current context information map.
-        @rtype: bool
-        @return: If the context information name exists in the
+        :rtype: bool
+        :return: If the context information name exists in the
         current context information map (and is valid).
         """
 
         # in case the context information name exists in the
         # context information map and is not invalid
         if context_name in self.context_map and\
             self.context_map[context_name]: return True
```

### Comparing `colony_print-0.1.4/src/colony_print/static/example/js/main.js` & `colony-print-0.2.0/src/colony_print/static/example/js/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -28,15 +28,15 @@
     var data = {
         base64: 1
     };
 
     // in case the target format is pdf extra values must be added
     // to the data map containin the size of the paper provided by
     // the default printer (for correct pdf generation)
-    if (format == "pdf") {
+    if (format === "pdf") {
         sizes(gateway, data);
     }
 
     // converts the data map that contains extra arguments into
     // a series of key value associations that are going to be
     // appended to the current url
     var extra = serialize(data);
```

### Comparing `colony_print-0.1.4/src/colony_print/static/example/xml/money_sale_slip.xml` & `colony-print-0.2.0/src/colony_print/static/example/xml/money_sale_slip.xml`

 * *Files identical despite different names*

### Comparing `colony_print-0.1.4/src/colony_print/static/example/print.html` & `colony-print-0.2.0/src/colony_print/static/example/print.html`

 * *Files identical despite different names*

### Comparing `colony_print-0.1.4/src/colony_print/main.py` & `colony-print-0.2.0/src/colony_print/main.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import appier_extras
 
 class ColonyPrintApp(appier.APIApp):
 
     def __init__(self, *args, **kwargs):
         appier.APIApp.__init__(
             self,
-            name = "colony_print",
+            name = "colony-print",
             parts = (
                 appier_extras.AdminPart,
             ),
             *args, **kwargs
         )
         self.nodes = dict()
         self.jobs = dict()
```

### Comparing `colony_print-0.1.4/src/colony_print/node.py` & `colony-print-0.2.0/src/colony_print/node.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
                 jobs = appier.get(
                     base_url + "nodes/%s/jobs" % node_id,
                     headers = headers,
                     timeout = 600
                 )
                 logging.info("Retrieved %d jobs for node '%s'" % (len(jobs), node_id))
                 for job in jobs: self.print_job(job)
-            except BaseException as exception:
+            except Exception as exception:
                 logging.info("Exception while looping '%s'" % str(exception))
                 logging.info("Sleeping for %.2f seconds" % self.sleep_time)
                 time.sleep(self.sleep_time)
 
     def print_job(self, job):
         data_b64 = job["data_b64"]
         name = job.get("name", "undefined")
```

### Comparing `colony_print-0.1.4/src/colony_print.egg-info/SOURCES.txt` & `colony-print-0.2.0/src/colony_print.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+README.md
 setup.cfg
 setup.py
 src/colony_print/__init__.py
 src/colony_print/main.py
 src/colony_print/node.py
 src/colony_print.egg-info/PKG-INFO
 src/colony_print.egg-info/SOURCES.txt
@@ -27,13 +28,11 @@
 src/colony_print/printing/manager/parser.py
 src/colony_print/printing/manager/system.py
 src/colony_print/printing/manager/visitor.py
 src/colony_print/printing/pdf/__init__.py
 src/colony_print/printing/pdf/exceptions.py
 src/colony_print/printing/pdf/system.py
 src/colony_print/printing/pdf/visitor.py
-src/colony_print/static/example/js
 src/colony_print/static/example/print.html
-src/colony_print/static/example/xml
 src/colony_print/static/example/js/main.js
 src/colony_print/static/example/xml/hello.xml
 src/colony_print/static/example/xml/money_sale_slip.xml
```

### Comparing `colony_print-0.1.4/setup.py` & `colony-print-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/python
 # -*- coding: utf-8 -*-
 
 import os
 import setuptools
 
 setuptools.setup(
-    name = "colony_print",
-    version = "0.1.4",
+    name = "colony-print",
+    version = "0.2.0",
     author = "Hive Solutions Lda.",
     author_email = "development@hive.pt",
     description = "Colony Print Infra-structure",
     license = "Apache License, Version 2.0",
     keywords = "colony print native",
-    url = "http://colony_print.hive.pt",
+    url = "http://colony-print.hive.pt",
     zip_safe = False,
     packages = [
         "colony_print",
         "colony_print.controllers",
         "colony_print.printing",
         "colony_print.printing.binie",
         "colony_print.printing.common",
@@ -32,15 +32,15 @@
             "static/example/*",
             "static/example/js/*",
             "static/example/xml/*"
         ]
     },
     install_requires = [
         "appier",
-        "appier_extras",
+        "appier-extras",
         "jinja2",
         "pillow",
         "reportlab"
     ],
     classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Topic :: Utilities",
@@ -51,10 +51,13 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.0",
         "Programming Language :: Python :: 3.1",
         "Programming Language :: Python :: 3.2",
         "Programming Language :: Python :: 3.3",
         "Programming Language :: Python :: 3.4",
         "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6"
-    ]
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7"
+    ],
+    long_description = open(os.path.join(os.path.dirname(__file__), "README.md"), "rb").read().decode("utf-8"),
+    long_description_content_type = "text/markdown"
 )
```

