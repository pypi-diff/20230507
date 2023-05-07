# Comparing `tmp/gsearch-nyaa-0.1.4.tar.gz` & `tmp/gsearch-nyaa-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gsearch-nyaa-0.1.4.tar", last modified: Mon May  1 20:39:59 2023, max compression
+gzip compressed data, was "gsearch-nyaa-0.1.5.tar", last modified: Sun May  7 04:53:00 2023, max compression
```

## Comparing `gsearch-nyaa-0.1.4.tar` & `gsearch-nyaa-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.026022 gsearch-nyaa-0.1.4/
--rw-rw-rw-   0        0        0     2427 2023-05-01 20:39:59.026022 gsearch-nyaa-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2181 2023-05-01 20:39:45.000000 gsearch-nyaa-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.003642 gsearch-nyaa-0.1.4/gsearch/
--rw-rw-rw-   0        0        0     1634 2023-05-01 20:06:24.000000 gsearch-nyaa-0.1.4/gsearch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 20:39:59.024855 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/
--rw-rw-rw-   0        0        0     2427 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 20:39:58.000000 gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 20:39:59.027155 gsearch-nyaa-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      833 2023-05-01 20:39:52.000000 gsearch-nyaa-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:53:00.540354 gsearch-nyaa-0.1.5/
+-rw-rw-rw-   0        0        0     2427 2023-05-07 04:53:00.540354 gsearch-nyaa-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2181 2023-05-01 20:39:45.000000 gsearch-nyaa-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 04:53:00.503355 gsearch-nyaa-0.1.5/gsearch/
+-rw-rw-rw-   0        0        0     1638 2023-05-07 04:52:32.000000 gsearch-nyaa-0.1.5/gsearch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-07 04:53:00.539354 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/
+-rw-rw-rw-   0        0        0     2427 2023-05-07 04:53:00.000000 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-07 04:53:00.000000 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 04:53:00.000000 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-07 04:53:00.000000 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-07 04:53:00.000000 gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-07 04:53:00.542354 gsearch-nyaa-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      833 2023-05-07 04:52:39.000000 gsearch-nyaa-0.1.5/setup.py
```

### Comparing `gsearch-nyaa-0.1.4/PKG-INFO` & `gsearch-nyaa-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
```

### Comparing `gsearch-nyaa-0.1.4/README.md` & `gsearch-nyaa-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `gsearch-nyaa-0.1.4/gsearch/__init__.py` & `gsearch-nyaa-0.1.5/gsearch/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         for result in result_block:
             with suppress(Exception):
                 url = result.css_first("a[href]").attrs["href"]
                 title = result.css_first("h3").text()
                 description_box = result.css_first(
                     'div[style="-webkit-line-clamp:2"]'
                 ).text()
-            yield GoogleSearchResult(url, title, description_box)
+                yield GoogleSearchResult(url, title, description_box)
 
     def search(self, query: str) -> List[GoogleSearchResult]:
         url = f"{self.BASE_URL}{query}"
         self.page.goto(url)
         content = self.page.content()
         return self.get_googlesearch_result(content)
```

### Comparing `gsearch-nyaa-0.1.4/gsearch_nyaa.egg-info/PKG-INFO` & `gsearch-nyaa-0.1.5/gsearch_nyaa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gsearch-nyaa
-Version: 0.1.4
+Version: 0.1.5
 Summary: A Python Package for Automated Google Searches and Scraping of Search Results
 Author: Praveen Senpai
 Author-email: pvnt20@gmail.com
 Description-Content-Type: text/markdown
 
 # GSearch - A Python Package for Automated Google Searches and Scraping of Search Results
```

### Comparing `gsearch-nyaa-0.1.4/setup.py` & `gsearch-nyaa-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     def run(self):
         install.run(self)
         subprocess.call(["playwright", "install", "chromium"])
 
 
 setup(
     name="gsearch-nyaa",
-    version="0.1.4",
+    version="0.1.5",
     author="Praveen Senpai",
     author_email="pvnt20@gmail.com",
     description="A Python Package for Automated Google Searches and Scraping of Search Results",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
```

