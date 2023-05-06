# Comparing `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3.tar.gz` & `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3.tar", last modified: Sat May  6 15:30:12 2023, max compression
+gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4.tar", last modified: Sat May  6 22:22:34 2023, max compression
```

## Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3.tar` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:30:12.300483 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-06 15:30:05.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 15:30:05.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 15:30:12.300483 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 15:30:05.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:30:12.300483 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect/
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-06 15:30:05.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 15:30:07.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 15:30:12.300483 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 15:30:12.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 15:30:12.300483 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-05-06 15:30:05.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:22:34.051093 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-06 22:22:21.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-06 22:22:21.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 22:22:34.051093 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-06 22:22:21.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:22:34.051093 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect/
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 2023-05-06 22:22:21.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-06 22:22:28.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:22:34.051093 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-06 22:22:34.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:22:33.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 22:22:34.051093 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-05-06 22:22:21.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/setup.py
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/LICENSE` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/README.md` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# this is needed to read the WAV file properly
 import numpy as np
 import torch
 
-from ovos_plugin_manager.templates.stt import STT
+from ovos_bus_client.session import SessionManager
 from ovos_plugin_manager.templates.transformers import AudioTransformer
 from ovos_utils.log import LOG
 from ovos_utils.xdg_utils import xdg_data_home
 from speechbrain.pretrained import EncoderClassifier
 
 
 class SpeechBrainLangClassifier(AudioTransformer):
@@ -35,30 +34,32 @@
         probs, _, _, _ = self.engine.classify_batch(signal)
         probs = torch.softmax(probs[0], dim=0)
         labels = self.engine.hparams.label_encoder.decode_ndim(range(len(probs)))
         results = {}
         for prob, label in sorted(zip(probs, labels), reverse=True):
             results[label.split(":")[0]] = prob.item()
         return results
-    
+
     # plugin api
     def transform(self, audio_data):
-        # Download Thai language sample from Omniglot and cvert to suitable form
         signal = self.audiochunk2array(audio_data)
-        prediction = self.engine.classify_batch(signal)
-
-        prob = prediction[1].exp()[0].item()
-        lang = prediction[3][0]
 
+        # list of lang codes for this request from bus message/config
+        s = SessionManager.get()
+        valid = [l.split("-")[0] for l in s.valid_languages]
+
+        probs = self.signal2probs(signal)
+        probs = [(k, v) for k, v in probs.items() if k in valid]
+        lang, prob = max(probs, key=lambda k: k[1])
         LOG.info(f"Detected speech language '{lang}' with probability {prob}")
         return audio_data, {"stt_lang": lang.split(":")[0], "lang_probability": prob}
 
 
 if __name__ == "__main__":
-    from speech_recognition import Recognizer, AudioFile, AudioData
+    from speech_recognition import Recognizer, AudioFile
 
     jfk = "/home/miro/PycharmProjects/ovos-stt-plugin-fasterwhisper/jfk.wav"
     with AudioFile(jfk) as source:
         audio = Recognizer().record(source)
 
     s = SpeechBrainLangClassifier()
     s.transform(audio.get_wav_data())
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a3
+Version: 0.0.0a4
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a3/setup.py` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a4/setup.py`

 * *Files identical despite different names*

