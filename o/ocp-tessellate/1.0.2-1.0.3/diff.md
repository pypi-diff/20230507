# Comparing `tmp/ocp_tessellate-1.0.2.tar.gz` & `tmp/ocp_tessellate-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocp_tessellate-1.0.2.tar", last modified: Thu Apr 27 18:57:05 2023, max compression
+gzip compressed data, was "ocp_tessellate-1.0.3.tar", last modified: Sun May  7 14:11:03 2023, max compression
```

## Comparing `ocp_tessellate-1.0.2.tar` & `ocp_tessellate-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.745693 ocp_tessellate-1.0.2/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-27 18:57:05.745747 ocp_tessellate-1.0.2/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.2/README.md
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.744843 ocp_tessellate-1.0.2/ocp_tessellate/
--rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.2/ocp_tessellate/__init__.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-04-27 18:56:38.000000 ocp_tessellate-1.0.2/ocp_tessellate/_version.py
--rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.2/ocp_tessellate/cad_objects.py
--rw-r--r--   0 bernhard   (501) staff       (20)    27010 2023-04-27 18:53:29.000000 ocp_tessellate-1.0.2/ocp_tessellate/convert.py
--rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-27 18:53:44.000000 ocp_tessellate-1.0.2/ocp_tessellate/defaults.py
--rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.2/ocp_tessellate/mp_tess.py
--rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.2/ocp_tessellate/mp_tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.2/ocp_tessellate/ocp_utils.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.2/ocp_tessellate/stepreader.py
--rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.2/ocp_tessellate/tessellator.py
--rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-27 16:19:21.000000 ocp_tessellate-1.0.2/ocp_tessellate/utils.py
-drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-04-27 18:57:05.745597 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/
--rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/PKG-INFO
--rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/SOURCES.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/dependency_links.txt
--rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-04-23 16:08:07.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/not-zip-safe
--rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/requires.txt
--rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-04-27 18:57:05.000000 ocp_tessellate-1.0.2/ocp_tessellate.egg-info/top_level.txt
--rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-04-27 18:57:05.745992 ocp_tessellate-1.0.2/setup.cfg
--rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-04-27 18:56:38.000000 ocp_tessellate-1.0.2/setup.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.857151 ocp_tessellate-1.0.3/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-05-07 14:11:03.857212 ocp_tessellate-1.0.3/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)       17 2023-01-23 07:09:46.000000 ocp_tessellate-1.0.3/README.md
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.856296 ocp_tessellate-1.0.3/ocp_tessellate/
+-rw-r--r--   0 bernhard   (501) staff       (20)     2926 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.3/ocp_tessellate/__init__.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1123 2023-05-07 13:49:09.000000 ocp_tessellate-1.0.3/ocp_tessellate/_version.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    12980 2023-04-15 16:48:19.000000 ocp_tessellate-1.0.3/ocp_tessellate/cad_objects.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    27059 2023-05-07 13:47:27.000000 ocp_tessellate-1.0.3/ocp_tessellate/convert.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    10515 2023-04-27 18:53:44.000000 ocp_tessellate-1.0.3/ocp_tessellate/defaults.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     1301 2023-02-10 14:10:23.000000 ocp_tessellate-1.0.3/ocp_tessellate/mp_tess.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     3033 2023-03-04 18:53:03.000000 ocp_tessellate-1.0.3/ocp_tessellate/mp_tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    19710 2023-04-07 11:30:03.000000 ocp_tessellate-1.0.3/ocp_tessellate/ocp_utils.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13370 2023-04-22 09:22:57.000000 ocp_tessellate-1.0.3/ocp_tessellate/stepreader.py
+-rw-r--r--   0 bernhard   (501) staff       (20)    13224 2023-04-22 15:51:39.000000 ocp_tessellate-1.0.3/ocp_tessellate/tessellator.py
+-rw-r--r--   0 bernhard   (501) staff       (20)     6223 2023-04-27 16:19:21.000000 ocp_tessellate-1.0.3/ocp_tessellate/utils.py
+drwxr-xr-x   0 bernhard   (501) staff       (20)        0 2023-05-07 14:11:03.857064 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/
+-rw-r--r--   0 bernhard   (501) staff       (20)      774 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/PKG-INFO
+-rw-r--r--   0 bernhard   (501) staff       (20)      561 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/SOURCES.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/dependency_links.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)        1 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/not-zip-safe
+-rw-r--r--   0 bernhard   (501) staff       (20)      102 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/requires.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)       15 2023-05-07 14:11:03.000000 ocp_tessellate-1.0.3/ocp_tessellate.egg-info/top_level.txt
+-rw-r--r--   0 bernhard   (501) staff       (20)      671 2023-05-07 14:11:03.857461 ocp_tessellate-1.0.3/setup.cfg
+-rw-r--r--   0 bernhard   (501) staff       (20)     1646 2023-05-07 13:49:09.000000 ocp_tessellate-1.0.3/setup.py
```

### Comparing `ocp_tessellate-1.0.2/PKG-INFO` & `ocp_tessellate-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp_tessellate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/__init__.py` & `ocp_tessellate-1.0.3/ocp_tessellate/__init__.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/_version.py` & `ocp_tessellate-1.0.3/ocp_tessellate/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,9 +24,9 @@
     r = re.compile(
         r"(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)\-{0,1}(?P<release>\D*)(?P<build>\d*)"
     )
     major, minor, patch, release, build = r.match(version).groups()
     return VersionInfo(major, minor, patch, release, build)
 
 
-__version__ = "1.0.2"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
+__version__ = "1.0.3"  # DO NOT EDIT THIS DIRECTLY!  It is managed by bumpversion
 __version_info__ = get_version(__version__)
```

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/cad_objects.py` & `ocp_tessellate-1.0.3/ocp_tessellate/cad_objects.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/convert.py` & `ocp_tessellate-1.0.3/ocp_tessellate/convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         )
 
     elif is_vertex_list(cad_objs):
         _debug("          conv: vertex_list")
         return OCP_Vertices(
             cad_objs,
             name=get_name(obj_name, cad_objs, "Vertex", "Vertices"),
-            color=get_rgba(obj_color, 1.0, THICK_EDGE_COLOR),
+            color=get_rgba(obj_color, 1.0, VERTEX_COLOR),
             size=6,
         )
 
     else:
         raise RuntimeError(
             f"Cannot transform {cad_objs}, e.g. mixed Compounds not supported here?"
         )
@@ -695,15 +695,16 @@
 
                 if (
                     render_joints
                     and hasattr(cad_obj, "joints")
                     and len(cad_obj.joints) > 0
                 ):
                     _debug("    to_assembly: joints")
-                    pg.name = obj_name
+                    if obj_name is not None:
+                        pg.name = obj_name
                     part.name = "shape"
                     # create a new part group for mates
                     pg2 = OCP_PartGroup(
                         [
                             conv(joint.symbol.wrapped, name)
                             for name, joint in cad_obj.joints.items()
                             if hasattr(joint, "symbol")
@@ -829,15 +830,15 @@
             pg.objects[0].loc = pg.loc * pg.objects[0].loc
         pg = pg.objects[0]
 
     set_instances([instance[1] for instance in instances])
     return pg
 
 
-def export_three_cad_viewer_json(obj, filename=None):
+def export_three_cad_viewer_json(*objs, filename=None):
     def decode(instances, shapes):
         def walk(obj):
             typ = None
             for attr in obj.keys():
                 if attr == "parts":
                     for part in obj["parts"]:
                         walk(part)
@@ -849,15 +850,15 @@
                     if typ == "shapes":
                         if obj["shape"].get("ref") is not None:
                             ind = obj["shape"]["ref"]
                             obj["shape"] = instances[ind]
 
         walk(shapes)
 
-    part_group = to_assembly(obj)
+    part_group = to_assembly(*objs)
     instances, shapes, states = tessellate_group(part_group)
     decode(instances, shapes)
 
     j = numpy_to_json([shapes, states])
     if filename is None:
         return j
     else:
```

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/defaults.py` & `ocp_tessellate-1.0.3/ocp_tessellate/defaults.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/mp_tess.py` & `ocp_tessellate-1.0.3/ocp_tessellate/mp_tess.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/mp_tessellator.py` & `ocp_tessellate-1.0.3/ocp_tessellate/mp_tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/ocp_utils.py` & `ocp_tessellate-1.0.3/ocp_tessellate/ocp_utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/stepreader.py` & `ocp_tessellate-1.0.3/ocp_tessellate/stepreader.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/tessellator.py` & `ocp_tessellate-1.0.3/ocp_tessellate/tessellator.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate/utils.py` & `ocp_tessellate-1.0.3/ocp_tessellate/utils.py`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate.egg-info/PKG-INFO` & `ocp_tessellate-1.0.3/ocp_tessellate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ocp-tessellate
-Version: 1.0.2
+Version: 1.0.3
 Summary: Tessellate OCP objects
 Home-page: https://github.com/bernhard-42/ocp-tessellate
 Author: Bernhard Walter
 Author-email: b_walter@arcor.de
 Keywords: CAD,cadquery
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: IPython
```

### Comparing `ocp_tessellate-1.0.2/ocp_tessellate.egg-info/SOURCES.txt` & `ocp_tessellate-1.0.3/ocp_tessellate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ocp_tessellate-1.0.2/setup.cfg` & `ocp_tessellate-1.0.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.2
+current_version = 1.0.3
 commit = False
 tag = False
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?P<release>\D*)(?P<build>\d*)
 serialize = 
 	{major}.{minor}.{patch}{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `ocp_tessellate-1.0.2/setup.py` & `ocp_tessellate-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 LONG_DESCRIPTION = (
     "Tessellate OCP (https://github.com/cadquery/OCP) objects to use with threejs"
 )
 
 setup_args = {
     "name": "ocp_tessellate",
-    "version": "1.0.2",
+    "version": "1.0.3",
     "description": "Tessellate OCP objects",
     "long_description": LONG_DESCRIPTION,
     "include_package_data": True,
     "python_requires": ">=3.9",
     "install_requires": [
         "webcolors~=1.12",
         "numpy",
```

