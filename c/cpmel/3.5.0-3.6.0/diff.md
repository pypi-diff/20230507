# Comparing `tmp/cpmel-3.5.0.tar.gz` & `tmp/cpmel-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cpmel-3.5.0.tar", last modified: Sun Nov  6 15:49:13 2022, max compression
+gzip compressed data, was "dist\cpmel-3.6.0.tar", last modified: Sun May  7 11:53:51 2023, max compression
```

## Comparing `cpmel-3.5.0.tar` & `cpmel-3.6.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/
--rw-rw-rw-   0        0        0    11558 2022-03-14 18:28:54.000000 cpmel-3.5.0/LICENSE
--rw-rw-rw-   0        0        0     6469 2022-11-06 15:49:14.000000 cpmel-3.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5166 2022-07-26 21:29:18.000000 cpmel-3.5.0/README.md
--rw-rw-rw-   0        0        0      108 2021-12-26 04:05:16.000000 cpmel-3.5.0/pyproject.toml
--rw-rw-rw-   0        0        0      112 2022-11-06 15:49:14.000000 cpmel-3.5.0/setup.cfg
--rw-rw-rw-   0        0        0     1711 2022-05-13 14:15:40.000000 cpmel-3.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/src/
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/src/cpmel/
--rw-rw-rw-   0        0        0      398 2022-03-17 19:51:32.000000 cpmel-3.5.0/src/cpmel/__init__.py
--rw-rw-rw-   0        0        0     4743 2022-04-18 18:04:28.000000 cpmel-3.5.0/src/cpmel/_args_conv.py
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/src/cpmel/_command/
--rw-rw-rw-   0        0        0      296 2022-03-14 20:50:26.000000 cpmel-3.5.0/src/cpmel/_command/__init__.py
--rw-rw-rw-   0        0        0     3050 2022-04-24 21:25:30.000000 cpmel-3.5.0/src/cpmel/_command/build_new_func.py
--rw-rw-rw-   0        0        0     4853 2022-04-24 21:26:46.000000 cpmel-3.5.0/src/cpmel/_command/commands.py
--rw-rw-rw-   0        0        0     2281 2022-04-24 20:37:02.000000 cpmel-3.5.0/src/cpmel/_mel.py
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/src/cpmel/_object_types/
--rw-rw-rw-   0        0        0      296 2022-03-16 20:11:10.000000 cpmel-3.5.0/src/cpmel/_object_types/__init__.py
--rw-rw-rw-   0        0        0    18437 2022-11-06 15:43:38.000000 cpmel-3.5.0/src/cpmel/_object_types/core.py
--rw-rw-rw-   0        0        0     8709 2022-07-26 19:14:38.000000 cpmel-3.5.0/src/cpmel/_object_types/other.py
--rw-rw-rw-   0        0        0      605 2022-08-06 14:02:34.000000 cpmel-3.5.0/src/cpmel/cmds.py
--rw-rw-rw-   0        0        0   301102 2022-08-06 14:13:18.000000 cpmel-3.5.0/src/cpmel/cmds.pyi
--rw-rw-rw-   0        0        0      552 2022-03-17 15:34:26.000000 cpmel-3.5.0/src/cpmel/exc.py
--rw-rw-rw-   0        0        0      482 2022-08-06 13:59:20.000000 cpmel-3.5.0/src/cpmel/object_types.py
--rw-rw-rw-   0        0        0     1270 2022-11-06 15:48:58.000000 cpmel-3.5.0/src/cpmel/versions.py
-drwxrwxrwx   0        0        0        0 2022-11-06 15:49:13.000000 cpmel-3.5.0/src/cpmel.egg-info/
--rw-rw-rw-   0        0        0     6469 2022-11-06 15:49:14.000000 cpmel-3.5.0/src/cpmel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      581 2022-11-06 15:49:14.000000 cpmel-3.5.0/src/cpmel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-06 15:49:14.000000 cpmel-3.5.0/src/cpmel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2022-11-06 15:49:14.000000 cpmel-3.5.0/src/cpmel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2022-11-06 15:49:14.000000 cpmel-3.5.0/src/cpmel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/
+-rw-rw-rw-   0        0        0    11558 2022-03-14 18:28:54.000000 cpmel-3.6.0/LICENSE
+-rw-rw-rw-   0        0        0     6461 2023-05-07 11:53:52.000000 cpmel-3.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5178 2023-05-07 11:22:56.000000 cpmel-3.6.0/README.md
+-rw-rw-rw-   0        0        0     5791 2023-05-07 11:53:46.000000 cpmel-3.6.0/README.rst
+-rw-rw-rw-   0        0        0      108 2021-12-26 04:05:16.000000 cpmel-3.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0      112 2023-05-07 11:53:52.000000 cpmel-3.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1707 2023-05-07 11:44:56.000000 cpmel-3.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/src/cpmel/
+-rw-rw-rw-   0        0        0      398 2022-03-17 19:51:32.000000 cpmel-3.6.0/src/cpmel/__init__.py
+-rw-rw-rw-   0        0        0     4743 2022-04-18 18:04:28.000000 cpmel-3.6.0/src/cpmel/_args_conv.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/src/cpmel/_command/
+-rw-rw-rw-   0        0        0      296 2022-03-14 20:50:26.000000 cpmel-3.6.0/src/cpmel/_command/__init__.py
+-rw-rw-rw-   0        0        0     3050 2022-04-24 21:25:30.000000 cpmel-3.6.0/src/cpmel/_command/build_new_func.py
+-rw-rw-rw-   0        0        0     4853 2022-04-24 21:26:46.000000 cpmel-3.6.0/src/cpmel/_command/commands.py
+-rw-rw-rw-   0        0        0     2281 2022-04-24 20:37:02.000000 cpmel-3.6.0/src/cpmel/_mel.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/src/cpmel/_object_types/
+-rw-rw-rw-   0        0        0      296 2022-03-16 20:11:10.000000 cpmel-3.6.0/src/cpmel/_object_types/__init__.py
+-rw-rw-rw-   0        0        0    19274 2023-05-07 09:37:18.000000 cpmel-3.6.0/src/cpmel/_object_types/core.py
+-rw-rw-rw-   0        0        0     8709 2022-07-26 19:14:38.000000 cpmel-3.6.0/src/cpmel/_object_types/other.py
+-rw-rw-rw-   0        0        0      630 2023-05-07 06:44:36.000000 cpmel-3.6.0/src/cpmel/cmds.py
+-rw-rw-rw-   0        0        0   301127 2023-05-07 06:44:36.000000 cpmel-3.6.0/src/cpmel/cmds.pyi
+-rw-rw-rw-   0        0        0      552 2022-03-17 15:34:26.000000 cpmel-3.6.0/src/cpmel/exc.py
+-rw-rw-rw-   0        0        0      482 2022-08-06 13:59:20.000000 cpmel-3.6.0/src/cpmel/object_types.py
+-rw-rw-rw-   0        0        0     1270 2023-05-07 11:23:30.000000 cpmel-3.6.0/src/cpmel/versions.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:53:51.000000 cpmel-3.6.0/src/cpmel.egg-info/
+-rw-rw-rw-   0        0        0     6461 2023-05-07 11:53:52.000000 cpmel-3.6.0/src/cpmel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2023-05-07 11:53:52.000000 cpmel-3.6.0/src/cpmel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 11:53:52.000000 cpmel-3.6.0/src/cpmel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-07 11:53:52.000000 cpmel-3.6.0/src/cpmel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-07 11:53:52.000000 cpmel-3.6.0/src/cpmel.egg-info/top_level.txt
```

### Comparing `cpmel-3.5.0/LICENSE` & `cpmel-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/PKG-INFO` & `cpmel-3.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cpmel
-Version: 3.5.0
+Version: 3.6.0
 Summary: 一个现代的maya python库
 Home-page: https://github.com/cpcgskill/CPMel
 Author: cpcgskill
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/CPMel/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -55,15 +54,16 @@
       * [属性相关操作](#属性相关操作)
 - [版权说明](#版权说明)
 
 ## 快速开始
 
 ### 安装
 
-注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是C:\Program Files\Autodesk\Maya2018\bin\mayapy.exe
+注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是"C:\\Program
+Files\\Autodesk\\<Maya版本>\\bin\\mayapy.exe"
 
 ```commandline
 python -m pip install cpmel
 ```
 
 在windows下maya的安装例子
 
@@ -259,8 +259,7 @@
 # 断开属性连接
 node.tx.disconnect(node.ty)
 ```
 
 ## 版权说明
 
 该项目签署了Apache-2.0 授权许可，详情请参阅 LICENSE
-
```

### Comparing `cpmel-3.5.0/README.md` & `cpmel-3.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,16 @@
       * [属性相关操作](#属性相关操作)
 - [版权说明](#版权说明)
 
 ## 快速开始
 
 ### 安装
 
-注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是C:\Program Files\Autodesk\Maya2018\bin\mayapy.exe
+注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是"C:\\Program
+Files\\Autodesk\\<Maya版本>\\bin\\mayapy.exe"
 
 ```commandline
 python -m pip install cpmel
 ```
 
 在windows下maya的安装例子
```

### Comparing `cpmel-3.5.0/setup.py` & `cpmel-3.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     package_dir={'': 'src'},
     # 使用自动搜索
     packages=setuptools.find_packages(where='src'),
     package_data={'cpmel': ['*.pyi']},
     python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*",
     # 指定依赖
     install_requires=[
-        'cpapi==1.0.2',
-        'cpref==1.1.0',
+        'cpapi==1.0',
+        'cpref==1.1',
     ],
 )
```

### Comparing `cpmel-3.5.0/src/cpmel/_args_conv.py` & `cpmel-3.6.0/src/cpmel/_args_conv.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/_command/build_new_func.py` & `cpmel-3.6.0/src/cpmel/_command/build_new_func.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/_command/commands.py` & `cpmel-3.6.0/src/cpmel/_command/commands.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/_mel.py` & `cpmel-3.6.0/src/cpmel/_mel.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/_object_types/core.py` & `cpmel-3.6.0/src/cpmel/_object_types/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -404,14 +404,36 @@
 
     def __rshift__(self, other):
         a = arg_conv(self)
         b = arg_conv(other)
         mc.connectAttr(a, b, f=True)
         return new_object(b)
 
+    def __iter__(self):
+        attr_plug = self.api1_m_plug()
+        if attr_plug.isCompound():
+            return (new_object(attr_plug.child(i).name()) for i in range(attr_plug.numChildren()))
+        elif attr_plug.isArray():
+            return (new_object(attr_plug.child(i).name()) for i in range(attr_plug.numElements()))
+        raise CPMelException('This plugin cannot create iterable objects')
+
+    @property
+    def childs(self):
+        attr_plug = self.api1_m_plug()
+        if not attr_plug.isCompound():
+            raise CPMelException('This plug is not a compound')
+        return list(self)
+
+    @property
+    def elements(self):
+        attr_plug = self.api1_m_plug()
+        if not attr_plug.isArray():
+            raise CPMelException('This plug is not a compound')
+        return list(self)
+
     def attr(self, name):
         return new_object("{}.{}".format(self.name(), name))
 
     def __getattr__(self, item):
         try:
             return self.attr(item)
         except CPMelException:
```

### Comparing `cpmel-3.5.0/src/cpmel/_object_types/other.py` & `cpmel-3.6.0/src/cpmel/_object_types/other.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/cmds.py` & `cpmel-3.6.0/src/cpmel/cmds.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 :bilibili: https://space.bilibili.com/351598127
 
 """
 from __future__ import unicode_literals, print_function
 
 from cpmel._command.build_new_func import new_func_list_from_module as _new_func_list_from_module
 import cpmel._mel as _mel
+from cpmel.exc import *
 
 _new_func_list_from_module(globals())
 
 mel = _mel.Mel()
 
 from cpmel.object_types import *
 from maya.mel import eval
```

### Comparing `cpmel-3.5.0/src/cpmel/cmds.pyi` & `cpmel-3.6.0/src/cpmel/cmds.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/python
 # -*-coding:utf-8 -*-
 from __future__ import unicode_literals, print_function, division
 from cpmel.object_types import *
 import cpmel._mel as _mel
+from cpmel.exc import *
 
 from typing import Union, AnyStr, Any, List
 
 mel = _mel.Mel()
 
 __CommandReturn = Union[list, tuple,
                       AnyStr,
```

### Comparing `cpmel-3.5.0/src/cpmel/exc.py` & `cpmel-3.6.0/src/cpmel/exc.py`

 * *Files identical despite different names*

### Comparing `cpmel-3.5.0/src/cpmel/versions.py` & `cpmel-3.6.0/src/cpmel/versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         s = "{}.{}.{}".format(self.major, self.minor, self.patch)
         if self.adv_ver < R:
             s += "-{}.{}".format(adv_ver_conv(self.adv_ver), self.adv_ver_index)
         return s
 
 
 def ver_info():
-    return VersionInfo(major=3, minor=5, patch=0, adv_ver=R, adv_ver_index=0)
+    return VersionInfo(major=3, minor=6, patch=0, adv_ver=R, adv_ver_index=0)
 
 
 def ver_str():
     return ver_info().to_str()
 
 
 if __name__ == "__main__":
```

### Comparing `cpmel-3.5.0/src/cpmel.egg-info/PKG-INFO` & `cpmel-3.6.0/src/cpmel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: cpmel
-Version: 3.5.0
+Version: 3.6.0
 Summary: 一个现代的maya python库
 Home-page: https://github.com/cpcgskill/CPMel
 Author: cpcgskill
 Author-email: cpcgskill@outlook.com
 License: Apache Software License (Apache 2.0)
 Project-URL: Bug Tracker, https://github.com/cpcgskill/CPMel/issues
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -55,15 +54,16 @@
       * [属性相关操作](#属性相关操作)
 - [版权说明](#版权说明)
 
 ## 快速开始
 
 ### 安装
 
-注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是C:\Program Files\Autodesk\Maya2018\bin\mayapy.exe
+注意下方的python是你的Python, 正常情况下可以直接通过python调用, 而Maya的python一般是"C:\\Program
+Files\\Autodesk\\<Maya版本>\\bin\\mayapy.exe"
 
 ```commandline
 python -m pip install cpmel
 ```
 
 在windows下maya的安装例子
 
@@ -259,8 +259,7 @@
 # 断开属性连接
 node.tx.disconnect(node.ty)
 ```
 
 ## 版权说明
 
 该项目签署了Apache-2.0 授权许可，详情请参阅 LICENSE
-
```

### Comparing `cpmel-3.5.0/src/cpmel.egg-info/SOURCES.txt` & `cpmel-3.6.0/src/cpmel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+README.rst
 pyproject.toml
 setup.cfg
 setup.py
 src/cpmel/__init__.py
 src/cpmel/_args_conv.py
 src/cpmel/_mel.py
 src/cpmel/cmds.py
```

