# Comparing `tmp/tuneflow-py-0.7.0.tar.gz` & `tmp/tuneflow-py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuneflow-py-0.7.0.tar", last modified: Sat Apr 29 04:12:50 2023, max compression
+gzip compressed data, was "tuneflow-py-0.7.1.tar", last modified: Sun May  7 06:23:45 2023, max compression
```

## Comparing `tuneflow-py-0.7.0.tar` & `tuneflow-py-0.7.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.7.0/LICENSE
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.7.0/README.md
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-04-29 04:12:20.000000 tuneflow-py-0.7.0/pyproject.toml
--rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/setup.cfg
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/__init__.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.7.0/src/tuneflow_py/base_plugin.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/
--rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/clip_descriptor.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/common.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4221 2023-03-30 21:53:07.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/param.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/text.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.7.0/src/tuneflow_py/descriptors/widget.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py/models/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/audio_plugin.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/note.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/src/tuneflow_py/models/protos/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/protos/song_pb2.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/tempo.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/time_signature.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/src/tuneflow_py/models/track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.7.0/src/tuneflow_py/utils.py
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.140665 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/
--rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/PKG-INFO
--rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/SOURCES.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/dependency_links.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/requires.txt
--rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-04-29 04:12:50.000000 tuneflow-py-0.7.0/src/tuneflow_py.egg-info/top_level.txt
-drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-04-29 04:12:50.150665 tuneflow-py-0.7.0/test/
--rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.7.0/test/test_audio_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.7.0/test/test_automation.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/test/test_lyric.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.7.0/test/test_marker.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.7.0/test/test_midi_clip.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.7.0/test/test_note.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.7.0/test/test_song.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.7.0/test/test_track.py
--rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.7.0/test/test_utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1065 2023-01-10 14:03:44.000000 tuneflow-py-0.7.1/LICENSE
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3809 2023-03-06 23:39:23.000000 tuneflow-py-0.7.1/README.md
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1288 2023-05-07 06:20:30.000000 tuneflow-py-0.7.1/pyproject.toml
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       38 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/setup.cfg
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/tuneflow_py/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1221 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/src/tuneflow_py/__init__.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1987 2023-02-28 00:04:43.000000 tuneflow-py-0.7.1/src/tuneflow_py/base_plugin.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      922 2023-03-30 21:40:36.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1857 2023-04-16 06:53:45.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/clip_descriptor.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      439 2023-03-30 21:53:05.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/common.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4270 2023-05-07 06:17:30.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/param.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4407 2023-03-30 21:53:10.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       71 2023-03-30 21:53:12.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/text.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5575 2023-03-31 22:25:01.000000 tuneflow-py-0.7.1/src/tuneflow_py/descriptors/widget.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/tuneflow_py/models/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     3128 2023-03-01 03:02:02.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/audio_plugin.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17158 2023-03-31 07:33:41.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33694 2023-04-16 21:13:50.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    17149 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1305 2023-04-10 18:15:27.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5275 2023-02-22 00:50:28.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/note.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/tuneflow_py/models/protos/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    76828 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/protos/song_pb2.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    25653 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)      873 2023-03-01 22:09:14.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/tempo.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1093 2023-02-22 00:28:50.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/time_signature.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16703 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/src/tuneflow_py/models/track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     6210 2023-03-29 01:48:05.000000 tuneflow-py-0.7.1/src/tuneflow_py/utils.py
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     4581 2023-05-07 06:23:45.000000 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/PKG-INFO
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     1164 2023-05-07 06:23:45.000000 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/SOURCES.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)        1 2023-05-07 06:23:45.000000 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/dependency_links.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       96 2023-05-07 06:23:45.000000 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/requires.txt
+-rw-r--r--   0 panacea   (1000) panacea   (1000)       12 2023-05-07 06:23:45.000000 tuneflow-py-0.7.1/src/tuneflow_py.egg-info/top_level.txt
+drwxr-xr-x   0 panacea   (1000) panacea   (1000)        0 2023-05-07 06:23:45.267295 tuneflow-py-0.7.1/test/
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    26849 2023-04-16 07:54:00.000000 tuneflow-py-0.7.1/test/test_audio_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24170 2023-03-31 07:02:16.000000 tuneflow-py-0.7.1/test/test_automation.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    16632 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/test/test_lyric.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     8001 2023-04-10 18:37:18.000000 tuneflow-py-0.7.1/test/test_marker.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    33568 2023-03-09 18:17:16.000000 tuneflow-py-0.7.1/test/test_midi_clip.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    24300 2023-02-22 00:33:25.000000 tuneflow-py-0.7.1/test/test_note.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)    14091 2023-03-31 16:54:59.000000 tuneflow-py-0.7.1/test/test_song.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     5693 2023-04-29 04:10:56.000000 tuneflow-py-0.7.1/test/test_track.py
+-rw-r--r--   0 panacea   (1000) panacea   (1000)     2071 2023-02-16 23:10:13.000000 tuneflow-py-0.7.1/test/test_utils.py
```

### Comparing `tuneflow-py-0.7.0/LICENSE` & `tuneflow-py-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/PKG-INFO` & `tuneflow-py-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.7.0/README.md` & `tuneflow-py-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/pyproject.toml` & `tuneflow-py-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "tuneflow-py"
-version = "0.7.0"
+version = "0.7.1"
 authors = [{ name = "TuneFlow", email = "contact@info.tuneflow.com" }]
 description = "Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = [
   "AI",
   "music",
```

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/__init__.py` & `tuneflow-py-0.7.1/src/tuneflow_py/__init__.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/base_plugin.py` & `tuneflow-py-0.7.1/src/tuneflow_py/base_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/audio_plugin_descriptor.py` & `tuneflow-py-0.7.1/src/tuneflow_py/descriptors/audio_plugin_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/clip_descriptor.py` & `tuneflow-py-0.7.1/src/tuneflow_py/descriptors/clip_descriptor.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/param.py` & `tuneflow-py-0.7.1/src/tuneflow_py/descriptors/param.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
     TickAtPlayheadSnappedToBeat = 6
     ''' A number that represents the start tick of the beat where the playhead is at. '''
 
     ClipAudioData = 7
     ''' A list of `AudioData` for specified clips. '''
 
+    Language = 8
+    ''' The user language. '''
+
 
 class ParamDescriptor(TypedDict):
     '''
     Definition of the config for a single param.
 
     Note that the members here use camel case to be
     consistent with the typescript plugins.
```

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/plugin.py` & `tuneflow-py-0.7.1/src/tuneflow_py/descriptors/plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/descriptors/widget.py` & `tuneflow-py-0.7.1/src/tuneflow_py/descriptors/widget.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/audio_plugin.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/audio_plugin.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/automation.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/clip.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/lyric.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/marker.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/note.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/protos/song_pb2.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/protos/song_pb2.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/song.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/tempo.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/tempo.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/time_signature.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/time_signature.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/models/track.py` & `tuneflow-py-0.7.1/src/tuneflow_py/models/track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py/utils.py` & `tuneflow-py-0.7.1/src/tuneflow_py/utils.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py.egg-info/PKG-INFO` & `tuneflow-py-0.7.1/src/tuneflow_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuneflow-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Implement your music models and algorithms directly in TuneFlow - The next-gen DAW for the AI era
 Author-email: TuneFlow <contact@info.tuneflow.com>
 Project-URL: Homepage, https://github.com/tuneflow/tuneflow-py
 Project-URL: Bug Tracker, https://github.com/tuneflow/tuneflow-py/issues
 Keywords: AI,music,DAW,TuneFlow,composition,songwriting,music production,music generation,music transcription,mixing,music theory,music information retrieval,MIR,music analysis,song analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tuneflow-py-0.7.0/src/tuneflow_py.egg-info/SOURCES.txt` & `tuneflow-py-0.7.1/src/tuneflow_py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_audio_clip.py` & `tuneflow-py-0.7.1/test/test_audio_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_automation.py` & `tuneflow-py-0.7.1/test/test_automation.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_lyric.py` & `tuneflow-py-0.7.1/test/test_lyric.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_marker.py` & `tuneflow-py-0.7.1/test/test_marker.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_midi_clip.py` & `tuneflow-py-0.7.1/test/test_midi_clip.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_note.py` & `tuneflow-py-0.7.1/test/test_note.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_song.py` & `tuneflow-py-0.7.1/test/test_song.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_track.py` & `tuneflow-py-0.7.1/test/test_track.py`

 * *Files identical despite different names*

### Comparing `tuneflow-py-0.7.0/test/test_utils.py` & `tuneflow-py-0.7.1/test/test_utils.py`

 * *Files identical despite different names*

