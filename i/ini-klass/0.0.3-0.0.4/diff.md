# Comparing `tmp/ini-klass-0.0.3.tar.gz` & `tmp/ini-klass-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ini-klass-0.0.3.tar", last modified: Sat Jul 30 09:10:27 2022, max compression
+gzip compressed data, was "dist/ini-klass-0.0.4.tar", last modified: Sun May  7 16:02:43 2023, max compression
```

## Comparing `ini-klass-0.0.3.tar` & `ini-klass-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tarik      (501) staff       (20)        0 2022-07-30 09:10:27.349021 ini-klass-0.0.3/
--rw-r--r--   0 tarik      (501) staff       (20)     1231 2022-07-30 09:10:27.348845 ini-klass-0.0.3/PKG-INFO
-drwxr-xr-x   0 tarik      (501) staff       (20)        0 2022-07-30 09:10:27.346850 ini-klass-0.0.3/ini/
--rw-r--r--   0 tarik      (501) staff       (20)      106 2022-06-27 12:25:03.000000 ini-klass-0.0.3/ini/__init__.py
--rw-r--r--   0 tarik      (501) staff       (20)     2205 2022-07-30 08:56:35.000000 ini-klass-0.0.3/ini/config.py
--rw-r--r--   0 tarik      (501) staff       (20)     2378 2022-06-27 12:25:03.000000 ini-klass-0.0.3/ini/item.py
--rw-r--r--   0 tarik      (501) staff       (20)      942 2022-06-27 12:25:03.000000 ini-klass-0.0.3/ini/section.py
-drwxr-xr-x   0 tarik      (501) staff       (20)        0 2022-07-30 09:10:27.347639 ini-klass-0.0.3/ini_klass.egg-info/
--rw-r--r--   0 tarik      (501) staff       (20)     1231 2022-07-30 09:10:26.000000 ini-klass-0.0.3/ini_klass.egg-info/PKG-INFO
--rw-r--r--   0 tarik      (501) staff       (20)      246 2022-07-30 09:10:27.000000 ini-klass-0.0.3/ini_klass.egg-info/SOURCES.txt
--rw-r--r--   0 tarik      (501) staff       (20)        1 2022-07-30 09:10:26.000000 ini-klass-0.0.3/ini_klass.egg-info/dependency_links.txt
--rw-r--r--   0 tarik      (501) staff       (20)        9 2022-07-30 09:10:27.000000 ini-klass-0.0.3/ini_klass.egg-info/top_level.txt
--rw-r--r--   0 tarik      (501) staff       (20)       38 2022-07-30 09:10:27.349075 ini-klass-0.0.3/setup.cfg
--rw-r--r--   0 tarik      (501) staff       (20)     1088 2022-07-30 09:06:41.000000 ini-klass-0.0.3/setup.py
-drwxr-xr-x   0 tarik      (501) staff       (20)        0 2022-07-30 09:10:27.348550 ini-klass-0.0.3/test/
--rw-r--r--   0 tarik      (501) staff       (20)      119 2022-06-27 12:25:03.000000 ini-klass-0.0.3/test/__init__.py
--rw-r--r--   0 tarik      (501) staff       (20)      433 2022-06-27 12:25:03.000000 ini-klass-0.0.3/test/nullable.py
--rw-r--r--   0 tarik      (501) staff       (20)      681 2022-06-27 12:25:03.000000 ini-klass-0.0.3/test/simple.py
+drwxr-xr-x   0 tarik      (501) staff       (20)        0 2023-05-07 16:02:43.000000 ini-klass-0.0.4/
+-rw-r--r--   0 tarik      (501) staff       (20)      799 2023-05-07 16:02:43.000000 ini-klass-0.0.4/PKG-INFO
+drwxr-xr-x   0 tarik      (501) staff       (20)        0 2023-05-07 16:02:43.000000 ini-klass-0.0.4/test/
+-rw-r--r--   0 tarik      (501) staff       (20)      433 2022-06-27 12:25:03.000000 ini-klass-0.0.4/test/nullable.py
+-rw-r--r--   0 tarik      (501) staff       (20)      119 2022-06-27 12:25:03.000000 ini-klass-0.0.4/test/__init__.py
+-rw-r--r--   0 tarik      (501) staff       (20)      805 2023-05-07 15:52:45.000000 ini-klass-0.0.4/test/simple.py
+-rw-r--r--   0 tarik      (501) staff       (20)     1088 2023-05-07 15:52:45.000000 ini-klass-0.0.4/setup.py
+drwxr-xr-x   0 tarik      (501) staff       (20)        0 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini/
+-rw-r--r--   0 tarik      (501) staff       (20)     2205 2022-07-30 08:56:35.000000 ini-klass-0.0.4/ini/config.py
+-rw-r--r--   0 tarik      (501) staff       (20)      106 2022-06-27 12:25:03.000000 ini-klass-0.0.4/ini/__init__.py
+-rw-r--r--   0 tarik      (501) staff       (20)      942 2022-06-27 12:25:03.000000 ini-klass-0.0.4/ini/section.py
+-rw-r--r--   0 tarik      (501) staff       (20)     2561 2023-05-07 15:52:45.000000 ini-klass-0.0.4/ini/item.py
+drwxr-xr-x   0 tarik      (501) staff       (20)        0 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini_klass.egg-info/
+-rw-r--r--   0 tarik      (501) staff       (20)      799 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini_klass.egg-info/PKG-INFO
+-rw-r--r--   0 tarik      (501) staff       (20)      246 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini_klass.egg-info/SOURCES.txt
+-rw-r--r--   0 tarik      (501) staff       (20)        9 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini_klass.egg-info/top_level.txt
+-rw-r--r--   0 tarik      (501) staff       (20)        1 2023-05-07 16:02:43.000000 ini-klass-0.0.4/ini_klass.egg-info/dependency_links.txt
+-rw-r--r--   0 tarik      (501) staff       (20)       38 2023-05-07 16:02:43.000000 ini-klass-0.0.4/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `ini-klass-0.0.3/ini/config.py` & `ini-klass-0.0.4/ini/config.py`

 * *Files identical despite different names*

### Comparing `ini-klass-0.0.3/ini/item.py` & `ini-klass-0.0.4/ini/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,18 +30,22 @@
         for k, v in item.items():
             if k is None:
                 continue
 
             if not v.startswith('"') and not v.endswith('"') and ',' in v:
                 tys = []
                 for sv in v.split(','):
+                    if len(sv.strip()) == 0 and not empty_to_none:
+                        continue
                     tys.append(self.__cast__(sv.strip(), empty_to_none))
 
                 setattr(self, k, tys)
             else:
+                if len(v) == 0 and not empty_to_none:
+                    continue
                 setattr(self, k, self.__cast__(v, empty_to_none))
 
     def __cast__(
         self,
         value: str,
         empty_to_none: Optional[bool] = False,
     ) -> Optional[Union[str, float, bool, List[Any]]]:
```

### Comparing `ini-klass-0.0.3/ini/section.py` & `ini-klass-0.0.4/ini/section.py`

 * *Files identical despite different names*

### Comparing `ini-klass-0.0.3/setup.py` & `ini-klass-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     long_description = open('readme.md', 'r', encoding='utf8').read()
 except Exception:
     long_description = description
 
 setup(
     name='ini-klass',
-    version='0.0.3',
+    version='0.0.4',
     author='Tarik Yilmaz',
     author_email='tarikyilmaz.54@gmail.com',
     description=description,
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/trk54ylmz/ini-klass',
     include_package_data=True,
```

### Comparing `ini-klass-0.0.3/test/simple.py` & `ini-klass-0.0.4/test/simple.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from unittest import TestCase
 
 
 class SimpleTest(TestCase):
     def setUp(self):
         path = Path(__file__).parent / 'simple.ini'
 
-        self.config = IniConfig.read(str(path))
+        self.config = IniConfig.read(str(path), empty_to_none=False)
 
     def test_numeric(self):
         self.assertEqual(self.config.example.id, 12)
 
     def test_string(self):
         self.assertEqual(self.config.example.name, 'John')
 
@@ -19,7 +19,10 @@
         self.assertEqual(self.config.example.status, True)
 
     def test_float(self):
         self.assertEqual(self.config.example.salary, 100.5)
 
     def test_list(self):
         self.assertEqual(self.config.example.group, ['car', 'book', 'phone'])
+
+    def test_empty_list(self):
+        self.assertEqual(self.config.example.detail, ['user', 'name'])
```

