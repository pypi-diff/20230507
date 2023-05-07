# Comparing `tmp/asap_stereo-0.3.0.tar.gz` & `tmp/asap_stereo-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asap_stereo-0.3.0.tar", last modified: Wed Mar 22 22:04:54 2023, max compression
+gzip compressed data, was "asap_stereo-0.3.1.tar", last modified: Sun May  7 18:58:59 2023, max compression
```

## Comparing `asap_stereo-0.3.0.tar` & `asap_stereo-0.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:04:54.992812 asap_stereo-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-03-22 22:04:54.992812 asap_stereo-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 22:04:54.992812 asap_stereo-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:04:54.988812 asap_stereo-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:04:54.988812 asap_stereo-0.3.0/src/asap_stereo/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   102161 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/asap.py
--rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/asap_ctx_workflow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow_hiproc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow_nomap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-03-22 22:04:38.000000 asap_stereo-0.3.0/src/asap_stereo/stereo_quality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 22:04:54.992812 asap_stereo-0.3.0/src/asap_stereo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-22 22:04:54.000000 asap_stereo-0.3.0/src/asap_stereo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:58:59.636950 asap_stereo-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-07 18:58:59.632950 asap_stereo-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:58:59.636950 asap_stereo-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:58:59.632950 asap_stereo-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:58:59.632950 asap_stereo-0.3.1/src/asap_stereo/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102151 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/asap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/asap_ctx_workflow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow_hiproc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13901 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow_nomap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17101 2023-05-07 18:58:41.000000 asap_stereo-0.3.1/src/asap_stereo/stereo_quality.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:58:59.632950 asap_stereo-0.3.1/src/asap_stereo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-07 18:58:59.000000 asap_stereo-0.3.1/src/asap_stereo.egg-info/top_level.txt
```

### Comparing `asap_stereo-0.3.0/LICENSE` & `asap_stereo-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/PKG-INFO` & `asap_stereo-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asap_stereo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A high level CLI and reproducible workflow for the Ames Stereo Pipeline
 Author-email: "Andrew M. Annex" <ama6fy@virginia.edu>
 License: BSD 3-Clause License
 Project-URL: repository, https://github.com/AndrewAnnex/asap_stereo/
 Keywords: mars,nasa,asp,ames,stereo,pipeline,cli,tool,workflow
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `asap_stereo-0.3.0/README.rst` & `asap_stereo-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/pyproject.toml` & `asap_stereo-0.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 authors = [
     {name = 'Andrew M. Annex', email='ama6fy@virginia.edu'}
 ]
 dependencies = [
     'requests',
     'fire',
     'moody>=0.2.0',
-    'sh',
+    'sh>=2.0.0',
     'papermill',
     'rasterio',
     'pyproj'
 ]
 classifiers=[
     'Natural Language :: English',
     'License :: OSI Approved :: BSD License',
```

### Comparing `asap_stereo-0.3.0/src/asap_stereo/asap.py` & `asap_stereo-0.3.1/src/asap_stereo/asap.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,17 @@
 
 import fire
 import sh
 from sh import Command
 import moody
 import pyproj
 import papermill as pm
+import pvl
+
+
 
 def custom_log(ran, call_args, pid=None):
     return ran
 
 here = os.path.dirname(__file__)
 
 cores = os.cpu_count()
@@ -156,29 +159,14 @@
             keys.append(f'--{key}')
         elif not key.startswith('-'):
             keys.append(f'-{key}')
         else:
             keys.append(key)
     return [x for x in itertools.chain.from_iterable(itertools.zip_longest(keys, kwargs.values())) if x is not None]
 
-def isis3_to_dict(instr: str)-> Dict:
-    """
-    Given a stdout string from ISIS3, return a Dict version
-    
-    :param instr:
-    :return: dictionary of isis output
-    """
-    groups = re.findall(r'Group([\S\s]*?)End_Group', instr)
-    out = {}
-    for group in groups:
-        lines = [x.replace('=', '').split() for x in group.split('\\n')]
-        group_name = lines[0][0]
-        out[group_name] = {t[0]: t[1] for t in lines[1:-1]}
-    return out
-
 
 def kwarg_parse(kwargs: Dict, key: str)-> str:
     if kwargs is None:
         return ''
     key_args = kwargs.get(key, {})
     if isinstance(key_args, str):
         return key_args
@@ -264,15 +252,15 @@
 
               ___   _____ ___    ____
              /   | / ___//   |  / __ \
             / /| | \__ \/ /| | / /_/ /
            / ___ |___/ / ___ |/ ____/
           /_/  |_/____/_/  |_/_/      𝑆 𝑇 𝐸 𝑅 𝐸 𝑂
 
-          asap_stereo (0.2.0)
+          asap_stereo (0.3.1)
 
           Github: https://github.com/AndrewAnnex/asap_stereo
           Cite: https://doi.org/10.5281/zenodo.4171570
 
     █████████████████████████████████████████████████████████████
     """
 
@@ -367,16 +355,21 @@
         self.ctxcal      = Command('ctxcal').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.ctxevenodd  = Command('ctxevenodd').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.hillshade   = Command('gdaldem').hillshade.bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.mapproject  = Command('mapproject').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.ipfind      = Command('ipfind').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.ipmatch     = Command('ipmatch').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
         self.gdaltranslate = Command('gdal_translate').bake(_out=sys.stdout, _err=sys.stderr, _log_msg=custom_log)
+        # get the help for paralle bundle adjust which changed between 3.x versions
+        pba_help = sh.parallel_bundle_adjust('--help')
+        pk = '--threads'
+        if hasattr(pba_help, '--threads-singleprocess'):
+            pk = '--threads-singleprocess'
         self.ba = Command('parallel_bundle_adjust').bake(
-                '--threads', _threads_singleprocess,
+                pk, _threads_singleprocess,
                 _out=sys.stdout, _err=sys.stderr, _log_msg=custom_log
             )
 
     @staticmethod
     def gen_csm(*cubs, meta_kernal=None, max_workers=_threads_singleprocess):
         """
         Given N cub files, generate json camera models for each using ale
@@ -423,16 +416,18 @@
         """
         wd = str(Path(img).absolute().parent)
         with silent_cd(wd):
             # currently have to cd into the directory to minify the length
             # of the file name parameter, isis3 inserts additional new lines to wrap
             # words in the terminal that will mess up isis3 to dict without management
             camrange = Command('camrange').bake(_log_msg=custom_log)
-            out = str(camrange(f'from={str(Path(img).name)}').stdout)
-            out_dict = isis3_to_dict(out)
+            from_path = str(Path(img).name)
+            to_path = f'{str(Path(img).stem)}_camrange'
+            cam_res = camrange(f'from={from_path}', f'to={to_path}')
+            out_dict = pvl.load(f'{to_path}.txt')
         return out_dict
 
     @staticmethod
     def get_image_band_stats(img)-> dict:
         """
         :param img: 
         :return: 
@@ -500,15 +495,15 @@
             if 'ERROR' in proj4str or len(proj4str) < 10:
                 raise RuntimeError(f'Gdalsrsinfo failed: {proj4str}')
         except (sh.ErrorReturnCode, RuntimeError) as e:
             warnings.warn(f'No SRS info, falling back to use ISIS caminfo.\n exception was: {e}')
             out_dict = CommonSteps.get_cam_info(img)
             lon = circ_mean(float(out_dict['UniversalGroundRange']['MinimumLongitude']), float(out_dict['UniversalGroundRange']['MaximumLongitude']))
             lat = (float(out_dict['UniversalGroundRange']['MinimumLatitude']) + float(out_dict['UniversalGroundRange']['MaximumLatitude'])) / 2
-            proj4str = f"+proj=ortho +lon_0={lon} +lat_0={lat} +x_0=0 +y_0=0 +a={out_dict['Target']['RadiusA']} +b={out_dict['Target']['RadiusB']} +units=m +no_defs"
+            proj4str = f"+proj=ortho +lon_0={lon} +lat_0={lat} +x_0=0 +y_0=0 +a={float(out_dict['Target']['RadiusA'])} +b={float(out_dict['Target']['RadiusB'])} +units=m +no_defs"
         return str(proj4str).rstrip('\n\' ').lstrip('\'')
 
     @staticmethod
     def get_map_info(img, key: str, group='UniversalGroundRange')-> str:
         out_dict = CommonSteps.get_cam_info(img)
         return out_dict[group][key]
 
@@ -984,15 +979,15 @@
 
               ___   _____ ___    ____
              /   | / ___//   |  / __ \
             / /| | \__ \/ /| | / /_/ /
            / ___ |___/ / ___ |/ ____/
           /_/  |_/____/_/  |_/_/      𝑆 𝑇 𝐸 𝑅 𝐸 𝑂
 
-          asap_stereo (0.2.0)
+          asap_stereo (0.3.1)
 
           Github: https://github.com/AndrewAnnex/asap_stereo
           Cite: https://doi.org/10.5281/zenodo.4171570
 
     █████████████████████████████████████████████████████████████
     """
 
@@ -1330,15 +1325,15 @@
 
               ___   _____ ___    ____
              /   | / ___//   |  / __ \
             / /| | \__ \/ /| | / /_/ /
            / ___ |___/ / ___ |/ ____/
           /_/  |_/____/_/  |_/_/      𝑆 𝑇 𝐸 𝑅 𝐸 𝑂
 
-          asap_stereo (0.2.0)
+          asap_stereo (0.3.1)
 
           Github: https://github.com/AndrewAnnex/asap_stereo
           Cite: https://doi.org/10.5281/zenodo.4171570
 
     █████████████████████████████████████████████████████████████
     """
 
@@ -1766,15 +1761,15 @@
 
               ___   _____ ___    ____
              /   | / ___//   |  / __ \
             / /| | \__ \/ /| | / /_/ /
            / ___ |___/ / ___ |/ ____/
           /_/  |_/____/_/  |_/_/      𝑆 𝑇 𝐸 𝑅 𝐸 𝑂
 
-          asap_stereo (0.2.0)
+          asap_stereo (0.3.1)
 
           Github: https://github.com/AndrewAnnex/asap_stereo
           Cite: https://doi.org/10.5281/zenodo.4171570
 
     █████████████████████████████████████████████████████████████
     """
 
@@ -1842,14 +1837,15 @@
     def normalize(self, image):
         # iterable of bands
         band_stats = self.cs.get_image_band_stats(image)
         # make output name
         out_name = Path(image).stem + '_normalized.vrt'
         # get bands scaling iterable, multiply by 1.001 for a little lower range
         scales = itertools.chain(((f'-scale_{bandif["band"]}', float(bandif["minimum"])*1.001, float(bandif["maximum"])*1.001, 1, 255) for bandif in band_stats))
+        scales = [str(_).strip("'()\"") for _ in scales]
         # run gdal translate
         _ = sh.gdal_translate(image, out_name, '-of', 'vrt', '-ot', 'Byte', *scales, '-a_nodata', 0, _out=sys.stdout, _err=sys.stderr)
         return out_name
 
     def find_matches(self, reference_image, *mobile_images, ipfindkwargs=None, ipmatchkwargs=None):
         """
         Generate GCPs for a mobile image relative to a reference image and echo to std out
@@ -2144,15 +2140,15 @@
                                                                  
               ___   _____ ___    ____                            
              /   | / ___//   |  / __ \                           
             / /| | \__ \/ /| | / /_/ /                           
            / ___ |___/ / ___ |/ ____/                            
           /_/  |_/____/_/  |_/_/      𝑆 𝑇 𝐸 𝑅 𝐸 𝑂               
 
-          asap_stereo (0.2.0)
+          asap_stereo (0.3.1)
 
           Github: https://github.com/AndrewAnnex/asap_stereo
           Cite: https://doi.org/10.5281/zenodo.4171570
 
     █████████████████████████████████████████████████████████████
     """
```

### Comparing `asap_stereo-0.3.0/src/asap_stereo/asap_ctx_workflow.ipynb` & `asap_stereo-0.3.1/src/asap_stereo/asap_ctx_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow.ipynb` & `asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow.ipynb`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow_hiproc.ipynb` & `asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow_hiproc.ipynb`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/src/asap_stereo/asap_hirise_workflow_nomap.ipynb` & `asap_stereo-0.3.1/src/asap_stereo/asap_hirise_workflow_nomap.ipynb`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/src/asap_stereo/stereo_quality.py` & `asap_stereo-0.3.1/src/asap_stereo/stereo_quality.py`

 * *Files identical despite different names*

### Comparing `asap_stereo-0.3.0/src/asap_stereo.egg-info/PKG-INFO` & `asap_stereo-0.3.1/src/asap_stereo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asap-stereo
-Version: 0.3.0
+Version: 0.3.1
 Summary: A high level CLI and reproducible workflow for the Ames Stereo Pipeline
 Author-email: "Andrew M. Annex" <ama6fy@virginia.edu>
 License: BSD 3-Clause License
 Project-URL: repository, https://github.com/AndrewAnnex/asap_stereo/
 Keywords: mars,nasa,asp,ames,stereo,pipeline,cli,tool,workflow
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `asap_stereo-0.3.0/src/asap_stereo.egg-info/SOURCES.txt` & `asap_stereo-0.3.1/src/asap_stereo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

