# Comparing `tmp/safrs-3.0.3.tar.gz` & `tmp/safrs-3.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safrs-3.0.3.tar", last modified: Mon Apr 24 17:20:34 2023, max compression
+gzip compressed data, was "safrs-3.0.4.tar", last modified: Sun May  7 19:16:40 2023, max compression
```

## Comparing `safrs-3.0.3.tar` & `safrs-3.0.4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.221684 safrs-3.0.3/
--rwxrwxrwx   0 t         (1000) t         (1000)    35120 2023-02-11 17:18:46.000000 safrs-3.0.3/LICENSE
--rwxrwxrwx   0 t         (1000) t         (1000)       90 2021-03-16 11:22:28.000000 safrs-3.0.3/MANIFEST.in
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-24 17:20:34.221684 safrs-3.0.3/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)    16881 2023-02-18 08:57:06.000000 safrs-3.0.3/README.md
--rwxrwxrwx   0 t         (1000) t         (1000)     1374 2023-02-11 17:18:46.000000 safrs-3.0.3/README.rst
--rwxrwxrwx   0 t         (1000) t         (1000)     1422 2023-04-24 17:19:50.000000 safrs-3.0.3/pyproject.toml
--rwxrwxrwx   0 t         (1000) t         (1000)      433 2023-02-11 20:26:11.000000 safrs-3.0.3/requirements.txt
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.210979 safrs-3.0.3/safrs/
--rwxrwxrwx   0 t         (1000) t         (1000)       93 2023-04-24 17:20:18.000000 safrs-3.0.3/safrs/__about__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1242 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/__init__.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1980 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/_safrs_relationship.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4082 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/api_methods.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3349 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/attr_parse.py
--rwxrwxrwx   0 t         (1000) t         (1000)    49278 2023-04-17 19:48:20.000000 safrs-3.0.3/safrs/base.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4047 2023-02-11 20:14:12.000000 safrs-3.0.3/safrs/config.py
--rwxrwxrwx   0 t         (1000) t         (1000)     3782 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/errors.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1401 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/jabase.py
--rwxrwxrwx   0 t         (1000) t         (1000)     4531 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/json_encoder.py
--rwxrwxrwx   0 t         (1000) t         (1000)    41386 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1682 2023-02-11 20:14:16.000000 safrs-3.0.3/safrs/jsonapi_attr.py
--rwxrwxrwx   0 t         (1000) t         (1000)     5857 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi_filters.py
--rwxrwxrwx   0 t         (1000) t         (1000)     9866 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/jsonapi_formatting.py
--rwxrwxrwx   0 t         (1000) t         (1000)     5188 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/request.py
--rwxrwxrwx   0 t         (1000) t         (1000)      262 2023-02-11 17:18:47.000000 safrs-3.0.3/safrs/response.py
--rwxrwxrwx   0 t         (1000) t         (1000)    31273 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_api.py
--rwxrwxrwx   0 t         (1000) t         (1000)     6085 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_init.py
--rwxrwxrwx   0 t         (1000) t         (1000)     7458 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/safrs_types.py
--rwxrwxrwx   0 t         (1000) t         (1000)    26470 2023-02-18 08:46:45.000000 safrs-3.0.3/safrs/swagger_doc.py
--rwxrwxrwx   0 t         (1000) t         (1000)     1205 2023-02-18 08:46:44.000000 safrs-3.0.3/safrs/util.py
-drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-04-24 17:20:34.220493 safrs-3.0.3/safrs.egg-info/
--rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/PKG-INFO
--rwxrwxrwx   0 t         (1000) t         (1000)      648 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/SOURCES.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        1 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/dependency_links.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      522 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/requires.txt
--rwxrwxrwx   0 t         (1000) t         (1000)        6 2023-04-24 17:20:34.000000 safrs-3.0.3/safrs.egg-info/top_level.txt
--rwxrwxrwx   0 t         (1000) t         (1000)      263 2023-04-24 17:20:34.223867 safrs-3.0.3/setup.cfg
--rwxrwxrwx   0 t         (1000) t         (1000)     1687 2023-04-24 17:20:28.000000 safrs-3.0.3/setup.py
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.261346 safrs-3.0.4/
+-rwxrwxrwx   0 t         (1000) t         (1000)    35120 2023-02-11 17:18:46.000000 safrs-3.0.4/LICENSE
+-rwxrwxrwx   0 t         (1000) t         (1000)       90 2021-03-16 11:22:28.000000 safrs-3.0.4/MANIFEST.in
+-rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-05-07 19:16:40.262343 safrs-3.0.4/PKG-INFO
+-rwxrwxrwx   0 t         (1000) t         (1000)    16881 2023-02-18 08:57:06.000000 safrs-3.0.4/README.md
+-rwxrwxrwx   0 t         (1000) t         (1000)     1374 2023-02-11 17:18:46.000000 safrs-3.0.4/README.rst
+-rwxrwxrwx   0 t         (1000) t         (1000)     1422 2023-05-07 19:15:35.000000 safrs-3.0.4/pyproject.toml
+-rwxrwxrwx   0 t         (1000) t         (1000)      433 2023-05-07 19:11:08.000000 safrs-3.0.4/requirements.txt
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.249378 safrs-3.0.4/safrs/
+-rwxrwxrwx   0 t         (1000) t         (1000)       93 2023-05-07 19:15:49.000000 safrs-3.0.4/safrs/__about__.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1242 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/__init__.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1980 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/_safrs_relationship.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4082 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/api_methods.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     3349 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/attr_parse.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    49491 2023-05-01 07:36:38.000000 safrs-3.0.4/safrs/base.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4047 2023-02-11 20:14:12.000000 safrs-3.0.4/safrs/config.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     3782 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/errors.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1401 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/jabase.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     4531 2023-05-07 19:01:25.000000 safrs-3.0.4/safrs/json_encoder.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    41386 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1682 2023-02-11 20:14:16.000000 safrs-3.0.4/safrs/jsonapi_attr.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     5857 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi_filters.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     9866 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/jsonapi_formatting.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     6290 2023-05-07 19:03:35.000000 safrs-3.0.4/safrs/request.py
+-rwxrwxrwx   0 t         (1000) t         (1000)      262 2023-02-11 17:18:47.000000 safrs-3.0.4/safrs/response.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    31273 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/safrs_api.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     6085 2023-05-07 19:00:53.000000 safrs-3.0.4/safrs/safrs_init.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     7458 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/safrs_types.py
+-rwxrwxrwx   0 t         (1000) t         (1000)    26470 2023-02-18 08:46:45.000000 safrs-3.0.4/safrs/swagger_doc.py
+-rwxrwxrwx   0 t         (1000) t         (1000)     1205 2023-02-18 08:46:44.000000 safrs-3.0.4/safrs/util.py
+drwxrwxrwx   0 t         (1000) t         (1000)        0 2023-05-07 19:16:40.260348 safrs-3.0.4/safrs.egg-info/
+-rwxrwxrwx   0 t         (1000) t         (1000)     2665 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/PKG-INFO
+-rwxrwxrwx   0 t         (1000) t         (1000)      648 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/SOURCES.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)        1 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/dependency_links.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)      522 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/requires.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)        6 2023-05-07 19:16:40.000000 safrs-3.0.4/safrs.egg-info/top_level.txt
+-rwxrwxrwx   0 t         (1000) t         (1000)      263 2023-05-07 19:16:40.263340 safrs-3.0.4/setup.cfg
+-rwxrwxrwx   0 t         (1000) t         (1000)     1687 2023-05-07 19:15:26.000000 safrs-3.0.4/setup.py
```

### Comparing `safrs-3.0.3/LICENSE` & `safrs-3.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/PKG-INFO` & `safrs-3.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.3
+Version: 3.0.4
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.3.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.4.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.3/README.md` & `safrs-3.0.4/README.md`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/README.rst` & `safrs-3.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/pyproject.toml` & `safrs-3.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "safrs"
 
-version = "3.0.3"
+version = "3.0.4"
 
 description="SAFRS : SqlAlchemy Flask-Restful Swagger"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
```

### Comparing `safrs-3.0.3/safrs/__init__.py` & `safrs-3.0.4/safrs/__init__.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/_safrs_relationship.py` & `safrs-3.0.4/safrs/_safrs_relationship.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/api_methods.py` & `safrs-3.0.4/safrs/api_methods.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/attr_parse.py` & `safrs-3.0.4/safrs/attr_parse.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/base.py` & `safrs-3.0.4/safrs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 
     db_commit = True  # commit instances automatically, see also _s_auto_commit property below
     url_prefix = ""
     allow_client_generated_ids = False  # Indicates whether the client is allowed to create the id
     exclude_attrs = []  # list of attribute names that should not be serialized
     exclude_rels = []  # list of relationship names that should not be serialized
     supports_includes = True  # Set to False if you don't want this class to return included items
-
+    
     # The swagger models are kept here, this lookup table will be used when the api swagger is generated
     # on startup
     swagger_models = {"instance": None, "collection": None}
     _s_expose = True  # indicates we want to expose this (see _s_check_perms)
     jsonapi_filter = jsonapi_filter  # filtering implementation
 
     # Cached lookup tables
@@ -114,14 +114,17 @@
     _rpc_api = safrs.jsonapi.SAFRSJSONRPCAPI
 
     _s_upsert = True  # indicates we want to lookup and use existing objects
     _s_allow_add_rels = True  # allow relationships to be added in post requests
 
     _s_pk_delimiter = "_"
 
+    _s_url_root = None # url prefix shown in the "links" field, if not set, request.url_root will be 
+
+    
     included_list = None
 
     def __new__(cls, *args, **kwargs):
         """
         If an object with given arguments already exists, this object is instantiated
         """
         if "id" not in kwargs or not cls._s_upsert:
@@ -861,15 +864,15 @@
                         # create an Included instance that will be used for serialization eventually
                         data = Included(rel_item, next_included_list)
                 elif relationship.direction in (ONETOMANY, MANYTOMANY):
                     # manytoone relationship contains a list of instances
                     # Data is optional, it's also really slow for large sets!
                     data = []
                     rel_query = getattr(self, rel_name)
-                    limit = request.page_limit
+                    limit = request.get_page_limit(rel_name)
                     if not get_config("ENABLE_RELATIONSHIPS"):
                         meta["warning"] = "ENABLE_RELATIONSHIPS set to false in config.py"
                     elif rel_query:
                         # todo: check if lazy=dynamic
                         # In order to work with the relationship as with Query,
                         # you need to configure it with lazy='dynamic'
                         # "limit" may not be possible !
@@ -912,23 +915,25 @@
 
     @classmethod
     def _s_count(cls):
         """
         returning None will cause our jsonapi to perform a count() on the result
         this can be overridden with a cached value for performance on large tables (>1G)
         """
+        max_table_count =  get_config("MAX_TABLE_COUNT")
+        
         try:
             count = cls.jsonapi_filter().count()
         except Exception as exc:
             # May happen for custom types, for ex. the psycopg2 extension
             safrs.log.warning(f"Can't get count for {cls} ({exc})")
             count = -1
 
-        if get_config("MAX_TABLE_COUNT"):
-            safrs.log.warning(f"Large table count detected, performance may be impacted, consider '{cls.__name__}._s_count' override")
+        if count > max_table_count:
+            safrs.log.warning(f"Large table count detected ({count}>{max_table_count}), performance may be impacted, consider '{cls.__name__}._s_count' override")
 
         return count
 
     #
     # Following methods are used to create the swagger2 API documentation
     #
     @classmethod
@@ -1074,25 +1079,25 @@
         """
         :param url_prefix:
         :return: endpoint url of this instance
         """
         try:
             params = {self._s_object_id: self.jsonapi_id}
             instance_url = url_for(self.get_endpoint(type="instance"), **params)
-            result = urljoin(request.url_root, instance_url)
+            result = urljoin(self._s_url_root, instance_url)
         except RuntimeError:
             # This happens when creating the swagger doc and there is no application registered
             result = ""
         return result
 
     @_s_url.expression
     def _s_url(cls, url_prefix=""):
         try:
             collection_url = url_for(cls.get_endpoint())
-            result = urljoin(request.url_root, collection_url)
+            result = urljoin(cls._s_url_root, collection_url)
         except RuntimeError:
             # This happens when creating the swagger doc and there is no application registered
             result = ""
         return result
 
     @classmethod
     def _s_meta(cls):
```

### Comparing `safrs-3.0.3/safrs/config.py` & `safrs-3.0.4/safrs/config.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/errors.py` & `safrs-3.0.4/safrs/errors.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/jabase.py` & `safrs-3.0.4/safrs/jabase.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/json_encoder.py` & `safrs-3.0.4/safrs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/jsonapi.py` & `safrs-3.0.4/safrs/jsonapi.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/jsonapi_attr.py` & `safrs-3.0.4/safrs/jsonapi_attr.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/jsonapi_filters.py` & `safrs-3.0.4/safrs/jsonapi_filters.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/jsonapi_formatting.py` & `safrs-3.0.4/safrs/jsonapi_formatting.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/request.py` & `safrs-3.0.4/safrs/request.py`

 * *Files 16% similar despite different names*

```diff
@@ -78,24 +78,45 @@
         page_offset = self.args.get("page[offset]", 0, type=int)
         if page_offset == 0 and "page[number]" in self.args and "page[size]" in self.args:
             page_size = self.args.get("page[size]", type=int)
             page_number = self.args.get("page[number]", type=int) - 1
             page_offset = page_number * page_size
         return page_offset
 
+    def get_page_offset(self, rel_name):
+        """
+            get the page offset for the included relationship resource 
+            :param rel_name: name of the relationship
+            :return: page offset for included resources
+        """
+        page_offset = self.args.get(f"page[{rel_name}][offset]", 0, type=int)
+        if page_offset == 0 and "page[{rel_name}][number]" in self.args and "page[{rel_name}][size]" in self.args:
+            page_size = self.args.get("page[{rel_name}][size]", type=int)
+            page_number = self.args.get("page[{rel_name}][number]", type=int) - 1
+            page_offset = page_number * page_size
+        return page_offset
+
     @property
     def page_limit(self):
         """
-        :return: page limit requested by the client when fetching lists
+            get the page limit for the included relationship resource 
+            :param rel_name: name of the relationship
+            :return: page limit for included resources
         """
         page_limit = self.args.get("page[limit]", get_config("DEFAULT_PAGE_LIMIT"), type=int)
         if "page[number]" in self.args and "page[size]" in self.args:
             return self.args.get("page[size]", type=int)
         return page_limit
 
+    def get_page_limit(self, rel_name):
+        page_limit = self.args.get(f"page[{rel_name}][limit]", self.page_limit, type=int)
+        if "page[{rel_name}][number]" in self.args and "page[{rel_name}][size]" in self.args:
+            return self.args.get("page[{rel_name}][size]", type=int)
+        return page_limit
+
     @property
     def is_bulk(self):
         """
         jsonapi bulk extension, http://springbot.github.io/json-api/extensions/bulk/
         """
         return "bulk" in self._extensions
```

### Comparing `safrs-3.0.3/safrs/safrs_api.py` & `safrs-3.0.4/safrs/safrs_api.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/safrs_init.py` & `safrs-3.0.4/safrs/safrs_init.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/safrs_types.py` & `safrs-3.0.4/safrs/safrs_types.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/swagger_doc.py` & `safrs-3.0.4/safrs/swagger_doc.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs/util.py` & `safrs-3.0.4/safrs/util.py`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs.egg-info/PKG-INFO` & `safrs-3.0.4/safrs.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.0.3
+Version: 3.0.4
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.3.tar.gz
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.0.4.tar.gz
 Description: SAFRS: Python OpenAPI & JSON:API Framework
         ==========================================
         
         Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
         
         Overview
         --------
```

### Comparing `safrs-3.0.3/safrs.egg-info/SOURCES.txt` & `safrs-3.0.4/safrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safrs-3.0.3/safrs.egg-info/requires.txt` & `safrs-3.0.4/safrs.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Flask-Cors>=3.0.10
 Flask-RESTful>=0.3.9
 Flask-SQLAlchemy>=3.0.3
-Flask>=2.2.2
+Flask==2.2.5
 Jinja2>=3.1.2
 MarkupSafe>=2.1.2
 PyYAML>=6.0
 SQLAlchemy>=2.0.3
 Werkzeug>=2.2.2
 aniso8601>=9.0.1
 build>=0.10.0
```

### Comparing `safrs-3.0.3/setup.py` & `safrs-3.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 
 def safrs_setup():
     with open("requirements.txt", "rt") as fp:
         install_requires = fp.read().strip().split("\n")
 
-    version = "3.0.3"
+    version = "3.0.4"
 
     setup(
         name="safrs",
         packages=find_packages(exclude=['test']),
         version=version,
         license="MIT",
         description="safrs : SqlAlchemy Flask-Restful Swagger2",
```

