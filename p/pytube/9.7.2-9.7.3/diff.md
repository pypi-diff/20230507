# Comparing `tmp/pytube-9.7.2.tar.gz` & `tmp/pytube-9.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytube-9.7.2.tar", last modified: Thu Nov 12 12:32:39 2020, max compression
+gzip compressed data, was "dist/pytube-9.7.3.tar", last modified: Wed Nov 18 14:40:57 2020, max compression
```

## Comparing `pytube-9.7.2.tar` & `pytube-9.7.3.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.071297 pytube-9.7.2/
--rw-r--r--   0 rghose   (35940) staff       (20)     1155 2020-10-31 00:20:53.000000 pytube-9.7.2/LICENSE
--rw-r--r--   0 rghose   (35940) staff       (20)       55 2020-10-31 00:20:53.000000 pytube-9.7.2/MANIFEST.in
--rw-r--r--   0 rghose   (35940) staff       (20)    18882 2020-11-12 12:32:39.071011 pytube-9.7.2/PKG-INFO
--rw-r--r--   0 rghose   (35940) staff       (20)    15518 2020-11-12 12:29:42.000000 pytube-9.7.2/README.md
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.058828 pytube-9.7.2/pytube/
--rw-r--r--   0 rghose   (35940) staff       (20)      538 2020-10-31 00:20:53.000000 pytube-9.7.2/pytube/__init__.py
--rw-r--r--   0 rghose   (35940) staff       (20)    11626 2020-11-07 20:44:50.000000 pytube-9.7.2/pytube/__main__.py
--rw-r--r--   0 rghose   (35940) staff       (20)     4967 2020-11-07 20:44:50.000000 pytube-9.7.2/pytube/captions.py
--rw-r--r--   0 rghose   (35940) staff       (20)     9667 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/cipher.py
--rwxr-xr-x   0 rghose   (35940) staff       (20)    15480 2020-10-31 00:20:53.000000 pytube-9.7.2/pytube/cli.py
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.063673 pytube-9.7.2/pytube/contrib/
--rw-r--r--   0 rghose   (35940) staff       (20)        0 2020-10-31 00:20:53.000000 pytube-9.7.2/pytube/contrib/__init__.py
--rw-r--r--   0 rghose   (35940) staff       (20)    13125 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/contrib/playlist.py
--rw-r--r--   0 rghose   (35940) staff       (20)     2181 2020-11-07 20:44:50.000000 pytube-9.7.2/pytube/exceptions.py
--rw-r--r--   0 rghose   (35940) staff       (20)    12447 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/extract.py
--rw-r--r--   0 rghose   (35940) staff       (20)     5893 2020-11-07 20:44:50.000000 pytube-9.7.2/pytube/helpers.py
--rw-r--r--   0 rghose   (35940) staff       (20)     3647 2020-10-31 00:20:53.000000 pytube-9.7.2/pytube/itags.py
--rw-r--r--   0 rghose   (35940) staff       (20)     1429 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/monostate.py
--rw-r--r--   0 rghose   (35940) staff       (20)    12745 2020-10-31 00:20:53.000000 pytube-9.7.2/pytube/query.py
--rw-r--r--   0 rghose   (35940) staff       (20)     6392 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/request.py
--rw-r--r--   0 rghose   (35940) staff       (20)    12807 2020-11-12 12:29:42.000000 pytube-9.7.2/pytube/streams.py
--rw-r--r--   0 rghose   (35940) staff       (20)       98 2020-11-12 12:31:37.000000 pytube-9.7.2/pytube/version.py
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.062430 pytube-9.7.2/pytube.egg-info/
--rw-r--r--   0 rghose   (35940) staff       (20)    18882 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/PKG-INFO
--rw-r--r--   0 rghose   (35940) staff       (20)      851 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/SOURCES.txt
--rw-r--r--   0 rghose   (35940) staff       (20)        1 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/dependency_links.txt
--rw-r--r--   0 rghose   (35940) staff       (20)       70 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/entry_points.txt
--rw-r--r--   0 rghose   (35940) staff       (20)       18 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/requires.txt
--rw-r--r--   0 rghose   (35940) staff       (20)        7 2020-11-12 12:32:38.000000 pytube-9.7.2/pytube.egg-info/top_level.txt
--rw-r--r--   0 rghose   (35940) staff       (20)        1 2020-10-31 00:46:56.000000 pytube-9.7.2/pytube.egg-info/zip-safe
--rw-r--r--   0 rghose   (35940) staff       (20)       38 2020-11-12 12:32:39.071420 pytube-9.7.2/setup.cfg
--rwxr-xr-x   0 rghose   (35940) staff       (20)     2140 2020-10-31 00:43:17.000000 pytube-9.7.2/setup.py
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.069913 pytube-9.7.2/tests/
--rw-r--r--   0 rghose   (35940) staff       (20)       81 2020-10-31 00:20:53.000000 pytube-9.7.2/tests/__init__.py
--rw-r--r--   0 rghose   (35940) staff       (20)     3234 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/conftest.py
-drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-12 12:32:39.070275 pytube-9.7.2/tests/contrib/
--rw-r--r--   0 rghose   (35940) staff       (20)     9108 2020-11-12 12:29:42.000000 pytube-9.7.2/tests/contrib/test_playlist.py
--rw-r--r--   0 rghose   (35940) staff       (20)     5870 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/test_captions.py
--rw-r--r--   0 rghose   (35940) staff       (20)      779 2020-11-12 12:29:42.000000 pytube-9.7.2/tests/test_cipher.py
--rw-r--r--   0 rghose   (35940) staff       (20)    17344 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/test_cli.py
--rw-r--r--   0 rghose   (35940) staff       (20)     2499 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/test_exceptions.py
--rw-r--r--   0 rghose   (35940) staff       (20)     3132 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/test_extract.py
--rw-r--r--   0 rghose   (35940) staff       (20)     5024 2020-11-12 12:29:42.000000 pytube-9.7.2/tests/test_helpers.py
--rw-r--r--   0 rghose   (35940) staff       (20)      300 2020-10-31 00:20:53.000000 pytube-9.7.2/tests/test_itags.py
--rw-r--r--   0 rghose   (35940) staff       (20)      992 2020-10-31 00:20:53.000000 pytube-9.7.2/tests/test_main.py
--rw-r--r--   0 rghose   (35940) staff       (20)     5638 2020-11-07 20:44:50.000000 pytube-9.7.2/tests/test_query.py
--rw-r--r--   0 rghose   (35940) staff       (20)     1370 2020-10-31 00:20:53.000000 pytube-9.7.2/tests/test_request.py
--rw-r--r--   0 rghose   (35940) staff       (20)    13691 2020-11-12 12:29:42.000000 pytube-9.7.2/tests/test_streams.py
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.140627 pytube-9.7.3/
+-rw-r--r--   0 rghose   (35940) staff       (20)     1155 2020-10-31 00:20:53.000000 pytube-9.7.3/LICENSE
+-rw-r--r--   0 rghose   (35940) staff       (20)       55 2020-10-31 00:20:53.000000 pytube-9.7.3/MANIFEST.in
+-rw-r--r--   0 rghose   (35940) staff       (20)    18882 2020-11-18 14:40:57.140336 pytube-9.7.3/PKG-INFO
+-rw-r--r--   0 rghose   (35940) staff       (20)    15518 2020-11-12 12:29:42.000000 pytube-9.7.3/README.md
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.126351 pytube-9.7.3/pytube/
+-rw-r--r--   0 rghose   (35940) staff       (20)      538 2020-10-31 00:20:53.000000 pytube-9.7.3/pytube/__init__.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    12655 2020-11-18 14:40:09.000000 pytube-9.7.3/pytube/__main__.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     4967 2020-11-07 20:44:50.000000 pytube-9.7.3/pytube/captions.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     9667 2020-11-12 12:29:42.000000 pytube-9.7.3/pytube/cipher.py
+-rwxr-xr-x   0 rghose   (35940) staff       (20)    15480 2020-10-31 00:20:53.000000 pytube-9.7.3/pytube/cli.py
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.129711 pytube-9.7.3/pytube/contrib/
+-rw-r--r--   0 rghose   (35940) staff       (20)        0 2020-10-31 00:20:53.000000 pytube-9.7.3/pytube/contrib/__init__.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    13125 2020-11-12 12:29:42.000000 pytube-9.7.3/pytube/contrib/playlist.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     2181 2020-11-07 20:44:50.000000 pytube-9.7.3/pytube/exceptions.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    14515 2020-11-18 14:40:09.000000 pytube-9.7.3/pytube/extract.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     5893 2020-11-07 20:44:50.000000 pytube-9.7.3/pytube/helpers.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     3647 2020-10-31 00:20:53.000000 pytube-9.7.3/pytube/itags.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     1474 2020-11-18 14:40:09.000000 pytube-9.7.3/pytube/metadata.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     1429 2020-11-12 12:29:42.000000 pytube-9.7.3/pytube/monostate.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    12745 2020-10-31 00:20:53.000000 pytube-9.7.3/pytube/query.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     6423 2020-11-18 14:40:09.000000 pytube-9.7.3/pytube/request.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    12807 2020-11-12 12:29:42.000000 pytube-9.7.3/pytube/streams.py
+-rw-r--r--   0 rghose   (35940) staff       (20)       98 2020-11-18 14:40:47.000000 pytube-9.7.3/pytube/version.py
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.129004 pytube-9.7.3/pytube.egg-info/
+-rw-r--r--   0 rghose   (35940) staff       (20)    18882 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/PKG-INFO
+-rw-r--r--   0 rghose   (35940) staff       (20)      893 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/SOURCES.txt
+-rw-r--r--   0 rghose   (35940) staff       (20)        1 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/dependency_links.txt
+-rw-r--r--   0 rghose   (35940) staff       (20)       70 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/entry_points.txt
+-rw-r--r--   0 rghose   (35940) staff       (20)       18 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/requires.txt
+-rw-r--r--   0 rghose   (35940) staff       (20)        7 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/top_level.txt
+-rw-r--r--   0 rghose   (35940) staff       (20)        1 2020-11-18 14:40:56.000000 pytube-9.7.3/pytube.egg-info/zip-safe
+-rw-r--r--   0 rghose   (35940) staff       (20)       38 2020-11-18 14:40:57.140767 pytube-9.7.3/setup.cfg
+-rwxr-xr-x   0 rghose   (35940) staff       (20)     2140 2020-10-31 00:43:17.000000 pytube-9.7.3/setup.py
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.138955 pytube-9.7.3/tests/
+-rw-r--r--   0 rghose   (35940) staff       (20)       81 2020-10-31 00:20:53.000000 pytube-9.7.3/tests/__init__.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     3234 2020-11-07 20:44:50.000000 pytube-9.7.3/tests/conftest.py
+drwxr-xr-x   0 rghose   (35940) staff       (20)        0 2020-11-18 14:40:57.139628 pytube-9.7.3/tests/contrib/
+-rw-r--r--   0 rghose   (35940) staff       (20)     9108 2020-11-12 12:29:42.000000 pytube-9.7.3/tests/contrib/test_playlist.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     5870 2020-11-07 20:44:50.000000 pytube-9.7.3/tests/test_captions.py
+-rw-r--r--   0 rghose   (35940) staff       (20)      779 2020-11-12 12:29:42.000000 pytube-9.7.3/tests/test_cipher.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    17344 2020-11-07 20:44:50.000000 pytube-9.7.3/tests/test_cli.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     2499 2020-11-07 20:44:50.000000 pytube-9.7.3/tests/test_exceptions.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     3372 2020-11-18 14:40:09.000000 pytube-9.7.3/tests/test_extract.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     5024 2020-11-12 12:29:42.000000 pytube-9.7.3/tests/test_helpers.py
+-rw-r--r--   0 rghose   (35940) staff       (20)      300 2020-10-31 00:20:53.000000 pytube-9.7.3/tests/test_itags.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     1786 2020-11-18 14:40:09.000000 pytube-9.7.3/tests/test_main.py
+-rw-r--r--   0 rghose   (35940) staff       (20)      546 2020-11-18 14:40:09.000000 pytube-9.7.3/tests/test_metadata.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     5638 2020-11-07 20:44:50.000000 pytube-9.7.3/tests/test_query.py
+-rw-r--r--   0 rghose   (35940) staff       (20)     1370 2020-10-31 00:20:53.000000 pytube-9.7.3/tests/test_request.py
+-rw-r--r--   0 rghose   (35940) staff       (20)    13691 2020-11-12 12:29:42.000000 pytube-9.7.3/tests/test_streams.py
```

### Comparing `pytube-9.7.2/LICENSE` & `pytube-9.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/PKG-INFO` & `pytube-9.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube
-Version: 9.7.2
+Version: 9.7.3
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/nficano/pytube
 Author: Nick Ficano, Harold Martin
 Author-email: nficano@gmail.com, harold.martin@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/nficano/pytube/issues
 Project-URL: Read the Docs, https://python-pytube.readthedocs.io/en/latest
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube Version: 9.7.2 Summary: Python 3 library for
+Metadata-Version: 2.1 Name: pytube Version: 9.7.3 Summary: Python 3 library for
 downloading YouTube Videos. Home-page: https://github.com/nficano/pytube
 Author: Nick Ficano, Harold Martin Author-email: nficano@gmail.com,
 harold.martin@gmail.com License: MIT Project-URL: Bug Reports, https://
 github.com/nficano/pytube/issues Project-URL: Read the Docs, https://python-
 pytube.readthedocs.io/en/latest Description: ## (24 JULY 2020) Note: Actively
 soliciting contributers! Ping @ronncc if you would like to help out
                                  [pytube logo]
```

### Comparing `pytube-9.7.2/README.md` & `pytube-9.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/__init__.py` & `pytube-9.7.3/pytube/__init__.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/__main__.py` & `pytube-9.7.3/pytube/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from pytube.exceptions import RecordingUnavailable
 from pytube.exceptions import VideoUnavailable
 from pytube.exceptions import VideoPrivate
 from pytube.extract import apply_descrambler
 from pytube.extract import apply_signature
 from pytube.extract import get_ytplayer_config
 from pytube.helpers import install_proxy
+from pytube.metadata import YouTubeMetadata
 from pytube.monostate import Monostate
 from pytube.monostate import OnComplete
 from pytube.monostate import OnProgress
 
 logger = logging.getLogger(__name__)
 
 
@@ -56,39 +57,37 @@
             progress events.
         :param func on_complete_callback:
             (Optional) User defined callback function for stream download
             complete events.
 
         """
         self.js: Optional[str] = None  # js fetched by js_url
-        self.js_url: Optional[
-            str
-        ] = None  # the url to the js, parsed from watch html
+        self.js_url: Optional[str] = None  # the url to the js, parsed from watch html
 
         # note: vid_info may eventually be removed. It sounds like it once had
         # additional formats, but that doesn't appear to still be the case.
 
         # the url to vid info, parsed from watch html
         self.vid_info_url: Optional[str] = None
-        self.vid_info_raw: Optional[
-            str
-        ] = None  # content fetched by vid_info_url
+        self.vid_info_raw: Optional[str] = None  # content fetched by vid_info_url
         self.vid_info: Optional[Dict] = None  # parsed content of vid_info_raw
 
-        self.watch_html: Optional[
-            str
-        ] = None  # the html of /watch?v=<video_id>
+        self.watch_html: Optional[str] = None  # the html of /watch?v=<video_id>
         self.embed_html: Optional[str] = None
         self.player_config_args: Dict = {}  # inline js in the html containing
         self.player_response: Dict = {}
         # streams
         self.age_restricted: Optional[bool] = None
 
         self.fmt_streams: List[Stream] = []
 
+        self.initial_data_raw = None
+        self.initial_data = {}
+        self._metadata: Optional[YouTubeMetadata] = None
+
         # video_id part of /watch?v=<video_id>
         self.video_id = extract.video_id(url)
 
         self.watch_url = f"https://youtube.com/watch?v={self.video_id}"
         self.embed_url = f"https://www.youtube.com/embed/{self.video_id}"
 
         # Shared between all instances of `Stream` (Borg pattern).
@@ -117,18 +116,19 @@
         self.vid_info = dict(parse_qsl(self.vid_info_raw))
         self.player_config_args = self.vid_info
         self.player_response = json.loads(self.vid_info['player_response'])
 
         # On pre-signed videos, we need to use get_ytplayer_config to fix
         #  the player_response item
         if 'streamingData' not in self.player_config_args['player_response']:
-            config_response = get_ytplayer_config(
-                self.watch_html
-            )['args']['player_response']
-            self.player_config_args['player_response'] = config_response
+            config_response = get_ytplayer_config(self.watch_html)
+            if 'args' in config_response:
+                self.player_config_args['player_response'] = config_response['args']['player_response']  # noqa: E501
+            else:
+                self.player_config_args['player_response'] = config_response
 
         # https://github.com/nficano/pytube/issues/165
         stream_maps = ["url_encoded_fmt_stream_map"]
         if "adaptive_fmts" in self.player_config_args:
             stream_maps.append("adaptive_fmts")
 
         # unscramble the progressive and adaptive stream manifests.
@@ -145,17 +145,20 @@
 
             apply_signature(self.player_config_args, fmt, self.js)
 
             # build instances of :class:`Stream <Stream>`
             self.initialize_stream_objects(fmt)
 
         # load the player_response object (contains subtitle information)
-        self.player_response = json.loads(
-            self.player_config_args["player_response"]
-        )
+        if isinstance(self.player_config_args["player_response"], str):
+            self.player_response = json.loads(
+                self.player_config_args["player_response"]
+            )
+        else:
+            self.player_response = self.player_config_args["player_response"]
         del self.player_config_args["player_response"]
         self.stream_monostate.title = self.title
         self.stream_monostate.duration = self.length
 
     def prefetch(self) -> None:
         """Eagerly download all necessary data.
 
@@ -183,14 +186,17 @@
                 self.video_id, self.watch_url
             )
         else:
             self.vid_info_url = extract.video_info_url(
                 video_id=self.video_id, watch_url=self.watch_url
             )
 
+        self.initial_data_raw = extract.initial_data(self.watch_html)
+        self.initial_data = json.loads(self.initial_data_raw)
+
         self.vid_info_raw = request.get(self.vid_info_url)
         if not self.age_restricted:
             self.js_url = extract.js_url(self.watch_html)
             self.js = request.get(self.js_url)
 
     def initialize_stream_objects(self, fmt: str) -> None:
         """Convert manifest data to instances of :class:`Stream <Stream>`.
@@ -283,28 +289,24 @@
     @property
     def description(self) -> str:
         """Get the video description.
 
         :rtype: str
 
         """
-        return self.player_response.get("videoDetails", {}).get(
-            "shortDescription"
-        )
+        return self.player_response.get("videoDetails", {}).get("shortDescription")
 
     @property
     def rating(self) -> float:
         """Get the video average rating.
 
         :rtype: float
 
         """
-        return self.player_response.get("videoDetails", {}).get(
-            "averageRating"
-        )
+        return self.player_response.get("videoDetails", {}).get("averageRating")
 
     @property
     def length(self) -> int:
         """Get the video length in seconds.
 
         :rtype: str
 
@@ -334,14 +336,33 @@
         """Get the video author.
         :rtype: str
         """
         return self.player_response.get("videoDetails", {}).get(
             "author", "unknown"
         )
 
+    @property
+    def keywords(self) -> List[str]:
+        """Get the video keywords.
+        :rtype: List[str]
+        """
+        return self.player_response.get('videoDetails', {}).get('keywords', [])
+
+    @property
+    def metadata(self) -> Optional[YouTubeMetadata]:
+        """Get the metadata for the video.
+
+        :rtype: YouTubeMetadata
+        """
+        if self._metadata:
+            return self._metadata
+        else:
+            self._metadata = extract.metadata(self.initial_data)
+            return self._metadata
+
     def register_on_progress_callback(self, func: OnProgress):
         """Register a download progress callback function post initialization.
 
         :param callable func:
             A callback function that takes ``stream``, ``chunk``,
              and ``bytes_remaining`` as parameters.
```

### Comparing `pytube-9.7.2/pytube/captions.py` & `pytube-9.7.3/pytube/captions.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/cipher.py` & `pytube-9.7.3/pytube/cipher.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/cli.py` & `pytube-9.7.3/pytube/cli.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/contrib/playlist.py` & `pytube-9.7.3/pytube/contrib/playlist.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/exceptions.py` & `pytube-9.7.3/pytube/exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/extract.py` & `pytube-9.7.3/pytube/extract.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 import logging
 import re
 from collections import OrderedDict
 from datetime import datetime
 from typing import Any
 from typing import Dict
 from typing import List
+from typing import Optional
 from typing import Tuple
 from urllib.parse import parse_qs
 from urllib.parse import parse_qsl
 from urllib.parse import quote
 from urllib.parse import unquote
 from urllib.parse import urlencode
 
 from pytube.cipher import Cipher
 from pytube.exceptions import LiveStreamError
 from pytube.exceptions import RegexMatchError
 from pytube.helpers import regex_search
+from pytube.metadata import YouTubeMetadata
 
 logger = logging.getLogger(__name__)
 
 
 def publish_date(watch_html: str):
     """Extract publish date
     :param str watch_html:
@@ -172,15 +174,15 @@
     "transforms".
 
     :param str html:
         The html contents of the watch page.
     """
     try:
         base_js = get_ytplayer_config(html)['assets']['js']
-    except KeyError:
+    except (KeyError, RegexMatchError):
         base_js = get_ytplayer_js(html)
     return "https://youtube.com" + base_js
 
 
 def mime_type_codec(mime_type_codec: str) -> Tuple[str, List[str]]:
     """Parse the type data.
 
@@ -244,31 +246,31 @@
         The html contents of the watch page.
     :rtype: str
     :returns:
         Substring of the html containing the encoded manifest data.
     """
     logger.debug("finding initial function name")
     config_patterns = [
-        r";ytplayer\.config\s*=\s*({.*?});",
+        r"ytplayer\.config\s*=\s*({.+?});ytplayer",
+        r"ytInitialPlayerResponse\s*=\s*({.+?(?<!gdpr)});"
     ]
     for pattern in config_patterns:
         regex = re.compile(pattern)
         function_match = regex.search(html)
         if function_match:
             logger.debug("finished regex search, matched: %s", pattern)
             yt_player_config = function_match.group(1)
             return json.loads(yt_player_config)
 
     # setConfig() needs to be handled a little differently.
     # We want to parse the entire argument to setConfig()
     #  and use then load that as json to find PLAYER_CONFIG
     #  inside of it.
     setconfig_patterns = [
-        r"yt\.setConfig\((.*'PLAYER_CONFIG':\s*{.+?})\);",
-        r"yt\.setConfig\((.*\"PLAYER_CONFIG\":\s*{.+?})\);"
+        r"yt\.setConfig\((.*['\"]PLAYER_CONFIG['\"]:\s*{.+?})\);"
     ]
     for pattern in setconfig_patterns:
         regex = re.compile(pattern)
         function_match = regex.search(html)
         if function_match:
             logger.debug("finished regex search, matched: %s", pattern)
             yt_config = function_match.group(1)
@@ -346,15 +348,18 @@
 
     """
     otf_type = "FORMAT_STREAM_TYPE_OTF"
 
     if key == "url_encoded_fmt_stream_map" and not stream_data.get(
         "url_encoded_fmt_stream_map"
     ):
-        streaming_data = json.loads(stream_data["player_response"])["streamingData"]
+        if isinstance(stream_data["player_response"], str):
+            streaming_data = json.loads(stream_data["player_response"])["streamingData"]
+        else:
+            streaming_data = stream_data["player_response"]
         formats = []
         if 'formats' in streaming_data.keys():
             formats.extend(streaming_data['formats'])
         if 'adaptiveFormats' in streaming_data.keys():
             formats.extend(streaming_data['adaptiveFormats'])
         try:
             stream_data[key] = [
@@ -392,7 +397,62 @@
     else:
         stream_data[key] = [
             {k: unquote(v) for k, v in parse_qsl(i)}
             for i in stream_data[key].split(",")
         ]
 
     logger.debug("applying descrambler")
+
+
+def initial_data(watch_html: str) -> str:
+    """Extract the ytInitialData json from the watch_html page.
+
+    This mostly contains metadata necessary for rendering the page on-load,
+    such as video information, copyright notices, etc.
+
+    @param watch_html: Html of the watch page
+    @return:
+    """
+    initial_data_pattern = r"window\[['\"]ytInitialData['\"]]\s*=\s*([^\n]+)"
+    try:
+        match = regex_search(initial_data_pattern, watch_html, 1)
+    except RegexMatchError:
+        return "{}"
+    else:
+        return match[:-1]
+
+
+def metadata(initial_data) -> Optional[YouTubeMetadata]:
+    """Get the informational metadata for the video.
+
+    e.g.:
+    [
+        {
+            'Song': '강남스타일(Gangnam Style)',
+            'Artist': 'PSY',
+            'Album': 'PSY SIX RULES Pt.1',
+            'Licensed to YouTube by': 'YG Entertainment Inc. [...]'
+        }
+    ]
+
+    :rtype: YouTubeMetadata
+    """
+    try:
+        metadata_rows: List = initial_data["contents"]["twoColumnWatchNextResults"][
+            "results"]["results"]["contents"][1]["videoSecondaryInfoRenderer"][
+            "metadataRowContainer"]["metadataRowContainerRenderer"]["rows"]
+    except (KeyError, IndexError):
+        # If there's an exception accessing this data, it probably doesn't exist.
+        return YouTubeMetadata([])
+
+    # Rows appear to only have "metadataRowRenderer" or "metadataRowHeaderRenderer"
+    #  and we only care about the former, so we filter the others
+    metadata_rows = filter(
+        lambda x: "metadataRowRenderer" in x.keys(),
+        metadata_rows
+    )
+
+    # We then access the metadataRowRenderer key in each element
+    #  and build a metadata object from this new list
+    metadata_rows = [x["metadataRowRenderer"] for x in metadata_rows]
+
+    return YouTubeMetadata(metadata_rows)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pytube-9.7.2/pytube/helpers.py` & `pytube-9.7.3/pytube/helpers.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/itags.py` & `pytube-9.7.3/pytube/itags.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/monostate.py` & `pytube-9.7.3/pytube/monostate.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/query.py` & `pytube-9.7.3/pytube/query.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube/request.py` & `pytube-9.7.3/pytube/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 logger = logging.getLogger(__name__)
 default_chunk_size = 4096  # 4kb
 default_range_size = 9437184  # 9MB
 
 
 def _execute_request(url, method=None, headers=None):
-    base_headers = {"User-Agent": "Mozilla/5.0"}
+    base_headers = {"User-Agent": "Mozilla/5.0", "accept-language": "en-US,en"}
     if headers:
         base_headers.update(headers)
     if url.lower().startswith("http"):
         request = Request(url, headers=base_headers, method=method)
     else:
         raise ValueError("Invalid URL")
     return urlopen(request)  # nosec
```

### Comparing `pytube-9.7.2/pytube/streams.py` & `pytube-9.7.3/pytube/streams.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/pytube.egg-info/PKG-INFO` & `pytube-9.7.3/pytube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytube
-Version: 9.7.2
+Version: 9.7.3
 Summary: Python 3 library for downloading YouTube Videos.
 Home-page: https://github.com/nficano/pytube
 Author: Nick Ficano, Harold Martin
 Author-email: nficano@gmail.com, harold.martin@gmail.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/nficano/pytube/issues
 Project-URL: Read the Docs, https://python-pytube.readthedocs.io/en/latest
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pytube Version: 9.7.2 Summary: Python 3 library for
+Metadata-Version: 2.1 Name: pytube Version: 9.7.3 Summary: Python 3 library for
 downloading YouTube Videos. Home-page: https://github.com/nficano/pytube
 Author: Nick Ficano, Harold Martin Author-email: nficano@gmail.com,
 harold.martin@gmail.com License: MIT Project-URL: Bug Reports, https://
 github.com/nficano/pytube/issues Project-URL: Read the Docs, https://python-
 pytube.readthedocs.io/en/latest Description: ## (24 JULY 2020) Note: Actively
 soliciting contributers! Ping @ronncc if you would like to help out
                                  [pytube logo]
```

### Comparing `pytube-9.7.2/pytube.egg-info/SOURCES.txt` & `pytube-9.7.3/pytube.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 pytube/captions.py
 pytube/cipher.py
 pytube/cli.py
 pytube/exceptions.py
 pytube/extract.py
 pytube/helpers.py
 pytube/itags.py
+pytube/metadata.py
 pytube/monostate.py
 pytube/query.py
 pytube/request.py
 pytube/streams.py
 pytube/version.py
 pytube.egg-info/PKG-INFO
 pytube.egg-info/SOURCES.txt
@@ -31,11 +32,12 @@
 tests/test_cipher.py
 tests/test_cli.py
 tests/test_exceptions.py
 tests/test_extract.py
 tests/test_helpers.py
 tests/test_itags.py
 tests/test_main.py
+tests/test_metadata.py
 tests/test_query.py
 tests/test_request.py
 tests/test_streams.py
 tests/contrib/test_playlist.py
```

### Comparing `pytube-9.7.2/setup.py` & `pytube-9.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/conftest.py` & `pytube-9.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/contrib/test_playlist.py` & `pytube-9.7.3/tests/contrib/test_playlist.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_captions.py` & `pytube-9.7.3/tests/test_captions.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_cipher.py` & `pytube-9.7.3/tests/test_cipher.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_cli.py` & `pytube-9.7.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_exceptions.py` & `pytube-9.7.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_extract.py` & `pytube-9.7.3/tests/test_extract.py`

 * *Files 6% similar despite different names*

```diff
@@ -98,7 +98,17 @@
         extract.get_ytplayer_js("")
 
 
 def test_signature_cipher_does_not_error(stream_dict):
     config_args = extract.get_ytplayer_config(stream_dict)['args']
     extract.apply_descrambler(config_args, "url_encoded_fmt_stream_map")
     assert "s" in config_args["url_encoded_fmt_stream_map"][0].keys()
+
+
+def test_initial_data_missing():
+    initial_data = extract.initial_data('')
+    assert initial_data == "{}"
+
+
+def test_initial_data(stream_dict):
+    initial_data = extract.initial_data(stream_dict)
+    assert 'contents' in initial_data
```

### Comparing `pytube-9.7.2/tests/test_helpers.py` & `pytube-9.7.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_query.py` & `pytube-9.7.3/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_request.py` & `pytube-9.7.3/tests/test_request.py`

 * *Files identical despite different names*

### Comparing `pytube-9.7.2/tests/test_streams.py` & `pytube-9.7.3/tests/test_streams.py`

 * *Files identical despite different names*

