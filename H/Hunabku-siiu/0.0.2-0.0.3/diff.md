# Comparing `tmp/Hunabku_siiu-0.0.2.tar.gz` & `tmp/Hunabku_siiu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Hunabku_siiu-0.0.2.tar", last modified: Sun Apr 16 08:07:16 2023, max compression
+gzip compressed data, was "Hunabku_siiu-0.0.3.tar", last modified: Sun May  7 18:37:12 2023, max compression
```

## Comparing `Hunabku_siiu-0.0.2.tar` & `Hunabku_siiu-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-16 08:07:16.000000 Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/hunabku_siiu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/SIIU.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 08:07:16.570952 Hunabku_siiu-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-16 08:06:57.000000 Hunabku_siiu-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-07 18:37:12.000000 Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/hunabku_siiu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/SIIU.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:37:12.462653 Hunabku_siiu-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-07 18:36:52.000000 Hunabku_siiu-0.0.3/setup.py
```

### Comparing `Hunabku_siiu-0.0.2/Hunabku_siiu.egg-info/PKG-INFO` & `Hunabku_siiu-0.0.3/Hunabku_siiu.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku-siiu
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.2/PKG-INFO` & `Hunabku_siiu-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Hunabku_siiu
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hunabku plguin
 Home-page: https://github.com/colav/Hunabku_plugins
 Author: Colav
 Author-email: colav@udea.edu.co
 License: BSD
 Description-Content-Type: text/markdown
```

### Comparing `Hunabku_siiu-0.0.2/README.md` & `Hunabku_siiu-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Hunabku_siiu-0.0.2/hunabku_siiu/endpoints/SIIU.py` & `Hunabku_siiu-0.0.3/hunabku_siiu/endpoints/SIIU.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from hunabku.HunabkuBase import HunabkuPluginBase, endpoint
 from hunabku.Config import Config, Param
 from pymongo import MongoClient
 from elasticsearch import Elasticsearch, helpers
 from elasticsearch_dsl import Search
 import time
 
+
 class SIIU(HunabkuPluginBase):
     config = Config()
     config += Param(mdb_uri="mongodb://localhost:27017/",
                     doc="MongoDB string connection")
     config += Param(mdb_name="siiu",
                     doc="MongoDB name for SIIU")
     config += Param(es_uri="http://localhost:9200",
@@ -37,31 +38,39 @@
                         The search by keyword perform a search in teh fields of text
                         NOMBRE_CORTO, NOMBRE_COMPLETO, PALABRAS_CLAVES, descriptive_text.TEXTO_INGRESADO
                         lots of text where indexed for this search.
 
         @apiParam {String} apikey  Credential for authentication
         @apiParam {String} search  keyword for text search.
         @apiParam {String} CODIGO  project id.
+        @apiParam {String} group_code  Colciencias Group ID ex:"COL0008423"
+        @apiParam {String} group_name  name of the research group (returns the projects for this group)
 
         @apiSuccess {Object}  Resgisters from MongoDB in Json format.
 
         @apiError (Error 401) msg  The HTTP 401 Unauthorized invalid authentication apikey for the target resource.
         @apiError (Error 400) msg  Bad request, if the query is not right.
 
         @apiExample {curl} Example usage:
             # all the products for the user
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&search=keyword
             # An specific product
             curl -i http://apis.colav.co/siiu/project?apikey=XXXX&CODIGO=2013-86
+            # An projects given a group id
+            curl -i http://apis.colav.co/siiu/project?apikey=XXXX&group_code=COL0008423
+            # An projects given a group name
+            curl -i http://apis.colav.co/siiu/project?apikey=XXXX&group_name="psicologia cognitiva"
 
         """
         if self.valid_apikey():
 
             keyword = self.request.args.get('search')
             codigo = self.request.args.get('CODIGO')
+            grp_codigo = self.request.args.get('group_code')
+            group_name = self.request.args.get('group_name')
             if keyword:
                 if not self.es.indices.exists(index=self.config.es_project_index):
                     response = self.app.response_class(
                         response=self.json.dumps(
                             {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
                         status=500,
                         mimetype='application/json'
@@ -90,25 +99,75 @@
                     status=200,
                     mimetype='application/json'
                 )
                 # get the end time
                 et = time.time()
                 # get the execution time
                 elapsed_time = et - st
-                print(f'Search for "{keyword}" Execution time:', elapsed_time, 'seconds')
+                print(f'Search for "{keyword}" Execution time:',
+                      elapsed_time, 'seconds')
                 return response
             if codigo:
                 data = list(self.dbclient[self.config.mdb_name]
                             ["project"].find({'CODIGO': codigo}, {'_id': 0, }))
                 response = self.app.response_class(
                     response=self.json.dumps(data),
                     status=200,
                     mimetype='application/json'
                 )
                 return response
+            if grp_codigo:
+                data = list(self.dbclient[self.config.mdb_name]
+                            ["project"].find({"project_participant.group.CODIGO_COLCIENCIAS": grp_codigo}, {"_id": 0}))
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                return response
+
+            if group_name:
+                if not self.es.indices.exists(index=self.config.es_project_index):
+                    response = self.app.response_class(
+                        response=self.json.dumps(
+                            {"msg": f"Internal error, index {self.config.es_project_index} not found in Elastic Search"}),
+                        status=500,
+                        mimetype='application/json'
+                    )
+                    return response
+                body = {
+                    "query": {
+                        "bool": {
+                            "must": [
+                                {"match_phrase": {
+                                    "project_participant.group.NOMBRE_COMPLETO":  group_name}},
+                            ]
+                        }
+                    }
+                }
+
+                # get the start time
+                st = time.time()
+                s = Search(using=self.es, index=self.config.es_project_index)
+                s = s.update_from_dict(body)
+                s = s.extra(track_total_hits=True)
+                s.execute()
+                data = [hit.to_dict() for hit in s.scan()]
+                response = self.app.response_class(
+                    response=self.json.dumps(data),
+                    status=200,
+                    mimetype='application/json'
+                )
+                # get the end time
+                et = time.time()
+                # get the execution time
+                elapsed_time = et - st
+                print(f'Search for "{group_name}" Execution time:',
+                      elapsed_time, 'seconds')
+                return response
 
             data = {
                 "error": "Bad Request", "message": "invalid parameters, please select the right combination of parameters."}
             response = self.app.response_class(
                 response=self.json.dumps(data),
                 status=400,
                 mimetype='application/json'
```

### Comparing `Hunabku_siiu-0.0.2/setup.py` & `Hunabku_siiu-0.0.3/setup.py`

 * *Files identical despite different names*

