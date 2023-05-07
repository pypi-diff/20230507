# Comparing `tmp/shttst-0.0.6.tar.gz` & `tmp/shttst-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shttst-0.0.6.tar", last modified: Wed May  3 08:58:20 2023, max compression
+gzip compressed data, was "shttst-0.0.7.tar", last modified: Sun May  7 14:49:36 2023, max compression
```

## Comparing `shttst-0.0.6.tar` & `shttst-0.0.7.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.849859 shttst-0.0.6/
--rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.6/LICENSE
--rw-rw-rw-   0        0        0      418 2023-05-03 08:58:20.847349 shttst-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.6/README.md
--rw-rw-rw-   0        0        0      582 2023-05-03 08:56:09.000000 shttst-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 08:58:20.849859 shttst-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.475942 shttst-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.509346 shttst-0.0.6/src/shttst/
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.592611 shttst-0.0.6/src/shttst/audio/
--rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.6/src/shttst/audio/__init__.py
--rw-rw-rw-   0        0        0     3124 2023-05-02 14:00:43.000000 shttst-0.0.6/src/shttst/audio/tools.py
--rw-rw-rw-   0        0        0     1133 2023-04-30 12:00:44.000000 shttst-0.0.6/src/shttst/audio/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.633564 shttst-0.0.6/src/shttst/dataset/
--rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.6/src/shttst/dataset/__init__.py
--rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.6/src/shttst/dataset/dataset_files.py
--rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.6/src/shttst/dataset/transcription_line.py
--rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.6/src/shttst/dataset/transcriptions.py
--rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.6/src/shttst/files.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.669444 shttst-0.0.6/src/shttst/models/
--rw-rw-rw-   0        0        0       55 2023-05-01 09:12:33.000000 shttst-0.0.6/src/shttst/models/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-05-02 14:38:55.000000 shttst-0.0.6/src/shttst/models/silero_vad.py
--rw-rw-rw-   0        0        0    19619 2023-05-02 13:23:05.000000 shttst-0.0.6/src/shttst/models/vocal_remover.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.692753 shttst-0.0.6/src/shttst/processing/
--rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.6/src/shttst/processing/__init__.py
--rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.6/src/shttst/processing/audio_to_dataset.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.754754 shttst-0.0.6/src/shttst/recipes/
--rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.6/src/shttst/recipes/__init__.py
--rw-rw-rw-   0        0        0     3338 2023-05-03 08:53:33.000000 shttst-0.0.6/src/shttst/recipes/chomik.py
--rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.6/src/shttst/recipes/multiset.py
--rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.6/src/shttst/recipes/prepare_tts_wavs.py
--rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.6/src/shttst/recipes/transcribe_directory.py
--rw-rw-rw-   0        0        0     1445 2023-05-03 08:50:38.000000 shttst-0.0.6/src/shttst/recipes/yt.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.844357 shttst-0.0.6/src/shttst/text/
--rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.6/src/shttst/text/__init__.py
--rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.6/src/shttst/text/shmart_cleaner.py
--rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.6/src/shttst/text/shmart_nums.py
--rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.6/src/shttst/text/symbols.py
--rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.6/src/shttst/text/text.py
-drwxrwxrwx   0        0        0        0 2023-05-03 08:58:20.553479 shttst-0.0.6/src/shttst.egg-info/
--rw-rw-rw-   0        0        0      418 2023-05-03 08:58:20.000000 shttst-0.0.6/src/shttst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      962 2023-05-03 08:58:20.000000 shttst-0.0.6/src/shttst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 08:58:20.000000 shttst-0.0.6/src/shttst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      119 2023-05-03 08:58:20.000000 shttst-0.0.6/src/shttst.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 08:58:20.000000 shttst-0.0.6/src/shttst.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:36.054608 shttst-0.0.7/
+-rw-rw-rw-   0        0        0     1069 2023-02-03 16:16:35.000000 shttst-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0      418 2023-05-07 14:49:36.053611 shttst-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       48 2023-04-24 20:31:57.000000 shttst-0.0.7/README.md
+-rw-rw-rw-   0        0        0      582 2023-05-07 14:49:12.000000 shttst-0.0.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-07 14:49:36.054608 shttst-0.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.699798 shttst-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.730460 shttst-0.0.7/src/shttst/
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.805442 shttst-0.0.7/src/shttst/audio/
+-rw-rw-rw-   0        0        0       20 2023-04-30 11:58:12.000000 shttst-0.0.7/src/shttst/audio/__init__.py
+-rw-rw-rw-   0        0        0     1510 2023-05-04 10:05:14.000000 shttst-0.0.7/src/shttst/audio/audiomentation.py
+-rw-rw-rw-   0        0        0     3110 2023-05-07 06:02:34.000000 shttst-0.0.7/src/shttst/audio/tools.py
+-rw-rw-rw-   0        0        0     1133 2023-04-30 12:00:44.000000 shttst-0.0.7/src/shttst/audio/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.860175 shttst-0.0.7/src/shttst/dataset/
+-rw-rw-rw-   0        0        0       63 2023-04-27 05:40:53.000000 shttst-0.0.7/src/shttst/dataset/__init__.py
+-rw-rw-rw-   0        0        0     1679 2023-05-03 08:55:12.000000 shttst-0.0.7/src/shttst/dataset/dataset_files.py
+-rw-rw-rw-   0        0        0      471 2023-04-27 06:45:40.000000 shttst-0.0.7/src/shttst/dataset/transcription_line.py
+-rw-rw-rw-   0        0        0      687 2023-04-27 06:23:23.000000 shttst-0.0.7/src/shttst/dataset/transcriptions.py
+-rw-rw-rw-   0        0        0     1553 2023-05-02 14:08:28.000000 shttst-0.0.7/src/shttst/files.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.896241 shttst-0.0.7/src/shttst/models/
+-rw-rw-rw-   0        0        0       55 2023-05-01 09:12:33.000000 shttst-0.0.7/src/shttst/models/__init__.py
+-rw-rw-rw-   0        0        0     2360 2023-05-07 14:47:03.000000 shttst-0.0.7/src/shttst/models/silero_vad.py
+-rw-rw-rw-   0        0        0    19617 2023-05-07 06:02:29.000000 shttst-0.0.7/src/shttst/models/vocal_remover.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.917777 shttst-0.0.7/src/shttst/processing/
+-rw-rw-rw-   0        0        0       31 2023-05-02 13:33:57.000000 shttst-0.0.7/src/shttst/processing/__init__.py
+-rw-rw-rw-   0        0        0     2125 2023-05-02 14:36:45.000000 shttst-0.0.7/src/shttst/processing/audio_to_dataset.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.984777 shttst-0.0.7/src/shttst/recipes/
+-rw-rw-rw-   0        0        0        0 2023-05-01 09:52:26.000000 shttst-0.0.7/src/shttst/recipes/__init__.py
+-rw-rw-rw-   0        0        0     3901 2023-05-07 07:35:41.000000 shttst-0.0.7/src/shttst/recipes/chomik.py
+-rw-rw-rw-   0        0        0     1126 2023-05-02 13:26:12.000000 shttst-0.0.7/src/shttst/recipes/multiset.py
+-rw-rw-rw-   0        0        0      922 2023-04-30 08:00:20.000000 shttst-0.0.7/src/shttst/recipes/prepare_tts_wavs.py
+-rw-rw-rw-   0        0        0     2211 2023-05-02 09:25:02.000000 shttst-0.0.7/src/shttst/recipes/transcribe_directory.py
+-rw-rw-rw-   0        0        0     1445 2023-05-03 08:50:38.000000 shttst-0.0.7/src/shttst/recipes/yt.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:36.051519 shttst-0.0.7/src/shttst/text/
+-rw-rw-rw-   0        0        0       98 2023-04-25 09:35:07.000000 shttst-0.0.7/src/shttst/text/__init__.py
+-rw-rw-rw-   0        0        0    13863 2023-04-25 09:44:50.000000 shttst-0.0.7/src/shttst/text/shmart_cleaner.py
+-rw-rw-rw-   0        0        0     3637 2023-04-24 20:27:02.000000 shttst-0.0.7/src/shttst/text/shmart_nums.py
+-rw-rw-rw-   0        0        0      171 2023-04-24 20:19:31.000000 shttst-0.0.7/src/shttst/text/symbols.py
+-rw-rw-rw-   0        0        0      782 2023-04-25 09:35:28.000000 shttst-0.0.7/src/shttst/text/text.py
+drwxrwxrwx   0        0        0        0 2023-05-07 14:49:35.760250 shttst-0.0.7/src/shttst.egg-info/
+-rw-rw-rw-   0        0        0      418 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      997 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      119 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-07 14:49:35.000000 shttst-0.0.7/src/shttst.egg-info/top_level.txt
```

### Comparing `shttst-0.0.6/LICENSE` & `shttst-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/pyproject.toml` & `shttst-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "shttst"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Shmart", email="szprytnyd@gmail.com" },
 ]
 description = "Shmart TTS tools."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `shttst-0.0.6/src/shttst/audio/tools.py` & `shttst-0.0.7/src/shttst/audio/tools.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     if type == 'classifier':
         model = TortoiseAudioClassifier()
     elif type == 'denoiser':
         model = ShmartVocalRemover()
     elif type == 'titanet':
         from nemo.collections.asr.models import EncDecSpeakerLabelModel
         model = EncDecSpeakerLabelModel.from_pretrained("nvidia/speakerverification_en_titanet_large", map_location='cpu')
-        model.eval()
+        model.cuda().eval()
     elif type == 'resemblyzer':
         from resemblyzer import VoiceEncoder
-        model = VoiceEncoder('cpu', verbose=False)
+        model = VoiceEncoder('cuda', verbose=False)
         model.eval()
     elif type == 'vad':
         model = ShmartSileroVad()
     elif type == 'whisper':
         from faster_whisper import WhisperModel
         model_path = huggingface_hub.snapshot_download("shmart/shmisper-medium-PL")
         model = WhisperModel(model_path, device="cuda", compute_type="float16")
@@ -44,28 +44,28 @@
     return model(file_path)
 
 def split_by_vad(file_path: str, max_duration: int, min_silence: int) -> str:
     model: ShmartSileroVad = get_model('vad')
     return model.vad_process(file_path, min_silence_duration=min_silence, desired_max_speech_duration=max_duration)
 
 def clean_audio_noise(file_path: str) -> str:
-    model: ShmartVocalRemover = get_model('denoiser')
-    vocals, instruments = model(file_path)
+    vr_model: ShmartVocalRemover = get_model('denoiser')
+    vocals, instruments = vr_model(file_path, tta=True)
     save_audio(file_path, vocals)
 
 def get_custom_embedding(file_path, type='titanet'):
     if type == 'titanet':
         from nemo.collections.asr.models import EncDecSpeakerLabelModel
         titanet_model: EncDecSpeakerLabelModel = get_model(type)
-        return titanet_model.get_embedding(file_path).tolist()
+        return titanet_model.get_embedding(file_path).squeeze(0).cpu()
     elif type == 'resemblyzer':
         from resemblyzer import VoiceEncoder, preprocess_wav
         wav = preprocess_wav(file_path)
         resemblyzer_model: VoiceEncoder = get_model(type)
-        return torch.from_numpy(resemblyzer_model.embed_utterance(wav)).tolist()
+        return torch.from_numpy(resemblyzer_model.embed_utterance(wav))
 
 def get_transcription(audio_path, options={
     'language': "pl",
     'beam_size': 5,
     'without_timestamps': True,
     'suppress_tokens': [],
     'log_prob_threshold': None,
@@ -76,8 +76,8 @@
     result, info = model.transcribe(audio_path, **options)
     try:
       return ' '.join([r.text for r in result]), info.duration
     except:
       return '', -1
     
 if __name__ == '__main__':
-    clean_audio_noise('\\content\\todo\\jzd\\wavs\\Jeden z dziesięciu edycja 136., odcinek 5_7.wav')
+    get_custom_embedding('\\content\\cyber\\2077\\wavs\\55.wav')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shttst-0.0.6/src/shttst/audio/utils.py` & `shttst-0.0.7/src/shttst/audio/utils.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/dataset/dataset_files.py` & `shttst-0.0.7/src/shttst/dataset/dataset_files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/dataset/transcriptions.py` & `shttst-0.0.7/src/shttst/dataset/transcriptions.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/files.py` & `shttst-0.0.7/src/shttst/files.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/models/silero_vad.py` & `shttst-0.0.7/src/shttst/models/silero_vad.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,17 @@
                                 onnx=False)
         self.vad_model = vad_model
         self.get_speech_timestamps = utils[0]
         self.read_audio = utils[2]
 
     def vad_process(self, audio_file, min_silence_duration = 200, initial_max_speech_duration=30, desired_max_speech_duration=14):
         with torch.no_grad():
-            wav = self.read_audio(audio_file, sampling_rate=16000)
+            audio_to_split = self.read_audio(audio_file, sampling_rate=16000)
             timestamps = self.get_speech_timestamps(
-                wav,
+                audio_to_split,
                 self.vad_model,
                 0.90,  # speech prob threshold
                 16000,  # sample rate
                 800,  # min speech duration in ms
                 initial_max_speech_duration,  # max speech duration in seconds
                 min_silence_duration,  # min silence duration
                 512,  # window size
```

### Comparing `shttst-0.0.6/src/shttst/models/vocal_remover.py` & `shttst-0.0.7/src/shttst/models/vocal_remover.py`

 * *Files 0% similar despite different names*

```diff
@@ -561,15 +561,15 @@
         model = CascadedNet(2048, 32, 128)
         model.load_state_dict(torch.load(get_checkpoint(), map_location='cpu'))
         model.to(self.device)
 
         self.model = model
         self.sp = Separator(self.model, self.device, 1, crop_size, post_process)
 
-    def __call__(self, wav_path, tta = False, hop_length=1024, sr=22050):
+    def __call__(self, wav_path, tta=False, hop_length=1024, sr=22050):
         X, sr = librosa.load(wav_path, sr=sr, mono=False, dtype=np.float32, res_type='kaiser_fast')
 
         if X.ndim == 1:
             X = np.asarray([X, X])
 
         X_spec = wave_to_spectrogram(X, hop_length, 2048)
```

### Comparing `shttst-0.0.6/src/shttst/processing/audio_to_dataset.py` & `shttst-0.0.7/src/shttst/processing/audio_to_dataset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/recipes/chomik.py` & `shttst-0.0.7/src/shttst/recipes/chomik.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,35 +3,38 @@
 import re
 from bs4 import BeautifulSoup
 from shttst.processing.audio_to_dataset import AudioToDatasetProcessor
 
 def unique_list(array):
     return list(set(array))
 
-def download_mp3(id, out_dir='/content/chomik/wavs') -> str:
+def download_mp3(id, out_dir='/content/chomik') -> str:
     try:
         os.makedirs(out_dir, exist_ok=True)
         MP3_URL = f"https://chomikuj.pl/Audio.ashx?id={id}&type=2&tp=mp3"
         resp = requests.get(MP3_URL)
 
         file_path = os.path.join(out_dir, f'{id}.mp3')
         with open(file_path, 'w+b') as fs:
             fs.write(resp.content)
 
         return file_path
     except Exception as e:
         print(e)
         return None
 
-def get_all_dirs(url):
+def get_all_dirs(url, only_sub_url=True):
     resp = requests.get(url)
     soup = BeautifulSoup(resp.content, "html.parser")
     results = soup.find(id="TreeContainer")
     results = results.find_all('a')
-    return unique_list([f"https://chomikuj.pl{r['href']}" for r in results])
+    results = unique_list([f"https://chomikuj.pl{r['href']}" for r in results])
+    if only_sub_url:
+        results = list(filter(lambda x: x.startswith(url), results))
+    return results
 
 def get_dir_pages(url):
     resp = requests.get(url)
     soup = BeautifulSoup(resp.content, "html.parser")
 
     number_of_pages = 1
     result = soup.find(id="galleryView")
@@ -57,40 +60,54 @@
     if result:
         audios = result.find_all('a', class_='downloadAction')
         
         return(unique_list([re.search(r'\d{10}', r['href']).group() for r in audios if '.mp3' in r['href']]))
     
     return []
 
-def download_chomik_dir(url: str, out_dir='/content/chomik/wavs'):
+def get_folder_id(url) -> str:
+    resp = requests.get(url)
+    soup = BeautifulSoup(resp.content, "html.parser")
+    return soup.find('input', {'name': 'folderId'}).attrs['value']
+
+def download_chomik_dir(url: str, out_dir='/content/chomik'):
+    folder_id = get_folder_id(url)
     max_pages = get_dir_pages(url)
     for i in range(max_pages):
         mp3s = get_page_mp3s(f'{url},{i+1}')
         for mp3 in mp3s:
-            download_mp3(mp3, out_dir)
+            download_mp3(mp3, os.path.join(out_dir, folder_id, 'wavs'))
 
-def download_all_chomik_dirs(url: str, out_dir='/content/chomik/wavs'):
+def download_all_chomik_dirs(url: str, out_dir='/content/chomik'):
     chomik_dirs = get_all_dirs(url)
     for dir in chomik_dirs:
         download_chomik_dir(dir, out_dir)
 
-def create_dataset_from_chomik_dir(url: str, keep_not_fine=False, denoise_all=False, use_classifier=True, out_dir='/content/chomik/wavs', vad_min_silence=1000, vad_max_duration=14):
+def create_dataset_from_chomik_dir(url: str, keep_not_fine=False, denoise_all=False, use_classifier=True, out_dir='/content/chomik', vad_min_silence=1000, vad_max_duration=14, total_size_per_dir=1024 * 1024 * 50):
+    folder_id = get_folder_id(url)
+    book_dir = os.path.join(out_dir, folder_id)
+    if os.path.exists(book_dir):
+        return
+    
     processor = AudioToDatasetProcessor(keep_not_fine, denoise_all, use_classifier)
     mp3s = get_page_mp3s(url)
+    total_size = 0
     for mp3 in mp3s:
-        path = download_mp3(mp3, out_dir)
+        if total_size >= total_size_per_dir:
+            break
+        path = download_mp3(mp3, os.path.join(book_dir, 'wavs'))
+        total_size += os.path.getsize(path)
         if path:
             processor(path, vad_min_silence=vad_min_silence, vad_max_duration=vad_max_duration)
         
 
 
 if __name__ == '__main__':
     # URL = "https://chomikuj.pl/JuRiWlO/Audiobooki/"
-    # download_all_chomik_dirs(URL)
-
-    URL = "https://chomikuj.pl/piotrbobisz/!Ostatnio+Dodane!/Audiobooki/Adam+Ferency*2c+Maja+Jaszewska/Nie+i+tak.+Adam+Ferency+w+rozmowie+z+Maj*c4*85+Jaszewsk*c4*85+(Czyta+Maja+Jaszewska)"
-    create_dataset_from_chomik_dir(URL, use_classifier=False)
+    URL = 'https://chomikuj.pl/piotrbobisz/!Ostatnio+Dodane!/Audiobooki'
+    for dir in get_all_dirs(URL):
+        create_dataset_from_chomik_dir(dir)
```

### Comparing `shttst-0.0.6/src/shttst/recipes/multiset.py` & `shttst-0.0.7/src/shttst/recipes/multiset.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/recipes/prepare_tts_wavs.py` & `shttst-0.0.7/src/shttst/recipes/prepare_tts_wavs.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/recipes/transcribe_directory.py` & `shttst-0.0.7/src/shttst/recipes/transcribe_directory.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/recipes/yt.py` & `shttst-0.0.7/src/shttst/recipes/yt.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/text/shmart_cleaner.py` & `shttst-0.0.7/src/shttst/text/shmart_cleaner.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/text/shmart_nums.py` & `shttst-0.0.7/src/shttst/text/shmart_nums.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst/text/text.py` & `shttst-0.0.7/src/shttst/text/text.py`

 * *Files identical despite different names*

### Comparing `shttst-0.0.6/src/shttst.egg-info/SOURCES.txt` & `shttst-0.0.7/src/shttst.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 src/shttst/files.py
 src/shttst.egg-info/PKG-INFO
 src/shttst.egg-info/SOURCES.txt
 src/shttst.egg-info/dependency_links.txt
 src/shttst.egg-info/requires.txt
 src/shttst.egg-info/top_level.txt
 src/shttst/audio/__init__.py
+src/shttst/audio/audiomentation.py
 src/shttst/audio/tools.py
 src/shttst/audio/utils.py
 src/shttst/dataset/__init__.py
 src/shttst/dataset/dataset_files.py
 src/shttst/dataset/transcription_line.py
 src/shttst/dataset/transcriptions.py
 src/shttst/models/__init__.py
```

