# Comparing `tmp/maya-rig-operation-graph-0.5.3.tar.gz` & `tmp/maya-rig-operation-graph-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya-rig-operation-graph-0.5.3.tar", last modified: Tue May  2 12:00:01 2023, max compression
+gzip compressed data, was "dist\maya-rig-operation-graph-0.6.0.tar", last modified: Sun May  7 12:06:01 2023, max compression
```

## Comparing `maya-rig-operation-graph-0.5.3.tar` & `maya-rig-operation-graph-0.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 11:59:34.000000 maya-rig-operation-graph-0.5.3/
--rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.5.3/LICENSE
--rw-rw-rw-   0        0        0     3819 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     2622 2023-05-02 12:00:00.000000 maya-rig-operation-graph-0.5.3/README.rst
--rw-rw-rw-   0        0        0      112 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     1912 2023-05-02 11:59:06.000000 maya-rig-operation-graph-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-02 11:59:34.000000 maya-rig-operation-graph-0.5.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-02 12:00:01.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/
--rw-rw-rw-   0        0        0     3819 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-02 12:00:02.000000 maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-02 12:00:01.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/
--rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/__init__.py
--rw-rw-rw-   0        0        0     2987 2023-05-02 03:34:50.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/_utils.py
--rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/additional.py
--rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/all.py
--rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/blend.py
--rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/clamp.py
--rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/distance.py
--rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/drive.py
--rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/logic.py
--rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.py
--rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.pyi
--rw-rw-rw-   0        0        0     5541 2023-04-30 10:34:56.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.py
--rw-rw-rw-   0        0        0     1737 2023-05-02 11:47:16.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.pyi
--rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/matrix.py
--rw-rw-rw-   0        0        0     3468 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/quaternion.py
--rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/random.py
--rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/reverse.py
--rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.5.3/src/rig_operation_graph/time.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:06:00.000000 maya-rig-operation-graph-0.6.0/
+-rw-rw-rw-   0        0        0    11558 2022-10-23 14:57:04.000000 maya-rig-operation-graph-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     3819 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2622 2023-05-07 12:06:00.000000 maya-rig-operation-graph-0.6.0/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1910 2023-05-07 11:58:18.000000 maya-rig-operation-graph-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:06:00.000000 maya-rig-operation-graph-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 12:06:00.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/
+-rw-rw-rw-   0        0        0     3819 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-07 12:06:02.000000 maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 12:06:00.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/
+-rw-rw-rw-   0        0        0      297 2022-05-11 13:52:18.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/__init__.py
+-rw-rw-rw-   0        0        0     3219 2023-05-06 17:11:50.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/_utils.py
+-rw-rw-rw-   0        0        0     1423 2022-10-06 03:06:38.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/additional.py
+-rw-rw-rw-   0        0        0     1250 2023-05-02 01:39:06.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/all.py
+-rw-rw-rw-   0        0        0     1271 2022-10-06 03:11:24.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/blend.py
+-rw-rw-rw-   0        0        0     1243 2022-10-06 03:26:24.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/clamp.py
+-rw-rw-rw-   0        0        0      858 2022-08-04 14:52:14.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/distance.py
+-rw-rw-rw-   0        0        0      800 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/drive.py
+-rw-rw-rw-   0        0        0     2267 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/logic.py
+-rw-rw-rw-   0        0        0     4858 2022-09-27 19:50:48.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math.py
+-rw-rw-rw-   0        0        0     1180 2022-08-04 17:29:44.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math.pyi
+-rw-rw-rw-   0        0        0     5757 2023-05-06 17:21:16.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math3d.py
+-rw-rw-rw-   0        0        0     1737 2023-05-02 11:47:16.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math3d.pyi
+-rw-rw-rw-   0        0        0     4714 2023-05-02 03:35:42.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/matrix.py
+-rw-rw-rw-   0        0        0     3817 2023-05-06 16:50:06.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/quaternion.py
+-rw-rw-rw-   0        0        0     2034 2022-08-23 07:56:04.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/random.py
+-rw-rw-rw-   0        0        0      591 2022-06-12 18:38:00.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/reverse.py
+-rw-rw-rw-   0        0        0      566 2022-08-22 02:24:00.000000 maya-rig-operation-graph-0.6.0/src/rig_operation_graph/time.py
```

### Comparing `maya-rig-operation-graph-0.5.3/LICENSE` & `maya-rig-operation-graph-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/PKG-INFO` & `maya-rig-operation-graph-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.5.3
+Version: 0.6.0
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.5.3/README.rst` & `maya-rig-operation-graph-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/setup.py` & `maya-rig-operation-graph-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import setuptools
 
 lib_name = 'maya-rig-operation-graph'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.5.3'
+version = '0.6.0'
 
 description = 'maya计算图的实现'
 with open("README.rst", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya-rig-operation-graph'
 project_urls = {
     'Bug Tracker': 'https://github.com/cpcgskill/maya-rig-operation-graph/issues',
 }
 license = 'Apache Software License (Apache 2.0)'
 
 packages = ['rig_operation_graph']
 python_requires = '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*'
 install_requires = [
-    'maya-rig-core>=0.2',
+    'maya-rig-core==0',
 ]
 
 setuptools.setup(
     name=lib_name,
     version=version,
     author=author,
     author_email=author_email,
```

### Comparing `maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/PKG-INFO` & `maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maya-rig-operation-graph
-Version: 0.5.3
+Version: 0.6.0
 Summary: maya计算图的实现
 Home-page: https://github.com/cpcgskill/maya-rig-operation-graph
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya-rig-operation-graph/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `maya-rig-operation-graph-0.5.3/src/maya_rig_operation_graph.egg-info/SOURCES.txt` & `maya-rig-operation-graph-0.6.0/src/maya_rig_operation_graph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/_utils.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,26 +32,30 @@
     if is_attr(in_value):
         in_attr = cc.new_object(in_value)
         in_attr >> out_attr
         return
     out_attr.set_value(in_value)
 
 
-def set_or_connect_3d(in_value, out_attr):
-    if is_attr(in_value):
-        in_attr = cc.new_object(in_value)
-        in_attr >> out_attr
-        return
-
+def set_or_connect_3d(in_attr, out_attr):
     attr_plug = out_attr.api1_m_plug()
-    out_attr_list = [cc.new_object(attr_plug.child(i).name()) for i in range(attr_plug.numChildren())]
+    child_of_out_attr_list = [cc.new_object(attr_plug.child(i).name()) for i in range(attr_plug.numChildren())]
 
-    set_or_connect(in_value[0], out_attr_list[0])
-    set_or_connect(in_value[1], out_attr_list[1])
-    set_or_connect(in_value[2], out_attr_list[2])
+    if is_attr(in_attr):
+        in_attr = cc.new_object(in_attr)
+        if in_attr.type() not in {'float', 'double'}:
+            in_attr >> out_attr
+            return
+        in_attr = [in_attr, in_attr, in_attr]
+    elif isinstance(in_attr, (int, float)):
+        in_attr = [in_attr, in_attr, in_attr]
+
+    set_or_connect(in_attr[0], child_of_out_attr_list[0])
+    set_or_connect(in_attr[1], child_of_out_attr_list[1])
+    set_or_connect(in_attr[2], child_of_out_attr_list[2])
 
 
 def set_or_connect_matrix(ctx, in_value, out_attr):
     if is_attr(in_value):
         in_attr = cc.new_object(in_value)
         in_attr >> out_attr
         return
```

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/additional.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/additional.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/all.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/all.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/blend.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/blend.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/clamp.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/clamp.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/distance.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/distance.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/drive.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/drive.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/logic.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/logic.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math.pyi` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,20 @@
     from maya_test_tools import question_open_maya_gui
 
     ctx = Ctx()
 
     out_attr = vector_add(ctx, (1, 1, 1), (-1, -1, -1))
     print(out_attr, out_attr.get_value())
 
+    out_attr = vector_add(ctx, (1, 1, 1), -1)
+    print(out_attr, out_attr.get_value())
+
+    out_attr = vector_add(ctx, (1, 1, 1), cc.new_object(out_attr.name()+'x'))
+    print(out_attr, out_attr.get_value())
+
     out_attr = vector_sub(ctx, out_attr, (-1, 1, -1))
     print(out_attr, out_attr.get_value())
 
     out_attr = vector_mul(ctx, out_attr, (1.5, 1.5, 1.5))
     print(out_attr, out_attr.get_value())
 
     out_attr = vector_div(ctx, out_attr, (3, 3, 3))
```

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/math3d.pyi` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/math3d.pyi`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/matrix.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/matrix.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/quaternion.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/quaternion.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,22 +66,29 @@
 
 def quaternion_to_euler(ctx, value):
     n = ctx.create_node('quatToEuler')
     set_or_connect_quaternion(value, n.attr('inputQuat'))
     return n.attr('outputRotate')
 
 
+def quaternion_from_euler(ctx, value):
+    n = ctx.create_node('eulerToQuat')
+    set_or_connect_3d(value, n.attr('inputRotate'))
+    return n.attr('outputQuat')
+
+
 __all__ = [
     'quaternion_product',
     'quaternion_add',
     'quaternion_sub',
     'quaternion_invert',
     'quaternion_normalize',
     'quaternion_conjugate',
     'quaternion_to_euler',
+    'quaternion_from_euler',
 ]
 
 if __name__ == '__main__':
     from maya_test_tools import question_open_maya_gui
 
     ctx = Ctx()
 
@@ -109,8 +116,12 @@
     out_attr = quaternion_conjugate(ctx, (0, 0, 0, 1))
     print("quaternion_conjugate:", out_attr.get_value())
 
     # Test quaternion_to_euler
     out_attr = quaternion_to_euler(ctx, (0, 0, 0, 1))
     print("quaternion_to_euler:", out_attr.get_value())
 
+    # Test quaternion_from_euler
+    out_attr = quaternion_from_euler(ctx, (0, 0, 0))
+    print("quaternion_from_euler:", out_attr.get_value())
+
     question_open_maya_gui()
```

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/random.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/random.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/reverse.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/reverse.py`

 * *Files identical despite different names*

### Comparing `maya-rig-operation-graph-0.5.3/src/rig_operation_graph/time.py` & `maya-rig-operation-graph-0.6.0/src/rig_operation_graph/time.py`

 * *Files identical despite different names*

