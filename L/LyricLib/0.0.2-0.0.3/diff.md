# Comparing `tmp/LyricLib-0.0.2.tar.gz` & `tmp/LyricLib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LyricLib-0.0.2.tar", last modified: Mon May  1 03:40:47 2023, max compression
+gzip compressed data, was "LyricLib-0.0.3.tar", last modified: Sun May  7 03:04:30 2023, max compression
```

## Comparing `LyricLib-0.0.2.tar` & `LyricLib-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 03:40:47.786404 LyricLib-0.0.2/
--rw-rw-rw-   0        0        0    12937 2023-05-01 02:54:44.000000 LyricLib-0.0.2/LICENSE.md
-drwxrwxrwx   0        0        0        0 2023-05-01 03:40:47.777440 LyricLib-0.0.2/LyricLib/
--rw-rw-rw-   0        0        0      619 2023-05-01 03:40:42.000000 LyricLib-0.0.2/LyricLib/__init__.py
--rw-rw-rw-   0        0        0     1241 2023-05-01 02:54:44.000000 LyricLib-0.0.2/LyricLib/constants.py
--rw-rw-rw-   0        0        0     1053 2023-05-01 02:54:44.000000 LyricLib-0.0.2/LyricLib/exceptions.py
--rw-rw-rw-   0        0        0     7715 2023-05-01 03:40:42.000000 LyricLib-0.0.2/LyricLib/main.py
--rw-rw-rw-   0        0        0    10867 2023-05-01 02:54:44.000000 LyricLib-0.0.2/LyricLib/subclass.py
-drwxrwxrwx   0        0        0        0 2023-05-01 03:40:47.783398 LyricLib-0.0.2/LyricLib.egg-info/
--rw-rw-rw-   0        0        0     2745 2023-05-01 03:40:47.000000 LyricLib-0.0.2/LyricLib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-01 03:40:47.000000 LyricLib-0.0.2/LyricLib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 03:40:47.000000 LyricLib-0.0.2/LyricLib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 03:40:47.000000 LyricLib-0.0.2/LyricLib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2745 2023-05-01 03:40:47.785441 LyricLib-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1795 2023-05-01 02:56:30.000000 LyricLib-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-01 03:40:47.786404 LyricLib-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1322 2023-05-01 03:40:42.000000 LyricLib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.431396 LyricLib-0.0.3/
+-rw-rw-rw-   0        0        0    12937 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LICENSE.md
+drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.416446 LyricLib-0.0.3/LyricLib/
+-rw-rw-rw-   0        0        0     1261 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/LICENSE(lrc-parser).md
+-rw-rw-rw-   0        0        0      619 2023-05-07 03:03:51.000000 LyricLib-0.0.3/LyricLib/__init__.py
+-rw-rw-rw-   0        0        0     1241 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/constants.py
+-rw-rw-rw-   0        0        0     1053 2023-05-01 02:54:44.000000 LyricLib-0.0.3/LyricLib/exceptions.py
+-rw-rw-rw-   0        0        0     7715 2023-05-01 03:40:42.000000 LyricLib-0.0.3/LyricLib/main.py
+-rw-rw-rw-   0        0        0    11166 2023-05-07 03:03:51.000000 LyricLib-0.0.3/LyricLib/subclass.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.425415 LyricLib-0.0.3/LyricLib.egg-info/
+-rw-rw-rw-   0        0        0     2745 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      404 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-07 03:04:30.000000 LyricLib-0.0.3/LyricLib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       41 2023-05-07 03:03:51.000000 LyricLib-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2745 2023-05-07 03:04:30.430400 LyricLib-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1795 2023-05-01 02:56:30.000000 LyricLib-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 03:04:30.427410 LyricLib-0.0.3/docs/
+-rw-rw-rw-   0        0        0     6577 2023-05-01 02:54:44.000000 LyricLib-0.0.3/docs/Lrc文件格式.md
+-rw-rw-rw-   0        0        0      470 2023-05-07 03:03:51.000000 LyricLib-0.0.3/docs/开发日志.TXT
+-rw-rw-rw-   0        0        0       42 2023-05-07 03:04:30.431396 LyricLib-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2023-05-07 03:03:51.000000 LyricLib-0.0.3/setup.py
```

### Comparing `LyricLib-0.0.2/LICENSE.md` & `LyricLib-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.2/LyricLib/__init__.py` & `LyricLib-0.0.3/LyricLib/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,10 +13,10 @@
 # 睿穆组织 开发交流群 861684859
 # Email TriM-Organization@hotmail.com
 # 版权所有 Lyric全体开发者
 # 若需转载或借鉴 许可声明请查看仓库目录下的 License.md
 
 from .main import *
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __all__ = []
 __author__ = (("金羿", "Eilles Wan"), ("thecasttim", "thecasttim"))
```

### Comparing `LyricLib-0.0.2/LyricLib/constants.py` & `LyricLib-0.0.3/LyricLib/constants.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.2/LyricLib/exceptions.py` & `LyricLib-0.0.3/LyricLib/exceptions.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.2/LyricLib/main.py` & `LyricLib-0.0.3/LyricLib/main.py`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.2/LyricLib/subclass.py` & `LyricLib-0.0.3/LyricLib/subclass.py`

 * *Files 3% similar despite different names*

```diff
@@ -200,18 +200,32 @@
 
     def __eq__(self, other) -> bool:
         if not isinstance(other, self.__class__):
             return False
         return self.__str__() == other.__str__()
 
     def __str__(self) -> str:
-        """直接以最完整的格式输出字符串"""
+        """
+        直接以最完整的格式输出字符串
+        """
         return "{}:{}:{}.{}".format(
             self.get_hours, self.get_minutes, self.get_seconds, self.get_microseconds
         )
+    
+    def __lt__(self, other) -> bool:
+        """
+        判小于
+        """
+        return self.in_microseconds < other.in_microseconds
+
+    def __cmp__(self, other) -> int:
+        """
+        比较
+        """
+        return self.in_microseconds - other.in_microseconds
 
     def to_lrc_str(self, format_style: str = STABLE_LRC_TIME_FORMAT_STYLE) -> str:
         """
         以特定样式的LRC格式的时间标签返回字符串
         """
         now_exp = self.__dict__()
         rep_exp = {}
```

### Comparing `LyricLib-0.0.2/LyricLib.egg-info/PKG-INFO` & `LyricLib-0.0.3/LyricLib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.2
+Version: 0.0.3
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `LyricLib-0.0.2/PKG-INFO` & `LyricLib-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LyricLib
-Version: 0.0.2
+Version: 0.0.3
 Summary: 歌词的处理库
 Home-page: https://github.com/TriM-Organization/Lyric
 Author: Eilles Wan, bgArray
 Author-email: TriM-Organization@hotmail.com
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `LyricLib-0.0.2/README.md` & `LyricLib-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `LyricLib-0.0.2/setup.py` & `LyricLib-0.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     author_email="TriM-Organization@hotmail.com",
     description="歌词的处理库\n"
     "A library for processing lyrics.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TriM-Organization/Lyric",
     packages=setuptools.find_packages(),
+    include_package_data=True,
     classifiers=[
         "Intended Audience :: Developers",
         "Natural Language :: Chinese (Simplified)",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python",
```

