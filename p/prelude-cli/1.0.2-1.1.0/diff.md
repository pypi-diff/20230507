# Comparing `tmp/prelude-cli-1.0.2.tar.gz` & `tmp/prelude-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.0.2.tar", last modified: Fri Apr 28 19:05:44 2023, max compression
+gzip compressed data, was "prelude-cli-1.1.0.tar", last modified: Sun May  7 12:45:14 2023, max compression
```

## Comparing `prelude-cli-1.0.2.tar` & `prelude-cli-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.161214 prelude-cli-1.0.2/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-28 19:05:44.161278 prelude-cli-1.0.2/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.0.2/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.157199 prelude-cli-1.0.2/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1078 2023-04-28 18:41:33.000000 prelude-cli-1.0.2/prelude_cli/cli.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.158362 prelude-cli-1.0.2/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      229 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.160987 prelude-cli-1.0.2/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     3945 2023-03-15 22:01:07.000000 prelude-cli-1.0.2/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     6089 2023-04-18 17:04:09.000000 prelude-cli-1.0.2/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3757 2023-04-21 20:11:38.000000 prelude-cli-1.0.2/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)    29181 2023-04-18 17:04:09.000000 prelude-cli-1.0.2/prelude_cli/views/interactive.py
--rw-r--r--   0 pack       (501) staff       (20)     1508 2023-04-11 22:16:02.000000 prelude-cli-1.0.2/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      272 2023-02-08 14:42:44.000000 prelude-cli-1.0.2/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-04-28 19:05:44.158167 prelude-cli-1.0.2/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      608 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       61 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-04-28 19:05:44.000000 prelude-cli-1.0.2/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.0.2/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      694 2023-04-28 19:05:44.161532 prelude-cli-1.0.2/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:45:14.854406 prelude-cli-1.1.0/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-07 12:45:14.854458 prelude-cli-1.1.0/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.1.0/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:45:14.851429 prelude-cli-1.1.0/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.1.0/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.1.0/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:45:14.852229 prelude-cli-1.1.0/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      241 2023-05-04 16:11:50.000000 prelude-cli-1.1.0/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:45:14.854111 prelude-cli-1.1.0/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     3872 2023-05-07 12:16:47.000000 prelude-cli-1.1.0/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.1.0/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     5021 2023-05-04 16:11:50.000000 prelude-cli-1.1.0/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     3256 2023-05-03 13:30:52.000000 prelude-cli-1.1.0/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     2246 2023-05-03 13:30:52.000000 prelude-cli-1.1.0/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.1.0/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-05-07 12:45:14.852046 prelude-cli-1.1.0/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-05-07 12:45:14.000000 prelude-cli-1.1.0/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.1.0/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-05-07 12:45:14.854682 prelude-cli-1.1.0/setup.cfg
```

### Comparing `prelude-cli-1.0.2/LICENSE` & `prelude-cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.2/PKG-INFO` & `prelude-cli-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.0.2/prelude_cli/views/build.py` & `prelude-cli-1.1.0/prelude_cli/views/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import prelude_cli.templates as templates
 import importlib.resources as pkg_resources
 
 from rich import print_json
 from datetime import datetime
 from pathlib import Path, PurePath
 
-from prelude_cli.views.shared import handle_api_error
+from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.build_controller import BuildController
 
 
 UUID = re.compile('[a-f0-9]{8}-?[a-f0-9]{4}-?4[a-f0-9]{3}-?[89ab][a-f0-9]{3}-?[a-f0-9]{12}')
 
 
 @click.group()
@@ -24,66 +24,75 @@
 
 @build.command('test')
 @click.argument('test_id')
 @click.pass_obj
 @handle_api_error
 def get_test(controller, test_id):
     """ List properties for a test """
-    print_json(data=controller.get_test(test_id=test_id))
+    with Spinner():
+        data = controller.get_test(test_id=test_id)
+    print_json(data=data)
 
 
 @build.command('create-test')
 @click.argument('name')
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
+@click.option('-u', '--unit', required=True, help='unit identifier', default=None, type=str)
+@click.option('-a', '--alert', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, type=str)
 @click.pass_obj
 @handle_api_error
-def create_test(controller, name, test):
+def create_test(controller, name, test, unit, alert):
     """ Create or update a security test """
     test_id = test or str(uuid.uuid4())
-    controller.create_test(test_id=test_id, name=name)
+    with Spinner():
+        controller.create_test(test_id=test_id, name=name, unit=unit, alert=alert)
 
     if not test:
         basename = f'{test_id}.go'
         template = pkg_resources.read_text(templates, 'template.go')
         template = template.replace('$ID', test_id)
         template = template.replace('$NAME', name)
+        template = template.replace('$UNIT', unit or '')
         template = template.replace('$CREATED', str(datetime.utcnow()))
-        controller.upload(test_id=test_id, filename=basename, data=template)
+        with Spinner():
+            controller.upload(test_id=test_id, filename=basename, data=template)
 
         with open(basename, 'w') as test_code:
             test_code.write(template)
             click.secho(f'Created {basename}', fg='green')
 
 
 @build.command('delete-test')
 @click.argument('test')
-@click.option('-t', '--test', help='test identifier', default=None, type=str)
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_test(controller, test):
     """ Delete a test """
-    controller.delete_test(test_id=test)
+    with Spinner():
+        controller.delete_test(test_id=test)
     click.secho(f'Deleted {test}', fg='green')
 
 
 @build.command('download')
 @click.argument('test')
 @click.pass_obj
 @handle_api_error
 def download(controller, test):
     """ Download a test to your local environment """
     click.secho(f'Downloading {test}')
     Path(test).mkdir(parents=True, exist_ok=True)
+    with Spinner():
+        attachments = controller.get_test(test_id=test).get('attachments')
 
-    for attach in controller.get_test(test_id=test).get('attachments'):
-        if Path(attach).suffix:
-            code = controller.download(test_id=test, filename=attach)
-            with open(PurePath(test, attach), 'wb') as f:
-                f.write(code)
+        for attach in attachments:
+            if Path(attach).suffix:
+                code = controller.download(test_id=test, filename=attach)
+                with open(PurePath(test, attach), 'wb') as f:
+                    f.write(code)
 
 
 @build.command('upload')
 @click.argument('path', type=click.Path(exists=True))
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
 @click.pass_obj
 @handle_api_error
@@ -93,37 +102,18 @@
         match = UUID.search(path)
         if match:
             return match.group(0)
         raise FileNotFoundError('You must supply a test ID or include it in the path')
 
     def upload(p: Path):
         with open(p, 'rb') as data:
-            controller.upload(test_id=identifier, filename=p.name, data=data.read(), binary=True)
+            with Spinner():
+                controller.upload(test_id=identifier, filename=p.name, data=data.read(), binary=True)
             click.secho(f'Uploaded {path}', fg='green')
 
     identifier = test or test_id()
     
     if Path(path).is_file():
         upload(p=Path(path))
     else:
         for obj in Path(path).rglob('*'):
             upload(p=Path(obj))
-
-
-@build.command('map')
-@click.argument('test')
-@click.argument('identifier')
-@click.pass_obj
-@handle_api_error
-def map(controller, test, identifier):
-    """ Map an identifier to a test """
-    print_json(data=controller.map(test_id=test, x=identifier))
-
-
-@build.command('unmap')
-@click.argument('test')
-@click.argument('identifier')
-@click.pass_obj
-@handle_api_error
-def unmap(controller, test, identifier):
-    """ Unmap an identifier from a test """
-    print_json(data=controller.unmap(test_id=test, x=identifier))
```

### Comparing `prelude-cli-1.0.2/prelude_cli/views/configure.py` & `prelude-cli-1.1.0/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.0.2/prelude_cli/views/detect.py` & `prelude-cli-1.1.0/prelude_cli/views/detect.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
 from rich import print_json
-from datetime import datetime, timedelta, time
+from datetime import datetime, timedelta
 
-from prelude_cli.views.shared import handle_api_error
-from prelude_sdk.models.codes import Decision, RunCode
+from prelude_sdk.models.codes import RunCode
+from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.detect_controller import DetectController
 
 
 @click.group()
 @click.pass_context
 def detect(ctx):
     """ Continuous security testing """
@@ -21,148 +21,123 @@
 @click.option('-e', '--edr_id', help='EDR id', type=str, default='')
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default='')
 @click.option('-i', '--endpoint_id', help='update a specific endpoint_id with the provided values', type=str, default='')
 @click.pass_obj
 @handle_api_error
 def register_endpoint(controller, host, serial_num, edr_id, tags, endpoint_id):
     """ Register a new endpoint """
-    token = controller.register_endpoint(host=host, serial_num=serial_num, edr_id=edr_id, tags=tags, endpoint_id=endpoint_id)
+    with Spinner():
+        token = controller.register_endpoint(host=host, serial_num=serial_num, edr_id=edr_id, tags=tags, endpoint_id=endpoint_id)
     click.secho(token)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
     """ List all security tests """
-    print_json(data=controller.list_tests())
+    with Spinner():
+        data = controller.list_tests()
+    print_json(data=data)
 
 
 @detect.command('enable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only enable for these tags (comma-separated list)', type=str, default='')
 @click.option('-r', '--run_code',
               help='provide a run_code',
               default=RunCode.DAILY.name, show_default=True,
               type=click.Choice([r.name for r in RunCode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def enable_test(controller, test, run_code, tags):
     """ Add test to your queue """
-    controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
+    with Spinner():
+        controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
 
 
 @detect.command('disable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only disable for these tags (comma-separated list)', type=str, default='')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def disable_test(controller, test, tags):
     """ Remove test from your queue """
-    controller.disable_test(ident=test, tags=tags)
+    with Spinner():
+        controller.disable_test(ident=test, tags=tags)
 
 
 @detect.command('social-stats')
 @click.argument('test')
 @click.option('-d', '--days', help='days to look back', default=30, type=int, show_default=True)
 @click.pass_obj
 @handle_api_error
 def social_statistics(controller, test, days):
     """ Pull social statistics for a specific test """
-    print_json(data=controller.social_stats(ident=test, days=days))
+    with Spinner():
+        data = controller.social_stats(ident=test, days=days)
+    print_json(data=data)
 
 
 @detect.command('delete-endpoint')
 @click.argument('endpoint_id')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_endpoint(controller, endpoint_id):
     """Delete a probe/endpoint"""
-    controller.delete_endpoint(ident=endpoint_id)
+    with Spinner():
+        controller.delete_endpoint(ident=endpoint_id)
 
 
 @detect.command('queue')
 @click.pass_obj
 @handle_api_error
 def queue(controller):
     """ List all tests in your active queue """
-    print_json(data=controller.list_queue())
-
-
-@detect.command('search')
-@click.argument('cve')
-@click.pass_obj
-@handle_api_error
-def search(controller, cve):
-    """ Search the NVD for a specific CVE identifier """
-    print("This product uses the NVD API but is not endorsed or certified by the NVD.\n")
-    print_json(data=controller.search(identifier=cve))
+    with Spinner():
+        data = controller.list_queue()
+    print_json(data=data)
 
 
 @detect.command('endpoints')
 @click.option('-d', '--days', help='only show endpoints that have run at least once in the past DAYS days', default=90, type=int)
 @click.pass_obj
 @handle_api_error
 def endpoints(controller, days):
     """ List all active endpoints associated to your account """
-    print_json(data=controller.list_endpoints(days=days))
-
-
-@detect.command('recommendations')
-@click.pass_obj
-@handle_api_error
-def recommendation(controller):
-    """ Print all security recommendations """
-    print_json(data=controller.recommendations())
-
-
-@detect.command('add-recommendation')
-@click.argument('title')
-@click.argument('description')
-@click.pass_obj
-@handle_api_error
-def add_recommendation(controller, title, description):
-    """ Create a new security recommendation """
-    controller.create_recommendation(title=title, description=description)
-
-
-@detect.command('decide-recommendation')
-@click.argument('id')
-@click.option('-d', '--decision', help='approve or deny the recommendation', default=Decision.APPROVE.name,
-              type=click.Choice([d.name for d in Decision], case_sensitive=False), show_default=True)
-@click.pass_obj
-@handle_api_error
-def decide_recommendation(controller, id, decision):
-    """ Update a security recommendation decision """
-    controller.make_decision(id=id, decision=Decision[decision.upper()].value)
+    with Spinner():
+        data = controller.list_endpoints(days=days)
+    print_json(data=data)
 
 
 @detect.command('activity')
 @click.option('-v', '--view',
               help='retrieve a specific result view',
               default='logs', show_default=True,
-              type=click.Choice(['logs', 'days', 'insights', 'probes', 'rules']))
+              type=click.Choice(['logs', 'days', 'insights', 'probes', 'units']))
 @click.option('-d', '--days', help='days to look back', default=30, type=int)
 @click.option('--tests', help='comma-separated list of test IDs', type=str)
 @click.option('--tags', help='comma-separated list of tags', type=str)
 @click.option('--endpoints', help='comma-separated list of endpoint IDs', type=str)
 @click.option('--dos', help='comma-separated list of DOS', type=str)
 @click.pass_obj
 @handle_api_error
 def describe_activity(controller, days, view, tests, tags, endpoints, dos):
     """ View my Detect results """
     filters = dict(
-        start=datetime.combine(datetime.utcnow() - timedelta(days=days), time.min),
-        finish=datetime.combine(datetime.utcnow(), time.max)
+        start=datetime.utcnow() - timedelta(days=days),
+        finish=datetime.utcnow() + timedelta(days=1)
     )
     if tests:
         filters['tests'] = tests
     if tags:
         filters['tags'] = tags
     if endpoints:
         filters['endpoints'] = endpoints
     if dos:
         filters['dos'] = dos
 
-    print_json(data=controller.describe_activity(view=view, filters=filters))
+    with Spinner():
+        data = controller.describe_activity(view=view, filters=filters)
+    print_json(data=data)
```

### Comparing `prelude-cli-1.0.2/prelude_cli/views/iam.py` & `prelude-cli-1.1.0/prelude_cli/views/iam.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import click
 
 from rich import print_json
 from datetime import datetime, timedelta
 
-from prelude_cli.views.shared import handle_api_error
 from prelude_sdk.models.codes import Permission, Mode
+from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.iam_controller import IAMController
 
 
 @click.group()
 @click.pass_context
 def iam(ctx):
     """ Prelude account management """
@@ -17,100 +17,88 @@
 
 @iam.command('create-account')
 @click.pass_obj
 @handle_api_error
 @click.confirmation_option(prompt='Overwrite local account credentials for selected profile?')
 def register_account(controller):
     """ Register a new account """
-    creds = controller.new_account(handle=click.prompt('Enter a handle'))
-    print_json(data=creds)
+    handle = click.prompt('Enter a handle')
+    with Spinner():
+        data = controller.new_account(handle=handle)
+    print_json(data=data)
     print("\nCheck your email to verify your account.\n")
 
 
 @iam.command('update-account')
 @click.option('-m', '--mode',
               help='provide a mode',
               default=Mode.MANUAL.name, show_default=True,
               type=click.Choice([m.name for m in Mode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def update_account(controller, mode):
     """ Update an account """
-    controller.update_account(mode=Mode[mode.upper()].value)
+    with Spinner():
+        controller.update_account(mode=Mode[mode.upper()].value)
 
 
 @iam.command('account')
 @click.pass_obj
 @handle_api_error
 def describe_account(controller):
     """ Get account details """
-    print_json(data=controller.get_account())
+    with Spinner():
+        data = controller.get_account()
+    print_json(data=data)
 
 
 @iam.command('create-user')
 @click.option('-d', '--days', help='days this account should remain active', default=365, type=int)
 @click.option('-p', '--permission', help='provide a permission level', default=Permission.SERVICE.name,
               type=click.Choice([p.name for p in Permission], case_sensitive=False), show_default=True)
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def create_user(controller, permission, handle, days):
     """ Create a new user in your account """
     expires = datetime.utcnow() + timedelta(days=days)
-    resp = controller.create_user(
-        handle=handle, 
-        permission=Permission[permission.upper()].value, 
-        expires=expires
-    )
-    print_json(data=resp)
+    with Spinner():
+        data = controller.create_user(
+            handle=handle,
+            permission=Permission[permission.upper()].value,
+            expires=expires
+        )
+    print_json(data=data)
     if permission != Permission.SERVICE.name:
         print("\nCheck your email to verify your account.\n")
 
 @iam.command('delete-user')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
     """ Remove a user from your account """
-    controller.delete_user(handle=handle)
-
-
-@iam.command('attach-partner')
-@click.argument('name')
-@click.option('--api', default='', help='API endpoint of the partner')
-@click.option('--user', default='', help='user identifier')
-@click.option('--secret', default='', help='secret for OAUTH use cases')
-@click.pass_obj
-@handle_api_error
-def attach_partner(controller, name, api, user, secret):
-    """ Attach an EDR to Detect """
-    controller.attach_partner(name=name, api=api, user=user, secret=secret)
-
-
-@iam.command('detach-partner')
-@click.confirmation_option(prompt='Are you sure?')
-@click.argument('name')
-@click.pass_obj
-@handle_api_error
-def detach_partner(controller, name):
-    """ Detach an existing partner from your account """
-    controller.detach_partner(name=name)
+    with Spinner():
+        controller.delete_user(handle=handle)
 
 
 @iam.command('logs')
 @click.option('-d', '--days', help='days back to search from today', default=7, type=int)
 @click.option('-l', '--limit', help='limit the number of results', default=1000, type=int)
 @click.pass_obj
 @handle_api_error
 def logs(controller, days, limit):
     """ Get audit logs """
-    print_json(data=controller.audit_logs(days=days, limit=limit))
+    with Spinner():
+        data = controller.audit_logs(days=days, limit=limit)
+    print_json(data=data)
 
 
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def purge(controller):
     """ Delete your account """
-    controller.purge_account()
+    with Spinner():
+        controller.purge_account()
```

### Comparing `prelude-cli-1.0.2/prelude_cli/views/partner.py` & `prelude-cli-1.1.0/prelude_cli/views/partner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 import click
 
 from rich import print_json
 
-from prelude_cli.views.shared import handle_api_error
+from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.partner_controller import PartnerController
 
 
 @click.group()
 @click.pass_context
 def partner(ctx):
     """ Partner system commands """
     ctx.obj = PartnerController(account=ctx.obj)
 
 
+@partner.command('attach')
+@click.argument('name')
+@click.option('--api', default='', help='API endpoint of the partner')
+@click.option('--user', default='', help='user identifier')
+@click.option('--secret', default='', help='secret for OAUTH use cases')
+@click.pass_obj
+@handle_api_error
+def attach_partner(controller, name, api, user, secret):
+    """ Attach an EDR to Detect """
+    with Spinner():
+        controller.attach(name=name, api=api, user=user, secret=secret)
+
+
+@partner.command('detach')
+@click.confirmation_option(prompt='Are you sure?')
+@click.argument('name')
+@click.pass_obj
+@handle_api_error
+def detach_partner(controller, name):
+    """ Detach an existing partner from your account """
+    with Spinner():
+        controller.detach(name=name)
+
+
 @partner.command('endpoints')
-@click.option('--name', required=True, help='partner name (e.g. "CrowdStrike")')
+@click.argument('name')
 @click.option('--platform', required=True, help='platform name (e.g. "windows")', type=click.Choice(['windows', 'linux', 'darwin'], case_sensitive=False))
 @click.option('--hostname', default='', help='hostname pattern (e.g. "mycompany-c24oi444")')
 @click.option('--offset', default=0, help='API pagination offset', type=int)
 @click.pass_obj
 @handle_api_error
 def partner_endpoints(controller, name, platform, hostname, offset):
-    """ Get a list of endpoints from all partners """
-    print_json(data=controller.endpoints(partner_name=name, platform=platform, hostname=hostname, offset=offset))
+    """ Get a list of endpoints from a partner """
+    with Spinner():
+        data = controller.endpoints(partner_name=name, platform=platform, hostname=hostname, offset=offset)
+    print_json(data=data)
 
 
 @partner.command('deploy')
 @click.confirmation_option(prompt='Are you sure?')
-@click.option('--name', required=True, help='partner name (e.g. "CrowdStrike")')
+@click.argument('name')
 @click.option('--host_ids', required=True, help='a list of host IDs to deploy to', multiple=True, default=[])
 @click.pass_obj
 @handle_api_error
 def partner_deploy(controller, name, host_ids):
     """ Deploy probes to hosts associated to a partner """
-    print_json(data=controller.deploy(partner_name=name, host_ids=host_ids))
+    with Spinner():
+        data = controller.deploy(partner_name=name, host_ids=host_ids)
+    print_json(data=data)
```

### Comparing `prelude-cli-1.0.2/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.1.0/prelude_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.0.2
+Version: 1.1.0
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

