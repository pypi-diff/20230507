# Comparing `tmp/mpl-smithchart-0.1.1.tar.gz` & `tmp/mpl-smithchart-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpl-smithchart-0.1.1.tar", last modified: Fri May  5 23:32:57 2023, max compression
+gzip compressed data, was "mpl-smithchart-0.1.2.tar", last modified: Sat May  6 22:25:47 2023, max compression
```

## Comparing `mpl-smithchart-0.1.1.tar` & `mpl-smithchart-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.763656 mpl-smithchart-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     4358 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/mpl_smithchart/
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    60665 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/smithaxes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/mpl_smithchart/smithhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 23:32:57.000000 mpl-smithchart-0.1.1/mpl_smithchart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    87334 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:32:57.763656 mpl-smithchart-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:32:57.759656 mpl-smithchart-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/tests/plotting_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 23:32:41.000000 mpl-smithchart-0.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.555513 mpl-smithchart-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4557 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/mpl_smithchart/
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/mpl_smithchart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60634 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/mpl_smithchart/smithaxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/mpl_smithchart/smithhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 22:25:47.000000 mpl-smithchart-0.1.2/mpl_smithchart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    87334 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 22:25:47.559513 mpl-smithchart-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/tests/plotting_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-06 22:25:32.000000 mpl-smithchart-0.1.2/tox.ini
```

### Comparing `mpl-smithchart-0.1.1/.github/workflows/ci.yml` & `mpl-smithchart-0.1.2/.github/workflows/ci.yml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 jobs:
   build:
     name: Python ${{matrix.python-version}}
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        python-version: [3.8, 3.9]
+        python-version: [3.8, 3.9, '3.10']
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{matrix.python-version}}
       uses: actions/setup-python@v4
       with:
```

### Comparing `mpl-smithchart-0.1.1/.gitignore` & `mpl-smithchart-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.1/.pre-commit-config.yaml` & `mpl-smithchart-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.1/COPYING` & `mpl-smithchart-0.1.2/COPYING`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.1/PKG-INFO` & `mpl-smithchart-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: mpl-smithchart
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extension for matplotlib providing a projection class to generate high quality Smith Chart plots.
 Author-email: Paul Staerke <paul.staerke@gmail.com>, Spencer Chang <spencer@sycee.xyz>
 License: BSD
 Project-URL: repository, https://github.com/schang412/mpl-smithchart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # mpl-smithchart
 
 [![ci](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml/badge.svg)](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml)
 
-This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot). It adds CI/CD automation to facilitate maintenance of the package.
+This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot).
+
+It adds/fixes the following:
+- CI/CD to facillitate package maintenance
+- addresses matplotlib deprecation warnings
+- updates numpy to newer version
+- fixes legend plotting
+- adds some automated testing of features
+- adds version lock file to show known-good build
 
 Below this line is the old README.
 ---
 
 ## New Release of Version 0.2
 
 After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
```

### Comparing `mpl-smithchart-0.1.1/README.md` & `mpl-smithchart-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # mpl-smithchart
 
 [![ci](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml/badge.svg)](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml)
 
-This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot). It adds CI/CD automation to facilitate maintenance of the package.
+This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot).
+
+It adds/fixes the following:
+- CI/CD to facillitate package maintenance
+- addresses matplotlib deprecation warnings
+- updates numpy to newer version
+- fixes legend plotting
+- adds some automated testing of features
+- adds version lock file to show known-good build
 
 Below this line is the old README.
 ---
 
 ## New Release of Version 0.2
 
 After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
```

### Comparing `mpl-smithchart-0.1.1/mpl_smithchart/smithaxes.py` & `mpl-smithchart-0.1.2/mpl_smithchart/smithaxes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# last edit: 11.04.2018
 '''
 Library for plotting fully automatic a Smith Chart with various customizable
 parameters and well selected default values. It also provides the following
 modifications and features:
 
     - circle shaped drawing area with labels placed around
     - :meth:`plot` accepts single real and complex numbers and numpy.ndarray's
@@ -411,27 +410,27 @@
             raise KeyError("%s is not a valid key" % key)
 
     def _init_axis(self):
         self.xaxis = mp.axis.XAxis(self)
         self.yaxis = mp.axis.YAxis(self)
         self._update_transScale()
 
-    def cla(self):
+    def clear(self):
         self._majorarcs = []
         self._minorarcs = []
 
         # deactivate grid function when calling base class
         tgrid = self.grid
 
         def dummy(*args, **kwargs):
             pass
 
         self.grid = dummy
         # Don't forget to call the base class
-        Axes.cla(self)
+        Axes.clear(self)
         self.grid = tgrid
 
         self._normbox = None
         self._impedance = self._get_key("axes.impedance")
         self._normalize = self._get_key("axes.normalize")
         self._current_zorder = self._get_key("plot.zorder")
 
@@ -457,28 +456,28 @@
 
         for tick, loc in zip(
             self.yaxis.get_major_ticks(),
             self.yaxis.get_majorticklocs(),
         ):
             # workaround for fixing to small infinity symbol
             if abs(loc) > self._near_inf:
-                tick.label.set_size(
-                    tick.label.get_size() +
+                tick.label1.set_size(
+                    tick.label1.get_size() +
                     self._get_key("symbol.infinity.correction"),
                 )
 
-            tick.label.set_verticalalignment('center')
+            tick.label1.set_verticalalignment('center')
 
             x = np.real(self._moebius_z(loc * 1j))
             if x < -0.1:
-                tick.label.set_horizontalalignment('right')
+                tick.label1.set_horizontalalignment('right')
             elif x > 0.1:
-                tick.label.set_horizontalalignment('left')
+                tick.label1.set_horizontalalignment('left')
             else:
-                tick.label.set_horizontalalignment('center')
+                tick.label1.set_horizontalalignment('center')
 
         self.yaxis.set_major_formatter(self.ImagFormatter(self))
         self.xaxis.set_major_formatter(self.RealFormatter(self))
 
         if self._get_key("axes.normalize") and self._get_key("axes.normalize.label"):
             x, y = z_to_xy(self._moebius_inv_z(-1 - 1j))
             box = self.text(
@@ -520,15 +519,15 @@
 
     def get_yaxis_transform(self, which='grid'):
         assert which in ['tick1', 'tick2', 'grid']
         return self._yaxis_transform
 
     def get_yaxis_text1_transform(self, pixelPad):
         if hasattr(self, 'yaxis') and len(self.yaxis.majorTicks) > 0:
-            font_size = self.yaxis.majorTicks[0].label.get_size()
+            font_size = self.yaxis.majorTicks[0].label1.get_size()
         else:
             font_size = self._get_key("font.size")
 
         offset = self._get_key("axes.ylabel.correction")[2]
         return (
             self._yaxis_text1_transform
             + self.PolarTranslate(
@@ -677,22 +676,22 @@
 
         class SmithHandlerLine2D(HandlerLine2D):
             def create_artists(
                 self, legend, orig_handle,
                 xdescent, ydescent, width, height, fontsize,
                 trans,
             ):
-                legline, legline_marker = HandlerLine2D.create_artists(
+                legline = HandlerLine2D.create_artists(
                     self, legend, orig_handle, xdescent, ydescent,
                     width, height, fontsize, trans,
                 )
 
                 if hasattr(orig_handle, "_markerhacked"):
-                    this_axes._hack_linedraw(legline_marker, True)
-                return legline, legline_marker
+                    this_axes._hack_linedraw(legline[0], True)
+                return legline
 
         return Axes.legend(self, *args, handler_map={Line2D: SmithHandlerLine2D()}, **kwargs)
 
     def plot(self, *args, **kwargs):
         '''
         Plot the given data into the Smith Chart. Behavior similar to basic
         :meth:`matplotlib.axes.Axes.plot`, but with some extensions:
@@ -755,15 +754,15 @@
                 except TypeError:
                     pass
 
             # if (converted) arg is an ndarray of complex type, split it
             if isinstance(arg, np.ndarray) and arg.dtype in [complex, np.complex128]:
                 new_args += z_to_xy(arg)
             else:
-                new_args += (arg,)
+                new_args += (arg, np.zeros_like(arg))
 
         # ensure newer plots are above older ones
         if 'zorder' not in kwargs:
             kwargs['zorder'] = self._current_zorder
             self._current_zorder += 0.001
 
         # extract or load non-matplotlib keyword arguments from parameters
```

### Comparing `mpl-smithchart-0.1.1/mpl_smithchart/smithhelper.py` & `mpl-smithchart-0.1.2/mpl_smithchart/smithhelper.py`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.1/mpl_smithchart.egg-info/PKG-INFO` & `mpl-smithchart-0.1.2/mpl_smithchart.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 Metadata-Version: 2.1
 Name: mpl-smithchart
-Version: 0.1.1
+Version: 0.1.2
 Summary: An extension for matplotlib providing a projection class to generate high quality Smith Chart plots.
 Author-email: Paul Staerke <paul.staerke@gmail.com>, Spencer Chang <spencer@sycee.xyz>
 License: BSD
 Project-URL: repository, https://github.com/schang412/mpl-smithchart
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: COPYING
 
 # mpl-smithchart
 
 [![ci](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml/badge.svg)](https://github.com/schang412/mpl-smithchart/actions/workflows/ci.yml)
 
-This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot). It adds CI/CD automation to facilitate maintenance of the package.
+This project is forked from [pySmithPlot](https://github.com/vMeijin/pySmithPlot).
+
+It adds/fixes the following:
+- CI/CD to facillitate package maintenance
+- addresses matplotlib deprecation warnings
+- updates numpy to newer version
+- fixes legend plotting
+- adds some automated testing of features
+- adds version lock file to show known-good build
 
 Below this line is the old README.
 ---
 
 ## New Release of Version 0.2
 
 After 2 years of getting dusty **pySmithPlot** now got some new features and bug fixes. Here is a short changelog:
```

### Comparing `mpl-smithchart-0.1.1/pdm.lock` & `mpl-smithchart-0.1.2/pdm.lock`

 * *Files identical despite different names*

### Comparing `mpl-smithchart-0.1.1/pyproject.toml` & `mpl-smithchart-0.1.2/pyproject.toml`

 * *Files identical despite different names*

