# Comparing `tmp/szurubooru_toolkit-0.7.7.tar.gz` & `tmp/szurubooru_toolkit-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "szurubooru_toolkit-0.7.7.tar", max compression
+gzip compressed data, was "szurubooru_toolkit-0.8.0.tar", max compression
```

## Comparing `szurubooru_toolkit-0.7.7.tar` & `szurubooru_toolkit-0.8.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
--rw-r--r--   0        0        0    35149 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/LICENSE
--rw-r--r--   0        0        0    20785 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/README.md
--rw-r--r--   0        0        0     2375 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     1363 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/__init__.py
--rw-r--r--   0        0        0     8413 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/config.py
--rw-r--r--   0        0        0     3973 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/danbooru.py
--rw-r--r--   0        0        0     3716 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/deepbooru.py
--rw-r--r--   0        0        0     1604 2023-03-15 19:34:09.107375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/gelbooru.py
--rw-r--r--   0        0        0     9364 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/saucenao.py
--rw-r--r--   0        0        0      358 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/__init__.py
--rw-r--r--   0        0        0    11693 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/auto_tagger.py
--rw-r--r--   0        0        0     3212 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/create_tags.py
--rw-r--r--   0        0        0     2622 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/delete_posts.py
--rw-r--r--   0        0        0     6110 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/import_from_booru.py
--rw-r--r--   0        0        0     3677 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/import_from_twitter.py
--rw-r--r--   0        0        0     3087 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/reset_posts.py
--rw-r--r--   0        0        0     4446 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/tag_posts.py
--rw-r--r--   0        0        0    10356 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/upload_media.py
--rw-r--r--   0        0        0    10195 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/szurubooru.py
--rw-r--r--   0        0        0     7036 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/twitter.py
--rw-r--r--   0        0        0    13441 2023-03-15 19:34:09.111375 szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/utils.py
--rw-r--r--   0        0        0    22325 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/LICENSE
+-rw-r--r--   0        0        0    22797 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/README.md
+-rw-r--r--   0        0        0     2466 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1363 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/__init__.py
+-rw-r--r--   0        0        0     8773 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/config.py
+-rw-r--r--   0        0        0     3870 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/danbooru.py
+-rw-r--r--   0        0        0     3716 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/deepbooru.py
+-rw-r--r--   0        0        0     1604 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/gelbooru.py
+-rw-r--r--   0        0        0     9364 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/saucenao.py
+-rw-r--r--   0        0        0      405 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/__init__.py
+-rw-r--r--   0        0        0    12349 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/auto_tagger.py
+-rw-r--r--   0        0        0     3459 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/create_tags.py
+-rw-r--r--   0        0        0     2841 2023-05-07 10:51:26.526708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/delete_posts.py
+-rw-r--r--   0        0        0     6461 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_booru.py
+-rw-r--r--   0        0        0     4044 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_twitter.py
+-rw-r--r--   0        0        0     6013 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_url.py
+-rw-r--r--   0        0        0     3314 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/reset_posts.py
+-rw-r--r--   0        0        0     4713 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/tag_posts.py
+-rw-r--r--   0        0        0    10615 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/upload_media.py
+-rw-r--r--   0        0        0    10195 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/szurubooru.py
+-rw-r--r--   0        0        0     7036 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/twitter.py
+-rw-r--r--   0        0        0    13441 2023-05-07 10:51:26.530708 szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/utils.py
+-rw-r--r--   0        0        0    24381 1970-01-01 00:00:00.000000 szurubooru_toolkit-0.8.0/PKG-INFO
```

### Comparing `szurubooru_toolkit-0.7.7/LICENSE` & `szurubooru_toolkit-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/README.md` & `szurubooru_toolkit-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -105,14 +105,16 @@
 | `upload_media` | `convert_quality` | Only images above this threshold will be converted to jpg if `convert_to_jpg` is True. | `"3MB\|500KB"` |
 | `upload_media` | `shrink` | Set to true to shrink images to shrink_dimensions based on shrink_threshold below. Images might slip through identical post check. | `false` |
 | `upload_media` | `shrink_threshold` | Images which total pixel size exceeds this treshold will be resized to `shrink_size`. E.g. 2000x3000 results in 6000000. | `"6000000"` |
 | `upload_media` | `shrink_dimensions` | Set the max value for width/height. Keeps aspect ratio. E.g. 2000x4000 results in 700x1400, 4000x2000 in 1400x700 (with `"1400x1400"`). | `"2500x2500"` |
 | `upload_media` | `default_safety` | # Set the default safety in case neither SauceNAO, nor Deepbooru could determine it | `safe` |
 | `import_from_booru` | `deepbooru_enabled` | Apply Deepbooru tagging additionally besides fetched tags from Booru | `false` |
 | `import_from_booru` | `hide_progress` | Set this to true to hide the progress bar | `false` |
+| `import_from_url` | `tmp_path` | Path to directory where temporary downloads from gallery-dl script will be saved | `false` |
+| `import_from_url` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `import_from_twitter` | `saucenao_enabled` | Tag posts with SauceNAO | `false` |
 | `import_from_twitter` | `deepbooru_enabled` | Tag posts with Deepbooru | `false` |
 | `import_from_twitter` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `create_tags` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `delete_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `reset_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `tag_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
@@ -133,14 +135,15 @@
 Following scripts are currently available:
 
 * `auto-tagger`: Batch tagging of posts with SauceNAO and Deepbooru
 * `create-tags`: Batch creation of tags with their categories
 * `delete-posts`: Batch delete of posts
 * `import-from-booru`: Batch importing of posts with their tags from various Boorus
 * `import-from-twitter`: Batch importing of Twitter favorites
+* `import-from-url`: Batch importing of URLs based on [gallery-dl](https://github.com/mikf/gallery-dl)
 * `reset-posts`: Batch resetting of posts (remove tags and sources)
 * `upload-media`: Batch upload of media files from local source folder
 * `tag-posts`: Manual batch tagging
 
 See the descriptions below on how to use them.
 
 If you installed this package with pip, you can generally just call the scripts from your shell (if your $PATH is set correctly).
@@ -223,14 +226,59 @@
 * `import-from-booru danbooru "tag1 tagN"`
 * `import-from-booru yandere "tag1 tag2 -tagN"`
 * `import-from-booru all "tag1 -tagN"`
 
 Note that if you specify `all` to download from all Boorus, you are limited to two tags because free Danbooru accounts are limited to two tags per query.
 If you have a Gold/Platinum account, set your credentials in `config.toml`. Note that it's currently untested if the script will work with upgraded accounts.
 
+### :link:	import-from-url
+This scripts imports posts with their tags from the URL passed to this script.
+In the background, it simply calls the [gallery-dl](https://github.com/mikf/gallery-dl) script and parses its output.
+Alternatively, an input file with multiple URLs can be specified.
+
+In the `config.toml` file, you have to specify a directory where posts will be temporarily saved to.
+Since this script is using the `upload-media` script to upload the post, following settings apply from the `upload-media` section:
+* max_similarity
+* convert_to_jpg
+* convert_threshold
+* shrink
+* shrink_threshold
+* shrink_dimensions
+
+:information_source:️ **Following Boorus are currently supported:**
+* Gelbooru
+* Danbooru
+* Sankaku
+* Konachan
+* Yandere
+
+Credentials in your `config.toml` file will be passed to the gallery-dl script if you use a single input URL to this script.
+
+__Usage__
+```
+usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [url ...]
+
+This script downloads and tags posts from various Boorus based on your input query.
+
+positional arguments:
+  url                   The URL for the posts you want to download and tag
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --range RANGE         Index range(s) specifying which files to download. These can be either a constant value, range, or slice (e.g. '5', '8-20', or '1:24:3')
+  --input-file INPUT_FILE
+                        Download URLs found in FILE.
+
+```
+
+__Examples__
+* `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
+* `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
+* `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+
 ### :dove: import-from-twitter
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `szurubooru_toolkit-0.7.7/pyproject.toml` & `szurubooru_toolkit-0.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -34,27 +34,28 @@
 check_untyped_defs = true
 disallow_incomplete_defs = true
 disallow_untyped_defs = true
 
 
 [tool.poetry]
 name = "szurubooru-toolkit"
-version = "0.7.7"
+version = "0.8.0"
 description = "Python package and script collection to manage szurubooru."
 authors = ["reluce <reluce@fkosquad.moe>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 repository = "https://github.com/reluce/szurubooru-toolkit"
 documentation = "https://github.com/reluce/szurubooru-toolkit"
 keywords = ["szurubooru", "szuru", "booru", "saucenao", "deepbooru"]
 
 [tool.poetry.scripts]
 auto-tagger = 'szurubooru_toolkit.scripts.auto_tagger:main'
 upload-media = 'szurubooru_toolkit.scripts.upload_media:main'
 create-tags = 'szurubooru_toolkit.scripts.create_tags:main'
+import-from-url = 'szurubooru_toolkit.scripts.import_from_url:main'
 import-from-booru = 'szurubooru_toolkit.scripts.import_from_booru:main'
 import-from-twitter = 'szurubooru_toolkit.scripts.import_from_twitter:main'
 tag-posts = 'szurubooru_toolkit.scripts.tag_posts:main'
 delete-posts = 'szurubooru_toolkit.scripts.delete_posts:main'
 reset-posts = 'szurubooru_toolkit.scripts.reset_posts:main'
 
 [tool.poetry.dependencies]
@@ -73,14 +74,15 @@
 tomlkit = "^0.10.0"
 syncer = "^1.3.0"
 loguru = "^0.6.0"
 pathvalidate = "^2.5.0"
 validators = "^0.18.2"
 lxml = "^4.8.0"
 tweepy = "^4.10.0"
+gallery-dl = "^1.25.1"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 flake8 = "^4.0.1"
 interrogate = "^1.5.0"
 isort = "^5.10.1"
 mkdocs = "^1.2.3"
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/__init__.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/config.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,18 +18,18 @@
             with open('config.toml') as f:
                 content = f.read()
 
                 try:
                     self.config = parse(content)
                 except Exception as e:
                     logger.critical(e)
-                    exit()
+                    exit(1)
         except FileNotFoundError as e:
             logger.critical(e)
-            exit()
+            exit(1)
 
         for key, value in self.config.items():
             setattr(self, key, value)
 
         self.check_attr_set()
         self.validate_path()
         self.validate_url()
@@ -74,144 +74,152 @@
                 'shrink',
                 'shrink_threshold',
                 'shrink_dimensions',
                 'default_safety',
             ],
             'import_from_booru': ['deepbooru_enabled', 'hide_progress'],
             'import_from_twitter': ['saucenao_enabled', 'deepbooru_enabled', 'hide_progress'],
+            'import_from_url': ['hide_progress', 'tmp_path'],
             'tag_posts': ['hide_progress'],
             'delete_posts': ['hide_progress'],
             'reset_posts': ['hide_progress'],
             'create_tags': ['hide_progress'],
             'logging': ['log_enabled', 'log_file', 'log_level', 'log_colorized'],
             'danbooru': ['user', 'api_key'],
             'gelbooru': ['user', 'api_key'],
             'konachan': ['user', 'password'],
             'yandere': ['user', 'password'],
+            'sankaku': ['user', 'password'],
             'pixiv': ['user', 'password', 'token'],
             'twitter': ['user_id', 'consumer_key', 'consumer_secret', 'access_token', 'access_token_secret'],
         }
 
         for section in req_opts:
             try:
                 getattr(self, section)
             except AttributeError:
                 logger.critical(f'The section "{section}" is not defined config.toml!')
-                exit()
+                exit(1)
 
         for section, options in req_opts.items():
             for option in options:
                 if option not in getattr(self, section):
                     logger.critical(
                         f'The option "{option}" in the "{section}" section was not set in config.toml! '
                         'Check the README for additional information.',
                     )
-                    exit()
+                    exit(1)
 
     def validate_path(self) -> None:
         """Check if the directories in config.toml exist.
 
         Paths have to exist, even if one is not being actively used.
         """
 
         if not Path(self.upload_media['src_path']).is_dir():
             logger.critical(f'The src_path "{self.upload_media["src_path"]}" specified in config.toml does not exist!')
-            exit()
+            exit(1)
+
+        if not Path(self.import_from_url['tmp_path']).is_dir():
+            logger.critical(
+                f'The tmp_path "{self.import_from_url["tmp_path"]}" specified in config.toml does not exist!',
+            )
+            exit(1)
 
         if not Path(self.logging['log_file']).parent.is_dir():
             logger.critical(
                 f'The log_file\'s parent directory "{Path(self.logging["log_file"]).parent}" '
                 'specified in config.toml does not exist!',
             )
-            exit()
+            exit(1)
 
     def validate_url(self) -> None:
         """Sanitize the szurubooru url in config.toml.
 
         Make sure that the URL itself is valid, of scheme HTTP/s and remove trailing '/' char.
         """
 
         self.szurubooru['url'] = self.szurubooru['url'].strip()
         result = validators.url(self.szurubooru['url'])
 
         if isinstance(result, ValidationFailure):
             logger.critical(f'Your szurubooru URL "{self.szurubooru["url"]}" in config.toml is not valid!')
-            exit()
+            exit(1)
 
         parsed_url = urllib.parse.urlsplit(self.szurubooru['url'])
 
         api_scheme = parsed_url.scheme
         if api_scheme not in ('http', 'https'):
             logger.critical('API URL must be of HTTP or HTTPS scheme!')
-            exit()
+            exit(1)
 
         if parsed_url.path.startswith('/'):
             self.szurubooru['url'] = self.szurubooru['url'].rstrip('/')
 
     def validate_deepbooru(self) -> None:
         """Check if deepbooru_model in config.toml is an existing file."""
 
         if not Path(self.auto_tagger['deepbooru_model']).exists():
             logger.critical(
                 f'Your Deepbooru model "{self.auto_tagger["deepbooru_model"]}" in config.toml does not exist!',
             )
-            exit()
+            exit(1)
 
     def validate_convert_attrs(self) -> None:
         """Convert the threshold from a human readable to a machine readable size."""
 
         human_readable = self.upload_media['convert_threshold']
 
         if not any(x in human_readable for x in ['KB', 'MB']):
             logger.critical(
                 f'Your convert_threshold "{self.upload_media["convert_threshold"]}" in config.toml is not valid!',
             )
-            exit()
+            exit(1)
 
         if 'KB' in human_readable:
             self.upload_media['convert_threshold'] = float(human_readable.replace('KB', '')) * 1000
         elif 'MB' in human_readable:
             self.upload_media['convert_threshold'] = float(human_readable.replace('MB', '')) * 1000000
 
         if not self.upload_media['convert_quality'].isnumeric():
             logger.critical(
                 f'Your convert_quality "{self.upload_media["convert_quality"]}" in config.toml \
                     is not a numeric value!',
             )
-            exit()
+            exit(1)
         else:
             self.upload_media['convert_quality'] = int(self.upload_media['convert_quality'])
 
         if self.upload_media['convert_quality'] > 95:
             logger.critical(
                 f'Your convert_quality value "{self.upload_media["convert_quality"]}" in config.toml \
                     is higher than the max value of 95!',
             )
-            exit()
+            exit(1)
 
     def validate_shrink_attrs(self) -> None:
         """Validate that the shink dimensions matches reg exp."""
 
         if not re.match(r'\d+x\d+', self.upload_media['shrink_dimensions']):
             logger.critical(
                 f'Your shrink_dimensions "{self.upload_media["shrink_dimensions"]}" in config.toml are not valid!',
             )
-            exit()
+            exit(1)
         else:
             dimensions = re.search(r'(\d+)x(\d+)', self.upload_media['shrink_dimensions'])
             max_width = int(dimensions.group(1))
             max_height = int(dimensions.group(2))
             self.upload_media['shrink_dimensions'] = (int(max_width), (max_height))
 
         if not self.upload_media['shrink_threshold'].isnumeric():
             logger.critical(
                 f'Your shrink_threshold "{self.upload_media["shrink_dimensions"]}" in config.toml \
                     is not a numeric value!',
             )
-            exit()
+            exit(1)
         else:
             self.upload_media['shrink_threshold'] = int(self.upload_media['shrink_threshold'])
 
     def validate_safety(self) -> None:
         """Check if default_safety in config.toml is set correctly."""
 
         if not self.upload_media['default_safety'] in ['safe', 'sketchy', 'unsafe']:
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/danbooru.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/danbooru.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,14 +76,18 @@
 
         Returns:
             list: A list with found tags.
         """
 
         tag_base_url = 'https://danbooru.donmai.us/tags.json'
 
+        session = requests.Session()
+        headers = {'User-Agent': 'Danbooru dummy agent'}
+        session.headers.update(headers)
+
         if limit > 1000:
             pages = limit // 1000
         else:
             pages = 1
 
         for page in range(1, pages + 1):
             tag_url = (
@@ -94,18 +98,14 @@
                 + query
                 + '&limit='
                 + str(limit)
                 + '&page='
                 + str(page)
             )
 
-            headers = {
-                'User-Agent': (
-                    'Mozilla/5.0 (Windows NT 10.0; Win64; x64)'
-                    'AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
-                ),
-            }
             try:
                 logger.info(f'Fetching tags from URL {tag_url}...')
-                yield requests.get(tag_url, timeout=30, headers=headers).json()
+                yield session.get(tag_url, timeout=30).json()
             except Exception as e:
                 logger.critical(f'Could not fetch tags: {e}')
+
+        session.close()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/deepbooru.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/deepbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/gelbooru.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/gelbooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/saucenao.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/saucenao.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/auto_tagger.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/auto_tagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -106,15 +106,15 @@
     # Get previously set sources and add new sources
     source = collect_sources(*source.splitlines(), *post.source.splitlines())
 
     if not limit_long == 0:
         # Sleep 35 seconds after short limit has been reached
         if limit_short == 0:
             print('')
-            logger.info('Short limit reached for SauceNAO, trying again in 35s...')
+            logger.debug('Short limit reached for SauceNAO, trying again in 35s...')
             sleep(35)
     else:
         limit_reached = True
         print('')
         logger.info('Your daily SauceNAO limit has been reached. Consider upgrading your account.')
 
     if tags:
@@ -155,170 +155,175 @@
     If called with no arguments, read from command line arguments.
 
     Args:
         post_id (str, optional): The `post_id` of the szurubooru post. Defaults to None.
         file_to_upload (bytes, optional): If set, will be uploaded to SauceNAO directly. Defaults to None.
     """
 
-    # If this script/function was called from the upload-media script,
-    # change output and behaviour of this script
-    from_upload_media = True if post_id else False
-
-    if not from_upload_media:
-        logger.info('Initializing script...')
-    else:
-        config.auto_tagger['hide_progress'] = True
-
-    if not config.auto_tagger['saucenao_enabled'] and not config.auto_tagger['deepbooru_enabled']:
-        logger.info('Nothing to do. Enable either SauceNAO or Deepbooru in your config.')
-        exit()
-
-    # If posts are being tagged directly from upload-media script
-    if not from_upload_media:
-        sankaku_url, query, add_tags, remove_tags = parse_args()
-    else:
-        sankaku_url = None
-        query = post_id
-        add_tags = None
-        remove_tags = None
-
-    if config.auto_tagger['saucenao_enabled']:
-        sauce = SauceNao(config)
-
-    if config.auto_tagger['deepbooru_enabled']:
-        from szurubooru_toolkit import Deepbooru
-
-        deepbooru = Deepbooru(config.auto_tagger['deepbooru_model'])
-
-    if not from_upload_media:
-        logger.info(f'Retrieving posts from {config.szurubooru["url"]} with query "{query}"...')
-
-    posts = szuru.get_posts(query)
-
     try:
-        total_posts = next(posts)
-    except StopIteration:
-        logger.info(f'Found no posts for your query: {query}')
-        exit()
-
-    if not from_upload_media:
-        logger.info(f'Found {total_posts} posts. Start tagging...')
-
-    if sankaku_url:
-        if query.isnumeric():
-            post = next(posts)
-            post.tags, post.safety = scrape_sankaku(sankaku_url)
-            post.source = sankaku_url
+        # If this script/function was called from the upload-media script,
+        # change output and behaviour of this script
+        from_upload_media = True if post_id else False
 
-            try:
-                szuru.update_post(post)
-                statistics(tagged=1)
-            except Exception as e:
-                statistics(untagged=1)
-                logger.error(f'Could not tag post with Sankaku: {e}')
+        if not from_upload_media:
+            logger.info('Initializing script...')
         else:
-            logger.critical('Can only tag a single post if you specify --sankaku_url.')
-    else:
-        for index, post in enumerate(
-            tqdm(
-                posts,
-                ncols=80,
-                position=0,
-                leave=False,
-                disable=config.auto_tagger['hide_progress'],
-                total=int(total_posts),
-            ),
-        ):
-            tags = []
-
-            # Download the file from szurubooru if its not already locally present.
-            # This might be the case if this function was called from upload_media.
-            if not file_to_upload:
-                if not config.szurubooru['public'] or config.auto_tagger['deepbooru_enabled']:
-                    image = download_media(post.content_url, post.md5)
-                    # Shrink files >2MB
-                    try:
-                        if len(image) > 2000000:
-                            image = shrink_img(image, resize=True, convert=True)
-                    except UnidentifiedImageError:
-                        logger.warning('Could not shrink image')
-                else:
-                    image = None  # Let SauceNAO download the image from public szurubooru URL
-            else:
-                image = file_to_upload
+            config.auto_tagger['hide_progress'] = True
 
-            if config.auto_tagger['saucenao_enabled']:
-                tags, post.source, post.safety, limit_reached = parse_saucenao_results(
-                    sauce,
-                    post,
-                    image,
-                )
-
-                if add_tags:
-                    post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags, add user tags
-                else:
-                    post.tags = list(set().union(post.tags, tags))  # Keep previous tags, add user tags
+        if not config.auto_tagger['saucenao_enabled'] and not config.auto_tagger['deepbooru_enabled']:
+            logger.info('Nothing to do. Enable either SauceNAO or Deepbooru in your config.')
+            exit()
+
+        # If posts are being tagged directly from upload-media script
+        if not from_upload_media:
+            sankaku_url, query, add_tags, remove_tags = parse_args()
+        else:
+            sankaku_url = None
+            query = post_id
+            add_tags = None
+            remove_tags = None
+
+        if config.auto_tagger['saucenao_enabled']:
+            sauce = SauceNao(config)
+
+        if config.auto_tagger['deepbooru_enabled']:
+            from szurubooru_toolkit import Deepbooru
+
+            deepbooru = Deepbooru(config.auto_tagger['deepbooru_model'])
+
+        if not from_upload_media:
+            logger.info(f'Retrieving posts from {config.szurubooru["url"]} with query "{query}"...')
+
+        posts = szuru.get_posts(query)
+
+        try:
+            total_posts = next(posts)
+        except StopIteration:
+            logger.info(f'Found no posts for your query: {query}')
+            exit()
+
+        if not from_upload_media:
+            logger.info(f'Found {total_posts} posts. Start tagging...')
+
+        if sankaku_url:
+            if query.isnumeric():
+                post = next(posts)
+                post.tags, post.safety = scrape_sankaku(sankaku_url)
+                post.source = sankaku_url
+
+                try:
+                    szuru.update_post(post)
+                    statistics(tagged=1)
+                except Exception as e:
+                    statistics(untagged=1)
+                    logger.error(f'Could not tag post with Sankaku: {e}')
             else:
-                limit_reached = False
-
-            if (not tags and config.auto_tagger['deepbooru_enabled']) or config.auto_tagger['deepbooru_forced']:
-                result = deepbooru.tag_image(
-                    image,
-                    config.auto_tagger['deepbooru_threshold'],
-                    config.auto_tagger['deepbooru_set_tag'],
-                )
-
-                if result is None:
-                    continue
-
-                tags, post.safety = result
-
-                if post.relations:
-                    set_tags_from_relations(post)
+                logger.critical('Can only tag a single post if you specify --sankaku_url.')
+        else:
+            for index, post in enumerate(
+                tqdm(
+                    posts,
+                    ncols=80,
+                    position=0,
+                    leave=False,
+                    disable=config.auto_tagger['hide_progress'],
+                    total=int(total_posts),
+                ),
+            ):
+                tags = []
+
+                # Download the file from szurubooru if its not already locally present.
+                # This might be the case if this function was called from upload_media.
+                if not file_to_upload:
+                    if not config.szurubooru['public'] or config.auto_tagger['deepbooru_enabled']:
+                        image = download_media(post.content_url, post.md5)
+                        # Shrink files >2MB
+                        try:
+                            if len(image) > 2000000:
+                                image = shrink_img(image, resize=True, convert=True)
+                        except UnidentifiedImageError:
+                            logger.warning('Could not shrink image')
+                    else:
+                        image = None  # Let SauceNAO download the image from public szurubooru URL
+                else:
+                    image = file_to_upload
 
-                if add_tags:
-                    post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags and add user tags
+                if config.auto_tagger['saucenao_enabled']:
+                    tags, post.source, post.safety, limit_reached = parse_saucenao_results(
+                        sauce,
+                        post,
+                        image,
+                    )
+
+                    if add_tags:
+                        post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags, add user tags
+                    else:
+                        post.tags = list(set().union(post.tags, tags))  # Keep previous tags, add user tags
                 else:
-                    post.tags = list(set().union(post.tags, tags))  # Keep previous tags
+                    limit_reached = False
 
-                if 'DeepBooru' in post.source:
-                    post.source = post.source.replace('DeepBooru\n', '')
-                    post.source = post.source.replace('\nDeepBooru', '')
+                if (not tags and config.auto_tagger['deepbooru_enabled']) or config.auto_tagger['deepbooru_forced']:
+                    result = deepbooru.tag_image(
+                        image,
+                        config.auto_tagger['deepbooru_threshold'],
+                        config.auto_tagger['deepbooru_set_tag'],
+                    )
+
+                    if result is None:
+                        continue
+
+                    tags, post.safety = result
+
+                    if post.relations:
+                        set_tags_from_relations(post)
+
+                    if add_tags:
+                        post.tags = list(set().union(post.tags, tags, add_tags))  # Keep previous tags and add user tags
+                    else:
+                        post.tags = list(set().union(post.tags, tags))  # Keep previous tags
+
+                    if 'DeepBooru' in post.source:
+                        post.source = post.source.replace('DeepBooru\n', '')
+                        post.source = post.source.replace('\nDeepBooru', '')
+
+                    if 'Deepbooru' not in post.source:
+                        post.source = collect_sources(post.source, 'Deepbooru')
+
+                    if tags:
+                        statistics(deepbooru=1)
+                    else:
+                        statistics(untagged=1)
+                elif not tags:
+                    statistics(untagged=1)
 
-                if 'Deepbooru' not in post.source:
-                    post.source = collect_sources(post.source, 'Deepbooru')
+                if remove_tags:
+                    [post.tags.remove(tag) for tag in remove_tags if tag in post.tags]
 
+                # If any tags were collected with SauceNAO or Deepbooru, remove tagme and deepbooru tag
                 if tags:
-                    statistics(deepbooru=1)
+                    [post.tags.remove(tag) for tag in post.tags if tag == 'tagme']
                 else:
-                    statistics(untagged=1)
-            elif not tags:
-                statistics(untagged=1)
+                    post.tags.append('tagme')
 
-            if remove_tags:
-                [post.tags.remove(tag) for tag in remove_tags if tag in post.tags]
-
-            # If any tags were collected with SauceNAO or Deepbooru, remove tagme and deepbooru tag
-            if tags:
-                [post.tags.remove(tag) for tag in post.tags if tag == 'tagme']
-            else:
-                post.tags.append('tagme')
-
-            szuru.update_post(post)
+                szuru.update_post(post)
 
-            if limit_reached and not config.auto_tagger['deepbooru_enabled']:
-                statistics(untagged=int(total_posts) - index - 1)  # Index starts at 0
-                break
-
-    if not from_upload_media:
-        total_tagged, total_deepbooru, total_untagged, total_skipped = statistics()
-
-        logger.success('Script has finished tagging.')
-        logger.success(f'Total:     {total_posts}')
-        logger.success(f'Tagged:    {str(total_tagged)}')
-        logger.success(f'Deepbooru: {str(total_deepbooru)}')
-        logger.success(f'Untagged:  {str(total_untagged)}')
-        logger.success(f'Skipped:   {str(total_skipped)}')
+                if limit_reached and not config.auto_tagger['deepbooru_enabled']:
+                    statistics(untagged=int(total_posts) - index - 1)  # Index starts at 0
+                    break
+
+        if not from_upload_media:
+            total_tagged, total_deepbooru, total_untagged, total_skipped = statistics()
+
+            logger.success('Script has finished tagging.')
+            logger.success(f'Total:     {total_posts}')
+            logger.success(f'Tagged:    {str(total_tagged)}')
+            logger.success(f'Deepbooru: {str(total_deepbooru)}')
+            logger.success(f'Untagged:  {str(total_untagged)}')
+            logger.success(f'Skipped:   {str(total_skipped)}')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/create_tags.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/create_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,44 +67,49 @@
     return category
 
 
 @logger.catch
 def main() -> None:
     """Read tags from file and create them in szurubooru."""
 
-    tags_file, query, min_post_count, limit, overwrite = parse_args()
+    try:
+        tags_file, query, min_post_count, limit, overwrite = parse_args()
 
-    if tags_file:
-        with open(tags_file) as tags_file:
-            lines = tags_file.readlines()
-
-            for line in tqdm(
-                lines,
-                ncols=80,
-                position=0,
-                leave=False,
-                disable=config.create_tags['hide_progress'],
-            ):
-                tag: list = line.strip().replace(' ', '').split(',')
-                tag_name = tag[0]
-                tag_category = tag[1]
-
-                try:
-                    szuru.create_tag(tag_name, tag_category)
-                except TagExistsError as e:  # noqa F841
-                    # logger.warning(e)  # Could result in lots of output with larger tag files
-                    pass
-    else:
-        results = Danbooru.download_tags(query, min_post_count, limit)
-
-        for result in results:
-            for tag in result:
-                try:
-                    szuru.create_tag(tag['name'], convert_tag_category(tag['category']), overwrite)
-                except TagExistsError as e:  # noqa F841
-                    pass
-
-    logger.success('Script finished creating tags!')
+        if tags_file:
+            with open(tags_file) as tags_file:
+                lines = tags_file.readlines()
+
+                for line in tqdm(
+                    lines,
+                    ncols=80,
+                    position=0,
+                    leave=False,
+                    disable=config.create_tags['hide_progress'],
+                ):
+                    tag: list = line.strip().replace(' ', '').split(',')
+                    tag_name = tag[0]
+                    tag_category = tag[1]
+
+                    try:
+                        szuru.create_tag(tag_name, tag_category)
+                    except TagExistsError as e:  # noqa F841
+                        # logger.warning(e)  # Could result in lots of output with larger tag files
+                        pass
+        else:
+            results = Danbooru.download_tags(query, min_post_count, limit)
+
+            for result in results:
+                for tag in result:
+                    try:
+                        szuru.create_tag(tag['name'], convert_tag_category(tag['category']), overwrite)
+                    except TagExistsError as e:  # noqa F841
+                        pass
+
+        logger.success('Script finished creating tags!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/delete_posts.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/delete_posts.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,37 +53,42 @@
     return except_ids, query
 
 
 @logger.catch
 def main() -> None:
     """Retrieve the posts from input query and delete them in szurubooru."""
 
-    except_ids, query = parse_args()
-
-    posts = szuru.get_posts(query, pagination=False, videos=True)
-
     try:
-        total_posts = next(posts)
-    except StopIteration:
-        logger.info(f'Found no posts for your query: {query}')
-        exit()
-
-    logger.info(f'Found {total_posts} posts. Start deleting...')
-    if except_ids:
-        logger.info(f'Won\'t delete the following ids: {except_ids}')
-
-    for post in tqdm(
-        posts,
-        ncols=80,
-        position=0,
-        leave=False,
-        total=int(total_posts),
-        disable=config.delete_posts['hide_progress'],
-    ):
-        if post.id not in except_ids:
-            szuru.delete_post(post)
+        except_ids, query = parse_args()
+
+        posts = szuru.get_posts(query, pagination=False, videos=True)
 
-    logger.success('Script finished deleting!')
+        try:
+            total_posts = next(posts)
+        except StopIteration:
+            logger.info(f'Found no posts for your query: {query}')
+            exit()
+
+        logger.info(f'Found {total_posts} posts. Start deleting...')
+        if except_ids:
+            logger.info(f'Won\'t delete the following ids: {except_ids}')
+
+        for post in tqdm(
+            posts,
+            ncols=80,
+            position=0,
+            leave=False,
+            total=int(total_posts),
+            disable=config.delete_posts['hide_progress'],
+        ):
+            if post.id not in except_ids:
+                szuru.delete_post(post)
+
+        logger.success('Script finished deleting!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/import_from_booru.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_booru.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,76 +112,81 @@
     upload_media.main(file, file_ext, metadata)
 
 
 @logger.catch
 def main() -> None:
     """Call respective functions to retrieve and upload posts based on user input."""
 
-    booru, query, limit = parse_args()
+    try:
+        booru, query, limit = parse_args()
 
-    if config.import_from_booru['deepbooru_enabled']:
-        config.upload_media['auto_tag'] = True
-        config.auto_tagger['saucenao_enabled'] = False
-        config.auto_tagger['deepbooru_enabled'] = True
-    else:
-        config.upload_media['auto_tag'] = False
-
-    if booru == 'all':
-        boorus = ['danbooru', 'gelbooru', 'yandere', 'konachan']
-    else:
-        boorus = [booru]
-
-    for booru in boorus:
-        logger.info(f'Retrieving posts from {booru} with query "{query}"...')
-
-        if booru == 'danbooru':
-            booru_client = Danbooru('danbooru', config.danbooru['user'], config.danbooru['api_key'])
-        elif booru == 'gelbooru':
-            booru_client = Gelbooru(config.gelbooru['user'], config.gelbooru['api_key'])
-        elif booru == 'konachan':
-            booru_client = Moebooru('konachan', config.konachan['user'], config.konachan['password'])
-        elif booru == 'yandere':
-            booru_client = Moebooru('yandere', config.yandere['user'], config.yandere['password'])
-
-        posts = get_posts_from_booru(booru_client, query, limit)
-
-        total_posts = next(posts)
-        logger.info(f'Found {total_posts} posts. Start importing...')
-
-        for post in tqdm(
-            posts,
-            ncols=80,
-            position=0,
-            leave=False,
-            total=int(total_posts),
-            disable=config.import_from_booru['hide_progress'],
-        ):
-            # Check by md5 hash if file is already uploaded
-            try:
-                if booru == 'gelbooru':
-                    md5 = Path(post.filename).stem
-                else:
-                    md5 = post['md5']
-            except KeyError:
-                print('')
-                logger.warning('Post has no MD5 attribute, it probably got removed from the site.')
-                continue
-
-            try:
-                file_ext = Path(post.filename).suffix[1:]  # Gelbooru, remove dot at the end
-            except AttributeError:
-                file_ext = post['file_url'].split('.')[-1]  # Other Boorus
-
-            result = szuru.get_posts(f'md5:{md5}')
-
-            try:
-                next(result)
-                logger.debug(f'Skipping post, already exists: {post}')
-            except StopIteration:
-                import_post(booru, post, file_ext, md5)
-                logger.debug(f'Importing post: {post}')
-
-    logger.success('Script finished importing!')
+        if config.import_from_booru['deepbooru_enabled']:
+            config.upload_media['auto_tag'] = True
+            config.auto_tagger['saucenao_enabled'] = False
+            config.auto_tagger['deepbooru_enabled'] = True
+        else:
+            config.upload_media['auto_tag'] = False
+
+        if booru == 'all':
+            boorus = ['danbooru', 'gelbooru', 'yandere', 'konachan']
+        else:
+            boorus = [booru]
+
+        for booru in boorus:
+            logger.info(f'Retrieving posts from {booru} with query "{query}"...')
+
+            if booru == 'danbooru':
+                booru_client = Danbooru('danbooru', config.danbooru['user'], config.danbooru['api_key'])
+            elif booru == 'gelbooru':
+                booru_client = Gelbooru(config.gelbooru['user'], config.gelbooru['api_key'])
+            elif booru == 'konachan':
+                booru_client = Moebooru('konachan', config.konachan['user'], config.konachan['password'])
+            elif booru == 'yandere':
+                booru_client = Moebooru('yandere', config.yandere['user'], config.yandere['password'])
+
+            posts = get_posts_from_booru(booru_client, query, limit)
+
+            total_posts = next(posts)
+            logger.info(f'Found {total_posts} posts. Start importing...')
+
+            for post in tqdm(
+                posts,
+                ncols=80,
+                position=0,
+                leave=False,
+                total=int(total_posts),
+                disable=config.import_from_booru['hide_progress'],
+            ):
+                # Check by md5 hash if file is already uploaded
+                try:
+                    if booru == 'gelbooru':
+                        md5 = Path(post.filename).stem
+                    else:
+                        md5 = post['md5']
+                except KeyError:
+                    print('')
+                    logger.warning('Post has no MD5 attribute, it probably got removed from the site.')
+                    continue
+
+                try:
+                    file_ext = Path(post.filename).suffix[1:]  # Gelbooru, remove dot at the end
+                except AttributeError:
+                    file_ext = post['file_url'].split('.')[-1]  # Other Boorus
+
+                result = szuru.get_posts(f'md5:{md5}')
+
+                try:
+                    next(result)
+                    logger.debug(f'Skipping post, already exists: {post}')
+                except StopIteration:
+                    import_post(booru, post, file_ext, md5)
+                    logger.debug(f'Importing post: {post}')
+
+        logger.success('Script finished importing!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/import_from_twitter.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/import_from_twitter.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,81 +40,86 @@
     return user_id, limit
 
 
 @logger.catch
 def main() -> None:
     """Call respective functions to retrieve and upload posts based on user input."""
 
-    user_id, limit = parse_args()
+    try:
+        user_id, limit = parse_args()
+
+        if not user_id:
+            if config.twitter['user_id'] != 'None':
+                user_id = config.twitter['user_id']
+            else:
+                logger.critical(
+                    'No user id specified! Pass --user-id to the script or configure the user_id in config.toml.',
+                )
+                exit()
 
-    if not user_id:
-        if config.twitter['user_id'] != 'None':
-            user_id = config.twitter['user_id']
+        if config.import_from_twitter['saucenao_enabled']:
+            config.auto_tagger['saucenao_enabled'] = True
         else:
-            logger.critical(
-                'No user id specified! Pass --user-id to the script or configure the user_id in config.toml.',
-            )
-            exit()
+            config.auto_tagger['saucenao_enabled'] = False
+
+        if config.import_from_twitter['deepbooru_enabled']:
+            config.auto_tagger['deepbooru_enabled'] = True
+        else:
+            config.auto_tagger['deepbooru_forced'] = False
+            config.auto_tagger['deepbooru_enabled'] = False
 
-    if config.import_from_twitter['saucenao_enabled']:
-        config.auto_tagger['saucenao_enabled'] = True
-    else:
-        config.auto_tagger['saucenao_enabled'] = False
-
-    if config.import_from_twitter['deepbooru_enabled']:
-        config.auto_tagger['deepbooru_enabled'] = True
-    else:
-        config.auto_tagger['deepbooru_forced'] = False
-        config.auto_tagger['deepbooru_enabled'] = False
-
-    if not config.import_from_twitter['saucenao_enabled'] and not config.import_from_twitter['deepbooru_enabled']:
-        config.upload_media['auto_tag'] = False
-
-    twitter = Twitter(
-        config.twitter['consumer_key'],
-        config.twitter['consumer_secret'],
-        config.twitter['access_token'],
-        config.twitter['access_token_secret'],
-    )
+        if not config.import_from_twitter['saucenao_enabled'] and not config.import_from_twitter['deepbooru_enabled']:
+            config.upload_media['auto_tag'] = False
 
-    try:
-        tweets = twitter.get_media_from_liked_tweets(user_id, limit)
-    except errors.Unauthorized:
-        logger.critical(
-            'You\'re unauthorized to retrieve the user\'s tweets! User profile is probably private. '
-            'Configure credentials in config.toml.',
+        twitter = Twitter(
+            config.twitter['consumer_key'],
+            config.twitter['consumer_secret'],
+            config.twitter['access_token'],
+            config.twitter['access_token_secret'],
         )
-        exit()
-
-    logger.info(f'Found {len(tweets)} tweets with media attachments. Start importing...')
 
-    for tweet in tqdm(
-        tweets,
-        ncols=80,
-        position=0,
-        leave=False,
-        total=len(tweets),
-        disable=config.import_from_twitter['hide_progress'],
-    ):
-        files = []
-        for media in tweet[1]:
-            files.append(download_media(media['url']))
-
-        for index, file in enumerate(files):
-            # Check by md5 hash if file is already uploaded
-            md5 = get_md5sum(file)
-            result = szuru.get_posts(f'md5:{md5}')
-
-            try:
-                next(result)
-                logger.debug(f'Skipping tweet, already exists: {tweet}')
-            except StopIteration:
-                logger.debug(f'Importing tweet: {tweet}')
+        try:
+            tweets = twitter.get_media_from_liked_tweets(user_id, limit)
+        except errors.Unauthorized:
+            logger.critical(
+                'You\'re unauthorized to retrieve the user\'s tweets! User profile is probably private. '
+                'Configure credentials in config.toml.',
+            )
+            exit()
 
-                metadata = {'tags': ['tagme'], 'safety': 'unsafe', 'source': tweet[0]}
-                upload_media.main(file, tweet[1][index]['file_ext'], metadata)
+        logger.info(f'Found {len(tweets)} tweets with media attachments. Start importing...')
 
-    logger.success('Script finished importing!')
+        for tweet in tqdm(
+            tweets,
+            ncols=80,
+            position=0,
+            leave=False,
+            total=len(tweets),
+            disable=config.import_from_twitter['hide_progress'],
+        ):
+            files = []
+            for media in tweet[1]:
+                files.append(download_media(media['url']))
+
+            for index, file in enumerate(files):
+                # Check by md5 hash if file is already uploaded
+                md5 = get_md5sum(file)
+                result = szuru.get_posts(f'md5:{md5}')
+
+                try:
+                    next(result)
+                    logger.debug(f'Skipping tweet, already exists: {tweet}')
+                except StopIteration:
+                    logger.debug(f'Importing tweet: {tweet}')
+
+                    metadata = {'tags': ['tagme'], 'safety': 'unsafe', 'source': tweet[0]}
+                    upload_media.main(file, tweet[1][index]['file_ext'], metadata)
+
+        logger.success('Script finished importing!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/reset_posts.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/reset_posts.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,39 +66,44 @@
     return add_tags, except_ids, query
 
 
 @logger.catch
 def main() -> None:
     """Retrieve the posts from input query and reset them in szurubooru."""
 
-    add_tags, except_ids, query = parse_args()
-
-    posts = szuru.get_posts(query, videos=True)
-
     try:
-        total_posts = next(posts)
-    except StopIteration:
-        logger.info(f'Found no posts for your query: {query}')
-        exit()
-
-    logger.info(f'Found {total_posts} posts. Start resetting...')
-    if except_ids:
-        logger.info(f'Won\'t reset the following ids: {except_ids}')
-
-    for post in tqdm(
-        posts,
-        ncols=80,
-        position=0,
-        leave=False,
-        total=int(total_posts),
-        disable=config.reset_posts['hide_progress'],
-    ):
-        if post.id not in except_ids:
-            post.tags = add_tags if add_tags else []
-            post.source = ''
-            szuru.update_post(post)
+        add_tags, except_ids, query = parse_args()
+
+        posts = szuru.get_posts(query, videos=True)
 
-    logger.success('Script finished resetting!')
+        try:
+            total_posts = next(posts)
+        except StopIteration:
+            logger.info(f'Found no posts for your query: {query}')
+            exit()
+
+        logger.info(f'Found {total_posts} posts. Start resetting...')
+        if except_ids:
+            logger.info(f'Won\'t reset the following ids: {except_ids}')
+
+        for post in tqdm(
+            posts,
+            ncols=80,
+            position=0,
+            leave=False,
+            total=int(total_posts),
+            disable=config.reset_posts['hide_progress'],
+        ):
+            if post.id not in except_ids:
+                post.tags = add_tags if add_tags else []
+                post.source = ''
+                szuru.update_post(post)
+
+        logger.success('Script finished resetting!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/tag_posts.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/tag_posts.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,52 +88,57 @@
     return add_tags, remove_tags, update_implications, args.mode, query
 
 
 @logger.catch
 def main() -> None:
     """Retrieve the posts from input query, set post.tags based on mode and update them in szurubooru."""
 
-    add_tags, remove_tags, update_implications, mode, query = parse_args()
-
-    posts = szuru.get_posts(query, videos=True)
-
     try:
-        total_posts = next(posts)
-    except StopIteration:
-        logger.info(f'Found no posts for your query: {query}')
-        exit()
-
-    logger.info(f'Found {total_posts} posts. Start tagging...')
-
-    for post in tqdm(
-        posts,
-        ncols=80,
-        position=0,
-        leave=False,
-        total=int(total_posts),
-        disable=config.tag_posts['hide_progress'],
-    ):
-        if mode == 'append':
-            if add_tags:
-                post.tags = list(set().union(post.tags, add_tags))
-        elif mode == 'overwrite':
-            if add_tags:
-                post.tags = add_tags
-
-        if remove_tags:
-            post.tags = [tag for tag in post.tags if tag not in remove_tags]
-
-        if update_implications:
-            for tag in post.tags:
-                szuru_tag = szuru.api.getTag(tag)
-                for implication in szuru_tag.implications:
-                    szuru_implication = szuru.api.getTag(implication)
-                    if szuru_implication not in post.tags:
-                        post.tags.append(szuru_implication.primary_name)
+        add_tags, remove_tags, update_implications, mode, query = parse_args()
 
-        szuru.update_post(post)
+        posts = szuru.get_posts(query, videos=True)
 
-    logger.success('Script finished tagging!')
+        try:
+            total_posts = next(posts)
+        except StopIteration:
+            logger.info(f'Found no posts for your query: {query}')
+            exit()
+
+        logger.info(f'Found {total_posts} posts. Start tagging...')
+
+        for post in tqdm(
+            posts,
+            ncols=80,
+            position=0,
+            leave=False,
+            total=int(total_posts),
+            disable=config.tag_posts['hide_progress'],
+        ):
+            if mode == 'append':
+                if add_tags:
+                    post.tags = list(set().union(post.tags, add_tags))
+            elif mode == 'overwrite':
+                if add_tags:
+                    post.tags = add_tags
+
+            if remove_tags:
+                post.tags = [tag for tag in post.tags if tag not in remove_tags]
+
+            if update_implications:
+                for tag in post.tags:
+                    szuru_tag = szuru.api.getTag(tag)
+                    for implication in szuru_tag.implications:
+                        szuru_implication = szuru.api.getTag(implication)
+                        if szuru_implication not in post.tags:
+                            post.tags.append(szuru_implication.primary_name)
+
+            szuru.update_post(post)
+
+        logger.success('Script finished tagging!')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/scripts/upload_media.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/scripts/upload_media.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,47 +272,52 @@
             if file_ext not in ['mp4', 'webm']:
                 auto_tagger(str(post_id), post.media)
 
 
 def main(file_to_upload: bytes = None, file_ext: str = None, metadata: dict = None) -> int:
     """Main logic of the script."""
 
-    if not file_to_upload:
-        files_to_upload = get_files(config.upload_media['src_path'])
-        from_import_from = False
-    else:
-        files_to_upload = file_to_upload
-        from_import_from = True
-        config.upload_media['hide_progress'] = True
-
-    if files_to_upload:
-        if not from_import_from:
-            logger.info('Found ' + str(len(files_to_upload)) + ' file(s). Starting upload...')
-
-            for file_to_upload in tqdm(
-                files_to_upload,
-                ncols=80,
-                position=0,
-                leave=False,
-                disable=config.upload_media['hide_progress'],
-            ):
-                with open(file_to_upload, 'rb') as f:
-                    file = f.read()
-                upload_post(file, file_ext=Path(file_to_upload).suffix[1:], file_to_upload=file_to_upload)
+    try:
+        if not file_to_upload:
+            files_to_upload = get_files(config.upload_media['src_path'])
+            from_import_from = False
+        else:
+            files_to_upload = file_to_upload
+            from_import_from = True
+            config.upload_media['hide_progress'] = True
 
-                if config.upload_media['cleanup']:
-                    if os.path.exists(file_to_upload):
-                        os.remove(file_to_upload)
+        if files_to_upload:
+            if not from_import_from:
+                logger.info('Found ' + str(len(files_to_upload)) + ' file(s). Starting upload...')
 
-            if config.upload_media['cleanup']:
-                cleanup_dirs(config.upload_media['src_path'])  # Remove dirs after files have been deleted
+                for file_to_upload in tqdm(
+                    files_to_upload,
+                    ncols=80,
+                    position=0,
+                    leave=False,
+                    disable=config.upload_media['hide_progress'],
+                ):
+                    with open(file_to_upload, 'rb') as f:
+                        file = f.read()
+                    upload_post(file, file_ext=Path(file_to_upload).suffix[1:], file_to_upload=file_to_upload)
+
+                    if config.upload_media['cleanup']:
+                        if os.path.exists(file_to_upload):
+                            os.remove(file_to_upload)
 
-            if not from_import_from:
-                logger.success('Script has finished uploading!')
+                if config.upload_media['cleanup']:
+                    cleanup_dirs(config.upload_media['src_path'])  # Remove dirs after files have been deleted
+
+                if not from_import_from:
+                    logger.success('Script has finished uploading!')
+            else:
+                upload_post(file_to_upload, file_ext, metadata)
         else:
-            upload_post(file_to_upload, file_ext, metadata)
-    else:
-        logger.info('No files found to upload.')
+            logger.info('No files found to upload.')
+    except KeyboardInterrupt:
+        print('')
+        logger.info('Received keyboard interrupt from user.')
+        exit(1)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/szurubooru.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/szurubooru.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/twitter.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/twitter.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/src/szurubooru_toolkit/utils.py` & `szurubooru_toolkit-0.8.0/src/szurubooru_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `szurubooru_toolkit-0.7.7/PKG-INFO` & `szurubooru_toolkit-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: szurubooru-toolkit
-Version: 0.7.7
+Version: 0.8.0
 Summary: Python package and script collection to manage szurubooru.
 Home-page: https://github.com/reluce/szurubooru-toolkit
 License: GPL-3.0-only
 Keywords: szurubooru,szuru,booru,saucenao,deepbooru
 Author: reluce
 Author-email: reluce@fkosquad.moe
 Requires-Python: >=3.8,<3.11
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: Pillow (>=9.1.1,<10.0.0)
 Requires-Dist: Pybooru (>=4.2.2,<5.0.0)
 Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
+Requires-Dist: gallery-dl (>=1.25.1,<2.0.0)
 Requires-Dist: keras (>=2.8.0,<3.0.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
 Requires-Dist: lxml (>=4.8.0,<5.0.0)
 Requires-Dist: numpy (>=1.22.1,<2.0.0)
 Requires-Dist: pathvalidate (>=2.5.0,<3.0.0)
 Requires-Dist: pygelbooru (>=0.3.2,<0.4.0)
 Requires-Dist: pysaucenao (>=1.6.1,<2.0.0)
@@ -142,14 +143,16 @@
 | `upload_media` | `convert_quality` | Only images above this threshold will be converted to jpg if `convert_to_jpg` is True. | `"3MB\|500KB"` |
 | `upload_media` | `shrink` | Set to true to shrink images to shrink_dimensions based on shrink_threshold below. Images might slip through identical post check. | `false` |
 | `upload_media` | `shrink_threshold` | Images which total pixel size exceeds this treshold will be resized to `shrink_size`. E.g. 2000x3000 results in 6000000. | `"6000000"` |
 | `upload_media` | `shrink_dimensions` | Set the max value for width/height. Keeps aspect ratio. E.g. 2000x4000 results in 700x1400, 4000x2000 in 1400x700 (with `"1400x1400"`). | `"2500x2500"` |
 | `upload_media` | `default_safety` | # Set the default safety in case neither SauceNAO, nor Deepbooru could determine it | `safe` |
 | `import_from_booru` | `deepbooru_enabled` | Apply Deepbooru tagging additionally besides fetched tags from Booru | `false` |
 | `import_from_booru` | `hide_progress` | Set this to true to hide the progress bar | `false` |
+| `import_from_url` | `tmp_path` | Path to directory where temporary downloads from gallery-dl script will be saved | `false` |
+| `import_from_url` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `import_from_twitter` | `saucenao_enabled` | Tag posts with SauceNAO | `false` |
 | `import_from_twitter` | `deepbooru_enabled` | Tag posts with Deepbooru | `false` |
 | `import_from_twitter` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `create_tags` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `delete_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `reset_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
 | `tag_posts` | `hide_progress` | Set this to true to hide the progress bar | `false` |
@@ -170,14 +173,15 @@
 Following scripts are currently available:
 
 * `auto-tagger`: Batch tagging of posts with SauceNAO and Deepbooru
 * `create-tags`: Batch creation of tags with their categories
 * `delete-posts`: Batch delete of posts
 * `import-from-booru`: Batch importing of posts with their tags from various Boorus
 * `import-from-twitter`: Batch importing of Twitter favorites
+* `import-from-url`: Batch importing of URLs based on [gallery-dl](https://github.com/mikf/gallery-dl)
 * `reset-posts`: Batch resetting of posts (remove tags and sources)
 * `upload-media`: Batch upload of media files from local source folder
 * `tag-posts`: Manual batch tagging
 
 See the descriptions below on how to use them.
 
 If you installed this package with pip, you can generally just call the scripts from your shell (if your $PATH is set correctly).
@@ -260,14 +264,59 @@
 * `import-from-booru danbooru "tag1 tagN"`
 * `import-from-booru yandere "tag1 tag2 -tagN"`
 * `import-from-booru all "tag1 -tagN"`
 
 Note that if you specify `all` to download from all Boorus, you are limited to two tags because free Danbooru accounts are limited to two tags per query.
 If you have a Gold/Platinum account, set your credentials in `config.toml`. Note that it's currently untested if the script will work with upgraded accounts.
 
+### :link:	import-from-url
+This scripts imports posts with their tags from the URL passed to this script.
+In the background, it simply calls the [gallery-dl](https://github.com/mikf/gallery-dl) script and parses its output.
+Alternatively, an input file with multiple URLs can be specified.
+
+In the `config.toml` file, you have to specify a directory where posts will be temporarily saved to.
+Since this script is using the `upload-media` script to upload the post, following settings apply from the `upload-media` section:
+* max_similarity
+* convert_to_jpg
+* convert_threshold
+* shrink
+* shrink_threshold
+* shrink_dimensions
+
+:information_source:️ **Following Boorus are currently supported:**
+* Gelbooru
+* Danbooru
+* Sankaku
+* Konachan
+* Yandere
+
+Credentials in your `config.toml` file will be passed to the gallery-dl script if you use a single input URL to this script.
+
+__Usage__
+```
+usage: import-from-url [-h] [--range RANGE] [--input-file INPUT_FILE] [url ...]
+
+This script downloads and tags posts from various Boorus based on your input query.
+
+positional arguments:
+  url                   The URL for the posts you want to download and tag
+
+optional arguments:
+  -h, --help            show this help message and exit
+  --range RANGE         Index range(s) specifying which files to download. These can be either a constant value, range, or slice (e.g. '5', '8-20', or '1:24:3')
+  --input-file INPUT_FILE
+                        Download URLs found in FILE.
+
+```
+
+__Examples__
+* `import-from-url "https://danbooru.donmai.us/posts?tags=foo"`
+* `import-from-url "https://chan.sankakucomplex.com/?tags=foo"`
+* `import-from-url "https://beta.sankakucomplex.com/post/show/<id>"`
+
 ### :dove: import-from-twitter
 This script fetches media files from your Twitter likes, uploads and optionally tags them.
 
 :warning: __OAuth 1.0a credentials are required to read the likes from a user. See https://developer.twitter.com/en/docs/authentication/oauth-1-0a on how to generate them.__
 
 The `user_id` can be converted on sites like https://tweeterid.com/. If you configured above credentials, you can also get your own ID from the `access_token`, which is in following format: `<user_id>-<random_string>`
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

