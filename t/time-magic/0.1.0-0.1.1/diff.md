# Comparing `tmp/time_magic-0.1.0.tar.gz` & `tmp/time_magic-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_magic-0.1.0.tar", last modified: Fri May  5 17:07:59 2023, max compression
+gzip compressed data, was "time_magic-0.1.1.tar", last modified: Sun May  7 07:44:49 2023, max compression
```

## Comparing `time_magic-0.1.0.tar` & `time_magic-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:07:59.844574 time_magic-0.1.0/
--rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      735 2023-05-05 17:07:59.842611 time_magic-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.1.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 17:07:59.844574 time_magic-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-05 17:07:08.000000 time_magic-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:07:59.829613 time_magic-0.1.0/time_magic/
--rw-rw-rw-   0        0        0      158 2023-05-05 17:05:23.000000 time_magic-0.1.0/time_magic/__init__.py
--rw-rw-rw-   0        0        0    10444 2023-05-05 17:05:25.000000 time_magic-0.1.0/time_magic/timebill.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:07:59.840616 time_magic-0.1.0/time_magic.egg-info/
--rw-rw-rw-   0        0        0      735 2023-05-05 17:07:59.000000 time_magic-0.1.0/time_magic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-05 17:07:59.000000 time_magic-0.1.0/time_magic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:07:59.000000 time_magic-0.1.0/time_magic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-05 17:07:59.000000 time_magic-0.1.0/time_magic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 17:07:59.000000 time_magic-0.1.0/time_magic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.120983 time_magic-0.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      735 2023-05-07 07:44:49.118973 time_magic-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 07:44:49.120983 time_magic-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-07 07:40:26.000000 time_magic-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.107005 time_magic-0.1.1/time_magic/
+-rw-rw-rw-   0        0        0      158 2023-05-07 07:40:26.000000 time_magic-0.1.1/time_magic/__init__.py
+-rw-rw-rw-   0        0        0    10732 2023-05-07 07:39:26.000000 time_magic-0.1.1/time_magic/timebill.py
+drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.117976 time_magic-0.1.1/time_magic.egg-info/
+-rw-rw-rw-   0        0        0      735 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2023-05-07 07:44:49.000000 time_magic-0.1.1/time_magic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/top_level.txt
```

### Comparing `time_magic-0.1.0/LICENSE` & `time_magic-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `time_magic-0.1.0/PKG-INFO` & `time_magic-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_magic
-Version: 0.1.0
+Version: 0.1.1
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `time_magic-0.1.0/setup.py` & `time_magic-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_magic",
-    version="0.1.0",
+    version="0.1.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="python tools all about time",
     keywords=["python", "timebill", "time_magic"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/time_magic",
```

### Comparing `time_magic-0.1.0/time_magic/timebill.py` & `time_magic-0.1.1/time_magic/timebill.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,32 @@
 logger = logging.getLogger(__name__)
 
 
 class TimeBill:
     """time bill bot"""
 
     def __init__(
-        self, count_types, origin_file: str, image_dir: str, begin_of_week: int = 3
+        self,
+        count_types,
+        origin_file: str,
+        image_dir: str,
+        begin_of_week: int = 3,
+        is_cover: bool = True,
     ):
         """
         origin_file: the file of origin data, each line is a record of time cost
         image_dir: the directory to save images
         begin_of_week: 0-6, 0 is Monday, 6 is Sunday, you can set anyday to your first day of week
+        is_cover: if True, the image will cover the old one
         """
         self.count_types = count_types
         self.origin_file = origin_file
         self.image_dir = image_dir
         self.begin_of_week = begin_of_week or 3
+        self.is_cover = is_cover
         self.files = {
             "DAY": self.origin_file.replace(".txt", "_count_day.txt"),
             "WEEK": self.origin_file.replace(".txt", "_count_week.txt"),
             "WEEK4": self.origin_file.replace(".txt", "_count_4weeks.txt"),
             "DayH": self.origin_file.replace(".txt", "_count_day_hour.txt"),
             "WeekH": self.origin_file.replace(".txt", "_count_week_hour.txt"),
             "Week4H": self.origin_file.replace(".txt", "_count_4weeks_hour.txt"),
@@ -212,17 +219,18 @@
                 f"{result_type}_{days}",
                 f"TimeBill_{days}Days_{start_day.strftime('%Y-%m-%d')}_{result_type}.png",
             )
             if not os.path.exists(os.path.dirname(pngfile)):
                 os.makedirs(os.path.dirname(pngfile))
             dfx = dfx.set_index("date")
             dfx = dfx[self.count_types]
-            if not os.path.exists(pngfile):
-                self.draw_area(dfx, title, pngfile)
             start_day += timedelta(days=days)
+            if os.path.exists(pngfile) and not self.is_cover:
+                continue
+            self.draw_area(dfx, title, pngfile)
 
     def draw_by_year(self, start_day, end_day, result_type="WEEK"):
         """draw by year, all data in one image
         start_day: the day of the year start
         end_day: the day of next year start
         """
         df = pd.read_csv(self.files[result_type], delimiter="\t")
@@ -240,21 +248,22 @@
                 end_day.strftime("%Y-%m-%d"),
                 f" {days} Days TimeBill ({result_type})",
             ]
         )
         pngfile = os.path.join(
             self.image_dir,
             f"{result_type}_YEAR",
-            f"TimeBill_Year_{start_day.strftime('%Y-%m-%d')}_{result_type}.png",
+            f"TimeBill_Year_{start_day.strftime('%Y-%m-%d')}_{end_day.strftime('%Y-%m-%d')}_{result_type}.png",
         )
         if not os.path.exists(os.path.dirname(pngfile)):
             os.makedirs(os.path.dirname(pngfile))
         dfx = dfx.set_index("date")
         dfx = dfx[self.count_types]
-        self.draw_area(dfx, title, pngfile)
+        if not os.path.exists(pngfile) or self.is_cover:
+            self.draw_area(dfx, title, pngfile)
 
     def update_draws(self, start_year=2017, month=7, day=20):
         """
         start_year: the year that start to count
         month: the month of the year that start to count
         day: the day of the month that start to count
         month-day can be your birthday or other special day
```

### Comparing `time_magic-0.1.0/time_magic.egg-info/PKG-INFO` & `time_magic-0.1.1/time_magic.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-magic
-Version: 0.1.0
+Version: 0.1.1
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

