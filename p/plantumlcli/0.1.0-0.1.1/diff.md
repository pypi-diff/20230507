# Comparing `tmp/plantumlcli-0.1.0.tar.gz` & `tmp/plantumlcli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantumlcli-0.1.0.tar", last modified: Sat May  6 15:02:47 2023, max compression
+gzip compressed data, was "plantumlcli-0.1.1.tar", last modified: Sun May  7 05:21:26 2023, max compression
```

## Comparing `plantumlcli-0.1.0.tar` & `plantumlcli-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/entry/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6126 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/general.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/entry/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/models/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/models/remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/plantumlcli/utils/function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/plantumlcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-06 15:02:47.000000 plantumlcli-0.1.0/plantumlcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:02:47.612231 plantumlcli-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-06 15:02:16.000000 plantumlcli-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7787 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/entry/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/entry/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/models/remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.409187 plantumlcli-0.1.1/plantumlcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/plantumlcli/utils/function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 05:21:26.405187 plantumlcli-0.1.1/plantumlcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9009 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 05:21:26.000000 plantumlcli-0.1.1/plantumlcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 05:21:26.413187 plantumlcli-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-05-07 05:20:46.000000 plantumlcli-0.1.1/setup.py
```

### Comparing `plantumlcli-0.1.0/LICENSE` & `plantumlcli-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.0/PKG-INFO` & `plantumlcli-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: lint
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plantumlcli)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/plantumlcli)
```

### Comparing `plantumlcli-0.1.0/README.md` & `plantumlcli-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.0/plantumlcli/entry/base.py` & `plantumlcli-0.1.1/plantumlcli/entry/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     if success:
         try:
             _duration, _version = _plantuml_version(plantuml)
         except Exception as e:
             success, plantuml = False, e
 
     if success:
-        click.secho('{name} plantuml detected.'.format(name=name.capitalize()), fg='green')
+        click.secho(f'{name.capitalize()} plantuml detected.', fg='green')
 
         click.echo(_version)
         if callback:
             callback(plantuml, _duration)
     else:
-        click.secho('{name} plantuml not detected or has problem.'.format(name=name.capitalize()), fg='red')
-        click.echo('Error : {error}'.format(error=repr(plantuml)))
+        click.secho(f'{name.capitalize()} plantuml not detected or has problem.', fg='red')
+        click.echo(f'Error : {plantuml!r}')
 
     return success
```

### Comparing `plantumlcli-0.1.0/plantumlcli/entry/cli.py` & `plantumlcli-0.1.1/plantumlcli/entry/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,16 @@
     Print version information of cli
     :param ctx: click context
     :param param: current parameter's metadata
     :param value: value of current parameter
     """
     if not value or ctx.resilient_parsing:
         return
-    click.echo('{title}, version {version}.'.format(title=__TITLE__.capitalize(), version=__VERSION__))
-    click.echo('Developed by {author}, {email}.'.format(author=__AUTHOR__, email=__AUTHOR_EMAIL__))
+    click.echo(f'{__TITLE__.capitalize()}, version {__VERSION__}.')
+    click.echo(f'Developed by {__AUTHOR__}, {__AUTHOR_EMAIL__}.')
     ctx.exit()
 
 
 # noinspection PyUnusedLocal
 def validate_concurrency(ctx: Context, param: Option, value: int):
     if value > 0:
         return value
@@ -66,28 +66,33 @@
 @click.option('-v', '--version', is_flag=True,
               callback=print_version, expose_value=False, is_eager=True,
               help="Show package's version information.")
 @click.option('-j', '--java', type=str, default=find_java_from_env(),
               help='Path of java executable file (will load from environment when not given).',
               show_default='java from ${PATH}')
 @click.option('-p', '--plantuml', envvar=PLANTUML_JAR_ENV, type=str, default=None,
-              help='Path of plantuml jar file (will load from ${{{env}}} when not given).'.format(
-                  env=PLANTUML_JAR_ENV))
+              help=f'Path of plantuml jar file (will load from ${{{PLANTUML_JAR_ENV}}} when not given).')
 @click.option('-r', '--remote-host', envvar=PLANTUML_HOST_ENV, type=str, default=OFFICIAL_PLANTUML_HOST,
-              help='Remote host of the online plantuml editor (will load from ${{{env}}} when not given).'.format(
-                  env=PLANTUML_HOST_ENV),
+              help=f'Remote host of the online plantuml editor '
+                   f'(will load from ${{{PLANTUML_HOST_ENV}}} when not given).',
               show_default=True)
 @click.option('-L', '--use-local', is_flag=True, help='Use local plantuml only.')
 @click.option('-R', '--use-remote', is_flag=True, help='Use remote plantuml only.')
 @click.option('-c', '--check', is_flag=True, help='Check usable plantuml.')
 @click.option('-u', '--url', is_flag=True, help='Print url of remote plantuml resource (ignore -L and -R).')
 @click.option('--homepage-url', is_flag=True, help='Print url of remote plantuml editor (ignore -L, -R and -u).')
 @click.option('-t', '--type', 'resource_type', default=PlantumlResourceType.PNG.name,
-              type=click.Choice(PlantumlResourceType.__members__.keys(), case_sensitive=False),
-              help='Type of plantuml resource.', show_default=True)
+              type=click.Choice(list(PlantumlResourceType.__members__.keys()), case_sensitive=False),
+              help='Type of plantuml resource. '
+                   'Please note that the PDF format is only supported by the '
+                   'plantuml-server 1.2023 or higher version and is not supported on the official website. '
+                   'Additionally, when using the local JAR for PDF export, '
+                   'you need to install the extra dependencies. For more information, '
+                   'please refer to: https://plantuml.com/en/pdf',
+              show_default=True)
 @click.option('-T', '--text', is_flag=True, help='Display text uml graph by stdout (ignore -t).')
 @click.option('-o', '--output', type=str, multiple=True,
               help='Paths of output files (relative path supported, based on output dir in -O).')
 @click.option('-O', '--output-dir', type=click.Path(exists=True, file_okay=False, writable=True), default='.',
               help='Base path for outputting files.', show_default='current path')
 @click.option('-n', '--concurrency', type=int, default=_DEFAULT_CONCURRENCY, callback=validate_concurrency,
               help='Concurrency when running plantuml.', show_default=True)
```

### Comparing `plantumlcli-0.1.0/plantumlcli/entry/general.py` & `plantumlcli-0.1.1/plantumlcli/entry/general.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     elif check_type == PlantumlCheckType.REMOTE:
         print_remote_check_info(remote_ok, remote)
     else:
         # nothing to check, maybe warnings can be placed here.
         pass
 
 
-def print_text_graph(plantuml: Plantuml, sources: Tuple[str], concurrency: int):
+def print_text_graph(plantuml: Plantuml, sources: Tuple[str], concurrency: int):  # noqa
     """
     Print text graph of source codes
     :param plantuml: plantuml object
     :param sources: source code files
     :param concurrency: concurrency when running this
     """
     _error_count = 0
@@ -72,36 +72,35 @@
         except (LocalPlantumlExecuteError, OSError, BaseHTTPError, HTTPError) as e:
             return False, e
 
     def _print_text(src: str, ret: Tuple[bool, Union[str, LocalPlantumlExecuteError]]):
         _success, _data = ret
 
         if _success:
-            click.secho('{source}: '.format(source=src), fg='green')
+            click.secho(f'{src}: ', fg='green')
             click.echo(_data)
         else:
             nonlocal _error_count
             if isinstance(_data, LocalPlantumlExecuteError):
-                click.secho('{source}: [error with exitcode {code}]'.format(source=src, code=_data.exitcode), fg='red')
+                click.secho(f'{src}: [error with exitcode {_data.exitcode}]', fg='red')
                 click.secho(_data.stderr, fg='red')
             else:
                 if hasattr(_data, 'response'):
                     response = getattr(_data, 'response')
                     if hasattr(response, 'status_code'):
                         code = getattr(response, 'status_code')
                     else:
                         code = None
                 else:
                     response, code = None, None
 
                 if code:
-                    click.secho('{source}: [{cls} {code}]'.format(
-                        source=src, cls=type(_data).__name__, code=code), fg='red')
+                    click.secho(f'{src}: [{type(_data).__name__} {code}]', fg='red')
                 else:
-                    click.secho('{source}: [{cls}]'.format(source=src, cls=type(_data).__name__), fg='red')
+                    click.secho(f'{src}: [{type(_data).__name__}]', fg='red')
 
                 click.secho(str(_data), fg='red')
                 if response is not None and code and response.content:
                     click.secho(auto_decode(response.content), fg='red')
                 click.secho('', fg='red')
 
             _error_count += 1
@@ -112,33 +111,32 @@
         post_process=lambda i, src, ret: _print_text(src, ret),
         concurrency=concurrency,
     )
 
     if _error_count > 0:
         raise _click_exception_with_exit_code(
             name='TextGraphError',
-            message='{count} error(s) found when generating text graph.'.format(count=_error_count),
+            message=f'{_error_count} error(s) found when generating text graph.',
             exitcode=-2,
         )
 
 
 def process_plantuml(plantuml: Plantuml, sources: Tuple[str],
                      outputs: Tuple[str], output_dir: Optional[str],
                      type_: PlantumlResourceType, concurrency: int):
     if outputs and len(outputs) != len(sources):
-        raise ValueError('Amount of output file(s) should be {expect}, but {actual} found.'
-                         .format(expect=len(sources), actual=len(outputs)))
+        raise ValueError(f'Amount of output file(s) should be {len(sources)}, but {len(outputs)} found.')
 
     def _output_filename(index: int):
         if outputs:
             name = outputs[index]
         else:
             _, _filename = os.path.split(sources[index])
             _name, _ = os.path.splitext(_filename)
-            name = '{name}.{ext}'.format(name=_name, ext=type_.name.lower())
+            name = f'{_name}.{type_.name.lower()}'
         return os.path.join(output_dir or os.curdir, name)
 
     def _process_code(index: int):
         return plantuml.dump_binary(type_, load_text_file(sources[index]))
 
     def _post_process_data(index: int, ret: bytes):
         save_binary_file(_output_filename(index), ret)
```

### Comparing `plantumlcli-0.1.0/plantumlcli/entry/local.py` & `plantumlcli-0.1.1/plantumlcli/entry/local.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import click
 
 from plantumlcli import LocalPlantuml
 from .base import _check_plantuml, _click_exception_with_exit_code
 
 
 def _additional_info_for_local(plantuml: LocalPlantuml, duration: float):
-    click.echo('Java executable : {path}'.format(path=os.path.abspath(plantuml.java)))
-    click.echo('Plantuml jar : {path}'.format(path=os.path.abspath(plantuml.plantuml)))
+    _ = duration
+    click.echo(f'Java executable : {os.path.abspath(plantuml.java)}')
+    click.echo(f'Plantuml jar : {os.path.abspath(plantuml.plantuml)}')
 
 
 def _check_local_plantuml(success, plantuml: Union[LocalPlantuml, Exception]) -> bool:
     return _check_plantuml('local', success, plantuml, _additional_info_for_local)
 
 
 def print_local_check_info(success, plantuml: Union[LocalPlantuml, Exception]) -> None:
```

### Comparing `plantumlcli-0.1.0/plantumlcli/entry/remote.py` & `plantumlcli-0.1.1/plantumlcli/entry/remote.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from .base import _check_plantuml, _click_exception_with_exit_code
 from ..models.base import PlantumlResourceType
 from ..models.remote import RemotePlantuml
 from ..utils import load_text_file, linear_process
 
 
 def _additional_info_for_remote(plantuml: RemotePlantuml, duration: float):
-    click.echo('Remote host : {host}'.format(host=plantuml.host))
-    click.echo('Connection time : {time}s'.format(time='%.3f' % (duration,)))
+    click.echo(f'Remote host : {plantuml.host}')
+    click.echo(f'Connection time : {"%.3f" % (duration,)}s')
 
 
 def _check_remote_plantuml(success: bool, plantuml: Union[RemotePlantuml, Exception]) -> bool:
     return _check_plantuml('remote', success, plantuml, _additional_info_for_remote)
 
 
 def print_remote_check_info(success, plantuml: Union[RemotePlantuml, Exception]) -> None:
```

### Comparing `plantumlcli-0.1.0/plantumlcli/models/base.py` & `plantumlcli-0.1.1/plantumlcli/models/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from abc import ABCMeta, abstractmethod
+from abc import ABCMeta
 from enum import IntEnum, unique
 from typing import TypeVar, Type, Optional, Tuple, Union, Any, Mapping
 
 from ..utils import check_func, save_binary_file, auto_decode
 
 
 @unique
@@ -16,33 +16,32 @@
     """
     More types will be added later
     """
     TXT = 1
     PNG = 2
     SVG = 3
     EPS = 4
+    PDF = 5
 
     @classmethod
     def load(cls, data: Union[int, str, 'PlantumlResourceType']) -> 'PlantumlResourceType':
         if isinstance(data, PlantumlResourceType):
             return data
         elif isinstance(data, int):
             if data in cls.__members__.values():
                 return cls.__members__[dict(zip(cls.__members__.values(), cls.__members__.keys()))[data]]
             else:
-                raise ValueError('Value {value} not found for enum {cls}.'.format(value=repr(data), cls=cls.__name__))
+                raise ValueError(f'Value {data!r} not found for enum {cls.__name__}.')
         elif isinstance(data, str):
             if data.upper() in cls.__members__.keys():
                 return cls.__members__[data.upper()]
             else:
-                raise KeyError('Key {key} not found for enum {cls}.'.format(key=repr(data), cls=cls.__name__))
+                raise KeyError(f'Key {data!r} not found for enum {cls.__name__}.')
         else:
-            raise TypeError('Data should be an int, str or {cls}, but {actual} found.'.format(
-                cls=cls.__name__, actual=type(data).__name__,
-            ))
+            raise TypeError(f'Data should be an int, str or {cls.__name__}, but {type(data).__name__} found.')
 
 
 class Plantuml(metaclass=ABCMeta):
     def __init__(self):
         """
         """
         pass
@@ -52,17 +51,16 @@
         """
         Autoload plantuml object from given arguments
         :return: autoloaded plantuml object
         """
         raise NotImplementedError  # pragma: no cover
 
     def _check_version(self, version: str):
-        pass
+        pass  # pragma: no cover
 
-    @abstractmethod
     def _get_version(self) -> str:
         raise NotImplementedError  # pragma: no cover
 
     @property
     def version(self) -> str:
         """
         Get version information from this plantuml
@@ -77,61 +75,65 @@
 
     def check(self) -> None:
         """
         Check this plantuml is okay or not, raise exception when not ok
         """
         return self._check()
 
+    def _check_type_supported(self, type_: PlantumlResourceType):
+        _ = type_
+        pass
+
     @check_func(keep_return=False)
     def test(self) -> bool:
         """
         Test this plantuml is okay or not
         :return: True if is okay, otherwise False
         """
         self._check()
         return True
 
-    @abstractmethod
     def _generate_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
         raise NotImplementedError  # pragma: no cover
 
+    def _get_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
+        self._check_type_supported(type_)
+        return self._generate_uml_data(type_, code)
+
     def dump(self, path: str, type_: Union[int, str, PlantumlResourceType], code: str):
         """
         Dump uml data to file
         :param path: file path
         :param type_: resource type
         :param code: source code
         """
-        save_binary_file(path, self._generate_uml_data(PlantumlResourceType.load(type_), code))
+        save_binary_file(path, self._get_uml_data(PlantumlResourceType.load(type_), code))
 
     def dump_binary(self, type_: Union[int, str, PlantumlResourceType], code: str) -> bytes:
         """
         Dump uml data to bytes
         :param type_: resource type
         :param code: source code
         """
-        return self._generate_uml_data(PlantumlResourceType.load(type_), code)
+        return self._get_uml_data(PlantumlResourceType.load(type_), code)
 
     def dump_txt(self, code: str) -> str:
         """
         Dump txt uml data to str
         :param code: source code
         :return: txt uml data
         """
-        return auto_decode(self._generate_uml_data(PlantumlResourceType.TXT, code))
+        return auto_decode(self._get_uml_data(PlantumlResourceType.TXT, code))
 
     def _properties(self) -> Mapping[str, Any]:
-        return {}
+        return {}  # pragma: no cover
 
     def __repr__(self):
-        return '<{cls} {properties}>'.format(
-            cls=self.__class__.__name__,
-            properties=', '.join(['{key}: {value}'.format(key=key, value=repr(value))
-                                  for key, value in sorted(self._properties().items())]),
-        )
+        prop_str = ', '.join([f'{key}: {value!r}' for key, value in sorted(self._properties().items())])
+        return f'<{self.__class__.__name__} {prop_str}>'
 
 
 _Tp = TypeVar('_Tp', bound=Plantuml)
 
 
 def try_plantuml(cls: Type[_Tp], *args, **kwargs) -> Tuple[bool, Union[Optional[_Tp], Exception]]:
     """
```

### Comparing `plantumlcli-0.1.0/plantumlcli/models/local.py` & `plantumlcli-0.1.1/plantumlcli/models/local.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,28 +26,28 @@
     return plantuml or find_plantuml_from_env()
 
 
 def _check_local(java: str, plantuml: str):
     if not java:
         raise ValueError('Java executable not given.')
     if not os.path.exists(java):
-        raise FileNotFoundError('Java executable {exec} not found.'.format(exec=repr(java)))
+        raise FileNotFoundError(f'Java executable {java!r} not found.')
     if not os.path.isfile(java):
-        raise IsADirectoryError('Java executable {exec} is not a file.'.format(exec=repr(java)))
+        raise IsADirectoryError(f'Java executable {java!r} is not a file.')
     if not os.access(java, os.X_OK):
-        raise PermissionError('Java executable {exec} not executable.'.format(exec=repr(java)))
+        raise PermissionError(f'Java executable {java!r} not executable.')  # pragma: no cover
 
     if not plantuml:
         raise ValueError('Plantuml jar file not given.')
     if not os.path.exists(plantuml):
-        raise FileNotFoundError('Plantuml jar file {jar} not found.'.format(jar=repr(plantuml)))
+        raise FileNotFoundError(f'Plantuml jar file {plantuml!r} not found.')
     if not os.path.isfile(plantuml):
-        raise IsADirectoryError('Plantuml jar file {jar} is not a file.'.format(jar=repr(plantuml)))
+        raise IsADirectoryError(f'Plantuml jar file {plantuml!r} is not a file.')
     if not os.access(plantuml, os.R_OK):
-        raise PermissionError('Plantuml jar file {jar} not readable.'.format(jar=repr(plantuml)))
+        raise PermissionError(f'Plantuml jar file {plantuml!r} not readable.')  # pragma: no cover
 
 
 class LocalPlantumlExecuteError(CommandLineExecuteError):
     pass
 
 
 class LocalPlantuml(Plantuml):
@@ -96,28 +96,29 @@
         }
 
     def __execute(self, *args) -> Tuple[str, str]:
         return execute(self.__java, '-jar', self.__plantuml, *args, exc=LocalPlantumlExecuteError)
 
     def _check_version(self, version: str):
         if (not version) or ("plantuml" not in version.lower()):
-            raise ValueError("Invalid version of plantuml - {version}.".format(version=repr(version)))
+            raise ValueError(f"Invalid version of plantuml - {version!r}.")
 
     def _get_version(self) -> str:
         _stdout, _ = self.__execute('-version')
         _lines = _stdout.strip().splitlines()
         _first_line = _lines[0].strip() if _lines else ''
         _line, _ = re.subn(r'\([^()]*?\)', '', _first_line)
         _line, _ = re.subn(r'\\s+', '', _line)
         return _line.strip()
 
     def _generate_uml_data(self, type_: PlantumlResourceType, code: str) -> bytes:
         with TemporaryDirectory(prefix='puml') as output_path_name:
             with NamedTemporaryFile(prefix='puml', suffix='.puml') as input_file:
                 save_text_file(input_file.name, code)
-                self.__execute('-t{type}'.format(type=type_.name.lower()), '-o', output_path_name, input_file.name)
+                self.__execute(f'-t{type_.name.lower()}', '-o', output_path_name, input_file.name)
                 _file_list = os.listdir(output_path_name)
                 if _file_list:
                     output_filename = os.path.join(output_path_name, _file_list[0])
                     return load_binary_file(output_filename)
                 else:
-                    raise FileNotFoundError('No expected file found in {path}.'.format(path=repr(output_path_name)))
+                    # When you see this error, it means bug, please open an issue for help us fix this
+                    raise FileNotFoundError(f'No expected file found in {output_path_name!r}.')  # pragma: no cover
```

### Comparing `plantumlcli-0.1.0/plantumlcli/models/remote.py` & `plantumlcli-0.1.1/plantumlcli/models/remote.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import base64
 import os
+import re
 import string
 import zlib
-from typing import Optional, Mapping, Any, Union
+from typing import Optional, Mapping, Any, Union, Tuple
 
 import requests
 from pyquery import PyQuery
 from urlobject import URLObject
 
 from .base import Plantuml, PlantumlResourceType
 
@@ -30,20 +31,19 @@
 
 def _host_process(host: str) -> URLObject:
     return URLObject(host).without_fragment().without_query()
 
 
 def _check_remote(host: str):
     if not host:
-        raise ValueError("Host should be present, but {actual} found.".format(actual=repr(host)))
+        raise ValueError(f"Host should be present, but {host!r} found.")
 
     _host_url = _host_process(host)
     if _host_url.scheme not in ['http', 'https']:
-        raise ValueError(
-            "Host's scheme should be http or https, but {actual} found.".format(actual=repr(_host_url.scheme)))
+        raise ValueError(f"Host's scheme should be http or https, but {_host_url.scheme!r} found.")
 
 
 class RemotePlantuml(Plantuml):
     __BYTE_TRANS = _trans_from_base64_to_plantuml
 
     def __init__(self, host: str, **kwargs):
         """
@@ -96,30 +96,45 @@
         return r
 
     def __get_homepage(self):
         return self.__request('')
 
     def _is_official(self):
         return self.__host.hostname in ('plantuml.com', 'www.plantuml.com') and \
-               len(self.__host.path.segments) > 0 and self.__host.path.segments[0] == 'plantuml'
+            len(self.__host.path.segments) > 0 and self.__host.path.segments[0] == 'plantuml'
 
     def _check_version(self, version: str):
         if not self._is_official():
             if (not version) or ("plantuml" not in version.lower()) or ("version" not in version.lower()):
-                raise ValueError("Invalid version information from homepage - {info}.".format(info=repr(version)))
+                raise ValueError(f"Invalid version information from homepage - {version!r}.")
+
+    def _check_type_supported(self, type_: PlantumlResourceType):
+        if type_ == PlantumlResourceType.PDF:
+            if self._is_official():
+                raise ValueError(f'Resource type {type_!r} not supported for plantuml official site - {self.__host!r}.')
+            else:
+                if self._get_server_version() < (1, 2023):
+                    raise ValueError(f'Resource type {type_!r} not supported for '
+                                     f'plantuml server site lower than 1.2023 - {self._get_server_version()!r}.')
 
     def _get_version(self) -> str:
         if not self._is_official():
             r = self.__get_homepage()
             return PyQuery(r.content.decode()).find('#footer').text().strip()
         else:
             return 'Official Site'
 
+    def _get_server_version(self) -> Tuple[int, int, int]:
+        (major, year, v), = re.findall(r'version\s*(?P<major>\d)(?P<year>\d{4})(?P<v>\d{2})',
+                                       self._get_version(), re.IGNORECASE)
+
+        return int(major), int(year), int(v.lstrip('0') or '0')
+
     def __get_uml_path(self, type_: str, code: str):
-        return "{}/{}".format(type_, self.__compress(code))
+        return f"{type_}/{self.__compress(code)}"
 
     def __get_uml_url(self, type_: str, code: str) -> str:
         return self.__request_url(self.__get_uml_path(type_, code))
 
     def __get_uml(self, type_: str, code: str) -> bytes:
         r = self.__request(self.__get_uml_path(type_, code))
         return r.content
```

### Comparing `plantumlcli-0.1.0/plantumlcli/utils/concurrent.py` & `plantumlcli-0.1.1/plantumlcli/utils/concurrent.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,16 @@
 
 
 def _default_final_error_process(errors: List[Tuple[int, _Ti, Exception]]):
     _, _, err = errors[0]
     raise err
 
 
-def linear_process(items: Iterable[_Ti],
-                   process: Callable[[int, _Ti], _Tr],
-                   post_process: Callable[[int, _Ti, _Tr], None],
-                   concurrency: int = None,
+def linear_process(items: Iterable[_Ti], process: Callable[[int, _Ti], _Tr],  # noqa
+                   post_process: Callable[[int, _Ti, _Tr], None], concurrency: int = None,
                    skip_once_error: bool = True,
                    final_error_process: Optional[Callable[[List[Tuple[int, _Ti, Exception]]], None]] = None):
     concurrency = concurrency or cpu_count()
     pool = ThreadPoolExecutor(max_workers=concurrency)
 
     _items = {index: item for index, item in enumerate(items)}
     _results, _errors = {}, []
```

### Comparing `plantumlcli-0.1.0/plantumlcli/utils/decorator.py` & `plantumlcli-0.1.1/plantumlcli/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.0/plantumlcli/utils/encoding.py` & `plantumlcli-0.1.1/plantumlcli/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.0/plantumlcli/utils/execute.py` & `plantumlcli-0.1.1/plantumlcli/utils/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,15 @@
         return self.__stdout
 
     @property
     def stderr(self) -> Optional[str]:
         return self.__stderr
 
     def __repr__(self):
-        return '<{cls} exitcode: {code}, command_line: {cmd}>'.format(
-            cls=self.__class__.__name__,
-            cmd=repr(self.__command_line),
-            code=repr(self.__exitcode),
-        )
+        return f'<{self.__class__.__name__} exitcode: {self.__exitcode!r}, command_line: {self.__command_line!r}>'
 
     @classmethod
     def try_raise(cls, command_line: Tuple[str], exitcode: int,
                   stdout: Optional[str] = None, stderr: Optional[str] = None, **kwargs):
         if exitcode != 0:
             raise cls(command_line, exitcode, stdout, stderr, **kwargs)
```

### Comparing `plantumlcli-0.1.0/plantumlcli/utils/file.py` & `plantumlcli-0.1.1/plantumlcli/utils/file.py`

 * *Files identical despite different names*

### Comparing `plantumlcli-0.1.0/plantumlcli.egg-info/PKG-INFO` & `plantumlcli-0.1.1/plantumlcli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantumlcli
-Version: 0.1.0
+Version: 0.1.1
 Summary: An easy-to-use plantuml cli for everyone.
 Home-page: https://github.com/HansBug/plantumlcli
 Author: HansBug
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://github.com/HansBug/plantumlcli/blob/main/README.md
 Project-URL: Source, https://github.com/HansBug/plantumlcli
@@ -21,14 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: doc
+Provides-Extra: lint
 License-File: LICENSE
 
 # plantumlcli
 
 [![PyPI](https://img.shields.io/pypi/v/plantumlcli)](https://pypi.org/project/plantumlcli/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/plantumlcli)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/plantumlcli)
```

### Comparing `plantumlcli-0.1.0/plantumlcli.egg-info/SOURCES.txt` & `plantumlcli-0.1.1/plantumlcli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements-doc.txt
+requirements-lint.txt
 requirements-test.txt
 requirements.txt
 setup.py
 plantumlcli/__init__.py
 plantumlcli.egg-info/PKG-INFO
 plantumlcli.egg-info/SOURCES.txt
 plantumlcli.egg-info/dependency_links.txt
```

### Comparing `plantumlcli-0.1.0/setup.py` & `plantumlcli-0.1.1/setup.py`

 * *Files identical despite different names*

