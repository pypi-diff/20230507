# Comparing `tmp/cagen-0.2.0b9.tar.gz` & `tmp/cagen-0.2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0b9.tar", last modified: Sun May  7 13:42:30 2023, max compression
+gzip compressed data, was "cagen-0.2.0rc1.tar", last modified: Sun May  7 17:31:34 2023, max compression
```

## Comparing `cagen-0.2.0b9.tar` & `cagen-0.2.0rc1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.880965 cagen-0.2.0b9/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b9/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-07 13:42:30.880965 cagen-0.2.0b9/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b9/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-07 13:42:25.000000 cagen-0.2.0b9/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-07 13:42:30.880965 cagen-0.2.0b9/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b9/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     5914 2023-05-07 13:42:03.000000 cagen-0.2.0b9/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b9/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.880965 cagen-0.2.0b9/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b9/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b9/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b9/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b9/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 13:42:30.877632 cagen-0.2.0b9/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-07 13:42:30.000000 cagen-0.2.0b9/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0rc1/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0rc1/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1148 2023-05-07 17:30:40.000000 cagen-0.2.0rc1/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-07 17:31:34.910588 cagen-0.2.0rc1/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0rc1/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     4659 2023-05-07 17:29:41.000000 cagen-0.2.0rc1/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0rc1/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0rc1/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0rc1/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     3998 2023-05-07 17:21:41.000000 cagen-0.2.0rc1/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0rc1/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-07 17:31:34.907255 cagen-0.2.0rc1/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4359 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       80 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-07 17:31:34.000000 cagen-0.2.0rc1/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0b9/PKG-INFO` & `cagen-0.2.0rc1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b9
+Version: 0.2.0rc1
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0b9/README.md` & `cagen-0.2.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b9/pyproject.toml` & `cagen-0.2.0rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,19 @@
 
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
-cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.beta-9"
+version = "0.2.0.rc1"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0b9/src/cagen/cmd.py` & `cagen-0.2.0rc1/src/cagen/cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,58 +31,38 @@
             evals=args.evals
             eassignments=libcagen.evaluate_assignments(assignments, evals)
             f.write(entry.to(mytemplatepath=args.template, additionalsearchlist=eassignments, destsyntax=args.syntax))
             print("{} -> {} ({}) using {}".format(args.source, args.to, args.syntax, args.template))
     else:
         print("Template {} not found".format(args.template))
 
-
-def cagen_list():
-    """Defines the `cagen-list` command line script function to call from pyproject.toml"""
-
-    parser = argparse.ArgumentParser(prog = "cagen-list", description="make a list of entries in Markdown format and it saves it in a file")
-    parser.add_argument("template", type=str, help="Mako template to use")
-    parser.add_argument("--group_by", type=str, help="group by an specific key. Eg. --group_by author. The field passed in --group_by is a key of metadata. In the case the key is a list (eg. 'keywords') then, it groups by each value, not each list.")
-    parser.add_argument("--title", type=str, default='List', help="the title of the generated list document. 'List' by default")
-    parser.add_argument("list", type=str, nargs='*', help="the file list of entries. Eg. this.md that.md ... Missing files are ignored")
-    args = parser.parse_args()
-
-    collection = libcagen.Collection(args.list)
-    # pass all parameters to desired template
-    if os.path.exists(args.template):
-        template = Template(filename=args.template, strict_undefined=True)
-        mysearchlist = {'collection': collection, 'title': args.title, 'group_by': args.group_by}
-        print(template.render(**mysearchlist))
-
-
 def cagen_make():
     """Defines the `cagen-make` command line script function to call from pyproject.toml"""
 
     maketemplate = """
 # Default template
 TMPHTML5 = templates/schema.tmpl
 TMPLIST = templates/list.md.tmpl
 
 # Select all markdowns file except index.md
 MARKDOWNS = $(shell find . -type f -name "*.md" ! -name "index.md" ! -name "README.md")
 ## List them as comma-separated and quotating list
-LISTMD = '"${shell echo $(MARKDOWNS) | sed 's/ /", "/g')}"'
+LISTMD = "$(shell echo $(MARKDOWNS) | sed 's/ /", "/g')"
 
 # Replace the extension.
 # By default HTML5
 MARKDOWNS_HTML5 = $(MARKDOWNS:.md=.html)
 
 # Extra metadata. Use if you want and edit freely
 REPOSITORY = "https://repo.or.cz/cagen.git"
 REVISIONNUMBER = $(shell git log --format=oneline $<  | wc -l)
 
 # Commands
 
 SSG = cagen
-SSGLIST = cagen-list
 
 # Processing
 
 .PHONY: all clean
 
 all: $(MARKDOWNS_HTML5)
```

### Comparing `cagen-0.2.0b9/src/cagen/libcagen.py` & `cagen-0.2.0rc1/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b9/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0rc1/src/cagen.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b9
+Version: 0.2.0rc1
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

