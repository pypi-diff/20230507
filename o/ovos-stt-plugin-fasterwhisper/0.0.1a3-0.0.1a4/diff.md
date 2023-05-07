# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a3.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a3.tar", last modified: Sun May  7 02:34:30 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a4.tar", last modified: Sun May  7 02:48:59 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:34:25.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.352932 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:48:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # this is needed to read the WAV file properly
-import numpy
-from faster_whisper import WhisperModel
+import numpy as np
+from faster_whisper import WhisperModel, decode_audio
+from ovos_bus_client.session import SessionManager
 from ovos_plugin_manager.templates.stt import STT
 from ovos_plugin_manager.templates.transformers import AudioTransformer
 from ovos_utils.log import LOG
 from speech_recognition import AudioData
 
 
 class FasterWhisperLangClassifier(AudioTransformer):
     def __init__(self, config=None):
         config = config or {}
         super().__init__("ovos-audio-transformer-plugin-fasterwhisper", 10, config)
         model = self.config.get("model")
         if not model:
             model = "small"
+
         assert model in FasterWhisperSTT.MODELS  # TODO - better error handling
 
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
         self.beam_size = self.config.get("beam_size", 5)
 
         if self.use_cuda:
@@ -25,29 +27,54 @@
         else:
             device = "cpu"
         self.engine = WhisperModel(model, device=device, compute_type=self.compute_type)
 
     @staticmethod
     def audiochunk2array(audio_data):
         # Convert buffer to float32 using NumPy
-        audio_as_np_int16 = numpy.frombuffer(audio_data, dtype=numpy.int16)
-        audio_as_np_float32 = audio_as_np_int16.astype(numpy.float32)
+        audio_as_np_int16 = np.frombuffer(audio_data, dtype=np.int16)
+        audio_as_np_float32 = audio_as_np_int16.astype(np.float32)
 
         # Normalise float32 array so that values are between -1.0 and +1.0
         max_int16 = 2 ** 15
         data = audio_as_np_float32 / max_int16
         return data
 
+    def detect(self, audio, valid_langs=None):
+        if not valid_langs:
+            s = SessionManager.get()
+            valid_langs = s.valid_languages
+        valid_langs = [l.lower().split("-")[0] for l in valid_langs]
+
+        if not self.engine.model.is_multilingual:
+            language = "en"
+            language_probability = 1
+        else:
+            sampling_rate = self.engine.feature_extractor.sampling_rate
+
+            if not isinstance(audio, np.ndarray):
+                audio = decode_audio(audio, sampling_rate=sampling_rate)
+
+            features = self.engine.feature_extractor(audio)
+
+            segment = features[:, : self.engine.feature_extractor.nb_max_frames]
+            encoder_output = self.engine.encode(segment)
+            results = self.engine.model.detect_language(encoder_output)[0]
+            results = [(l[2:-2], p) for l, p in results if l[2:-2] in valid_langs]
+            total = sum(l[1] for l in results) or 1
+            results = sorted([(l, p / total) for l, p in results], key=lambda k: k[1], reverse=True)
+
+            language, language_probability = results[0]
+        return language, language_probability
+
     # plugin api
     def transform(self, audio_data):
-        # segments is an iterator, transcription is not done here
-        _, info = self.engine.transcribe(self.audiochunk2array(audio_data), beam_size=self.beam_size,
-                                         condition_on_previous_text=False)
-        LOG.info(f"Detected speech language '{info.language}' with probability {info.language_probability}")
-        return audio_data, {"stt_lang": info.language, "lang_probability": info.language_probability}
+        lang, prob = self.detect(self.audiochunk2array(audio_data))
+        LOG.info(f"Detected speech language '{lang}' with probability {prob}")
+        return audio_data, {"stt_lang": lang, "lang_probability": prob}
 
 
 class FasterWhisperSTT(STT):
     MODELS = ("tiny.en", "tiny", "base.en", "base", "small.en", "small", "medium.en", "medium", "large", "large-v2")
     LANGUAGES = {
         "en": "english",
         "zh": "chinese",
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.py`

 * *Files identical despite different names*

