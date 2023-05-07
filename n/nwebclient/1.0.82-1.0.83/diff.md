# Comparing `tmp/nwebclient-1.0.82.tar.gz` & `tmp/nwebclient-1.0.83.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nwebclient-1.0.82.tar", last modified: Sat May  6 15:07:30 2023, max compression
+gzip compressed data, was "dist/nwebclient-1.0.83.tar", last modified: Sat May  6 17:29:42 2023, max compression
```

## Comparing `nwebclient-1.0.82.tar` & `nwebclient-1.0.83.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 15:07:30.452704 nwebclient-1.0.82/
--rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.82/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-06 15:07:30.452704 nwebclient-1.0.82/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.82/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 15:07:30.452704 nwebclient-1.0.82/nwebclient/
--rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.82/nwebclient/__init__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.82/nwebclient/__main__.py
--rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.82/nwebclient/crypt.py
--rw-r--r--   0 pi        (1000) pi        (1000)    10950 2023-05-06 15:07:15.000000 nwebclient-1.0.82/nwebclient/sd.py
--rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.82/nwebclient/sdb.py
--rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.82/nwebclient/ticker.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 15:07:30.452704 nwebclient-1.0.82/nwebclient.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-06 15:07:30.000000 nwebclient-1.0.82/nwebclient.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-06 15:07:30.452704 nwebclient-1.0.82/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-06 15:07:27.000000 nwebclient-1.0.82/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 17:29:42.120960 nwebclient-1.0.83/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1060 2023-01-18 15:38:31.000000 nwebclient-1.0.83/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-06 17:29:42.120960 nwebclient-1.0.83/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      692 2023-01-18 15:38:31.000000 nwebclient-1.0.83/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 17:29:42.120960 nwebclient-1.0.83/nwebclient/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4704 2023-03-17 18:34:02.000000 nwebclient-1.0.83/nwebclient/__init__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     2584 2023-02-01 15:16:08.000000 nwebclient-1.0.83/nwebclient/__main__.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     3316 2023-05-05 19:49:25.000000 nwebclient-1.0.83/nwebclient/crypt.py
+-rw-r--r--   0 pi        (1000) pi        (1000)    10951 2023-05-06 17:29:25.000000 nwebclient-1.0.83/nwebclient/sd.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     6100 2023-05-05 17:05:53.000000 nwebclient-1.0.83/nwebclient/sdb.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     4114 2023-04-26 14:15:39.000000 nwebclient-1.0.83/nwebclient/ticker.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-05-06 17:29:42.120960 nwebclient-1.0.83/nwebclient.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     1460 2023-05-06 17:29:41.000000 nwebclient-1.0.83/nwebclient.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      364 2023-05-06 17:29:42.000000 nwebclient-1.0.83/nwebclient.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-05-06 17:29:41.000000 nwebclient-1.0.83/nwebclient.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)      120 2023-05-06 17:29:41.000000 nwebclient-1.0.83/nwebclient.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       20 2023-05-06 17:29:41.000000 nwebclient-1.0.83/nwebclient.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-05-06 17:29:41.000000 nwebclient-1.0.83/nwebclient.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-05-06 17:29:42.120960 nwebclient-1.0.83/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      880 2023-05-06 17:29:39.000000 nwebclient-1.0.83/setup.py
```

### Comparing `nwebclient-1.0.82/LICENSE` & `nwebclient-1.0.83/LICENSE`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/PKG-INFO` & `nwebclient-1.0.83/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.82
+Version: 1.0.83
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.82/README.md` & `nwebclient-1.0.83/README.md`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient/__init__.py` & `nwebclient-1.0.83/nwebclient/__init__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient/__main__.py` & `nwebclient-1.0.83/nwebclient/__main__.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient/crypt.py` & `nwebclient-1.0.83/nwebclient/crypt.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient/sd.py` & `nwebclient-1.0.83/nwebclient/sd.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,19 +48,19 @@
     save_mode='sdb'
     loaded_model = None
     gen_count = 0
     api = None
     cn_image = None
     diff_cn = None
     def __init__(self, model_id="XpucT/Deliberate"):
-        self.info("Loading Stable Diffusion Dependencies...");
         self.model_id = model_id
     def load(self):
         if self.loaded_model == self.model_id or self.generator == 'automatic1111':
             return
+        self.info("Loading Stable Diffusion Dependencies...");
         from diffusers import PNDMScheduler, DDIMScheduler, LMSDiscreteScheduler, EulerDiscreteScheduler, DPMSolverMultistepScheduler
         from diffusers import UniPCMultistepScheduler
         import torch
         from diffusers import StableDiffusionPipeline
         from diffusers import StableDiffusionControlNetPipeline, ControlNetModel
         self.scheduler = DPMSolverMultistepScheduler.from_pretrained(self.model_id, subfolder="scheduler")
         device = "cuda"
@@ -108,15 +108,15 @@
     def genCnPose1111(self, loop_number=1):
         self.initA1111();
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, controlnet_units=[self.cn_image],cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genA1111(self, loop_number=1):  
         self.initA1111();
-        if self.model_id.endwith('.safetensors') and self.model_id != self.loaded_model:
+        if self.model_id.endswith('.safetensors') and self.model_id != self.loaded_model:
              self.a1111setModel(self.model_id)
         result = self.api.txt2img(prompt=self.prompt,negative_prompt=self.negative_prompt, height=self.height, width=self.width, cfg_scale=7)
         self.save_image(result.image, 0,loop_number)
         self.gen_count = self.gen_count + 1
     def genDiffusers(self, loop_number=1):
         if self.pipe is None:
             self.load()
```

### Comparing `nwebclient-1.0.82/nwebclient/sdb.py` & `nwebclient-1.0.83/nwebclient/sdb.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient/ticker.py` & `nwebclient-1.0.83/nwebclient/ticker.py`

 * *Files identical despite different names*

### Comparing `nwebclient-1.0.82/nwebclient.egg-info/PKG-INFO` & `nwebclient-1.0.83/nwebclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwebclient
-Version: 1.0.82
+Version: 1.0.83
 Summary: NWebClient via HTTP
 Home-page: https://bsnx.net/4.0/group/pynwebclient
 Author: Bjoern Salgert
 Author-email: bjoern.salgert@hs-duesseldorf.de
 License: UNKNOWN
 Description: # NWeb Client
```

### Comparing `nwebclient-1.0.82/setup.py` & `nwebclient-1.0.83/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nwebclient",
-    version="1.0.82",
+    version="1.0.83",
     author="Bjoern Salgert",
     author_email="bjoern.salgert@hs-duesseldorf.de",
     description="NWebClient via HTTP",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://bsnx.net/4.0/group/pynwebclient",
     packages=setuptools.find_packages(),
```

