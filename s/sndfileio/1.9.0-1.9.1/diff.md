# Comparing `tmp/sndfileio-1.9.0.tar.gz` & `tmp/sndfileio-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sndfileio-1.9.0.tar", last modified: Sun Jul  3 09:34:57 2022, max compression
+gzip compressed data, was "sndfileio-1.9.1.tar", last modified: Sun May  7 11:06:33 2023, max compression
```

## Comparing `sndfileio-1.9.0.tar` & `sndfileio-1.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-07-03 09:34:57.848541 sndfileio-1.9.0/
--rw-rw-r--   0 em        (1000) em        (1000)     1060 2021-11-13 21:40:24.000000 sndfileio-1.9.0/LICENSE.md
--rw-rw-r--   0 em        (1000) em        (1000)       25 2021-11-13 21:40:24.000000 sndfileio-1.9.0/MANIFEST.in
--rw-rw-r--   0 em        (1000) em        (1000)     2249 2022-07-03 09:34:57.847540 sndfileio-1.9.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     1933 2022-03-07 08:14:11.000000 sndfileio-1.9.0/README.rst
--rw-rw-r--   0 em        (1000) em        (1000)       38 2022-07-03 09:34:57.848541 sndfileio-1.9.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)     1011 2022-07-03 09:34:39.000000 sndfileio-1.9.0/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-07-03 09:34:57.846541 sndfileio-1.9.0/sndfileio/
--rwxrwxr-x   0 em        (1000) em        (1000)     2413 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     1796 2022-03-07 08:16:05.000000 sndfileio-1.9.0/sndfileio/backend_lameenc.py
--rw-rw-r--   0 em        (1000) em        (1000)     3041 2022-07-03 09:12:18.000000 sndfileio-1.9.0/sndfileio/backend_miniaudio.py
--rw-rw-r--   0 em        (1000) em        (1000)     4862 2022-07-03 09:30:45.000000 sndfileio-1.9.0/sndfileio/datastructs.py
--rwxrwxr-x   0 em        (1000) em        (1000)     4796 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/dsp.py
--rw-rw-r--   0 em        (1000) em        (1000)     1170 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/mp3.py
--rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/py.typed
--rwxrwxr-x   0 em        (1000) em        (1000)     7639 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/resampling.py
--rwxrwxr-x   0 em        (1000) em        (1000)    34835 2022-07-03 09:31:26.000000 sndfileio-1.9.0/sndfileio/sndfileio.py
--rwxrwxr-x   0 em        (1000) em        (1000)      585 2021-11-13 21:40:24.000000 sndfileio-1.9.0/sndfileio/testing.py
--rwxrwxr-x   0 em        (1000) em        (1000)     9967 2022-07-03 09:12:18.000000 sndfileio-1.9.0/sndfileio/util.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2022-07-03 09:34:57.847540 sndfileio-1.9.0/sndfileio.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)     2249 2022-07-03 09:34:57.000000 sndfileio-1.9.0/sndfileio.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      452 2022-07-03 09:34:57.000000 sndfileio-1.9.0/sndfileio.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2022-07-03 09:34:57.000000 sndfileio-1.9.0/sndfileio.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       86 2022-07-03 09:34:57.000000 sndfileio-1.9.0/sndfileio.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       10 2022-07-03 09:34:57.000000 sndfileio-1.9.0/sndfileio.egg-info/top_level.txt
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-07 11:06:33.981746 sndfileio-1.9.1/
+-rw-rw-r--   0 em        (1000) em        (1000)     1060 2021-11-13 21:40:24.000000 sndfileio-1.9.1/LICENSE.md
+-rw-rw-r--   0 em        (1000) em        (1000)       25 2021-11-13 21:40:24.000000 sndfileio-1.9.1/MANIFEST.in
+-rw-rw-r--   0 em        (1000) em        (1000)     2249 2023-05-07 11:06:33.980746 sndfileio-1.9.1/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     1933 2022-03-07 08:14:11.000000 sndfileio-1.9.1/README.rst
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-05-07 11:06:33.981746 sndfileio-1.9.1/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      988 2023-05-07 11:05:27.000000 sndfileio-1.9.1/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-07 11:06:33.979746 sndfileio-1.9.1/sndfileio/
+-rwxrwxr-x   0 em        (1000) em        (1000)     2413 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1796 2022-03-07 08:16:05.000000 sndfileio-1.9.1/sndfileio/backend_lameenc.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3041 2022-07-03 09:12:18.000000 sndfileio-1.9.1/sndfileio/backend_miniaudio.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4862 2022-07-03 09:30:45.000000 sndfileio-1.9.1/sndfileio/datastructs.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     4796 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/dsp.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1170 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/mp3.py
+-rw-rw-r--   0 em        (1000) em        (1000)        0 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/py.typed
+-rwxrwxr-x   0 em        (1000) em        (1000)     7639 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/resampling.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    35191 2023-05-07 11:03:35.000000 sndfileio-1.9.1/sndfileio/sndfileio.py
+-rwxrwxr-x   0 em        (1000) em        (1000)      585 2021-11-13 21:40:24.000000 sndfileio-1.9.1/sndfileio/testing.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     9967 2022-07-03 09:12:18.000000 sndfileio-1.9.1/sndfileio/util.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-05-07 11:06:33.980746 sndfileio-1.9.1/sndfileio.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)     2249 2023-05-07 11:06:33.000000 sndfileio-1.9.1/sndfileio.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      452 2023-05-07 11:06:33.000000 sndfileio-1.9.1/sndfileio.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-05-07 11:06:33.000000 sndfileio-1.9.1/sndfileio.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       86 2023-05-07 11:06:33.000000 sndfileio-1.9.1/sndfileio.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       10 2023-05-07 11:06:33.000000 sndfileio-1.9.1/sndfileio.egg-info/top_level.txt
```

### Comparing `sndfileio-1.9.0/LICENSE.md` & `sndfileio-1.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/PKG-INFO` & `sndfileio-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sndfileio
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple API for reading / writing soundfiles
 Home-page: https://github.com/gesellkammer/sndfileio
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: LGPL
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `sndfileio-1.9.0/README.rst` & `sndfileio-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/setup.py` & `sndfileio-1.9.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from setuptools import setup
 import os
 
 thisdir = os.path.abspath(os.path.dirname(__file__))
 long_description = open(os.path.join(thisdir, 'README.rst')).read()
 
 setup(
-    version="1.9.0",
+    version="1.9.1",
     name="sndfileio",
     python_requires=">=3.8",
     install_requires=[
         "numpy>1.8",
         "scipy",
-        # "pysndfile",
         "soundfile",
         "miniaudio",
         "nnresample",
         "numpyx>=0.4.1",
         "tinytag",
         "filetype",
         "lameenc"],
```

### Comparing `sndfileio-1.9.0/sndfileio/__init__.py` & `sndfileio-1.9.1/sndfileio/__init__.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/backend_lameenc.py` & `sndfileio-1.9.1/sndfileio/backend_lameenc.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/backend_miniaudio.py` & `sndfileio-1.9.1/sndfileio/backend_miniaudio.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/datastructs.py` & `sndfileio-1.9.1/sndfileio/datastructs.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/dsp.py` & `sndfileio-1.9.1/sndfileio/dsp.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/mp3.py` & `sndfileio-1.9.1/sndfileio/mp3.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/resampling.py` & `sndfileio-1.9.1/sndfileio/resampling.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/sndfileio.py` & `sndfileio-1.9.1/sndfileio/sndfileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     import pysndfile
     from .datastructs import sample_t
     from typing import Dict, Tuple, Union, Iterator, Optional as Opt, List, Callable, Type
 
 
 logger = logging.getLogger("sndfileio")
 
+
 __all__ = [
     "sndread",
     "sndread_chunked",
     "sndget",
     "sndinfo",
     "sndwrite",
     "sndwrite_like",
@@ -49,14 +50,18 @@
     return _find_spec(pkg) is not None
 
 
 class SndfileError(IOError):
     pass
 
 
+def _normalize_path(path: str) -> str:
+    return _os.path.expanduser(path)
+
+
 def sndread(path: str, start: float = 0, end: float = 0) -> sample_t:
     """
     Read a soundfile as a numpy array.
 
     This is a float array defined between -1 and 1, independently of the format
     of the soundfile
 
@@ -76,14 +81,15 @@
         # Normalize and save as flac
         from sndfileio import sndread, sndwrite
         samples, sr = sndread("in.wav")
         maxvalue = max(samples.max(), -samples.min())
         samples *= 1/maxvalue
         sndwrite(samples, sr, "out.flac")
     """
+    path = _normalize_path(path)
     if not _os.path.exists(path):
         raise IOError(f"File not found: {path}")
     backend = _get_backend(path)
     if not backend:
         raise RuntimeError(f"No backend available to read {path}")
     logger.debug(f"sndread: using backend {backend.name}")
     return backend.read(path, start=start, end=end)
@@ -111,14 +117,15 @@
         >>> with sndwrite_chunked("out.flac", 44100) as writer:
         ...     for buf in sndread_chunked("in.flac"):
         ...         # do some processing, like changing the gain
         ...         buf *= 0.5
         ...         writer.write(buf)
 
     """
+    path = _normalize_path(path)
     backend = _get_backend(path, key=lambda backend: backend.can_read_chunked)
     if backend:
         logger.debug(f"sndread_chunked: using backend {backend.name}")
         return backend.read_chunked(path, chunksize, start=start, stop=stop)
     else:
         raise SndfileError("chunked reading is not supported by the "
                            "available backends")
@@ -141,14 +148,15 @@
 
         >>> from sndfileio import *
         >>> info = sndinfo("sndfile.wav")
         >>> print(f"Duration: {info.duration}s, samplerate: {info.samplerate}")
         Duration: 0.4s, samplerate: 44100
 
     """
+    path = _normalize_path(path)
     backend = _get_backend(path)
     if not backend:
         raise FormatNotSupported("sndinfo: no backend supports this filetype")
     logger.debug(f"sndinfo: using backend {backend.name}")
     return backend.getinfo(path)
 
 
@@ -172,14 +180,15 @@
         from sndfileio import *
         samples, info = sndget("in.wav")
         maxvalue = max(samples.max(), -samples.min())
         samples *= 1/maxvalue
         sndwrite("out.flac", samples, info.samplerate, metadata=info.metadata)
 
     """
+    path = _normalize_path(path)
     backend = _get_backend(path)
     if not backend:
         raise RuntimeError(f"No backend available to read {path}")
     logger.debug(f"sndread: using backend {backend.name}")
     return backend.read_with_info(path, start=start, end=end)
 
 
@@ -261,14 +270,15 @@
         # Normalize and save as flac
         >>> samples, sr = sndread("sndfile.wav")
         >>> maxvalue = max(samples.max(), -samples.min())
         >>> samples *= 1/maxvalue
         >>> sndwrite("out.flac", samples, sr)
 
     """
+    outfile = _normalize_path(outfile)
     fileformat, encoding = _resolve_encoding(outfile, samples=samples, fileformat=fileformat,
                                              encoding=encoding)
     if encoding.startswith('pcm') and normalize_if_clipping:
         clipping = ((samples > 1).any() or (samples < -1).any())
         if clipping:
             maxvalue = max(samples.max(), abs(samples.min()))
             logger.warning(f"Clipping found when writing pcm data to {outfile}")
@@ -329,14 +339,15 @@
         with sndwrite_chunked("out.flac", 44100) as writer:
             for buf in sndread_chunked("in.flac"):
                 # do some processing, like changing the gain
                 buf *= 0.5
                 writer.write(buf)
 
     """
+    outfile = _normalize_path(outfile)
     fileformat, encoding = _resolve_encoding(outfile, fileformat=fileformat,
                                              encoding=encoding)
     backends = [backend for backend in _get_backends()
                 if backend.can_write_chunked and fileformat in backend.filetypes_write]
     if not backends:
         raise SndfileError(f"No backend found to support the format {fileformat}")
     backend = min(backends, key=lambda backend: backend.priority)
@@ -380,14 +391,15 @@
         fadesize = int(0.5*sr)
         ramp = np.linspace(0, 1, fadesize))
         samples[:fadesize, 0] *= ramp
         samples[:fadesize, 1] *= ramp
         sndwrite_like(samples, "stereo.wav", "out.wav")
 
     """
+    outfile = _normalize_path(outfile)
     info = sndinfo(likefile)
     ext = _os.path.splitext(outfile)[1]
     outfileformat = util.fileformat_from_ext(ext)
     if outfileformat != info.fileformat:
         logger.warning(f"Trying to save to a file with extension {ext}, but fileformat"
                        f"will be {info.fileformat}")
     sndwrite(outfile=outfile, samples=samples, sr=sr or info.samplerate,
@@ -441,14 +453,15 @@
         quality: the quality, a value between 1-7 (where 1 is highest and 7 is fastest)
 
     .. note::
         To write samples in chunks use sndwrite_chunked. `bitrate` and `quality` can
         be passed as **options.
 
     """
+    outfile = _normalize_path(outfile)
     mp3backend = _BACKENDS['lameenc']
     if not mp3backend.is_available():
         raise RuntimeError("lameenc backend is not available")
     writer = mp3backend.writer(outfile=outfile, sr=sr, encoding='pcm16', fileformat='mp3',
                                bitrate=bitrate, quality=quality)
     writer.write(samples)
 
@@ -540,27 +553,27 @@
     def is_available(self) -> bool:
         """ Is this backend available? """
         return _is_package_installed(self.name)
 
     def writer(self, outfile: str, sr: int, encoding: str, fileformat: str,
                bitrate=0, metadata: Dict[str, str] = None, **options
                ) -> SndWriter:
-        """ Open outfile for write with the given properties 
+        """ Open outfile for write with the given properties
 
         Args:
             sr: samplerate
             outfile: the file to write
             encoding: the encoding used (pcm16, float32, etc)
             fileformat: the file format
             bitrate: used when writing to a compressed file.
             metadata: if given, a dict str: str. Allowed keys are: *title*, *comment*,
                 *artist*, *tracknumber*, *album*, *software*
 
         Returns:
-            a :class:`SndWriter` 
+            a :class:`SndWriter`
         """
         pass
         if self._writer is None:
             raise SndfileError(f"The backend {self.name} does not support writing")
         return self._writer(backend=self, sr=sr, outfile=outfile, encoding=encoding,
                             fileformat=fileformat, bitrate=bitrate, metadata=metadata,
                             **options)
@@ -680,15 +693,15 @@
             filetypes_write=["aif", "aiff", "wav", "flac"],
             can_read_chunked=True,
             can_write_chunked=True,
             name='soundfile',
             supports_metadata=True
         )
         self._writer = _SoundfileWriter
-        
+
     def read_with_info(self, path: str, start: float = 0, end: float = 0) -> Tuple[np.ndarray, SndInfo]:
         snd = _soundfile.SoundFile(path, 'r')
         info = self._getinfo(snd)
         samples = self._read(snd, start=start, end=end)
         return samples, info
 
     def _read(self, snd: _soundfile.SoundFile, start: float = 0, end: float = 0) -> np.ndarray:
@@ -951,8 +964,7 @@
     backends = _get_backends()
     if not backends:
         raise SndfileError("No available backends for writing")
     backends = [b for b in backends if fileformat in b.filetypes_write]
     if backends:
         return min(backends, key=lambda backend: backend.priority)
     return None
-
```

### Comparing `sndfileio-1.9.0/sndfileio/testing.py` & `sndfileio-1.9.1/sndfileio/testing.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio/util.py` & `sndfileio-1.9.1/sndfileio/util.py`

 * *Files identical despite different names*

### Comparing `sndfileio-1.9.0/sndfileio.egg-info/PKG-INFO` & `sndfileio-1.9.1/sndfileio.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sndfileio
-Version: 1.9.0
+Version: 1.9.1
 Summary: Simple API for reading / writing soundfiles
 Home-page: https://github.com/gesellkammer/sndfileio
 Author: Eduardo Moguillansky
 Author-email: eduardo.moguillansky@gmail.com
 License: LGPL
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

