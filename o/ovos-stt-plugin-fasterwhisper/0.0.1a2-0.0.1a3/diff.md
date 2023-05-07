# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a2.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a2.tar", last modified: Thu May  4 14:16:10 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a3.tar", last modified: Sun May  7 02:34:30 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     7104 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 14:16:03.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:09.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:16:10.023252 ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-04 14:16:00.000000 ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:34:25.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:34:30.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:34:30.810165 ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-07 02:34:19.000000 ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/README.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 class FasterWhisperLangClassifier(AudioTransformer):
     def __init__(self, config=None):
         config = config or {}
         super().__init__("ovos-audio-transformer-plugin-fasterwhisper", 10, config)
         model = self.config.get("model")
         if not model:
-            model = "small.en"
+            model = "small"
         assert model in FasterWhisperSTT.MODELS  # TODO - better error handling
 
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
         self.beam_size = self.config.get("beam_size", 5)
 
         if self.use_cuda:
@@ -36,15 +36,16 @@
         max_int16 = 2 ** 15
         data = audio_as_np_float32 / max_int16
         return data
 
     # plugin api
     def transform(self, audio_data):
         # segments is an iterator, transcription is not done here
-        _, info = self.engine.transcribe(self.audiochunk2array(audio_data), beam_size=self.beam_size)
+        _, info = self.engine.transcribe(self.audiochunk2array(audio_data), beam_size=self.beam_size,
+                                         condition_on_previous_text=False)
         LOG.info(f"Detected speech language '{info.language}' with probability {info.language_probability}")
         return audio_data, {"stt_lang": info.language, "lang_probability": info.language_probability}
 
 
 class FasterWhisperSTT(STT):
     MODELS = ("tiny.en", "tiny", "base.en", "base", "small.en", "small", "medium.en", "medium", "large", "large-v2")
     LANGUAGES = {
@@ -149,15 +150,15 @@
         "su": "sundanese",
     }
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         model = self.config.get("model")
         if not model:
-            model = "small.en"
+            model = "small"
         assert model in self.MODELS  # TODO - better error handling
 
         self.beam_size = self.config.get("beam_size", 5)
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
 
         if self.use_cuda:
@@ -168,15 +169,17 @@
 
     @staticmethod
     def audiodata2array(audio_data):
         assert isinstance(audio_data, AudioData)
         return FasterWhisperLangClassifier.audiochunk2array(audio_data.get_wav_data())
 
     def execute(self, audio, language=None):
-        segments, _ = self.engine.transcribe(self.audiodata2array(audio), beam_size=self.beam_size)
+        lang = language or self.lang
+        segments, _ = self.engine.transcribe(self.audiodata2array(audio), beam_size=self.beam_size,
+                                             condition_on_previous_text=False, language=lang.split("-")[0].lower())
         # segments is an iterator, transcription only happens here
         transcription = "".join(segment.text for segment in segments).strip()
         return transcription
 
     @property
     def available_languages(self) -> set:
         return set(FasterWhisperSTT.LANGUAGES.keys())
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a2/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a3/setup.py`

 * *Files identical despite different names*

