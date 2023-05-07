# Comparing `tmp/maya_rig_core-0.2.2.tar.gz` & `tmp/maya_rig_core-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\maya_rig_core-0.2.2.tar", last modified: Sun Oct  2 16:15:28 2022, max compression
+gzip compressed data, was "dist\maya_rig_core-0.2.3.tar", last modified: Sun May  7 12:09:29 2023, max compression
```

## Comparing `maya_rig_core-0.2.2.tar` & `maya_rig_core-0.2.3.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-10-02 16:15:27.000000 maya_rig_core-0.2.2/
--rw-rw-rw-   0        0        0    11558 2022-09-27 19:48:00.000000 maya_rig_core-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     6033 2022-10-02 16:15:30.000000 maya_rig_core-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     4754 2022-09-28 16:54:34.000000 maya_rig_core-0.2.2/README.md
--rw-rw-rw-   0        0        0      112 2022-10-02 16:15:30.000000 maya_rig_core-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1911 2022-10-02 16:13:08.000000 maya_rig_core-0.2.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/
-drwxrwxrwx   0        0        0        0 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/
--rw-rw-rw-   0        0        0     6033 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      450 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/maya_rig_core.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-10-02 16:15:28.000000 maya_rig_core-0.2.2/src/rig_core/
--rw-rw-rw-   0        0        0      294 2022-03-21 21:57:28.000000 maya_rig_core-0.2.2/src/rig_core/__init__.py
--rw-rw-rw-   0        0        0      538 2022-06-25 21:30:36.000000 maya_rig_core-0.2.2/src/rig_core/all.py
--rw-rw-rw-   0        0        0     3613 2022-10-02 15:28:22.000000 maya_rig_core-0.2.2/src/rig_core/contextmanager.py
--rw-rw-rw-   0        0        0    13147 2022-10-02 15:45:58.000000 maya_rig_core-0.2.2/src/rig_core/ctx.py
--rw-rw-rw-   0        0        0     5911 2022-08-24 00:21:54.000000 maya_rig_core-0.2.2/src/rig_core/db.py
--rw-rw-rw-   0        0        0     1465 2022-10-02 15:27:38.000000 maya_rig_core-0.2.2/src/rig_core/filter.py
--rw-rw-rw-   0        0        0     4707 2022-10-02 15:27:38.000000 maya_rig_core-0.2.2/src/rig_core/joint_tree.py
--rw-rw-rw-   0        0        0     1098 2022-10-02 15:27:38.000000 maya_rig_core-0.2.2/src/rig_core/response.py
--rw-rw-rw-   0        0        0     1720 2022-10-02 15:28:42.000000 maya_rig_core-0.2.2/src/rig_core/tag.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/
+-rw-rw-rw-   0        0        0    11558 2022-09-27 19:48:00.000000 maya_rig_core-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     6010 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4754 2022-09-28 16:54:34.000000 maya_rig_core-0.2.3/README.md
+-rw-rw-rw-   0        0        0     5257 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/README.rst
+-rw-rw-rw-   0        0        0      112 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1907 2023-05-07 11:56:56.000000 maya_rig_core-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/
+-rw-rw-rw-   0        0        0     6010 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 12:09:30.000000 maya_rig_core-0.2.3/src/maya_rig_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 12:09:28.000000 maya_rig_core-0.2.3/src/rig_core/
+-rw-rw-rw-   0        0        0      294 2022-03-21 21:57:28.000000 maya_rig_core-0.2.3/src/rig_core/__init__.py
+-rw-rw-rw-   0        0        0      538 2022-06-25 21:30:36.000000 maya_rig_core-0.2.3/src/rig_core/all.py
+-rw-rw-rw-   0        0        0     3613 2022-10-02 15:28:22.000000 maya_rig_core-0.2.3/src/rig_core/contextmanager.py
+-rw-rw-rw-   0        0        0    13599 2022-11-27 14:56:44.000000 maya_rig_core-0.2.3/src/rig_core/ctx.py
+-rw-rw-rw-   0        0        0     5911 2022-08-24 00:21:54.000000 maya_rig_core-0.2.3/src/rig_core/db.py
+-rw-rw-rw-   0        0        0     1465 2022-10-02 15:27:38.000000 maya_rig_core-0.2.3/src/rig_core/filter.py
+-rw-rw-rw-   0        0        0     4848 2022-10-02 16:28:52.000000 maya_rig_core-0.2.3/src/rig_core/joint_tree.py
+-rw-rw-rw-   0        0        0     1098 2022-10-02 15:27:38.000000 maya_rig_core-0.2.3/src/rig_core/response.py
+-rw-rw-rw-   0        0        0     1811 2022-11-27 14:56:44.000000 maya_rig_core-0.2.3/src/rig_core/tag.py
```

### Comparing `maya_rig_core-0.2.2/LICENSE` & `maya_rig_core-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/PKG-INFO` & `maya_rig_core-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: maya_rig_core
-Version: 0.2.2
+Version: 0.2.3
 Summary: 一个好用的绑定核心库
 Home-page: https://github.com/cpcgskill/maya_rig_core
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya_rig_core/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -204,9 +203,7 @@
 ## 版权说明
 
 该项目签署了Apache-2.0 授权许可，详情请参阅 LICENSE
 
 
 
 
-
-
```

### Comparing `maya_rig_core-0.2.2/README.md` & `maya_rig_core-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/setup.py` & `maya_rig_core-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,30 @@
 import setuptools
 
 lib_name = 'maya_rig_core'
 
 author = 'cpcgskill',
 author_email = 'cpcgskill@outlook.com'
 
-version = '0.2.2'
+version = '0.2.3'
 
 description = '一个好用的绑定核心库'
 with open("README.md", "rb") as f:
     long_description = f.read().decode(encoding='utf-8')
 
 project_homepage = 'https://github.com/cpcgskill/maya_rig_core'
 project_urls = {
     'Bug Tracker': 'https://github.com/cpcgskill/maya_rig_core/issues',
 }
 license = 'Apache Software License (Apache 2.0)'
 
 python_requires = '>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*'
 install_requires = [
     'maya-test-tools==0.1.0',
-    'cpmel==3.4.1',
+    'cpmel==3',
 ]
 
 setuptools.setup(
     name=lib_name,
     version=version,
     author=author,
     author_email=author_email,
```

### Comparing `maya_rig_core-0.2.2/src/maya_rig_core.egg-info/PKG-INFO` & `maya_rig_core-0.2.3/src/maya_rig_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: maya-rig-core
-Version: 0.2.2
+Version: 0.2.3
 Summary: 一个好用的绑定核心库
 Home-page: https://github.com/cpcgskill/maya_rig_core
 Author: ('cpcgskill',)
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/maya_rig_core/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -204,9 +203,7 @@
 ## 版权说明
 
 该项目签署了Apache-2.0 授权许可，详情请参阅 LICENSE
 
 
 
 
-
-
```

### Comparing `maya_rig_core-0.2.2/src/rig_core/all.py` & `maya_rig_core-0.2.3/src/rig_core/all.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/src/rig_core/contextmanager.py` & `maya_rig_core-0.2.3/src/rig_core/contextmanager.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/src/rig_core/ctx.py` & `maya_rig_core-0.2.3/src/rig_core/ctx.py`

 * *Files 2% similar despite different names*

```diff
@@ -162,41 +162,44 @@
         """
         node = cc.new_object(node)
         if cc.objExists('{}.{}'.format(node.name(), name)):
             return node.attr(name)
         else:
             return cls.add_attribute(node, name, default, min, max, typ, key)
 
-    def locator(self, n=None):
+    def locator(self, n=None, tags=[]):
         """
 
         :type n: AnyStr
+        :type tags: List[AnyStr]
         :rtype: cc.Transform
         """
         if n is None:
             n = 'space_locator'
         if 'invisible_locator' in self.feature:
             loc = self.create_node('transform')
         else:
             loc = cc.spaceLocator()[0]
+        self.add_tags(loc, *tags)
         loc.rename(n)
         if self.root_object is not None:
             loc.parent = self.root_object
         return loc
 
-    def locator_list(self, count=None, n=None):
+    def locator_list(self, count=None, n=None, tags=[]):
         """
 
         :type count: int
         :type n: AnyStr
+        :type tags: List[AnyStr]
         :rtype: List[cc.Transform]
         """
         if n is None:
             n = 'space_locator'
-        return [self.locator(n="{}{}".format(n, i)) for i in range(count)]
+        return [self.locator(n="{}{}".format(n, i), tags=tags) for i in range(count)]
 
     def controller(self, tags=[], point=None):
         """
         :type tags: List[AnyStr]
         :param point: 控制器的位置
         :rtype: cc.Transform
         """
@@ -290,14 +293,21 @@
     def enter_new_tag_rt(self, tag_attr):
         """进入新的tag_rt， 新的与旧的互相隔离"""
         old_rt = self.tag_rt
         self.tag_rt = tag.TagRt('_'.join([tag_attr, old_rt.tag_attr]))
         yield
         self.tag_rt = old_rt
 
+    @contextlib.contextmanager
+    def add_base_tags_as_new_tag_rt(self, base_tags):
+        old_rt = self.tag_rt
+        self.tag_rt = tag.TagRt(tag_attr=old_rt.tag_attr, base_tags=old_rt.base_tags + list(base_tags))
+        yield
+        self.tag_rt = old_rt
+
     @property
     def all_node_db_rt(self):
         return self._all_node_db_rt
 
     @all_node_db_rt.setter
     def all_node_db_rt(self, rt):
         if isinstance(rt, db.AllNodeDbRt):
@@ -415,11 +425,13 @@
         :return: 一个 yield 生成出来的节点的列表的上下文管理器。
             ps: 这个生成出来的节点的列表要在上下文管理器退出时才会被填充
         """
         with rig_contextmanager.enter_build_block(key) as wing_build_complete_of_nodes:
             yield wing_build_complete_of_nodes
 
     def create_quick_select_set(self, objs, name='quick_select_set'):
-        return cc.sets(*objs, n=name)
+        node = cc.sets(*objs, n=name)
+        self.add_nodes(node)
+        return node
 
 
 __all__ = ['Ctx']
```

### Comparing `maya_rig_core-0.2.2/src/rig_core/db.py` & `maya_rig_core-0.2.3/src/rig_core/db.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/src/rig_core/filter.py` & `maya_rig_core-0.2.3/src/rig_core/filter.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/src/rig_core/joint_tree.py` & `maya_rig_core-0.2.3/src/rig_core/joint_tree.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,21 +31,29 @@
         self.obj = obj
         self.point = point
         self.name = name
 
         # 如果create_only属性为真将会仅创建，而不参与蒙皮
         self.create_only = create_only
 
-        self.parent = None
-        self.childs = list()
+        self._parent = None
+        self._childs = list()
+
+    @property
+    def parent(self):
+        return self._parent
+
+    @property
+    def childs(self):
+        return self._childs
 
     def add_childs(self, *jins):
         for jin in jins:
             self.childs.append(jin)
-            jin.parent = self
+            jin._parent = self
         return self
 
     def add_child_from_object(self, obj):
         return self.add_childs(Joint(obj=obj))
 
     def add_child_from_object_list(self, objs):
         for i in objs:
```

### Comparing `maya_rig_core-0.2.2/src/rig_core/response.py` & `maya_rig_core-0.2.3/src/rig_core/response.py`

 * *Files identical despite different names*

### Comparing `maya_rig_core-0.2.2/src/rig_core/tag.py` & `maya_rig_core-0.2.3/src/rig_core/tag.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,35 +21,36 @@
     try:
         return node.attr(attr)
     except CPMelException:
         return None
 
 
 class TagRt(object):
-    def __init__(self, tag_attr="tag_runtime"):
+    def __init__(self, tag_attr="tag_runtime", base_tags=[]):
         self.tag_attr = tag_attr
+        self.base_tags = list(base_tags)
         self.cache = dict()
 
     def get_tags(self, obj):
         cache = self.cache.get(hash(obj))
         if cache is not None:
             return cache
         attr = attribute_exists(obj, self.tag_attr)
         if attr:
             tags = json.loads(cc.getAttr(attr))
         else:
-            tags = []
+            tags = self.base_tags
         return tags
 
     def set_tags(self, obj, tags):
         attr = attribute_exists(obj, self.tag_attr)
         if attr is None:
             cc.addAttr(obj, ln=self.tag_attr, dt="string")
         attr = attribute_exists(obj, self.tag_attr)
-        tags = list(set(tags))
+        tags = list(set(list(tags) + self.base_tags))
         cc.setAttr(attr, json.dumps(tags), type="string")
         self.cache[hash(obj)] = tags
         return self
 
     def add_tags(self, obj, *new_tags):
         tags = self.get_tags(obj)
         for i in new_tags:
```

