# Comparing `tmp/aij-webcam-1.1.3.tar.gz` & `tmp/aij-webcam-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-webcam-1.1.3.tar", last modified: Sat May  6 19:27:30 2023, max compression
+gzip compressed data, was "aij-webcam-1.1.4.tar", last modified: Sat May  6 21:02:10 2023, max compression
```

## Comparing `aij-webcam-1.1.3.tar` & `aij-webcam-1.1.4.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/
--rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0     4270 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.3/README.md
--rw-rw-rw-   0        0        0     6368 2023-05-06 19:27:10.000000 aij-webcam-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/
--rw-rw-rw-   0        0        0     4270 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      175 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/aij_webcam.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/news/
--rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.3/src/news/__init__.py
--rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.3/src/news/core.py
--rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.3/src/news/publisher.py
--rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.3/src/news/subscriber.py
-drwxrwxrwx   0        0        0        0 2023-05-06 19:27:32.000000 aij-webcam-1.1.3/src/webcam/
--rw-rw-rw-   0        0        0    17500 2023-05-05 13:14:12.000000 aij-webcam-1.1.3/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/
+-rw-rw-rw-   0        0        0     1100 2023-05-05 12:30:16.000000 aij-webcam-1.1.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     4270 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1830 2023-05-05 12:30:36.000000 aij-webcam-1.1.4/README.md
+-rw-rw-rw-   0        0        0     6392 2023-05-06 21:01:56.000000 aij-webcam-1.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/
+-rw-rw-rw-   0        0        0     4270 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       81 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      175 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/aij_webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/intro/
+-rw-rw-rw-   0        0        0      463 2023-05-06 21:00:54.000000 aij-webcam-1.1.4/src/intro/__init__.py
+-rw-rw-rw-   0        0        0     4524 2023-05-06 21:01:00.000000 aij-webcam-1.1.4/src/intro/intro.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/news/
+-rw-rw-rw-   0        0        0      567 2023-05-05 12:40:48.000000 aij-webcam-1.1.4/src/news/__init__.py
+-rw-rw-rw-   0        0        0     4490 2023-05-05 12:35:58.000000 aij-webcam-1.1.4/src/news/core.py
+-rw-rw-rw-   0        0        0     3663 2023-05-05 12:51:30.000000 aij-webcam-1.1.4/src/news/publisher.py
+-rw-rw-rw-   0        0        0     1196 2023-05-05 12:37:32.000000 aij-webcam-1.1.4/src/news/subscriber.py
+drwxrwxrwx   0        0        0        0 2023-05-06 21:02:12.000000 aij-webcam-1.1.4/src/webcam/
+-rw-rw-rw-   0        0        0    17500 2023-05-06 19:32:44.000000 aij-webcam-1.1.4/src/webcam/__init__.py
```

### Comparing `aij-webcam-1.1.3/LICENSE.txt` & `aij-webcam-1.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/PKG-INFO` & `aij-webcam-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.3/README.md` & `aij-webcam-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/pyproject.toml` & `aij-webcam-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij-webcam"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.3"
+version = "1.1.4"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist GUI Application"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -148,14 +148,15 @@
 "Source" = "https://github.com/codesapienbe/aij-webcam"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
 aijrun = "webcam:main"
 aijnews = "news:main"
+aijintro = "intro:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-webcam-1.1.3/src/aij_webcam.egg-info/PKG-INFO` & `aij-webcam-1.1.4/src/aij_webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij-webcam
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI Journalist GUI Application
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-webcam-1.1.3/src/news/__init__.py` & `aij-webcam-1.1.4/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/src/news/core.py` & `aij-webcam-1.1.4/src/news/core.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/src/news/publisher.py` & `aij-webcam-1.1.4/src/news/publisher.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/src/news/subscriber.py` & `aij-webcam-1.1.4/src/news/subscriber.py`

 * *Files identical despite different names*

### Comparing `aij-webcam-1.1.3/src/webcam/__init__.py` & `aij-webcam-1.1.4/src/webcam/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
             logo_resized = cv2.resize(logo, (100, 100), interpolation=cv2.INTER_AREA)
             # get the height and width of the logo
             logo_height, logo_width, _ = logo_resized.shape
             # get the height and width of the main image
             image_height, image_width, _ = image.shape
             # calculate the x and y coordinates of the logo
             x = image_width - logo_width - 10
-            y = image_height - logo_height - 10
+            y = image_height - logo_height - 30
             # draw the logo on the main image
             image[y:y + logo_height, x:x + logo_width] = logo_resized
         else:
             draw_text(image, 0, 20, 'AIJ', color)
 
         cv2.imshow('AI News', image)
```

