# Comparing `tmp/canonical-0.8.0.tar.gz` & `tmp/canonical-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonical-0.8.0.tar", last modified: Sat Feb  4 19:34:52 2023, max compression
+gzip compressed data, was "canonical-0.9.0.tar", last modified: Sat Feb  4 20:54:11 2023, max compression
```

## Comparing `canonical-0.8.0.tar` & `canonical-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.297018 canonical-0.8.0/
--rw-r--r--   0 cochise    (501) staff       (20)      319 2022-05-23 09:14:59.000000 canonical-0.8.0/MANIFEST.in
--rw-r--r--   0 cochise    (501) staff       (20)     1079 2023-02-04 19:34:52.296868 canonical-0.8.0/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      228 2022-05-23 09:22:06.000000 canonical-0.8.0/README.md
--rw-r--r--   0 cochise    (501) staff       (20)        6 2023-02-04 19:34:46.000000 canonical-0.8.0/VERSION
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.294729 canonical-0.8.0/canonical/
--rw-r--r--   0 cochise    (501) staff       (20)      655 2023-01-30 16:47:57.000000 canonical-0.8.0/canonical/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)     1195 2023-01-24 12:07:19.000000 canonical-0.8.0/canonical/emailaddress.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.296201 canonical-0.8.0/canonical/exc/
--rw-r--r--   0 cochise    (501) staff       (20)      539 2023-01-30 18:09:56.000000 canonical-0.8.0/canonical/exc/__init__.py
--rw-r--r--   0 cochise    (501) staff       (20)      719 2023-01-24 12:00:48.000000 canonical-0.8.0/canonical/exc/ratelimited.py
--rw-r--r--   0 cochise    (501) staff       (20)      617 2023-01-30 18:09:41.000000 canonical-0.8.0/canonical/exc/staleresource.py
--rw-r--r--   0 cochise    (501) staff       (20)      673 2023-01-24 12:38:44.000000 canonical-0.8.0/canonical/fields.py
--rw-r--r--   0 cochise    (501) staff       (20)     2320 2023-01-30 19:43:09.000000 canonical-0.8.0/canonical/genericpostaladdress.py
--rw-r--r--   0 cochise    (501) staff       (20)     2228 2022-12-26 15:57:29.000000 canonical-0.8.0/canonical/list_.py
--rw-r--r--   0 cochise    (501) staff       (20)     1195 2022-12-26 15:47:30.000000 canonical-0.8.0/canonical/listmeta.py
--rw-r--r--   0 cochise    (501) staff       (20)     5855 2023-01-30 19:41:57.000000 canonical-0.8.0/canonical/objectmeta.py
--rw-r--r--   0 cochise    (501) staff       (20)      873 2023-01-24 12:02:33.000000 canonical-0.8.0/canonical/package.json
--rw-r--r--   0 cochise    (501) staff       (20)     1608 2023-01-24 12:44:27.000000 canonical-0.8.0/canonical/phonenumber.py
--rw-r--r--   0 cochise    (501) staff       (20)     4190 2023-02-04 19:07:27.000000 canonical-0.8.0/canonical/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)     2621 2023-01-30 19:11:37.000000 canonical-0.8.0/canonical/resourcemetaclass.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.295536 canonical-0.8.0/canonical.egg-info/
--rw-r--r--   0 cochise    (501) staff       (20)     1079 2023-02-04 19:34:52.000000 canonical-0.8.0/canonical.egg-info/PKG-INFO
--rw-r--r--   0 cochise    (501) staff       (20)      602 2023-02-04 19:34:52.000000 canonical-0.8.0/canonical.egg-info/SOURCES.txt
--rw-r--r--   0 cochise    (501) staff       (20)        1 2023-02-04 19:34:52.000000 canonical-0.8.0/canonical.egg-info/dependency_links.txt
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-02-04 19:34:52.000000 canonical-0.8.0/canonical.egg-info/requires.txt
--rw-r--r--   0 cochise    (501) staff       (20)       42 2023-02-04 19:34:52.000000 canonical-0.8.0/canonical.egg-info/top_level.txt
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.296479 canonical-0.8.0/examples/
--rw-r--r--   0 cochise    (501) staff       (20)     4778 2023-02-04 18:55:56.000000 canonical-0.8.0/examples/resource.py
--rw-r--r--   0 cochise    (501) staff       (20)       38 2023-02-04 19:34:52.297058 canonical-0.8.0/setup.cfg
--rw-r--r--   0 cochise    (501) staff       (20)     1304 2022-05-23 09:14:59.000000 canonical-0.8.0/setup.py
-drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 19:34:52.296579 canonical-0.8.0/tests/
--rw-r--r--   0 cochise    (501) staff       (20)      725 2023-01-24 12:12:27.000000 canonical-0.8.0/tests/test_unit_email.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.741546 canonical-0.9.0/
+-rw-r--r--   0 cochise    (501) staff       (20)      319 2022-05-23 09:14:59.000000 canonical-0.9.0/MANIFEST.in
+-rw-r--r--   0 cochise    (501) staff       (20)     1079 2023-02-04 20:54:11.741407 canonical-0.9.0/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)      228 2022-05-23 09:22:06.000000 canonical-0.9.0/README.md
+-rw-r--r--   0 cochise    (501) staff       (20)        6 2023-02-04 20:09:50.000000 canonical-0.9.0/VERSION
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.739343 canonical-0.9.0/canonical/
+-rw-r--r--   0 cochise    (501) staff       (20)      655 2023-01-30 16:47:57.000000 canonical-0.9.0/canonical/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1195 2023-01-24 12:07:19.000000 canonical-0.9.0/canonical/emailaddress.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.740573 canonical-0.9.0/canonical/exc/
+-rw-r--r--   0 cochise    (501) staff       (20)      539 2023-01-30 18:09:56.000000 canonical-0.9.0/canonical/exc/__init__.py
+-rw-r--r--   0 cochise    (501) staff       (20)      719 2023-01-24 12:00:48.000000 canonical-0.9.0/canonical/exc/ratelimited.py
+-rw-r--r--   0 cochise    (501) staff       (20)      617 2023-01-30 18:09:41.000000 canonical-0.9.0/canonical/exc/staleresource.py
+-rw-r--r--   0 cochise    (501) staff       (20)      673 2023-01-24 12:38:44.000000 canonical-0.9.0/canonical/fields.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2320 2023-01-30 19:43:09.000000 canonical-0.9.0/canonical/genericpostaladdress.py
+-rw-r--r--   0 cochise    (501) staff       (20)     2228 2022-12-26 15:57:29.000000 canonical-0.9.0/canonical/list_.py
+-rw-r--r--   0 cochise    (501) staff       (20)     1195 2022-12-26 15:47:30.000000 canonical-0.9.0/canonical/listmeta.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5882 2023-02-04 20:11:04.000000 canonical-0.9.0/canonical/objectmeta.py
+-rw-r--r--   0 cochise    (501) staff       (20)      873 2023-01-24 12:02:33.000000 canonical-0.9.0/canonical/package.json
+-rw-r--r--   0 cochise    (501) staff       (20)     1608 2023-01-24 12:44:27.000000 canonical-0.9.0/canonical/phonenumber.py
+-rw-r--r--   0 cochise    (501) staff       (20)     4190 2023-02-04 20:53:56.000000 canonical-0.9.0/canonical/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)     5211 2023-02-04 20:53:58.000000 canonical-0.9.0/canonical/resourcemetaclass.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.739897 canonical-0.9.0/canonical.egg-info/
+-rw-r--r--   0 cochise    (501) staff       (20)     1079 2023-02-04 20:54:11.000000 canonical-0.9.0/canonical.egg-info/PKG-INFO
+-rw-r--r--   0 cochise    (501) staff       (20)      602 2023-02-04 20:54:11.000000 canonical-0.9.0/canonical.egg-info/SOURCES.txt
+-rw-r--r--   0 cochise    (501) staff       (20)        1 2023-02-04 20:54:11.000000 canonical-0.9.0/canonical.egg-info/dependency_links.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-02-04 20:54:11.000000 canonical-0.9.0/canonical.egg-info/requires.txt
+-rw-r--r--   0 cochise    (501) staff       (20)       42 2023-02-04 20:54:11.000000 canonical-0.9.0/canonical.egg-info/top_level.txt
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.740871 canonical-0.9.0/examples/
+-rw-r--r--   0 cochise    (501) staff       (20)     4778 2023-02-04 18:55:56.000000 canonical-0.9.0/examples/resource.py
+-rw-r--r--   0 cochise    (501) staff       (20)       38 2023-02-04 20:54:11.741583 canonical-0.9.0/setup.cfg
+-rw-r--r--   0 cochise    (501) staff       (20)     1304 2022-05-23 09:14:59.000000 canonical-0.9.0/setup.py
+drwxr-xr-x   0 cochise    (501) staff       (20)        0 2023-02-04 20:54:11.741162 canonical-0.9.0/tests/
+-rw-r--r--   0 cochise    (501) staff       (20)      725 2023-01-24 12:12:27.000000 canonical-0.9.0/tests/test_unit_email.py
```

### Comparing `canonical-0.8.0/PKG-INFO` & `canonical-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonical
-Version: 0.8.0
+Version: 0.9.0
 Summary: Common models and types for business applications
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `canonical-0.8.0/canonical/__init__.py` & `canonical-0.9.0/canonical/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/emailaddress.py` & `canonical-0.9.0/canonical/emailaddress.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/exc/__init__.py` & `canonical-0.9.0/canonical/exc/__init__.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/exc/ratelimited.py` & `canonical-0.9.0/canonical/exc/ratelimited.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/exc/staleresource.py` & `canonical-0.9.0/canonical/exc/staleresource.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/fields.py` & `canonical-0.9.0/canonical/fields.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/genericpostaladdress.py` & `canonical-0.9.0/canonical/genericpostaladdress.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/list_.py` & `canonical-0.9.0/canonical/list_.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/listmeta.py` & `canonical-0.9.0/canonical/listmeta.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/objectmeta.py` & `canonical-0.9.0/canonical/objectmeta.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 import datetime
 from typing import Any
 
 import pydantic
 
 
-class ObjectMeta(pydantic.BaseModel):
+class BaseMeta(pydantic.BaseModel):
     name: str | None = pydantic.Field(
         default=None,
         title="Name",
         description=(
             "Name must be unique within a namespace. Is required when creating "
             "resources, although some resources may allow a client to request "
             "the generation of an appropriate name automatically. Name is "
@@ -24,14 +24,50 @@
             "definition. Cannot be updated.\n\n"
             "If the resource is not identified by symbolic names, but an "
             "auto-generated identifier instead, this field contains the "
             "same value as the `uid` field."
         )
     )
 
+    namespace: str | None = pydantic.Field(
+        default=None,
+        title="Namespace",
+        description=(
+            "Namespace defines the space within which each name must be "
+            "unique. An empty namespace is equivalent to the `default` "
+            "namespace, but `default` is the canonical representation. "
+            "Not all objects are required to be scoped to a namespace "
+            "- the value of this field for those objects will be empty."
+            "Not all servers may implement the concept of namespaces."
+        )
+    )
+
+    labels: dict[str, str] = pydantic.Field(
+        default={},
+        title='Labels',
+        description=(
+            "Map of string keys and values that can be used to "
+            "organize and categorize (scope and select) objects."
+        )
+    )
+
+    annotations: dict[str, Any] = pydantic.Field(
+        default={},
+        title='Annotations',
+        description=(
+            "Annotations is an unstructured key value map stored "
+            "with a resource that may be set by external tools "
+            "to store and retrieve arbitrary metadata. They are "
+            "not queryable and should be preserved when modifying"
+            "objects."
+        )
+    )
+
+
+class ObjectMeta(BaseMeta):
     generation: int = pydantic.Field(
         default=0,
         title='Generation',
         description=(
             "A sequence number representing a specific generation "
             "of the desired state. Populated by the system. Read-only."
         )
@@ -51,27 +87,14 @@
             "length of the suffix required to make the value unique on the server."
             "\n\n"
             "If this field is specified and the generated name exists, the "
             "server will return a 409."
         )
     )
 
-    namespace: str | None = pydantic.Field(
-        default=None,
-        title="Namespace",
-        description=(
-            "Namespace defines the space within which each name must be "
-            "unique. An empty namespace is equivalent to the `default` "
-            "namespace, but `default` is the canonical representation. "
-            "Not all objects are required to be scoped to a namespace "
-            "- the value of this field for those objects will be empty."
-            "Not all servers may implement the concept of namespaces."
-        )
-    )
-
     creation_timestamp: datetime.datetime | None = pydantic.Field(
         default=None,
         title="Created",
         alias='creationTimestamp',
         description=(
             "The `creationTimestamp` field is a timestamp representing "
             "the server time when this object was created. It is not "
@@ -108,35 +131,14 @@
             "a resource and is not allowed to change on PUT operations.\n\n"
             "Depending on the implementation, the `uid` field may be either "
             "an integer or a string, but clients should treat this value "
             "as opaque."
         )
     )
 
-    labels: dict[str, str] = pydantic.Field(
-        default={},
-        title='Labels',
-        description=(
-            "Map of string keys and values that can be used to "
-            "organize and categorize (scope and select) objects."
-        )
-    )
-
-    annotations: dict[str, Any] = pydantic.Field(
-        default={},
-        title='Annotations',
-        description=(
-            "Annotations is an unstructured key value map stored "
-            "with a resource that may be set by external tools "
-            "to store and retrieve arbitrary metadata. They are "
-            "not queryable and should be preserved when modifying"
-            "objects."
-        )
-    )
-
     links: dict[str, pydantic.AnyUrl] = pydantic.Field(
         default={},
         title='Links',
         description=(
             "A mapping of operations to links that may be used by clients "
             "to traverse the REStful API and discover additional "
             "methods on resources."
```

### Comparing `canonical-0.8.0/canonical/package.json` & `canonical-0.9.0/canonical/package.json`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/phonenumber.py` & `canonical-0.9.0/canonical/phonenumber.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical/resource.py` & `canonical-0.9.0/canonical/resource.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/canonical.egg-info/PKG-INFO` & `canonical-0.9.0/canonical.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonical
-Version: 0.8.0
+Version: 0.9.0
 Summary: Common models and types for business applications
 Home-page: https://gitlab.com/unimatrixone
 Author: Cochise Ruhulessin
 Author-email: cochise.ruhulessin@unimatrixone.io
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
```

### Comparing `canonical-0.8.0/canonical.egg-info/SOURCES.txt` & `canonical-0.9.0/canonical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/examples/resource.py` & `canonical-0.9.0/examples/resource.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/setup.py` & `canonical-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `canonical-0.8.0/tests/test_unit_email.py` & `canonical-0.9.0/tests/test_unit_email.py`

 * *Files identical despite different names*

