# Comparing `tmp/elm-messenger-0.1.2.tar.gz` & `tmp/elm-messenger-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elm-messenger-0.1.2.tar", last modified: Thu May  4 12:39:55 2023, max compression
+gzip compressed data, was "elm-messenger-0.1.3.tar", last modified: Sun May  7 08:28:02 2023, max compression
```

## Comparing `elm-messenger-0.1.2.tar` & `elm-messenger-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/
--rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/MANIFEST.in
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/Readme.md
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/elm_messenger.egg-info/
--rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/PKG-INFO
--rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/SOURCES.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/dependency_links.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/entry_points.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/requires.txt
--rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-04 12:39:55.000000 elm-messenger-0.1.2/elm_messenger.egg-info/top_level.txt
-drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/messengercli/
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/messengercli/__init__.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/messengercli/command_line.py
--rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9159 2023-05-04 10:54:19.000000 elm-messenger-0.1.2/messengercli/messenger.py
--rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-04 12:39:55.466770 elm-messenger-0.1.2/setup.cfg
--rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.2/setup.py
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       18 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/MANIFEST.in
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      122 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/Readme.md
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/elm_messenger.egg-info/
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      387 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/PKG-INFO
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      344 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/SOURCES.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        1 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/dependency_links.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       61 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/entry_points.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)        6 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/requires.txt
+-rw-r--r--   0 linsy     (1000) linsy     (1000)       13 2023-05-07 08:28:02.000000 elm-messenger-0.1.3/elm_messenger.egg-info/top_level.txt
+drwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/messengercli/
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)        0 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/messengercli/__init__.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)      120 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/messengercli/command_line.py
+-rwxr-xr-x   0 linsy     (1000) linsy     (1000)     9317 2023-05-07 08:25:40.000000 elm-messenger-0.1.3/messengercli/messenger.py
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      407 2023-05-07 08:28:02.056569 elm-messenger-0.1.3/setup.cfg
+-rw-r--r--   0 linsy     (1000) linsy     (1000)      161 2023-05-04 10:50:53.000000 elm-messenger-0.1.3/setup.py
```

### Comparing `elm-messenger-0.1.2/messengercli/messenger.py` & `elm-messenger-0.1.3/messengercli/messenger.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,30 +233,34 @@
                 ),
             )
 
 
 @app.command()
 def init(
     name: str,
+    template_repo=typer.Option(
+        "https://github.com/linsyking/messenger-templates",
+        "--template-repo",
+        "-t",
+        help="Use customized repository for cloning templates.",
+    ),
 ):
     input(
         f"""Thanks for using Messenger.
 See https://github.com/linsyking/Messenger.git for more information.
 Here is my plan:
 - Create a directory named {name}
 - Install the core Messenger liberary
 - Install the elm packages needed
 Press Enter to continue
 """
     )
     os.makedirs(name, exist_ok=True)
     os.chdir(name)
-    os.system(
-        f"git clone https://github.com/linsyking/messenger-templates .messenger --depth=1"
-    )
+    os.system(f"git clone {template_repo} .messenger --depth=1")
     shutil.copytree(".messenger/core/", "./src")
     shutil.copytree(".messenger/public/", "./public")
     shutil.copy(".messenger/.gitignore", "./.gitignore")
     shutil.copy(".messenger/Makefile", "./Makefile")
     shutil.copy(".messenger/elm.json", "./elm.json")
 
     os.makedirs("src/Scenes", exist_ok=True)
```

