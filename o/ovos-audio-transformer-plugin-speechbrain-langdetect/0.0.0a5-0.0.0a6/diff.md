# Comparing `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5.tar.gz` & `tmp/ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5.tar", last modified: Sun May  7 02:14:06 2023, max compression
+gzip compressed data, was "ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6.tar", last modified: Sun May  7 02:16:00 2023, max compression
```

## Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5.tar` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:14:06.613095 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:13:59.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:13:59.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 02:14:06.613095 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 02:13:59.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:14:06.613095 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect/
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-07 02:13:59.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:14:01.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:14:06.613095 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:14:06.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:14:06.613095 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-05-07 02:13:59.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:16:00.504147 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:15:52.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:15:52.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 02:16:00.504147 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-07 02:15:52.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:16:00.500147 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-07 02:15:52.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:15:55.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:16:00.504147 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:16:00.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:16:00.504147 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3240 2023-05-07 02:15:52.000000 ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/setup.py
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/LICENSE` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/README.md` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/README.md`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,20 +52,23 @@
 
         probs = self.signal2probs(signal)
         probs = [(k, v) for k, v in probs.items() if k in valid]
         total = sum(p[1] for p in probs) or 1
         probs = [(k, v/total) for k, v in probs]
         lang, prob = max(probs, key=lambda k: k[1])
         LOG.info(f"Detected speech language '{lang}' with probability {prob}")
-        return audio_data, {"stt_lang": lang.split(":")[0], "lang_probability": prob}
+        return audio_data, {"stt_lang": lang.split(":")[0],
+                            "lang_probability": prob,
+                            "lang_predictions": probs}
 
 
 if __name__ == "__main__":
     from speech_recognition import Recognizer, AudioFile
 
     jfk = "/home/miro/PycharmProjects/ovos-stt-plugin-fasterwhisper/jfk.wav"
     with AudioFile(jfk) as source:
         audio = Recognizer().record(source)
 
     s = SpeechBrainLangClassifier()
-    s.transform(audio.get_wav_data())
+    _, ctxt = s.transform(audio.get_wav_data())
+    print(ctxt)
     # {'stt_lang': 'en', 'lang_probability': 0.8076384663581848}
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-audio-transformer-plugin-speechbrain-langdetect
-Version: 0.0.0a5
+Version: 0.0.0a6
 Summary: A speech lang detection plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-audio-transformer-plugin-speechbrain-langdetect
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: ovos plugin
```

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/ovos_audio_transformer_plugin_speechbrain_langdetect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a5/setup.py` & `ovos-audio-transformer-plugin-speechbrain-langdetect-0.0.0a6/setup.py`

 * *Files identical despite different names*

