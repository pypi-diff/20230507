# Comparing `tmp/pulsectl-asyncio-1.0.0.tar.gz` & `tmp/pulsectl-asyncio-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-asyncio-1.0.0.tar", last modified: Tue Feb 21 21:25:03 2023, max compression
+gzip compressed data, was "pulsectl-asyncio-1.1.0.tar", last modified: Sun May  7 20:25:20 2023, max compression
```

## Comparing `pulsectl-asyncio-1.0.0.tar` & `pulsectl-asyncio-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/pulsectl_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio/pa_asyncio_mainloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27244 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio/pulsectl_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-02-21 21:25:03.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-02-21 21:25:03.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 21:25:03.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-21 21:25:03.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 21:25:03.000000 pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 21:25:03.086284 pulsectl-asyncio-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/tests/test_async_with_dummy_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-21 21:24:51.000000 pulsectl-asyncio-1.0.0/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.012627 pulsectl-asyncio-1.1.0/pulsectl_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/pa_asyncio_mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/pulsectl_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.012627 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/tests/test_async_with_dummy_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/tests/test_examples.py
```

### Comparing `pulsectl-asyncio-1.0.0/LICENSE` & `pulsectl-asyncio-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.0.0/PKG-INFO` & `pulsectl-asyncio-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pulsectl-asyncio-1.0.0/README.md` & `pulsectl-asyncio-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.0.0/pulsectl_asyncio/pa_asyncio_mainloop.py` & `pulsectl-asyncio-1.1.0/pulsectl_asyncio/pa_asyncio_mainloop.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.0.0/pulsectl_asyncio/pulsectl_async.py` & `pulsectl-asyncio-1.1.0/pulsectl_asyncio/pulsectl_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
 				await self._event_mask_set('null')
 
 	async def get_peak_sample(self, source, timeout, stream_idx=None):
 		'''Returns peak (max) value in 0-1.0 range for samples in source/stream within timespan.
 			"source" can be either int index of pulseaudio source
 				(i.e. source.index), its name (source.name), or None to use default source.
 			Resulting value is what pulseaudio returns as
-				PA_SAMPLE_FLOAT32BE float after "timeout" seconds.
+				PA_SAMPLE_FLOAT32NE float after "timeout" seconds.
 			If specified source does not exist, 0 should be returned after timeout.
 			This can be used to detect if there's any sound
 				on the microphone or any sound played through a sink via its monitor_source index,
 				or same for any specific stream connected to these (if "stream_idx" is passed).
 			Sample stream masquerades as
 				application.id=org.PulseAudio.pavucontrol to avoid being listed in various mixer apps.
 			Example - get peak for specific sink input "si" for 0.8 seconds:
@@ -550,15 +550,15 @@
 	async def subscribe_peak_sample(self, source, rate=25, stream_idx=None, allow_suspend=False
 			) -> AsyncIterator[float]:
 		"""
 		Subscribe to a (downsampled) audio stream to monitor audio volume.
 
 		Using PulseAudio's `stream_connect_record` method, the stream can either be a normal record stream from a
 		source, a stream from a sink monitor source or a monitor stream of a specific sink input. To monitor the volume,
-		we use the PA_SAMPLE_FLOAT32BE sample format. This method returns an asynchronous generator, which yields the
+		we use the PA_SAMPLE_FLOAT32NE sample format. This method returns an asynchronous generator, which yields the
 		volume samples as they are streamed from the PulseAudio server.
 
 		Example usage for monitoring a source (e.g. microphone input) with 5Hz::
 
 		  async for volume in pulse.subscribe_peak_sample(source.name, rate=5):
 		      print("volume =", volume)
 
@@ -574,28 +574,27 @@
 		:param stream_idx: When `source` is a sink monitor source, specify the index (!) of a sink input, to monitor
 			this single sink input stream instead of the sink sum signal.
 		:param allow_suspend: If True, the flat DONT_INHIBIT_AUTO_SUSPEND is set on the stream, such that Pulse Audio
 			will automatically suspend the source or sink after some seconds, despite our monitor stream running. This
 			is useful for monitoring sinks, but prevents actively monitoring sources for more than a few seconds.
 		"""
 		proplist = c.pa.proplist_from_string('')
-		ss = c.PA_SAMPLE_SPEC(format=c.PA_SAMPLE_FLOAT32BE, rate=rate, channels=1)
+		ss = c.PA_SAMPLE_SPEC(format=c.PA_SAMPLE_FLOAT32NE, rate=rate, channels=1)
 		s = c.pa.stream_new_with_proplist(self._ctx, 'peak detect', c.byref(ss), None, proplist)
 		queue = asyncio.Queue()
 		c.pa.proplist_free(proplist)
 
 		@c.PA_STREAM_REQUEST_CB_T
 		def read_cb(s, nbytes, _userdata):
 			bs = c.c_int(nbytes)
 			buff = c.c_void_p()
 			c.pa.stream_peek(s, buff, c.byref(bs))
 			try:
 				if not buff or bs.value < 4:
 					return
-				# This assumes that native byte order for floats is BE, same as pavucontrol
 				queue.put_nowait(c.cast(buff, c.POINTER(c.c_float))[0])
 			finally:
 				# stream_drop() flushes buffered data (incl. buff=NULL "hole" data)
 				# stream.h: "should not be called if the buffer is empty"
 				if bs.value:
 					c.pa.stream_drop(s)
```

### Comparing `pulsectl-asyncio-1.0.0/pulsectl_asyncio.egg-info/PKG-INFO` & `pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.0.0
+Version: 1.1.0
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pulsectl-asyncio-1.0.0/setup.cfg` & `pulsectl-asyncio-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pulsectl-asyncio
-version = 1.0.0
+version = 1.1.0
 url = https://github.com/mhthies/pulsectl-asyncio
 author = Michael Thies
 author_email = mail@mhthies.de
 description = Asyncio frontend for the pulsectl Python bindings of libpulse
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -23,14 +23,14 @@
 	Operating System :: POSIX
 	Development Status :: 5 - Production/Stable
 
 [options]
 packages = pulsectl_asyncio
 python_requires = >=3.6
 install_requires = 
-	pulsectl >=21.10.2,<=22.3.2
+	pulsectl >=22.5.0,<=22.5.1
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pulsectl-asyncio-1.0.0/tests/test_async_with_dummy_instance.py` & `pulsectl-asyncio-1.1.0/tests/test_async_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.0.0/tests/test_examples.py` & `pulsectl-asyncio-1.1.0/tests/test_examples.py`

 * *Files identical despite different names*

