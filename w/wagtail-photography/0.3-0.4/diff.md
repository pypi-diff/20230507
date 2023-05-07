# Comparing `tmp/wagtail-photography-0.3.tar.gz` & `tmp/wagtail-photography-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-photography-0.3.tar", last modified: Sun May  7 17:03:38 2023, max compression
+gzip compressed data, was "wagtail-photography-0.4.tar", last modified: Sun May  7 18:00:36 2023, max compression
```

## Comparing `wagtail-photography-0.3.tar` & `wagtail-photography-0.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/
--rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-0.3/LICENSE
--rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-0.3/MANIFEST.in
--rw-rw-r--   0 ave       (1000) ave       (1000)     2247 2023-05-07 17:03:38.183061 wagtail-photography-0.3/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1331 2023-05-07 16:45:56.000000 wagtail-photography-0.3/README.md
--rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-0.3/pyproject.toml
--rw-rw-r--   0 ave       (1000) ave       (1000)      967 2023-05-07 17:03:38.183061 wagtail-photography-0.3/setup.cfg
--rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-0.3/setup.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.3/wagtail_photography/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-0.3/wagtail_photography/apps.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/blocks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-0.3/wagtail_photography/forms.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/migrations/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/migrations/0001_initial.py
--rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.3/wagtail_photography/migrations/__init__.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     5147 2023-04-30 05:36:56.000000 wagtail-photography-0.3/wagtail_photography/models.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/static/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-0.3/wagtail_photography/static/app.js
--rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-0.3/wagtail_photography/static/photo_gallery.css
--rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-0.3/wagtail_photography/static/photo_gallery_admin.css
--rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-0.3/wagtail_photography/static/photo_gallery_admin.js
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/templates/
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/templates/blocks/
--rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/templates/blocks/photo_gallery.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/templates/includes/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/templates/includes/photo_swipe.html
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/
--rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/album_detail.html
--rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/extra_css.html
--rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/extra_js.html
--rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-0.3/wagtail_photography/tests.py
--rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/views.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/wagtail_hooks.py
--rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-0.3/wagtail_photography/widgets.py
-drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 17:03:38.183061 wagtail-photography-0.3/wagtail_photography.egg-info/
--rw-rw-r--   0 ave       (1000) ave       (1000)     2247 2023-05-07 17:03:38.000000 wagtail-photography-0.3/wagtail_photography.egg-info/PKG-INFO
--rw-rw-r--   0 ave       (1000) ave       (1000)     1131 2023-05-07 17:03:38.000000 wagtail-photography-0.3/wagtail_photography.egg-info/SOURCES.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 17:03:38.000000 wagtail-photography-0.3/wagtail_photography.egg-info/dependency_links.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       39 2023-05-07 17:03:38.000000 wagtail-photography-0.3/wagtail_photography.egg-info/requires.txt
--rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 17:03:38.000000 wagtail-photography-0.3/wagtail_photography.egg-info/top_level.txt
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11356 2023-04-24 20:19:57.000000 wagtail-photography-0.4/LICENSE
+-rw-rw-r--   0 ave       (1000) ave       (1000)      156 2023-04-24 20:32:56.000000 wagtail-photography-0.4/MANIFEST.in
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2291 2023-05-07 18:00:36.914357 wagtail-photography-0.4/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1375 2023-05-07 17:24:51.000000 wagtail-photography-0.4/README.md
+-rw-rw-r--   0 ave       (1000) ave       (1000)       88 2023-04-24 20:20:58.000000 wagtail-photography-0.4/pyproject.toml
+-rw-rw-r--   0 ave       (1000) ave       (1000)      983 2023-05-07 18:00:36.914357 wagtail-photography-0.4/setup.cfg
+-rw-rw-r--   0 ave       (1000) ave       (1000)       38 2023-04-26 01:55:13.000000 wagtail-photography-0.4/setup.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      169 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/apps.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1372 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/blocks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1276 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/forms.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/migrations/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2623 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/migrations/0001_initial.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)        0 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/migrations/__init__.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     5147 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/models.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/static/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1234 2023-04-26 02:00:09.000000 wagtail-photography-0.4/wagtail_photography/static/app.js
+-rw-rw-r--   0 ave       (1000) ave       (1000)      384 2023-04-26 02:00:09.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)     3119 2023-04-26 02:01:14.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.css
+-rw-rw-r--   0 ave       (1000) ave       (1000)    11256 2023-04-26 02:01:14.000000 wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.js
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.910357 wagtail-photography-0.4/wagtail_photography/templates/
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/blocks/
+-rw-rw-r--   0 ave       (1000) ave       (1000)      980 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/blocks/photo_gallery.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/includes/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2526 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/includes/photo_swipe.html
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1378 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/album_detail.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)      541 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_css.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1106 2023-04-30 05:36:56.000000 wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_js.html
+-rw-rw-r--   0 ave       (1000) ave       (1000)       60 2023-04-24 19:22:23.000000 wagtail-photography-0.4/wagtail_photography/tests.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)      373 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/views.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1221 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/wagtail_hooks.py
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1030 2023-04-29 01:28:30.000000 wagtail-photography-0.4/wagtail_photography/widgets.py
+drwxrwxr-x   0 ave       (1000) ave       (1000)        0 2023-05-07 18:00:36.914357 wagtail-photography-0.4/wagtail_photography.egg-info/
+-rw-rw-r--   0 ave       (1000) ave       (1000)     2291 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/PKG-INFO
+-rw-rw-r--   0 ave       (1000) ave       (1000)     1131 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/SOURCES.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)        1 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/dependency_links.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       54 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/requires.txt
+-rw-rw-r--   0 ave       (1000) ave       (1000)       20 2023-05-07 18:00:36.000000 wagtail-photography-0.4/wagtail_photography.egg-info/top_level.txt
```

### Comparing `wagtail-photography-0.3/LICENSE` & `wagtail-photography-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/PKG-INFO` & `wagtail-photography-0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.3
+Version: 0.4
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
@@ -38,40 +38,38 @@
 Quick start
 -----------
 
 1. Install library
 
    ```pip install wagtail-photography```
 
-
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
       ...
-      "generic_chooser"
+      "generic_chooser",
       "wagtail_photography",
    ]
    ```
 
-
 3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
 
-```python
-from wagtail.images.views.serve import ServeView
-
-urlpatterns = [
-    ...
-
-    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
-
-    ...
-
-    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
-    re_path(r'', include(wagtail_urls)),
-]
-```
-
-3. Run ``python manage.py migrate`` to create the wagtail_photography models.
+   ```python
+   from wagtail.images.views.serve import ServeView
+   
+   urlpatterns = [
+       ...
+   
+       re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+   
+       ...
+   
+       # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+       re_path(r'', include(wagtail_urls)),
+   ]
+   ```
+   
+4. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
-4. Start the development server and visit http://127.0.0.1:8000/admin/
+5. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.3/README.md` & `wagtail-photography-0.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -14,40 +14,38 @@
 Quick start
 -----------
 
 1. Install library
 
    ```pip install wagtail-photography```
 
-
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
       ...
-      "generic_chooser"
+      "generic_chooser",
       "wagtail_photography",
    ]
    ```
 
-
 3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
 
-```python
-from wagtail.images.views.serve import ServeView
-
-urlpatterns = [
-    ...
-
-    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
-
-    ...
-
-    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
-    re_path(r'', include(wagtail_urls)),
-]
-```
-
-3. Run ``python manage.py migrate`` to create the wagtail_photography models.
+   ```python
+   from wagtail.images.views.serve import ServeView
+   
+   urlpatterns = [
+       ...
+   
+       re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+   
+       ...
+   
+       # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+       re_path(r'', include(wagtail_urls)),
+   ]
+   ```
+   
+4. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
-4. Start the development server and visit http://127.0.0.1:8000/admin/
+5. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.3/setup.cfg` & `wagtail-photography-0.4/setup.cfg`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wagtail-photography
-version = 0.3
+version = 0.4
 description = A Wagtail app to display photographs
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/TechnoConserve/wagtail-photography
 author = Avery Uslaner
 author_email = uslaner.avery@gmail.com
 license = Apache License 2.0
@@ -23,14 +23,15 @@
 	Topic :: Internet :: WWW/HTTP :: Dynamic Content
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
-	wagtail
+	django<4.2
+	wagtail<5.0
 	wagtail-generic-chooser>=0.2.1
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wagtail-photography-0.3/wagtail_photography/blocks.py` & `wagtail-photography-0.4/wagtail_photography/blocks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/forms.py` & `wagtail-photography-0.4/wagtail_photography/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/migrations/0001_initial.py` & `wagtail-photography-0.4/wagtail_photography/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/models.py` & `wagtail-photography-0.4/wagtail_photography/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/static/app.js` & `wagtail-photography-0.4/wagtail_photography/static/app.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/static/photo_gallery_admin.css` & `wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.css`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/static/photo_gallery_admin.js` & `wagtail-photography-0.4/wagtail_photography/static/photo_gallery_admin.js`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/templates/blocks/photo_gallery.html` & `wagtail-photography-0.4/wagtail_photography/templates/blocks/photo_gallery.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/templates/includes/photo_swipe.html` & `wagtail-photography-0.4/wagtail_photography/templates/includes/photo_swipe.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/album_detail.html` & `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/album_detail.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/extra_css.html` & `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_css.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/templates/wagtail_photography/extra_js.html` & `wagtail-photography-0.4/wagtail_photography/templates/wagtail_photography/extra_js.html`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/wagtail_hooks.py` & `wagtail-photography-0.4/wagtail_photography/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography/widgets.py` & `wagtail-photography-0.4/wagtail_photography/widgets.py`

 * *Files identical despite different names*

### Comparing `wagtail-photography-0.3/wagtail_photography.egg-info/PKG-INFO` & `wagtail-photography-0.4/wagtail_photography.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-photography
-Version: 0.3
+Version: 0.4
 Summary: A Wagtail app to display photographs
 Home-page: https://github.com/TechnoConserve/wagtail-photography
 Author: Avery Uslaner
 Author-email: uslaner.avery@gmail.com
 License: Apache License 2.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Wagtail
@@ -38,40 +38,38 @@
 Quick start
 -----------
 
 1. Install library
 
    ```pip install wagtail-photography```
 
-
 2. Add "wagtail_photography" and wagtail-generic-chooser to your INSTALLED_APPS setting like this:
 
    ```python
    INSTALLED_APPS = [
       ...
-      "generic_chooser"
+      "generic_chooser",
       "wagtail_photography",
    ]
    ```
 
-
 3. [Setup Wagtail to dynamically serve image urls](https://docs.wagtail.org/en/stable/advanced_topics/images/image_serve_view.html#setup):
 
-```python
-from wagtail.images.views.serve import ServeView
-
-urlpatterns = [
-    ...
-
-    re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
-
-    ...
-
-    # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
-    re_path(r'', include(wagtail_urls)),
-]
-```
-
-3. Run ``python manage.py migrate`` to create the wagtail_photography models.
+   ```python
+   from wagtail.images.views.serve import ServeView
+   
+   urlpatterns = [
+       ...
+   
+       re_path(r'^images/([^/]*)/(\d*)/([^/]*)/[^/]*$', ServeView.as_view(), name='wagtailimages_serve'),
+   
+       ...
+   
+       # Ensure that the wagtailimages_serve line appears above the default Wagtail page serving route
+       re_path(r'', include(wagtail_urls)),
+   ]
+   ```
+   
+4. Run ``python manage.py migrate`` to create the wagtail_photography models.
 
-4. Start the development server and visit http://127.0.0.1:8000/admin/
+5. Start the development server and visit http://127.0.0.1:8000/admin/
    to create an album.
```

### Comparing `wagtail-photography-0.3/wagtail_photography.egg-info/SOURCES.txt` & `wagtail-photography-0.4/wagtail_photography.egg-info/SOURCES.txt`

 * *Files identical despite different names*

