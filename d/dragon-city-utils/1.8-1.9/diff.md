# Comparing `tmp/dragon-city-utils-1.8.tar.gz` & `tmp/dragon-city-utils-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragon-city-utils-1.8.tar", last modified: Tue Mar  7 01:10:26 2023, max compression
+gzip compressed data, was "dragon-city-utils-1.9.tar", last modified: Tue Mar  7 01:14:13 2023, max compression
```

## Comparing `dragon-city-utils-1.8.tar` & `dragon-city-utils-1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.454981 dragon-city-utils-1.8/
--rw-rw-rw-   0        0        0     2659 2023-03-07 01:10:26.453984 dragon-city-utils-1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2376 2023-03-05 15:09:32.000000 dragon-city-utils-1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.275983 dragon-city-utils-1.8/dcutils/
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.332982 dragon-city-utils-1.8/dcutils/calculators/
--rw-rw-rw-   0        0        0      212 2023-03-05 14:23:15.000000 dragon-city-utils-1.8/dcutils/calculators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.336981 dragon-city-utils-1.8/dcutils/calculators/elements/
--rw-rw-rw-   0        0        0      744 2023-03-05 14:04:39.000000 dragon-city-utils-1.8/dcutils/calculators/elements/__init__.py
--rw-rw-rw-   0        0        0     2059 2023-03-05 14:03:46.000000 dragon-city-utils-1.8/dcutils/calculators/elements/config.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.338992 dragon-city-utils-1.8/dcutils/calculators/food/
--rw-rw-rw-   0        0        0      176 2023-03-05 14:10:21.000000 dragon-city-utils-1.8/dcutils/calculators/food/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.345981 dragon-city-utils-1.8/dcutils/calculators/orb_recall/
--rw-rw-rw-   0        0        0     1090 2023-03-05 14:33:54.000000 dragon-city-utils-1.8/dcutils/calculators/orb_recall/__init__.py
--rw-rw-rw-   0        0        0      362 2023-03-05 14:27:12.000000 dragon-city-utils-1.8/dcutils/calculators/orb_recall/config.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.355982 dragon-city-utils-1.8/dcutils/static/
--rw-rw-rw-   0        0        0        0 2023-03-07 00:56:25.000000 dragon-city-utils-1.8/dcutils/static/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.368988 dragon-city-utils-1.8/dcutils/static/animations/
--rw-rw-rw-   0        0        0       94 2023-03-03 17:28:33.000000 dragon-city-utils-1.8/dcutils/static/animations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.414980 dragon-city-utils-1.8/dcutils/static/animations/flash/
--rw-rw-rw-   0        0        0      715 2023-03-03 18:45:36.000000 dragon-city-utils-1.8/dcutils/static/animations/flash/dragon.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.417984 dragon-city-utils-1.8/dcutils/static/animations/spine/
--rw-rw-rw-   0        0        0     1119 2023-03-03 18:57:26.000000 dragon-city-utils-1.8/dcutils/static/animations/spine/dragon.py
--rw-rw-rw-   0        0        0      266 2023-03-03 01:37:05.000000 dragon-city-utils-1.8/dcutils/static/base.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.380979 dragon-city-utils-1.8/dcutils/static/islands/
--rw-rw-rw-   0        0        0       65 2023-03-03 21:55:42.000000 dragon-city-utils-1.8/dcutils/static/islands/__init__.py
--rw-rw-rw-   0        0        0      469 2023-03-03 21:55:12.000000 dragon-city-utils-1.8/dcutils/static/islands/package.py
--rw-rw-rw-   0        0        0     4357 2023-03-07 01:10:08.000000 dragon-city-utils-1.8/dcutils/static/localization.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.386984 dragon-city-utils-1.8/dcutils/static/sounds/
--rw-rw-rw-   0        0        0       62 2023-03-04 02:17:42.000000 dragon-city-utils-1.8/dcutils/static/sounds/__init__.py
--rw-rw-rw-   0        0        0      309 2023-03-04 01:57:21.000000 dragon-city-utils-1.8/dcutils/static/sounds/musics.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.405986 dragon-city-utils-1.8/dcutils/static/sprites/
--rw-rw-rw-   0        0        0      175 2023-03-03 01:52:57.000000 dragon-city-utils-1.8/dcutils/static/sprites/__init__.py
--rw-rw-rw-   0        0        0      569 2023-03-03 01:51:53.000000 dragon-city-utils-1.8/dcutils/static/sprites/chest.py
--rw-rw-rw-   0        0        0     1038 2023-03-03 01:50:15.000000 dragon-city-utils-1.8/dcutils/static/sprites/dragon.py
--rw-rw-rw-   0        0        0      716 2023-03-03 01:51:11.000000 dragon-city-utils-1.8/dcutils/static/sprites/dragon_thumb.py
-drwxrwxrwx   0        0        0        0 2023-03-07 01:10:26.451986 dragon-city-utils-1.8/dragon_city_utils.egg-info/
--rw-rw-rw-   0        0        0     2659 2023-03-07 01:10:26.000000 dragon-city-utils-1.8/dragon_city_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1558 2023-03-07 01:10:26.000000 dragon-city-utils-1.8/dragon_city_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-07 01:10:26.000000 dragon-city-utils-1.8/dragon_city_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-03-07 01:10:26.000000 dragon-city-utils-1.8/dragon_city_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-03-07 01:10:26.000000 dragon-city-utils-1.8/dragon_city_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-07 01:10:26.455979 dragon-city-utils-1.8/setup.cfg
--rw-rw-rw-   0        0        0      611 2023-03-07 01:10:21.000000 dragon-city-utils-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.843319 dragon-city-utils-1.9/
+-rw-rw-rw-   0        0        0     2659 2023-03-07 01:14:13.842321 dragon-city-utils-1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2376 2023-03-05 15:09:32.000000 dragon-city-utils-1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.661321 dragon-city-utils-1.9/dcutils/
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.701324 dragon-city-utils-1.9/dcutils/calculators/
+-rw-rw-rw-   0        0        0      212 2023-03-05 14:23:15.000000 dragon-city-utils-1.9/dcutils/calculators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.709323 dragon-city-utils-1.9/dcutils/calculators/elements/
+-rw-rw-rw-   0        0        0      744 2023-03-05 14:04:39.000000 dragon-city-utils-1.9/dcutils/calculators/elements/__init__.py
+-rw-rw-rw-   0        0        0     2059 2023-03-05 14:03:46.000000 dragon-city-utils-1.9/dcutils/calculators/elements/config.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.711321 dragon-city-utils-1.9/dcutils/calculators/food/
+-rw-rw-rw-   0        0        0      176 2023-03-05 14:10:21.000000 dragon-city-utils-1.9/dcutils/calculators/food/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.716330 dragon-city-utils-1.9/dcutils/calculators/orb_recall/
+-rw-rw-rw-   0        0        0     1090 2023-03-05 14:33:54.000000 dragon-city-utils-1.9/dcutils/calculators/orb_recall/__init__.py
+-rw-rw-rw-   0        0        0      362 2023-03-05 14:27:12.000000 dragon-city-utils-1.9/dcutils/calculators/orb_recall/config.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.727322 dragon-city-utils-1.9/dcutils/static/
+-rw-rw-rw-   0        0        0        0 2023-03-07 00:56:25.000000 dragon-city-utils-1.9/dcutils/static/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.730321 dragon-city-utils-1.9/dcutils/static/animations/
+-rw-rw-rw-   0        0        0       94 2023-03-03 17:28:33.000000 dragon-city-utils-1.9/dcutils/static/animations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.768320 dragon-city-utils-1.9/dcutils/static/animations/flash/
+-rw-rw-rw-   0        0        0      715 2023-03-03 18:45:36.000000 dragon-city-utils-1.9/dcutils/static/animations/flash/dragon.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.774322 dragon-city-utils-1.9/dcutils/static/animations/spine/
+-rw-rw-rw-   0        0        0     1119 2023-03-03 18:57:26.000000 dragon-city-utils-1.9/dcutils/static/animations/spine/dragon.py
+-rw-rw-rw-   0        0        0      266 2023-03-03 01:37:05.000000 dragon-city-utils-1.9/dcutils/static/base.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.736320 dragon-city-utils-1.9/dcutils/static/islands/
+-rw-rw-rw-   0        0        0       65 2023-03-03 21:55:42.000000 dragon-city-utils-1.9/dcutils/static/islands/__init__.py
+-rw-rw-rw-   0        0        0      469 2023-03-03 21:55:12.000000 dragon-city-utils-1.9/dcutils/static/islands/package.py
+-rw-rw-rw-   0        0        0     4644 2023-03-07 01:13:44.000000 dragon-city-utils-1.9/dcutils/static/localization.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.742326 dragon-city-utils-1.9/dcutils/static/sounds/
+-rw-rw-rw-   0        0        0       62 2023-03-04 02:17:42.000000 dragon-city-utils-1.9/dcutils/static/sounds/__init__.py
+-rw-rw-rw-   0        0        0      309 2023-03-04 01:57:21.000000 dragon-city-utils-1.9/dcutils/static/sounds/musics.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.756321 dragon-city-utils-1.9/dcutils/static/sprites/
+-rw-rw-rw-   0        0        0      175 2023-03-03 01:52:57.000000 dragon-city-utils-1.9/dcutils/static/sprites/__init__.py
+-rw-rw-rw-   0        0        0      569 2023-03-03 01:51:53.000000 dragon-city-utils-1.9/dcutils/static/sprites/chest.py
+-rw-rw-rw-   0        0        0     1038 2023-03-03 01:50:15.000000 dragon-city-utils-1.9/dcutils/static/sprites/dragon.py
+-rw-rw-rw-   0        0        0      716 2023-03-03 01:51:11.000000 dragon-city-utils-1.9/dcutils/static/sprites/dragon_thumb.py
+drwxrwxrwx   0        0        0        0 2023-03-07 01:14:13.840322 dragon-city-utils-1.9/dragon_city_utils.egg-info/
+-rw-rw-rw-   0        0        0     2659 2023-03-07 01:14:13.000000 dragon-city-utils-1.9/dragon_city_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1558 2023-03-07 01:14:13.000000 dragon-city-utils-1.9/dragon_city_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-07 01:14:13.000000 dragon-city-utils-1.9/dragon_city_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-03-07 01:14:13.000000 dragon-city-utils-1.9/dragon_city_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-03-07 01:14:13.000000 dragon-city-utils-1.9/dragon_city_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-07 01:14:13.843319 dragon-city-utils-1.9/setup.cfg
+-rw-rw-rw-   0        0        0      611 2023-03-07 01:14:09.000000 dragon-city-utils-1.9/setup.py
```

### Comparing `dragon-city-utils-1.8/PKG-INFO` & `dragon-city-utils-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon-city-utils
-Version: 1.8
+Version: 1.9
 Summary: Utilities and tools for things related to Dragon City
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

### Comparing `dragon-city-utils-1.8/README.md` & `dragon-city-utils-1.9/README.md`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/calculators/elements/__init__.py` & `dragon-city-utils-1.9/dcutils/calculators/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/calculators/elements/config.py` & `dragon-city-utils-1.9/dcutils/calculators/elements/config.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/calculators/orb_recall/__init__.py` & `dragon-city-utils-1.9/dcutils/calculators/orb_recall/__init__.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/static/animations/flash/dragon.py` & `dragon-city-utils-1.9/dcutils/static/animations/flash/dragon.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/static/animations/spine/dragon.py` & `dragon-city-utils-1.9/dcutils/static/animations/spine/dragon.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/static/localization.py` & `dragon-city-utils-1.9/dcutils/static/localization.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,23 +10,35 @@
         self.__localization_dict = FromList(self.__localization).join_keys_of_child_dicts_in_a_new_dict()
 
     def __fetch(self) -> list[dict]:
         response = httpx.get(self.__endpoint_url)
         data = response.json()
         return data
 
+    @validate_arguments
     @classmethod
     def load(cls, loc: list[dict]):
         cls.__localization = loc
         cls.__localization_dict = FromList(loc).join_keys_of_child_dicts_in_a_new_dict()
 
         return cls
 
     @validate_arguments
     @classmethod
+    def load_dict(cls, loc: dict):
+        cls.__localization_dict = loc
+        cls.__localization = {}
+
+        for key, value in loc.items():
+            cls.__localization[key] = value
+
+        return cls
+
+    @validate_arguments
+    @classmethod
     def get_value_from_key(cls, key: str) -> str | None:
         if key in cls.__localization_dict.keys():
             return cls.__localization_dict[key]
 
     @validate_arguments
     @classmethod
     def get_key_from_value(cls, value: str) -> str | None:
```

### Comparing `dragon-city-utils-1.8/dcutils/static/sprites/chest.py` & `dragon-city-utils-1.9/dcutils/static/sprites/chest.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/static/sprites/dragon.py` & `dragon-city-utils-1.9/dcutils/static/sprites/dragon.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dcutils/static/sprites/dragon_thumb.py` & `dragon-city-utils-1.9/dcutils/static/sprites/dragon_thumb.py`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/dragon_city_utils.egg-info/PKG-INFO` & `dragon-city-utils-1.9/dragon_city_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragon-city-utils
-Version: 1.8
+Version: 1.9
 Summary: Utilities and tools for things related to Dragon City
 Author: Marcuth
 Author-email: marcuth2006@gmail.com
 License: MIT License
 Keywords: dragoncity dcutils tools
 Description-Content-Type: text/markdown
```

### Comparing `dragon-city-utils-1.8/dragon_city_utils.egg-info/SOURCES.txt` & `dragon-city-utils-1.9/dragon_city_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragon-city-utils-1.8/setup.py` & `dragon-city-utils-1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as file:
     readme_content = file.read()
 
 setup(
     name="dragon-city-utils",
-    version="1.8",
+    version="1.9",
     license="MIT License",
     author="Marcuth",
     long_description=readme_content,
     long_description_content_type="text/markdown",
     author_email="marcuth2006@gmail.com",
     keywords="dragoncity dcutils tools",
     description=f"Utilities and tools for things related to Dragon City",
```

