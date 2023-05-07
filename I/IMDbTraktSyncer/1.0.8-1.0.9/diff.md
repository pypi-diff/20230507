# Comparing `tmp/IMDbTraktSyncer-1.0.8.tar.gz` & `tmp/IMDbTraktSyncer-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.0.8.tar", last modified: Sat May  6 04:57:14 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.0.9.tar", last modified: Sun May  7 03:06:22 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.0.8.tar` & `IMDbTraktSyncer-1.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.858586 IMDbTraktSyncer-1.0.8/
-drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.838585 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0     7796 2023-05-06 04:53:07.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0      642 2023-05-05 01:55:31.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2038 2023-05-06 03:24:18.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1408 2023-05-06 03:16:22.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-06 04:33:00.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-06 04:57:14.856089 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     5945 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-06 04:57:14.000000 IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     5945 2023-05-06 04:57:14.858087 IMDbTraktSyncer-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5335 2023-05-06 04:29:30.000000 IMDbTraktSyncer-1.0.8/README.md
--rw-rw-rw-   0        0        0       42 2023-05-06 04:57:14.859085 IMDbTraktSyncer-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1280 2023-05-06 04:56:52.000000 IMDbTraktSyncer-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:06:22.619098 IMDbTraktSyncer-1.0.9/
+drwxrwxrwx   0        0        0        0 2023-05-07 03:06:22.598310 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0     7944 2023-05-07 03:02:56.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-06 06:40:54.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0      642 2023-05-06 06:40:54.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2038 2023-05-06 06:40:54.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1408 2023-05-06 06:40:54.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-06 06:40:54.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-07 03:06:22.616611 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     5959 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-07 03:06:22.000000 IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5959 2023-05-07 03:06:22.618599 IMDbTraktSyncer-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5342 2023-05-07 03:05:58.000000 IMDbTraktSyncer-1.0.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-07 03:06:22.619606 IMDbTraktSyncer-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-07 03:05:11.000000 IMDbTraktSyncer-1.0.9/setup.py
```

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,17 @@
     directory = os.path.dirname(os.path.realpath(__file__))
     
     #Start web driver
     print('Starting webdriver')
     options = Options()
     options.add_argument("--headless=new")
     options.add_argument('--user-agent=Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.3')
-    options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False})
+    options.add_experimental_option("prefs", {"download.default_directory": directory, "download.directory_upgrade": True, "download.prompt_for_download": False, "credentials_enable_service": False, "profile.password_manager_enabled": False})
     options.add_argument("--disable-save-password-bubble")
+    options.add_argument("--disable-autofill-for-password-fields")
     options.add_argument('--disable-notifications')
     options.add_argument("--disable-third-party-cookies")
     options.add_argument("--disable-dev-shm-usage")
     options.add_argument("--no-sandbox")
     options.add_argument("--disable-extensions")
     options.add_experimental_option("excludeSwitches", ["enable-automation"])
     options.add_experimental_option("useAutomationExtension", False)
```

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/checkChromedriver.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.0.9/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.8
-Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
+Version: 1.0.9
+Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.0.8/LICENSE` & `IMDbTraktSyncer-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.0.8/PKG-INFO` & `IMDbTraktSyncer-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.0.8
-Summary: This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
+Version: 1.0.9
+Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.0.8/README.md` & `IMDbTraktSyncer-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # IMDb-Trakt-Syncer
-This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
+This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb. Currently season and episode ratings are not supported. Ratings already set will not be overwritten. This script should work on an OS where python and chromedriver are supported (Windows, Linux, Mac, and ChromeOS).
 ## Install Instructions:
 1. Install [Python](https://www.python.org/downloads/) and [Google Chrome](https://www.google.com/chrome/). _If these are already installed on your machine you can ignore this step. Please note this script does not effect Chrome in anyway it is simply required in order for chromedriver to work._
 2. Run `python -m pip install IMDbTraktSyncer` in command line.
 3. Login to [Trakt](https://trakt.tv/oauth/applications) and create a new API application. We will name it `IMDbTraktSyncer`. In the Redirect uri field enter `urn:ietf:wg:oauth:2.0:oob` then Save. 
 4. Run the script by calling `IMDbTraktSyncer` in command line. 
 5. Follow the prompts on first run. It will ask you to fill in your Trakt client id and client secret from step 3. It will also ask you to enter your IMDb username and password. Please note that these details are saved insecurely as credentials.txt in the same folder as the script. Recommended to change your password to something unique beforehand.
 6. Done, setup complete. The script will continue to run and sync your ratings. This may take some time, you can follow its progress in the command line.
```

### Comparing `IMDbTraktSyncer-1.0.8/setup.py` & `IMDbTraktSyncer-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.0.8'
-DESCRIPTION = 'This script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
+VERSION = '1.0.9'
+DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
```

