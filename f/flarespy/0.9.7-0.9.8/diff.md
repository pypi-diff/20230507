# Comparing `tmp/flarespy-0.9.7.tar.gz` & `tmp/flarespy-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flarespy-0.9.7.tar", max compression
+gzip compressed data, was "flarespy-0.9.8.tar", max compression
```

## Comparing `flarespy-0.9.7.tar` & `flarespy-0.9.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.7/LICENSE
--rw-r--r--   0        0        0      428 2023-04-25 23:11:23.194116 flarespy-0.9.7/pyproject.toml
--rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.7/src/flarespy/Flare_model.py
--rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.7/src/flarespy/__init__.py
--rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.7/src/flarespy/data/model.dat
--rw-r--r--   0        0        0    34997 2023-04-25 23:10:54.809941 flarespy-0.9.7/src/flarespy/flarefinder.py
--rw-r--r--   0        0        0     4674 2023-04-25 16:16:25.193202 flarespy-0.9.7/src/flarespy/utils.py
--rw-r--r--   0        0        0       22 2023-04-25 23:11:23.188897 flarespy-0.9.7/src/flarespy/version.py
--rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-09-03 06:20:05.854812 flarespy-0.9.8/LICENSE
+-rw-r--r--   0        0        0      428 2023-04-27 01:21:12.567489 flarespy-0.9.8/pyproject.toml
+-rw-r--r--   0        0        0     3036 2023-02-03 08:53:00.981401 flarespy-0.9.8/src/flarespy/Flare_model.py
+-rw-r--r--   0        0        0      118 2022-09-03 06:20:05.855706 flarespy-0.9.8/src/flarespy/__init__.py
+-rw-r--r--   0        0        0   569289 2023-03-30 09:22:45.813451 flarespy-0.9.8/src/flarespy/data/model.dat
+-rw-r--r--   0        0        0    35050 2023-04-27 02:00:18.325408 flarespy-0.9.8/src/flarespy/flarefinder.py
+-rw-r--r--   0        0        0     4674 2023-04-25 16:16:25.193202 flarespy-0.9.8/src/flarespy/utils.py
+-rw-r--r--   0        0        0       22 2023-04-27 01:21:12.570155 flarespy-0.9.8/src/flarespy/version.py
+-rw-r--r--   0        0        0      726 1970-01-01 00:00:00.000000 flarespy-0.9.8/PKG-INFO
```

### Comparing `flarespy-0.9.7/LICENSE` & `flarespy-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.7/src/flarespy/Flare_model.py` & `flarespy-0.9.8/src/flarespy/Flare_model.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.7/src/flarespy/data/model.dat` & `flarespy-0.9.8/src/flarespy/data/model.dat`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.7/src/flarespy/flarefinder.py` & `flarespy-0.9.8/src/flarespy/flarefinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
     get_flare_probability,
 )
 
 logging.getLogger("astroquery").setLevel(logging.WARNING)
 
 CUSTOM_SIMBAD = Simbad()
 CUSTOM_SIMBAD.add_votable_fields("otype")
-CUSTOM_SIMBAD.add_votable_fields("otypes")
 CUSTOM_SIMBAD.add_votable_fields("ids")
 
 VIZIER = Vizier(columns=["Plx", "Gmag", "BP-RP"])
 
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 
 STELLAR_PARAM_COLUMNS = [
@@ -194,16 +193,18 @@
         """
 
         period_array = np.array([1, 2, 4]) * self.period
         std_array = np.zeros_like(period_array)
         folded_lc_list = []
         trend_folded_flux_list = []
 
+        lc = self.copy()
+        lc.flux[self.eclipse_mask] = np.nan
         for i, period in enumerate(period_array):
-            folded_lc = self.fold(period)
+            folded_lc = lc.fold(period)
             detrended_folded_flux, trend_folded_flux = flatten(
                 folded_lc.time.value,
                 folded_lc.flux,
                 method="median",
                 window_length=period / 50,
                 return_trend=True,
             )
@@ -543,17 +544,15 @@
         self.meta["EXCLUDE"] = False
         if simbad_result is not None:
             self._is_cv(simbad_result)
 
     def _is_cv(self, simbad_result):
         obj_type = simbad_result["OTYPE"]
         self.stellar_parameters.obj_type = obj_type
-
-        obj_type_list = simbad_result["OTYPES"].split("|")
-        if obj_type in EXCLUDED_OTYPES or "CV*" in obj_type_list:
+        if obj_type in EXCLUDED_OTYPES:
             self.meta["EXCLUDE"] = True
 
     def _query_gaia_dr3_params(self):
         """
         Query parallax, Gmag and BP-RP from Gaia DR3
         """
 
@@ -714,15 +713,16 @@
                     ax_label = fig.add_subplot(111)
                     ax_label.spines[["top", "bottom", "left", "right"]].set_visible(False)
                     ax_label.set_xlabel("Time - 2457000 [BTJD days]")
                     ax_label.set_ylabel("Normalized Flux")
                     ax_label.minorticks_off()
 
                     ax_original_lc = fig.add_subplot(221)
-                    self.scatter(ax=ax_original_lc, label="")
+                    self[~self.eclipse_mask].scatter(ax=ax_original_lc, label="")
+                    self[self.eclipse_mask].scatter(ax=ax_original_lc, label="", c="tab:gray")
                     self.plot(
                         ax=ax_original_lc,
                         column="trend_flux",
                         color="tab:red",
                         label="",
                     )
                     ax_original_lc.set_xlabel("")
```

### Comparing `flarespy-0.9.7/src/flarespy/utils.py` & `flarespy-0.9.8/src/flarespy/utils.py`

 * *Files identical despite different names*

### Comparing `flarespy-0.9.7/PKG-INFO` & `flarespy-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flarespy
-Version: 0.9.7
+Version: 0.9.8
 Summary: Find flares in TESS light curves
 Home-page: https://github.com/keyuxing/flarespy
 License: MIT
 Author: Keyu Xing
 Author-email: kyxing@mail.bnu.edu.cn
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

