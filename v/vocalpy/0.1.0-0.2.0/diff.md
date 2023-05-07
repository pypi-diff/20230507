# Comparing `tmp/vocalpy-0.1.0.tar.gz` & `tmp/vocalpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocalpy-0.1.0.tar", last modified: Sat Feb 12 13:28:44 2022, max compression
+gzip compressed data, was "vocalpy-0.2.0.tar", last modified: Sun May  7 21:52:39 2023, max compression
```

## Comparing `vocalpy-0.1.0.tar` & `vocalpy-0.2.0.tar`

### file list

```diff
@@ -1,37 +1,82 @@
--rw-r--r--   0        0        0     1025 2021-02-28 20:59:43.055174 vocalpy-0.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0      281 2022-02-12 13:13:05.148974 vocalpy-0.1.0/.gitignore
--rw-r--r--   0        0        0      642 2022-02-12 13:13:05.148974 vocalpy-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1540 2021-02-28 20:59:43.047175 vocalpy-0.1.0/LICENSE
--rw-r--r--   0        0        0     2064 2021-02-28 20:59:43.043175 vocalpy-0.1.0/Makefile
--rw-r--r--   0        0        0      628 2022-02-12 13:28:27.088579 vocalpy-0.1.0/README.md
--rw-r--r--   0        0        0     2310 2022-02-12 13:13:05.148974 vocalpy-0.1.0/noxfile.py
--rw-r--r--   0        0        0     1304 2022-02-12 13:13:05.148974 vocalpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      142 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/__init__.py
--rw-r--r--   0        0        0       32 2022-02-12 13:28:27.084579 vocalpy-0.1.0/src/vocalpy/annotation/__init__.py
--rw-r--r--   0        0        0       30 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/constants.py
--rw-r--r--   0        0        0        0 2022-01-19 13:41:23.833910 vocalpy-0.1.0/src/vocalpy/converters.py
--rw-r--r--   0        0        0      108 2022-01-19 14:01:57.169852 vocalpy-0.1.0/src/vocalpy/dataclasses/__init__.py
--rw-r--r--   0        0        0     1849 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/dataclasses/audio.py
--rw-r--r--   0        0        0    12407 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/dataclasses/spectrogram.py
--rw-r--r--   0        0        0       29 2022-02-12 13:28:27.084579 vocalpy-0.1.0/src/vocalpy/dataset/__init__.py
--rw-r--r--   0        0        0        0 2022-02-12 13:28:27.080579 vocalpy-0.1.0/src/vocalpy/segmenter.py
--rw-r--r--   0        0        0       27 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/signal/__init__.py
--rw-r--r--   0        0        0     3194 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/signal/spectrogram.py
--rw-r--r--   0        0        0     5478 2022-02-12 13:13:05.148974 vocalpy-0.1.0/src/vocalpy/spect_maker.py
--rw-r--r--   0        0        0      528 2022-01-19 13:41:23.833910 vocalpy-0.1.0/src/vocalpy/validators.py
--rw-r--r--   0        0        0        0 2021-02-28 20:59:43.055174 vocalpy-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0       24 2021-02-28 20:59:43.055174 vocalpy-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/data_for_tests/generated/.gitkeep
--rw-r--r--   0        0        0        0 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/data_for_tests/source/.gitkeep
--rw-r--r--   0        0        0       88 2021-02-28 20:59:43.055174 vocalpy-0.1.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     3290 2021-02-28 20:59:43.055174 vocalpy-0.1.0/tests/fixtures/annot.py
--rw-r--r--   0        0        0     3594 2021-02-28 20:59:43.059174 vocalpy-0.1.0/tests/fixtures/audio.py
--rw-r--r--   0        0        0     5910 2021-02-28 20:59:43.059174 vocalpy-0.1.0/tests/fixtures/spect.py
--rw-r--r--   0        0        0      824 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/fixtures/test_data.py
--rw-r--r--   0        0        0        0 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/test_dataclasses/__init__.py
--rw-r--r--   0        0        0      392 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/test_dataclasses/test_audio.py
--rw-r--r--   0        0        0     2572 2022-02-12 13:13:05.152974 vocalpy-0.1.0/tests/test_dataclasses/test_spectrogram.py
--rw-r--r--   0        0        0        0 2022-02-12 13:28:27.088579 vocalpy-0.1.0/tests/test_signal/__init__.py
--rw-r--r--   0        0        0        0 2022-02-12 13:28:27.088579 vocalpy-0.1.0/tests/test_signal/test_spectrogram.py
--rw-r--r--   0        0        0     1411 2022-02-12 13:28:27.084579 vocalpy-0.1.0/tests/test_spect_maker.py
--rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 vocalpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1307 2023-05-07 21:41:12.898528 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      248 2023-05-07 21:39:43.229568 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      615 2023-05-07 21:39:43.228362 vocalpy-0.2.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      750 2023-05-07 20:16:29.801006 vocalpy-0.2.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      286 2023-04-25 13:42:56.058591 vocalpy-0.2.0/.gitignore
+-rw-r--r--   0        0        0      769 2023-04-25 13:42:56.059258 vocalpy-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      367 2023-05-07 21:38:34.576998 vocalpy-0.2.0/.readthedocs.yaml
+-rw-r--r--   0        0        0     5556 2023-05-07 20:52:52.998672 vocalpy-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1867 2023-05-07 20:53:11.404957 vocalpy-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1540 2023-04-08 15:55:30.246016 vocalpy-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2064 2023-04-08 15:55:30.246197 vocalpy-0.2.0/Makefile
+-rw-r--r--   0        0        0     3341 2023-05-07 20:54:49.402519 vocalpy-0.2.0/README.md
+-rw-r--r--   0        0        0      251 2023-05-07 20:48:44.343584 vocalpy-0.2.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0    29965 2023-05-07 20:41:50.515176 vocalpy-0.2.0/docs/_static/vocalpy-logomark.png
+-rw-r--r--   0        0        0   285798 2023-05-07 20:41:50.763203 vocalpy-0.2.0/docs/_static/vocalpy-primary.png
+-rw-r--r--   0        0        0   194159 2023-05-07 20:41:50.588788 vocalpy-0.2.0/docs/_static/vocalpy-secondary.png
+-rw-r--r--   0        0        0     6436 2023-05-07 21:36:59.006708 vocalpy-0.2.0/noxfile.py
+-rw-r--r--   0        0        0     1447 2023-05-07 21:50:50.220546 vocalpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    19133 2023-04-25 13:43:12.342347 vocalpy-0.2.0/src/scripts/attrs-sqlalchemy.ipynb
+-rw-r--r--   0        0        0     5151 2023-04-25 13:43:12.360555 vocalpy-0.2.0/src/scripts/carpentries-sql-practice.ipynb
+-rw-r--r--   0        0        0    46531 2023-04-25 13:43:12.330739 vocalpy-0.2.0/src/scripts/dataclass-orm.ipynb
+-rw-r--r--   0        0        0    21715 2023-04-25 13:43:12.389389 vocalpy-0.2.0/src/scripts/dataset.ipynb
+-rw-r--r--   0        0        0     3130 2023-05-04 01:22:37.617838 vocalpy-0.2.0/src/scripts/sqlite-python-tutorial.ipynb
+-rw-r--r--   0        0        0    22868 2023-05-07 21:52:26.377951 vocalpy-0.2.0/src/scripts/vocalpy-sqlalchemy-orm.ipynb
+-rw-r--r--   0        0        0      804 2023-05-07 21:50:50.216183 vocalpy-0.2.0/src/vocalpy/__about__.py
+-rw-r--r--   0        0        0     1304 2023-05-07 21:44:06.314669 vocalpy-0.2.0/src/vocalpy/__init__.py
+-rw-r--r--   0        0        0       33 2023-04-25 13:42:56.065849 vocalpy-0.2.0/src/vocalpy/annotation/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-04 01:22:20.075891 vocalpy-0.2.0/src/vocalpy/annotation_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.076056 vocalpy-0.2.0/src/vocalpy/annotator.py
+-rw-r--r--   0        0        0     7738 2023-05-07 21:44:41.309650 vocalpy-0.2.0/src/vocalpy/audio.py
+-rw-r--r--   0        0        0      635 2023-05-04 01:22:20.078518 vocalpy-0.2.0/src/vocalpy/audio_file.py
+-rw-r--r--   0        0        0       30 2023-04-25 13:42:56.066572 vocalpy-0.2.0/src/vocalpy/constants.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.247903 vocalpy-0.2.0/src/vocalpy/converters.py
+-rw-r--r--   0        0        0     4879 2023-05-04 01:22:20.079083 vocalpy-0.2.0/src/vocalpy/dataset.py
+-rw-r--r--   0        0        0     2552 2023-05-07 21:02:40.315808 vocalpy-0.2.0/src/vocalpy/dataset_file.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.079995 vocalpy-0.2.0/src/vocalpy/feature_extractor.py
+-rw-r--r--   0        0        0     1918 2023-05-04 01:22:20.080691 vocalpy-0.2.0/src/vocalpy/feature_file.py
+-rw-r--r--   0        0        0     1118 2023-04-25 13:42:56.072844 vocalpy-0.2.0/src/vocalpy/paths.py
+-rw-r--r--   0        0        0      146 2023-05-07 20:16:29.802759 vocalpy-0.2.0/src/vocalpy/repository/__init__.py
+-rw-r--r--   0        0        0      441 2023-05-07 20:16:29.803288 vocalpy-0.2.0/src/vocalpy/repository/base.py
+-rw-r--r--   0        0        0     3136 2023-05-04 01:22:20.081989 vocalpy-0.2.0/src/vocalpy/repository/orm.py
+-rw-r--r--   0        0        0      677 2023-05-07 20:16:29.803723 vocalpy-0.2.0/src/vocalpy/repository/sqlalchemy.py
+-rw-r--r--   0        0        0     3155 2023-05-07 21:44:06.438381 vocalpy-0.2.0/src/vocalpy/segmenter.py
+-rw-r--r--   0        0        0     2502 2023-05-07 21:44:06.401117 vocalpy-0.2.0/src/vocalpy/sequence.py
+-rw-r--r--   0        0        0      114 2023-05-04 01:22:20.084546 vocalpy-0.2.0/src/vocalpy/signal/__init__.py
+-rw-r--r--   0        0        0     2301 2023-05-07 21:45:30.491360 vocalpy-0.2.0/src/vocalpy/signal/audio.py
+-rw-r--r--   0        0        0     2244 2023-05-04 01:22:20.085058 vocalpy-0.2.0/src/vocalpy/signal/preprocess.py
+-rw-r--r--   0        0        0     3012 2023-05-07 21:45:41.887997 vocalpy-0.2.0/src/vocalpy/signal/segment.py
+-rw-r--r--   0        0        0     3062 2023-05-07 21:07:37.895584 vocalpy-0.2.0/src/vocalpy/signal/spectrogram.py
+-rw-r--r--   0        0        0     7437 2023-05-04 01:22:20.086913 vocalpy-0.2.0/src/vocalpy/spectrogram.py
+-rw-r--r--   0        0        0     1491 2023-05-04 01:22:20.087395 vocalpy-0.2.0/src/vocalpy/spectrogram_file.py
+-rw-r--r--   0        0        0     8358 2023-05-07 21:44:06.512977 vocalpy-0.2.0/src/vocalpy/spectrogram_maker.py
+-rw-r--r--   0        0        0      508 2023-05-04 01:22:20.088654 vocalpy-0.2.0/src/vocalpy/spectrogram_parameters.py
+-rw-r--r--   0        0        0     1565 2023-05-07 21:44:06.416113 vocalpy-0.2.0/src/vocalpy/unit.py
+-rw-r--r--   0        0        0      738 2023-04-25 13:42:56.074584 vocalpy-0.2.0/src/vocalpy/validators.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.249971 vocalpy-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-08 15:55:30.250132 vocalpy-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0      112 2023-04-25 13:42:56.075165 vocalpy-0.2.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2744 2023-04-25 13:42:56.075834 vocalpy-0.2.0/tests/fixtures/annot.py
+-rw-r--r--   0        0        0     4620 2023-04-25 13:42:56.076380 vocalpy-0.2.0/tests/fixtures/audio.py
+-rw-r--r--   0        0        0      834 2023-04-25 13:42:56.076724 vocalpy-0.2.0/tests/fixtures/datasets.py
+-rw-r--r--   0        0        0     6669 2023-05-04 01:22:20.090376 vocalpy-0.2.0/tests/fixtures/spect.py
+-rw-r--r--   0        0        0     1032 2023-04-25 13:42:56.077753 vocalpy-0.2.0/tests/fixtures/test_data.py
+-rw-r--r--   0        0        0     2248 2023-04-25 13:42:56.078328 vocalpy-0.2.0/tests/scripts/generate_data_for_tests.py
+-rw-r--r--   0        0        0     2695 2023-05-04 01:22:20.090889 vocalpy-0.2.0/tests/test_annotation_file.py
+-rw-r--r--   0        0        0     8793 2023-05-07 21:46:44.905812 vocalpy-0.2.0/tests/test_audio.py
+-rw-r--r--   0        0        0      992 2023-05-04 01:22:20.091867 vocalpy-0.2.0/tests/test_audio_file.py
+-rw-r--r--   0        0        0     1605 2023-05-04 01:22:20.092370 vocalpy-0.2.0/tests/test_dataset.py
+-rw-r--r--   0        0        0     2819 2023-05-07 21:46:44.715868 vocalpy-0.2.0/tests/test_paths.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093556 vocalpy-0.2.0/tests/test_repository/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 01:22:20.093841 vocalpy-0.2.0/tests/test_repository/test_repository.py
+-rw-r--r--   0        0        0     2258 2023-05-07 21:46:44.720020 vocalpy-0.2.0/tests/test_segmenter.py
+-rw-r--r--   0        0        0      547 2023-05-07 21:46:44.670223 vocalpy-0.2.0/tests/test_sequence.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252298 vocalpy-0.2.0/tests/test_signal/__init__.py
+-rw-r--r--   0        0        0      314 2023-05-07 20:16:29.809278 vocalpy-0.2.0/tests/test_signal/test_audio.py
+-rw-r--r--   0        0        0      629 2023-05-07 20:16:29.809675 vocalpy-0.2.0/tests/test_signal/test_segment.py
+-rw-r--r--   0        0        0        0 2023-04-08 15:55:30.252385 vocalpy-0.2.0/tests/test_signal/test_spectrogram.py
+-rw-r--r--   0        0        0     4186 2023-05-04 01:22:20.095358 vocalpy-0.2.0/tests/test_spectrogram.py
+-rw-r--r--   0        0        0     1500 2023-05-04 01:22:20.095856 vocalpy-0.2.0/tests/test_spectrogram_file.py
+-rw-r--r--   0        0        0     4476 2023-05-07 21:09:06.876025 vocalpy-0.2.0/tests/test_spectrogram_maker.py
+-rw-r--r--   0        0        0      848 2023-05-07 21:46:44.691384 vocalpy-0.2.0/tests/test_unit.py
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 vocalpy-0.2.0/PKG-INFO
```

### Comparing `vocalpy-0.1.0/LICENSE` & `vocalpy-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vocalpy-0.1.0/Makefile` & `vocalpy-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `vocalpy-0.1.0/pyproject.toml` & `vocalpy-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -3,50 +3,57 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "vocalpy"
 authors = [
     {name = "David Nicholson", email = "nickledave@users.noreply.github.com"}
 ]
-description = "common core package for computational vocal learning research in Python"
-version = "0.1.0"
+description = "Core package for acoustic communication in Python"
+version = "0.2.0"
 classifiers = [
         'License :: OSI Approved :: BSD License',
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: Implementation :: CPython'
 ]
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
-    "attrs >=21.4.0",
-    "crowsetta >=3.2",
+    "attrs >=23.1.0",
+    "crowsetta >=5.0.0",
     "dask >=2.10.1",
     "evfuncs >= 0.3.3",
-    "pandas >=1.3.5",
-    "numpy >=1.18.1",
-    "scipy >=1.4.1",
-    "SoundFile >=0.10.3",
+    "librosa >= 0.10.0.post2",
+    "numpy >=1.21.0",
+    "pandas >= 1.3.5",
+    "scipy >=1.7.0",
+    "SoundFile >=0.12.1",
+    "SQLAlchemy >=2.0.12",
 ]
 
 [project.urls]
 Home = "https://github.com/NickleDave/vocalpy"
 
 [project.optional-dependencies]
 dev = [
     "twine >=3.7.1",
     "black >=21.12b0",
     "ipython >=8.0.0",
     "nox >= 2022.1.7",
+    "vocalpy[doc, test]"
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-cov >=2.11.1",
+    "pytest-xdist >=3.2.0",
 ]
 doc = [
+    "ipython != 8.7.0",
+    "jupyterlab >=3.0.3",
+    "jupytext >=1.13.8",
+    "myst-nb >=0.15.0",
     "sphinx >=4.4.0"
 ]
```

### Comparing `vocalpy-0.1.0/src/vocalpy/signal/spectrogram.py` & `vocalpy-0.2.0/src/vocalpy/signal/spectrogram.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,54 +1,48 @@
 """functions for making spectrograms
 
 filters adapted from SciPy cookbook
 https://scipy-cookbook.readthedocs.io/items/ButterworthBandpass.html
 spectrogram adapted from code by Kyle Kastner and Tim Sainburg
 https://github.com/timsainb/python_spectrograms_and_inversion
 """
+from __future__ import annotations
+
 import numpy as np
 import scipy.signal
 
+from ..audio import Audio
+from ..spectrogram import Spectrogram
 
-__all__ = [
-    'butter_bandpass',
-    'butter_bandpass_filter',
-    'spectrogram'
-]
+__all__ = ["butter_bandpass", "butter_bandpass_filter", "spectrogram"]
 
 
 def butter_bandpass(lowcut, highcut, fs, order=5):
     nyq = 0.5 * fs
     low = lowcut / nyq
     high = highcut / nyq
-    b, a = scipy.signal.butter(order, [low, high], btype='band')
+    b, a = scipy.signal.butter(order, [low, high], btype="band")
     return b, a
 
 
 def butter_bandpass_filter(data, lowcut, highcut, fs, order=5):
     b, a = butter_bandpass(lowcut, highcut, fs, order=order)
     y = scipy.signal.lfilter(b, a, data)
     return y
 
 
-def spectrogram(data,
-                samplerate,
-                fft_size=512,
-                step_size=64,
-                thresh=None,
-                transform_type=None,
-                freq_cutoffs=None):
+def spectrogram(
+    audio: Audio, fft_size: int = 512, step_size: int = 64, thresh=None, transform_type=None, freq_cutoffs=None
+) -> Spectrogram:
     """creates a spectrogram
 
     Parameters
     ----------
-    data : numpy.ndarray
-        audio signal
-    samplerate : int
-        sampling frequency in Hz
+    audio : vocalpy.Audio
+        The audio from which a spectrogram should be generated.
     fft_size : int
         size of window for Fast Fourier transform, number of time bins.
     step_size : int
         step size for Fast Fourier transform
     transform_type : str
         one of {'log_spect', 'log_spect_plus_one'}.
         'log_spect' transforms the spectrogram to log(spectrogram), and
@@ -57,47 +51,44 @@
     thresh: int
         threshold minimum power for log spectrogram
     freq_cutoffs : tuple
         of two elements, lower and higher frequencies.
 
     Return
     ------
-    s : numpy.ndarray
-        spectrogram
-    f : numpy.ndarray
-        vector of centers of time bins from spectrogram
-    t : numpy.ndarray
-        vector of centers of frequency bins from spectrogram
+    spectrogram : vocalpy.Spectrogram
     """
+    if not isinstance(audio, Audio):
+        raise TypeError("`audio` must be a `vocalpy.Audio` instance")
+
     noverlap = fft_size - step_size
 
     if freq_cutoffs:
-        data = butter_bandpass_filter(data,
-                                      freq_cutoffs[0],
-                                      freq_cutoffs[1],
-                                      samplerate)
+        data = butter_bandpass_filter(audio.data, freq_cutoffs[0], freq_cutoffs[1], audio.samplerate)
+    else:
+        data = audio.data
 
-    # below only take [:3] from return of specgram because we don't need the image
-    f, t, s = scipy.signal.spectrogram(data, samplerate, nperseg=fft_size, noverlap=noverlap)
+    f, t, s = scipy.signal.spectrogram(data, audio.samplerate, nperseg=fft_size, noverlap=noverlap)
 
     if transform_type:
-        if transform_type == 'log_spect':
+        if transform_type == "log_spect":
             s /= s.max()  # volume normalize to max 1
             s = np.log10(s)  # take log
             if thresh:
                 # I know this is weird, maintaining 'legacy' behavior
                 s[s < -thresh] = -thresh
-        elif transform_type == 'log_spect_plus_one':
+        elif transform_type == "log_spect_plus_one":
             s = np.log10(s + 1)
             if thresh:
                 s[s < thresh] = thresh
     else:
         if thresh:
             s[s < thresh] = thresh  # set anything less than the threshold as the threshold
 
     if freq_cutoffs:
-        f_inds = np.nonzero((f >= freq_cutoffs[0]) &
-                            (f < freq_cutoffs[1]))[0]  # returns tuple
+        f_inds = np.nonzero((f >= freq_cutoffs[0]) & (f < freq_cutoffs[1]))[0]  # returns tuple
         s = s[f_inds, :]
         f = f[f_inds]
 
-    return s, f, t
+    spect = Spectrogram(data=s, frequencies=f, times=t, source_audio_path=audio.path)
+
+    return spect
```

### Comparing `vocalpy-0.1.0/tests/fixtures/annot.py` & `vocalpy-0.2.0/tests/fixtures/annot.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """fixtures relating to annotation files"""
 import crowsetta
 import pytest
-import toml
+
+from .test_data import SOURCE_TEST_DATA_ROOT
+
+ANNOT_FILE_YARDEN = SOURCE_TEST_DATA_ROOT.joinpath('spect_mat_annot_yarden', 'llb3', 'llb3_annot_subset.mat')
 
 
 @pytest.fixture
-def annot_file_yarden(source_test_data_root):
-    return source_test_data_root.joinpath('spect_mat_annot_yarden', 'llb3', 'llb3_annot_subset.mat')
+def annot_file_yarden():
+    return ANNOT_FILE_YARDEN
 
 
 @pytest.fixture
 def annot_list_yarden(annot_file_yarden):
     scribe = crowsetta.Transcriber(format='yarden')
     annot_list = scribe.from_file(annot_file_yarden)
     return annot_list
@@ -21,51 +24,43 @@
     """labelset as it would be loaded from a toml file
 
     don't return a set because we need to use this to test functions that convert it to a set
     """
     return [str(an_int) for an_int in [1, 2, 3, 6, 7, 8, 9, 10, 11, 12, 13, 14, 16, 17, 18, 19]]
 
 
+ANNOT_DIR_NOTMAT = SOURCE_TEST_DATA_ROOT.joinpath('audio_cbin_annot_notmat', 'gy6or6', '032312')
+
+
 @pytest.fixture
-def annot_dir_notmat(source_test_data_root):
-    return source_test_data_root.joinpath('audio_cbin_annot_notmat',
-                                          'gy6or6',
-                                          '032312')
+def annot_dir_notmat():
+    return ANNOT_DIR_NOTMAT
+
+
+ANNOT_PATHS_LIST_NOTMAT = sorted(ANNOT_DIR_NOTMAT.glob('*.not.mat'))
 
 
 @pytest.fixture
-def annot_files_notmat(annot_dir_notmat):
-    return sorted(annot_dir_notmat.glob('*.not.mat'))
+def annot_paths_list_notmat():
+    return ANNOT_PATHS_LIST_NOTMAT
 
 
 @pytest.fixture
-def annot_list_notmat(annot_files_notmat):
+def annot_list_notmat():
     scribe = crowsetta.Transcriber(format='notmat')
-    annot_list = scribe.from_file(annot_files_notmat)
+    annot_list = scribe.from_file(ANNOT_PATHS_LIST_NOTMAT)
     return annot_list
 
 
-@pytest.fixture
-def labelset_notmat(generated_test_configs_root):
-    """labelset as it would be loaded from a toml file
-
-    don't return a set because we need to use this to test functions that convert it to a set"""
-    a_train_notmat_config = sorted(
-        generated_test_configs_root.glob('*train*notmat*toml')
-    )[0]  # get first config.toml from glob list
-    # doesn't really matter which config, they all have labelset
-    with a_train_notmat_config.open('r') as fp:
-        a_train_notmat_toml = toml.load(fp)
-    labelset = a_train_notmat_toml['PREP']['labelset']
-    return labelset
+ANNOT_FILE_KOUMURA = SOURCE_TEST_DATA_ROOT.joinpath('audio_wav_annot_koumura', 'Bird0', 'Annotation.xml')
 
 
 @pytest.fixture
 def annot_file_koumura(source_test_data_root):
-    return source_test_data_root.joinpath('audio_wav_annot_koumura', 'Bird0', 'Annotation.xml')
+    return ANNOT_FILE_KOUMURA
 
 
 @pytest.fixture
 def annot_list_koumura(annot_file_koumura):
     scribe = crowsetta.Transcriber(format='koumura')
     annot_list = scribe.from_file(annot_file_koumura)
     return annot_list
```

### Comparing `vocalpy-0.1.0/tests/fixtures/audio.py` & `vocalpy-0.2.0/tests/fixtures/audio.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 """fixtures relating to audio files"""
 import pytest
 
+from .test_data import DATA_ROOTS_WITH_SUBDIRS, SOURCE_TEST_DATA_ROOT
+
 
 @pytest.fixture
 def default_spect_params():
     return dict(fft_size=512,
                 step_size=64,
                 freq_cutoffs=(500, 10000),
                 thresh=6.25,
                 transform_type='log_spect',
                 freqbins_key='f',
                 timebins_key='t',
                 spect_key='s'
                 )
 
 
+AUDIO_DIR_CBIN = SOURCE_TEST_DATA_ROOT / 'audio_cbin_annot_notmat' / 'gy6or6' / '032312'
+
+
 @pytest.fixture
 def audio_dir_cbin(source_test_data_root):
-    return source_test_data_root.joinpath('audio_cbin_annot_notmat', 'gy6or6', '032312')
+    return AUDIO_DIR_CBIN
+
+
+AUDIO_LIST_CBIN = sorted(AUDIO_DIR_CBIN.glob('*.cbin'))
 
 
 @pytest.fixture
 def audio_list_cbin(audio_dir_cbin):
-    return sorted(audio_dir_cbin.glob('*.cbin'))
+    return AUDIO_LIST_CBIN
+
+
+@pytest.fixture(params=AUDIO_LIST_CBIN)
+def a_cbin_path(request):
+    return request.param
 
 
 @pytest.fixture
 def audio_list_cbin_all_labels_in_labelset(audio_list_cbin,
                                            annot_list_notmat,
                                            labelset_notmat):
     """list of .cbin audio files where all labels in associated annotation **are** in labelset"""
@@ -57,23 +70,34 @@
         annot = annot[0]
         if not set(annot.seq.labels).issubset(labelset_notmat):
             audio_list_labels_in_labelset.append(audio_path)
 
     return audio_list_labels_in_labelset
 
 
+AUDIO_DIR_WAV =  SOURCE_TEST_DATA_ROOT / 'audio_wav_annot_birdsongrec' / 'Bird0' / 'Wave'
+
+
 # TODO: add .WAV from TIMIT
 @pytest.fixture
 def audio_dir_wav(source_test_data_root):
-    return source_test_data_root.joinpath('audio_wav_annot_koumura', 'Bird0', 'Wave')
+    return AUDIO_DIR_WAV
+
+
+AUDIO_LIST_WAV = sorted(AUDIO_DIR_WAV.glob('*.wav'))
 
 
 @pytest.fixture
 def audio_list_wav(audio_dir_wav):
-    return sorted(audio_dir_wav.glob('*.wav'))
+    return AUDIO_LIST_WAV
+
+
+@pytest.fixture(params=AUDIO_LIST_WAV)
+def a_wav_path(request):
+    return request.param
 
 
 @pytest.fixture
 def specific_audio_dir(audio_dir_cbin,
                        audio_dir_wav):
     """factory fixture, returns a function that
     returns a fixture containing a list of Annotation objects,
@@ -106,7 +130,31 @@
         'wav': audio_list_wav,
     }
 
     def _specific_audio_list(format):
         return FORMAT_AUDIO_LIST_FIXTURE_MAP[format]
 
     return _specific_audio_list
+
+
+AUDIO_DIR_WAV_WITH_SUBDIRS = DATA_ROOTS_WITH_SUBDIRS / 'wav'
+
+AUDIO_LIST_WAV_WITH_SUBDIRS = sorted(AUDIO_DIR_WAV_WITH_SUBDIRS.glob('**/*wav'))
+
+AUDIO_DIR_CBIN_WITH_SUBDIRS = DATA_ROOTS_WITH_SUBDIRS / 'cbin'
+
+AUDIO_LIST_CBIN_WITH_SUBDIRS = sorted(AUDIO_DIR_CBIN_WITH_SUBDIRS.glob('**/*cbin'))
+
+
+ALL_AUDIO_PATHS = (
+    AUDIO_LIST_WAV +
+    AUDIO_LIST_CBIN
+)
+
+@pytest.fixture(params=ALL_AUDIO_PATHS)
+def an_audio_path(request):
+    """Parametrized fixture that returns one audio path
+    from all the audio paths in :mod:`tests.fixtures.audio`.
+
+    Used for testing .e.g. :class:`vocalpy.dataset.AudioFile`.
+    """
+    return request.param
```

### Comparing `vocalpy-0.1.0/tests/fixtures/test_data.py` & `vocalpy-0.2.0/tests/fixtures/test_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 from pathlib import Path
 
 import pytest
 
 HERE = Path(__file__).parent
 
 
+TEST_DATA_ROOT = HERE.joinpath('..', 'data-for-tests')
+
 @pytest.fixture
 def test_data_root():
     """Path that points to root of test_data directory"""
-    return HERE.joinpath('..', 'data_for_tests')
+    return TEST_DATA_ROOT
+
+
+SOURCE_TEST_DATA_ROOT = TEST_DATA_ROOT / 'source'
 
 
 @pytest.fixture
 def source_test_data_root(test_data_root):
     """'source' test data, i.e., files **not** created by ``vocalpy``,
     that is, the input data used when vak does create files (csv files, logs,
     neural network checkpoints, etc.)
     """
-    return test_data_root.joinpath('source')
+    return SOURCE_TEST_DATA_ROOT
+
+
+GENERATED_TEST_DATA_ROOT = TEST_DATA_ROOT / 'generated'
 
 
 @pytest.fixture
 def generated_test_data_root(test_data_root):
     """'generated' test data, i.e., files **not** created by ``vak``, that is,
     the input data used when vak does create files (csv files, logs,
     neural network checkpoints, etc.)
     """
-    return test_data_root.joinpath('generated')
+    return GENERATED_TEST_DATA_ROOT
+
+
+DATA_ROOTS_WITH_SUBDIRS = GENERATED_TEST_DATA_ROOT / 'root_with_subdirs_to_test_paths'
```

