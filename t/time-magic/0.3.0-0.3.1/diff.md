# Comparing `tmp/time_magic-0.3.0.tar.gz` & `tmp/time_magic-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_magic-0.3.0.tar", last modified: Sun May  7 13:48:33 2023, max compression
+gzip compressed data, was "time_magic-0.3.1.tar", last modified: Sun May  7 14:09:10 2023, max compression
```

## Comparing `time_magic-0.3.0.tar` & `time_magic-0.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.665326 time_magic-0.3.0/
--rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.3.0/LICENSE
--rw-rw-rw-   0        0        0      735 2023-05-07 13:48:33.664331 time_magic-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.3.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 13:48:33.665326 time_magic-0.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-07 13:42:32.000000 time_magic-0.3.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.652361 time_magic-0.3.0/time_magic/
--rw-rw-rw-   0        0        0      266 2023-05-07 13:42:32.000000 time_magic-0.3.0/time_magic/__init__.py
--rw-rw-rw-   0        0        0     2802 2023-05-07 13:46:43.000000 time_magic-0.3.0/time_magic/life_in_weeks.py
--rw-rw-rw-   0        0        0     3217 2023-05-07 12:35:03.000000 time_magic-0.3.0/time_magic/seven_years_circle.py
--rw-rw-rw-   0        0        0    10703 2023-05-07 13:46:43.000000 time_magic-0.3.0/time_magic/timebill.py
-drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.661350 time_magic-0.3.0/time_magic.egg-info/
--rw-rw-rw-   0        0        0      735 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 14:09:10.945598 time_magic-0.3.1/
+-rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0      735 2023-05-07 14:09:10.944601 time_magic-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.3.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:09:10.946605 time_magic-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-07 13:55:59.000000 time_magic-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:09:10.930638 time_magic-0.3.1/time_magic/
+-rw-rw-rw-   0        0        0      266 2023-05-07 13:55:59.000000 time_magic-0.3.1/time_magic/__init__.py
+-rw-rw-rw-   0        0        0     2882 2023-05-07 13:58:37.000000 time_magic-0.3.1/time_magic/life_in_weeks.py
+-rw-rw-rw-   0        0        0     3217 2023-05-07 12:35:03.000000 time_magic-0.3.1/time_magic/seven_years_circle.py
+-rw-rw-rw-   0        0        0    10772 2023-05-07 13:59:35.000000 time_magic-0.3.1/time_magic/timebill.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:09:10.943604 time_magic-0.3.1/time_magic.egg-info/
+-rw-rw-rw-   0        0        0      735 2023-05-07 14:09:10.000000 time_magic-0.3.1/time_magic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-07 14:09:10.000000 time_magic-0.3.1/time_magic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:09:10.000000 time_magic-0.3.1/time_magic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-07 14:09:10.000000 time_magic-0.3.1/time_magic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 14:09:10.000000 time_magic-0.3.1/time_magic.egg-info/top_level.txt
```

### Comparing `time_magic-0.3.0/LICENSE` & `time_magic-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `time_magic-0.3.0/PKG-INFO` & `time_magic-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_magic
-Version: 0.3.0
+Version: 0.3.1
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `time_magic-0.3.0/setup.py` & `time_magic-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_magic",
-    version="0.3.0",
+    version="0.3.1",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="python tools all about time",
     keywords=["python", "timebill", "time_magic"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/time_magic",
```

### Comparing `time_magic-0.3.0/time_magic/life_in_weeks.py` & `time_magic-0.3.1/time_magic/life_in_weeks.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 class LifeInWeeks:
     def __init__(
         self,
         birthday: str = "1970-1-1",
         figure_scale=1.0,
         dpi=100,
         edgecolor="black",
+        bbox_inches=None,
         years=90,
         weeks_per_year=52,
     ):
         self.years = years
         self.weeks_per_year = weeks_per_year
         self.figure_scale = figure_scale
         self.dpi = dpi
         self.edgecolor = edgecolor
+        self.bbox_inches = bbox_inches
         self.birthday = datetime.datetime.strptime(birthday, "%Y-%m-%d").date()
 
     def _patch(self, week, age, color):
         return plt.Rectangle(
             (week, age),
             1,
             1,
             linewidth=1,
             edgecolor=self.edgecolor,
             facecolor=color,
         )
 
     def draw(self):
-        fig, ax = plt.subplots(
-            figsize=(8.27 * self.figure_scale, 11.69 * self.figure_scale), dpi=self.dpi
-        )
+        figsize = (8.27 * self.figure_scale, 11.69 * self.figure_scale)
+        fig, ax = plt.subplots(figsize=figsize, dpi=self.dpi)
 
-        ax.set_title("A 90-Year Human Life in Weeks", fontsize=16)
+        ax.set_title(f"Life in Weeks Since {self.birthday}", fontsize=16)
         ax.set_xlabel("Week of Year", fontsize=12)
         ax.set_ylabel("Age", fontsize=12)
 
         ax.set_xlim([0, self.weeks_per_year])
         ax.set_ylim([0, self.years])
         ax.set_xticks(np.arange(0, self.weeks_per_year + 1, 13))
         ax.set_yticks(np.arange(0, self.years + 1, 20))
@@ -73,15 +74,15 @@
                     else:
                         color = (0.9, 0.8, 0.7, 1.0)
                 else:
                     color = (0.8, 1.0, 0.8, 1.0)  # light green
                 ax.add_patch(self._patch(week, age, color))
 
         buffer = io.BytesIO()
-        fig.savefig(buffer, format="png", dpi=self.dpi)  # , bbox_inches="tight")
+        fig.savefig(buffer, format="png", dpi=self.dpi, bbox_inches=self.bbox_inches)
         imgbytes = buffer.getvalue()
         plt.close(fig)
 
         return imgbytes
 
     def save(self, filepath="life_in_weeks.png", imgbytes=None):
         imgbytes = imgbytes or self.draw()
```

### Comparing `time_magic-0.3.0/time_magic/seven_years_circle.py` & `time_magic-0.3.1/time_magic/seven_years_circle.py`

 * *Files identical despite different names*

### Comparing `time_magic-0.3.0/time_magic/timebill.py` & `time_magic-0.3.1/time_magic/timebill.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,28 @@
     def __init__(
         self,
         count_types,
         origin_file: str,
         image_dir: str,
         begin_of_week: int = 3,
         is_cover: bool = True,
+        bbox_inches=None,
     ):
         """
         origin_file: the file of origin data, each line is a record of time cost
         image_dir: the directory to save images
         begin_of_week: 0-6, 0 is Monday, 6 is Sunday, you can set anyday to your first day of week
         is_cover: if True, the image will cover the old one
         """
         self.count_types = count_types
         self.origin_file = origin_file
         self.image_dir = image_dir
         self.begin_of_week = begin_of_week or 3
         self.is_cover = is_cover
+        self.bbox_inches = bbox_inches
         self.files = {
             "DAY": self.origin_file.replace(".txt", "_count_day.txt"),
             "WEEK": self.origin_file.replace(".txt", "_count_week.txt"),
             "WEEK4": self.origin_file.replace(".txt", "_count_4weeks.txt"),
             "DayH": self.origin_file.replace(".txt", "_count_day_hour.txt"),
             "WeekH": self.origin_file.replace(".txt", "_count_week_hour.txt"),
             "Week4H": self.origin_file.replace(".txt", "_count_4weeks_hour.txt"),
@@ -170,15 +172,15 @@
             kind="area",
             figsize=(20, 10),
             title=title,
             grid=False,
             stacked=True,
         )
         fig = ax.get_figure()
-        fig.savefig(pngfile)  # , bbox_inches="tight")
+        fig.savefig(pngfile, bbox_inches=self.bbox_inches)
         plt.close()
         logger.info("done %s", pngfile)
 
     def draw_by_weeks(
         self,
         start_day="2018-5-3",
         default_end_day="2023-4-25",
```

### Comparing `time_magic-0.3.0/time_magic.egg-info/PKG-INFO` & `time_magic-0.3.1/time_magic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-magic
-Version: 0.3.0
+Version: 0.3.1
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

