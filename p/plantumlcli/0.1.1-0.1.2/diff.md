# Comparing `tmp/plantumlcli-0.1.1.tar.gz` & `tmp/plantumlcli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantumlcli-0.1.1.tar", last modified: Sun May  7 05:21:26 2023, max compression
+gzip compressed data, was "plantumlcli-0.1.2.tar", last modified: Sun May  7 08:00:23 2023, max compression
```

## Comparing `plantumlcli-0.1.1.tar` & `plantumlcli-0.1.2.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/entry/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7816 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/entry/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/plantumlcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/models/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/plantumlcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/plantumlcli/utils/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 08:00:23.245155 plantumlcli-0.1.2/plantumlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9058 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 08:00:23.000000 plantumlcli-0.1.2/plantumlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-pdf.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 08:00:23.249155 plantumlcli-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 07:59:40.000000 plantumlcli-0.1.2/setup.py
```

### Comparing `plantumlcli-0.1.1/LICENSE` & `plantumlcli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/PKG-INFO` & `plantumlcli-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: pdf
 Provides-Extra: doc
 Provides-Extra: lint
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
@@ -63,15 +64,21 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.6+ is required, pypy is also tested to be okay.
+Python 3.7+ is required, pypy is also tested to be okay.
+
+If you need to export the diagrams to PDF format, just install like this
+
+```bash
+pip install plantumlcli[pdf]
+```
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
 
@@ -89,15 +96,17 @@
 
 ```bash
 plantumlcli -c   # check both environments
 plantumlcli -cL  # check local environment only
 plantumlcli -cR  # check remote environment only
 ```
 
-In default, no local plantuml jar can be used, the remote host is set to the official one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by environment variables or command lines.
+In default, no local plantuml jar can be used, the remote host is set to the official
+one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by
+environment variables or command lines.
 
 ```bash
 plantumlcli -c                                             # local not okay, remote okay
 PLANTUML_HOST=http://plantuml.example.com plantumlcli -cR  # remote okay
 plantumlcli -cR -r http://plantuml.example.com             # remote okay
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -cL         # local okay
 plantumlcli -cL -p /my/path/plantuml.jar                   # local okay
@@ -114,15 +123,16 @@
 
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli source.puml     # use local plantuml jar to build png
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -L source.puml  # force use local plantuml jar to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml source.puml     # use your plantuml host to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml -R source.puml  # force use your plantuml host to build png
 ```
 
-You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L` and `-R` commands)
+You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L`
+and `-R` commands)
 
 ```bash
 plantumlcli -u helloworld.puml              # get png URL of helloworld.puml
 plantumlcli -u -t eps helloworld.puml       # get eps URL of helloworld.puml
 plantumlcli --homepage-url helloworld.puml  # get online editor's URL of helloworld.puml
 plantumlcli -u helloworld.puml common.puml  # get png URL of the 2 puml files (one line for one URL, in order)
 ```
@@ -139,61 +149,67 @@
 from pathlib import Path
 from plantumlcli import LocalPlantuml, RemotePlantuml
 
 if __name__ == "__main__":
     code = Path('source.puml').read_text()
 
     local = LocalPlantuml.autoload()
-    print(local.dump_txt(code))                           # print text graph of code
+    print(local.dump_txt(code))  # print text graph of code
     local.dump('/my/path/source_local.png', 'png', code)  # save png to /my/path/source_local.png
     local.dump('/my/path/source_local.eps', 'eps', code)  # save eps to /my/path/source_local.eps
 
     remote = RemotePlantuml.autoload()
-    print(remote.dump_txt(code))                            # print text graph of code
+    print(remote.dump_txt(code))  # print text graph of code
     remote.dump('/my/path/source_remote.png', 'png', code)  # save png to /my/path/source_remote.png
     remote.dump('/my/path/source_remote.eps', 'eps', code)  # save eps to /my/path/source_remote.eps
-    print(remote.get_url('png', code))                      # get png url from remote host
-    print(remote.get_homepage_url(code))                    # get online editor's url from remote host
+    print(remote.get_url('png', code))  # get png url from remote host
+    print(remote.get_homepage_url(code))  # get online editor's url from remote host
 
 ```
 
 ## Contributing
 
 Thank you for considering contributing to plantumlcli!
 
-We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md for more guides.
+We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md
+for more guides.
 
-And users can join our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
+And users can join
+our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or
+contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
 
 ## Links
 
 Github: [https://github.com/HansBug/plantumlcli](https://github.com/HansBug/plantumlcli)
 
-Documentation(just readme yet, will be written soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
+Documentation(just readme yet, will be written
+soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
 
 Issue Tracker: [https://github.com/HansBug/plantumlcli/issues](https://github.com/HansBug/plantumlcli/issues)
 
 Pypi: [https://pypi.org/project/plantumlcli/](https://pypi.org/project/plantumlcli/)
 
-Test pypi(pre-released versions can be found here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
+Test pypi(pre-released versions can be found
+here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
 
 ## Change log
 
 ### Version 0.0.3
 
 Released 2021-10-8
 
 * Fix the problem when using official site.
 * click version requirement changed to >= 7.0, will not conflict with other packages any more.
 
 ### Version 0.0.2
 
 Released 2020-11-30
 
-* Fix a bug on windows platform, issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
+* Fix a bug on windows platform,
+  issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
 
 ### Version 0.0.1
 
 Released 2020-11-29
 
 * The first official `plantumlcli` version, cheers!!! :beers:
```

### Comparing `plantumlcli-0.1.1/README.md` & `plantumlcli-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,21 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.6+ is required, pypy is also tested to be okay.
+Python 3.7+ is required, pypy is also tested to be okay.
+
+If you need to export the diagrams to PDF format, just install like this
+
+```bash
+pip install plantumlcli[pdf]
+```
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
 
@@ -59,15 +65,17 @@
 
 ```bash
 plantumlcli -c   # check both environments
 plantumlcli -cL  # check local environment only
 plantumlcli -cR  # check remote environment only
 ```
 
-In default, no local plantuml jar can be used, the remote host is set to the official one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by environment variables or command lines.
+In default, no local plantuml jar can be used, the remote host is set to the official
+one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by
+environment variables or command lines.
 
 ```bash
 plantumlcli -c                                             # local not okay, remote okay
 PLANTUML_HOST=http://plantuml.example.com plantumlcli -cR  # remote okay
 plantumlcli -cR -r http://plantuml.example.com             # remote okay
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -cL         # local okay
 plantumlcli -cL -p /my/path/plantuml.jar                   # local okay
@@ -84,15 +92,16 @@
 
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli source.puml     # use local plantuml jar to build png
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -L source.puml  # force use local plantuml jar to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml source.puml     # use your plantuml host to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml -R source.puml  # force use your plantuml host to build png
 ```
 
-You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L` and `-R` commands)
+You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L`
+and `-R` commands)
 
 ```bash
 plantumlcli -u helloworld.puml              # get png URL of helloworld.puml
 plantumlcli -u -t eps helloworld.puml       # get eps URL of helloworld.puml
 plantumlcli --homepage-url helloworld.puml  # get online editor's URL of helloworld.puml
 plantumlcli -u helloworld.puml common.puml  # get png URL of the 2 puml files (one line for one URL, in order)
 ```
@@ -109,61 +118,67 @@
 from pathlib import Path
 from plantumlcli import LocalPlantuml, RemotePlantuml
 
 if __name__ == "__main__":
     code = Path('source.puml').read_text()
 
     local = LocalPlantuml.autoload()
-    print(local.dump_txt(code))                           # print text graph of code
+    print(local.dump_txt(code))  # print text graph of code
     local.dump('/my/path/source_local.png', 'png', code)  # save png to /my/path/source_local.png
     local.dump('/my/path/source_local.eps', 'eps', code)  # save eps to /my/path/source_local.eps
 
     remote = RemotePlantuml.autoload()
-    print(remote.dump_txt(code))                            # print text graph of code
+    print(remote.dump_txt(code))  # print text graph of code
     remote.dump('/my/path/source_remote.png', 'png', code)  # save png to /my/path/source_remote.png
     remote.dump('/my/path/source_remote.eps', 'eps', code)  # save eps to /my/path/source_remote.eps
-    print(remote.get_url('png', code))                      # get png url from remote host
-    print(remote.get_homepage_url(code))                    # get online editor's url from remote host
+    print(remote.get_url('png', code))  # get png url from remote host
+    print(remote.get_homepage_url(code))  # get online editor's url from remote host
 
 ```
 
 ## Contributing
 
 Thank you for considering contributing to plantumlcli!
 
-We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md for more guides.
+We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md
+for more guides.
 
-And users can join our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
+And users can join
+our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or
+contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
 
 ## Links
 
 Github: [https://github.com/HansBug/plantumlcli](https://github.com/HansBug/plantumlcli)
 
-Documentation(just readme yet, will be written soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
+Documentation(just readme yet, will be written
+soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
 
 Issue Tracker: [https://github.com/HansBug/plantumlcli/issues](https://github.com/HansBug/plantumlcli/issues)
 
 Pypi: [https://pypi.org/project/plantumlcli/](https://pypi.org/project/plantumlcli/)
 
-Test pypi(pre-released versions can be found here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
+Test pypi(pre-released versions can be found
+here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
 
 ## Change log
 
 ### Version 0.0.3
 
 Released 2021-10-8
 
 * Fix the problem when using official site.
 * click version requirement changed to >= 7.0, will not conflict with other packages any more.
 
 ### Version 0.0.2
 
 Released 2020-11-30
 
-* Fix a bug on windows platform, issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
+* Fix a bug on windows platform,
+  issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
 
 ### Version 0.0.1
 
 Released 2020-11-29
 
 * The first official `plantumlcli` version, cheers!!! :beers:
```

### Comparing `plantumlcli-0.1.1/plantumlcli/entry/base.py` & `plantumlcli-0.1.2/plantumlcli/entry/base.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/entry/cli.py` & `plantumlcli-0.1.2/plantumlcli/entry/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -79,19 +79,17 @@
 @click.option('-R', '--use-remote', is_flag=True, help='Use remote plantuml only.')
 @click.option('-c', '--check', is_flag=True, help='Check usable plantuml.')
 @click.option('-u', '--url', is_flag=True, help='Print url of remote plantuml resource (ignore -L and -R).')
 @click.option('--homepage-url', is_flag=True, help='Print url of remote plantuml editor (ignore -L, -R and -u).')
 @click.option('-t', '--type', 'resource_type', default=PlantumlResourceType.PNG.name,
               type=click.Choice(list(PlantumlResourceType.__members__.keys()), case_sensitive=False),
               help='Type of plantuml resource. '
-                   'Please note that the PDF format is only supported by the '
-                   'plantuml-server 1.2023 or higher version and is not supported on the official website. '
-                   'Additionally, when using the local JAR for PDF export, '
-                   'you need to install the extra dependencies. For more information, '
-                   'please refer to: https://plantuml.com/en/pdf',
+                   '(Attention that the PDF format is only natively supported by '
+                   'few versions of plantuml-server. Please install \'plantumlcli[pdf]\' '
+                   'and Cairo environment to make sure the export to PDF can be processed.)',
               show_default=True)
 @click.option('-T', '--text', is_flag=True, help='Display text uml graph by stdout (ignore -t).')
 @click.option('-o', '--output', type=str, multiple=True,
               help='Paths of output files (relative path supported, based on output dir in -O).')
 @click.option('-O', '--output-dir', type=click.Path(exists=True, file_okay=False, writable=True), default='.',
               help='Base path for outputting files.', show_default='current path')
 @click.option('-n', '--concurrency', type=int, default=_DEFAULT_CONCURRENCY, callback=validate_concurrency,
```

### Comparing `plantumlcli-0.1.1/plantumlcli/entry/general.py` & `plantumlcli-0.1.2/plantumlcli/entry/general.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/entry/local.py` & `plantumlcli-0.1.2/plantumlcli/entry/local.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/entry/remote.py` & `plantumlcli-0.1.2/plantumlcli/entry/remote.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/models/base.py` & `plantumlcli-0.1.2/plantumlcli/models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 from abc import ABCMeta
 from enum import IntEnum, unique
 from typing import TypeVar, Type, Optional, Tuple, Union, Any, Mapping
 
 from ..utils import check_func, save_binary_file, auto_decode
 
 
+def _has_cairosvg():
+    try:
+        import cairosvg
+    except (ImportError, ModuleNotFoundError):
+        return False
+    else:
+        return True
+
+
 @unique
 class PlantumlType(IntEnum):
     LOCAL = 1
     REMOTE = 2
 
 
 @unique
```

### Comparing `plantumlcli-0.1.1/plantumlcli/models/local.py` & `plantumlcli-0.1.2/plantumlcli/models/local.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import re
 import shutil
 from tempfile import TemporaryDirectory, NamedTemporaryFile
 from typing import Tuple, Optional, Mapping, Any
 
-from .base import Plantuml, PlantumlResourceType
+from .base import Plantuml, PlantumlResourceType, _has_cairosvg
 from ..utils import load_binary_file, save_text_file, CommandLineExecuteError, execute
 
 PLANTUML_JAR_ENV = 'PLANTUML_JAR'
 
 
 def find_java_from_env() -> Optional[str]:
     return shutil.which('java')
@@ -107,18 +107,23 @@
         _lines = _stdout.strip().splitlines()
         _first_line = _lines[0].strip() if _lines else ''
         _line, _ = re.subn(r'\([^()]*?\)', '', _first_line)
         _line, _ = re.subn(r'\\s+', '', _line)
         return _line.strip()
 
     def _generate_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
-        with TemporaryDirectory(prefix='puml') as output_path_name:
-            with NamedTemporaryFile(prefix='puml', suffix='.puml') as input_file:
-                save_text_file(input_file.name, code)
-                self.__execute(f'-t{type_.name.lower()}', '-o', output_path_name, input_file.name)
-                _file_list = os.listdir(output_path_name)
-                if _file_list:
-                    output_filename = os.path.join(output_path_name, _file_list[0])
-                    return load_binary_file(output_filename)
-                else:
-                    # When you see this error, it means bug, please open an issue for help us fix this
-                    raise FileNotFoundError(f'No expected file found in {output_path_name!r}.')  # pragma: no cover
+        if type_ == PlantumlResourceType.PDF and _has_cairosvg():
+            import cairosvg
+
+            return cairosvg.svg2pdf(bytestring=self._generate_uml_data(PlantumlResourceType.SVG, code))
+        else:
+            with TemporaryDirectory(prefix='puml') as output_path_name:
+                with NamedTemporaryFile(prefix='puml', suffix='.puml') as input_file:
+                    save_text_file(input_file.name, code)
+                    self.__execute(f'-t{type_.name.lower()}', '-o', output_path_name, input_file.name)
+                    _file_list = os.listdir(output_path_name)
+                    if _file_list:
+                        output_filename = os.path.join(output_path_name, _file_list[0])
+                        return load_binary_file(output_filename)
+                    else:
+                        # When you see this error, it means bug, please open an issue for help us fix this
+                        raise FileNotFoundError(f'No expected file found in {output_path_name!r}.')  # pragma: no cover
```

### Comparing `plantumlcli-0.1.1/plantumlcli/models/remote.py` & `plantumlcli-0.1.2/plantumlcli/models/remote.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import zlib
 from typing import Optional, Mapping, Any, Union, Tuple
 
 import requests
 from pyquery import PyQuery
 from urlobject import URLObject
 
-from .base import Plantuml, PlantumlResourceType
+from .base import Plantuml, PlantumlResourceType, _has_cairosvg
 
 PLANTUML_HOST_ENV = 'PLANTUML_HOST'
 OFFICIAL_PLANTUML_HOST = 'http://www.plantuml.com/plantuml'
 
 
 def find_plantuml_host_from_env() -> Optional[None]:
     return os.environ.get(PLANTUML_HOST_ENV, None)
@@ -105,20 +105,22 @@
     def _check_version(self, version: str):
         if not self._is_official():
             if (not version) or ("plantuml" not in version.lower()) or ("version" not in version.lower()):
                 raise ValueError(f"Invalid version information from homepage - {version!r}.")
 
     def _check_type_supported(self, type_: PlantumlResourceType):
         if type_ == PlantumlResourceType.PDF:
-            if self._is_official():
-                raise ValueError(f'Resource type {type_!r} not supported for plantuml official site - {self.__host!r}.')
-            else:
-                if self._get_server_version() < (1, 2023):
-                    raise ValueError(f'Resource type {type_!r} not supported for '
-                                     f'plantuml server site lower than 1.2023 - {self._get_server_version()!r}.')
+            if not _has_cairosvg():
+                if self._is_official():
+                    raise ValueError(f'Resource type {type_!r} not supported for plantuml official '
+                                     f'site - {self.__host!r}.')
+                else:
+                    if self._get_server_version() < (1, 2023):
+                        raise ValueError(f'Resource type {type_!r} not supported for '
+                                         f'plantuml server site lower than 1.2023 - {self._get_server_version()!r}.')
 
     def _get_version(self) -> str:
         if not self._is_official():
             r = self.__get_homepage()
             return PyQuery(r.content.decode()).find('#footer').text().strip()
         else:
             return 'Official Site'
@@ -136,15 +138,21 @@
         return self.__request_url(self.__get_uml_path(type_, code))
 
     def __get_uml(self, type_: str, code: str) -> bytes:
         r = self.__request(self.__get_uml_path(type_, code))
         return r.content
 
     def _generate_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
-        return self.__get_uml(type_.name.lower(), code)
+        if type_ == PlantumlResourceType.PDF and _has_cairosvg():
+            import cairosvg
+
+            binary = self.__get_uml(PlantumlResourceType.SVG.name.lower(), code)
+            return cairosvg.svg2pdf(bytestring=binary)
+        else:
+            return self.__get_uml(type_.name.lower(), code)
 
     def _generate_uml_url(self, type_: PlantumlResourceType, code: str) -> str:
         return self.__get_uml_url(type_.name.lower(), code)
 
     def get_url(self, type_: Union[int, str, PlantumlResourceType], code: str) -> str:
         """
         Get resource url for the source code
```

### Comparing `plantumlcli-0.1.1/plantumlcli/utils/concurrent.py` & `plantumlcli-0.1.2/plantumlcli/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/utils/decorator.py` & `plantumlcli-0.1.2/plantumlcli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/utils/encoding.py` & `plantumlcli-0.1.2/plantumlcli/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/utils/execute.py` & `plantumlcli-0.1.2/plantumlcli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli/utils/file.py` & `plantumlcli-0.1.2/plantumlcli/utils/file.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.1/plantumlcli.egg-info/PKG-INFO` & `plantumlcli-0.1.2/plantumlcli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -20,14 +20,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
+Provides-Extra: pdf
 Provides-Extra: doc
 Provides-Extra: lint
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
@@ -63,15 +64,21 @@
 Install from source code
 
 ```bash
 git clone https://github.com/HansBug/plantumlcli
 cd plantumlcli && pip install .
 ```
 
-Python 3.6+ is required, pypy is also tested to be okay.
+Python 3.7+ is required, pypy is also tested to be okay.
+
+If you need to export the diagrams to PDF format, just install like this
+
+```bash
+pip install plantumlcli[pdf]
+```
 
 ## Using with cli
 
 ### Basic Usage
 
 Show version of `plantumlcli`
 
@@ -89,15 +96,17 @@
 
 ```bash
 plantumlcli -c   # check both environments
 plantumlcli -cL  # check local environment only
 plantumlcli -cR  # check remote environment only
 ```
 
-In default, no local plantuml jar can be used, the remote host is set to the official one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by environment variables or command lines.
+In default, no local plantuml jar can be used, the remote host is set to the official
+one (http://www.plantuml.com/plantuml). But don't worry, you can specify your plantuml jar file or remote host by
+environment variables or command lines.
 
 ```bash
 plantumlcli -c                                             # local not okay, remote okay
 PLANTUML_HOST=http://plantuml.example.com plantumlcli -cR  # remote okay
 plantumlcli -cR -r http://plantuml.example.com             # remote okay
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -cL         # local okay
 plantumlcli -cL -p /my/path/plantuml.jar                   # local okay
@@ -114,15 +123,16 @@
 
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli source.puml     # use local plantuml jar to build png
 PLANTUML_JAR=/my/path/plantuml.jar plantumlcli -L source.puml  # force use local plantuml jar to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml source.puml     # use your plantuml host to build png
 PLANTUML_HOST=http://plantuml.example.com plantuml -R source.puml  # force use your plantuml host to build png
 ```
 
-You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L` and `-R` commands)
+You can also get the URL address of remote plantuml (in these cases, remote plantuml will be used regardless of `-L`
+and `-R` commands)
 
 ```bash
 plantumlcli -u helloworld.puml              # get png URL of helloworld.puml
 plantumlcli -u -t eps helloworld.puml       # get eps URL of helloworld.puml
 plantumlcli --homepage-url helloworld.puml  # get online editor's URL of helloworld.puml
 plantumlcli -u helloworld.puml common.puml  # get png URL of the 2 puml files (one line for one URL, in order)
 ```
@@ -139,61 +149,67 @@
 from pathlib import Path
 from plantumlcli import LocalPlantuml, RemotePlantuml
 
 if __name__ == "__main__":
     code = Path('source.puml').read_text()
 
     local = LocalPlantuml.autoload()
-    print(local.dump_txt(code))                           # print text graph of code
+    print(local.dump_txt(code))  # print text graph of code
     local.dump('/my/path/source_local.png', 'png', code)  # save png to /my/path/source_local.png
     local.dump('/my/path/source_local.eps', 'eps', code)  # save eps to /my/path/source_local.eps
 
     remote = RemotePlantuml.autoload()
-    print(remote.dump_txt(code))                            # print text graph of code
+    print(remote.dump_txt(code))  # print text graph of code
     remote.dump('/my/path/source_remote.png', 'png', code)  # save png to /my/path/source_remote.png
     remote.dump('/my/path/source_remote.eps', 'eps', code)  # save eps to /my/path/source_remote.eps
-    print(remote.get_url('png', code))                      # get png url from remote host
-    print(remote.get_homepage_url(code))                    # get online editor's url from remote host
+    print(remote.get_url('png', code))  # get png url from remote host
+    print(remote.get_homepage_url(code))  # get online editor's url from remote host
 
 ```
 
 ## Contributing
 
 Thank you for considering contributing to plantumlcli!
 
-We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md for more guides.
+We appreciate all contributions to improve plantumlcli, both logic and system designs. Please refer to CONTRIBUTING.md
+for more guides.
 
-And users can join our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
+And users can join
+our [slack communication channel](https://join.slack.com/t/hansbug/shared_invite/zt-z3rtyooz-Rf6QZ9eNy6t5vvUGnicfdw), or
+contact the core developer [HansBug](https://github.com/HansBug) for more detailed discussion.
 
 ## Links
 
 Github: [https://github.com/HansBug/plantumlcli](https://github.com/HansBug/plantumlcli)
 
-Documentation(just readme yet, will be written soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
+Documentation(just readme yet, will be written
+soon): [https://github.com/HansBug/plantumlcli/blob/main/README.md](https://github.com/HansBug/plantumlcli/blob/main/README.md)
 
 Issue Tracker: [https://github.com/HansBug/plantumlcli/issues](https://github.com/HansBug/plantumlcli/issues)
 
 Pypi: [https://pypi.org/project/plantumlcli/](https://pypi.org/project/plantumlcli/)
 
-Test pypi(pre-released versions can be found here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
+Test pypi(pre-released versions can be found
+here): [https://test.pypi.org/project/plantumlcli/](https://test.pypi.org/project/plantumlcli/)
 
 ## Change log
 
 ### Version 0.0.3
 
 Released 2021-10-8
 
 * Fix the problem when using official site.
 * click version requirement changed to >= 7.0, will not conflict with other packages any more.
 
 ### Version 0.0.2
 
 Released 2020-11-30
 
-* Fix a bug on windows platform, issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
+* Fix a bug on windows platform,
+  issue: [https://github.com/HansBug/plantumlcli/issues/1](https://github.com/HansBug/plantumlcli/issues/1)
 
 ### Version 0.0.1
 
 Released 2020-11-29
 
 * The first official `plantumlcli` version, cheers!!! :beers:
```

### Comparing `plantumlcli-0.1.1/plantumlcli.egg-info/SOURCES.txt` & `plantumlcli-0.1.2/plantumlcli.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements-doc.txt
 requirements-lint.txt
+requirements-pdf.txt
 requirements-test.txt
 requirements.txt
 setup.py
 plantumlcli/__init__.py
 plantumlcli.egg-info/PKG-INFO
 plantumlcli.egg-info/SOURCES.txt
 plantumlcli.egg-info/dependency_links.txt
```

### Comparing `plantumlcli-0.1.1/plantumlcli.egg-info/requires.txt` & `plantumlcli-0.1.2/plantumlcli.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,20 +18,26 @@
 sphinx-multiversion~=0.2.4
 where~=1.0.2
 easydict<2,>=1.7
 
 [lint]
 flake8>=5.0.0
 
+[pdf]
+cairosvg>=2.6.0
+
 [test]
 flake8~=3.5
 pytest~=6.2.5
 pytest-cov~=3.0.0
 pytest-mock~=3.6.1
 pytest-rerunfailures~=10.2
 pytest-timeout~=2.0.2
 more-itertools<8,>=7
 testtools>=2
 coverage>=5
 mock>=4.0.3
 huggingface_hub
 pysyslimit>=0.5.0
+
+[test:python_version > "3.8"]
+cairosvg>=2.6.0
```

### Comparing `plantumlcli-0.1.1/setup.py` & `plantumlcli-0.1.2/setup.py`

 * *Files identical despite different names*

