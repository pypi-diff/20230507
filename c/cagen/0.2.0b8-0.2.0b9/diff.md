# Comparing `tmp/cagen-0.2.0b8.tar.gz` & `tmp/cagen-0.2.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0b8.tar", last modified: Fri May  5 16:51:47 2023, max compression
+gzip compressed data, was "cagen-0.2.0b9.tar", last modified: Sun May  7 13:42:30 2023, max compression
```

## Comparing `cagen-0.2.0b8.tar` & `cagen-0.2.0b9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:51:47.981975 cagen-0.2.0b8/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b8/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:51:47.981975 cagen-0.2.0b8/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b8/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-05 16:51:33.000000 cagen-0.2.0b8/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 16:51:47.981975 cagen-0.2.0b8/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:51:47.978642 cagen-0.2.0b8/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:51:47.978642 cagen-0.2.0b8/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b8/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     5256 2023-05-05 16:51:26.000000 cagen-0.2.0b8/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b8/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:51:47.978642 cagen-0.2.0b8/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b8/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b8/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b8/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b8/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:51:47.978642 cagen-0.2.0b8/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 16:51:47.000000 cagen-0.2.0b8/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.880965 cagen-0.2.0b9/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b9/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-07 13:42:30.880965 cagen-0.2.0b9/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b9/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-07 13:42:25.000000 cagen-0.2.0b9/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-07 13:42:30.880965 cagen-0.2.0b9/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b9/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     5914 2023-05-07 13:42:03.000000 cagen-0.2.0b9/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b9/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.880965 cagen-0.2.0b9/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b9/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b9/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b9/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b9/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0b8/PKG-INFO` & `cagen-0.2.0b9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b8
+Version: 0.2.0b9
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0b8/README.md` & `cagen-0.2.0b9/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b8/pyproject.toml` & `cagen-0.2.0b9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.beta-8"
+version = "0.2.0.beta-9"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0b8/src/cagen/cmd.py` & `cagen-0.2.0b9/src/cagen/cmd.py`

 * *Files 16% similar despite different names*

```diff
@@ -59,22 +59,24 @@
 
     maketemplate = """
 # Default template
 TMPHTML5 = templates/schema.tmpl
 TMPLIST = templates/list.md.tmpl
 
 # Select all markdowns file except index.md
-MARKDOWNS = $(shell find . -type f -name "*.md" ! -name "index.md")
+MARKDOWNS = $(shell find . -type f -name "*.md" ! -name "index.md" ! -name "README.md")
+## List them as comma-separated and quotating list
+LISTMD = '"${shell echo $(MARKDOWNS) | sed 's/ /", "/g')}"'
 
 # Replace the extension.
 # By default HTML5
 MARKDOWNS_HTML5 = $(MARKDOWNS:.md=.html)
 
 # Extra metadata. Use if you want and edit freely
-REPOSITORY = "https://git.sr.ht/~somenxavierb/cmpalgorithms"
+REPOSITORY = "https://repo.or.cz/cagen.git"
 REVISIONNUMBER = $(shell git log --format=oneline $<  | wc -l)
 
 # Commands
 
 SSG = cagen
 SSGLIST = cagen-list
 
@@ -82,36 +84,44 @@
 
 .PHONY: all clean
 
 all: $(MARKDOWNS_HTML5)
 
 # .MD.HTML -> .HTML
 %.html: %.md
-\t$(SSG) $< $@ $(TMPHTML5) --metadata sourcefile="$(shell echo $<)"
+\t$(SSG) $@ $(TMPHTML5) --source $< --metadata sourcefile="$(shell echo $<)" revisionnumber=$(REVISIONNUMBER) repository=$(REPOSITORY)
 
 # List files
 ## index.md
 index.md: $(MARKDOWNS)
-\t$(SSGLIST) --title Index $(TMPLIST) $(MARKDOWNS)
+\t$(SSG) $@ $(TMPLIST) --metadata title='Index' collection='Collection([$(LISTMD)])' --evals collection
+
 ## keywords.md aka glossary of keywords
-keywords.md: $(MARKDOWNS)
-\t$(SSGLIST) --title Glossary --group_by keywords $(TMPLIST) $(MARKDOWNS)
+#keywords.md: $(MARKDOWNS)
+#\t$(SSGLIST) --title Glossary --group_by keywords $(TMPLIST) $(MARKDOWNS)
 
 clean:
 \trm $(MARKDOWNS_HTML5)
 """
 
     parser = argparse.ArgumentParser(prog = "cagen-make", description="creates a Makefile file for using GNU Make to generate HTML5 files using cagen")
-    parser.add_argument("--init", action='store_true', help="creates the Makefile")
+    parser.add_argument("directory", type=str, help="creates the Makefile in the DIRECTORY")
     parser.add_argument("--templates", action='store_true', help="creates the directory 'templates' in the current directory with the copy of basic cagen templates")
     args = parser.parse_args()
 
-    if args.init:
-        with open("Makefile", "w") as f:
-            f.write(maketemplate)
-    elif args.templates:
-        if not os.path.exists('templates'):
-            os.makedirs('templates')
-            for f in importlib.resources.files('cagen.templates').iterdir():
-                shutil.copy(f, 'templates/' + f.name)
+    if args.directory:
+        # If args.directory exists, then create the Makefile
+        if os.path.exists(args.directory):
+            with open(args.directory + "/" + "Makefile", "w") as f:
+                f.write(maketemplate)
+
+            # Create templates directory if user wants
+            if args.templates:
+                destination = args.directory + "/" + "templates"
+                if not os.path.exists(destination):
+                    os.makedirs(destination)
+                    for f in importlib.resources.files('cagen.templates').iterdir():
+                        shutil.copy(f, destination + "/" + f.name)
+        else:
+            print("The directory {} does not exist. Please create it".format(args.directory))
     else:
         print("See --help for hints")
```

### Comparing `cagen-0.2.0b8/src/cagen/libcagen.py` & `cagen-0.2.0b9/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b8/src/cagen/templates/schema.tmpl` & `cagen-0.2.0b9/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b8/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0b9/src/cagen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b8
+Version: 0.2.0b9
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

