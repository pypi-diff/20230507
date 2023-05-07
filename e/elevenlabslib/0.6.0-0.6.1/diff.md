# Comparing `tmp/elevenlabslib-0.6.0.tar.gz` & `tmp/elevenlabslib-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elevenlabslib-0.6.0.tar", last modified: Sun Apr 30 12:48:16 2023, max compression
+gzip compressed data, was "elevenlabslib-0.6.1.tar", last modified: Sun May  7 11:13:14 2023, max compression
```

## Comparing `elevenlabslib-0.6.0.tar` & `elevenlabslib-0.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.057144 elevenlabslib-0.6.0/
--rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.6.0/LICENSE
--rw-rw-rw-   0        0        0     2705 2023-04-30 12:48:16.055143 elevenlabslib-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.6.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.041143 elevenlabslib-0.6.0/elevenlabslib/
--rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsHistoryItem.py
--rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsSample.py
--rw-rw-rw-   0        0        0    14498 2023-04-30 12:31:41.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsUser.py
--rw-rw-rw-   0        0        0    32952 2023-04-30 12:27:19.000000 elevenlabslib-0.6.0/elevenlabslib/ElevenLabsVoice.py
--rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.6.0/elevenlabslib/__init__.py
--rw-rw-rw-   0        0        0     5592 2023-04-30 12:39:02.000000 elevenlabslib-0.6.0/elevenlabslib/helpers.py
-drwxrwxrwx   0        0        0        0 2023-04-30 12:48:16.054142 elevenlabslib-0.6.0/elevenlabslib.egg-info/
--rw-rw-rw-   0        0        0     2705 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      405 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-30 12:48:16.000000 elevenlabslib-0.6.0/elevenlabslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      855 2023-04-30 12:47:22.000000 elevenlabslib-0.6.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-30 12:48:16.057144 elevenlabslib-0.6.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-17 22:48:32.000000 elevenlabslib-0.6.1/LICENSE
+-rw-rw-rw-   0        0        0     2705 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2050 2023-04-25 20:14:38.000000 elevenlabslib-0.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.184857 elevenlabslib-0.6.1/elevenlabslib/
+-rw-rw-rw-   0        0        0     4534 2023-04-25 19:28:01.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsHistoryItem.py
+-rw-rw-rw-   0        0        0     3021 2023-04-25 18:32:03.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsSample.py
+-rw-rw-rw-   0        0        0    14498 2023-05-06 21:48:53.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsUser.py
+-rw-rw-rw-   0        0        0    33572 2023-05-05 17:09:22.000000 elevenlabslib-0.6.1/elevenlabslib/ElevenLabsVoice.py
+-rw-rw-rw-   0        0        0      533 2023-04-30 12:44:41.000000 elevenlabslib-0.6.1/elevenlabslib/__init__.py
+-rw-rw-rw-   0        0        0     5592 2023-04-30 12:39:02.000000 elevenlabslib-0.6.1/elevenlabslib/helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-07 11:13:14.199857 elevenlabslib-0.6.1/elevenlabslib.egg-info/
+-rw-rw-rw-   0        0        0     2705 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      405 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-07 11:13:14.000000 elevenlabslib-0.6.1/elevenlabslib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      855 2023-05-07 11:12:39.000000 elevenlabslib-0.6.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 11:13:14.200857 elevenlabslib-0.6.1/setup.cfg
```

### Comparing `elevenlabslib-0.6.0/LICENSE` & `elevenlabslib-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/PKG-INFO` & `elevenlabslib-0.6.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.6.0/README.md` & `elevenlabslib-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsHistoryItem.py` & `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsHistoryItem.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsSample.py` & `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsSample.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsUser.py` & `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsUser.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib/ElevenLabsVoice.py` & `elevenlabslib-0.6.1/elevenlabslib/ElevenLabsVoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,39 +218,47 @@
         """
         audioData = self.generate_audio_bytes(prompt, stability, similarity_boost, model_id)
         play_audio_bytes(audioData, playInBackground, portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
         return audioData
 
     def generate_and_stream_audio(self, prompt:str, portaudioDeviceID:Optional[int] = None,
                                   stability:Optional[float]=None, similarity_boost:Optional[float]=None, streamInBackground=False,
-                     onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1"):
+                                  onPlaybackStart:Callable=lambda: None, onPlaybackEnd:Callable=lambda: None, model_id:str="eleven_monolingual_v1", latencyOptimizationLevel:int=0):
         """
 
         Note:
-            No longer suffers from the skipping issues it had in the past.
+            The latencyOptimizationLevel ranges from 0 to 4. Each level trades off some more quality for speed.
+
+            The levels are as follows:
+                - 0: Normal, no optimizations applied
+                - 1: 50% of possible latency optimization
+                - 2: 75% of possible latency optimization
+                - 3: 100% of possible latency optimization
+                - 4: 100% + text normalizer disabled (best latency but can mispronounce numbers/dates)
 
         Generate audio bytes from the given prompt and stream them using sounddevice.
 
         If streamInBackground is true, it will download the audio data in a separate thread, without pausing the main thread.
 
         Parameters:
             streamInBackground (bool): Whether or not to play the audio (and let the download complete) in a separate thread.
             prompt (str): The text prompt to generate audio from.
             portaudioDeviceID (int, optional): The ID of the audio device to use for playback. Defaults to the default output device.
             stability: A float between 0 and 1 representing the stability of the generated audio. If None, the current stability setting is used.
             similarity_boost: A float between 0 and 1 representing the similarity boost of the generated audio. If None, the current similarity boost setting is used.
             onPlaybackStart: Function to call once the playback begins
             onPlaybackEnd: Function to call once the playback ends
             model_id (str): The ID of the TTS model to use for the generation. Defaults to monolingual english.
+            latencyOptimizationLevel (int): The level of latency optimization (0-4) to apply.
 
         """
         payload = self._generate_payload(prompt, stability, similarity_boost, model_id)
         path = "/text-to-speech/" + self._voiceID + "/stream"
 
-        streamedResponse = requests.post(api_endpoint + path, headers=self._linkedUser.headers, json=payload, stream=True)
+        streamedResponse = requests.post(api_endpoint + path, headers=self._linkedUser.headers, json=payload, stream=True, params={"optimize_streaming_latency":latencyOptimizationLevel})
 
         streamer = _AudioChunkStreamer(portaudioDeviceID, onPlaybackStart, onPlaybackEnd)
 
         if streamInBackground:
             mainThread = threading.Thread(target=streamer.begin_streaming, args=(streamedResponse,))
             mainThread.start()
         else:
```

### Comparing `elevenlabslib-0.6.0/elevenlabslib/__init__.py` & `elevenlabslib-0.6.1/elevenlabslib/__init__.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib/helpers.py` & `elevenlabslib-0.6.1/elevenlabslib/helpers.py`

 * *Files identical despite different names*

### Comparing `elevenlabslib-0.6.0/elevenlabslib.egg-info/PKG-INFO` & `elevenlabslib-0.6.1/elevenlabslib.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elevenlabslib
-Version: 0.6.0
+Version: 0.6.1
 Summary: Complete python wrapper for the elevenlabs API
 Author-email: lugia19 <lugia19@lugia19.com>
 Project-URL: Documentation, https://elevenlabslib.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/lugia19/elevenlabslib
 Project-URL: Bug Tracker, https://github.com/lugia19/elevenlabslib
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `elevenlabslib-0.6.0/pyproject.toml` & `elevenlabslib-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0",
             "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elevenlabslib"
-version = "0.6.0"
+version = "0.6.1"
 authors = [
   { name="lugia19", email="lugia19@lugia19.com" },
 ]
 description = "Complete python wrapper for the elevenlabs API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies=[
```

