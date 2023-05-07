# Comparing `tmp/HumanCursor-0.0.5.tar.gz` & `tmp/HumanCursor-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.5.tar", last modified: Fri May  5 15:45:41 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.6.tar", last modified: Sun May  7 16:22:49 2023, max compression
```

## Comparing `HumanCursor-0.0.5.tar` & `HumanCursor-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/
-drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.959745 HumanCursor-0.0.5/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5384 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      451 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-05 15:45:41.000000 HumanCursor-0.0.5/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     5384 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.964646 HumanCursor-0.0.5/humancursor/
--rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.5/humancursor/__init__.py
--rw-rw-rw-   0        0        0     2027 2023-05-05 14:49:34.000000 HumanCursor-0.0.5/humancursor/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.970351 HumanCursor-0.0.5/humancursor/test/
--rw-rw-rw-   0        0        0      275 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/humancursor/test/system.py
--rw-rw-rw-   0        0        0     1119 2023-05-05 15:45:08.000000 HumanCursor-0.0.5/humancursor/test/web.py
-drwxrwxrwx   0        0        0        0 2023-05-05 15:45:41.979754 HumanCursor-0.0.5/humancursor/utilities/
--rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.5/humancursor/utilities/calc.py
--rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.5/humancursor/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.5/humancursor/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.5/humancursor/web_cursor.py
--rw-rw-rw-   0        0        0      667 2023-05-05 15:39:56.000000 HumanCursor-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 15:45:41.982925 HumanCursor-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.904893 HumanCursor-0.0.6/
+drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.826840 HumanCursor-0.0.6/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5384 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      451 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-07 16:22:49.000000 HumanCursor-0.0.6/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5384 2023-05-07 16:22:49.903858 HumanCursor-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4903 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.843884 HumanCursor-0.0.6/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.6/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     2282 2023-05-07 16:22:16.000000 HumanCursor-0.0.6/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.868708 HumanCursor-0.0.6/humancursor/test/
+-rw-rw-rw-   0        0        0      275 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/humancursor/test/system.py
+-rw-rw-rw-   0        0        0     1119 2023-05-05 15:45:08.000000 HumanCursor-0.0.6/humancursor/test/web.py
+drwxrwxrwx   0        0        0        0 2023-05-07 16:22:49.902015 HumanCursor-0.0.6/humancursor/utilities/
+-rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.6/humancursor/utilities/calc.py
+-rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.6/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.6/humancursor/utilities/web_adjuster.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.6/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      667 2023-05-07 16:22:16.000000 HumanCursor-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 16:22:49.904893 HumanCursor-0.0.6/setup.cfg
```

### Comparing `HumanCursor-0.0.5/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.6/HumanCursor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.5/LICENSE` & `HumanCursor-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/PKG-INFO` & `HumanCursor-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.5/README.md` & `HumanCursor-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/humancursor/system_cursor.py` & `HumanCursor-0.0.6/humancursor/system_cursor.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from humancursor.utilities.calc import generate_random_curve_parameters
 
 
 class SystemCursor:
     def __init__(self):
         pyautogui.MINIMUM_DURATION = 0
         pyautogui.MINIMUM_SLEEP = 0
-        pyautogui.PAUSE = 0.015
+        pyautogui.PAUSE = 0
 
     @staticmethod
     def move_to(point: list, duration: int = None, human_curve=None):
         """Moves to certain coordinates of screen"""
         from_point = pyautogui.position()
 
         if not human_curve:
@@ -52,7 +52,14 @@
 
     def click_on(self, point: list, clicks: int = 1):
         """Clicks a specified number of times, on the specified coordinates"""
         self.move_to(point)
         for _ in range(clicks):
             pyautogui.click()
             sleep(random.uniform(0.150, 0.300))
+
+    def drag_and_drop(self, from_point: list, to_point: list):
+        """Drags from a certain point, and releases to another"""
+        self.move_to(from_point)
+        pyautogui.mouseDown()
+        self.move_to(to_point)
+        pyautogui.mouseUp()
```

### Comparing `HumanCursor-0.0.5/humancursor/test/web.py` & `HumanCursor-0.0.6/humancursor/test/web.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/humancursor/utilities/calc.py` & `HumanCursor-0.0.6/humancursor/utilities/calc.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/humancursor/utilities/human_curve_generator.py` & `HumanCursor-0.0.6/humancursor/utilities/human_curve_generator.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/humancursor/utilities/web_adjuster.py` & `HumanCursor-0.0.6/humancursor/utilities/web_adjuster.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/humancursor/web_cursor.py` & `HumanCursor-0.0.6/humancursor/web_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.5/pyproject.toml` & `HumanCursor-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

