# Comparing `tmp/time_magic-0.1.1.tar.gz` & `tmp/time_magic-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "time_magic-0.1.1.tar", last modified: Sun May  7 07:44:49 2023, max compression
+gzip compressed data, was "time_magic-0.3.0.tar", last modified: Sun May  7 13:48:33 2023, max compression
```

## Comparing `time_magic-0.1.1.tar` & `time_magic-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.120983 time_magic-0.1.1/
--rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      735 2023-05-07 07:44:49.118973 time_magic-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-07 07:44:49.120983 time_magic-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1049 2023-05-07 07:40:26.000000 time_magic-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.107005 time_magic-0.1.1/time_magic/
--rw-rw-rw-   0        0        0      158 2023-05-07 07:40:26.000000 time_magic-0.1.1/time_magic/__init__.py
--rw-rw-rw-   0        0        0    10732 2023-05-07 07:39:26.000000 time_magic-0.1.1/time_magic/timebill.py
-drwxrwxrwx   0        0        0        0 2023-05-07 07:44:49.117976 time_magic-0.1.1/time_magic.egg-info/
--rw-rw-rw-   0        0        0      735 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-07 07:44:49.000000 time_magic-0.1.1/time_magic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-07 07:44:48.000000 time_magic-0.1.1/time_magic.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.665326 time_magic-0.3.0/
+-rw-rw-rw-   0        0        0     1087 2023-05-05 12:27:17.000000 time_magic-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      735 2023-05-07 13:48:33.664331 time_magic-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0       31 2023-05-05 12:27:17.000000 time_magic-0.3.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 13:48:33.665326 time_magic-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1049 2023-05-07 13:42:32.000000 time_magic-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.652361 time_magic-0.3.0/time_magic/
+-rw-rw-rw-   0        0        0      266 2023-05-07 13:42:32.000000 time_magic-0.3.0/time_magic/__init__.py
+-rw-rw-rw-   0        0        0     2802 2023-05-07 13:46:43.000000 time_magic-0.3.0/time_magic/life_in_weeks.py
+-rw-rw-rw-   0        0        0     3217 2023-05-07 12:35:03.000000 time_magic-0.3.0/time_magic/seven_years_circle.py
+-rw-rw-rw-   0        0        0    10703 2023-05-07 13:46:43.000000 time_magic-0.3.0/time_magic/timebill.py
+drwxrwxrwx   0        0        0        0 2023-05-07 13:48:33.661350 time_magic-0.3.0/time_magic.egg-info/
+-rw-rw-rw-   0        0        0      735 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-07 13:48:33.000000 time_magic-0.3.0/time_magic.egg-info/top_level.txt
```

### Comparing `time_magic-0.1.1/LICENSE` & `time_magic-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `time_magic-0.1.1/PKG-INFO` & `time_magic-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time_magic
-Version: 0.1.1
+Version: 0.3.0
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

### Comparing `time_magic-0.1.1/setup.py` & `time_magic-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="time_magic",
-    version="0.1.1",
+    version="0.3.0",
     author="liujuanjuan1984",
     author_email="qiaoanlu@163.com",
     description="python tools all about time",
     keywords=["python", "timebill", "time_magic"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/liujuanjuan1984/time_magic",
```

### Comparing `time_magic-0.1.1/time_magic/timebill.py` & `time_magic-0.3.0/time_magic/timebill.py`

 * *Files 2% similar despite different names*

```diff
@@ -170,15 +170,15 @@
             kind="area",
             figsize=(20, 10),
             title=title,
             grid=False,
             stacked=True,
         )
         fig = ax.get_figure()
-        fig.savefig(pngfile)
+        fig.savefig(pngfile)  # , bbox_inches="tight")
         plt.close()
         logger.info("done %s", pngfile)
 
     def draw_by_weeks(
         self,
         start_day="2018-5-3",
         default_end_day="2023-4-25",
@@ -197,16 +197,15 @@
 
         days = 7 * weeks
         start_day = datetime.strptime(start_day, "%Y-%m-%d")
         default_end_day = datetime.strptime(default_end_day, "%Y-%m-%d")
 
         while start_day < datetime.now() and start_day < default_end_day:
             end_day = start_day + timedelta(days=days - 1)
-            if end_day > datetime.now():
-                logger.info("end_day > now, break")
+            if start_day > datetime.now():
                 break
             dfx = df[(df["date"] >= start_day) & (df["date"] <= end_day)]
             title = "".join(
                 [
                     start_day.strftime("%Y-%m-%d"),
                     " - ",
                     end_day.strftime("%Y-%m-%d"),
@@ -248,15 +247,15 @@
                 end_day.strftime("%Y-%m-%d"),
                 f" {days} Days TimeBill ({result_type})",
             ]
         )
         pngfile = os.path.join(
             self.image_dir,
             f"{result_type}_YEAR",
-            f"TimeBill_Year_{start_day.strftime('%Y-%m-%d')}_{end_day.strftime('%Y-%m-%d')}_{result_type}.png",
+            f"TimeBill_{start_day.strftime('%Y-%m-%d')}_{end_day.strftime('%Y-%m-%d')}_{result_type}.png",
         )
         if not os.path.exists(os.path.dirname(pngfile)):
             os.makedirs(os.path.dirname(pngfile))
         dfx = dfx.set_index("date")
         dfx = dfx[self.count_types]
         if not os.path.exists(pngfile) or self.is_cover:
             self.draw_area(dfx, title, pngfile)
```

### Comparing `time_magic-0.1.1/time_magic.egg-info/PKG-INFO` & `time_magic-0.3.0/time_magic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: time-magic
-Version: 0.1.1
+Version: 0.3.0
 Summary: python tools all about time
 Home-page: https://github.com/liujuanjuan1984/time_magic
 Author: liujuanjuan1984
 Author-email: qiaoanlu@163.com
 Project-URL: Github Repo, https://github.com/liujuanjuan1984/time_magic
 Project-URL: Bug Tracker, https://github.com/liujuanjuan1984/time_magic/issues
 Project-URL: About Quorum, https://github.com/rumsystem/quorum
```

