# Comparing `tmp/pystarshade-0.1.2.tar.gz` & `tmp/pystarshade-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pystarshade-0.1.2.tar", last modified: Sat Apr 22 18:56:08 2023, max compression
+gzip compressed data, was "dist/pystarshade-0.1.5.tar", last modified: Sun May  7 21:18:40 2023, max compression
```

## Comparing `pystarshade-0.1.2.tar` & `pystarshade-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,24 @@
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-04-22 18:56:08.000000 pystarshade-0.1.2/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade/
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade/apodization/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3163 2023-04-21 21:25:36.000000 pystarshade-0.1.2/pystarshade/apodization/apodization.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.2/pystarshade/apodization/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       48 2023-04-18 00:42:34.000000 pystarshade-0.1.2/pystarshade/apodization/sample.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.2/pystarshade/version.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.2/pystarshade/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     1086 2023-04-21 21:24:04.000000 pystarshade-0.1.2/pystarshade/example_star_exo.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     3772 2023-04-21 21:24:55.000000 pystarshade-0.1.2/pystarshade/simulate_field.py
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade/diffraction/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2829 2023-04-21 21:21:37.000000 pystarshade-0.1.2/pystarshade/diffraction/field.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.2/pystarshade/diffraction/__init__.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2110 2023-04-18 00:42:34.000000 pystarshade-0.1.2/pystarshade/diffraction/bluestein_fft.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2797 2023-04-21 21:01:22.000000 pystarshade-0.1.2/pystarshade/diffraction/util.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     5999 2023-04-21 21:23:21.000000 pystarshade-0.1.2/pystarshade/diffraction/diffract.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)     2254 2023-04-21 21:13:19.000000 pystarshade-0.1.2/README.md
-drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/
--rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/dependency_links.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/top_level.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/requires.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      588 2023-04-22 18:56:08.000000 pystarshade-0.1.2/pystarshade.egg-info/SOURCES.txt
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-04-22 18:53:48.000000 pystarshade-0.1.2/setup.py
--rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-04-22 18:56:08.000000 pystarshade-0.1.2/PKG-INFO
--rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-04-22 18:56:08.000000 pystarshade-0.1.2/setup.cfg
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:18:40.000000 pystarshade-0.1.5/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade/
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade/apodization/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3163 2023-04-21 21:25:36.000000 pystarshade-0.1.5/pystarshade/apodization/apodize.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.5/pystarshade/apodization/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.5/pystarshade/version.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-18 00:42:34.000000 pystarshade-0.1.5/pystarshade/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6714 2023-05-07 21:16:01.000000 pystarshade-0.1.5/pystarshade/simulate_field.py
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade/diffraction/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     6682 2023-05-06 16:20:58.000000 pystarshade-0.1.5/pystarshade/diffraction/field.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-04-21 21:01:22.000000 pystarshade-0.1.5/pystarshade/diffraction/__init__.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     2004 2023-05-06 19:54:21.000000 pystarshade-0.1.5/pystarshade/diffraction/bluestein_fft.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     3362 2023-05-06 19:55:46.000000 pystarshade-0.1.5/pystarshade/diffraction/util.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     5953 2023-05-03 22:04:10.000000 pystarshade-0.1.5/pystarshade/diffraction/diffract.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)     2404 2023-05-07 21:09:32.000000 pystarshade-0.1.5/README.md
+drwxrwxr-x   0 ielo      (1000) ielo      (1000)        0 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)        1 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/dependency_links.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/top_level.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       12 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/requires.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      518 2023-05-07 21:18:40.000000 pystarshade-0.1.5/pystarshade.egg-info/SOURCES.txt
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      869 2023-05-07 21:18:36.000000 pystarshade-0.1.5/setup.py
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)      737 2023-05-07 21:18:40.000000 pystarshade-0.1.5/PKG-INFO
+-rw-rw-r--   0 ielo      (1000) ielo      (1000)       38 2023-05-07 21:18:40.000000 pystarshade-0.1.5/setup.cfg
```

### Comparing `pystarshade-0.1.2/pystarshade/apodization/apodization.py` & `pystarshade-0.1.5/pystarshade/apodization/apodize.py`

 * *Files identical despite different names*

### Comparing `pystarshade-0.1.2/pystarshade/simulate_field.py` & `pystarshade-0.1.5/pystarshade/simulate_field.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,73 @@
 import numpy as np
-from apodization.apodization import *
+from apodization.apodize import *
 from diffraction.util import *
 from diffraction.field import *
 from diffraction.diffract import *
 
-def point_source_to_ccd(mag_s, loc_s, wl, dist_xo_ss, dist_ss_t, focal_length_lens, radius_lens, N_x = 6001, N_t = 1001, N_pix = 1001,
+def source_field_to_ccd(source_field, wl, dist_xo_ss, dist_ss_t, focal_length_lens, radius_lens, 
+                        N_s = 333, N_x = 6401, N_t = 1001, N_pix = 4001, 
+                        ds = 10*0.03*au_to_meter, dx = 0.01, dt = 0.0116, dp=.5*1.9e-7):
+    """
+    Propagate an (N_s * N_s) source field (far field) through a starshade to a CCD.    
+    Field incident on starshade is calculated as sum of planar waves for each source pixel.
+    Fresnel diffraction from starshade to telescope, followed by Fraunhofer diffraction from telescope to CCD. 
+    Uses Babinets principle, alongside Bluestein FFTs for high-resolution diffraction. 
+    Based on calculations (Taaki et al. 2023 in prep.).
+
+    Args:
+        source_field (float): N_s * N_s source field
+        wl (float): Wavelength of light.
+        dist_xo_ss (float): Distance between source plane and starshade.
+        dist_ss_t (float): Distance between starshade and telescope.
+        focal_length_lens (float): Focal length of the telescope lens.
+        radius_lens (float): Radius of the telescope lens.
+        N_s (int): Number of pixels in the source field. 
+        N_x (int): Number of non-zero samples in starshade plane. Diameter of the starshade ~ N_x * dx. 
+        N_t (int): Number of output samples in the telescope plane. Diameter of the telescope ~ N_t * dt.
+        N_pix (int): Number of output pixels required.
+        ds (float): Source field sampling
+        dx (float): Input sampling. Default is 0.01.
+        dt (float): Telescope sampling, must be less than (1/dx)*wl*dist_ss_t.
+        dp (float): Pixel size sampling, depends on the telescope and the desired field-of-view. 
+
+    Returns:
+        The resulting field on the CCD plane of size (N_pix, N_pix).
+
+    """
+
+    source_prop = SourceField(ds, N_s, wl, dist_xo_ss, source_field)
+    field_incident_ss = source_prop.farfield(dx, N_x, 0)
+
+    ss_complement = 1-eval_hypergauss(N_x, dx)
+
+    field_after_ss = field_incident_ss * ss_complement 
+    field_after_ss = bluestein_pad(field_after_ss, N_x, N_t)
+
+    fresnel = FresnelSingle(dx, dt, N_x, dist_ss_t, wl)
+    test_new, dt = fresnel.zoom_fresnel_single_fft(field_after_ss, N_t)
+
+    field_free_prop = source_prop.farfield(dt, N_t, dist_ss_t)
+
+    pupil_mask = grey_pupil_func(N_t, dx = dt, r = radius_lens)
+    N_xt, N_yt = N_in_2d(pupil_mask) # Number of non-zero samples in telescope pupil
+
+    field_aperture_freesp = bluestein_pad(field_free_prop*pupil_mask, N_xt, N_pix)
+    field_aperture_ss = bluestein_pad(test_new*pupil_mask, N_xt, N_pix)
+
+    fraunhofer = Fraunhofer(dt, dp, N_xt, focal_length_lens, wl)
+    out_field_free_space, dp = fraunhofer.zoom_fraunhofer(field_aperture_freesp, N_pix)
+    out_field_compl_ss, dp = fraunhofer.zoom_fraunhofer(field_aperture_ss, N_pix)
+
+    out_field_ss = out_field_free_space - out_field_compl_ss
+    return out_field_ss
+
+
+def point_source_to_ccd(mag_s, loc_s, wl, dist_xo_ss, dist_ss_t, focal_length_lens, radius_lens, 
+                        N_x = 6401, N_t = 1001, N_pix = 1001,
                         dx = 0.01, dt = 0.0116, dp=1.9e-7):
     """
     Propagate a collection of point-sources located in the source plane through a starshade to a CCD.
     Sequentially performs Fresnel diffraction from starshade to telescope, followed by Fraunhofer diffraction from telescope to CCD. 
     Uses Babinets principle, alongside Bluestein FFTs for high-resolution diffraction. 
     Based on calculations (Taaki et al. 2023 in prep.).
 
@@ -26,50 +85,54 @@
         dx (float): Input sampling. Default is 0.01.
         dt (float): Telescope sampling, must be less than (1/dx)*wl*dist_ss_t.
         dp (float): Pixel size sampling, depends on the telescope and the desired field-of-view. 
 
     Returns:
         The resulting field on the CCD plane of size (N_pix, N_pix).
 
-    Note:
-        The pixel size sampling (dp) determines the output field-of-view, with a resolution of the system not greater than 0.1 AU.
-        It is desired to have 1 pixel per 0.1 AU. Some examples for calculating dp are provided in the comments.
-        Example calculation: dp = 633e-9 * focal_length_lens / (20 * (2*radius_lens))
     """
 
     N_X = N_x + N_t - 1 # The number of input samples required to perform Fresnel propagation with a Bluestein FFT
 
     no_sources = len(mag_s)
     k_list = []
     pointsource_list = []
     field_incident_ss = np.zeros((N_X, N_X), dtype='complex128')
     for i in range(no_sources):
-        ps = PointSource(dx, N_X, 633e-9, *loc_s[i], mag_s[i])
+        ps = PointSource(dx, N_X, wl, *loc_s[i], mag_s[i])
         pointsource_list.append(ps)
         k_list.append(ps.wave_numbers())
         field_incident_ss += ps.plane_wave(k_list[i], 0)
 
+# optional add Gaussian background dust disk term
+#    gs = GaussianSource(dx, N_X, wl, 0, 0, dist_xo_ss, .75*10e-18, 5*au_to_meter)
+#    gs_A, gs_inv_sigma = gs.far_field_gaussian_params()
+#    field_incident_ss += gs.far_field_gaussian(gs_A, gs_inv_sigma, 0)
+
     ss_complement = 1-eval_hypergauss(N_X, dx) # Complement of starshade aperture
 
     field_after_ss = field_incident_ss * ss_complement
 
-    fresnel = FresnelSingle(dx, dt, N_x, dist_ss_t, 633e-9)
-    test_new, dt = fresnel.zoom_fresnel_single_fft(field_after_ss, N_t)
+    fresnel = FresnelSingle(dx, dt, N_x, dist_ss_t, wl)
+    field_ss_prop, dt = fresnel.zoom_fresnel_single_fft(field_after_ss, N_t)
 
     pupil_mask = grey_pupil_func(N_t, dx = dt, r = radius_lens)
 
     field_free_prop = np.zeros((N_t, N_t), dtype='complex128')
     for i in range(no_sources):
         pointsource_list[i].update(d_x = dt, N = N_t)
         field_free_prop += pointsource_list[i].plane_wave(k_list[i], dist_ss_t)
+   
+#    gs.update(d_x = dt, N = N_t)
+#    field_free_prop += gs.far_field_gaussian(gs_A, gs_inv_sigma, dist_ss_t)
 
     N_xt, N_yt = N_in_2d(pupil_mask) # Number of non-zero samples in telescope pupil
 
     field_aperture_freesp = bluestein_pad(field_free_prop*pupil_mask, N_xt, N_pix)
-    field_aperture_ss = bluestein_pad(test_new*pupil_mask, N_xt, N_pix)
+    field_aperture_ss = bluestein_pad(field_ss_prop*pupil_mask, N_xt, N_pix)
 
-    fraunhofer = Fraunhofer(dt, dp, N_xt, focal_length_lens, 633e-9)
+    fraunhofer = Fraunhofer(dt, dp, N_xt, focal_length_lens, wl)
     out_field_free_space, dp = fraunhofer.zoom_fraunhofer(field_aperture_freesp, N_pix)
     out_field_compl_ss, dp = fraunhofer.zoom_fraunhofer(field_aperture_ss, N_pix)
 
     out_field_ss = out_field_free_space - out_field_compl_ss
     return out_field_ss
```

### Comparing `pystarshade-0.1.2/pystarshade/diffraction/bluestein_fft.py` & `pystarshade-0.1.5/pystarshade/diffraction/bluestein_fft.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import numpy as np
+from diffraction.util import trunc_2d
 
 def zoom_fft_2d_mod(x, N_x, N_out, Z_pad):
     """
     MODIFIED VERSION: computes the Bluestein FFT on fftshift(x) (without explicitly shifting x).
     Compute a zoomed 2D FFT using the Bluestein algorithm. 
     The input x is centered. 
     Args:
@@ -16,16 +17,15 @@
     N_chirp = N_x + N_out - 1
     N_X = Z_pad*N_x + 1 #X before truncation
 
     bit_x = N_x % 2
     bit_chirp = N_chirp % 2
     bit_out = N_out % 2
 
-    trunc_x = x[(x.shape[0]//2) - (N_chirp//2) : (x.shape[0]//2) + (N_chirp//2) + bit_x, 
-                (x.shape[1]//2) - (N_chirp//2) : (x.shape[1]//2) + (N_chirp//2) + bit_x]
+    trunc_x = trunc_2d(x, N_chirp)
 
     b = np.exp(-1*np.pi*(1/(N_X))*1j*np.arange(- (N_chirp//2), (N_chirp//2) + bit_chirp)**2)
     h = np.exp(   np.pi*(1/(N_X))*1j*np.arange(- (N_out//2) - (N_x//2) , (N_out//2) + (N_x//2) + bit_chirp)**2)
     h = np.roll(h, (N_chirp//2) + 1)
     ft_h = np.fft.fft(h)
 
     zoom_fft = np.outer(b, b) * (np.fft.ifft2( np.fft.fft2(np.outer(b, b) * trunc_x) * np.outer(ft_h, ft_h) ) )
```

### Comparing `pystarshade-0.1.2/pystarshade/diffraction/diffract.py` & `pystarshade-0.1.5/pystarshade/diffraction/diffract.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,14 @@
             wavelength : Wavelength of the light.
             z: Propagation distance in m.
 
         Returns:
             float: Zero-padding factor (ZP * N_in) to achieve the desired frequency spacing.
         """
         ZP = ((self.max_freq * self.wl_z / self.d_f) - 1) / self.N_in
-        ZP = np.ceil(ZP)
-        ZP += ZP % 2
         return ZP
 
     def zoom_fresnel_single_fft(self, field, N_out):
         """
         Single FFT fresnel diffraction using Bluestein FFT
 
         Output on grid defined by (N_out/ZP*N_in)*wl_z/d_x, (N_out/ZP*N_in)*wl_z/d_x
```

### Comparing `pystarshade-0.1.2/README.md` & `pystarshade-0.1.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
 ## Overview
 
 Developed by Jamila Taaki (UIUC).
 
-PyStarshade is a Python library for computing end-to-end Starshade simulations with Fresnel diffraction methods. This library efficiently calculates output fields using Bluestein FFTs.
+PyStarshade is a Python library for Starshade simulations from star-planet system to CCD with Fresnel diffraction methods. This library efficiently calculates output fields using Bluestein FFTs.
 
-What is a Bluestein FFT? The Bluestein Fast Fourier Transform (1968) is an algorithm that computes M equispaced samples of the Discrete-Time Fourier Transform (DTFT) over an arbitrary frequency region between [0, 1/dx] for a compact input signal containing N non-zero samples, each with a size of dx. The computational complexity of this method in one dimension is O((N+M)log(N+M)). The Bluestein FFT is particularly advantageous when large zero-padding factors would be needed for performing the calculation using a direct FFT.
+What is a Bluestein FFT? The Bluestein Fast Fourier Transform (1968) is an algorithm that computes M equispaced samples of the Discrete-Time Fourier Transform (DTFT) over an arbitrary frequency region between [0, 1/dx] for a compact input signal containing N non-zero samples, each with a size of dx. The computational complexity of this method in one dimension is O((N+M)log(N+M)). The Bluestein FFT is particularly advantageous when large zero-padding factors would be needed for performing optical propagation using FFT's.
 
 This means that end-to-end simulation can be performed with arbitrary high-resolution sampling in each plane of propagation. 
 
 This library is compatible with Python 3.6 and later versions. 
 
 
 ## Example
-Log starlight supression with a truncated Hypergaussian apodization, sweeping star planet brightness ratios between (10e-8, 10e-3). Planet at a 0.2 au separation and 10 pc distance from Earth. 
+Log starlight supression with a truncated Hypergaussian apodization, sweeping star planet brightness ratios between (10e-8, 10e-3). Planet at a 2 AU separation and 10 pc distance from Earth. 
 <p align="center">
   <img src="images/contrast_.gif" alt="Star planet brightness ratio range (10e-8, 10e-3)">
 </p>
 
 ## Installation
 
 You can install PyStarshade using pip:
@@ -30,38 +30,43 @@
 ```
 
 ## Dependencies
 
 Scipy, Numpy
 
 ## Quickstart
-See simulate_field.py
+import pystarshade
+
 Nominal parameters: 
 
 ## Organization
 
 <pre>
 Pystarshade
+├── examples
+│   ├── haystacks_model.py
+│   └── star_exo.py
 ├── images
-│   └── contrast_.gif
+│   └── contrast_.gif
+├── __init__.py
+├── pystarshade
+│   ├── apodization
+│   │   ├── apodization.py
+│   │   ├── __init__.py
+│   │   └── sample.py
+│   ├── diffraction
+│   │   ├── bluestein_fft.py
+│   │   ├── diffract.py
+│   │   ├── field.py
+│   │   ├── __init__.py
+│   │   └── util.py
+│   ├── __init__.py
+│   ├── simulate_field.py
+│   └── version.py
 ├── README.md
-├── setup.py
-└── starshade
-    ├── apodization
-    │   ├── apodization.py
-    │   ├── __init__.py
-    │   └── sample.py
-    ├── diffraction
-    │   ├── bluestein_fft.py
-    │   ├── diffract.py
-    │   ├── field.py
-    │   ├── __init__.py
-    │   └── util.py
-    ├── example_star_exo.py
-    ├── __init__.py
-    ├── simulate_field.py
-    └── version.py
+└── setup.py
+
 </pre>
 
 ## License
 
 [PyStarshade] is released under the [GNU General Public License v3.0](LICENSE).
```

### Comparing `pystarshade-0.1.2/pystarshade.egg-info/PKG-INFO` & `pystarshade-0.1.5/pystarshade.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.2
+Version: 0.1.5
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pystarshade-0.1.2/pystarshade.egg-info/SOURCES.txt` & `pystarshade-0.1.5/pystarshade.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 README.md
 setup.py
 pystarshade/__init__.py
-pystarshade/example_star_exo.py
 pystarshade/simulate_field.py
 pystarshade/version.py
 pystarshade.egg-info/PKG-INFO
 pystarshade.egg-info/SOURCES.txt
 pystarshade.egg-info/dependency_links.txt
 pystarshade.egg-info/requires.txt
 pystarshade.egg-info/top_level.txt
 pystarshade/apodization/__init__.py
-pystarshade/apodization/apodization.py
-pystarshade/apodization/sample.py
+pystarshade/apodization/apodize.py
 pystarshade/diffraction/__init__.py
 pystarshade/diffraction/bluestein_fft.py
 pystarshade/diffraction/diffract.py
 pystarshade/diffraction/field.py
 pystarshade/diffraction/util.py
```

### Comparing `pystarshade-0.1.2/setup.py` & `pystarshade-0.1.5/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pystarshade",
-    version="0.1.2",
+    version="0.1.5",
     description="A python package for end-to-end starshade simulation",
     author="Jamila Taaki",
     author_email="xiaziyna@gmail.com",
     url="https://github.com/xiaziyna/PyStarshade",
     packages=find_packages(),
     install_requires=[
         "numpy",
```

### Comparing `pystarshade-0.1.2/PKG-INFO` & `pystarshade-0.1.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystarshade
-Version: 0.1.2
+Version: 0.1.5
 Summary: A python package for end-to-end starshade simulation
 Home-page: https://github.com/xiaziyna/PyStarshade
 Author: Jamila Taaki
 Author-email: xiaziyna@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
```

