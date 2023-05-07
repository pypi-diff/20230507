# Comparing `tmp/qudi_hira_analysis-1.4.7.tar.gz` & `tmp/qudi_hira_analysis-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qudi_hira_analysis-1.4.7.tar", max compression
+gzip compressed data, was "qudi_hira_analysis-1.4.8.tar", max compression
```

## Comparing `qudi_hira_analysis-1.4.7.tar` & `qudi_hira_analysis-1.4.8.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1069 2023-02-26 15:52:31.954729 qudi_hira_analysis-1.4.7/LICENSE
--rw-r--r--   0        0        0    13537 2023-05-05 08:04:35.317049 qudi_hira_analysis-1.4.7/README.md
--rw-r--r--   0        0        0      928 2023-05-05 09:40:20.528557 qudi_hira_analysis-1.4.7/pyproject.toml
--rw-r--r--   0        0        0      171 2023-03-05 21:19:20.709702 qudi_hira_analysis-1.4.7/qudi_hira_analysis/__init__.py
--rw-r--r--   0        0        0    11333 2023-05-04 17:12:59.438304 qudi_hira_analysis-1.4.7/qudi_hira_analysis/analysis_logic.py
--rw-r--r--   0        0        0    13663 2023-05-05 06:54:48.308721 qudi_hira_analysis-1.4.7/qudi_hira_analysis/data_handler.py
--rw-r--r--   0        0        0        0 2023-03-05 21:19:20.710018 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/__init__.py
--rw-r--r--   0        0        0     1936 2023-03-05 21:19:20.710848 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/antibunchingmethods.py
--rw-r--r--   0        0        0    24480 2023-03-05 21:19:20.711380 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/decaylikemethods.py
--rw-r--r--   0        0        0    40854 2023-03-05 21:19:20.711692 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
--rw-r--r--   0        0        0    23135 2023-05-04 17:12:59.439365 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/generalmethods.py
--rw-r--r--   0        0        0     5848 2023-03-05 21:19:20.712252 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
--rw-r--r--   0        0        0    10577 2023-03-05 21:19:20.712412 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/linearmethods.py
--rw-r--r--   0        0        0    41457 2023-03-05 21:19:20.712635 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
--rw-r--r--   0        0        0    16450 2023-03-05 21:19:20.712885 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
--rw-r--r--   0        0        0   106110 2023-03-05 21:19:20.713199 qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/sinemethods.py
--rw-r--r--   0        0        0     1792 2023-04-12 17:43:42.063526 qudi_hira_analysis-1.4.7/qudi_hira_analysis/helper_functions.py
--rw-r--r--   0        0        0    13657 2023-05-04 17:12:59.439937 qudi_hira_analysis-1.4.7/qudi_hira_analysis/io_handler.py
--rw-r--r--   0        0        0     6753 2023-05-05 09:23:13.898423 qudi_hira_analysis-1.4.7/qudi_hira_analysis/measurement_dataclass.py
--rw-r--r--   0        0        0    18711 2023-05-04 17:12:59.440573 qudi_hira_analysis-1.4.7/qudi_hira_analysis/qudi_fit_logic.py
--rw-r--r--   0        0        0    14535 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.7/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-03-04 13:38:16.100952 qudi_hira_analysis-1.4.8/LICENSE
+-rw-r--r--   0        0        0      963 2023-05-07 10:54:15.037621 qudi_hira_analysis-1.4.8/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-03-05 20:29:56.471910 qudi_hira_analysis-1.4.8/qudi_hira_analysis/__init__.py
+-rw-r--r--   0        0        0    11605 2023-05-02 16:38:14.760200 qudi_hira_analysis-1.4.8/qudi_hira_analysis/analysis_logic.py
+-rw-r--r--   0        0        0    14131 2023-05-07 10:33:43.608599 qudi_hira_analysis-1.4.8/qudi_hira_analysis/data_handler.py
+-rw-r--r--   0        0        0        0 2023-03-05 20:20:55.998728 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/__init__.py
+-rw-r--r--   0        0        0     1992 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/antibunchingmethods.py
+-rw-r--r--   0        0        0    25064 2023-01-10 21:18:35.126407 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/decaylikemethods.py
+-rw-r--r--   0        0        0    41794 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/gaussianlikemethods.py
+-rw-r--r--   0        0        0    23680 2023-05-03 10:28:04.680129 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/generalmethods.py
+-rw-r--r--   0        0        0     5998 2023-03-05 20:29:56.434172 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py
+-rw-r--r--   0        0        0    10849 2023-03-05 20:29:56.418510 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/linearmethods.py
+-rw-r--r--   0        0        0    42414 2023-03-05 20:29:56.402925 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py
+-rw-r--r--   0        0        0    16836 2023-03-05 20:29:56.449756 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/poissonianlikemethods.py
+-rw-r--r--   0        0        0   108340 2023-04-03 12:15:20.198945 qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/sinemethods.py
+-rw-r--r--   0        0        0     1854 2023-03-09 22:52:17.007898 qudi_hira_analysis-1.4.8/qudi_hira_analysis/helper_functions.py
+-rw-r--r--   0        0        0    13999 2023-05-03 10:06:55.899922 qudi_hira_analysis-1.4.8/qudi_hira_analysis/io_handler.py
+-rw-r--r--   0        0        0     6955 2023-05-07 10:33:43.609598 qudi_hira_analysis-1.4.8/qudi_hira_analysis/measurement_dataclass.py
+-rw-r--r--   0        0        0    19138 2023-04-17 14:03:20.837890 qudi_hira_analysis-1.4.8/qudi_hira_analysis/qudi_fit_logic.py
+-rw-r--r--   0        0        0    14433 2023-05-07 10:54:00.298947 qudi_hira_analysis-1.4.8/README.md
+-rw-r--r--   0        0        0    15379 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.8/setup.py
+-rw-r--r--   0        0        0    15032 1970-01-01 00:00:00.000000 qudi_hira_analysis-1.4.8/PKG-INFO
```

### Comparing `qudi_hira_analysis-1.4.7/LICENSE` & `qudi_hira_analysis-1.4.8/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 Dinesh Pinto
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 Dinesh Pinto
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `qudi_hira_analysis-1.4.7/README.md` & `qudi_hira_analysis-1.4.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: qudi-hira-analysis
+Version: 1.4.8
+Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
+Home-page: https://github.com/dineshpinto/qudi-hira-analysis
+License: MIT
+Keywords: python,qubit,analysis,nv centers,photon timetrace
+Author: dineshpinto
+Author-email: annual.fallout_0z@icloud.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: lmfit (>=1.1.0,<2.0.0)
+Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
+Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pyspm (>=0.3.0,<0.4.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: xlrd (>=2.0.1,<3.0.0)
+Project-URL: Repository, https://github.com/dineshpinto/qudi-hira-analysis
+Description-Content-Type: text/markdown
+
 [![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)
 [![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)
 [![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)
 [![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)
 [![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)
 [![codecov](https://codecov.io/gh/dineshpinto/qudi-hira-analysis/branch/main/graph/badge.svg?token=FMXDAYW8DW)](https://codecov.io/gh/dineshpinto/qudi-hira-analysis)
 
@@ -26,14 +51,20 @@
 
 ## Installation
 
 ```bash
 pip install qudi-hira-analysis
 ```
 
+### Update to latest version
+
+```bash
+pip install --upgrade qudi-hira-analysis
+```
+
 ## Citation
 
 If you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670
 
 ## Examples
 
 First set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure
@@ -141,22 +172,22 @@
 
 ```python
 autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
 
 fig, ax = plt.subplots()
 
 for autocorrelation in autocorrelation_measurements.values():
-  autocorrelation.data["Time (ns)"] = autocorrelation.data["Time (ps)"] * 1e-3
-  # Plot the data
-  sns.lineplot(data=autocorrelation.data, x="Time (ns)", y="g2(t) norm", ax=ax)
-  # Fit the data using the antibunching function
-  fit_x, fit_y, result = dh.fit(x="Time (ns)", y="g2(t) norm", data=autocorrelation.data,
-                                fit_function=dh.fit_function.antibunching)
-  # Plot the fit
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")
+    autocorrelation.data["Time (ns)"] = autocorrelation.data["Time (ps)"] * 1e-3
+    # Plot the data
+    sns.lineplot(data=autocorrelation.data, x="Time (ns)", y="g2(t) norm", ax=ax)
+    # Fit the data using the antibunching function
+    fit_x, fit_y, result = dh.fit(x="Time (ns)", y="g2(t) norm", data=autocorrelation.data,
+                                  fit_function=dh.fit_function.antibunching)
+    # Plot the fit
+    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")
 
 # Save the figure to the figure folder specified earlier
 dh.save_figures(filepath="autocorrelation_variation", fig=fig)
 ```
 
 ### Example 3: ODMR measurements (double Lorentzian fit)
 
@@ -189,23 +220,34 @@
 
 dh.save_figures(filepath="rabi_variation", fig=fig)
 ```
 
 ### Example 5: Temperature data
 
 ```python
-temperature_measurements = dh.load_measurements(measurement_str="Temperature")
+temperature_measurements = dh.load_measurements(measurement_str="Temperature", qudi=False)
 
 temperature = pd.concat([t.data for t in temperature_measurements.values()])
 
 fig, ax = plt.subplots()
 sns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)
 dh.save_figures(filepath="temperature_monitoring", fig=fig)
 ```
 
+### Example 6: PYS data (pi3diamond compatibility)
+
+```python
+pys_measurements = dh.load_measurements(measurement_str="ndmin", extension=".pys", qudi=False)
+pys = pys_measurements[list(pys_measurements)[0]].data
+
+fig, ax = plt.subplots()
+sns.lineplot(x=pys["time_bins"], y=pys["counts"], ax=ax)
+dh.save_figures(filepath="pys_measurement", fig=fig)
+```
+
 ## Measurement Dataclass Schema
 
 ```mermaid
 flowchart LR
     subgraph Standard Data
         MeasurementDataclass --o filepath1[filepath: Path];
         MeasurementDataclass --o data1[data: DataFrame];
@@ -229,15 +271,16 @@
         RawTimetrace --o data4[data: DataFrame];
         RawTimetrace --o params4[params: dict];
     end
 ```
 
 ## Supports common fitting routines
 
-To get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:
+To get the full list of available fit routines, explore the `dh.fit_function` attribute or call `dh.get_all_fits()`. The
+fit functions are:
 
 | Dimension | Fit                           |
 |-----------|-------------------------------|
 | 1d        | decayexponential              |
 |           | biexponential                 |
 |           | decayexponentialstretched     |
 |           | gaussian                      |
@@ -375,7 +418,8 @@
 + `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)
 + `make html`: Converts all notebooks to HTML
 + `make py`  : Converts all notebooks to Python (can be useful for VCS)
 + `make all` : Sequentially runs all the notebooks in folder
 
 To use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then
 install make with `choco install make`
+
```

### Comparing `qudi_hira_analysis-1.4.7/pyproject.toml` & `qudi_hira_analysis-1.4.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-[tool.poetry]
-name = "qudi-hira-analysis"
-version = "1.4.7"
-repository = "https://github.com/dineshpinto/qudi-hira-analysis"
-homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
-keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
-description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
-authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{ include = "qudi_hira_analysis" }]
-
-[tool.poetry.dependencies]
-python = "^3.10"
-lmfit = "^1.1.0"
-matplotlib = "^3.6.2"
-numpy = "^1.24.0"
-pandas = "^2.0.0"
-xlrd = "^2.0.1"
-openpyxl = "^3.0.10"
-tqdm = "^4.64.1"
-pyspm = "^0.3.0"
-
-[tool.poetry.group.dev.dependencies]
-seaborn = "^0.12.2"
-jupyterlab = "^3.6.2"
-notebook = "^6.5.4"
-
-
-[tool.poetry.group.test.dependencies]
-coverage = "^7.2.5"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "qudi-hira-analysis"
+version = "1.4.8"
+repository = "https://github.com/dineshpinto/qudi-hira-analysis"
+homepage = "https://github.com/dineshpinto/qudi-hira-analysis"
+keywords = ["python", "qubit", "analysis", "nv centers", "photon timetrace"]
+description = "A Python toolkit to analzye photon timetrace data from qubit sensors"
+authors = ["dineshpinto <annual.fallout_0z@icloud.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{ include = "qudi_hira_analysis" }]
+
+[tool.poetry.dependencies]
+python = "^3.10"
+lmfit = "^1.1.0"
+matplotlib = "^3.6.2"
+numpy = "^1.24.0"
+pandas = "^2.0.0"
+xlrd = "^2.0.1"
+openpyxl = "^3.0.10"
+tqdm = "^4.64.1"
+pyspm = "^0.3.0"
+
+[tool.poetry.group.dev.dependencies]
+seaborn = "^0.12.2"
+jupyterlab = "^3.6.2"
+notebook = "^6.5.4"
+
+
+[tool.poetry.group.test.dependencies]
+coverage = "^7.2.5"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/analysis_logic.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/analysis_logic.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-from __future__ import annotations
-
-import logging
-from typing import Tuple, TYPE_CHECKING
-
-import numpy as np
-import pandas as pd
-
-from qudi_hira_analysis.qudi_fit_logic import FitLogic
-
-if TYPE_CHECKING:
-    from lmfit.model import ModelResult
-
-logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
-
-
-class FitMethodsAndEstimators:
-    # Fit methods with corresponding estimators
-    antibunching: tuple = ("antibunching", "dip")
-    hyperbolicsaturation: tuple = ("hyperbolicsaturation", "generic")
-    lorentzian: tuple = ("lorentzian", "dip")
-    lorentziandouble: tuple = ("lorentziandouble", "dip")
-    sineexponentialdecay: tuple = ("sineexponentialdecay", "generic")
-    decayexponential: tuple = ("decayexponential", "generic")
-    gaussian: tuple = ("gaussian", "dip")
-    gaussiandouble: tuple = ("gaussiandouble", "dip")
-    gaussianlinearoffset: tuple = ("gaussianlinearoffset", "dip")
-    lorentziantriple: tuple = ("lorentziantriple", "dip")
-    biexponential: tuple = ("biexponential", "generic")
-    decayexponentialstretched: tuple = ("decayexponentialstretched", "generic")
-    linear: tuple = ("linear", "generic")
-    sine: tuple = ("sine", "generic")
-    sinedouble: tuple = ("sinedouble", "generic")
-    sinedoublewithexpdecay: tuple = ("sinedoublewithexpdecay", "generic")
-    sinedoublewithtwoexpdecay: tuple = ("sinedoublewithtwoexpdecay", "generic")
-    sinestretchedexponentialdecay: tuple = ("sinestretchedexponentialdecay", "generic")
-    sinetriple: tuple = ("sinetriple", "generic")
-    sinetriplewithexpdecay: tuple = ("sinetriplewithexpdecay", "generic")
-    sinetriplewiththreeexpdecay: tuple = ("sinetriplewiththreeexpdecay", "generic")
-    twoDgaussian: tuple = ("twoDgaussian", "generic")
-
-
-class AnalysisLogic(FitLogic):
-    fit_function = FitMethodsAndEstimators
-
-    def __init__(self):
-        super().__init__()
-        self.log = logging.getLogger(__name__)
-
-    def _perform_fit(
-            self,
-            x: np.ndarray,
-            y: np.ndarray,
-            fit_function: str,
-            estimator: str,
-            dims: str = "1d") -> Tuple[np.ndarray, np.ndarray, ModelResult]:
-        """
-        Fits available:
-            | Dimension | Fit                           |
-            |-----------|-------------------------------|
-            | 1d        | decayexponential              |
-            |           | biexponential                 |
-            |           | decayexponentialstretched     |
-            |           | gaussian                      |
-            |           | gaussiandouble                |
-            |           | gaussianlinearoffset          |
-            |           | hyperbolicsaturation          |
-            |           | linear                        |
-            |           | lorentzian                    |
-            |           | lorentziandouble              |
-            |           | lorentziantriple              |
-            |           | sine                          |
-            |           | sinedouble                    |
-            |           | sinedoublewithexpdecay        |
-            |           | sinedoublewithtwoexpdecay     |
-            |           | sineexponentialdecay          |
-            |           | sinestretchedexponentialdecay |
-            |           | sinetriple                    |
-            |           | sinetriplewithexpdecay        |
-            |           | sinetriplewiththreeexpdecay   |
-            | 2d        | twoDgaussian                  |
-        Estimators:
-            - generic
-            - dip
-        """
-        fit = {dims: {'default': {'fit_function': fit_function, 'estimator': estimator}}}
-        user_fit = self.validate_load_fits(fit)
-
-        use_settings = {}
-        for key in user_fit[dims]["default"]["parameters"].keys():
-            use_settings[key] = False
-        user_fit[dims]["default"]["use_settings"] = use_settings
-
-        fc = self.make_fit_container("test", dims)
-        fc.set_fit_functions(user_fit[dims])
-        fc.set_current_fit("default")
-        fc.use_settings = None
-        fit_x, fit_y, result = fc.do_fit(x, y)
-        return fit_x, fit_y, result
-
-    def fit(
-            self,
-            x: str | np.ndarray | pd.Series,
-            y: str | np.ndarray | pd.Series,
-            fit_function: FitMethodsAndEstimators,
-            data: pd.DataFrame = None,
-    ) -> Tuple[np.ndarray, np.ndarray, ModelResult]:
-        if "twoD" in fit_function[0]:
-            dims = "2d"
-        else:
-            dims = "1d"
-
-        if data is None:
-            if isinstance(x, pd.Series) or isinstance(x, pd.Index):
-                x = x.to_numpy()
-            if isinstance(y, pd.Series):
-                y = y.to_numpy()
-        elif isinstance(data, pd.DataFrame):
-            x = data[x].to_numpy()
-            y = data[y].to_numpy()
-        else:
-            raise TypeError("Data must be a pandas DataFrame or None")
-
-        return self._perform_fit(
-            x=x,
-            y=y,
-            fit_function=fit_function[0],
-            estimator=fit_function[1],
-            dims=dims
-        )
-
-    def get_all_fits(self) -> Tuple[list, list]:
-        one_d_fits = list(self.fit_list['1d'].keys())
-        two_d_fits = list(self.fit_list['2d'].keys())
-        self.log.info(f"1d fits: {one_d_fits}\n2d fits: {two_d_fits}")
-        return one_d_fits, two_d_fits
-
-    @staticmethod
-    def analyse_mean(
-            laser_data: np.ndarray,
-            signal_start: float = 100e-9,
-            signal_end: float = 300e-9,
-            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
-        # Get number of lasers
-        num_of_lasers = laser_data.shape[0]
-
-        if not isinstance(bin_width, float):
-            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
-
-        # Convert the times in seconds to bins (i.e. array indices)
-        signal_start_bin = round(signal_start / bin_width)
-        signal_end_bin = round(signal_end / bin_width)
-
-        # initialize data arrays for signal and measurement error
-        signal_data = np.empty(num_of_lasers, dtype=float)
-        error_data = np.empty(num_of_lasers, dtype=float)
-
-        # loop over all laser pulses and analyze them
-        for ii, laser_arr in enumerate(laser_data):
-            # calculate the mean of the data in the signal window
-            signal = laser_arr[signal_start_bin:signal_end_bin].mean()
-            signal_sum = laser_arr[signal_start_bin:signal_end_bin].sum()
-            signal_error = np.sqrt(signal_sum) / (signal_end_bin - signal_start_bin)
-
-            # Avoid numpy C type variables overflow and NaN values
-            if signal < 0 or signal != signal:
-                signal_data[ii] = 0.0
-                error_data[ii] = 0.0
-            else:
-                signal_data[ii] = signal
-                error_data[ii] = signal_error
-
-        return signal_data, error_data
-
-    @staticmethod
-    def analyse_mean_reference(
-            laser_data: np.ndarray,
-            signal_start: float = 100e-9,
-            signal_end: float = 300e-9,
-            norm_start: float = 1000e-9,
-            norm_end: float = 2000e-9,
-            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
-        """
-        This method takes the mean of the signal window.
-        It then does not divide by the background window to normalize
-        but rather substracts the background window to generate the output.
-        """
-        # Get number of lasers
-        num_of_lasers = laser_data.shape[0]
-
-        if not isinstance(bin_width, float):
-            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
-
-        # Convert the times in seconds to bins (i.e. array indices)
-        signal_start_bin = round(signal_start / bin_width)
-        signal_end_bin = round(signal_end / bin_width)
-        norm_start_bin = round(norm_start / bin_width)
-        norm_end_bin = round(norm_end / bin_width)
-
-        # initialize data arrays for signal and measurement error
-        signal_data = np.empty(num_of_lasers, dtype=float)
-        error_data = np.empty(num_of_lasers, dtype=float)
-
-        # loop over all laser pulses and analyze them
-        for ii, laser_arr in enumerate(laser_data):
-            # calculate the sum and mean of the data in the normalization window
-            tmp_data = laser_arr[norm_start_bin:norm_end_bin]
-            reference_sum = np.sum(tmp_data)
-            reference_mean = (reference_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
-
-            # calculate the sum and mean of the data in the signal window
-            tmp_data = laser_arr[signal_start_bin:signal_end_bin]
-            signal_sum = np.sum(tmp_data)
-            signal_mean = (signal_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
-
-            signal_data[ii] = signal_mean - reference_mean
-
-            # calculate with respect to gaussian error 'evolution'
-            error_data[ii] = signal_data[ii] * np.sqrt(1 / abs(signal_sum) + 1 / abs(reference_sum))
-
-        return signal_data, error_data
-
-    @staticmethod
-    def analyse_mean_norm(
-            laser_data: np.ndarray,
-            signal_start: float = 100e-9,
-            signal_end: float = 300e-9,
-            norm_start: float = 1000e-9,
-            norm_end=2000e-9,
-            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
-        # Get number of lasers
-        num_of_lasers = laser_data.shape[0]
-
-        if not isinstance(bin_width, float):
-            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
-
-        # Convert the times in seconds to bins (i.e. array indices)
-        signal_start_bin = round(signal_start / bin_width)
-        signal_end_bin = round(signal_end / bin_width)
-        norm_start_bin = round(norm_start / bin_width)
-        norm_end_bin = round(norm_end / bin_width)
-
-        # initialize data arrays for signal and measurement error
-        signal_data = np.empty(num_of_lasers, dtype=float)
-        error_data = np.empty(num_of_lasers, dtype=float)
-
-        # loop over all laser pulses and analyze them
-        for ii, laser_arr in enumerate(laser_data):
-            # calculate the sum and mean of the data in the normalization window
-            tmp_data = laser_arr[norm_start_bin:norm_end_bin]
-            reference_sum = np.sum(tmp_data)
-            reference_mean = (reference_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
-
-            # calculate the sum and mean of the data in the signal window
-            tmp_data = laser_arr[signal_start_bin:signal_end_bin]
-            signal_sum = np.sum(tmp_data)
-            signal_mean = (signal_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
-
-            # Calculate normalized signal while avoiding division by zero
-            if reference_mean > 0 and signal_mean >= 0:
-                signal_data[ii] = signal_mean / reference_mean
-            else:
-                signal_data[ii] = 0.0
-
-            # Calculate measurement error while avoiding division by zero
-            if reference_sum > 0 and signal_sum > 0:
-                # calculate with respect to gaussian error 'evolution'
-                error_data[ii] = signal_data[ii] * np.sqrt(1 / signal_sum + 1 / reference_sum)
-            else:
-                error_data[ii] = 0.0
-
-        return signal_data, error_data
+from __future__ import annotations
+
+import logging
+from typing import Tuple, TYPE_CHECKING
+
+import numpy as np
+import pandas as pd
+
+from qudi_hira_analysis.qudi_fit_logic import FitLogic
+
+if TYPE_CHECKING:
+    from lmfit.model import ModelResult
+
+logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
+
+
+class FitMethodsAndEstimators:
+    # Fit methods with corresponding estimators
+    antibunching: tuple = ("antibunching", "dip")
+    hyperbolicsaturation: tuple = ("hyperbolicsaturation", "generic")
+    lorentzian: tuple = ("lorentzian", "dip")
+    lorentziandouble: tuple = ("lorentziandouble", "dip")
+    sineexponentialdecay: tuple = ("sineexponentialdecay", "generic")
+    decayexponential: tuple = ("decayexponential", "generic")
+    gaussian: tuple = ("gaussian", "dip")
+    gaussiandouble: tuple = ("gaussiandouble", "dip")
+    gaussianlinearoffset: tuple = ("gaussianlinearoffset", "dip")
+    lorentziantriple: tuple = ("lorentziantriple", "dip")
+    biexponential: tuple = ("biexponential", "generic")
+    decayexponentialstretched: tuple = ("decayexponentialstretched", "generic")
+    linear: tuple = ("linear", "generic")
+    sine: tuple = ("sine", "generic")
+    sinedouble: tuple = ("sinedouble", "generic")
+    sinedoublewithexpdecay: tuple = ("sinedoublewithexpdecay", "generic")
+    sinedoublewithtwoexpdecay: tuple = ("sinedoublewithtwoexpdecay", "generic")
+    sinestretchedexponentialdecay: tuple = ("sinestretchedexponentialdecay", "generic")
+    sinetriple: tuple = ("sinetriple", "generic")
+    sinetriplewithexpdecay: tuple = ("sinetriplewithexpdecay", "generic")
+    sinetriplewiththreeexpdecay: tuple = ("sinetriplewiththreeexpdecay", "generic")
+    twoDgaussian: tuple = ("twoDgaussian", "generic")
+
+
+class AnalysisLogic(FitLogic):
+    fit_function = FitMethodsAndEstimators
+
+    def __init__(self):
+        super().__init__()
+        self.log = logging.getLogger(__name__)
+
+    def _perform_fit(
+            self,
+            x: np.ndarray,
+            y: np.ndarray,
+            fit_function: str,
+            estimator: str,
+            dims: str = "1d") -> Tuple[np.ndarray, np.ndarray, ModelResult]:
+        """
+        Fits available:
+            | Dimension | Fit                           |
+            |-----------|-------------------------------|
+            | 1d        | decayexponential              |
+            |           | biexponential                 |
+            |           | decayexponentialstretched     |
+            |           | gaussian                      |
+            |           | gaussiandouble                |
+            |           | gaussianlinearoffset          |
+            |           | hyperbolicsaturation          |
+            |           | linear                        |
+            |           | lorentzian                    |
+            |           | lorentziandouble              |
+            |           | lorentziantriple              |
+            |           | sine                          |
+            |           | sinedouble                    |
+            |           | sinedoublewithexpdecay        |
+            |           | sinedoublewithtwoexpdecay     |
+            |           | sineexponentialdecay          |
+            |           | sinestretchedexponentialdecay |
+            |           | sinetriple                    |
+            |           | sinetriplewithexpdecay        |
+            |           | sinetriplewiththreeexpdecay   |
+            | 2d        | twoDgaussian                  |
+        Estimators:
+            - generic
+            - dip
+        """
+        fit = {dims: {'default': {'fit_function': fit_function, 'estimator': estimator}}}
+        user_fit = self.validate_load_fits(fit)
+
+        use_settings = {}
+        for key in user_fit[dims]["default"]["parameters"].keys():
+            use_settings[key] = False
+        user_fit[dims]["default"]["use_settings"] = use_settings
+
+        fc = self.make_fit_container("test", dims)
+        fc.set_fit_functions(user_fit[dims])
+        fc.set_current_fit("default")
+        fc.use_settings = None
+        fit_x, fit_y, result = fc.do_fit(x, y)
+        return fit_x, fit_y, result
+
+    def fit(
+            self,
+            x: str | np.ndarray | pd.Series,
+            y: str | np.ndarray | pd.Series,
+            fit_function: FitMethodsAndEstimators,
+            data: pd.DataFrame = None,
+    ) -> Tuple[np.ndarray, np.ndarray, ModelResult]:
+        if "twoD" in fit_function[0]:
+            dims = "2d"
+        else:
+            dims = "1d"
+
+        if data is None:
+            if isinstance(x, pd.Series) or isinstance(x, pd.Index):
+                x = x.to_numpy()
+            if isinstance(y, pd.Series):
+                y = y.to_numpy()
+        elif isinstance(data, pd.DataFrame):
+            x = data[x].to_numpy()
+            y = data[y].to_numpy()
+        else:
+            raise TypeError("Data must be a pandas DataFrame or None")
+
+        return self._perform_fit(
+            x=x,
+            y=y,
+            fit_function=fit_function[0],
+            estimator=fit_function[1],
+            dims=dims
+        )
+
+    def get_all_fits(self) -> Tuple[list, list]:
+        one_d_fits = list(self.fit_list['1d'].keys())
+        two_d_fits = list(self.fit_list['2d'].keys())
+        self.log.info(f"1d fits: {one_d_fits}\n2d fits: {two_d_fits}")
+        return one_d_fits, two_d_fits
+
+    @staticmethod
+    def analyse_mean(
+            laser_data: np.ndarray,
+            signal_start: float = 100e-9,
+            signal_end: float = 300e-9,
+            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
+        # Get number of lasers
+        num_of_lasers = laser_data.shape[0]
+
+        if not isinstance(bin_width, float):
+            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
+
+        # Convert the times in seconds to bins (i.e. array indices)
+        signal_start_bin = round(signal_start / bin_width)
+        signal_end_bin = round(signal_end / bin_width)
+
+        # initialize data arrays for signal and measurement error
+        signal_data = np.empty(num_of_lasers, dtype=float)
+        error_data = np.empty(num_of_lasers, dtype=float)
+
+        # loop over all laser pulses and analyze them
+        for ii, laser_arr in enumerate(laser_data):
+            # calculate the mean of the data in the signal window
+            signal = laser_arr[signal_start_bin:signal_end_bin].mean()
+            signal_sum = laser_arr[signal_start_bin:signal_end_bin].sum()
+            signal_error = np.sqrt(signal_sum) / (signal_end_bin - signal_start_bin)
+
+            # Avoid numpy C type variables overflow and NaN values
+            if signal < 0 or signal != signal:
+                signal_data[ii] = 0.0
+                error_data[ii] = 0.0
+            else:
+                signal_data[ii] = signal
+                error_data[ii] = signal_error
+
+        return signal_data, error_data
+
+    @staticmethod
+    def analyse_mean_reference(
+            laser_data: np.ndarray,
+            signal_start: float = 100e-9,
+            signal_end: float = 300e-9,
+            norm_start: float = 1000e-9,
+            norm_end: float = 2000e-9,
+            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
+        """
+        This method takes the mean of the signal window.
+        It then does not divide by the background window to normalize
+        but rather substracts the background window to generate the output.
+        """
+        # Get number of lasers
+        num_of_lasers = laser_data.shape[0]
+
+        if not isinstance(bin_width, float):
+            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
+
+        # Convert the times in seconds to bins (i.e. array indices)
+        signal_start_bin = round(signal_start / bin_width)
+        signal_end_bin = round(signal_end / bin_width)
+        norm_start_bin = round(norm_start / bin_width)
+        norm_end_bin = round(norm_end / bin_width)
+
+        # initialize data arrays for signal and measurement error
+        signal_data = np.empty(num_of_lasers, dtype=float)
+        error_data = np.empty(num_of_lasers, dtype=float)
+
+        # loop over all laser pulses and analyze them
+        for ii, laser_arr in enumerate(laser_data):
+            # calculate the sum and mean of the data in the normalization window
+            tmp_data = laser_arr[norm_start_bin:norm_end_bin]
+            reference_sum = np.sum(tmp_data)
+            reference_mean = (reference_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
+
+            # calculate the sum and mean of the data in the signal window
+            tmp_data = laser_arr[signal_start_bin:signal_end_bin]
+            signal_sum = np.sum(tmp_data)
+            signal_mean = (signal_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
+
+            signal_data[ii] = signal_mean - reference_mean
+
+            # calculate with respect to gaussian error 'evolution'
+            error_data[ii] = signal_data[ii] * np.sqrt(1 / abs(signal_sum) + 1 / abs(reference_sum))
+
+        return signal_data, error_data
+
+    @staticmethod
+    def analyse_mean_norm(
+            laser_data: np.ndarray,
+            signal_start: float = 100e-9,
+            signal_end: float = 300e-9,
+            norm_start: float = 1000e-9,
+            norm_end=2000e-9,
+            bin_width: float = 1e-9) -> Tuple[np.ndarray, np.ndarray]:
+        # Get number of lasers
+        num_of_lasers = laser_data.shape[0]
+
+        if not isinstance(bin_width, float):
+            return np.zeros(num_of_lasers), np.zeros(num_of_lasers)
+
+        # Convert the times in seconds to bins (i.e. array indices)
+        signal_start_bin = round(signal_start / bin_width)
+        signal_end_bin = round(signal_end / bin_width)
+        norm_start_bin = round(norm_start / bin_width)
+        norm_end_bin = round(norm_end / bin_width)
+
+        # initialize data arrays for signal and measurement error
+        signal_data = np.empty(num_of_lasers, dtype=float)
+        error_data = np.empty(num_of_lasers, dtype=float)
+
+        # loop over all laser pulses and analyze them
+        for ii, laser_arr in enumerate(laser_data):
+            # calculate the sum and mean of the data in the normalization window
+            tmp_data = laser_arr[norm_start_bin:norm_end_bin]
+            reference_sum = np.sum(tmp_data)
+            reference_mean = (reference_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
+
+            # calculate the sum and mean of the data in the signal window
+            tmp_data = laser_arr[signal_start_bin:signal_end_bin]
+            signal_sum = np.sum(tmp_data)
+            signal_mean = (signal_sum / len(tmp_data)) if len(tmp_data) != 0 else 0.0
+
+            # Calculate normalized signal while avoiding division by zero
+            if reference_mean > 0 and signal_mean >= 0:
+                signal_data[ii] = signal_mean / reference_mean
+            else:
+                signal_data[ii] = 0.0
+
+            # Calculate measurement error while avoiding division by zero
+            if reference_sum > 0 and signal_sum > 0:
+                # calculate with respect to gaussian error 'evolution'
+                error_data[ii] = signal_data[ii] * np.sqrt(1 / signal_sum + 1 / reference_sum)
+            else:
+                error_data[ii] = 0.0
+
+        return signal_data, error_data
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/antibunchingmethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/antibunchingmethods.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,56 @@
-from collections import OrderedDict
-
-import numpy as np
-from lmfit.models import Model
-
-
-def make_antibunching_model(self, prefix=None):
-    def antibunching(x: np.ndarray, n: float, a: float, b: float, tau0: float, tau1: float, tau2: float) \
-            -> np.ndarray:
-        """
-        Fit to function
-            f(x; n, a, tau0, tau1, tau2) =
-                a * ((1 - (1+b) * exp(-|x-tau0|/tau1) + a * exp(-|x-tau0|/tau2)) * 1/n + 1 - 1/n)
-        """
-        return a * ((1 - (1 + b) * np.exp(-np.abs(x - tau0) / tau1) + b *
-                     np.exp(-np.abs(x - tau0) / tau2)) * 1 / n + 1 - 1 / n)
-
-    antibunching_model = Model(antibunching, independent_vars=['x'])
-    params = antibunching_model.make_params()
-
-    return antibunching_model, params
-
-
-def estimate_antibunching_dip(self, x_axis, data, params):
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    params["n"].set(value=1)
-    params["a"].set(value=1)
-    params["b"].set(value=np.max(data) - np.min(data))
-    params["tau0"].set(value=0)
-    params["tau1"].set(value=20)
-    params["tau2"].set(value=30)
-
-    return error, params
-
-
-def make_antibunching_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    model, params = self.make_antibunching_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The 1D antibunching fit did not work. Error '
-                         'message: {0}\n'.format(result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-    result.result_str_dict = result_str_dict
-
-    return result
+from collections import OrderedDict
+
+import numpy as np
+from lmfit.models import Model
+
+
+def make_antibunching_model(self, prefix=None):
+    def antibunching(x: np.ndarray, n: float, a: float, b: float, tau0: float, tau1: float, tau2: float) \
+            -> np.ndarray:
+        """
+        Fit to function
+            f(x; n, a, tau0, tau1, tau2) =
+                a * ((1 - (1+b) * exp(-|x-tau0|/tau1) + a * exp(-|x-tau0|/tau2)) * 1/n + 1 - 1/n)
+        """
+        return a * ((1 - (1 + b) * np.exp(-np.abs(x - tau0) / tau1) + b *
+                     np.exp(-np.abs(x - tau0) / tau2)) * 1 / n + 1 - 1 / n)
+
+    antibunching_model = Model(antibunching, independent_vars=['x'])
+    params = antibunching_model.make_params()
+
+    return antibunching_model, params
+
+
+def estimate_antibunching_dip(self, x_axis, data, params):
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    params["n"].set(value=1)
+    params["a"].set(value=1)
+    params["b"].set(value=np.max(data) - np.min(data))
+    params["tau0"].set(value=0)
+    params["tau1"].set(value=20)
+    params["tau2"].set(value=30)
+
+    return error, params
+
+
+def make_antibunching_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    model, params = self.make_antibunching_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The 1D antibunching fit did not work. Error '
+                         'message: {0}\n'.format(result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+    result.result_str_dict = result_str_dict
+
+    return result
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/decaylikemethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/decaylikemethods.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,584 +1,584 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains methods for decay-like fitting, these methods
-are imported by class FitLogic.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-import numpy as np
-from lmfit.models import Model
-from scipy.ndimage import filters
-
-
-############################################################################
-#                                                                          #
-#               Defining Exponential Models                                #
-#                                                                          #
-############################################################################
-
-####################################################
-#  General case: bare stretched exponential decay  #
-####################################################
-
-def make_barestretchedexponentialdecay_model(self, prefix=None):
-    """ Create a general bare exponential decay model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-
-    """
-
-    def barestretchedexponentialdecay_function(x, beta, lifetime):
-        """ Function of a bare exponential decay.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. time
-        @param float lifetime: constant lifetime
-
-        @return: bare exponential decay function: in order to use it as a model
-        """
-        return np.exp(-np.power(x / lifetime, beta))
-
-    if not isinstance(prefix, str) and prefix is not None:
-
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                       'cannot be used as a prefix and will be ignored for now.'
-                       'Correct that!'.format(prefix, type(prefix)))
-        model = Model(barestretchedexponentialdecay_function,
-                      independent_vars=['x'])
-    else:
-        model = Model(barestretchedexponentialdecay_function,
-                      independent_vars=['x'], prefix=prefix)
-
-    params = model.make_params()
-
-    return model, params
-
-
-##############################
-#  Single exponential decay  #
-##############################
-
-def make_bareexponentialdecay_model(self, prefix=None):
-    """ Create a bare single exponential decay model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_barestretchedexponentialdecay_model.
-    """
-
-    bare_exp_decay, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
-
-    bare_exp_decay.set_param_hint(name='beta', value=1, vary=False)
-    params = bare_exp_decay.make_params()
-
-    return bare_exp_decay, params
-
-
-def make_decayexponential_model(self, prefix=None):
-    """ Create a exponential decay model with an amplitude and offset.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_barestretchedexponentialdecay_model.
-    """
-
-    bare_exp_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
-
-    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    exponentialdecay_model = amplitude_model * bare_exp_model + constant_model
-    params = exponentialdecay_model.make_params()
-
-    return exponentialdecay_model, params
-
-
-#################################
-#  Stretched exponential decay  #
-#################################
-
-def make_decayexponentialstretched_model(self, prefix=None):
-    """ Create a stretched exponential decay model with offset.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_barestretchedexponentialdecay_model.
-    """
-
-    bare_stre_exp_decay, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
-    amplitude_model, params = self.make_amplitude_model()
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    stre_exp_decay_offset = amplitude_model * bare_stre_exp_decay + constant_model
-    params = stre_exp_decay_offset.make_params()
-
-    return stre_exp_decay_offset, params
-
-
-#################################
-#      Biexponential decay      #
-#################################
-
-def make_biexponential_model(self, prefix=None):
-    """ Create a exponential model with an amplitude and offset.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_barestretchedexponential_model.
-    """
-
-    exp0_model, params = self.make_bareexponentialdecay_model(prefix='e0_')
-    amp0_model, params = self.make_amplitude_model(prefix='e0_')
-
-    exp1_model, params = self.make_bareexponentialdecay_model(prefix='e1_')
-    amp1_model, params = self.make_amplitude_model(prefix='e1_')
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    exponential_model = amp0_model * exp0_model + amp1_model * exp1_model + constant_model
-    params = exponential_model.make_params()
-
-    return exponential_model, params
-
-
-############################################################################
-#                                                                          #
-#                Fit methods and their estimators                          #
-#                                                                          #
-############################################################################
-
-##########################################
-#  single exponential decay with offset  #
-##########################################
-
-def make_decayexponential_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Performes a exponential decay with offset fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    exponentialdecay, params = self.make_decayexponential_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = exponentialdecay.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = exponentialdecay.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The exponentialdecay with offset fit did not work. '
-                         'Message: {}'.format(str(result.message)))
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error': result.params['amplitude'].stderr,
-                                    'unit': units[1]}  # amplitude
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}  # lifetime
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}  # offset
-
-    result.result_str_dict = result_str_dict
-
-    return result
-
-
-def estimate_decayexponential(self, x_axis, data, params):
-    """ Estimation of the initial values for an exponential decay function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # calculation of offset, take the last 10% from the end of the data
-    # and perform the mean from those.
-    offset = data[-max(1, int(len(x_axis) / 10)):].mean()
-
-    # substraction of offset, check whether
-    if data[0] < data[-1]:
-        data_level = offset - data
-    else:
-        data_level = data - offset
-
-    # check if the data level contain still negative values and correct
-    # the data level therefore. Otherwise problems in the logarithm appear.
-    if data_level.min() <= 0:
-        data_level = data_level - data_level.min()
-
-    # remove all the data that can be smaller than or equals to std.
-    # when the data is smaller than std, it is beyond resolution
-    # which is not helpful to our fitting.
-    for i in range(0, len(x_axis)):
-        if data_level[i] <= data_level.std():
-            break
-
-    # values and bound of parameter.
-    ampl = data[-max(1, int(len(x_axis) / 10)):].std()
-    min_lifetime = 2 * (x_axis[1] - x_axis[0])
-
-    try:
-        data_level_log = np.log(data_level[0:i])
-
-        # linear fit, see linearmethods.py
-        linear_result = self.make_linear_fit(x_axis=x_axis[0:i], data=data_level_log, estimator=self.estimate_linear)
-        params['lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
-
-        # amplitude can be positive of negative
-        if data[0] < data[-1]:
-            params['amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
-        else:
-            params['amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
-    except:
-        self.log.warning('Lifetime too small in estimate_exponentialdecay, beyond resolution!')
-
-        params['lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
-        params['amplitude'].set(value=data_level[0])
-
-    params['offset'].set(value=offset)
-
-    return error, params
-
-
-#############################################
-#  stretched exponential decay with offset  #
-#############################################
-
-def make_decayexponentialstretched_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Performes a stretched exponential decay with offset fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param object estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    stret_exp_decay_offset, params = self.make_decayexponentialstretched_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = stret_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = stret_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The double exponentialdecay with offset fit did not work. '
-                         'Message: {}'.format(str(result.message)))
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error': result.params['amplitude'].stderr,
-                                    'unit': units[1]}  # amplitude
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}  # lifetime
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}  # offset
-
-    result_str_dict['Beta'] = {'value': result.params['beta'].value,
-                               'error': result.params['beta'].stderr,
-                               'unit': ''}  # Beta (exponent of exponential exponent)
-
-    result.result_str_dict = result_str_dict
-
-    return result
-
-
-def estimate_decayexponentialstretched(self, x_axis, data, params):
-    """ Provide an estimation for initial values for a stretched exponential decay with offset.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # Smooth very radically the provided data, so that noise fluctuations will
-    # not disturb the parameter estimation.
-    std_dev = 10
-    data_smoothed = filters.gaussian_filter1d(data, std_dev)
-
-    # calculation of offset, take the last 10% from the end of the data
-    # and perform the mean from those.
-    offset = data_smoothed[-max(1, int(len(x_axis) / 10)):].mean()
-
-    # substraction of the offset and correction of the decay behaviour
-    # (decay to a bigger value or decay to a smaller value)
-    if data_smoothed[0] < data_smoothed[-1]:
-        data_smoothed = offset - data_smoothed
-        ampl_sign = -1
-    else:
-        data_smoothed = data_smoothed - offset
-        ampl_sign = 1
-
-    if data_smoothed.min() <= 0:
-        data_smoothed = data_smoothed - data_smoothed.min()
-
-    # Take all values up to the standard deviation, the remaining values are
-    # more disturbing the estimation then helping:
-    for stop_index in range(0, len(x_axis)):
-        if data_smoothed[stop_index] <= data_smoothed.std():
-            break
-
-    data_level_log = np.log(data_smoothed[0:stop_index])
-
-    # make a polynomial fit with a second order polynom on the remaining data:
-    poly_coef = np.polyfit(x_axis[0:stop_index], data_level_log, deg=2)
-
-    # obtain the values from the polynomical fit
-    lifetime = 1 / np.sqrt(abs(poly_coef[0]))
-    amplitude = np.exp(poly_coef[2])
-
-    # Include all the estimated fit parameter:
-    params['amplitude'].set(value=amplitude * ampl_sign)
-    params['offset'].set(value=offset)
-
-    min_lifetime = 2 * (x_axis[1] - x_axis[0])
-    params['lifetime'].set(value=lifetime, min=min_lifetime)
-
-    # as an arbitrary starting point:
-    params['beta'].set(value=2, min=0)
-
-    return error, params
-
-
-#############################################
-#  biexponential function with offset       #
-#############################################
-
-
-def make_biexponential_fit(self, x_axis, data, estimator,
-                           units=None,
-                           add_params=None, **kwargs):
-    """ Perform a biexponential fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    model, params = self.make_biexponential_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The double gaussian dip fit did not work: {0}'.format(
-            result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = dict()
-
-    result_str_dict['1st amplitude'] = {'value': result.params['e0_amplitude'].value,
-                                        'error': result.params['e0_amplitude'].stderr,
-                                        'unit': units[1]}  # amplitude
-
-    result_str_dict['1st lifetime'] = {'value': result.params['e0_lifetime'].value,
-                                       'error': result.params['e0_lifetime'].stderr,
-                                       'unit': units[0]}  # lifetime
-
-    result_str_dict['1st beta'] = {'value': result.params['e0_beta'].value,
-                                   'error': result.params['e0_beta'].stderr,
-                                   'unit': ''}  # Beta (exponent of exponential exponent)
-
-    result_str_dict['2nd amplitude'] = {'value': result.params['e1_amplitude'].value,
-                                        'error': result.params['e1_amplitude'].stderr,
-                                        'unit': units[1]}  # amplitude
-
-    result_str_dict['2nd lifetime'] = {'value': result.params['e1_lifetime'].value,
-                                       'error': result.params['e1_lifetime'].stderr,
-                                       'unit': units[0]}  # lifetime
-
-    result_str_dict['2nd beta'] = {'value': result.params['e1_beta'].value,
-                                   'error': result.params['e1_beta'].stderr,
-                                   'unit': ''}  # Beta (exponent of exponential exponent)
-
-    result_str_dict['offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}  # offset
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_biexponential(self, x_axis, data, params):
-    """ Estimation of the initial values for an biexponential function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # calculation of offset, take the last 10% from the end of the data
-    # and perform the mean from those.
-    offset = data[-max(1, int(len(x_axis) / 10)):].mean()
-
-    # substraction of offset, check whether
-    if data[0] < data[-1]:
-        data_level = offset - data
-    else:
-        data_level = data - offset
-
-    # check if the data level contain still negative values and correct
-    # the data level therefore. Otherwise problems in the logarithm appear.
-    if data_level.min() <= 0:
-        data_level = data_level - data_level.min()
-
-    # remove all the data that can be smaller than or equals to std.
-    # when the data is smaller than std, it is beyond resolution
-    # which is not helpful to our fitting.
-    for i in range(0, len(x_axis)):
-        if data_level[i] <= data_level.std():
-            break
-
-    # values and bound of parameter.
-    ampl = data[-max(1, int(len(x_axis) / 10)):].std()
-    min_lifetime = 1e-16
-
-    try:
-        data_level_log = np.log(data_level[0:i])
-
-        # linear fit, see linearmethods.py
-        linear_result = self.make_linear_fit(x_axis=x_axis[0:i], data=data_level_log, estimator=self.estimate_linear)
-        params['e0_lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
-        params['e1_lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
-
-        # amplitude can be positive of negative
-        if data[0] < data[-1]:
-            params['e0_amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
-            params['e1_amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
-        else:
-            params['e0_amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
-            params['e1_amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
-    except:
-        self.log.warning('Lifetime too small in estimate_exponential, beyond resolution!')
-
-        params['e0_lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
-        params['e1_lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
-        params['e0_amplitude'].set(value=data_level[0])
-        params['e1_amplitude'].set(value=data_level[0])
-
-    params['offset'].set(value=offset)
-
-    return error, params
+# -*- coding: utf-8 -*-
+"""
+This file contains methods for decay-like fitting, these methods
+are imported by class FitLogic.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+import numpy as np
+from lmfit.models import Model
+from scipy.ndimage import filters
+
+
+############################################################################
+#                                                                          #
+#               Defining Exponential Models                                #
+#                                                                          #
+############################################################################
+
+####################################################
+#  General case: bare stretched exponential decay  #
+####################################################
+
+def make_barestretchedexponentialdecay_model(self, prefix=None):
+    """ Create a general bare exponential decay model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+
+    """
+
+    def barestretchedexponentialdecay_function(x, beta, lifetime):
+        """ Function of a bare exponential decay.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. time
+        @param float lifetime: constant lifetime
+
+        @return: bare exponential decay function: in order to use it as a model
+        """
+        return np.exp(-np.power(x / lifetime, beta))
+
+    if not isinstance(prefix, str) and prefix is not None:
+
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                       'cannot be used as a prefix and will be ignored for now.'
+                       'Correct that!'.format(prefix, type(prefix)))
+        model = Model(barestretchedexponentialdecay_function,
+                      independent_vars=['x'])
+    else:
+        model = Model(barestretchedexponentialdecay_function,
+                      independent_vars=['x'], prefix=prefix)
+
+    params = model.make_params()
+
+    return model, params
+
+
+##############################
+#  Single exponential decay  #
+##############################
+
+def make_bareexponentialdecay_model(self, prefix=None):
+    """ Create a bare single exponential decay model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_barestretchedexponentialdecay_model.
+    """
+
+    bare_exp_decay, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
+
+    bare_exp_decay.set_param_hint(name='beta', value=1, vary=False)
+    params = bare_exp_decay.make_params()
+
+    return bare_exp_decay, params
+
+
+def make_decayexponential_model(self, prefix=None):
+    """ Create a exponential decay model with an amplitude and offset.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_barestretchedexponentialdecay_model.
+    """
+
+    bare_exp_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
+
+    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    exponentialdecay_model = amplitude_model * bare_exp_model + constant_model
+    params = exponentialdecay_model.make_params()
+
+    return exponentialdecay_model, params
+
+
+#################################
+#  Stretched exponential decay  #
+#################################
+
+def make_decayexponentialstretched_model(self, prefix=None):
+    """ Create a stretched exponential decay model with offset.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_barestretchedexponentialdecay_model.
+    """
+
+    bare_stre_exp_decay, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
+    amplitude_model, params = self.make_amplitude_model()
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    stre_exp_decay_offset = amplitude_model * bare_stre_exp_decay + constant_model
+    params = stre_exp_decay_offset.make_params()
+
+    return stre_exp_decay_offset, params
+
+
+#################################
+#      Biexponential decay      #
+#################################
+
+def make_biexponential_model(self, prefix=None):
+    """ Create a exponential model with an amplitude and offset.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_barestretchedexponential_model.
+    """
+
+    exp0_model, params = self.make_bareexponentialdecay_model(prefix='e0_')
+    amp0_model, params = self.make_amplitude_model(prefix='e0_')
+
+    exp1_model, params = self.make_bareexponentialdecay_model(prefix='e1_')
+    amp1_model, params = self.make_amplitude_model(prefix='e1_')
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    exponential_model = amp0_model * exp0_model + amp1_model * exp1_model + constant_model
+    params = exponential_model.make_params()
+
+    return exponential_model, params
+
+
+############################################################################
+#                                                                          #
+#                Fit methods and their estimators                          #
+#                                                                          #
+############################################################################
+
+##########################################
+#  single exponential decay with offset  #
+##########################################
+
+def make_decayexponential_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Performes a exponential decay with offset fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    exponentialdecay, params = self.make_decayexponential_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = exponentialdecay.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = exponentialdecay.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The exponentialdecay with offset fit did not work. '
+                         'Message: {}'.format(str(result.message)))
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error': result.params['amplitude'].stderr,
+                                    'unit': units[1]}  # amplitude
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}  # lifetime
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}  # offset
+
+    result.result_str_dict = result_str_dict
+
+    return result
+
+
+def estimate_decayexponential(self, x_axis, data, params):
+    """ Estimation of the initial values for an exponential decay function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # calculation of offset, take the last 10% from the end of the data
+    # and perform the mean from those.
+    offset = data[-max(1, int(len(x_axis) / 10)):].mean()
+
+    # substraction of offset, check whether
+    if data[0] < data[-1]:
+        data_level = offset - data
+    else:
+        data_level = data - offset
+
+    # check if the data level contain still negative values and correct
+    # the data level therefore. Otherwise problems in the logarithm appear.
+    if data_level.min() <= 0:
+        data_level = data_level - data_level.min()
+
+    # remove all the data that can be smaller than or equals to std.
+    # when the data is smaller than std, it is beyond resolution
+    # which is not helpful to our fitting.
+    for i in range(0, len(x_axis)):
+        if data_level[i] <= data_level.std():
+            break
+
+    # values and bound of parameter.
+    ampl = data[-max(1, int(len(x_axis) / 10)):].std()
+    min_lifetime = 2 * (x_axis[1] - x_axis[0])
+
+    try:
+        data_level_log = np.log(data_level[0:i])
+
+        # linear fit, see linearmethods.py
+        linear_result = self.make_linear_fit(x_axis=x_axis[0:i], data=data_level_log, estimator=self.estimate_linear)
+        params['lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
+
+        # amplitude can be positive of negative
+        if data[0] < data[-1]:
+            params['amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
+        else:
+            params['amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
+    except:
+        self.log.warning('Lifetime too small in estimate_exponentialdecay, beyond resolution!')
+
+        params['lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
+        params['amplitude'].set(value=data_level[0])
+
+    params['offset'].set(value=offset)
+
+    return error, params
+
+
+#############################################
+#  stretched exponential decay with offset  #
+#############################################
+
+def make_decayexponentialstretched_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Performes a stretched exponential decay with offset fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param object estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    stret_exp_decay_offset, params = self.make_decayexponentialstretched_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = stret_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = stret_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The double exponentialdecay with offset fit did not work. '
+                         'Message: {}'.format(str(result.message)))
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error': result.params['amplitude'].stderr,
+                                    'unit': units[1]}  # amplitude
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}  # lifetime
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}  # offset
+
+    result_str_dict['Beta'] = {'value': result.params['beta'].value,
+                               'error': result.params['beta'].stderr,
+                               'unit': ''}  # Beta (exponent of exponential exponent)
+
+    result.result_str_dict = result_str_dict
+
+    return result
+
+
+def estimate_decayexponentialstretched(self, x_axis, data, params):
+    """ Provide an estimation for initial values for a stretched exponential decay with offset.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # Smooth very radically the provided data, so that noise fluctuations will
+    # not disturb the parameter estimation.
+    std_dev = 10
+    data_smoothed = filters.gaussian_filter1d(data, std_dev)
+
+    # calculation of offset, take the last 10% from the end of the data
+    # and perform the mean from those.
+    offset = data_smoothed[-max(1, int(len(x_axis) / 10)):].mean()
+
+    # substraction of the offset and correction of the decay behaviour
+    # (decay to a bigger value or decay to a smaller value)
+    if data_smoothed[0] < data_smoothed[-1]:
+        data_smoothed = offset - data_smoothed
+        ampl_sign = -1
+    else:
+        data_smoothed = data_smoothed - offset
+        ampl_sign = 1
+
+    if data_smoothed.min() <= 0:
+        data_smoothed = data_smoothed - data_smoothed.min()
+
+    # Take all values up to the standard deviation, the remaining values are
+    # more disturbing the estimation then helping:
+    for stop_index in range(0, len(x_axis)):
+        if data_smoothed[stop_index] <= data_smoothed.std():
+            break
+
+    data_level_log = np.log(data_smoothed[0:stop_index])
+
+    # make a polynomial fit with a second order polynom on the remaining data:
+    poly_coef = np.polyfit(x_axis[0:stop_index], data_level_log, deg=2)
+
+    # obtain the values from the polynomical fit
+    lifetime = 1 / np.sqrt(abs(poly_coef[0]))
+    amplitude = np.exp(poly_coef[2])
+
+    # Include all the estimated fit parameter:
+    params['amplitude'].set(value=amplitude * ampl_sign)
+    params['offset'].set(value=offset)
+
+    min_lifetime = 2 * (x_axis[1] - x_axis[0])
+    params['lifetime'].set(value=lifetime, min=min_lifetime)
+
+    # as an arbitrary starting point:
+    params['beta'].set(value=2, min=0)
+
+    return error, params
+
+
+#############################################
+#  biexponential function with offset       #
+#############################################
+
+
+def make_biexponential_fit(self, x_axis, data, estimator,
+                           units=None,
+                           add_params=None, **kwargs):
+    """ Perform a biexponential fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    model, params = self.make_biexponential_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The double gaussian dip fit did not work: {0}'.format(
+            result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = dict()
+
+    result_str_dict['1st amplitude'] = {'value': result.params['e0_amplitude'].value,
+                                        'error': result.params['e0_amplitude'].stderr,
+                                        'unit': units[1]}  # amplitude
+
+    result_str_dict['1st lifetime'] = {'value': result.params['e0_lifetime'].value,
+                                       'error': result.params['e0_lifetime'].stderr,
+                                       'unit': units[0]}  # lifetime
+
+    result_str_dict['1st beta'] = {'value': result.params['e0_beta'].value,
+                                   'error': result.params['e0_beta'].stderr,
+                                   'unit': ''}  # Beta (exponent of exponential exponent)
+
+    result_str_dict['2nd amplitude'] = {'value': result.params['e1_amplitude'].value,
+                                        'error': result.params['e1_amplitude'].stderr,
+                                        'unit': units[1]}  # amplitude
+
+    result_str_dict['2nd lifetime'] = {'value': result.params['e1_lifetime'].value,
+                                       'error': result.params['e1_lifetime'].stderr,
+                                       'unit': units[0]}  # lifetime
+
+    result_str_dict['2nd beta'] = {'value': result.params['e1_beta'].value,
+                                   'error': result.params['e1_beta'].stderr,
+                                   'unit': ''}  # Beta (exponent of exponential exponent)
+
+    result_str_dict['offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}  # offset
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_biexponential(self, x_axis, data, params):
+    """ Estimation of the initial values for an biexponential function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # calculation of offset, take the last 10% from the end of the data
+    # and perform the mean from those.
+    offset = data[-max(1, int(len(x_axis) / 10)):].mean()
+
+    # substraction of offset, check whether
+    if data[0] < data[-1]:
+        data_level = offset - data
+    else:
+        data_level = data - offset
+
+    # check if the data level contain still negative values and correct
+    # the data level therefore. Otherwise problems in the logarithm appear.
+    if data_level.min() <= 0:
+        data_level = data_level - data_level.min()
+
+    # remove all the data that can be smaller than or equals to std.
+    # when the data is smaller than std, it is beyond resolution
+    # which is not helpful to our fitting.
+    for i in range(0, len(x_axis)):
+        if data_level[i] <= data_level.std():
+            break
+
+    # values and bound of parameter.
+    ampl = data[-max(1, int(len(x_axis) / 10)):].std()
+    min_lifetime = 1e-16
+
+    try:
+        data_level_log = np.log(data_level[0:i])
+
+        # linear fit, see linearmethods.py
+        linear_result = self.make_linear_fit(x_axis=x_axis[0:i], data=data_level_log, estimator=self.estimate_linear)
+        params['e0_lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
+        params['e1_lifetime'].set(value=-1 / linear_result.params['slope'].value, min=min_lifetime)
+
+        # amplitude can be positive of negative
+        if data[0] < data[-1]:
+            params['e0_amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
+            params['e1_amplitude'].set(value=-np.exp(linear_result.params['offset'].value), max=-ampl)
+        else:
+            params['e0_amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
+            params['e1_amplitude'].set(value=np.exp(linear_result.params['offset'].value), min=ampl)
+    except:
+        self.log.warning('Lifetime too small in estimate_exponential, beyond resolution!')
+
+        params['e0_lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
+        params['e1_lifetime'].set(value=x_axis[i] - x_axis[0], min=min_lifetime)
+        params['e0_amplitude'].set(value=data_level[0])
+        params['e1_amplitude'].set(value=data_level[0])
+
+    params['offset'].set(value=offset)
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/gaussianlikemethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/gaussianlikemethods.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,940 +1,940 @@
-# -*- coding: utf-8 -*-
-
-"""
-This file contains methods for gaussian-like fitting, these methods
-are imported by class FitLogic.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-
-from collections import OrderedDict
-
-import numpy as np
-from lmfit import Parameters
-from lmfit.models import Model
-from scipy.ndimage import filters
-
-
-############################################################################
-#                                                                          #
-#                          Defining models                                 #
-#                                                                          #
-############################################################################
-
-####################################
-# Gaussian model                   #
-####################################
-
-
-def make_gaussianwithoutoffset_model(self, prefix=None):
-    """ Create a model of a gaussian with specified amplitude.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-
-    For further information have a look in:
-    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html
-    """
-
-    def physical_gauss(x, center, sigma):
-        """ Function of a bare Gaussian with unit height at center.
-
-        @param numpy.array x: independent variable - e.g. frequency
-        @param float center: center around which the distributions (expectation
-                             value).
-        @param float sigma: standard deviation of the gaussian
-
-        @return: numpy.array with length equals to input x and with the values
-                 of a bare Gaussian.
-        """
-        return np.exp(- np.power((center - x), 2) / (2 * np.power(sigma, 2)))
-
-    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                       'cannot be used as a prefix and will be ignored for now.'
-                       'Correct that!'.format(prefix, type(prefix)))
-        gaussian_model = Model(physical_gauss, independent_vars=['x'])
-    else:
-        gaussian_model = Model(physical_gauss, independent_vars=['x'],
-                               prefix=prefix)
-
-    full_gaussian_model = amplitude_model * gaussian_model
-
-    if prefix is None:
-        prefix = ''
-    full_gaussian_model.set_param_hint('{0!s}fwhm'.format(prefix),
-                                       expr="2.3548200450309493*{0}sigma".format(prefix))
-
-    params = full_gaussian_model.make_params()
-
-    return full_gaussian_model, params
-
-####################################
-# 1D Gaussian model with offset    #
-####################################
-
-def make_gaussian_model(self, prefix=None):
-    """ Create a gauss model with amplitude and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-    """
-
-    gaussian_model, params = self.make_gaussianwithoutoffset_model(prefix=prefix)
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    gaussian_offset_model = gaussian_model + constant_model
-
-    if prefix is None:
-        prefix = ''
-
-    gaussian_offset_model.set_param_hint('{0}contrast'.format(prefix),
-                                         expr='({0}amplitude/offset)*100'.format(prefix))
-
-    params = gaussian_offset_model.make_params()
-
-    return gaussian_offset_model, params
-
-######################################################
-# 1D Gaussian model with linear (inclined) offset    #
-######################################################
-
-def make_gaussianlinearoffset_model(self, prefix=None):
-    """ Create a gauss with a linear offset (i.e. a slope).
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-    """
-
-    # Note that the offset parameter comes here from the gauss model and not
-    # from the slope model.
-    slope_model, params = self.make_slope_model(prefix)
-    gaussian_model, params = self.make_gaussian_model(prefix)
-
-    gaussian_linear_offset = gaussian_model + slope_model
-    params = gaussian_linear_offset.make_params()
-
-    return gaussian_linear_offset, params
-
-##########################################
-# 1D Multiple Gaussian Model with offset #
-##########################################
-
-
-def make_multiplegaussianoffset_model(self, no_of_functions=1):
-    """ Create a model with multiple gaussian with offset.
-
-    @param no_of_functions: for default=1 there is one gaussian, else
-                            more functions are added
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-    """
-
-    if no_of_functions == 1:
-        multi_gaussian_model, params = self.make_gaussian_model()
-    else:
-
-        prefix = 'g0_'
-        multi_gaussian_model, params = self.make_gaussianwithoutoffset_model(prefix=prefix)
-
-        constant_model, params = self.make_constant_model()
-        multi_gaussian_model = multi_gaussian_model + constant_model
-
-        multi_gaussian_model.set_param_hint('{0}contrast'.format(prefix),
-                                            expr='({0}amplitude/offset)*100'.format(prefix))
-
-        for ii in range(1, no_of_functions):
-
-            prefix = 'g{0:d}_'.format(ii)
-            multi_gaussian_model += self.make_gaussianwithoutoffset_model(prefix=prefix)[0]
-            multi_gaussian_model.set_param_hint('{0}contrast'.format(prefix),
-                                                expr='({0}amplitude/offset)*100'.format(prefix))
-
-    params = multi_gaussian_model.make_params()
-
-    return multi_gaussian_model, params
-
-##########################################
-#   1D Double Gaussian Model with offset #
-##########################################
-
-
-def make_gaussiandouble_model(self):
-    """ Create a model with double gaussian with offset.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-    """
-
-    return self.make_multiplegaussianoffset_model(no_of_functions=2)
-
-##########################################
-#   1D Triple Gaussian Model with offset #
-##########################################
-
-
-def make_gaussiantriple_model(self):
-    """ Create a model with double gaussian with offset.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-    """
-
-    return self.make_multiplegaussianoffset_model(no_of_functions=3)
-
-#####################
-# 2D gaussian model #
-#####################
-
-def make_twoDgaussian_model(self, prefix=None):
-    """ Creates a model of the 2D gaussian function.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_gaussianwithoutoffset_model.
-
-    """
-
-    def twoDgaussian_function(x, amplitude, center_x, center_y, sigma_x, sigma_y,
-                              theta, offset):
-        """ Provide a two dimensional gaussian function.
-
-        @param float amplitude: Amplitude of gaussian
-        @param float center_x: x value of maximum
-        @param float center_y: y value of maximum
-        @param float sigma_x: standard deviation in x direction
-        @param float sigma_y: standard deviation in y direction
-        @param float theta: angle for eliptical gaussians
-        @param float offset: offset
-
-        @return callable function: returns the reference to the function
-
-        Function taken from:
-        http://stackoverflow.com/questions/21566379/fitting-a-2d-gaussian-function-using-scipy-optimize-curve-fit-valueerror-and-m/21566831
-
-        Question from: http://stackoverflow.com/users/2097737/bland
-                       http://stackoverflow.com/users/3273102/kokomoking
-                       http://stackoverflow.com/users/2767207/jojodmo
-        Answer: http://stackoverflow.com/users/1461210/ali-m
-                http://stackoverflow.com/users/5234/mrjrdnthms
-        """
-
-        # FIXME: x_data_tuple: dimension of arrays
-        # @param np.arra[k][M] x_data_tuple: array which is (k,M)-shaped,
-        #                                   x and y values
-
-        (u, v) = x
-        center_x = float(center_x)
-        center_y = float(center_y)
-
-        a = (np.cos(theta) ** 2) / (2 * sigma_x ** 2) \
-            + (np.sin(theta) ** 2) / (2 * sigma_y ** 2)
-        b = -(np.sin(2 * theta)) / (4 * sigma_x ** 2) \
-            + (np.sin(2 * theta)) / (4 * sigma_y ** 2)
-        c = (np.sin(theta) ** 2) / (2 * sigma_x ** 2) \
-            + (np.cos(theta) ** 2) / (2 * sigma_y ** 2)
-        g = offset + amplitude * np.exp(- (a * ((u - center_x) ** 2)
-                                           + 2 * b * (u - center_x) * (v - center_y)
-                                           + c * ((v - center_y) ** 2)))
-        return g.ravel()
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                     'cannot be used as a prefix and will be ignored for now.'
-                     'Correct that!'.format(prefix, type(prefix)))
-        gaussian_2d_model = Model(twoDgaussian_function, independent_vars=['x'])
-    else:
-        gaussian_2d_model = Model(twoDgaussian_function, independent_vars=['x'],
-                               prefix=prefix)
-
-    params = gaussian_2d_model.make_params()
-
-    return gaussian_2d_model, params
-
-################################################################################
-#                                                                              #
-#                    Fit functions and their estimators                        #
-#                                                                              #
-################################################################################
-
-###################################
-# 1D Gaussian with flat offset    #
-###################################
-
-def make_gaussian_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a 1D gaussian peak fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-
-    mod_final, params = self.make_gaussian_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The 1D gaussian peak fit did not work. Error '
-                       'message: {0}\n'.format(result.message))
-
-    if units is None:
-            units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = OrderedDict()  # create result string for gui
-
-    #result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-    #                                    'error': result.params['amplitude'].stderr,
-    #                                    'unit': units[1]}                               #amplitude
-
-    result_str_dict['Position'] = {'value': result.params['center'].value,
-                                        'error': result.params['center'].stderr,
-                                        'unit': units[0]}                               #position
-
-    #result_str_dict['Standard deviation'] = {'value': result.params['sigma'].value,
-    #                                'error': result.params['sigma'].stderr,
-    #                                'unit': units[0]}                               #standart deviation
-
-    result_str_dict['Linewidth'] = {'value': result.params['fwhm'].value,
-                                        'error': result.params['fwhm'].stderr,
-                                        'unit': units[0]}                               #FWHM
-
-    result_str_dict['Contrast'] = {'value': result.params['contrast'].value,
-                                        'error': result.params['contrast'].stderr,
-                                        'unit': '%'}                                    #Contrast
-    result.result_str_dict = result_str_dict
-
-    return result
-
-
-
-def estimate_gaussian_peak(self, x_axis, data, params):
-    """ Provides a gaussian offset peak estimator.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-        Explanation of the return parameter:
-            int error: error code (0:OK, -1:error)
-            Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # If the estimator is not good enough one can start improvement with
-    # a convolution
-
-    # auxiliary variables
-    stepsize = abs(x_axis[1] - x_axis[0])
-    n_steps = len(x_axis)
-
-    # Smooth the provided data, so that noise fluctuations will not disturb the
-    # parameter estimation. This value performs the best in many scenarios:
-    std_dev = 2
-    data_smoothed = filters.gaussian_filter1d(data, std_dev)
-
-    # Define constraints:
-    # maximal and minimal the length of the given array to the right and to the
-    # left:
-    center_min = (x_axis[0]) - n_steps * stepsize
-    center_max = (x_axis[-1]) + n_steps * stepsize
-    ampl_min = 0
-    sigma_min = stepsize
-    sigma_max = 3 * (x_axis[-1] - x_axis[0])
-
-    # set parameters:
-    offset = data_smoothed.min()
-    params['offset'].set(value=offset)
-
-    # it is more reliable to select the maximal value rather then
-    # calculating the first moment of the gaussian distribution (which is the
-    # mean value), since it is unreliable if the distribution begins or ends at
-    # the edges of the data (but it helps a lot for standard deviation):
-    mean_val_calc = np.sum(x_axis*data_smoothed) / np.sum(data_smoothed)
-    params['center'].set(value=x_axis[np.argmax(data_smoothed)],
-                         min=center_min, max=center_max)
-
-    # calculate the second moment of the gaussian distribution:
-    #   int (x^2 * f(x) dx) :
-    mom2 = np.sum(x_axis ** 2 * data_smoothed) / np.sum(data_smoothed)
-
-    # and use the standard formula to obtain the standard deviation:
-    #   sigma^2 = int( (x - mean)^2 f(x) dx ) = int (x^2 * f(x) dx) - mean^2
-
-    # If the mean is situated at the edges of the distribution then this
-    # procedure performs better then setting the initial value for sigma to
-    # 1/3 of the length of the distribution since the calculated value for the
-    # mean is then higher, which will decrease eventually the initial value for
-    # sigma. But if the peak values is within the distribution the standard
-    # deviation formula performs even better:
-    params['sigma'].set(value=np.sqrt(abs(mom2 - mean_val_calc**2)),
-                        min=sigma_min, max=sigma_max)
-    # params['sigma'].set(value=(x_axis.max() - x_axis.min()) / 3.)
-
-    # Do not set the maximal amplitude value based on the distribution, since
-    # the fit will fail if the peak is at the edges or beyond the range of the
-    # x values.
-    params['amplitude'].set(value=data_smoothed.max()-data_smoothed.min(),
-                            min=ampl_min)
-
-    return error, params
-
-def estimate_gaussian_dip(self, x_axis, data, params):
-    """ Provides a gaussian offset dip estimator.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-        Explanation of the return parameter:
-            int error: error code (0:OK, -1:error)
-            Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # the peak and dip gaussian have the same parameters:
-    params_peak = params
-    data_negative = data * (-1)
-
-    error, params_ret = self.estimate_gaussian_peak(x_axis,
-                                                          data_negative,
-                                                          params_peak
-                                                          )
-
-    params['sigma'] = params_ret['sigma']
-    params['offset'].set(value=-params_ret['offset'])
-    # set the maximum to infinity, since that is the default value.
-    params['amplitude'].set(value=-params_ret['amplitude'].value, min=-np.inf,
-                            max=1e-12)
-    params['center'] = params_ret['center']
-
-    return error, params
-
-##############################################
-# 1D Gaussian with linear inclined offset    #
-##############################################
-
-def make_gaussianlinearoffset_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a 1D gaussian peak fit with linear offset on the provided data.
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-
-    mod_final, params = self.make_gaussianlinearoffset_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The 1D gaussian peak fit did not work. Error '
-                       'message: {0}\n'.format(result.message))
-    if units is None:
-            units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = OrderedDict()  # create result string for gui
-
-    #result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-    #                                    'error': result.params['amplitude'].stderr,
-    #                                    'unit': units[1]}                               #amplitude
-
-    result_str_dict['Position'] = {'value': result.params['center'].value,
-                                        'error': result.params['center'].stderr,
-                                        'unit': units[0]}                               #position
-
-    #result_str_dict['Standard deviation'] = {'value': result.params['sigma'].value,
-    #                                'error': result.params['sigma'].stderr,
-    #                                'unit': units[0]}                               #standart deviation
-
-    result_str_dict['Linewidth'] = {'value': result.params['fwhm'].value,
-                                        'error': result.params['fwhm'].stderr,
-                                        'unit': units[0]}                               #FWHM
-
-    result_str_dict['Contrast'] = {'value': result.params['contrast'].value,
-                                        'error': result.params['contrast'].stderr,
-                                        'unit': '%'}                                    #Contrast
-
-    #result_str_dict['Slope'] = {'value': result.params['slope'].value,
-    #                                    'error': result.params['slope'].stderr,
-    #                                    'unit': ''}                                    #Slope
-
-    result.result_str_dict = result_str_dict
-
-    return result
-
-def estimate_gaussianlinearoffset_peak(self, x_axis, data, params):
-    """ Provides a gauss peak estimator with a linear changing offset.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-        Explanation of the return parameter:
-            int error: error code (0:OK, -1:error)
-            Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # try at first a fit with the ordinary gauss function
-    res_ordinary_gauss = self.make_gaussian_fit(
-        x_axis=x_axis,
-        data=data,
-        units=None,
-        estimator=self.estimate_gaussian_peak
-    )
-
-    # subtract the result and perform again a linear fit:
-    data_subtracted = data - res_ordinary_gauss.best_fit
-
-    res_linear = self.make_linear_fit(
-        x_axis=x_axis,
-        data=data_subtracted,
-        estimator=self.estimate_linear
-    )
-
-    # this way works much better than performing at first a linear fit,
-    # subtracting the fit and make an ordinary gaussian fit. Especially for a
-    # peak at the borders, this method is much more beneficial.
-
-    # assign the obtained values for the initial fit:
-    params['offset'] = res_ordinary_gauss.params['offset']
-    params['center'] = res_ordinary_gauss.params['center']
-    params['amplitude'] = res_ordinary_gauss.params['amplitude']
-    params['sigma'] = res_ordinary_gauss.params['sigma']
-    params['slope'] = res_linear.params['slope']
-
-    return error, params
-
-#################################
-# Two Gaussian with flat offset #
-#################################
-
-def make_gaussiandouble_fit(self, x_axis, data, estimator,
-                            units=None,
-                            add_params=None,
-                            threshold_fraction=0.4,
-                            minimal_threshold=0.2,
-                            sigma_threshold_fraction=0.3, **kwargs):
-    """ Perform a 1D two gaussian dip fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-    @param float threshold_fraction : Threshold to find second gaussian
-    @param float minimal_threshold: Threshold is lowerd to minimal this
-                                    value as a fraction
-    @param float sigma_threshold_fraction: Threshold for detecting
-                                           the end of the peak
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    model, params = self.make_multiplegaussianoffset_model(no_of_functions=2)
-
-    error, params = estimator(x_axis, data, params,
-                              threshold_fraction,
-                              minimal_threshold,
-                              sigma_threshold_fraction
-                              )
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The double gaussian dip fit did not work: {0}'.format(
-            result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-
-    result_str_dict['Position 0'] = {'value': result.params['g0_center'].value,
-                                     'error': result.params['g0_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Position 1'] = {'value': result.params['g1_center'].value,
-                                     'error': result.params['g1_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Contrast 0'] = {'value': abs(result.params['g0_contrast'].value),
-                                     'error': result.params['g0_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['Contrast 1'] = {'value': abs(result.params['g1_contrast'].value),
-                                     'error': result.params['g1_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['Linewidth 0'] = {'value': result.params['g0_sigma'].value,
-                                      'error': result.params['g0_sigma'].stderr,
-                                      'unit': units[0]}
-
-    result_str_dict['Linewidth 1'] = {'value': result.params['g1_sigma'].value,
-                                      'error': result.params['g1_sigma'].stderr,
-                                      'unit': units[0]}
-
-    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-def estimate_gaussiandouble_peak(self, x_axis, data, params,
-                                threshold_fraction=0.4, minimal_threshold=0.1,
-                                sigma_threshold_fraction=0.2):
-    """ Provide an estimator for a double gaussian peak fit with the parameters
-    coming from the physical properties of an experiment done in gated counter:
-                    - positive peak
-                    - no values below 0
-                    - rather broad overlapping functions
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-    @param float threshold_fraction : Threshold to find second gaussian
-    @param float minimal_threshold: Threshold is lowerd to minimal this
-                                    value as a fraction
-    @param float sigma_threshold_fraction: Threshold for detecting
-                                           the end of the peak
-
-    @return int error: error code (0:OK, -1:error)
-    @return Parameters object params: estimated values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-
-    mod_lor, params_lor = self.make_multiplelorentzian_model(no_of_functions=2)
-
-    error, params_lor = self.estimate_lorentziandouble_dip(x_axis=x_axis,
-                                                     data=-data,
-                                                     params=params_lor,
-                                                     threshold_fraction=threshold_fraction,
-                                                     minimal_threshold=minimal_threshold,
-                                                     sigma_threshold_fraction=sigma_threshold_fraction)
-
-    params['g0_amplitude'].value = -params_lor['l0_amplitude'].value
-    params['g0_center'].value = params_lor['l0_center'].value
-    params['g0_sigma'].value = params_lor['l0_sigma'].value/(np.sqrt(2*np.log(2)))
-    params['g1_amplitude'].value = -params_lor['l1_amplitude'].value
-    params['g1_center'].value = params_lor['l1_center'].value
-    params['g1_sigma'].value = params_lor['l1_sigma'].value/(np.sqrt(2*np.log(2)))
-    params['offset'].value = -params_lor['offset'].value
-
-    return error, params
-
-def estimate_gaussiandouble_dip(self, x_axis, data, params,
-                               threshold_fraction=0.4, minimal_threshold=0.1,
-                               sigma_threshold_fraction=0.2):
-    """ Provide an estimator for a double gaussian dip fit with the parameters
-    coming from the physical properties of an experiment done in gated counter:
-                    - positive peak
-                    - no values below 0
-                    - rather broad overlapping functions
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-    @param float threshold_fraction : Threshold to find second gaussian
-    @param float minimal_threshold: Threshold is lowerd to minimal this
-                                    value as a fraction
-    @param float sigma_threshold_fraction: Threshold for detecting
-                                           the end of the peak
-
-    @return int error: error code (0:OK, -1:error)
-    @return Parameters object params: estimated values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    mod_lor, params_lor = self.make_multiplelorentzian_model(no_of_functions=2)
-
-    error, params_lor = self.estimate_lorentziandouble_dip(x_axis=x_axis,
-                                                     data=data,
-                                                     params=params_lor,
-                                                     threshold_fraction=threshold_fraction,
-                                                     minimal_threshold=minimal_threshold,
-                                                     sigma_threshold_fraction=sigma_threshold_fraction)
-
-    params['g0_amplitude'].value = params_lor['l0_amplitude'].value
-    params['g0_center'].value = params_lor['l0_center'].value
-    params['g0_sigma'].value = params_lor['l0_sigma'].value/(np.sqrt(2*np.log(2)))
-    params['g1_amplitude'].value = params_lor['l1_amplitude'].value
-    params['g1_center'].value = params_lor['l1_center'].value
-    params['g1_sigma'].value = params_lor['l1_sigma'].value/(np.sqrt(2*np.log(2)))
-    params['offset'].value = params_lor['offset'].value
-
-    return error, params
-
-###################################
-# 2D Gaussian with flat offset    #
-###################################
-
-# TODO: I think this has an offset, and it should be named so to be consistent with
-#       the 1D functions.
-
-def make_twoDgaussian_fit(self, xy_axes, data, estimator, units=None, add_params=None, **kwargs):
-    """ This method performes a 2D gaussian fit on the provided data.
-
-    @param numpy.array xy_axes: 2D axes values. xy_axes[0] contains x_axis and
-                                xy_axes[1] contains y_axis
-    @param numpy.array data: 2D matrix data, should have the dimension as
-                             len(xy_axes[0]) x len(xy_axes[1]).
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-
-    x_axis, y_axis = xy_axes
-
-    gaussian_2d_model, params = self.make_twoDgaussian_model()
-
-    error, params = estimator(x_axis=x_axis, y_axis=y_axis,
-                              data=data, params=params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = gaussian_2d_model.fit(data, x=xy_axes, params=params, **kwargs)
-    except:
-        result = gaussian_2d_model.fit(data, x=xy_axes, params=params, **kwargs)
-        self.log.warning('The 2D gaussian fit did not work: {0}'.format(
-                       result.message))
-
-    return result
-
-def estimate_twoDgaussian(self, x_axis, y_axis, data, params):
-    """ Provide a simple two dimensional gaussian function.
-
-    @param numpy.array x_axis: 1D x axis values
-    @param numpy.array y_axis: 1D y axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-        Explanation of the return parameter:
-            int error: error code (0:OK, -1:error)
-            Parameters object params: set parameters of initial values
-    """
-
-    # TODO:Make clever estimator
-    # FIXME: 1D array x_axis, y_axis, 2D data???
-
-    #            #needed me 1 hour to think about, but not needed in the end...maybe needed at a later point
-    #            len_x=np.where(x_axis[0]==x_axis)[0][1]
-    #            len_y=len(data)/len_x
-
-    amplitude = float(data.max() - data.min())
-
-    center_x = x_axis[data.argmax()]
-    center_y = y_axis[data.argmax()]
-
-    sigma_x = (x_axis.max() - x_axis.min()) / 3.
-    sigma_y = (y_axis.max() - y_axis.min()) / 3.
-    theta = 0.0
-    offset = float(data.min())
-
-    # check for sensible values
-    parameters = [x_axis, y_axis, data]
-
-    error = 0
-    for var in parameters:
-        # FIXME: Why don't you check earlier?
-        # FIXME: Check for 1D array, 2D
-        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
-            self.log.error('Given parameter is not an array.')
-            amplitude = 0.
-            center_x = 0.
-            center_y = 0.
-            sigma_x = 0.
-            sigma_y = 0.
-            theta = 0.0
-            offset = 0.
-            error = -1
-
-    # auxiliary variables:
-    stepsize_x = x_axis[1]-x_axis[0]
-    stepsize_y = y_axis[1]-y_axis[0]
-    n_steps_x = len(x_axis)
-    n_steps_y = len(y_axis)
-
-    # populate the parameter container:
-    params['amplitude'].set(value=amplitude, min=100, max=1e7)
-    params['sigma_x'].set(value=sigma_x, min=1*stepsize_x,
-                          max=3*(x_axis[-1]-x_axis[0]))
-    params['sigma_y'].set(value=sigma_y, min=1*stepsize_y,
-                          max=3*(y_axis[-1]-y_axis[0]))
-    params['center_x'].set(value=center_x, min=(x_axis[0])-n_steps_x*stepsize_x,
-                           max=x_axis[-1]+n_steps_x*stepsize_x)
-    params['center_y'].set(value=center_y, min=(y_axis[0])-n_steps_y*stepsize_y,
-                           max=y_axis[-1]+n_steps_y*stepsize_y)
-    params['theta'].set(value=theta, min=0, max=np.pi)
-    params['offset'].set(value=offset, min=0, max=1e7)
-
-    return error, params
-
-def estimate_twoDgaussian_MLE(self, x_axis, y_axis, data, params):
-    """ Provide an estimator for 2D gaussian based on maximum likelihood estimation.
-
-    @param numpy.array x_axis: 1D x axis values
-    @param numpy.array y_axis: 1D y axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-        Explanation of the return parameter:
-            int error: error code (0:OK, -1:error)
-            Parameters object params: set parameters of initial values
-
-    For the parameters characterizing of the two dimensional gaussian a maximum
-    likelihood estimation is used (at the moment only for the center_x and
-    center_y values).
-    """
-
-    # TODO: Make good estimates for sigma_x, sigma_y and theta
-
-    amplitude = float(data.max() - data.min())
-
-    # By calculating the log likelihood of the 2D gaussian pdf, one obtain for
-    # the minimization of the center_x or center_y values the following formula
-    # (which are in fact just the expectation/mean value formula):
-    center_x = np.sum(x_axis * data) / np.sum(data)
-    center_y = np.sum(y_axis * data) / np.sum(data)
-
-    sigma_x = (x_axis.max() - x_axis.min()) / 3.
-    sigma_y = (y_axis.max() - y_axis.min()) / 3.
-    theta = 0.0
-    offset = float(data.min())
-    error = 0
-    # check for sensible values
-    parameters = [x_axis, y_axis, data]
-    for var in parameters:
-        # FIXME: Why don't you check earlier?
-        # FIXME: Check for 1D array, 2D
-        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
-            self.log.error('Given parameter is not an array.')
-            amplitude = 0.
-            center_x = 0.
-            center_y = 0.
-            sigma_x = 0.
-            sigma_y = 0.
-            theta = 0.0
-            offset = 0.
-            error = -1
-
-    # auxiliary variables:
-    stepsize_x = x_axis[1]-x_axis[0]
-    stepsize_y = y_axis[1]-y_axis[0]
-    n_steps_x = len(x_axis)
-    n_steps_y = len(y_axis)
-
-    # populate the parameter container:
-    params['amplitude'].set(value=amplitude, min=100, max=1e7)
-    params['sigma_x'].set(value=sigma_x, min=1*stepsize_x,
-                          max=3*(x_axis[-1]-x_axis[0]))
-    params['sigma_y'].set(value=sigma_y, min=1*stepsize_y,
-                          max=3*(y_axis[-1]-y_axis[0]))
-    params['center_x'].set(value=center_x, min=(x_axis[0])-n_steps_x*stepsize_x,
-                           max=x_axis[-1]+n_steps_x*stepsize_x)
-    params['center_y'].set(value=center_y, min=(y_axis[0])-n_steps_y*stepsize_y,
-                           max=y_axis[-1]+n_steps_y*stepsize_y)
-    params['theta'].set(value=theta, min=0, max=np.pi)
-    params['offset'].set(value=offset, min=0, max=1e7)
-
-    return error, params
+# -*- coding: utf-8 -*-
+
+"""
+This file contains methods for gaussian-like fitting, these methods
+are imported by class FitLogic.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+
+from collections import OrderedDict
+
+import numpy as np
+from lmfit import Parameters
+from lmfit.models import Model
+from scipy.ndimage import filters
+
+
+############################################################################
+#                                                                          #
+#                          Defining models                                 #
+#                                                                          #
+############################################################################
+
+####################################
+# Gaussian model                   #
+####################################
+
+
+def make_gaussianwithoutoffset_model(self, prefix=None):
+    """ Create a model of a gaussian with specified amplitude.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+
+    For further information have a look in:
+    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html
+    """
+
+    def physical_gauss(x, center, sigma):
+        """ Function of a bare Gaussian with unit height at center.
+
+        @param numpy.array x: independent variable - e.g. frequency
+        @param float center: center around which the distributions (expectation
+                             value).
+        @param float sigma: standard deviation of the gaussian
+
+        @return: numpy.array with length equals to input x and with the values
+                 of a bare Gaussian.
+        """
+        return np.exp(- np.power((center - x), 2) / (2 * np.power(sigma, 2)))
+
+    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                       'cannot be used as a prefix and will be ignored for now.'
+                       'Correct that!'.format(prefix, type(prefix)))
+        gaussian_model = Model(physical_gauss, independent_vars=['x'])
+    else:
+        gaussian_model = Model(physical_gauss, independent_vars=['x'],
+                               prefix=prefix)
+
+    full_gaussian_model = amplitude_model * gaussian_model
+
+    if prefix is None:
+        prefix = ''
+    full_gaussian_model.set_param_hint('{0!s}fwhm'.format(prefix),
+                                       expr="2.3548200450309493*{0}sigma".format(prefix))
+
+    params = full_gaussian_model.make_params()
+
+    return full_gaussian_model, params
+
+####################################
+# 1D Gaussian model with offset    #
+####################################
+
+def make_gaussian_model(self, prefix=None):
+    """ Create a gauss model with amplitude and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+    """
+
+    gaussian_model, params = self.make_gaussianwithoutoffset_model(prefix=prefix)
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    gaussian_offset_model = gaussian_model + constant_model
+
+    if prefix is None:
+        prefix = ''
+
+    gaussian_offset_model.set_param_hint('{0}contrast'.format(prefix),
+                                         expr='({0}amplitude/offset)*100'.format(prefix))
+
+    params = gaussian_offset_model.make_params()
+
+    return gaussian_offset_model, params
+
+######################################################
+# 1D Gaussian model with linear (inclined) offset    #
+######################################################
+
+def make_gaussianlinearoffset_model(self, prefix=None):
+    """ Create a gauss with a linear offset (i.e. a slope).
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+    """
+
+    # Note that the offset parameter comes here from the gauss model and not
+    # from the slope model.
+    slope_model, params = self.make_slope_model(prefix)
+    gaussian_model, params = self.make_gaussian_model(prefix)
+
+    gaussian_linear_offset = gaussian_model + slope_model
+    params = gaussian_linear_offset.make_params()
+
+    return gaussian_linear_offset, params
+
+##########################################
+# 1D Multiple Gaussian Model with offset #
+##########################################
+
+
+def make_multiplegaussianoffset_model(self, no_of_functions=1):
+    """ Create a model with multiple gaussian with offset.
+
+    @param no_of_functions: for default=1 there is one gaussian, else
+                            more functions are added
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+    """
+
+    if no_of_functions == 1:
+        multi_gaussian_model, params = self.make_gaussian_model()
+    else:
+
+        prefix = 'g0_'
+        multi_gaussian_model, params = self.make_gaussianwithoutoffset_model(prefix=prefix)
+
+        constant_model, params = self.make_constant_model()
+        multi_gaussian_model = multi_gaussian_model + constant_model
+
+        multi_gaussian_model.set_param_hint('{0}contrast'.format(prefix),
+                                            expr='({0}amplitude/offset)*100'.format(prefix))
+
+        for ii in range(1, no_of_functions):
+
+            prefix = 'g{0:d}_'.format(ii)
+            multi_gaussian_model += self.make_gaussianwithoutoffset_model(prefix=prefix)[0]
+            multi_gaussian_model.set_param_hint('{0}contrast'.format(prefix),
+                                                expr='({0}amplitude/offset)*100'.format(prefix))
+
+    params = multi_gaussian_model.make_params()
+
+    return multi_gaussian_model, params
+
+##########################################
+#   1D Double Gaussian Model with offset #
+##########################################
+
+
+def make_gaussiandouble_model(self):
+    """ Create a model with double gaussian with offset.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+    """
+
+    return self.make_multiplegaussianoffset_model(no_of_functions=2)
+
+##########################################
+#   1D Triple Gaussian Model with offset #
+##########################################
+
+
+def make_gaussiantriple_model(self):
+    """ Create a model with double gaussian with offset.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+    """
+
+    return self.make_multiplegaussianoffset_model(no_of_functions=3)
+
+#####################
+# 2D gaussian model #
+#####################
+
+def make_twoDgaussian_model(self, prefix=None):
+    """ Creates a model of the 2D gaussian function.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_gaussianwithoutoffset_model.
+
+    """
+
+    def twoDgaussian_function(x, amplitude, center_x, center_y, sigma_x, sigma_y,
+                              theta, offset):
+        """ Provide a two dimensional gaussian function.
+
+        @param float amplitude: Amplitude of gaussian
+        @param float center_x: x value of maximum
+        @param float center_y: y value of maximum
+        @param float sigma_x: standard deviation in x direction
+        @param float sigma_y: standard deviation in y direction
+        @param float theta: angle for eliptical gaussians
+        @param float offset: offset
+
+        @return callable function: returns the reference to the function
+
+        Function taken from:
+        http://stackoverflow.com/questions/21566379/fitting-a-2d-gaussian-function-using-scipy-optimize-curve-fit-valueerror-and-m/21566831
+
+        Question from: http://stackoverflow.com/users/2097737/bland
+                       http://stackoverflow.com/users/3273102/kokomoking
+                       http://stackoverflow.com/users/2767207/jojodmo
+        Answer: http://stackoverflow.com/users/1461210/ali-m
+                http://stackoverflow.com/users/5234/mrjrdnthms
+        """
+
+        # FIXME: x_data_tuple: dimension of arrays
+        # @param np.arra[k][M] x_data_tuple: array which is (k,M)-shaped,
+        #                                   x and y values
+
+        (u, v) = x
+        center_x = float(center_x)
+        center_y = float(center_y)
+
+        a = (np.cos(theta) ** 2) / (2 * sigma_x ** 2) \
+            + (np.sin(theta) ** 2) / (2 * sigma_y ** 2)
+        b = -(np.sin(2 * theta)) / (4 * sigma_x ** 2) \
+            + (np.sin(2 * theta)) / (4 * sigma_y ** 2)
+        c = (np.sin(theta) ** 2) / (2 * sigma_x ** 2) \
+            + (np.cos(theta) ** 2) / (2 * sigma_y ** 2)
+        g = offset + amplitude * np.exp(- (a * ((u - center_x) ** 2)
+                                           + 2 * b * (u - center_x) * (v - center_y)
+                                           + c * ((v - center_y) ** 2)))
+        return g.ravel()
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                     'cannot be used as a prefix and will be ignored for now.'
+                     'Correct that!'.format(prefix, type(prefix)))
+        gaussian_2d_model = Model(twoDgaussian_function, independent_vars=['x'])
+    else:
+        gaussian_2d_model = Model(twoDgaussian_function, independent_vars=['x'],
+                               prefix=prefix)
+
+    params = gaussian_2d_model.make_params()
+
+    return gaussian_2d_model, params
+
+################################################################################
+#                                                                              #
+#                    Fit functions and their estimators                        #
+#                                                                              #
+################################################################################
+
+###################################
+# 1D Gaussian with flat offset    #
+###################################
+
+def make_gaussian_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a 1D gaussian peak fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+
+    mod_final, params = self.make_gaussian_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The 1D gaussian peak fit did not work. Error '
+                       'message: {0}\n'.format(result.message))
+
+    if units is None:
+            units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = OrderedDict()  # create result string for gui
+
+    #result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+    #                                    'error': result.params['amplitude'].stderr,
+    #                                    'unit': units[1]}                               #amplitude
+
+    result_str_dict['Position'] = {'value': result.params['center'].value,
+                                        'error': result.params['center'].stderr,
+                                        'unit': units[0]}                               #position
+
+    #result_str_dict['Standard deviation'] = {'value': result.params['sigma'].value,
+    #                                'error': result.params['sigma'].stderr,
+    #                                'unit': units[0]}                               #standart deviation
+
+    result_str_dict['Linewidth'] = {'value': result.params['fwhm'].value,
+                                        'error': result.params['fwhm'].stderr,
+                                        'unit': units[0]}                               #FWHM
+
+    result_str_dict['Contrast'] = {'value': result.params['contrast'].value,
+                                        'error': result.params['contrast'].stderr,
+                                        'unit': '%'}                                    #Contrast
+    result.result_str_dict = result_str_dict
+
+    return result
+
+
+
+def estimate_gaussian_peak(self, x_axis, data, params):
+    """ Provides a gaussian offset peak estimator.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+        Explanation of the return parameter:
+            int error: error code (0:OK, -1:error)
+            Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # If the estimator is not good enough one can start improvement with
+    # a convolution
+
+    # auxiliary variables
+    stepsize = abs(x_axis[1] - x_axis[0])
+    n_steps = len(x_axis)
+
+    # Smooth the provided data, so that noise fluctuations will not disturb the
+    # parameter estimation. This value performs the best in many scenarios:
+    std_dev = 2
+    data_smoothed = filters.gaussian_filter1d(data, std_dev)
+
+    # Define constraints:
+    # maximal and minimal the length of the given array to the right and to the
+    # left:
+    center_min = (x_axis[0]) - n_steps * stepsize
+    center_max = (x_axis[-1]) + n_steps * stepsize
+    ampl_min = 0
+    sigma_min = stepsize
+    sigma_max = 3 * (x_axis[-1] - x_axis[0])
+
+    # set parameters:
+    offset = data_smoothed.min()
+    params['offset'].set(value=offset)
+
+    # it is more reliable to select the maximal value rather then
+    # calculating the first moment of the gaussian distribution (which is the
+    # mean value), since it is unreliable if the distribution begins or ends at
+    # the edges of the data (but it helps a lot for standard deviation):
+    mean_val_calc = np.sum(x_axis*data_smoothed) / np.sum(data_smoothed)
+    params['center'].set(value=x_axis[np.argmax(data_smoothed)],
+                         min=center_min, max=center_max)
+
+    # calculate the second moment of the gaussian distribution:
+    #   int (x^2 * f(x) dx) :
+    mom2 = np.sum(x_axis ** 2 * data_smoothed) / np.sum(data_smoothed)
+
+    # and use the standard formula to obtain the standard deviation:
+    #   sigma^2 = int( (x - mean)^2 f(x) dx ) = int (x^2 * f(x) dx) - mean^2
+
+    # If the mean is situated at the edges of the distribution then this
+    # procedure performs better then setting the initial value for sigma to
+    # 1/3 of the length of the distribution since the calculated value for the
+    # mean is then higher, which will decrease eventually the initial value for
+    # sigma. But if the peak values is within the distribution the standard
+    # deviation formula performs even better:
+    params['sigma'].set(value=np.sqrt(abs(mom2 - mean_val_calc**2)),
+                        min=sigma_min, max=sigma_max)
+    # params['sigma'].set(value=(x_axis.max() - x_axis.min()) / 3.)
+
+    # Do not set the maximal amplitude value based on the distribution, since
+    # the fit will fail if the peak is at the edges or beyond the range of the
+    # x values.
+    params['amplitude'].set(value=data_smoothed.max()-data_smoothed.min(),
+                            min=ampl_min)
+
+    return error, params
+
+def estimate_gaussian_dip(self, x_axis, data, params):
+    """ Provides a gaussian offset dip estimator.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+        Explanation of the return parameter:
+            int error: error code (0:OK, -1:error)
+            Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # the peak and dip gaussian have the same parameters:
+    params_peak = params
+    data_negative = data * (-1)
+
+    error, params_ret = self.estimate_gaussian_peak(x_axis,
+                                                          data_negative,
+                                                          params_peak
+                                                          )
+
+    params['sigma'] = params_ret['sigma']
+    params['offset'].set(value=-params_ret['offset'])
+    # set the maximum to infinity, since that is the default value.
+    params['amplitude'].set(value=-params_ret['amplitude'].value, min=-np.inf,
+                            max=1e-12)
+    params['center'] = params_ret['center']
+
+    return error, params
+
+##############################################
+# 1D Gaussian with linear inclined offset    #
+##############################################
+
+def make_gaussianlinearoffset_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a 1D gaussian peak fit with linear offset on the provided data.
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+
+    mod_final, params = self.make_gaussianlinearoffset_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The 1D gaussian peak fit did not work. Error '
+                       'message: {0}\n'.format(result.message))
+    if units is None:
+            units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = OrderedDict()  # create result string for gui
+
+    #result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+    #                                    'error': result.params['amplitude'].stderr,
+    #                                    'unit': units[1]}                               #amplitude
+
+    result_str_dict['Position'] = {'value': result.params['center'].value,
+                                        'error': result.params['center'].stderr,
+                                        'unit': units[0]}                               #position
+
+    #result_str_dict['Standard deviation'] = {'value': result.params['sigma'].value,
+    #                                'error': result.params['sigma'].stderr,
+    #                                'unit': units[0]}                               #standart deviation
+
+    result_str_dict['Linewidth'] = {'value': result.params['fwhm'].value,
+                                        'error': result.params['fwhm'].stderr,
+                                        'unit': units[0]}                               #FWHM
+
+    result_str_dict['Contrast'] = {'value': result.params['contrast'].value,
+                                        'error': result.params['contrast'].stderr,
+                                        'unit': '%'}                                    #Contrast
+
+    #result_str_dict['Slope'] = {'value': result.params['slope'].value,
+    #                                    'error': result.params['slope'].stderr,
+    #                                    'unit': ''}                                    #Slope
+
+    result.result_str_dict = result_str_dict
+
+    return result
+
+def estimate_gaussianlinearoffset_peak(self, x_axis, data, params):
+    """ Provides a gauss peak estimator with a linear changing offset.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+        Explanation of the return parameter:
+            int error: error code (0:OK, -1:error)
+            Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # try at first a fit with the ordinary gauss function
+    res_ordinary_gauss = self.make_gaussian_fit(
+        x_axis=x_axis,
+        data=data,
+        units=None,
+        estimator=self.estimate_gaussian_peak
+    )
+
+    # subtract the result and perform again a linear fit:
+    data_subtracted = data - res_ordinary_gauss.best_fit
+
+    res_linear = self.make_linear_fit(
+        x_axis=x_axis,
+        data=data_subtracted,
+        estimator=self.estimate_linear
+    )
+
+    # this way works much better than performing at first a linear fit,
+    # subtracting the fit and make an ordinary gaussian fit. Especially for a
+    # peak at the borders, this method is much more beneficial.
+
+    # assign the obtained values for the initial fit:
+    params['offset'] = res_ordinary_gauss.params['offset']
+    params['center'] = res_ordinary_gauss.params['center']
+    params['amplitude'] = res_ordinary_gauss.params['amplitude']
+    params['sigma'] = res_ordinary_gauss.params['sigma']
+    params['slope'] = res_linear.params['slope']
+
+    return error, params
+
+#################################
+# Two Gaussian with flat offset #
+#################################
+
+def make_gaussiandouble_fit(self, x_axis, data, estimator,
+                            units=None,
+                            add_params=None,
+                            threshold_fraction=0.4,
+                            minimal_threshold=0.2,
+                            sigma_threshold_fraction=0.3, **kwargs):
+    """ Perform a 1D two gaussian dip fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+    @param float threshold_fraction : Threshold to find second gaussian
+    @param float minimal_threshold: Threshold is lowerd to minimal this
+                                    value as a fraction
+    @param float sigma_threshold_fraction: Threshold for detecting
+                                           the end of the peak
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    model, params = self.make_multiplegaussianoffset_model(no_of_functions=2)
+
+    error, params = estimator(x_axis, data, params,
+                              threshold_fraction,
+                              minimal_threshold,
+                              sigma_threshold_fraction
+                              )
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The double gaussian dip fit did not work: {0}'.format(
+            result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+
+    result_str_dict['Position 0'] = {'value': result.params['g0_center'].value,
+                                     'error': result.params['g0_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Position 1'] = {'value': result.params['g1_center'].value,
+                                     'error': result.params['g1_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Contrast 0'] = {'value': abs(result.params['g0_contrast'].value),
+                                     'error': result.params['g0_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['Contrast 1'] = {'value': abs(result.params['g1_contrast'].value),
+                                     'error': result.params['g1_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['Linewidth 0'] = {'value': result.params['g0_sigma'].value,
+                                      'error': result.params['g0_sigma'].stderr,
+                                      'unit': units[0]}
+
+    result_str_dict['Linewidth 1'] = {'value': result.params['g1_sigma'].value,
+                                      'error': result.params['g1_sigma'].stderr,
+                                      'unit': units[0]}
+
+    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+def estimate_gaussiandouble_peak(self, x_axis, data, params,
+                                threshold_fraction=0.4, minimal_threshold=0.1,
+                                sigma_threshold_fraction=0.2):
+    """ Provide an estimator for a double gaussian peak fit with the parameters
+    coming from the physical properties of an experiment done in gated counter:
+                    - positive peak
+                    - no values below 0
+                    - rather broad overlapping functions
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+    @param float threshold_fraction : Threshold to find second gaussian
+    @param float minimal_threshold: Threshold is lowerd to minimal this
+                                    value as a fraction
+    @param float sigma_threshold_fraction: Threshold for detecting
+                                           the end of the peak
+
+    @return int error: error code (0:OK, -1:error)
+    @return Parameters object params: estimated values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+
+    mod_lor, params_lor = self.make_multiplelorentzian_model(no_of_functions=2)
+
+    error, params_lor = self.estimate_lorentziandouble_dip(x_axis=x_axis,
+                                                     data=-data,
+                                                     params=params_lor,
+                                                     threshold_fraction=threshold_fraction,
+                                                     minimal_threshold=minimal_threshold,
+                                                     sigma_threshold_fraction=sigma_threshold_fraction)
+
+    params['g0_amplitude'].value = -params_lor['l0_amplitude'].value
+    params['g0_center'].value = params_lor['l0_center'].value
+    params['g0_sigma'].value = params_lor['l0_sigma'].value/(np.sqrt(2*np.log(2)))
+    params['g1_amplitude'].value = -params_lor['l1_amplitude'].value
+    params['g1_center'].value = params_lor['l1_center'].value
+    params['g1_sigma'].value = params_lor['l1_sigma'].value/(np.sqrt(2*np.log(2)))
+    params['offset'].value = -params_lor['offset'].value
+
+    return error, params
+
+def estimate_gaussiandouble_dip(self, x_axis, data, params,
+                               threshold_fraction=0.4, minimal_threshold=0.1,
+                               sigma_threshold_fraction=0.2):
+    """ Provide an estimator for a double gaussian dip fit with the parameters
+    coming from the physical properties of an experiment done in gated counter:
+                    - positive peak
+                    - no values below 0
+                    - rather broad overlapping functions
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+    @param float threshold_fraction : Threshold to find second gaussian
+    @param float minimal_threshold: Threshold is lowerd to minimal this
+                                    value as a fraction
+    @param float sigma_threshold_fraction: Threshold for detecting
+                                           the end of the peak
+
+    @return int error: error code (0:OK, -1:error)
+    @return Parameters object params: estimated values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    mod_lor, params_lor = self.make_multiplelorentzian_model(no_of_functions=2)
+
+    error, params_lor = self.estimate_lorentziandouble_dip(x_axis=x_axis,
+                                                     data=data,
+                                                     params=params_lor,
+                                                     threshold_fraction=threshold_fraction,
+                                                     minimal_threshold=minimal_threshold,
+                                                     sigma_threshold_fraction=sigma_threshold_fraction)
+
+    params['g0_amplitude'].value = params_lor['l0_amplitude'].value
+    params['g0_center'].value = params_lor['l0_center'].value
+    params['g0_sigma'].value = params_lor['l0_sigma'].value/(np.sqrt(2*np.log(2)))
+    params['g1_amplitude'].value = params_lor['l1_amplitude'].value
+    params['g1_center'].value = params_lor['l1_center'].value
+    params['g1_sigma'].value = params_lor['l1_sigma'].value/(np.sqrt(2*np.log(2)))
+    params['offset'].value = params_lor['offset'].value
+
+    return error, params
+
+###################################
+# 2D Gaussian with flat offset    #
+###################################
+
+# TODO: I think this has an offset, and it should be named so to be consistent with
+#       the 1D functions.
+
+def make_twoDgaussian_fit(self, xy_axes, data, estimator, units=None, add_params=None, **kwargs):
+    """ This method performes a 2D gaussian fit on the provided data.
+
+    @param numpy.array xy_axes: 2D axes values. xy_axes[0] contains x_axis and
+                                xy_axes[1] contains y_axis
+    @param numpy.array data: 2D matrix data, should have the dimension as
+                             len(xy_axes[0]) x len(xy_axes[1]).
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+
+    x_axis, y_axis = xy_axes
+
+    gaussian_2d_model, params = self.make_twoDgaussian_model()
+
+    error, params = estimator(x_axis=x_axis, y_axis=y_axis,
+                              data=data, params=params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = gaussian_2d_model.fit(data, x=xy_axes, params=params, **kwargs)
+    except:
+        result = gaussian_2d_model.fit(data, x=xy_axes, params=params, **kwargs)
+        self.log.warning('The 2D gaussian fit did not work: {0}'.format(
+                       result.message))
+
+    return result
+
+def estimate_twoDgaussian(self, x_axis, y_axis, data, params):
+    """ Provide a simple two dimensional gaussian function.
+
+    @param numpy.array x_axis: 1D x axis values
+    @param numpy.array y_axis: 1D y axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+        Explanation of the return parameter:
+            int error: error code (0:OK, -1:error)
+            Parameters object params: set parameters of initial values
+    """
+
+    # TODO:Make clever estimator
+    # FIXME: 1D array x_axis, y_axis, 2D data???
+
+    #            #needed me 1 hour to think about, but not needed in the end...maybe needed at a later point
+    #            len_x=np.where(x_axis[0]==x_axis)[0][1]
+    #            len_y=len(data)/len_x
+
+    amplitude = float(data.max() - data.min())
+
+    center_x = x_axis[data.argmax()]
+    center_y = y_axis[data.argmax()]
+
+    sigma_x = (x_axis.max() - x_axis.min()) / 3.
+    sigma_y = (y_axis.max() - y_axis.min()) / 3.
+    theta = 0.0
+    offset = float(data.min())
+
+    # check for sensible values
+    parameters = [x_axis, y_axis, data]
+
+    error = 0
+    for var in parameters:
+        # FIXME: Why don't you check earlier?
+        # FIXME: Check for 1D array, 2D
+        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
+            self.log.error('Given parameter is not an array.')
+            amplitude = 0.
+            center_x = 0.
+            center_y = 0.
+            sigma_x = 0.
+            sigma_y = 0.
+            theta = 0.0
+            offset = 0.
+            error = -1
+
+    # auxiliary variables:
+    stepsize_x = x_axis[1]-x_axis[0]
+    stepsize_y = y_axis[1]-y_axis[0]
+    n_steps_x = len(x_axis)
+    n_steps_y = len(y_axis)
+
+    # populate the parameter container:
+    params['amplitude'].set(value=amplitude, min=100, max=1e7)
+    params['sigma_x'].set(value=sigma_x, min=1*stepsize_x,
+                          max=3*(x_axis[-1]-x_axis[0]))
+    params['sigma_y'].set(value=sigma_y, min=1*stepsize_y,
+                          max=3*(y_axis[-1]-y_axis[0]))
+    params['center_x'].set(value=center_x, min=(x_axis[0])-n_steps_x*stepsize_x,
+                           max=x_axis[-1]+n_steps_x*stepsize_x)
+    params['center_y'].set(value=center_y, min=(y_axis[0])-n_steps_y*stepsize_y,
+                           max=y_axis[-1]+n_steps_y*stepsize_y)
+    params['theta'].set(value=theta, min=0, max=np.pi)
+    params['offset'].set(value=offset, min=0, max=1e7)
+
+    return error, params
+
+def estimate_twoDgaussian_MLE(self, x_axis, y_axis, data, params):
+    """ Provide an estimator for 2D gaussian based on maximum likelihood estimation.
+
+    @param numpy.array x_axis: 1D x axis values
+    @param numpy.array y_axis: 1D y axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+        Explanation of the return parameter:
+            int error: error code (0:OK, -1:error)
+            Parameters object params: set parameters of initial values
+
+    For the parameters characterizing of the two dimensional gaussian a maximum
+    likelihood estimation is used (at the moment only for the center_x and
+    center_y values).
+    """
+
+    # TODO: Make good estimates for sigma_x, sigma_y and theta
+
+    amplitude = float(data.max() - data.min())
+
+    # By calculating the log likelihood of the 2D gaussian pdf, one obtain for
+    # the minimization of the center_x or center_y values the following formula
+    # (which are in fact just the expectation/mean value formula):
+    center_x = np.sum(x_axis * data) / np.sum(data)
+    center_y = np.sum(y_axis * data) / np.sum(data)
+
+    sigma_x = (x_axis.max() - x_axis.min()) / 3.
+    sigma_y = (y_axis.max() - y_axis.min()) / 3.
+    theta = 0.0
+    offset = float(data.min())
+    error = 0
+    # check for sensible values
+    parameters = [x_axis, y_axis, data]
+    for var in parameters:
+        # FIXME: Why don't you check earlier?
+        # FIXME: Check for 1D array, 2D
+        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
+            self.log.error('Given parameter is not an array.')
+            amplitude = 0.
+            center_x = 0.
+            center_y = 0.
+            sigma_x = 0.
+            sigma_y = 0.
+            theta = 0.0
+            offset = 0.
+            error = -1
+
+    # auxiliary variables:
+    stepsize_x = x_axis[1]-x_axis[0]
+    stepsize_y = y_axis[1]-y_axis[0]
+    n_steps_x = len(x_axis)
+    n_steps_y = len(y_axis)
+
+    # populate the parameter container:
+    params['amplitude'].set(value=amplitude, min=100, max=1e7)
+    params['sigma_x'].set(value=sigma_x, min=1*stepsize_x,
+                          max=3*(x_axis[-1]-x_axis[0]))
+    params['sigma_y'].set(value=sigma_y, min=1*stepsize_y,
+                          max=3*(y_axis[-1]-y_axis[0]))
+    params['center_x'].set(value=center_x, min=(x_axis[0])-n_steps_x*stepsize_x,
+                           max=x_axis[-1]+n_steps_x*stepsize_x)
+    params['center_y'].set(value=center_y, min=(y_axis[0])-n_steps_y*stepsize_y,
+                           max=y_axis[-1]+n_steps_y*stepsize_y)
+    params['theta'].set(value=theta, min=0, max=np.pi)
+    params['offset'].set(value=offset, min=0, max=1e7)
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/generalmethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/generalmethods.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,545 +1,545 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains general methods which are imported by class FitLogic.
-These general methods are available for all different fitting methods.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-
-from collections import OrderedDict
-
-import lmfit
-import numpy as np
-from lmfit import Parameters
-from scipy.ndimage import convolve1d
-from scipy.signal import gaussian
-
-
-############################################################################
-#                                                                          #
-#                             General methods                              #
-#                                                                          #
-############################################################################
-
-def _substitute_params(self, initial_params, update_params=None):
-    """ Substitute all parameters handed in the update_parameters object in an
-        initial set of parameters.
-
-    @param lmfit.parameter.Parameters initial_params: object containing initial
-                                                      parameters which will be
-                                                      either updated or set.
-    @param lmfit.parameter.Parameters or dict update_params:
-                parameter object or dict with parameters to update the
-                initial_params. For a lmfit.parameter.Parameters object have a
-                look at:
-
-    https://lmfit.github.io/lmfit-py/parameters.html#lmfit.parameter.Parameters
-
-                An update_params can also be a dict e.g. like:
-                    update_dict=dict()
-                    update_dict['c']={'min':0, 'max':120, 'vary':True,
-                                      'value':0.1, 'expr':None}
-
-    @return lmfit.parameter.Parameters: object with substituted parameters. If
-                                        update_params is None, then no parameter
-                                        will be updated in initial_params and it
-                                        will be returned as it is.
-    """
-
-    if update_params is None:
-        return initial_params
-
-    # Check the case for an lmfit.parameter.Parameters
-    elif type(update_params) == lmfit.parameter.Parameters:
-
-        # Go though each parameter in the Parameters object
-        for para in update_params:
-
-            if para not in initial_params:
-                initial_params.add(para)
-            if update_params[para].min is not None:
-                initial_params[para].min = update_params[para].min
-
-            if update_params[para].max is not None:
-                initial_params[para].max = update_params[para].max
-
-            if update_params[para].vary is not None:
-                initial_params[para].vary = update_params[para].vary
-
-            if update_params[para].expr is not None:
-                initial_params[para].expr = update_params[para].expr
-
-            if update_params[para].value is not None:
-
-                # Adapt the limits to the value:
-                if (initial_params[para].min is not None) and (initial_params[para].min > update_params[para].value):
-                   initial_params[para].min = update_params[para].value
-
-                if (initial_params[para].max is not None) and (initial_params[para].max < update_params[para].value):
-                   initial_params[para].max = update_params[para].value
-
-                initial_params[para].value = update_params[para].value
-
-    # Check the case for an OrderedDict or dict parameter:
-    elif type(update_params) == OrderedDict or type(update_params) == dict:
-
-        for para in update_params:
-            if para not in initial_params:
-                initial_params.add(para)
-            if 'min' in update_params[para]:
-                initial_params[para].min = update_params[para]['min']
-
-            if 'max' in update_params[para]:
-                initial_params[para].max = update_params[para]['max']
-
-            if 'vary' in update_params[para]:
-                initial_params[para].vary = update_params[para]['vary']
-
-            if 'expr' in update_params[para]:
-                initial_params[para].expr = update_params[para]['expr']
-
-            if 'value' in update_params[para]:
-
-                # Adapt the limits to the value:
-                if (initial_params[para].min is not None) and (initial_params[para].min > update_params[para]['value']):
-                    initial_params[para].min = update_params[para]['value']
-
-                if (initial_params[para].max is not None) and (initial_params[para].max < update_params[para]['value']):
-                    initial_params[para].max = update_params[para]['value']
-
-                initial_params[para].value = update_params[para]['value']
-
-    else:
-        self.log.error('The type of the passed update_params object <{0}> is '
-                     'neither of type lmfit.parameter.Parameters, '
-                     'OrderedDict or dict! Correct that, the initial_params'
-                     'will be returned.'.format(type(update_params)))
-
-    return initial_params
-
-def create_fit_string(self, result, model, units=None, decimal_digits_value_given=None,
-                      decimal_digits_err_given=None):
-    """ This method can produces a well readable string from the results of a fitted model.
-    If units is not given or one unit missing there will be no unit in string.
-    If decimal_digits_value_given is not provided it will be set to precision of error and digits
-    of error will be set to 1.
-
-    @param lmfit object result: the fitting result
-    @param lmfit object model: the corresponding model
-    @param dict units: units for parameters of model if not given all units are set to "arb. u."
-    @param int decimal_digits_err_given: (optional) number of decimals displayed in output for error
-    @param int decimal_digits_value_given: (optional) number of decimals displayed in output for value
-
-    @return str fit_result: readable string
-    """
-    if units is None:
-        units = dict()
-    # TODO: Add multiplicator
-    # TODO: Add decimal dict
-    # TODO: Add sensible output such that e only multiple of 3 and err and value have same exponent
-
-    fit_result = ''
-    for variable in model.param_names:
-        # check order of number
-        exponent_error = int("{:e}".format(result.params[variable].stderr)[-3:])
-        exponent_value = int("{:e}".format(result.params[variable].value)[-3:])
-        if decimal_digits_value_given is None:
-            decimal_digits_value = int(exponent_value-exponent_error+1)
-            if decimal_digits_value <= 0:
-                decimal_digits_value = 1
-        if decimal_digits_err_given is None:
-            decimal_digits_err = 1
-            if decimal_digits_err <= 0:
-                decimal_digits_err = 1
-        try:
-            fit_result += ("{0} [{1}] : {2} ± {3}\n".format(str(variable),
-                                                            units[variable],
-                                                            "{0:.{1}e}".format(
-                                                                float(result.params[variable].value),
-                                                                decimal_digits_value),
-                                                            "{0:.{1}e}".format(
-                                                                float(result.params[variable].stderr),
-                                                                decimal_digits_err)))
-        except:
-            # self.log.warning('No unit given for parameter {}, setting unit '
-            #             'to empty string'.format(variable))
-            fit_result += ("{0} [{1}] : {2} ± {3}\n".format(str(variable),
-                                                            "arb. u.",
-                                                            "{0:.{1}e}".format(
-                                                                float(result.params[variable].value),
-                                                                decimal_digits_value),
-                                                            "{0:.{1}e}".format(
-                                                                float(result.params[variable].stderr),
-                                                                decimal_digits_err)))
-    return fit_result
-
-
-def _search_end_of_dip(self, direction, data, peak_arg, start_arg, end_arg, sigma_threshold, minimal_threshold, make_prints):
-    """
-    data has to be offset leveled such that offset is substracted
-    """
-    # Todo: Create doc string
-    absolute_min  = data[peak_arg]
-
-    if direction == 'left':
-        mult = -1
-        sigma_arg=start_arg
-    elif direction == 'right':
-        mult = +1
-        sigma_arg=end_arg
-    else:
-        print('No valid direction in search end of peak')
-    ii=0
-
-    #if the minimum is at the end set this as boarder
-    if (peak_arg != start_arg and direction=='left' or
-        peak_arg != end_arg   and direction=='right'):
-        while True:
-            # if no minimum can be found decrease threshold
-            if ((peak_arg-ii<start_arg and direction == 'left') or
-                (peak_arg+ii>end_arg   and direction=='right')):
-                sigma_threshold*=0.9
-                ii=0
-                if make_prints:
-                    print('h1 sigma_threshold',sigma_threshold)
-
-            #if the dip is always over threshold the end is as
-            # set before
-            if abs(sigma_threshold/absolute_min)<abs(minimal_threshold):
-                if make_prints:
-                    print('h2')
-                break
-
-             #check if value was changed and search is finished
-            if ((sigma_arg == start_arg and direction == 'left') or
-                (sigma_arg == end_arg   and direction=='right')):
-                # check if if value is lower as threshold this is the
-                # searched value
-                if make_prints:
-                    print('h3')
-                if abs(data[peak_arg+(mult*ii)])<abs(sigma_threshold):
-                    # value lower than threshold found - left end found
-                    sigma_arg=peak_arg+(mult*ii)
-                    if make_prints:
-                        print('h4')
-                    break
-            ii+=1
-
-    # in this case the value is the last index and should be search set
-    # as right argument
-    else:
-        if make_prints:
-            print('neu h10')
-        sigma_arg=peak_arg
-
-    return sigma_threshold,sigma_arg
-
-
-def _search_double_dip(self, x_axis, data, threshold_fraction=0.3,
-                       minimal_threshold=0.01, sigma_threshold_fraction=0.3,
-                       make_prints=False):
-    """ This method searches for a double dip. There are three values which can be set in order to adjust
-    the search. A threshold which defines when  a minimum is a dip,
-    this threshold is then lowered if no dip can be found until the
-    minimal threshold which sets the absolute boarder and a
-    sigma_threshold_fraction which defines when the
-
-    @param array x_axis: x values
-    @param array data: value of each data point corresponding to
-                        x values
-    @param float threshold_fraction: x values
-    @param float minimal_threshold: x values
-    @param float sigma_threshold_fraction: x values
-
-
-    @return int error: error code (0:OK, -1:error)
-    @return int sigma0_argleft: index of left side of 1st peak
-    @return int dip0_arg: index of max of 1st peak
-    @return int sigma0_argright: index of right side of 1st peak
-    @return int sigma1_argleft: index of left side of 2nd peak
-    @return int dip1_arg: index of max side of 2nd peak
-    @return int sigma1_argright: index of right side of 2nd peak
-    """
-
-    if sigma_threshold_fraction is None:
-        sigma_threshold_fraction=threshold_fraction
-
-    error=0
-
-    #first search for absolute minimum
-    absolute_min=data.min()
-    absolute_argmin=data.argmin()
-
-    #adjust thresholds
-    threshold=threshold_fraction*absolute_min
-    sigma_threshold=sigma_threshold_fraction*absolute_min
-
-    dip0_arg = absolute_argmin
-
-    # ====== search for the left end of the dip ======
-
-    sigma_threshold, sigma0_argleft = self._search_end_of_dip(
-                             direction='left',
-                             data=data,
-                             peak_arg = absolute_argmin,
-                             start_arg = 0,
-                             end_arg = len(data)-1,
-                             sigma_threshold = sigma_threshold,
-                             minimal_threshold = minimal_threshold,
-                             make_prints= make_prints)
-
-    if make_prints:
-        print('Left sigma of main peak: ',x_axis[sigma0_argleft])
-
-    # ====== search for the right end of the dip ======
-    # reset sigma_threshold
-
-    sigma_threshold, sigma0_argright = self._search_end_of_dip(
-                             direction='right',
-                             data=data,
-                             peak_arg = absolute_argmin,
-                             start_arg = 0,
-                             end_arg = len(data)-1,
-                             sigma_threshold = sigma_threshold_fraction*absolute_min,
-                             minimal_threshold = minimal_threshold,
-                             make_prints= make_prints)
-
-    if make_prints:
-        print('Right sigma of main peak: ',x_axis[sigma0_argright])
-
-    # ======== search for second lorentzian dip ========
-    left_index=int(0)
-    right_index=len(x_axis)-1
-
-    mid_index_left=sigma0_argleft
-    mid_index_right=sigma0_argright
-
-    # if main first dip covers the whole left side search on the right
-    # side only
-    if mid_index_left==left_index:
-        if make_prints:
-            print('h11', left_index,mid_index_left,mid_index_right,right_index)
-        #if one dip is within the second they have to be set to one
-        if mid_index_right==right_index:
-            dip1_arg=dip0_arg
-        else:
-            dip1_arg=data[mid_index_right:right_index].argmin()+mid_index_right
-
-    #if main first dip covers the whole right side search on the left
-    # side only
-    elif mid_index_right==right_index:
-        if make_prints:
-            print('h12')
-        #if one dip is within the second they have to be set to one
-        if mid_index_left==left_index:
-            dip1_arg=dip0_arg
-        else:
-            dip1_arg=data[left_index:mid_index_left].argmin()
-
-    # search for peak left and right of the dip
-    else:
-        while True:
-            #set search area excluding the first dip
-            left_min=data[left_index:mid_index_left].min()
-            left_argmin=data[left_index:mid_index_left].argmin()
-            right_min=data[mid_index_right:right_index].min()
-            right_argmin=data[mid_index_right:right_index].argmin()
-
-            if abs(left_min) > abs(threshold) and \
-               abs(left_min) > abs(right_min):
-                if make_prints:
-                    print('h13')
-                # there is a minimum on the left side which is higher
-                # than the minimum on the right side
-                dip1_arg = left_argmin+left_index
-                break
-            elif abs(right_min)>abs(threshold):
-                # there is a minimum on the right side which is higher
-                # than on left side
-                dip1_arg=right_argmin+mid_index_right
-                if make_prints:
-                    print('h14')
-                break
-            else:
-                # no minimum at all over threshold so lowering threshold
-                #  and resetting search area
-                threshold*=0.9
-                left_index=int(0)
-                right_index=len(x_axis)-1
-                mid_index_left=sigma0_argleft
-                mid_index_right=sigma0_argright
-                if make_prints:
-                    print('h15')
-                #if no second dip can be found set both to same value
-                if abs(threshold/absolute_min)<abs(minimal_threshold):
-                    if make_prints:
-                        print('h16')
-                    self.log.warning('Threshold to minimum ratio was too '
-                            'small to estimate two minima. So both '
-                            'are set to the same value')
-                    error=-1
-                    dip1_arg=dip0_arg
-                    break
-
-    # if the dip is exactly at one of the boarders that means
-    # the dips are most probably overlapping
-    if dip1_arg in (sigma0_argleft, sigma0_argright):
-        #print('Dips are overlapping')
-        distance_left  = abs(dip0_arg - sigma0_argleft)
-        distance_right = abs(dip0_arg - sigma0_argright)
-        sigma1_argleft = sigma0_argleft
-        sigma1_argright = sigma0_argright
-        if distance_left > distance_right:
-            dip1_arg = dip0_arg - abs(distance_left-distance_right)
-        elif distance_left < distance_right:
-            dip1_arg = dip0_arg + abs(distance_left-distance_right)
-        else:
-            dip1_arg = dip0_arg
-        #print(distance_left,distance_right,dip1_arg)
-    else:
-        # if the peaks are not overlapping search for left and right
-        # boarder of the dip
-
-        # ====== search for the right end of the dip ======
-        sigma_threshold, sigma1_argleft = self._search_end_of_dip(
-                                 direction='left',
-                                 data=data,
-                                 peak_arg = dip1_arg,
-                                 start_arg = 0,
-                                 end_arg = len(data)-1,
-                                 sigma_threshold = sigma_threshold_fraction*absolute_min,
-                                 minimal_threshold = minimal_threshold,
-                                 make_prints= make_prints)
-
-        # ====== search for the right end of the dip ======
-        sigma_threshold, sigma1_argright = self._search_end_of_dip(
-                                 direction='right',
-                                 data=data,
-                                 peak_arg = dip1_arg,
-                                 start_arg = 0,
-                                 end_arg = len(data)-1,
-                                 sigma_threshold = sigma_threshold_fraction*absolute_min,
-                                 minimal_threshold = minimal_threshold,
-                                 make_prints= make_prints)
-
-    return error, sigma0_argleft, dip0_arg, sigma0_argright, sigma1_argleft, dip1_arg, sigma1_argright
-
-
-############################################################################
-#                                                                          #
-#             Additional routines with Lorentzian-like filter              #
-#                                                                          #
-############################################################################
-
-def find_offset_parameter(self, x_values=None, data=None):
-    """ This method convolves the data with a Lorentzian and the finds the
-    offset which is supposed to be the most likely valy via a histogram.
-    Additional the smoothed data is returned
-
-    @param array x_values: x values
-    @param array data: value of each data point corresponding to
-                        x values
-
-    @return int error: error code (0:OK, -1:error)
-    @return float array data_smooth: smoothed data
-    @return float offset: estimated offset
-
-
-    """
-    # lorentzian filter
-    mod, params = self.make_lorentzian_model()
-
-    # Todo: exclude filter in seperate method to be used in other methods
-
-    if len(x_values) < 20.:
-        len_x = 5
-    elif len(x_values) >= 100.:
-        len_x = 10
-    else:
-        len_x = int(len(x_values)/10.)+1
-
-    lorentz = mod.eval(x=np.linspace(0, len_x, len_x), amplitude=1, offset=0.,
-                       sigma=len_x / 4., center=len_x / 2.)
-    data_smooth = convolve1d(data, lorentz / lorentz.sum(),
-                             mode='constant', cval=data.max())
-
-    # finding most frequent value which is supposed to be the offset
-    hist = np.histogram(data_smooth, bins=10)
-    offset = (hist[1][hist[0].argmax()]+hist[1][hist[0].argmax()+1])/2.
-
-    return data_smooth, offset
-
-############################################################################
-#                                                                          #
-#             Additional routines with gaussian-like filter              #
-#                                                                          #
-############################################################################
-
-def gaussian_smoothing(self, data=None, filter_len=None, filter_sigma=None):
-    """ This method convolves the data with a gaussian
-     the smoothed data is returned
-
-    @param array data: raw data
-    @param int filter_len: length of filter
-    @param int filter_sigma: width of gaussian
-
-    @return array: smoothed data
-
-    """
-    #Todo: Check for wrong data type
-    if filter_len is None:
-        if len(data) < 20.:
-            filter_len = 5
-        elif len(data) >= 100.:
-            filter_len = 10
-        else:
-            filter_len = int(len(data) / 10.) + 1
-    if filter_sigma is None:
-        filter_sigma = filter_len
-
-    gaus = gaussian(filter_len, filter_sigma)
-    return convolve1d(data, gaus / gaus.sum(), mode='mirror')
-
-
-
-def _check_1D_input(self, x_axis, data, params):
-    """ Helper function to check the input of the fit for general consistency.
-
-    @param numpy.array x_axis: x values
-    @param numpy.array data: value of each data point corresponding to x values
-    @param lmfit.Parameters params: a parameter object which will be filled with
-                                    initial values for the fit
-
-    @return int: error code (0:OK, -1:error)
-    """
-
-    error = 0
-    parameters = [x_axis, data]
-    for var in parameters:
-        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
-            self.log.error('Given parameter is no array.')
-            error = -1
-        elif len(np.shape(var)) != 1:
-            self.log.error('Given parameter is no one dimensional array.')
-            error = -1
-    if not isinstance(params, Parameters):
-        self.log.error('Parameters object is not valid in estimate_gaussian.')
-        error = -1
-
-    return error
-
+# -*- coding: utf-8 -*-
+"""
+This file contains general methods which are imported by class FitLogic.
+These general methods are available for all different fitting methods.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+
+from collections import OrderedDict
+
+import lmfit
+import numpy as np
+from lmfit import Parameters
+from scipy.ndimage import convolve1d
+from scipy.signal import gaussian
+
+
+############################################################################
+#                                                                          #
+#                             General methods                              #
+#                                                                          #
+############################################################################
+
+def _substitute_params(self, initial_params, update_params=None):
+    """ Substitute all parameters handed in the update_parameters object in an
+        initial set of parameters.
+
+    @param lmfit.parameter.Parameters initial_params: object containing initial
+                                                      parameters which will be
+                                                      either updated or set.
+    @param lmfit.parameter.Parameters or dict update_params:
+                parameter object or dict with parameters to update the
+                initial_params. For a lmfit.parameter.Parameters object have a
+                look at:
+
+    https://lmfit.github.io/lmfit-py/parameters.html#lmfit.parameter.Parameters
+
+                An update_params can also be a dict e.g. like:
+                    update_dict=dict()
+                    update_dict['c']={'min':0, 'max':120, 'vary':True,
+                                      'value':0.1, 'expr':None}
+
+    @return lmfit.parameter.Parameters: object with substituted parameters. If
+                                        update_params is None, then no parameter
+                                        will be updated in initial_params and it
+                                        will be returned as it is.
+    """
+
+    if update_params is None:
+        return initial_params
+
+    # Check the case for an lmfit.parameter.Parameters
+    elif type(update_params) == lmfit.parameter.Parameters:
+
+        # Go though each parameter in the Parameters object
+        for para in update_params:
+
+            if para not in initial_params:
+                initial_params.add(para)
+            if update_params[para].min is not None:
+                initial_params[para].min = update_params[para].min
+
+            if update_params[para].max is not None:
+                initial_params[para].max = update_params[para].max
+
+            if update_params[para].vary is not None:
+                initial_params[para].vary = update_params[para].vary
+
+            if update_params[para].expr is not None:
+                initial_params[para].expr = update_params[para].expr
+
+            if update_params[para].value is not None:
+
+                # Adapt the limits to the value:
+                if (initial_params[para].min is not None) and (initial_params[para].min > update_params[para].value):
+                   initial_params[para].min = update_params[para].value
+
+                if (initial_params[para].max is not None) and (initial_params[para].max < update_params[para].value):
+                   initial_params[para].max = update_params[para].value
+
+                initial_params[para].value = update_params[para].value
+
+    # Check the case for an OrderedDict or dict parameter:
+    elif type(update_params) == OrderedDict or type(update_params) == dict:
+
+        for para in update_params:
+            if para not in initial_params:
+                initial_params.add(para)
+            if 'min' in update_params[para]:
+                initial_params[para].min = update_params[para]['min']
+
+            if 'max' in update_params[para]:
+                initial_params[para].max = update_params[para]['max']
+
+            if 'vary' in update_params[para]:
+                initial_params[para].vary = update_params[para]['vary']
+
+            if 'expr' in update_params[para]:
+                initial_params[para].expr = update_params[para]['expr']
+
+            if 'value' in update_params[para]:
+
+                # Adapt the limits to the value:
+                if (initial_params[para].min is not None) and (initial_params[para].min > update_params[para]['value']):
+                    initial_params[para].min = update_params[para]['value']
+
+                if (initial_params[para].max is not None) and (initial_params[para].max < update_params[para]['value']):
+                    initial_params[para].max = update_params[para]['value']
+
+                initial_params[para].value = update_params[para]['value']
+
+    else:
+        self.log.error('The type of the passed update_params object <{0}> is '
+                     'neither of type lmfit.parameter.Parameters, '
+                     'OrderedDict or dict! Correct that, the initial_params'
+                     'will be returned.'.format(type(update_params)))
+
+    return initial_params
+
+def create_fit_string(self, result, model, units=None, decimal_digits_value_given=None,
+                      decimal_digits_err_given=None):
+    """ This method can produces a well readable string from the results of a fitted model.
+    If units is not given or one unit missing there will be no unit in string.
+    If decimal_digits_value_given is not provided it will be set to precision of error and digits
+    of error will be set to 1.
+
+    @param lmfit object result: the fitting result
+    @param lmfit object model: the corresponding model
+    @param dict units: units for parameters of model if not given all units are set to "arb. u."
+    @param int decimal_digits_err_given: (optional) number of decimals displayed in output for error
+    @param int decimal_digits_value_given: (optional) number of decimals displayed in output for value
+
+    @return str fit_result: readable string
+    """
+    if units is None:
+        units = dict()
+    # TODO: Add multiplicator
+    # TODO: Add decimal dict
+    # TODO: Add sensible output such that e only multiple of 3 and err and value have same exponent
+
+    fit_result = ''
+    for variable in model.param_names:
+        # check order of number
+        exponent_error = int("{:e}".format(result.params[variable].stderr)[-3:])
+        exponent_value = int("{:e}".format(result.params[variable].value)[-3:])
+        if decimal_digits_value_given is None:
+            decimal_digits_value = int(exponent_value-exponent_error+1)
+            if decimal_digits_value <= 0:
+                decimal_digits_value = 1
+        if decimal_digits_err_given is None:
+            decimal_digits_err = 1
+            if decimal_digits_err <= 0:
+                decimal_digits_err = 1
+        try:
+            fit_result += ("{0} [{1}] : {2} ± {3}\n".format(str(variable),
+                                                            units[variable],
+                                                            "{0:.{1}e}".format(
+                                                                float(result.params[variable].value),
+                                                                decimal_digits_value),
+                                                            "{0:.{1}e}".format(
+                                                                float(result.params[variable].stderr),
+                                                                decimal_digits_err)))
+        except:
+            # self.log.warning('No unit given for parameter {}, setting unit '
+            #             'to empty string'.format(variable))
+            fit_result += ("{0} [{1}] : {2} ± {3}\n".format(str(variable),
+                                                            "arb. u.",
+                                                            "{0:.{1}e}".format(
+                                                                float(result.params[variable].value),
+                                                                decimal_digits_value),
+                                                            "{0:.{1}e}".format(
+                                                                float(result.params[variable].stderr),
+                                                                decimal_digits_err)))
+    return fit_result
+
+
+def _search_end_of_dip(self, direction, data, peak_arg, start_arg, end_arg, sigma_threshold, minimal_threshold, make_prints):
+    """
+    data has to be offset leveled such that offset is substracted
+    """
+    # Todo: Create doc string
+    absolute_min  = data[peak_arg]
+
+    if direction == 'left':
+        mult = -1
+        sigma_arg=start_arg
+    elif direction == 'right':
+        mult = +1
+        sigma_arg=end_arg
+    else:
+        print('No valid direction in search end of peak')
+    ii=0
+
+    #if the minimum is at the end set this as boarder
+    if (peak_arg != start_arg and direction=='left' or
+        peak_arg != end_arg   and direction=='right'):
+        while True:
+            # if no minimum can be found decrease threshold
+            if ((peak_arg-ii<start_arg and direction == 'left') or
+                (peak_arg+ii>end_arg   and direction=='right')):
+                sigma_threshold*=0.9
+                ii=0
+                if make_prints:
+                    print('h1 sigma_threshold',sigma_threshold)
+
+            #if the dip is always over threshold the end is as
+            # set before
+            if abs(sigma_threshold/absolute_min)<abs(minimal_threshold):
+                if make_prints:
+                    print('h2')
+                break
+
+             #check if value was changed and search is finished
+            if ((sigma_arg == start_arg and direction == 'left') or
+                (sigma_arg == end_arg   and direction=='right')):
+                # check if if value is lower as threshold this is the
+                # searched value
+                if make_prints:
+                    print('h3')
+                if abs(data[peak_arg+(mult*ii)])<abs(sigma_threshold):
+                    # value lower than threshold found - left end found
+                    sigma_arg=peak_arg+(mult*ii)
+                    if make_prints:
+                        print('h4')
+                    break
+            ii+=1
+
+    # in this case the value is the last index and should be search set
+    # as right argument
+    else:
+        if make_prints:
+            print('neu h10')
+        sigma_arg=peak_arg
+
+    return sigma_threshold,sigma_arg
+
+
+def _search_double_dip(self, x_axis, data, threshold_fraction=0.3,
+                       minimal_threshold=0.01, sigma_threshold_fraction=0.3,
+                       make_prints=False):
+    """ This method searches for a double dip. There are three values which can be set in order to adjust
+    the search. A threshold which defines when  a minimum is a dip,
+    this threshold is then lowered if no dip can be found until the
+    minimal threshold which sets the absolute boarder and a
+    sigma_threshold_fraction which defines when the
+
+    @param array x_axis: x values
+    @param array data: value of each data point corresponding to
+                        x values
+    @param float threshold_fraction: x values
+    @param float minimal_threshold: x values
+    @param float sigma_threshold_fraction: x values
+
+
+    @return int error: error code (0:OK, -1:error)
+    @return int sigma0_argleft: index of left side of 1st peak
+    @return int dip0_arg: index of max of 1st peak
+    @return int sigma0_argright: index of right side of 1st peak
+    @return int sigma1_argleft: index of left side of 2nd peak
+    @return int dip1_arg: index of max side of 2nd peak
+    @return int sigma1_argright: index of right side of 2nd peak
+    """
+
+    if sigma_threshold_fraction is None:
+        sigma_threshold_fraction=threshold_fraction
+
+    error=0
+
+    #first search for absolute minimum
+    absolute_min=data.min()
+    absolute_argmin=data.argmin()
+
+    #adjust thresholds
+    threshold=threshold_fraction*absolute_min
+    sigma_threshold=sigma_threshold_fraction*absolute_min
+
+    dip0_arg = absolute_argmin
+
+    # ====== search for the left end of the dip ======
+
+    sigma_threshold, sigma0_argleft = self._search_end_of_dip(
+                             direction='left',
+                             data=data,
+                             peak_arg = absolute_argmin,
+                             start_arg = 0,
+                             end_arg = len(data)-1,
+                             sigma_threshold = sigma_threshold,
+                             minimal_threshold = minimal_threshold,
+                             make_prints= make_prints)
+
+    if make_prints:
+        print('Left sigma of main peak: ',x_axis[sigma0_argleft])
+
+    # ====== search for the right end of the dip ======
+    # reset sigma_threshold
+
+    sigma_threshold, sigma0_argright = self._search_end_of_dip(
+                             direction='right',
+                             data=data,
+                             peak_arg = absolute_argmin,
+                             start_arg = 0,
+                             end_arg = len(data)-1,
+                             sigma_threshold = sigma_threshold_fraction*absolute_min,
+                             minimal_threshold = minimal_threshold,
+                             make_prints= make_prints)
+
+    if make_prints:
+        print('Right sigma of main peak: ',x_axis[sigma0_argright])
+
+    # ======== search for second lorentzian dip ========
+    left_index=int(0)
+    right_index=len(x_axis)-1
+
+    mid_index_left=sigma0_argleft
+    mid_index_right=sigma0_argright
+
+    # if main first dip covers the whole left side search on the right
+    # side only
+    if mid_index_left==left_index:
+        if make_prints:
+            print('h11', left_index,mid_index_left,mid_index_right,right_index)
+        #if one dip is within the second they have to be set to one
+        if mid_index_right==right_index:
+            dip1_arg=dip0_arg
+        else:
+            dip1_arg=data[mid_index_right:right_index].argmin()+mid_index_right
+
+    #if main first dip covers the whole right side search on the left
+    # side only
+    elif mid_index_right==right_index:
+        if make_prints:
+            print('h12')
+        #if one dip is within the second they have to be set to one
+        if mid_index_left==left_index:
+            dip1_arg=dip0_arg
+        else:
+            dip1_arg=data[left_index:mid_index_left].argmin()
+
+    # search for peak left and right of the dip
+    else:
+        while True:
+            #set search area excluding the first dip
+            left_min=data[left_index:mid_index_left].min()
+            left_argmin=data[left_index:mid_index_left].argmin()
+            right_min=data[mid_index_right:right_index].min()
+            right_argmin=data[mid_index_right:right_index].argmin()
+
+            if abs(left_min) > abs(threshold) and \
+               abs(left_min) > abs(right_min):
+                if make_prints:
+                    print('h13')
+                # there is a minimum on the left side which is higher
+                # than the minimum on the right side
+                dip1_arg = left_argmin+left_index
+                break
+            elif abs(right_min)>abs(threshold):
+                # there is a minimum on the right side which is higher
+                # than on left side
+                dip1_arg=right_argmin+mid_index_right
+                if make_prints:
+                    print('h14')
+                break
+            else:
+                # no minimum at all over threshold so lowering threshold
+                #  and resetting search area
+                threshold*=0.9
+                left_index=int(0)
+                right_index=len(x_axis)-1
+                mid_index_left=sigma0_argleft
+                mid_index_right=sigma0_argright
+                if make_prints:
+                    print('h15')
+                #if no second dip can be found set both to same value
+                if abs(threshold/absolute_min)<abs(minimal_threshold):
+                    if make_prints:
+                        print('h16')
+                    self.log.warning('Threshold to minimum ratio was too '
+                            'small to estimate two minima. So both '
+                            'are set to the same value')
+                    error=-1
+                    dip1_arg=dip0_arg
+                    break
+
+    # if the dip is exactly at one of the boarders that means
+    # the dips are most probably overlapping
+    if dip1_arg in (sigma0_argleft, sigma0_argright):
+        #print('Dips are overlapping')
+        distance_left  = abs(dip0_arg - sigma0_argleft)
+        distance_right = abs(dip0_arg - sigma0_argright)
+        sigma1_argleft = sigma0_argleft
+        sigma1_argright = sigma0_argright
+        if distance_left > distance_right:
+            dip1_arg = dip0_arg - abs(distance_left-distance_right)
+        elif distance_left < distance_right:
+            dip1_arg = dip0_arg + abs(distance_left-distance_right)
+        else:
+            dip1_arg = dip0_arg
+        #print(distance_left,distance_right,dip1_arg)
+    else:
+        # if the peaks are not overlapping search for left and right
+        # boarder of the dip
+
+        # ====== search for the right end of the dip ======
+        sigma_threshold, sigma1_argleft = self._search_end_of_dip(
+                                 direction='left',
+                                 data=data,
+                                 peak_arg = dip1_arg,
+                                 start_arg = 0,
+                                 end_arg = len(data)-1,
+                                 sigma_threshold = sigma_threshold_fraction*absolute_min,
+                                 minimal_threshold = minimal_threshold,
+                                 make_prints= make_prints)
+
+        # ====== search for the right end of the dip ======
+        sigma_threshold, sigma1_argright = self._search_end_of_dip(
+                                 direction='right',
+                                 data=data,
+                                 peak_arg = dip1_arg,
+                                 start_arg = 0,
+                                 end_arg = len(data)-1,
+                                 sigma_threshold = sigma_threshold_fraction*absolute_min,
+                                 minimal_threshold = minimal_threshold,
+                                 make_prints= make_prints)
+
+    return error, sigma0_argleft, dip0_arg, sigma0_argright, sigma1_argleft, dip1_arg, sigma1_argright
+
+
+############################################################################
+#                                                                          #
+#             Additional routines with Lorentzian-like filter              #
+#                                                                          #
+############################################################################
+
+def find_offset_parameter(self, x_values=None, data=None):
+    """ This method convolves the data with a Lorentzian and the finds the
+    offset which is supposed to be the most likely valy via a histogram.
+    Additional the smoothed data is returned
+
+    @param array x_values: x values
+    @param array data: value of each data point corresponding to
+                        x values
+
+    @return int error: error code (0:OK, -1:error)
+    @return float array data_smooth: smoothed data
+    @return float offset: estimated offset
+
+
+    """
+    # lorentzian filter
+    mod, params = self.make_lorentzian_model()
+
+    # Todo: exclude filter in seperate method to be used in other methods
+
+    if len(x_values) < 20.:
+        len_x = 5
+    elif len(x_values) >= 100.:
+        len_x = 10
+    else:
+        len_x = int(len(x_values)/10.)+1
+
+    lorentz = mod.eval(x=np.linspace(0, len_x, len_x), amplitude=1, offset=0.,
+                       sigma=len_x / 4., center=len_x / 2.)
+    data_smooth = convolve1d(data, lorentz / lorentz.sum(),
+                             mode='constant', cval=data.max())
+
+    # finding most frequent value which is supposed to be the offset
+    hist = np.histogram(data_smooth, bins=10)
+    offset = (hist[1][hist[0].argmax()]+hist[1][hist[0].argmax()+1])/2.
+
+    return data_smooth, offset
+
+############################################################################
+#                                                                          #
+#             Additional routines with gaussian-like filter              #
+#                                                                          #
+############################################################################
+
+def gaussian_smoothing(self, data=None, filter_len=None, filter_sigma=None):
+    """ This method convolves the data with a gaussian
+     the smoothed data is returned
+
+    @param array data: raw data
+    @param int filter_len: length of filter
+    @param int filter_sigma: width of gaussian
+
+    @return array: smoothed data
+
+    """
+    #Todo: Check for wrong data type
+    if filter_len is None:
+        if len(data) < 20.:
+            filter_len = 5
+        elif len(data) >= 100.:
+            filter_len = 10
+        else:
+            filter_len = int(len(data) / 10.) + 1
+    if filter_sigma is None:
+        filter_sigma = filter_len
+
+    gaus = gaussian(filter_len, filter_sigma)
+    return convolve1d(data, gaus / gaus.sum(), mode='mirror')
+
+
+
+def _check_1D_input(self, x_axis, data, params):
+    """ Helper function to check the input of the fit for general consistency.
+
+    @param numpy.array x_axis: x values
+    @param numpy.array data: value of each data point corresponding to x values
+    @param lmfit.Parameters params: a parameter object which will be filled with
+                                    initial values for the fit
+
+    @return int: error code (0:OK, -1:error)
+    """
+
+    error = 0
+    parameters = [x_axis, data]
+    for var in parameters:
+        if not isinstance(var, (frozenset, list, set, tuple, np.ndarray)):
+            self.log.error('Given parameter is no array.')
+            error = -1
+        elif len(np.shape(var)) != 1:
+            self.log.error('Given parameter is no one dimensional array.')
+            error = -1
+    if not isinstance(params, Parameters):
+        self.log.error('Parameters object is not valid in estimate_gaussian.')
+        error = -1
+
+    return error
+
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/hyperbolicsaturationmethods.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains methods for hyperbolic saturation fitting, these methods
-are imported by class FitLogic.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-
-import numpy as np
-from lmfit.models import Model
-
-
-################################################################################
-#                                                                              #
-#                Hyperbolic saturation models                                  #
-#                                                                              #
-################################################################################
-
-def make_hyperbolicsaturation_model(self, prefix=None):
-    """ Create a model of the fluorescence depending on excitation power with
-        linear offset.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-    """
-
-    def hyperbolicsaturation_function(x, I_sat, P_sat):
-        """ Fluorescence depending excitation power function
-
-        @param numpy.array x: 1D array as the independent variable e.g. power
-        @param float I_sat: Saturation Intensity
-        @param float P_sat: Saturation power
-
-        @return: hyperbolicsaturation function: for using it as a model
-        """
-
-        return I_sat * (x / (x + P_sat))
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                     'cannot be used as a prefix and will be ignored for now.'
-                     'Correct that!'.format(prefix, type(prefix)))
-
-        mod_sat = Model(hyperbolicsaturation_function, independent_vars=['x'])
-    else:
-        mod_sat = Model(hyperbolicsaturation_function, independent_vars=['x'],
-                        prefix=prefix)
-
-    linear_model, params = self.make_linear_model(prefix=prefix)
-    complete_model = mod_sat + linear_model
-
-    params = complete_model.make_params()
-
-    return complete_model, params
-
-
-def make_hyperbolicsaturation_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a fit on the provided data with a fluorescence depending function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-
-    mod_final, params = self.make_hyperbolicsaturation_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    # overwrite values of additional parameters
-    params = self._substitute_params(
-        initial_params=params,
-        update_params=add_params)
-
-    result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
-
-    return result
-
-
-def estimate_hyperbolicsaturation(self, x_axis, data, params):
-    """ Provides an estimation for a saturation like function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    x_axis_half = x_axis[len(x_axis)//2:]
-    data_half = data[len(x_axis)//2:]
-
-    results_lin = self.make_linear_fit(x_axis=x_axis_half, data=data_half,
-                                           estimator=self.estimate_linear)
-
-    est_slope = results_lin.params['slope'].value
-    est_offset = data.min()
-
-    data_red = data - est_slope*x_axis - est_offset
-    est_I_sat = np.mean(data_red[len(data_red)//2:])
-    est_P_sat = est_I_sat/2
-
-    params['I_sat'].value = est_I_sat
-    params['slope'].value = est_slope
-    params['offset'].value = est_offset
-    params['P_sat'].value = est_P_sat
-
-
-    return error, params
+# -*- coding: utf-8 -*-
+"""
+This file contains methods for hyperbolic saturation fitting, these methods
+are imported by class FitLogic.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+
+import numpy as np
+from lmfit.models import Model
+
+
+################################################################################
+#                                                                              #
+#                Hyperbolic saturation models                                  #
+#                                                                              #
+################################################################################
+
+def make_hyperbolicsaturation_model(self, prefix=None):
+    """ Create a model of the fluorescence depending on excitation power with
+        linear offset.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+    """
+
+    def hyperbolicsaturation_function(x, I_sat, P_sat):
+        """ Fluorescence depending excitation power function
+
+        @param numpy.array x: 1D array as the independent variable e.g. power
+        @param float I_sat: Saturation Intensity
+        @param float P_sat: Saturation power
+
+        @return: hyperbolicsaturation function: for using it as a model
+        """
+
+        return I_sat * (x / (x + P_sat))
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                     'cannot be used as a prefix and will be ignored for now.'
+                     'Correct that!'.format(prefix, type(prefix)))
+
+        mod_sat = Model(hyperbolicsaturation_function, independent_vars=['x'])
+    else:
+        mod_sat = Model(hyperbolicsaturation_function, independent_vars=['x'],
+                        prefix=prefix)
+
+    linear_model, params = self.make_linear_model(prefix=prefix)
+    complete_model = mod_sat + linear_model
+
+    params = complete_model.make_params()
+
+    return complete_model, params
+
+
+def make_hyperbolicsaturation_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a fit on the provided data with a fluorescence depending function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+
+    mod_final, params = self.make_hyperbolicsaturation_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    # overwrite values of additional parameters
+    params = self._substitute_params(
+        initial_params=params,
+        update_params=add_params)
+
+    result = mod_final.fit(data, x=x_axis, params=params, **kwargs)
+
+    return result
+
+
+def estimate_hyperbolicsaturation(self, x_axis, data, params):
+    """ Provides an estimation for a saturation like function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    x_axis_half = x_axis[len(x_axis)//2:]
+    data_half = data[len(x_axis)//2:]
+
+    results_lin = self.make_linear_fit(x_axis=x_axis_half, data=data_half,
+                                           estimator=self.estimate_linear)
+
+    est_slope = results_lin.params['slope'].value
+    est_offset = data.min()
+
+    data_red = data - est_slope*x_axis - est_offset
+    est_I_sat = np.mean(data_red[len(data_red)//2:])
+    est_P_sat = est_I_sat/2
+
+    params['I_sat'].value = est_I_sat
+    params['slope'].value = est_slope
+    params['offset'].value = est_offset
+    params['P_sat'].value = est_P_sat
+
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/linearmethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/linearmethods.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,272 +1,272 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains methods for linear fitting, these methods
-are imported by class FitLogic. The functions can be used for amy
-types of offsets or slopes in other methods.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-import numpy as np
-from lmfit.models import Model
-
-
-############################################################################
-#                                                                          #
-#                              linear fitting                              #
-#                                                                          #
-############################################################################
-
-def make_constant_model(self, prefix=None):
-    """ Create constant model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-
-    For further information have a look in:
-    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.GaussianModel
-    """
-    def constant_function(x, offset):
-        """ Function of a constant value.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. time
-        @param float offset: constant offset
-
-        @return: constant function, in order to use it as a model
-        """
-
-        return offset
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
-                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
-                                                                                    type(prefix)))
-        model = Model(constant_function, independent_vars=['x'])
-    else:
-        model = Model(constant_function, independent_vars=['x'], prefix=prefix)
-
-    params = model.make_params()
-
-    return model, params
-
-
-def make_amplitude_model(self, prefix=None):
-    """ Create a constant model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_constant_model.
-    """
-
-    def amplitude_function(x, amplitude):
-        """ Function of a constant value.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. time
-        @param float amplitude: constant offset
-
-        @return: constant function, in order to use it as a model
-        """
-
-        return amplitude
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
-                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
-                                                                                    type(prefix)))
-        model = Model(amplitude_function, independent_vars=['x'])
-    else:
-        model = Model(amplitude_function, independent_vars=['x'], prefix=prefix)
-
-    params = model.make_params()
-
-    return model, params
-
-
-def make_slope_model(self, prefix=None):
-    """ Create a slope model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_constant_model.
-    """
-
-    def slope_function(x, slope):
-        """ Function of a constant value.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. time
-        @param float slope: constant slope
-
-        @return: slope function, in order to use it as a model
-        """
-
-        return slope
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
-                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
-                                                                                    type(prefix)))
-        model = Model(slope_function, independent_vars=['x'])
-    else:
-        model = Model(slope_function, independent_vars=['x'], prefix=prefix)
-
-    params = model.make_params()
-
-    return model, params
-
-
-def make_linear_model(self, prefix=None):
-    """ Create linear model.
-
-    @param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_constant_model.
-    """
-
-    def linear_function(x):
-        """ Function of a linear model.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. time
-
-        @return: linear function, in order to use it as a model
-        """
-
-        return x
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
-                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
-                                                                                    type(prefix)))
-        linear_mod = Model(linear_function, independent_vars=['x'])
-    else:
-        linear_mod = Model(linear_function, independent_vars=['x'], prefix=prefix)
-
-    slope, slope_param = self.make_slope_model(prefix=prefix)
-    constant, constant_param = self.make_constant_model(prefix=prefix)
-
-    model = slope * linear_mod + constant
-    params = model.make_params()
-
-    return model, params
-
-
-def make_linear_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Performe a linear fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    # Make mathematical fit model
-    linear, params = self.make_linear_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params, update_params=add_params)
-
-    result = linear.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()
-
-    result_str_dict['Slope'] = {'value': result.params['slope'].value,
-                                'error': result.params['slope'].stderr,
-                                'unit': '{0}/{1}'.format(units[1], units[0])}
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_linear(self, x_axis, data, params):
-    """ Provide an estimation for the initial values of a linear function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    try:
-        # calculate the parameters using Least-squares estimation of linear
-        # regression
-        a_1 = 0
-        a_2 = 0
-        x_mean = x_axis.mean()
-        data_mean = data.mean()
-
-        for i in range(0, len(x_axis)):
-            a_1 += (x_axis[i]-x_mean)*(data[i]-data_mean)
-            a_2 += np.power(x_axis[i]-x_mean, 2)
-        slope = a_1/a_2
-        intercept = data_mean - slope * x_mean
-        params['offset'].value = intercept
-        params['slope'].value = slope
-    except:
-        self.log.warning('The estimation for linear fit did not work.')
-        params['slope'].value = 0
-        params['offset'].value = 0
-
-    return error, params
-
+# -*- coding: utf-8 -*-
+"""
+This file contains methods for linear fitting, these methods
+are imported by class FitLogic. The functions can be used for amy
+types of offsets or slopes in other methods.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+import numpy as np
+from lmfit.models import Model
+
+
+############################################################################
+#                                                                          #
+#                              linear fitting                              #
+#                                                                          #
+############################################################################
+
+def make_constant_model(self, prefix=None):
+    """ Create constant model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+
+    For further information have a look in:
+    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.GaussianModel
+    """
+    def constant_function(x, offset):
+        """ Function of a constant value.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. time
+        @param float offset: constant offset
+
+        @return: constant function, in order to use it as a model
+        """
+
+        return offset
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
+                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
+                                                                                    type(prefix)))
+        model = Model(constant_function, independent_vars=['x'])
+    else:
+        model = Model(constant_function, independent_vars=['x'], prefix=prefix)
+
+    params = model.make_params()
+
+    return model, params
+
+
+def make_amplitude_model(self, prefix=None):
+    """ Create a constant model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_constant_model.
+    """
+
+    def amplitude_function(x, amplitude):
+        """ Function of a constant value.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. time
+        @param float amplitude: constant offset
+
+        @return: constant function, in order to use it as a model
+        """
+
+        return amplitude
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
+                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
+                                                                                    type(prefix)))
+        model = Model(amplitude_function, independent_vars=['x'])
+    else:
+        model = Model(amplitude_function, independent_vars=['x'], prefix=prefix)
+
+    params = model.make_params()
+
+    return model, params
+
+
+def make_slope_model(self, prefix=None):
+    """ Create a slope model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_constant_model.
+    """
+
+    def slope_function(x, slope):
+        """ Function of a constant value.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. time
+        @param float slope: constant slope
+
+        @return: slope function, in order to use it as a model
+        """
+
+        return slope
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
+                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
+                                                                                    type(prefix)))
+        model = Model(slope_function, independent_vars=['x'])
+    else:
+        model = Model(slope_function, independent_vars=['x'], prefix=prefix)
+
+    params = model.make_params()
+
+    return model, params
+
+
+def make_linear_model(self, prefix=None):
+    """ Create linear model.
+
+    @param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_constant_model.
+    """
+
+    def linear_function(x):
+        """ Function of a linear model.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. time
+
+        @return: linear function, in order to use it as a model
+        """
+
+        return x
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and cannot be used as '
+                       'a prefix and will be ignored for now. Correct that!'.format(prefix,
+                                                                                    type(prefix)))
+        linear_mod = Model(linear_function, independent_vars=['x'])
+    else:
+        linear_mod = Model(linear_function, independent_vars=['x'], prefix=prefix)
+
+    slope, slope_param = self.make_slope_model(prefix=prefix)
+    constant, constant_param = self.make_constant_model(prefix=prefix)
+
+    model = slope * linear_mod + constant
+    params = model.make_params()
+
+    return model, params
+
+
+def make_linear_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Performe a linear fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    # Make mathematical fit model
+    linear, params = self.make_linear_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params, update_params=add_params)
+
+    result = linear.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()
+
+    result_str_dict['Slope'] = {'value': result.params['slope'].value,
+                                'error': result.params['slope'].stderr,
+                                'unit': '{0}/{1}'.format(units[1], units[0])}
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_linear(self, x_axis, data, params):
+    """ Provide an estimation for the initial values of a linear function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    try:
+        # calculate the parameters using Least-squares estimation of linear
+        # regression
+        a_1 = 0
+        a_2 = 0
+        x_mean = x_axis.mean()
+        data_mean = data.mean()
+
+        for i in range(0, len(x_axis)):
+            a_1 += (x_axis[i]-x_mean)*(data[i]-data_mean)
+            a_2 += np.power(x_axis[i]-x_mean, 2)
+        slope = a_1/a_2
+        intercept = data_mean - slope * x_mean
+        params['offset'].value = intercept
+        params['slope'].value = slope
+    except:
+        self.log.warning('The estimation for linear fit did not work.')
+        params['slope'].value = 0
+        params['offset'].value = 0
+
+    return error, params
+
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/lorentzianlikemethods.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,957 +1,957 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains methods for lorentzian-like fitting, these methods
-are imported by class FitLogic.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Developed from PI3diamond code Copyright (C) 2009 Helmut Rathgen <helmut.rathgen@gmail.com>
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-
-from collections import OrderedDict
-
-import numpy as np
-from lmfit import Parameters
-from lmfit.models import Model
-from scipy.interpolate import InterpolatedUnivariateSpline
-from scipy.ndimage import filters
-
-################################################################################
-#                                                                              #
-#                       Defining Lorentzian Models                             #
-#                                                                              #
-################################################################################
-
-
-"""
-Information about the general Lorentzian Model
-==============================================
-
-The lorentzian has the following general form:
-
-                                 _                       _
-                            A   |           sigma         |
-    f(x; A, x_0, sigma) = ----- |  ---------------------- |
-                            pi  |_ (x_0 - x)^2 + sigma^2 _|
-
-That is the appearance if the lorentzian is considered as a probability
-distribution. Then it is also called a Cauchy distribution. For physical
-applications it is sensible to redefine the Lorentzian like that:
-
-                 !      A
-    f(x=x_0) = I = -----------
-                    pi * sigma
-
-
-                                 _                            _
-                                |         (sigma)^2          |
-    L(x; I, x_0, sigma) =   I * |  --------------------------  |
-                                |_ (x_0 - x)^2 + (sigma)^2  _|
-
-We will call this notation the physical definition of the Lorentzian, with I as
-the height of the Lorentzian, x_0 is its location and sigma as the half
-width at half maximum (HWHM).
-
-Note that the fitting algorithm is using now the equation L(x; I, x_0, sigma)
-and not f(x; A, x_0, sigma), therefore all the parameters are defined according
-to L(x; I, x_0, sigma). The full width at half maximum (FWHM) is therefore
-2*sigma.
-
-The indefinite Integral of the Lorentzian is
-
-    integral(f(x),x) = A/pi *Arctan( (x-x0)/sigma)
-
-Plugging in the limits [0 to inf] we get:
-
-    integral(f(x), {x,0,inf}) = (A * sigma/pi) *(  pi/(2*sigma) + Arctan(x_0/sigma)/sigma) ) = F
-
-(You can confirm that with Mathematica.) For the assumption that
-
-    x_0 >> sigma
-
-we can take the limit of Arctan to which it converges: pi/2
-
-That simplifies the formula further to
-
-F = (A * sigma/pi) * (  pi/(2*sigma) + pi/(2*sigma) ) = A
-
-Using the formula for I (above) we can solve the equation for sigma:
-
-sigma = A / (pi* I) = F /(pi * I)
-
-The parameter I can be really easy determined, since it will be just the
-maximal/minimal value of the Lorentzian. If the area F is calculated
-numerically, then the parameter sigma can be estimated.
-
-"""
-
-####################################
-# Lorentzian model                 #
-####################################
-
-def make_lorentzianwithoutoffset_model(self, prefix=None):
-    """ Create a model of a bare physical Lorentzian with an amplitude.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-
-        For further information have a look in:
-    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.LorentzianModel
-    """
-
-    def physical_lorentzian(x, center, sigma):
-        """ Function of a Lorentzian with unit height at center.
-
-        @param numpy.array x: independent variable - e.g. frequency
-        @param float center: center around which the distributions will be
-        @param float sigma: half length at half maximum
-
-        @return: numpy.array with length equals to input x and with the values
-                 of a lorentzian.
-        """
-        return np.power(sigma, 2) / (np.power((center - x), 2) + np.power(sigma, 2))
-
-    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error(
-            'The passed prefix <{0}> of type {1} is not a string and'
-            'cannot be used as a prefix and will be ignored for now.'
-            'Correct that!'.format(prefix, type(prefix)))
-        lorentz_model = Model(physical_lorentzian, independent_vars=['x'])
-    else:
-        lorentz_model = Model(
-            physical_lorentzian,
-            independent_vars=['x'],
-            prefix=prefix)
-
-    full_lorentz_model = amplitude_model * lorentz_model
-    params = full_lorentz_model.make_params()
-
-    # introduces a new parameter, which is solely depending on others and which
-    # will be not optimized:
-    if prefix is None:
-        prefix = ''
-    full_lorentz_model.set_param_hint(
-        '{0!s}fwhm'.format(prefix),
-        expr="2*{0!s}sigma".format(prefix))
-    # full_lorentz_model.set_param_hint('{0}contrast'.format(prefix),
-    #                                   expr='(-100.0)')
-                                      # expr='({0!s}amplitude/offset)*100'.format(prefix))
-    # params.add('{0}contrast'.format(prefix), expr='({0!s}amplitude/offset)*100'.format(prefix))
-
-    return full_lorentz_model, params
-
-
-####################################
-# Lorentzian model with offset     #
-####################################
-
-
-def make_lorentzian_model(self, prefix=None):
-    """ Create a Lorentz model with amplitude and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_lorentzian_model.
-    """
-
-    lorentz_model, params = self.make_lorentzianwithoutoffset_model(prefix=prefix)
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    lorentz_offset_model = lorentz_model + constant_model
-
-    if prefix is None:
-        prefix = ''
-
-    lorentz_offset_model.set_param_hint('{0}contrast'.format(prefix),
-                                        expr='({0}amplitude/offset)*100'.format(prefix))
-
-    params = lorentz_offset_model.make_params()
-
-    return lorentz_offset_model, params
-
-
-#################################################
-#    Mulitiple Lorentzian model with offset     #
-#################################################
-
-def make_multiplelorentzian_model(self, no_of_functions=1):
-    """ Create a model with multiple lorentzians with offset.
-
-    @param no_of_functions: for default=1 there is one lorentzian, else
-                            more functions are added
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_lorentzian_model.
-    """
-
-    if no_of_functions == 1:
-        multi_lorentz_model, params = self.make_lorentzian_model()
-    else:
-        prefix = 'l0_'
-        multi_lorentz_model, params = self.make_lorentzianwithoutoffset_model(prefix=prefix)
-
-        constant_model, params = self.make_constant_model()
-        multi_lorentz_model = multi_lorentz_model + constant_model
-
-        multi_lorentz_model.set_param_hint(
-            '{0}contrast'.format(prefix),
-            expr='({0}amplitude/offset)*100'.format(prefix))
-
-
-        for ii in range(1, no_of_functions):
-            prefix = 'l{0:d}_'.format(ii)
-            multi_lorentz_model += self.make_lorentzianwithoutoffset_model(prefix=prefix)[0]
-            multi_lorentz_model.set_param_hint(
-                '{0}contrast'.format(prefix),
-                expr='({0}amplitude/offset)*100'.format(prefix))
-
-    params = multi_lorentz_model.make_params()
-
-    return multi_lorentz_model, params
-
-#################################################
-#    Double Lorentzian model with offset        #
-#################################################
-
-def make_lorentziandouble_model(self):
-    """ Create a model with double lorentzian with offset.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_lorentzian_model.
-    """
-
-    return self.make_multiplelorentzian_model(no_of_functions=2)
-
-#################################################
-#       Triple Lorentzian model with offset     #
-#################################################
-
-def make_lorentziantriple_model(self):
-    """ Create a model with triple lorentzian with offset.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_lorentzian_model.
-    """
-
-    return self.make_multiplelorentzian_model(no_of_functions=3)
-
-################################################################################
-#                                                                              #
-#                    Fit functions and their estimators                        #
-#                                                                              #
-################################################################################
-
-################################################################################
-#                 Single Lorentzian with offset fitting                        #
-################################################################################
-
-def make_lorentzian_fit(self, x_axis, data, estimator, units=None,
-                        add_params=None, **kwargs):
-    """ Perform a 1D lorentzian fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-
-    model, params = self.make_lorentzian_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.warning('The 1D lorentzian fit did not work. Error '
-                         'message: {0}\n'.format(result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-
-    if units is None:
-        units = ["arb. units"]
-
-    result_str_dict['Position'] = {'value': result.params['center'].value,
-                                   'error': result.params['center'].stderr,
-                                   'unit': units[0]}
-
-    result_str_dict['Contrast'] = {'value': abs(result.params['contrast'].value),
-                                   'error': result.params['contrast'].stderr,
-                                   'unit': '%'}
-
-    result_str_dict['FWHM'] = {'value': result.params['fwhm'].value,
-                               'error': result.params['fwhm'].stderr,
-                               'unit': units[0]}
-
-    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-def estimate_lorentzian_dip(self, x_axis, data, params):
-    """ Provides an estimator to obtain initial values for lorentzian function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-    # check if parameters make sense
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # check if input x-axis is ordered and increasing
-    sorted_indices = np.argsort(x_axis)
-    if not np.all(sorted_indices == np.arange(len(x_axis))):
-        x_axis = x_axis[sorted_indices]
-        data = data[sorted_indices]
-
-    data_smooth, offset = self.find_offset_parameter(x_axis, data)
-
-    # data_level = data-offset
-    data_level = data_smooth - offset
-
-    # calculate from the leveled data the amplitude:
-    amplitude = data_level.min()
-
-    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
-    fit_function = InterpolatedUnivariateSpline(x_axis, data_level,
-                                            k=smoothing_spline)
-    numerical_integral = fit_function.integral(x_axis[0], x_axis[-1])
-
-    x_zero = x_axis[np.argmin(data_smooth)]
-
-    # according to the derived formula, calculate sigma. The crucial part is
-    # here that the offset was estimated correctly, then the area under the
-    # curve is calculated correctly:
-    sigma = np.abs(numerical_integral / (np.pi * amplitude))
-
-    # auxiliary variables
-    stepsize = x_axis[1] - x_axis[0]
-    n_steps = len(x_axis)
-
-    params['amplitude'].set(value=amplitude, max=-1e-12)
-    params['sigma'].set(value=sigma, min=stepsize / 2,
-                        max=(x_axis[-1] - x_axis[0]) * 10)
-    params['center'].set(value=x_zero, min=(x_axis[0]) - n_steps * stepsize,
-                         max=(x_axis[-1]) + n_steps * stepsize)
-    params['offset'].set(value=offset)
-
-    return error, params
-
-def estimate_lorentzian_peak (self, x_axis, data, params):
-    """ Provides a lorentzian offset peak estimator.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    # check if parameters make sense
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # the peak and dip lorentzians have the same parameters:
-    params_dip = params
-    data_negative = data * (-1)
-
-    error, params_ret = self.estimate_lorentzian_dip(
-        x_axis,
-        data_negative,
-        params_dip)
-
-    params['sigma'] = params_ret['sigma']
-    params['offset'].set(value=-params_ret['offset'])
-    # set the maximum to infinity, since that is the default value.
-    params['amplitude'].set(
-        value=-params_ret['amplitude'].value,
-        min=-1e-12,
-        max=np.inf)
-    params['center'] = params_ret['center']
-
-    return error, params
-
-
-################################################################################
-#                   Double Lorentzian with offset fitting                      #
-################################################################################
-
-def make_lorentziandouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a 1D double lorentzian dip fit with offset on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-
-    """
-
-    model, params = self.make_lorentziandouble_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    # redefine values of additional parameters
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.error('The double lorentzian fit did not '
-                     'work: {0}'.format(result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-
-    if units is None:
-        units = ["arb. u."]
-
-    result_str_dict['Position 0'] = {'value': result.params['l0_center'].value,
-                                     'error': result.params['l0_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Position 1'] = {'value': result.params['l1_center'].value,
-                                     'error': result.params['l1_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Splitting'] = {'value': (result.params['l1_center'].value -
-                                              result.params['l0_center'].value),
-                                    'error': (result.params['l0_center'].stderr +
-                                              result.params['l1_center'].stderr),
-                                    'unit': units[0]}
-
-    result_str_dict['Contrast 0'] = {'value': abs(result.params['l0_contrast'].value),
-                                     'error': result.params['l0_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['Contrast 1'] = {'value': abs(result.params['l1_contrast'].value),
-                                     'error': result.params['l1_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['FWHM 0'] = {'value': result.params['l0_fwhm'].value,
-                                 'error': result.params['l0_fwhm'].stderr,
-                                 'unit': units[0]}
-
-    result_str_dict['FWHM 1'] = {'value': result.params['l1_fwhm'].value,
-                                 'error': result.params['l1_fwhm'].stderr,
-                                 'unit': units[0]}
-
-    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-def estimate_lorentziandouble_dip(self, x_axis, data, params,
-                                  threshold_fraction=0.3,
-                                  minimal_threshold=0.01,
-                                  sigma_threshold_fraction=0.3):
-    """ Provide an estimator for double lorentzian dip with offset.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # smooth with gaussian filter and find offset:
-    data_smooth, offset = self.find_offset_parameter(x_axis, data)
-
-    # level data:
-    data_level = data_smooth - offset
-
-    # search for double lorentzian dip:
-    ret_val = self._search_double_dip(x_axis, data_level, threshold_fraction,
-                                      minimal_threshold,
-                                      sigma_threshold_fraction)
-
-    error = ret_val[0]
-    sigma0_argleft, dip0_arg, sigma0_argright = ret_val[1:4]
-    sigma1_argleft, dip1_arg, sigma1_argright = ret_val[4:7]
-
-    if dip0_arg == dip1_arg:
-        lorentz0_amplitude = data_level[dip0_arg] / 2.
-        lorentz1_amplitude = lorentz0_amplitude
-    else:
-        lorentz0_amplitude = data_level[dip0_arg]
-        lorentz1_amplitude = data_level[dip1_arg]
-
-    lorentz0_center = x_axis[dip0_arg]
-    lorentz1_center = x_axis[dip1_arg]
-
-    # Both sigmas are set to the same value
-    # numerical_integral_0 = (np.sum(data_level[sigma0_argleft:sigma0_argright]) *
-    #                    (x_axis[sigma0_argright] - x_axis[sigma0_argleft]) /
-    #                     len(data_level[sigma0_argleft:sigma0_argright]))
-
-    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
-    fit_function = InterpolatedUnivariateSpline(x_axis, data_level,
-                                            k=smoothing_spline)
-    numerical_integral_0 = fit_function.integral(x_axis[sigma0_argleft],
-                                             x_axis[sigma0_argright])
-
-    lorentz0_sigma = abs(numerical_integral_0 / (np.pi * lorentz0_amplitude))
-
-    numerical_integral_1 = numerical_integral_0
-
-    lorentz1_sigma = abs(numerical_integral_1 / (np.pi * lorentz1_amplitude))
-
-    # esstimate amplitude
-    # lorentz0_amplitude = -1*abs(lorentz0_amplitude*np.pi*lorentz0_sigma)
-    # lorentz1_amplitude = -1*abs(lorentz1_amplitude*np.pi*lorentz1_sigma)
-
-    stepsize = x_axis[1] - x_axis[0]
-    full_width = x_axis[-1] - x_axis[0]
-    n_steps = len(x_axis)
-
-    if lorentz0_center < lorentz1_center:
-        params['l0_amplitude'].set(value=lorentz0_amplitude, max=-0.01)
-        params['l0_sigma'].set(value=lorentz0_sigma, min=stepsize / 2,
-                               max=full_width * 4)
-        params['l0_center'].set(value=lorentz0_center,
-                                min=(x_axis[0]) - n_steps * stepsize,
-                                max=(x_axis[-1]) + n_steps * stepsize)
-        params['l1_amplitude'].set(value=lorentz1_amplitude, max=-0.01)
-        params['l1_sigma'].set(value=lorentz1_sigma, min=stepsize / 2,
-                               max=full_width * 4)
-        params['l1_center'].set(value=lorentz1_center,
-                                min=(x_axis[0]) - n_steps * stepsize,
-                                max=(x_axis[-1]) + n_steps * stepsize)
-    else:
-        params['l0_amplitude'].set(value=lorentz1_amplitude, max=-0.01)
-        params['l0_sigma'].set(value=lorentz1_sigma, min=stepsize / 2,
-                               max=full_width * 4)
-        params['l0_center'].set(value=lorentz1_center,
-                                min=(x_axis[0]) - n_steps * stepsize,
-                                max=(x_axis[-1]) + n_steps * stepsize)
-        params['l1_amplitude'].set(value=lorentz0_amplitude, max=-0.01)
-        params['l1_sigma'].set(value=lorentz0_sigma, min=stepsize / 2,
-                               max=full_width * 4)
-        params['l1_center'].set(value=lorentz0_center,
-                                min=(x_axis[0]) - n_steps * stepsize,
-                                max=(x_axis[-1]) + n_steps * stepsize)
-
-    params['offset'].set(value=offset)
-
-    return error, params
-
-def estimate_lorentziandouble_peak(self, x_axis, data, params,
-                                   threshold_fraction=0.3,
-                                   minimal_threshold=0.01,
-                                   sigma_threshold_fraction=0.3):
-    """ Provide an estimator for double lorentzian peak with offset.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    # check if parameters make sense
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # the peak and dip lorentzians have the same parameters:
-    params_dip = params
-    data_negative = data * (-1)
-
-    error, params_ret = self.estimate_lorentziandouble_dip(x_axis,
-                                                           data_negative,
-                                                           params_dip)
-
-    params['l0_sigma'] = params_ret['l0_sigma']
-    # set the maximum to infinity, since that is the default value.
-    params['l0_amplitude'].set(value=-params_ret['l0_amplitude'].value, min=-1e-12,
-                               max=np.inf)
-    params['l0_center'] = params_ret['l0_center']
-    params['l1_amplitude'].set(value=-params_ret['l1_amplitude'].value, min=-1e-12,
-                               max=np.inf)
-    params['l1_sigma'] = params_ret['l1_sigma']
-    params['l1_center'] = params_ret['l1_center']
-
-    params['offset'].set(value=-params_ret['offset'])
-
-    return error, params
-
-
-############################################################################
-#                               N15 fitting                                #
-############################################################################
-
-def estimate_lorentziandouble_N15(self, x_axis, data, params):
-    """ Estimation of a the hyperfine interaction of a N15 nuclear spin.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-
-    Provide an estimation of all fitting parameters for fitting the
-    two equidistant lorentzian dips of the hyperfine interaction
-    of a N15 nuclear spin. Here the splitting is set as an expression,
-    if the splitting is not exactly 3.03MHz the fit will not work.
-    """
-
-    # check if parameters make sense
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    hf_splitting = 3.03 * 1e6 # Hz
-
-    # this is an estimator, for a physical application, therefore the x_axis
-    # should fulfill certain constraints:
-    length_x_scan = x_axis[-1] - x_axis[0]
-
-    if length_x_scan < hf_splitting/2 or hf_splitting > 1e9:
-        self.log.error('The N15 estimator expects an x_axis with a length in the '
-                       'range [{0},{1}]Hz, but the passed x_axis has a length of '
-                       '{2}, which is not sensible for the N15 estimator. Correct '
-                       'that!'.format(hf_splitting / 2, 1e9, length_x_scan))
-        return -1, params
-
-    data_smooth_lorentz, offset = self.find_offset_parameter(x_axis, data)
-
-    # filter should always have a length of approx linewidth 1MHz
-    points_within_1MHz = len(x_axis) / (x_axis.max() - x_axis.min()) * 1e6
-
-    # filter should have a width of 4 MHz
-    x_filter = np.linspace(0, 4 * points_within_1MHz, 4 * points_within_1MHz)
-    lorentz = np.piecewise(x_filter, [(x_filter >= 0) * (x_filter < len(x_filter) / 4),
-                                      (x_filter >= len(x_filter) / 4) * (x_filter < len(x_filter) * 3 / 4),
-                                      (x_filter >= len(x_filter) * 3 / 4)],
-                           [1, 0, 1])
-
-    # if the filter is smaller than 3 points a convolution does not make sense
-    if len(lorentz) >= 3:
-        data_convolved = filters.convolve1d(data_smooth_lorentz,
-                                            lorentz / lorentz.sum(),
-                                            mode='constant',
-                                            cval=data_smooth_lorentz.max())
-        x_axis_min = x_axis[data_convolved.argmin()] - hf_splitting / 2.
-    else:
-        x_axis_min = x_axis[data_smooth_lorentz.argmin()]
-
-    # data_level = data_smooth_lorentz - data_smooth_lorentz.max()
-    data_level = data_smooth_lorentz - offset
-
-    minimum_level = data_level.min()
-    # integral of data:
-    fit_function = InterpolatedUnivariateSpline(x_axis, data_level, k=1)
-    Integral = fit_function.integral(x_axis[0], x_axis[-1])
-
-    # assume both peaks contribute to the linewidth, so devive by 2, that makes
-    # the peaks narrower
-    sigma = abs(Integral / (np.pi * minimum_level))
-
-    amplitude = -abs(minimum_level)
-
-    minimal_sigma = x_axis[1] - x_axis[0]
-    maximal_sigma = x_axis[-1] - x_axis[0]
-
-    params['l0_amplitude'].set(value=amplitude, max=-1e-6)
-    params['l0_center'].set(value=x_axis_min)
-    params['l0_sigma'].set(value=sigma, min=minimal_sigma,
-                           max=maximal_sigma)
-    params['l1_amplitude'].set(value=params['l0_amplitude'].value,
-                               max=-1e-6)
-    params['l1_center'].set(value=params['l0_center'].value + hf_splitting,
-                            expr='l0_center+{0}'.format(hf_splitting))
-    params['l1_sigma'].set(value=params['l0_sigma'].value,
-                           min=minimal_sigma, max=maximal_sigma,
-                           expr='l0_sigma')
-    params['offset'].set(value=offset)
-
-    return error, params
-
-
-############################################################################
-#                                                                          #
-#                      Triple Lorentzian fitting                           #
-#                                                                          #
-############################################################################
-#Todo: check where code breaks
-# Old Method Names:
-# make_N14_fit
-
-def make_lorentziantriple_fit(self, x_axis, data, estimator, units=None,
-                            add_params=None, **kwargs):
-    """ Perform a triple lorentzian fit
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object model: lmfit.model.ModelFit object, all parameters
-                          provided about the fitting, like: success,
-                          initial fitting values, best fitting values, data
-                          with best fit with given axis,...
-    """
-
-    model, params = self.make_lorentziantriple_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = model.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.error('The triple lorentzian fit did not '
-                       'work: {0}'.format(result.message))
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-
-    if units is None:
-        units = ["arb. units"]
-
-    result_str_dict['Position 0'] = {'value': result.params['l0_center'].value,
-                                     'error': result.params['l0_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Position 1'] = {'value': result.params['l1_center'].value,
-                                     'error': result.params['l1_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Position 2'] = {'value': result.params['l2_center'].value,
-                                     'error': result.params['l2_center'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Contrast 0'] = {'value': abs(result.params['l0_contrast'].value),
-                                     'error': result.params['l0_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['Contrast 1'] = {'value': abs(result.params['l1_contrast'].value),
-                                     'error': result.params['l1_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['Contrast 2'] = {'value': abs(result.params['l2_contrast'].value),
-                                     'error': result.params['l2_contrast'].stderr,
-                                     'unit': '%'}
-
-    result_str_dict['FWHM 0'] = {'value': result.params['l0_sigma'].value,
-                                 'error': result.params['l0_sigma'].stderr,
-                                 'unit': units[0]}
-
-    result_str_dict['FWHM 1'] = {'value': result.params['l1_sigma'].value,
-                                 'error': result.params['l1_sigma'].stderr,
-                                 'unit': units[0]}
-
-    result_str_dict['FWHM 2'] = {'value': result.params['l2_sigma'].value,
-                                 'error': result.params['l2_sigma'].stderr,
-                                 'unit': units[0]}
-
-    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-def estimate_lorentziantriple_N14(self, x_axis, data, params):
-    """ Estimation of a the hyperfine interaction of a N14 nuclear spin.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-
-    Provide an estimation of all fitting parameters for fitting the
-    three equidistant lorentzian dips of the hyperfine interaction
-    of a N14 nuclear spin. Here the splitting is set as an expression,
-    if the splitting is not exactly 2.15MHz the fit will not work.
-
-    Note that this estimator is really specific to a physical scenario.
-    Therefore the x_axis is expected to be in SI units Hz, and the x_axis should
-    be at least half of the hyperfine interaction long (2.15MHz) but also be
-    less then 1 GHz. Otherwise the underlying estimation algorithm will not
-    work.
-    """
-
-    # check if parameters make sense
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    hf_splitting = 2.15e6 # hyperfine splitting for a N14 spin
-
-    # this is an estimator, for a physical application, therefore the x_axis
-    # should fulfill certain constraints:
-    length_x_scan = x_axis[-1] - x_axis[0]
-
-    if length_x_scan < hf_splitting/2 or hf_splitting > 1e9:
-        self.log.error('The N14 estimator expects an x_axis with a length in the '
-                     'range [{0},{1}]Hz, but the passed x_axis has a length of '
-                     '{2}, which is not sensible for the N14 estimator. Correct '
-                     'that!'.format(hf_splitting/2, 1e9, length_x_scan))
-        return -1, params
-
-    # find the offset parameter, which should be in the fit the zero level:
-    data_smooth_lorentz, offset = self.find_offset_parameter(x_axis, data)
-
-    # Create now a filter of length 5MHz, then create a step-wise function with
-    # three dips. This step-wise function will be convolved with the smoothed
-    # data, where the maximal contribution will be if the peaks are within the
-    # filter. Take that to obtain from that the accurate peak position:
-
-    # filter of one dip should always have a length of approx linewidth 1MHz
-    points_within_1MHz = len(x_axis)/(x_axis.max()-x_axis.min()) * 1e6
-
-    # filter should have a width of 5MHz
-    x_filter = np.linspace(0, 5*points_within_1MHz, 5*points_within_1MHz)
-    lorentz = np.piecewise(x_filter, [(x_filter >= 0)                   * (x_filter < len(x_filter)*1/5),
-                                      (x_filter >= len(x_filter)*1/5)   * (x_filter < len(x_filter)*2/5),
-                                      (x_filter >= len(x_filter)*2/5)   * (x_filter < len(x_filter)*3/5),
-                                      (x_filter >= len(x_filter)*3/5)   * (x_filter < len(x_filter)*4/5),
-                                      (x_filter >= len(x_filter)*4/5)],
-                           [1, 0, 1, 0, 1])
-
-    # if the filter is smaller than 5 points a convolution does not make sense
-    if len(lorentz) >= 5:
-        data_convolved = filters.convolve1d(data_smooth_lorentz,
-                                            lorentz/lorentz.sum(),
-                                            mode='constant',
-                                            cval=data_smooth_lorentz.max())
-        x_axis_min = x_axis[data_convolved.argmin()]-2.15*1e6
-    else:
-        x_axis_min = x_axis[data_smooth_lorentz.argmin()]-2.15*1e6
-
-    # level of the data, that means the offset is subtracted and the real data
-    # are present
-    data_level = data_smooth_lorentz - offset
-    minimum_level = data_level.min()
-
-    # In order to perform a smooth integral to obtain the area under the curve
-    # make an interpolation of the passed data, in case they are very sparse.
-    # That increases the accuracy of the calculated Integral.
-    # integral of data corresponds to sqrt(2) * Amplitude * Sigma
-
-    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
-    fit_function = InterpolatedUnivariateSpline(x_axis, data_level, k=smoothing_spline)
-    integrated_area = fit_function.integral(x_axis[0], x_axis[-1])
-
-    # sigma = abs(integrated_area / (minimum_level/np.pi))
-    # That is wrong, so commenting out:
-    sigma = abs(integrated_area /(np.pi * minimum_level))/3
-
-    amplitude = -1*abs(minimum_level)
-
-    # Since the total amplitude of the lorentzian is depending on sigma it makes
-    # sense to vary sigma within an interval, which is smaller than the minimal
-    # distance between two points. Then the fit algorithm will have a larger
-    # range to determine the amplitude properly. That is the main issue with the
-    # fit!
-    minimal_linewidth = (x_axis[1]-x_axis[0])/4
-    maximal_linewidth = x_axis[-1]-x_axis[0]
-
-    # The linewidth of all the lorentzians are set to be the same! that is a
-    # physical constraint for the N14 fitting.
-
-    # Fill the parameter container, with the estimated values, which should be
-    # passed to the fit algorithm:
-    params['l0_amplitude'].set(value=amplitude, max=-1e-6)
-    params['l0_center'].set(value=x_axis_min)
-    params['l0_sigma'].set(value=sigma, min=minimal_linewidth,
-                           max=maximal_linewidth)
-    params['l1_amplitude'].set(value=amplitude, max=-1e-6)
-    params['l1_center'].set(value=x_axis_min+hf_splitting,
-                            expr='l0_center+{0}'.format(hf_splitting))
-    params['l1_sigma'].set(value=sigma, min=minimal_linewidth,
-                           max=maximal_linewidth, expr='l0_sigma')
-    params['l2_amplitude'].set(value=amplitude, max=-1e-6)
-    params['l2_center'].set(value=x_axis_min+hf_splitting*2,
-                            expr='l0_center+{0}'.format(hf_splitting*2))
-    params['l2_sigma'].set(value=sigma, min=minimal_linewidth,
-                           max=maximal_linewidth, expr='l0_sigma')
-    params['offset'].set(value=offset)
-
-    return error, params
+# -*- coding: utf-8 -*-
+"""
+This file contains methods for lorentzian-like fitting, these methods
+are imported by class FitLogic.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Developed from PI3diamond code Copyright (C) 2009 Helmut Rathgen <helmut.rathgen@gmail.com>
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+
+from collections import OrderedDict
+
+import numpy as np
+from lmfit import Parameters
+from lmfit.models import Model
+from scipy.interpolate import InterpolatedUnivariateSpline
+from scipy.ndimage import filters
+
+################################################################################
+#                                                                              #
+#                       Defining Lorentzian Models                             #
+#                                                                              #
+################################################################################
+
+
+"""
+Information about the general Lorentzian Model
+==============================================
+
+The lorentzian has the following general form:
+
+                                 _                       _
+                            A   |           sigma         |
+    f(x; A, x_0, sigma) = ----- |  ---------------------- |
+                            pi  |_ (x_0 - x)^2 + sigma^2 _|
+
+That is the appearance if the lorentzian is considered as a probability
+distribution. Then it is also called a Cauchy distribution. For physical
+applications it is sensible to redefine the Lorentzian like that:
+
+                 !      A
+    f(x=x_0) = I = -----------
+                    pi * sigma
+
+
+                                 _                            _
+                                |         (sigma)^2          |
+    L(x; I, x_0, sigma) =   I * |  --------------------------  |
+                                |_ (x_0 - x)^2 + (sigma)^2  _|
+
+We will call this notation the physical definition of the Lorentzian, with I as
+the height of the Lorentzian, x_0 is its location and sigma as the half
+width at half maximum (HWHM).
+
+Note that the fitting algorithm is using now the equation L(x; I, x_0, sigma)
+and not f(x; A, x_0, sigma), therefore all the parameters are defined according
+to L(x; I, x_0, sigma). The full width at half maximum (FWHM) is therefore
+2*sigma.
+
+The indefinite Integral of the Lorentzian is
+
+    integral(f(x),x) = A/pi *Arctan( (x-x0)/sigma)
+
+Plugging in the limits [0 to inf] we get:
+
+    integral(f(x), {x,0,inf}) = (A * sigma/pi) *(  pi/(2*sigma) + Arctan(x_0/sigma)/sigma) ) = F
+
+(You can confirm that with Mathematica.) For the assumption that
+
+    x_0 >> sigma
+
+we can take the limit of Arctan to which it converges: pi/2
+
+That simplifies the formula further to
+
+F = (A * sigma/pi) * (  pi/(2*sigma) + pi/(2*sigma) ) = A
+
+Using the formula for I (above) we can solve the equation for sigma:
+
+sigma = A / (pi* I) = F /(pi * I)
+
+The parameter I can be really easy determined, since it will be just the
+maximal/minimal value of the Lorentzian. If the area F is calculated
+numerically, then the parameter sigma can be estimated.
+
+"""
+
+####################################
+# Lorentzian model                 #
+####################################
+
+def make_lorentzianwithoutoffset_model(self, prefix=None):
+    """ Create a model of a bare physical Lorentzian with an amplitude.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+
+        For further information have a look in:
+    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.LorentzianModel
+    """
+
+    def physical_lorentzian(x, center, sigma):
+        """ Function of a Lorentzian with unit height at center.
+
+        @param numpy.array x: independent variable - e.g. frequency
+        @param float center: center around which the distributions will be
+        @param float sigma: half length at half maximum
+
+        @return: numpy.array with length equals to input x and with the values
+                 of a lorentzian.
+        """
+        return np.power(sigma, 2) / (np.power((center - x), 2) + np.power(sigma, 2))
+
+    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error(
+            'The passed prefix <{0}> of type {1} is not a string and'
+            'cannot be used as a prefix and will be ignored for now.'
+            'Correct that!'.format(prefix, type(prefix)))
+        lorentz_model = Model(physical_lorentzian, independent_vars=['x'])
+    else:
+        lorentz_model = Model(
+            physical_lorentzian,
+            independent_vars=['x'],
+            prefix=prefix)
+
+    full_lorentz_model = amplitude_model * lorentz_model
+    params = full_lorentz_model.make_params()
+
+    # introduces a new parameter, which is solely depending on others and which
+    # will be not optimized:
+    if prefix is None:
+        prefix = ''
+    full_lorentz_model.set_param_hint(
+        '{0!s}fwhm'.format(prefix),
+        expr="2*{0!s}sigma".format(prefix))
+    # full_lorentz_model.set_param_hint('{0}contrast'.format(prefix),
+    #                                   expr='(-100.0)')
+                                      # expr='({0!s}amplitude/offset)*100'.format(prefix))
+    # params.add('{0}contrast'.format(prefix), expr='({0!s}amplitude/offset)*100'.format(prefix))
+
+    return full_lorentz_model, params
+
+
+####################################
+# Lorentzian model with offset     #
+####################################
+
+
+def make_lorentzian_model(self, prefix=None):
+    """ Create a Lorentz model with amplitude and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_lorentzian_model.
+    """
+
+    lorentz_model, params = self.make_lorentzianwithoutoffset_model(prefix=prefix)
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    lorentz_offset_model = lorentz_model + constant_model
+
+    if prefix is None:
+        prefix = ''
+
+    lorentz_offset_model.set_param_hint('{0}contrast'.format(prefix),
+                                        expr='({0}amplitude/offset)*100'.format(prefix))
+
+    params = lorentz_offset_model.make_params()
+
+    return lorentz_offset_model, params
+
+
+#################################################
+#    Mulitiple Lorentzian model with offset     #
+#################################################
+
+def make_multiplelorentzian_model(self, no_of_functions=1):
+    """ Create a model with multiple lorentzians with offset.
+
+    @param no_of_functions: for default=1 there is one lorentzian, else
+                            more functions are added
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_lorentzian_model.
+    """
+
+    if no_of_functions == 1:
+        multi_lorentz_model, params = self.make_lorentzian_model()
+    else:
+        prefix = 'l0_'
+        multi_lorentz_model, params = self.make_lorentzianwithoutoffset_model(prefix=prefix)
+
+        constant_model, params = self.make_constant_model()
+        multi_lorentz_model = multi_lorentz_model + constant_model
+
+        multi_lorentz_model.set_param_hint(
+            '{0}contrast'.format(prefix),
+            expr='({0}amplitude/offset)*100'.format(prefix))
+
+
+        for ii in range(1, no_of_functions):
+            prefix = 'l{0:d}_'.format(ii)
+            multi_lorentz_model += self.make_lorentzianwithoutoffset_model(prefix=prefix)[0]
+            multi_lorentz_model.set_param_hint(
+                '{0}contrast'.format(prefix),
+                expr='({0}amplitude/offset)*100'.format(prefix))
+
+    params = multi_lorentz_model.make_params()
+
+    return multi_lorentz_model, params
+
+#################################################
+#    Double Lorentzian model with offset        #
+#################################################
+
+def make_lorentziandouble_model(self):
+    """ Create a model with double lorentzian with offset.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_lorentzian_model.
+    """
+
+    return self.make_multiplelorentzian_model(no_of_functions=2)
+
+#################################################
+#       Triple Lorentzian model with offset     #
+#################################################
+
+def make_lorentziantriple_model(self):
+    """ Create a model with triple lorentzian with offset.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_lorentzian_model.
+    """
+
+    return self.make_multiplelorentzian_model(no_of_functions=3)
+
+################################################################################
+#                                                                              #
+#                    Fit functions and their estimators                        #
+#                                                                              #
+################################################################################
+
+################################################################################
+#                 Single Lorentzian with offset fitting                        #
+################################################################################
+
+def make_lorentzian_fit(self, x_axis, data, estimator, units=None,
+                        add_params=None, **kwargs):
+    """ Perform a 1D lorentzian fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+
+    model, params = self.make_lorentzian_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.warning('The 1D lorentzian fit did not work. Error '
+                         'message: {0}\n'.format(result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+
+    if units is None:
+        units = ["arb. units"]
+
+    result_str_dict['Position'] = {'value': result.params['center'].value,
+                                   'error': result.params['center'].stderr,
+                                   'unit': units[0]}
+
+    result_str_dict['Contrast'] = {'value': abs(result.params['contrast'].value),
+                                   'error': result.params['contrast'].stderr,
+                                   'unit': '%'}
+
+    result_str_dict['FWHM'] = {'value': result.params['fwhm'].value,
+                               'error': result.params['fwhm'].stderr,
+                               'unit': units[0]}
+
+    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+def estimate_lorentzian_dip(self, x_axis, data, params):
+    """ Provides an estimator to obtain initial values for lorentzian function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+    # check if parameters make sense
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # check if input x-axis is ordered and increasing
+    sorted_indices = np.argsort(x_axis)
+    if not np.all(sorted_indices == np.arange(len(x_axis))):
+        x_axis = x_axis[sorted_indices]
+        data = data[sorted_indices]
+
+    data_smooth, offset = self.find_offset_parameter(x_axis, data)
+
+    # data_level = data-offset
+    data_level = data_smooth - offset
+
+    # calculate from the leveled data the amplitude:
+    amplitude = data_level.min()
+
+    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
+    fit_function = InterpolatedUnivariateSpline(x_axis, data_level,
+                                            k=smoothing_spline)
+    numerical_integral = fit_function.integral(x_axis[0], x_axis[-1])
+
+    x_zero = x_axis[np.argmin(data_smooth)]
+
+    # according to the derived formula, calculate sigma. The crucial part is
+    # here that the offset was estimated correctly, then the area under the
+    # curve is calculated correctly:
+    sigma = np.abs(numerical_integral / (np.pi * amplitude))
+
+    # auxiliary variables
+    stepsize = x_axis[1] - x_axis[0]
+    n_steps = len(x_axis)
+
+    params['amplitude'].set(value=amplitude, max=-1e-12)
+    params['sigma'].set(value=sigma, min=stepsize / 2,
+                        max=(x_axis[-1] - x_axis[0]) * 10)
+    params['center'].set(value=x_zero, min=(x_axis[0]) - n_steps * stepsize,
+                         max=(x_axis[-1]) + n_steps * stepsize)
+    params['offset'].set(value=offset)
+
+    return error, params
+
+def estimate_lorentzian_peak (self, x_axis, data, params):
+    """ Provides a lorentzian offset peak estimator.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    # check if parameters make sense
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # the peak and dip lorentzians have the same parameters:
+    params_dip = params
+    data_negative = data * (-1)
+
+    error, params_ret = self.estimate_lorentzian_dip(
+        x_axis,
+        data_negative,
+        params_dip)
+
+    params['sigma'] = params_ret['sigma']
+    params['offset'].set(value=-params_ret['offset'])
+    # set the maximum to infinity, since that is the default value.
+    params['amplitude'].set(
+        value=-params_ret['amplitude'].value,
+        min=-1e-12,
+        max=np.inf)
+    params['center'] = params_ret['center']
+
+    return error, params
+
+
+################################################################################
+#                   Double Lorentzian with offset fitting                      #
+################################################################################
+
+def make_lorentziandouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a 1D double lorentzian dip fit with offset on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+
+    """
+
+    model, params = self.make_lorentziandouble_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    # redefine values of additional parameters
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.error('The double lorentzian fit did not '
+                     'work: {0}'.format(result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+
+    if units is None:
+        units = ["arb. u."]
+
+    result_str_dict['Position 0'] = {'value': result.params['l0_center'].value,
+                                     'error': result.params['l0_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Position 1'] = {'value': result.params['l1_center'].value,
+                                     'error': result.params['l1_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Splitting'] = {'value': (result.params['l1_center'].value -
+                                              result.params['l0_center'].value),
+                                    'error': (result.params['l0_center'].stderr +
+                                              result.params['l1_center'].stderr),
+                                    'unit': units[0]}
+
+    result_str_dict['Contrast 0'] = {'value': abs(result.params['l0_contrast'].value),
+                                     'error': result.params['l0_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['Contrast 1'] = {'value': abs(result.params['l1_contrast'].value),
+                                     'error': result.params['l1_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['FWHM 0'] = {'value': result.params['l0_fwhm'].value,
+                                 'error': result.params['l0_fwhm'].stderr,
+                                 'unit': units[0]}
+
+    result_str_dict['FWHM 1'] = {'value': result.params['l1_fwhm'].value,
+                                 'error': result.params['l1_fwhm'].stderr,
+                                 'unit': units[0]}
+
+    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+def estimate_lorentziandouble_dip(self, x_axis, data, params,
+                                  threshold_fraction=0.3,
+                                  minimal_threshold=0.01,
+                                  sigma_threshold_fraction=0.3):
+    """ Provide an estimator for double lorentzian dip with offset.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # smooth with gaussian filter and find offset:
+    data_smooth, offset = self.find_offset_parameter(x_axis, data)
+
+    # level data:
+    data_level = data_smooth - offset
+
+    # search for double lorentzian dip:
+    ret_val = self._search_double_dip(x_axis, data_level, threshold_fraction,
+                                      minimal_threshold,
+                                      sigma_threshold_fraction)
+
+    error = ret_val[0]
+    sigma0_argleft, dip0_arg, sigma0_argright = ret_val[1:4]
+    sigma1_argleft, dip1_arg, sigma1_argright = ret_val[4:7]
+
+    if dip0_arg == dip1_arg:
+        lorentz0_amplitude = data_level[dip0_arg] / 2.
+        lorentz1_amplitude = lorentz0_amplitude
+    else:
+        lorentz0_amplitude = data_level[dip0_arg]
+        lorentz1_amplitude = data_level[dip1_arg]
+
+    lorentz0_center = x_axis[dip0_arg]
+    lorentz1_center = x_axis[dip1_arg]
+
+    # Both sigmas are set to the same value
+    # numerical_integral_0 = (np.sum(data_level[sigma0_argleft:sigma0_argright]) *
+    #                    (x_axis[sigma0_argright] - x_axis[sigma0_argleft]) /
+    #                     len(data_level[sigma0_argleft:sigma0_argright]))
+
+    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
+    fit_function = InterpolatedUnivariateSpline(x_axis, data_level,
+                                            k=smoothing_spline)
+    numerical_integral_0 = fit_function.integral(x_axis[sigma0_argleft],
+                                             x_axis[sigma0_argright])
+
+    lorentz0_sigma = abs(numerical_integral_0 / (np.pi * lorentz0_amplitude))
+
+    numerical_integral_1 = numerical_integral_0
+
+    lorentz1_sigma = abs(numerical_integral_1 / (np.pi * lorentz1_amplitude))
+
+    # esstimate amplitude
+    # lorentz0_amplitude = -1*abs(lorentz0_amplitude*np.pi*lorentz0_sigma)
+    # lorentz1_amplitude = -1*abs(lorentz1_amplitude*np.pi*lorentz1_sigma)
+
+    stepsize = x_axis[1] - x_axis[0]
+    full_width = x_axis[-1] - x_axis[0]
+    n_steps = len(x_axis)
+
+    if lorentz0_center < lorentz1_center:
+        params['l0_amplitude'].set(value=lorentz0_amplitude, max=-0.01)
+        params['l0_sigma'].set(value=lorentz0_sigma, min=stepsize / 2,
+                               max=full_width * 4)
+        params['l0_center'].set(value=lorentz0_center,
+                                min=(x_axis[0]) - n_steps * stepsize,
+                                max=(x_axis[-1]) + n_steps * stepsize)
+        params['l1_amplitude'].set(value=lorentz1_amplitude, max=-0.01)
+        params['l1_sigma'].set(value=lorentz1_sigma, min=stepsize / 2,
+                               max=full_width * 4)
+        params['l1_center'].set(value=lorentz1_center,
+                                min=(x_axis[0]) - n_steps * stepsize,
+                                max=(x_axis[-1]) + n_steps * stepsize)
+    else:
+        params['l0_amplitude'].set(value=lorentz1_amplitude, max=-0.01)
+        params['l0_sigma'].set(value=lorentz1_sigma, min=stepsize / 2,
+                               max=full_width * 4)
+        params['l0_center'].set(value=lorentz1_center,
+                                min=(x_axis[0]) - n_steps * stepsize,
+                                max=(x_axis[-1]) + n_steps * stepsize)
+        params['l1_amplitude'].set(value=lorentz0_amplitude, max=-0.01)
+        params['l1_sigma'].set(value=lorentz0_sigma, min=stepsize / 2,
+                               max=full_width * 4)
+        params['l1_center'].set(value=lorentz0_center,
+                                min=(x_axis[0]) - n_steps * stepsize,
+                                max=(x_axis[-1]) + n_steps * stepsize)
+
+    params['offset'].set(value=offset)
+
+    return error, params
+
+def estimate_lorentziandouble_peak(self, x_axis, data, params,
+                                   threshold_fraction=0.3,
+                                   minimal_threshold=0.01,
+                                   sigma_threshold_fraction=0.3):
+    """ Provide an estimator for double lorentzian peak with offset.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    # check if parameters make sense
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # the peak and dip lorentzians have the same parameters:
+    params_dip = params
+    data_negative = data * (-1)
+
+    error, params_ret = self.estimate_lorentziandouble_dip(x_axis,
+                                                           data_negative,
+                                                           params_dip)
+
+    params['l0_sigma'] = params_ret['l0_sigma']
+    # set the maximum to infinity, since that is the default value.
+    params['l0_amplitude'].set(value=-params_ret['l0_amplitude'].value, min=-1e-12,
+                               max=np.inf)
+    params['l0_center'] = params_ret['l0_center']
+    params['l1_amplitude'].set(value=-params_ret['l1_amplitude'].value, min=-1e-12,
+                               max=np.inf)
+    params['l1_sigma'] = params_ret['l1_sigma']
+    params['l1_center'] = params_ret['l1_center']
+
+    params['offset'].set(value=-params_ret['offset'])
+
+    return error, params
+
+
+############################################################################
+#                               N15 fitting                                #
+############################################################################
+
+def estimate_lorentziandouble_N15(self, x_axis, data, params):
+    """ Estimation of a the hyperfine interaction of a N15 nuclear spin.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+
+    Provide an estimation of all fitting parameters for fitting the
+    two equidistant lorentzian dips of the hyperfine interaction
+    of a N15 nuclear spin. Here the splitting is set as an expression,
+    if the splitting is not exactly 3.03MHz the fit will not work.
+    """
+
+    # check if parameters make sense
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    hf_splitting = 3.03 * 1e6 # Hz
+
+    # this is an estimator, for a physical application, therefore the x_axis
+    # should fulfill certain constraints:
+    length_x_scan = x_axis[-1] - x_axis[0]
+
+    if length_x_scan < hf_splitting/2 or hf_splitting > 1e9:
+        self.log.error('The N15 estimator expects an x_axis with a length in the '
+                       'range [{0},{1}]Hz, but the passed x_axis has a length of '
+                       '{2}, which is not sensible for the N15 estimator. Correct '
+                       'that!'.format(hf_splitting / 2, 1e9, length_x_scan))
+        return -1, params
+
+    data_smooth_lorentz, offset = self.find_offset_parameter(x_axis, data)
+
+    # filter should always have a length of approx linewidth 1MHz
+    points_within_1MHz = len(x_axis) / (x_axis.max() - x_axis.min()) * 1e6
+
+    # filter should have a width of 4 MHz
+    x_filter = np.linspace(0, 4 * points_within_1MHz, 4 * points_within_1MHz)
+    lorentz = np.piecewise(x_filter, [(x_filter >= 0) * (x_filter < len(x_filter) / 4),
+                                      (x_filter >= len(x_filter) / 4) * (x_filter < len(x_filter) * 3 / 4),
+                                      (x_filter >= len(x_filter) * 3 / 4)],
+                           [1, 0, 1])
+
+    # if the filter is smaller than 3 points a convolution does not make sense
+    if len(lorentz) >= 3:
+        data_convolved = filters.convolve1d(data_smooth_lorentz,
+                                            lorentz / lorentz.sum(),
+                                            mode='constant',
+                                            cval=data_smooth_lorentz.max())
+        x_axis_min = x_axis[data_convolved.argmin()] - hf_splitting / 2.
+    else:
+        x_axis_min = x_axis[data_smooth_lorentz.argmin()]
+
+    # data_level = data_smooth_lorentz - data_smooth_lorentz.max()
+    data_level = data_smooth_lorentz - offset
+
+    minimum_level = data_level.min()
+    # integral of data:
+    fit_function = InterpolatedUnivariateSpline(x_axis, data_level, k=1)
+    Integral = fit_function.integral(x_axis[0], x_axis[-1])
+
+    # assume both peaks contribute to the linewidth, so devive by 2, that makes
+    # the peaks narrower
+    sigma = abs(Integral / (np.pi * minimum_level))
+
+    amplitude = -abs(minimum_level)
+
+    minimal_sigma = x_axis[1] - x_axis[0]
+    maximal_sigma = x_axis[-1] - x_axis[0]
+
+    params['l0_amplitude'].set(value=amplitude, max=-1e-6)
+    params['l0_center'].set(value=x_axis_min)
+    params['l0_sigma'].set(value=sigma, min=minimal_sigma,
+                           max=maximal_sigma)
+    params['l1_amplitude'].set(value=params['l0_amplitude'].value,
+                               max=-1e-6)
+    params['l1_center'].set(value=params['l0_center'].value + hf_splitting,
+                            expr='l0_center+{0}'.format(hf_splitting))
+    params['l1_sigma'].set(value=params['l0_sigma'].value,
+                           min=minimal_sigma, max=maximal_sigma,
+                           expr='l0_sigma')
+    params['offset'].set(value=offset)
+
+    return error, params
+
+
+############################################################################
+#                                                                          #
+#                      Triple Lorentzian fitting                           #
+#                                                                          #
+############################################################################
+#Todo: check where code breaks
+# Old Method Names:
+# make_N14_fit
+
+def make_lorentziantriple_fit(self, x_axis, data, estimator, units=None,
+                            add_params=None, **kwargs):
+    """ Perform a triple lorentzian fit
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object model: lmfit.model.ModelFit object, all parameters
+                          provided about the fitting, like: success,
+                          initial fitting values, best fitting values, data
+                          with best fit with given axis,...
+    """
+
+    model, params = self.make_lorentziantriple_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = model.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.error('The triple lorentzian fit did not '
+                       'work: {0}'.format(result.message))
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+
+    if units is None:
+        units = ["arb. units"]
+
+    result_str_dict['Position 0'] = {'value': result.params['l0_center'].value,
+                                     'error': result.params['l0_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Position 1'] = {'value': result.params['l1_center'].value,
+                                     'error': result.params['l1_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Position 2'] = {'value': result.params['l2_center'].value,
+                                     'error': result.params['l2_center'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Contrast 0'] = {'value': abs(result.params['l0_contrast'].value),
+                                     'error': result.params['l0_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['Contrast 1'] = {'value': abs(result.params['l1_contrast'].value),
+                                     'error': result.params['l1_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['Contrast 2'] = {'value': abs(result.params['l2_contrast'].value),
+                                     'error': result.params['l2_contrast'].stderr,
+                                     'unit': '%'}
+
+    result_str_dict['FWHM 0'] = {'value': result.params['l0_sigma'].value,
+                                 'error': result.params['l0_sigma'].stderr,
+                                 'unit': units[0]}
+
+    result_str_dict['FWHM 1'] = {'value': result.params['l1_sigma'].value,
+                                 'error': result.params['l1_sigma'].stderr,
+                                 'unit': units[0]}
+
+    result_str_dict['FWHM 2'] = {'value': result.params['l2_sigma'].value,
+                                 'error': result.params['l2_sigma'].stderr,
+                                 'unit': units[0]}
+
+    result_str_dict['chi_sqr'] = {'value': result.chisqr, 'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+def estimate_lorentziantriple_N14(self, x_axis, data, params):
+    """ Estimation of a the hyperfine interaction of a N14 nuclear spin.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+
+    Provide an estimation of all fitting parameters for fitting the
+    three equidistant lorentzian dips of the hyperfine interaction
+    of a N14 nuclear spin. Here the splitting is set as an expression,
+    if the splitting is not exactly 2.15MHz the fit will not work.
+
+    Note that this estimator is really specific to a physical scenario.
+    Therefore the x_axis is expected to be in SI units Hz, and the x_axis should
+    be at least half of the hyperfine interaction long (2.15MHz) but also be
+    less then 1 GHz. Otherwise the underlying estimation algorithm will not
+    work.
+    """
+
+    # check if parameters make sense
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    hf_splitting = 2.15e6 # hyperfine splitting for a N14 spin
+
+    # this is an estimator, for a physical application, therefore the x_axis
+    # should fulfill certain constraints:
+    length_x_scan = x_axis[-1] - x_axis[0]
+
+    if length_x_scan < hf_splitting/2 or hf_splitting > 1e9:
+        self.log.error('The N14 estimator expects an x_axis with a length in the '
+                     'range [{0},{1}]Hz, but the passed x_axis has a length of '
+                     '{2}, which is not sensible for the N14 estimator. Correct '
+                     'that!'.format(hf_splitting/2, 1e9, length_x_scan))
+        return -1, params
+
+    # find the offset parameter, which should be in the fit the zero level:
+    data_smooth_lorentz, offset = self.find_offset_parameter(x_axis, data)
+
+    # Create now a filter of length 5MHz, then create a step-wise function with
+    # three dips. This step-wise function will be convolved with the smoothed
+    # data, where the maximal contribution will be if the peaks are within the
+    # filter. Take that to obtain from that the accurate peak position:
+
+    # filter of one dip should always have a length of approx linewidth 1MHz
+    points_within_1MHz = len(x_axis)/(x_axis.max()-x_axis.min()) * 1e6
+
+    # filter should have a width of 5MHz
+    x_filter = np.linspace(0, 5*points_within_1MHz, 5*points_within_1MHz)
+    lorentz = np.piecewise(x_filter, [(x_filter >= 0)                   * (x_filter < len(x_filter)*1/5),
+                                      (x_filter >= len(x_filter)*1/5)   * (x_filter < len(x_filter)*2/5),
+                                      (x_filter >= len(x_filter)*2/5)   * (x_filter < len(x_filter)*3/5),
+                                      (x_filter >= len(x_filter)*3/5)   * (x_filter < len(x_filter)*4/5),
+                                      (x_filter >= len(x_filter)*4/5)],
+                           [1, 0, 1, 0, 1])
+
+    # if the filter is smaller than 5 points a convolution does not make sense
+    if len(lorentz) >= 5:
+        data_convolved = filters.convolve1d(data_smooth_lorentz,
+                                            lorentz/lorentz.sum(),
+                                            mode='constant',
+                                            cval=data_smooth_lorentz.max())
+        x_axis_min = x_axis[data_convolved.argmin()]-2.15*1e6
+    else:
+        x_axis_min = x_axis[data_smooth_lorentz.argmin()]-2.15*1e6
+
+    # level of the data, that means the offset is subtracted and the real data
+    # are present
+    data_level = data_smooth_lorentz - offset
+    minimum_level = data_level.min()
+
+    # In order to perform a smooth integral to obtain the area under the curve
+    # make an interpolation of the passed data, in case they are very sparse.
+    # That increases the accuracy of the calculated Integral.
+    # integral of data corresponds to sqrt(2) * Amplitude * Sigma
+
+    smoothing_spline = 1    # must be 1<= smoothing_spline <= 5
+    fit_function = InterpolatedUnivariateSpline(x_axis, data_level, k=smoothing_spline)
+    integrated_area = fit_function.integral(x_axis[0], x_axis[-1])
+
+    # sigma = abs(integrated_area / (minimum_level/np.pi))
+    # That is wrong, so commenting out:
+    sigma = abs(integrated_area /(np.pi * minimum_level))/3
+
+    amplitude = -1*abs(minimum_level)
+
+    # Since the total amplitude of the lorentzian is depending on sigma it makes
+    # sense to vary sigma within an interval, which is smaller than the minimal
+    # distance between two points. Then the fit algorithm will have a larger
+    # range to determine the amplitude properly. That is the main issue with the
+    # fit!
+    minimal_linewidth = (x_axis[1]-x_axis[0])/4
+    maximal_linewidth = x_axis[-1]-x_axis[0]
+
+    # The linewidth of all the lorentzians are set to be the same! that is a
+    # physical constraint for the N14 fitting.
+
+    # Fill the parameter container, with the estimated values, which should be
+    # passed to the fit algorithm:
+    params['l0_amplitude'].set(value=amplitude, max=-1e-6)
+    params['l0_center'].set(value=x_axis_min)
+    params['l0_sigma'].set(value=sigma, min=minimal_linewidth,
+                           max=maximal_linewidth)
+    params['l1_amplitude'].set(value=amplitude, max=-1e-6)
+    params['l1_center'].set(value=x_axis_min+hf_splitting,
+                            expr='l0_center+{0}'.format(hf_splitting))
+    params['l1_sigma'].set(value=sigma, min=minimal_linewidth,
+                           max=maximal_linewidth, expr='l0_sigma')
+    params['l2_amplitude'].set(value=amplitude, max=-1e-6)
+    params['l2_center'].set(value=x_axis_min+hf_splitting*2,
+                            expr='l0_center+{0}'.format(hf_splitting*2))
+    params['l2_sigma'].set(value=sigma, min=minimal_linewidth,
+                           max=maximal_linewidth, expr='l0_sigma')
+    params['offset'].set(value=offset)
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/poissonianlikemethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/poissonianlikemethods.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,386 +1,386 @@
-# -*- coding: utf-8 -*-
-
-"""
-This file contains the Qudi fitting logic functions needed for
-poissinian-like-methods.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-from collections import OrderedDict
-
-import numpy as np
-from lmfit import Parameters
-from lmfit.models import Model
-from scipy.interpolate import InterpolatedUnivariateSpline
-from scipy.ndimage import filters
-from scipy.signal import gaussian
-from scipy.special import gammaln, xlogy
-
-
-################################################################################
-#                                                                              #
-#                      Defining Poissonian models                              #
-#                                                                              #
-################################################################################
-
-
-def poisson(self, x, mu):
-    """
-    Poisson function taken from:
-    https://github.com/scipy/scipy/blob/master/scipy/stats/_discrete_distns.py
-
-    For license see documentation/BSDLicense_scipy.md
-
-    Author:  Travis Oliphant  2002-2011 with contributions from
-             SciPy Developers 2004-2011
-    """
-    if len(np.atleast_1d(x)) == 1:
-        check_val = x
-    else:
-        check_val = x[0]
-
-    if check_val > 1e18:
-        self.log.warning('The current value in the poissonian distribution '
-                         'exceeds 1e18! Due to numerical imprecision a valid '
-                         'functional output cannot be guaranteed any more!')
-
-    # According to the central limit theorem, a poissonian distribution becomes
-    # a gaussian distribution for large enough x. Since the numerical precision
-    # is limited to calculate the logarithmized poissonian and obtain from that
-    # the exponential value, a self defined cutoff is introduced and set to
-    # 1e12. Beyond that number a gaussian distribution is assumed, which is a
-    # completely valid assumption.
-
-    if check_val < 1e12:
-        return np.exp(xlogy(x, mu) - gammaln(x + 1) - mu)
-    else:
-        return np.exp(-((x - mu) ** 2) / (2 * mu)) / (np.sqrt(2 * np.pi * mu))
-
-
-def make_poissonian_model(self, prefix=None):
-    """ Create a model of a single poissonian with an offset.
-
-    param str prefix: optional string, which serves as a prefix for all
-                       parameters used in this model. That will prevent
-                       name collisions if this model is used in a composite
-                       way.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-    """
-    def poisson_function(x, mu):
-        """ Function of a poisson distribution.
-
-        @param numpy.array x: 1D array as the independent variable - e.g. occurences
-        @param float mu: expectation value
-
-        @return: poisson function: in order to use it as a model
-        """
-        return self.poisson(x, mu)
-
-    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
-
-    if not isinstance(prefix, str) and prefix is not None:
-
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                       'cannot be used as a prefix and will be ignored for now.'
-                       'Correct that!'.format(prefix, type(prefix)))
-
-        poissonian_model = Model(poisson_function, independent_vars=['x'])
-
-    else:
-
-        poissonian_model = Model(poisson_function, independent_vars=['x'],
-                                 prefix=prefix)
-
-    poissonian_ampl_model = amplitude_model * poissonian_model
-    params = poissonian_ampl_model.make_params()
-
-    return poissonian_ampl_model, params
-
-
-def make_poissonianmultiple_model(self, no_of_functions=1):
-    """ Create a model with multiple poissonians with amplitude.
-
-    @param no_of_functions: for default=1 there is one poissonian, else
-                            more functions are added
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_poissonian_model.
-    """
-
-    if no_of_functions == 1:
-        multi_poisson_model, params = self.make_poissonian_model()
-    else:
-        multi_poisson_model, params = self.make_poissonian_model(prefix='p0_')
-
-        for ii in range(1, no_of_functions):
-            multi_poisson_model += self.make_poissonian_model(prefix='p{0:d}_'.format(ii))[0]
-    params = multi_poisson_model.make_params()
-
-    return multi_poisson_model, params
-
-def make_poissoniandouble_model(self):
-    return self.make_poissonianmultiple_model(2)
-
-################################################################################
-#                                                                              #
-#                    Poissonian fits and their estimators                      #
-#                                                                              #
-################################################################################
-
-
-def make_poissonian_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Performe a poissonian fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-
-    poissonian_model, params = self.make_poissonian_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-
-    try:
-        result = poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The poissonian fit did not work. Check if a poisson '
-                         'distribution is needed or a normal approximation can be'
-                         'used. For values above 10 a normal/ gaussian distribution '
-                         'is a good approximation.')
-        result = poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
-        print(result.message)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui   oder OrderedDict()
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error': result.params['amplitude'].stderr,
-                                    'unit': units[1]}     # Amplitude
-
-    result_str_dict['Event rate'] = {'value': result.params['mu'].value,
-                                    'error': result.params['mu'].stderr,
-                                    'unit': units[0]}      # event rate
-
-    result.result_str_dict = result_str_dict
-
-    return result
-
-
-def estimate_poissonian(self, x_axis, data, params):
-    """ Provide an estimator for initial values of a poissonian function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # a gaussian filter is appropriate due to the well approximation of poisson
-    # distribution
-    # gaus = gaussian(10,10)
-    # data_smooth = filters.convolve1d(data, gaus/gaus.sum(), mode='mirror')
-    data_smooth = self.gaussian_smoothing(data=data, filter_len=10,
-                                          filter_sigma=10)
-
-    # set parameters
-    mu = x_axis[np.argmax(data_smooth)]
-    params['mu'].value = mu
-    params['amplitude'].value = data_smooth.max() / self.poisson(mu, mu)
-
-    return error, params
-
-
-def make_poissoniandouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a double poissonian fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-
-    double_poissonian_model, params = self.make_poissoniandouble_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-
-    try:
-        result = double_poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The double poissonian fit did not work. Check if a '
-                         'poisson distribution is needed or a normal '
-                         'approximation can be used. For values above 10 a '
-                         'normal/ gaussian distribution is a good '
-                         'approximation.')
-        result = double_poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
-
-    # Write the parameters to allow human-readable output to be generated
-    result_str_dict = OrderedDict()
-    if units is None:
-        units = ["arb. units", 'arb. unit']
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['p0_amplitude'].value,
-                                      'error': result.params['p0_amplitude'].stderr,
-                                      'unit': units[0]}
-
-    result_str_dict['Event rate 1'] = {'value': result.params['p0_mu'].value,
-                                       'error': result.params['p0_mu'].stderr,
-                                       'unit':  units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['p1_amplitude'].value,
-                                      'error': result.params['p1_amplitude'].stderr,
-                                      'unit': units[0]}
-
-    result_str_dict['Event rate 2'] = {'value': result.params['p1_mu'].value,
-                                       'error': result.params['p1_mu'].stderr,
-                                       'unit':  units[1]}
-
-    result.result_str_dict = result_str_dict
-
-    return result
-
-
-def estimate_poissoniandouble(self, x_axis, data, params, threshold_fraction=0.4,
-                              minimal_threshold=0.1, sigma_threshold_fraction=0.2):
-    """ Provide initial values for a double poissonian fit.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-    @param float threshold_fraction : Threshold to find second poissonian
-    @param float minimal_threshold: Threshold is lowered to minimal this
-                                    value as a fraction
-    @param float sigma_threshold_fraction: Threshold for detecting
-                                           the end of the peak
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-
-    The parameters coming from the physical properties of an experiment
-    done in gated counter:
-                    - positive peak
-                    - no values below 0
-                    - rather broad overlapping functions
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # TODO: make the filter an extra function shared and usable for other functions.
-    # Calculate here also an interpolation factor, which will be based on the
-    # given data set. If the convolution later on has more points, then the fit
-    # has a higher chance to be successful. The interpol_factor multiplies the
-    # number of points.
-    # Set the interpolation factor according to the amount of data. Too much
-    # interpolation is not good for the peak estimation, also too less in not
-    # good.
-
-    if len(x_axis) < 20.:
-        len_x = 5
-        interpol_factor = 8
-    elif len(x_axis) >= 100.:
-        len_x = 10
-        interpol_factor = 1
-    else:
-        if len(x_axis) < 60:
-            interpol_factor = 4
-        else:
-            interpol_factor = 2
-        len_x = int(len(x_axis) / 10.) + 1
-
-    # Create the interpolation function, based on the data:
-    interpol_function = InterpolatedUnivariateSpline(x_axis, data, k=1)
-    # adjust the x_axis to that:
-    x_axis_interpol = np.linspace(x_axis[0], x_axis[-1], len(x_axis) * interpol_factor)
-    # create actually the interpolated data:
-    interpol_data = interpol_function(x_axis_interpol)
-
-    # Use a gaussian function to convolve with the data, to smooth the datatrace.
-    # Then the peak search algorithm performs much better.
-    gaus = gaussian(len_x, len_x)
-    data_smooth = filters.convolve1d(interpol_data, gaus / gaus.sum(), mode='mirror')
-
-    # search for double gaussian
-    search_results = self._search_double_dip(x_axis_interpol,
-                                             data_smooth * (-1),
-                                             threshold_fraction,
-                                             minimal_threshold,
-                                             sigma_threshold_fraction,
-                                             make_prints=False)
-    error = search_results[0]
-    sigma0_argleft, dip0_arg, sigma0_argright = search_results[1:4]
-    sigma1_argleft, dip1_arg, sigma1_argright = search_results[4:7]
-
-    # set the initial values for the fit:
-    params['p0_mu'].set(value=x_axis_interpol[dip0_arg])
-    amplitude0 = (data_smooth[dip0_arg] / self.poisson(x_axis_interpol[dip0_arg], x_axis_interpol[dip0_arg]))
-    params['p0_amplitude'].set(value=amplitude0, min=1e-15)
-
-    params['p1_mu'].set(value=x_axis_interpol[dip1_arg])
-    amplitude1 = (data_smooth[dip1_arg] / self.poisson(x_axis_interpol[dip1_arg], x_axis_interpol[dip1_arg]))
-    params['p1_amplitude'].set(value=amplitude1, min=1e-15)
-
-    return error, params
+# -*- coding: utf-8 -*-
+
+"""
+This file contains the Qudi fitting logic functions needed for
+poissinian-like-methods.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+from collections import OrderedDict
+
+import numpy as np
+from lmfit import Parameters
+from lmfit.models import Model
+from scipy.interpolate import InterpolatedUnivariateSpline
+from scipy.ndimage import filters
+from scipy.signal import gaussian
+from scipy.special import gammaln, xlogy
+
+
+################################################################################
+#                                                                              #
+#                      Defining Poissonian models                              #
+#                                                                              #
+################################################################################
+
+
+def poisson(self, x, mu):
+    """
+    Poisson function taken from:
+    https://github.com/scipy/scipy/blob/master/scipy/stats/_discrete_distns.py
+
+    For license see documentation/BSDLicense_scipy.md
+
+    Author:  Travis Oliphant  2002-2011 with contributions from
+             SciPy Developers 2004-2011
+    """
+    if len(np.atleast_1d(x)) == 1:
+        check_val = x
+    else:
+        check_val = x[0]
+
+    if check_val > 1e18:
+        self.log.warning('The current value in the poissonian distribution '
+                         'exceeds 1e18! Due to numerical imprecision a valid '
+                         'functional output cannot be guaranteed any more!')
+
+    # According to the central limit theorem, a poissonian distribution becomes
+    # a gaussian distribution for large enough x. Since the numerical precision
+    # is limited to calculate the logarithmized poissonian and obtain from that
+    # the exponential value, a self defined cutoff is introduced and set to
+    # 1e12. Beyond that number a gaussian distribution is assumed, which is a
+    # completely valid assumption.
+
+    if check_val < 1e12:
+        return np.exp(xlogy(x, mu) - gammaln(x + 1) - mu)
+    else:
+        return np.exp(-((x - mu) ** 2) / (2 * mu)) / (np.sqrt(2 * np.pi * mu))
+
+
+def make_poissonian_model(self, prefix=None):
+    """ Create a model of a single poissonian with an offset.
+
+    param str prefix: optional string, which serves as a prefix for all
+                       parameters used in this model. That will prevent
+                       name collisions if this model is used in a composite
+                       way.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+    """
+    def poisson_function(x, mu):
+        """ Function of a poisson distribution.
+
+        @param numpy.array x: 1D array as the independent variable - e.g. occurences
+        @param float mu: expectation value
+
+        @return: poisson function: in order to use it as a model
+        """
+        return self.poisson(x, mu)
+
+    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
+
+    if not isinstance(prefix, str) and prefix is not None:
+
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                       'cannot be used as a prefix and will be ignored for now.'
+                       'Correct that!'.format(prefix, type(prefix)))
+
+        poissonian_model = Model(poisson_function, independent_vars=['x'])
+
+    else:
+
+        poissonian_model = Model(poisson_function, independent_vars=['x'],
+                                 prefix=prefix)
+
+    poissonian_ampl_model = amplitude_model * poissonian_model
+    params = poissonian_ampl_model.make_params()
+
+    return poissonian_ampl_model, params
+
+
+def make_poissonianmultiple_model(self, no_of_functions=1):
+    """ Create a model with multiple poissonians with amplitude.
+
+    @param no_of_functions: for default=1 there is one poissonian, else
+                            more functions are added
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_poissonian_model.
+    """
+
+    if no_of_functions == 1:
+        multi_poisson_model, params = self.make_poissonian_model()
+    else:
+        multi_poisson_model, params = self.make_poissonian_model(prefix='p0_')
+
+        for ii in range(1, no_of_functions):
+            multi_poisson_model += self.make_poissonian_model(prefix='p{0:d}_'.format(ii))[0]
+    params = multi_poisson_model.make_params()
+
+    return multi_poisson_model, params
+
+def make_poissoniandouble_model(self):
+    return self.make_poissonianmultiple_model(2)
+
+################################################################################
+#                                                                              #
+#                    Poissonian fits and their estimators                      #
+#                                                                              #
+################################################################################
+
+
+def make_poissonian_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Performe a poissonian fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+
+    poissonian_model, params = self.make_poissonian_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+
+    try:
+        result = poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The poissonian fit did not work. Check if a poisson '
+                         'distribution is needed or a normal approximation can be'
+                         'used. For values above 10 a normal/ gaussian distribution '
+                         'is a good approximation.')
+        result = poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
+        print(result.message)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui   oder OrderedDict()
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error': result.params['amplitude'].stderr,
+                                    'unit': units[1]}     # Amplitude
+
+    result_str_dict['Event rate'] = {'value': result.params['mu'].value,
+                                    'error': result.params['mu'].stderr,
+                                    'unit': units[0]}      # event rate
+
+    result.result_str_dict = result_str_dict
+
+    return result
+
+
+def estimate_poissonian(self, x_axis, data, params):
+    """ Provide an estimator for initial values of a poissonian function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # a gaussian filter is appropriate due to the well approximation of poisson
+    # distribution
+    # gaus = gaussian(10,10)
+    # data_smooth = filters.convolve1d(data, gaus/gaus.sum(), mode='mirror')
+    data_smooth = self.gaussian_smoothing(data=data, filter_len=10,
+                                          filter_sigma=10)
+
+    # set parameters
+    mu = x_axis[np.argmax(data_smooth)]
+    params['mu'].value = mu
+    params['amplitude'].value = data_smooth.max() / self.poisson(mu, mu)
+
+    return error, params
+
+
+def make_poissoniandouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a double poissonian fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+
+    double_poissonian_model, params = self.make_poissoniandouble_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+
+    try:
+        result = double_poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The double poissonian fit did not work. Check if a '
+                         'poisson distribution is needed or a normal '
+                         'approximation can be used. For values above 10 a '
+                         'normal/ gaussian distribution is a good '
+                         'approximation.')
+        result = double_poissonian_model.fit(data, x=x_axis, params=params, **kwargs)
+
+    # Write the parameters to allow human-readable output to be generated
+    result_str_dict = OrderedDict()
+    if units is None:
+        units = ["arb. units", 'arb. unit']
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['p0_amplitude'].value,
+                                      'error': result.params['p0_amplitude'].stderr,
+                                      'unit': units[0]}
+
+    result_str_dict['Event rate 1'] = {'value': result.params['p0_mu'].value,
+                                       'error': result.params['p0_mu'].stderr,
+                                       'unit':  units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['p1_amplitude'].value,
+                                      'error': result.params['p1_amplitude'].stderr,
+                                      'unit': units[0]}
+
+    result_str_dict['Event rate 2'] = {'value': result.params['p1_mu'].value,
+                                       'error': result.params['p1_mu'].stderr,
+                                       'unit':  units[1]}
+
+    result.result_str_dict = result_str_dict
+
+    return result
+
+
+def estimate_poissoniandouble(self, x_axis, data, params, threshold_fraction=0.4,
+                              minimal_threshold=0.1, sigma_threshold_fraction=0.2):
+    """ Provide initial values for a double poissonian fit.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+    @param float threshold_fraction : Threshold to find second poissonian
+    @param float minimal_threshold: Threshold is lowered to minimal this
+                                    value as a fraction
+    @param float sigma_threshold_fraction: Threshold for detecting
+                                           the end of the peak
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+
+    The parameters coming from the physical properties of an experiment
+    done in gated counter:
+                    - positive peak
+                    - no values below 0
+                    - rather broad overlapping functions
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # TODO: make the filter an extra function shared and usable for other functions.
+    # Calculate here also an interpolation factor, which will be based on the
+    # given data set. If the convolution later on has more points, then the fit
+    # has a higher chance to be successful. The interpol_factor multiplies the
+    # number of points.
+    # Set the interpolation factor according to the amount of data. Too much
+    # interpolation is not good for the peak estimation, also too less in not
+    # good.
+
+    if len(x_axis) < 20.:
+        len_x = 5
+        interpol_factor = 8
+    elif len(x_axis) >= 100.:
+        len_x = 10
+        interpol_factor = 1
+    else:
+        if len(x_axis) < 60:
+            interpol_factor = 4
+        else:
+            interpol_factor = 2
+        len_x = int(len(x_axis) / 10.) + 1
+
+    # Create the interpolation function, based on the data:
+    interpol_function = InterpolatedUnivariateSpline(x_axis, data, k=1)
+    # adjust the x_axis to that:
+    x_axis_interpol = np.linspace(x_axis[0], x_axis[-1], len(x_axis) * interpol_factor)
+    # create actually the interpolated data:
+    interpol_data = interpol_function(x_axis_interpol)
+
+    # Use a gaussian function to convolve with the data, to smooth the datatrace.
+    # Then the peak search algorithm performs much better.
+    gaus = gaussian(len_x, len_x)
+    data_smooth = filters.convolve1d(interpol_data, gaus / gaus.sum(), mode='mirror')
+
+    # search for double gaussian
+    search_results = self._search_double_dip(x_axis_interpol,
+                                             data_smooth * (-1),
+                                             threshold_fraction,
+                                             minimal_threshold,
+                                             sigma_threshold_fraction,
+                                             make_prints=False)
+    error = search_results[0]
+    sigma0_argleft, dip0_arg, sigma0_argright = search_results[1:4]
+    sigma1_argleft, dip1_arg, sigma1_argright = search_results[4:7]
+
+    # set the initial values for the fit:
+    params['p0_mu'].set(value=x_axis_interpol[dip0_arg])
+    amplitude0 = (data_smooth[dip0_arg] / self.poisson(x_axis_interpol[dip0_arg], x_axis_interpol[dip0_arg]))
+    params['p0_amplitude'].set(value=amplitude0, min=1e-15)
+
+    params['p1_mu'].set(value=x_axis_interpol[dip1_arg])
+    amplitude1 = (data_smooth[dip1_arg] / self.poisson(x_axis_interpol[dip1_arg], x_axis_interpol[dip1_arg]))
+    params['p1_amplitude'].set(value=amplitude1, min=1e-15)
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/fitmethods/sinemethods.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/fitmethods/sinemethods.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,2230 +1,2230 @@
-# -*- coding: utf-8 -*-
-"""
-This file contains methods for sine fitting, these methods
-are imported by class FitLogic.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-import numpy as np
-from lmfit.models import Model
-from scipy import signal
-
-
-def get_ft_windows():
-    """ Retrieve the available windows to be applied on signal data before FT.
-
-    @return: dict with keys being the window name and items being again a dict
-             containing the actual function and the normalization factor to
-             calculate correctly the amplitude spectrum in the Fourier Transform
-
-    To find out the amplitude normalization factor check either the scipy
-    implementation on
-        https://github.com/scipy/scipy/blob/v0.15.1/scipy/signal/windows.py#L336
-    or just perform a sum of the window (oscillating parts of the window should
-    be averaged out and constant offset factor will remain):
-        MM=1000000  # choose a big number
-        print(sum(signal.hanning(MM))/MM)
-    """
-
-    win = {'none': {'func': np.ones, 'ampl_norm': 1.0},
-           'hamming': {'func': signal.hamming, 'ampl_norm': 1.0/0.54},
-           'hann': {'func': signal.hann, 'ampl_norm': 1.0/0.5},
-           'blackman': {'func': signal.blackman, 'ampl_norm': 1.0/0.42},
-           'triang': {'func': signal.triang, 'ampl_norm': 1.0/0.5},
-           'flattop': {'func': signal.flattop, 'ampl_norm': 1.0/0.2156},
-           'bartlett': {'func': signal.bartlett, 'ampl_norm': 1.0/0.5},
-           'parzen': {'func': signal.parzen, 'ampl_norm': 1.0/0.375},
-           'bohman': {'func': signal.bohman, 'ampl_norm': 1.0/0.4052847},
-           'blackmanharris': {'func': signal.blackmanharris, 'ampl_norm': 1.0/0.35875},
-           'nuttall': {'func': signal.nuttall, 'ampl_norm': 1.0/0.3635819},
-           'barthann': {'func': signal.barthann, 'ampl_norm': 1.0/0.5}}
-    return win
-
-
-def compute_ft(x_val, y_val, zeropad_num=0, window='none', base_corr=True, psd=False):
-    """ Compute the Discrete fourier Transform of the power spectral density
-
-    @param numpy.array x_val: 1D array
-    @param numpy.array y_val: 1D array of same size as x_val
-    @param int zeropad_num: optional, zeropadding (adding zeros to the end of
-                            the array). zeropad_num >= 0, the size of the array
-                            which is add to the end of the y_val before
-                            performing the Fourier Transform (FT). The
-                            resulting array will have the length
-                                (len(y_val)/2)*(zeropad_num+1)
-                            Note that zeropadding will not change or add more
-                            information to the dft, it will solely interpolate
-                            between the dft_y values (corresponds to a Sinc
-                            interpolation method).
-                            Set zeropad_num=1 to obtain output arrays which
-                            have the same size as the input arrays.
-                            Default is zeropad_num=0.
-    @param str window: optional, the window function which should be applied to
-                       the y values before Fourier Transform is calculated.
-    @param bool base_corr: Select whether baseline correction shoud be performed
-                           before calculating the FT.
-    @param bool psd: optional, select whether the Discrete Fourier Transform or
-                     the Power Spectral Density (PSD, which is just the FT of
-                     the absolute square of the y-values) should be computed.
-                     Default is psd=False.
-
-    @return: tuple(dft_x, dft_y):
-                be aware that the return arrays' length depend on the zeropad
-                number like
-                    len(dft_x) = len(dft_y) = (len(y_val)/2)*(zeropad_num+1)
-
-    Pay attention that the return values of the FT have only half of the
-    entries compared to the used signal input (if zeropad=0).
-
-    In general, a window function should be applied on the y data before
-    calculating the FT, to reduce spectral leakage. The Hann window for
-    instance is almost never a bad choice. Use it like window='hann'
-
-    Keep always in mind the relation to the Fourier transform space:
-        T = delta_t * N_samples
-    where delta_t is the distance between the time points and N_samples are the
-    amount of points in the time domain. Consequently the sample rate is
-        f_samplerate = T / N_samples
-
-    Keep also in mind that the FT returns value from 0 to f_samplerate, or
-        equivalently -f_samplerate/2 to f_samplerate/2.
-
-    Difference between PSD and DFT:
-    The power spectral density (PSD) describes how the power of your signal is
-    distributed over frequency whilst the DFT shows the spectral content of
-    your signal, i.e. the amplitude and phase of harmonics in your signal.
-    """
-
-    avail_windows = get_ft_windows()
-
-    x_val = np.array(x_val)
-    y_val = np.array(y_val)
-
-    # Make a baseline correction to avoid a constant offset near zero
-    # frequencies. Offset of the y_val from mean corresponds to half the value
-    # at fft_y[0].
-    corrected_y = y_val
-    if base_corr:
-        corrected_y = y_val - y_val.mean()
-
-    ampl_norm_fact = 1.0
-    # apply window to data to account for spectral leakage:
-    if window in avail_windows:
-        window_val = avail_windows[window]['func'](len(y_val))
-        corrected_y = corrected_y * window_val
-        # to get the correct amplitude in the amplitude spectrum
-        ampl_norm_fact = avail_windows[window]['ampl_norm']
-
-    # zeropad for sinc interpolation:
-    zeropad_arr = np.zeros(len(corrected_y)*(zeropad_num+1))
-    zeropad_arr[:len(corrected_y)] = corrected_y
-
-    # Get the amplitude values from the fourier transformed y values.
-    fft_y = np.abs(np.fft.fft(zeropad_arr))
-
-    # Power spectral density (PSD) or just amplitude spectrum of fourier signal:
-    power_value = 1.0
-    if psd:
-        power_value = 2.0
-
-    # The factor 2 accounts for the fact that just the half of the spectrum was
-    # taken. The ampl_norm_fact is the normalization factor due to the applied
-    # window function (the offset value in the window function):
-    fft_y = ((2/len(y_val)) * fft_y * ampl_norm_fact)**power_value
-
-    # Due to the sampling theorem you can only identify frequencies at half
-    # of the sample rate, therefore the FT contains an almost symmetric
-    # spectrum (the asymmetry results from aliasing effects). Therefore take
-    # the half of the values for the display.
-    middle = int((len(zeropad_arr)+1)//2)
-
-    # sample spacing of x_axis, if x is a time axis than it corresponds to a
-    # timestep:
-    x_spacing = np.round(x_val[-1] - x_val[-2], 12)
-
-    # use the helper function of numpy to calculate the x_values for the
-    # fourier space. That function will handle an occuring devision by 0:
-    fft_x = np.fft.fftfreq(len(zeropad_arr), d=x_spacing)
-
-    return abs(fft_x[:middle]), fft_y[:middle]
-
-
-################################################################################
-#                                                                              #
-#                               Defining Sine models                           #
-#                                                                              #
-################################################################################
-
-##################################################
-# Bare sine with unitary amplitude and no offset #
-##################################################
-
-def make_baresine_model(self, prefix=None):
-    """ Create a bare sine model without amplitude and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params)
-
-    Explanation of the objects:
-        object lmfit.model.CompositeModel model:
-            A model the lmfit module will use for that fit. Here a
-            gaussian model. Returns an object of the class
-            lmfit.model.CompositeModel.
-
-        object lmfit.parameter.Parameters params:
-            It is basically an OrderedDict, so a dictionary, with keys
-            denoting the parameters as string names and values which are
-            lmfit.parameter.Parameter (without s) objects, keeping the
-            information about the current value.
-
-        For further information have a look in:
-    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.GaussianModel
-    """
-
-    def bare_sine_function(x, frequency, phase):
-        """ Function of a bare sine.
-
-        @param numpy.array x: independant variable - e.g. time
-        @param float frequency: frequency
-        @param float phase: phase
-
-        @return: reference to method of a sine function in order to use it as a
-                 model
-        """
-
-        return np.sin(2*np.pi*frequency*x+phase)
-
-    if not isinstance(prefix, str) and prefix is not None:
-        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
-                       'cannot be used as a prefix and will be ignored for now.'
-                       'Correct that!'.format(prefix, type(prefix)))
-        model = Model(bare_sine_function, independent_vars=['x'])
-    else:
-        model = Model(bare_sine_function, independent_vars=['x'], prefix=prefix)
-
-    params = model.make_params()
-
-    return model, params
-
-###############################
-# Centred sine with no offset #
-###############################
-
-
-def make_sinewithoutoffset_model(self, prefix=None):
-    """ Create a model of sine with an amplitude.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-    baresine_model, params = self.make_baresine_model(prefix=prefix)
-    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
-
-    sine_model = amplitude_model*baresine_model
-    params = sine_model.make_params()
-
-    return sine_model, params
-
-############################
-# General sine with offset #
-############################
-
-
-def make_sine_model(self, prefix=None):
-    """ Create a sine model with amplitude and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    sine_offset_model = sine_model + constant_model
-    params = sine_offset_model.make_params()
-
-    return sine_offset_model, params
-
-###############################################
-# Sinus with exponential decay but not offset #
-###############################################
-
-
-def make_sineexpdecaywithoutoffset_model(self, prefix=None):
-    """ Create a model of a sine with exponential decay.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
-    bareexponentialdecay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
-
-    sine_exp_decay_model = sine_model*bareexponentialdecay_model
-    params = sine_exp_decay_model.make_params()
-
-    return sine_exp_decay_model, params
-
-###################################################
-# Sinus with exponential decay and offset fitting #
-###################################################
-
-def make_sineexponentialdecay_model(self, prefix=None):
-    """ Create a model of a sine with exponential decay and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    sine_exp_decay_model, params = self.make_sineexpdecaywithoutoffset_model(prefix=prefix)
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    sine_exp_decay_offset_model = sine_exp_decay_model + constant_model
-    params = sine_exp_decay_offset_model.make_params()
-
-    return sine_exp_decay_offset_model, params
-
-###################################################
-# Sinus with stretched exponential decay fitting  #
-###################################################
-
-def make_sinestretchedexponentialdecay_model(self, prefix=None):
-    """ Create a model of a sine with stretched exponential decay.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
-    bare_stretched_exp_decay_model, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    model = sine_model * bare_stretched_exp_decay_model + constant_model
-    params = model.make_params()
-
-    return model, params
-
-###########################################
-# Sum of two individual Sinus with offset #
-###########################################
-
-
-def make_sinedouble_model(self, prefix=None):
-    """ Create a model of two summed sine with an offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
-    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    two_sine_offset = sine_model1 + sine_model2 + constant_model
-    params = two_sine_offset.make_params()
-
-    return two_sine_offset, params
-
-################################################################################
-#    Sum of two individual Sinus with offset and single exponential decay      #
-################################################################################
-
-
-def make_sinedoublewithexpdecay_model(self, prefix=None):
-    """ Create a model of two summed sine with an exponential decay and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
-    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
-    bare_exp_decay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    two_sine_exp_decay_offset = (sine_model1 + sine_model2)*bare_exp_decay_model + constant_model
-    params = two_sine_exp_decay_offset.make_params()
-
-    return two_sine_exp_decay_offset, params
-
-###############################################################
-# Sum of two individual Sinus exponential decays (and offset) #
-###############################################################
-
-
-def make_sinedoublewithtwoexpdecay_model(self, prefix=None):
-    """ Create a model of two summed sine with three exponential decays and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_exp_decay_model1, params = self.make_sineexpdecaywithoutoffset_model(prefix='e1_'+add_text)
-    sine_exp_decay_model2, params = self.make_sineexpdecaywithoutoffset_model(prefix='e2_'+add_text)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    sinedoublewithtwoexpdecay = sine_exp_decay_model1 + sine_exp_decay_model2 + constant_model
-    params = sinedoublewithtwoexpdecay.make_params()
-
-    return sinedoublewithtwoexpdecay, params
-
-#############################################
-# Sum of three individual Sinus with offset #
-#############################################
-
-
-def make_sinetriple_model(self, prefix=None):
-    """ Create a model of three summed sine with an offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
-    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
-    sine_model3, params = self.make_sinewithoutoffset_model(prefix='s3_'+add_text)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    three_sine_offset = sine_model1 + sine_model2 + sine_model3 + constant_model
-    params = three_sine_offset.make_params()
-
-    return three_sine_offset, params
-
-##########################################################################
-# Sum of three individual Sinus with offset and single exponential decay #
-##########################################################################
-
-
-def make_sinetriplewithexpdecay_model(self, prefix=None):
-    """ Create a model of three summed sine with an exponential decay and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
-    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
-    sine_model3, params = self.make_sinewithoutoffset_model(prefix='s3_'+add_text)
-    bare_exp_decay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    three_sine_exp_decay_offset = (
-        sine_model1 + sine_model2 + sine_model3) * bare_exp_decay_model + constant_model
-    params = three_sine_exp_decay_offset.make_params()
-
-    return three_sine_exp_decay_offset, params
-
-#########################################################################
-# Sum of three individual Sinus with offset and three exponential decay #
-#########################################################################
-
-
-def make_sinetriplewiththreeexpdecay_model(self, prefix=None):
-    """ Create a model of three summed sine with three exponential decays and offset.
-
-    @param str prefix: optional, if multiple models should be used in a
-                       composite way and the parameters of each model should be
-                       distinguished from each other to prevent name collisions.
-
-    @return tuple: (object model, object params), for more description see in
-                   the method make_baresine_model.
-    """
-
-    if prefix is None:
-        add_text = ''
-    else:
-        add_text = prefix
-
-    sine_exp_decay_model1, params = self.make_sineexpdecaywithoutoffset_model(prefix='e1_'+add_text)
-    sine_exp_decay_model2, params = self.make_sineexpdecaywithoutoffset_model(prefix='e2_'+add_text)
-    sine_exp_decay_model3, params = self.make_sineexpdecaywithoutoffset_model(prefix='e3_'+add_text)
-
-    constant_model, params = self.make_constant_model(prefix=prefix)
-
-    three_sine_exp_decay_offset = sine_exp_decay_model1 + sine_exp_decay_model2 + sine_exp_decay_model3 + constant_model
-    params = three_sine_exp_decay_offset.make_params()
-
-    return three_sine_exp_decay_offset, params
-
-################################################################################
-#                                                                              #
-#                        General estimators used later                         #
-#                                                                              #
-################################################################################
-
-
-def estimate_baresine(self, x_axis, data, params):
-    """ Bare sine estimator with a frequency and phase.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        lmfit.Parameters params: derived OrderedDict object contains the initial
-                                 values for the fit.
-    """
-
-    # Convert for safety:
-    x_axis = np.array(x_axis)
-    data = np.array(data)
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # calculate dft with zeropadding to obtain nicer interpolation between the
-    # appearing peaks.
-    dft_x, dft_y = compute_ft(x_axis, data, zeropad_num=1)
-
-    stepsize = x_axis[1]-x_axis[0]  # for frequency axis
-    frequency_max = np.abs(dft_x[np.log(dft_y).argmax()])
-
-    # find minimal distance to the next meas point in the corresponding time value>
-    min_x_diff = np.ediff1d(x_axis).min()
-
-    # How many points are used to sample the estimated frequency with min_x_diff:
-    iter_steps = int(1/(frequency_max*min_x_diff))
-    if iter_steps < 1:
-        iter_steps = 1
-
-    sum_res = np.zeros(iter_steps)
-
-    # Procedure: Create sin waves with different phases and perform a summation.
-    #            The sum shows how well the sine was fitting to the actual data.
-    #            The best fitting sine should be a maximum of the summed time
-    #            trace.
-
-    for iter_s in range(iter_steps):
-        func_val = np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps *2*np.pi)
-        sum_res[iter_s] = np.abs(data - func_val).sum()
-
-    # The minimum indicates where the sine function was fittng the worst,
-    # therefore subtract pi. This will also ensure that the estimated phase will
-    # be in the interval [-pi,pi].
-    phase = sum_res.argmax()/iter_steps *2*np.pi - np.pi
-
-    params['frequency'].set(value=frequency_max, min=0.0, max=1/stepsize*3)
-    params['phase'].set(value=phase, min=-np.pi, max=np.pi)
-
-    return error, params
-
-
-def estimate_sinewithoutoffset(self, x_axis, data, params):
-    """ Sine estimator, with an amplitude, frequency and phase.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        lmfit.Parameters params: derived OrderedDict object contains the initial
-                                 values for the fit.
-    """
-
-    # Convert for safety:
-    x_axis = np.array(x_axis)
-    data = np.array(data)
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # sort the input
-    sorted_indices = x_axis.argsort()
-    x_axis = x_axis[sorted_indices]
-    data = data[sorted_indices]
-
-    # estimate amplitude
-    ampl_val = max(np.abs(data.min()), np.abs(data.max()))
-
-    # calculate dft with zeropadding to obtain nicer interpolation between the
-    # appearing peaks.
-    dft_x, dft_y = compute_ft(x_axis, data, zeropad_num=1)
-
-    stepsize = x_axis[1] - x_axis[0]  # for frequency axis
-
-    # remove the zero values so that it is still possible to take
-    # the logarithm. The logarithm acts as a non linear filter
-    # which decrease the noise in the dft and enhances the
-    # prominent frequencies.
-    indicies = np.where(dft_y > 0.0)
-
-    dft_x_red = dft_x[indicies]
-    dft_y_red = dft_y[indicies]
-
-    frequency_max = np.abs(dft_x_red[np.log(dft_y_red).argmax()])
-
-    # find minimal distance to the next meas point in the corresponding time value>
-    diff_array = np.ediff1d(x_axis)
-    min_x_diff = diff_array.min()
-
-    # if at least two identical values are in the array, then the difference is of course zero,
-    # catch that case.
-    for tries, diff_array_step in enumerate(diff_array):
-        if np.isclose(min_x_diff, 0.0, atol=1e-12):
-            index = np.argmin(diff_array)
-            diff_array = np.delete(diff_array, index)
-            min_x_diff = diff_array.min()
-
-        else:
-            if len(diff_array) == 0:
-                self.log.error(
-                    'The passed x_axis for the sinus estimation contains the same values!'
-                    ' Cannot do the fit!')
-
-                return -1, params
-            else:
-                min_x_diff = diff_array.min()
-            break
-
-    # How many points are used to sample the estimated frequency with min_x_diff:
-    iter_steps = int(1/(frequency_max*min_x_diff))
-    if iter_steps < 1:
-        iter_steps = 1
-
-    sum_res = np.zeros(iter_steps)
-
-    # Procedure: Create sin waves with different phases and perform a summation.
-    #            The sum shows how well the sine was fitting to the actual data.
-    #            The best fitting sine should be a maximum of the summed time
-    #            trace.
-
-    for iter_s in range(iter_steps):
-        func_val = ampl_val * np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps*2*np.pi)
-        sum_res[iter_s] = np.abs(data - func_val).sum()
-
-    # The minimum indicates where the sine function was fitting the worst,
-    # therefore subtract pi. This will also ensure that the estimated phase will
-    # be in the interval [-pi,pi].
-    phase = sum_res.argmax()/iter_steps *2*np.pi - np.pi
-
-    # values and bounds of initial parameters
-    params['amplitude'].set(value=ampl_val)
-    params['frequency'].set(value=frequency_max, min=0.0, max=1/stepsize*3)
-    params['phase'].set(value=phase, min=-np.pi, max=np.pi)
-
-    return error, params
-
-
-################################################################################
-#                                                                              #
-#              Fitting methods and their estimators                            #
-#                                                                              #
-################################################################################
-
-########
-# Sine #
-########
-
-def make_sine_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a sine fit with a constant offset on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-
-    sine, params = self.make_sine_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = sine.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = sine.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.error('The sine fit did not work.\n'
-                       'Error message: {0}\n'.format(result.message))
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()
-
-    period = 1 / result.params['frequency'].value
-    try:
-        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
-    except ZeroDivisionError:
-        period_err = np.inf
-
-    result_str_dict['Period'] = {'value': period if period else 0.0,
-                                 'error': period_err if period_err else 0.0,
-                                 'unit': units[0]}
-
-    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
-                                    'error': result.params['frequency'].stderr,
-                                    'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
-                                'error': 180/np.pi*result.params['phase'].stderr,
-                                'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error':  result.params['amplitude'].stderr,
-                                    'unit': units[1]}
-
-    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
-                                   'error':  (np.abs((2*result.params['amplitude'].value) /
-                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
-                                             result.params['amplitude'].stderr))*100,
-                                   'unit': '%'}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sine(self, x_axis, data, params):
-    """ Provides an estimator to obtain initial values for sine fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # set the offset as the average of the data
-    offset = np.average(data)
-
-    # level data
-    data_level = data - offset
-
-    error, params = self.estimate_sinewithoutoffset(x_axis=x_axis, data=data_level, params=params)
-
-    params['offset'].set(value=offset)
-
-    return error, params
-
-##########################
-# Sine exponential decay #
-##########################
-
-
-def make_sineexponentialdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a sine exponential decay fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    sine_exp_decay_offset, params = self.make_sineexponentialdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-
-        result = sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.error('The sineexponentialdecayoffset fit did not work.\n'
-                       'Error message: {0}'.format(result.message))
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()
-
-    period = 1/result.params['frequency'].value
-    try:
-        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
-    except ZeroDivisionError:
-        period_err = np.inf
-
-    result_str_dict['Period'] = {'value': period if period else 0.0,
-                                 'error': period_err if period_err else 0.0,
-                                 'unit': units[0]}
-
-    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
-                                    'error': result.params['frequency'].stderr,
-                                    'unit': 'Hz' if units[0] == 's' else '1/'+units[0]}
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error': result.params['amplitude'].stderr,
-                                    'unit': units[1]}
-
-    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
-                                   'error':  (np.abs((2*result.params['amplitude'].value) /
-                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
-                                             result.params['amplitude'].stderr))*100,
-                                   'unit': '%'}
-
-    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
-                                'error': 180/np.pi*result.params['phase'].stderr,
-                                'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}
-
-    result_str_dict['Beta'] = {'value': result.params['beta'].value,
-                               'error': result.params['beta'].stderr,
-                               'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sineexponentialdecay(self, x_axis, data, params=None):
-    """ Provide an estimator to obtain initial values for a sine exponential
-        decay with offset function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    # Convert for safety:
-    x_axis = np.array(x_axis)
-    data = np.array(data)
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # set the offset as the mean of the data
-    offset = np.mean(data)
-
-    # level data
-    data_level = data - offset
-
-    # estimate amplitude
-    ampl_val = max(np.abs(data_level.min()), np.abs(data_level.max()))
-
-    dft_x, dft_y = compute_ft(x_axis, data_level, zeropad_num=1)
-
-    stepsize = x_axis[1] - x_axis[0]  # for frequency axis
-
-    frequency_max = np.abs(dft_x[dft_y.argmax()])
-
-    # remove noise
-    a = np.std(dft_y)
-    for i in range(0, len(dft_x)):
-        if dft_y[i] <= a:
-            dft_y[i] = 0
-
-    # calculating the width of the FT peak for the estimation of lifetime
-    s = 0
-    for i in range(0, len(dft_x)):
-        s += dft_y[i]*abs(dft_x[1]-dft_x[0])/max(dft_y)
-    lifetime_val = 0.5/s
-
-    # find minimal distance to the next meas point in the corresponding x value
-    min_x_diff = np.ediff1d(x_axis).min()
-
-    # How many points are used to sample the estimated frequency with min_x_diff:
-    iter_steps = int(1/(frequency_max*min_x_diff))
-    if iter_steps < 1:
-        iter_steps = 1
-
-    sum_res = np.zeros(iter_steps)
-
-    # Procedure: Create sin waves with different phases and perform a summation.
-    #            The sum shows how well the sine was fitting to the actual data.
-    #            The best fitting sine should be a maximum of the summed time
-    #            trace.
-
-    for iter_s in range(iter_steps):
-        func_val = ampl_val * np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps *2*np.pi)
-        sum_res[iter_s] = np.abs(data_level - func_val).sum()
-
-    # The minimum indicates where the sine function was fittng the worst,
-    # therefore subtract pi. This will also ensure that the estimated phase will
-    # be in the interval [-pi,pi].
-    phase = (sum_res.argmax()/iter_steps *2*np.pi - np.pi)%(2*np.pi)
-
-    # values and bounds of initial parameters
-    params['frequency'].set(value=frequency_max,
-                            min=min(0.1 / (x_axis[-1]-x_axis[0]), dft_x[3]),
-                            max=min(0.5 / stepsize, dft_x.max()-abs(dft_x[2]-dft_x[0])))
-    params['phase'].set(value=phase, min=-2*np.pi, max=2*np.pi)
-    params['amplitude'].set(value=ampl_val, min=0)
-    params['offset'].set(value=offset)
-
-    params['lifetime'].set(value=lifetime_val,
-                           min=2*(x_axis[1]-x_axis[0]),
-                           max=1/(abs(dft_x[1]-dft_x[0])*0.5))
-
-    return error, params
-
-###################################################
-# Sinus with stretched exponential decay fitting  #
-###################################################
-
-
-def make_sinestretchedexponentialdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a sine stretched exponential decay fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    sine_stretched_exp_decay, params = self.make_sinestretchedexponentialdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = sine_stretched_exp_decay.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        result = sine_stretched_exp_decay.fit(data, x=x_axis, params=params, **kwargs)
-        self.log.error('The sineexponentialdecay fit did not work.\n'
-                       'Error message: {0}'.format(result.message))
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()
-
-    period = 1 / result.params['frequency'].value
-    try:
-        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
-    except ZeroDivisionError:
-        period_err = np.inf
-
-    result_str_dict['Period'] = {'value': period if period else 0.0,
-                                 'error': period_err if period_err else 0.0,
-                                 'unit': units[0]}
-
-    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
-                                    'error': result.params['frequency'].stderr,
-                                    'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
-                                    'error': result.params['amplitude'].stderr,
-                                    'unit': units[1]}
-
-    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
-                                   'error':  (np.abs((2*result.params['amplitude'].value) /
-                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
-                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
-                                             result.params['amplitude'].stderr))*100,
-                                   'unit': '%'}
-
-    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
-                                'error': 180/np.pi*result.params['phase'].stderr,
-                                'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}
-
-    result_str_dict['Beta'] = {'value': result.params['beta'].value,
-                               'error': result.params['beta'].stderr,
-                               'unit': ''}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinestretchedexponentialdecay(self, x_axis, data, params):
-    """ Provide a estimation of a initial values for a sine stretched exponential decay function.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param Parameters object params: object includes parameter dictionary which can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error, params = self.estimate_sineexponentialdecay(x_axis, data, params)
-    #TODO: estimate the exponent cleaverly! For now, set the initial value to 2
-    #      since the usual values for our cases are between 1 and 3.
-    params['beta'].set(value=2, min=0.0, max=10)
-
-    return error, params
-
-###########################################
-# Sum of two individual Sinus with offset #
-###########################################
-
-
-def make_sinedouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a two sine with offset fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    two_sine_offset, params = self.make_sinedouble_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The twosineexpdecayoffset fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['s1_frequency'].value
-    try:
-        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency'])**2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['s2_frequency'].value
-    try:
-        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency'])**2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
-                                      'error': result.params['s1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
-                                      'error': result.params['s2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
-                                      'error': result.params['s1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
-                                      'error': result.params['s2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    amp_string = 's1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                    'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                   'unit': '%'}
-
-    amp_string = 's2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                             (result.params['offset'].value+result.params[amp_string].value)*100),
-                                   'error':  (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                             (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                             result.params[amp_string].stderr))*100,
-                                   'unit': '%'}
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
-                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
-                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinedouble(self, x_axis, data, params):
-    """ Provides an estimator for initial values of two sines with offset fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make two consecutive
-    # sine offset fits where for the second the first fit is subtracted to
-    # delete the first sine in the data.
-
-    result1 = self.make_sine_fit(x_axis=x_axis, data=data, estimator=self.estimate_sine)
-    data_sub = data - result1.best_fit
-
-    result2 = self.make_sine_fit(x_axis=x_axis, data=data_sub, estimator=self.estimate_sine)
-
-    # Fill the parameter dict:
-    params['s1_amplitude'].set(value=result1.params['amplitude'].value)
-    params['s1_frequency'].set(value=result1.params['frequency'].value)
-    params['s1_phase'].set(value=result1.params['phase'].value)
-
-    params['s2_amplitude'].set(value=result2.params['amplitude'].value)
-    params['s2_frequency'].set(value=result2.params['frequency'].value)
-    params['s2_phase'].set(value=result2.params['phase'].value)
-
-    params['offset'].set(value=data.mean())
-
-    return error, params
-
-################################################################################
-#    Sum of two individual Sinus with offset and single exponential decay      #
-################################################################################
-
-
-def make_sinedoublewithexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a two sine with one exponential decay offset fit on the provided
-        data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    two_sine_exp_decay_offset, params = self.make_sinedoublewithexpdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = two_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The sinedoublewithexpdecay fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = two_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['s1_frequency'].value
-    try:
-        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['s2_frequency'].value
-    try:
-        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
-                                      'error': result.params['s1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
-                                      'error': result.params['s2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
-                                      'error': result.params['s1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
-                                      'error': result.params['s2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    amp_string = 's1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 's2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
-                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
-                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinedoublewithexpdecay(self, x_axis, data, params):
-    """ Provides an estimator for initial values of two sine with offset and
-        exponential decay fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make two consecutive
-    # sine offset fits where for the second the first fit is subtracted to
-    # delete the first sine in the data.
-
-    result1 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data,
-        estimator=self.estimate_sineexponentialdecay)
-    data_sub = data - result1.best_fit
-
-    result2 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub,
-        estimator=self.estimate_sineexponentialdecay)
-
-    # Fill the parameter dict:
-    params['s1_amplitude'].set(value=result1.params['amplitude'].value)
-    params['s1_frequency'].set(value=result1.params['frequency'].value)
-    params['s1_phase'].set(value=result1.params['phase'].value)
-
-    params['s2_amplitude'].set(value=result2.params['amplitude'].value)
-    params['s2_frequency'].set(value=result2.params['frequency'].value)
-    params['s2_phase'].set(value=result2.params['phase'].value)
-
-    lifetime = (result1.params['lifetime'].value + result2.params['lifetime'].value)/2
-    params['lifetime'].set(value=lifetime, min=2*(x_axis[1]-x_axis[0]))
-    params['offset'].set(value=data.mean())
-
-    return error, params
-
-
-###############################################################
-# Sum of two individual Sinus exponential decays (and offset) #
-###############################################################
-# Problem with stderr: x.stderr will always be 0 for this model!
-
-
-def make_sinedoublewithtwoexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a two sine with two exponential decay and offset fit on the
-        provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    two_sine_two_exp_decay_offset, params = self.make_sinedoublewithtwoexpdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = two_sine_two_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The sinedoublewithtwoexpdecay fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = two_sine_two_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['e1_frequency'].value
-    try:
-        period1_err = result.params['e1_frequency'].stderr / (result.params['e1_frequency']) ** 2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['e2_frequency'].value
-    try:
-        period2_err = result.params['e2_frequency'].stderr / (result.params['e2_frequency']) ** 2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['e1_frequency'].value,
-                                      'error': result.params['e1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['e2_frequency'].value,
-                                      'error': result.params['e2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['e1_amplitude'].value,
-                                      'error': result.params['e1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['e2_amplitude'].value,
-                                      'error': result.params['e2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    amp_string = 'e1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 'e2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['e1_phase'].value,
-                                  'error': 180/np.pi*result.params['e1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['e2_phase'].value,
-                                  'error': 180/np.pi*result.params['e2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Lifetime 1'] = {'value': result.params['e1_lifetime'].value,
-                                     'error': result.params['e1_lifetime'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Lifetime 2'] = {'value': result.params['e2_lifetime'].value,
-                                     'error': result.params['e2_lifetime'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinedoublewithtwoexpdecay(self, x_axis, data, params):
-    """ Provides an estimator for initial values of two sine with offset and
-        two exponential decay fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make two consecutive
-    # sine offset fits where for the second the first fit is subtracted to
-    # delete the first sine in the data.
-
-    result1 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data,
-        estimator=self.estimate_sineexponentialdecay)
-    data_sub = data - result1.best_fit
-
-    result2 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub,
-        estimator=self.estimate_sineexponentialdecay)
-
-    # Fill the parameter dict:
-    params['e1_amplitude'].set(value=result1.params['amplitude'].value)
-    params['e1_frequency'].set(value=result1.params['frequency'].value)
-    params['e1_phase'].set(value=result1.params['phase'].value)
-    params['e1_lifetime'].set(value=result1.params['lifetime'].value,
-                              min=2*(x_axis[1]-x_axis[0]))
-
-    params['e2_amplitude'].set(value=result2.params['amplitude'].value)
-    params['e2_frequency'].set(value=result2.params['frequency'].value)
-    params['e2_phase'].set(value=result2.params['phase'].value)
-    params['e2_lifetime'].set(value=result2.params['lifetime'].value,
-                              min=2*(x_axis[1]-x_axis[0]))
-
-    params['offset'].set(value=data.mean())
-
-    return error, params
-
-#############################################
-# Sum of three individual Sinus with offset #
-#############################################
-
-
-def make_sinetriple_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a three sine with offset fit on the provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    two_sine_offset, params = self.make_sinetriple_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The threesineexpdecayoffset fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['s1_frequency'].value
-    try:
-        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['s2_frequency'].value
-    try:
-        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    period3 = 1 / result.params['s3_frequency'].value
-    try:
-        period3_err = result.params['s3_frequency'].stderr / (result.params['s3_frequency']) ** 2
-    except ZeroDivisionError:
-        period3_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
-                                   'error': period3_err if period3_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
-                                      'error': result.params['s1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
-                                      'error': result.params['s2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 3'] = {'value': result.params['s3_frequency'].value,
-                                      'error': result.params['s3_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
-                                      'error': result.params['s1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
-                                      'error': result.params['s2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 3'] = {'value': result.params['s3_amplitude'].value,
-                                      'error': result.params['s3_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    amp_string = 's1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 's2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 's3_amplitude'
-    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
-                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
-                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['s3_phase'].value,
-                                  'error': 180/np.pi*result.params['s3_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinetriple(self, x_axis, data, params):
-    """ Provides an estimator for initial values of three sines with offset fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make three consecutive
-    # sine offset fits where for the next fit the previous is subtracted to
-    # delete its contribution in the data.
-
-    res1 = self.make_sine_fit(x_axis=x_axis, data=data, estimator=self.estimate_sine)
-    data_sub1 = data - res1.best_fit
-
-    res2 = self.make_sine_fit(x_axis=x_axis, data=data_sub1, estimator=self.estimate_sine)
-    data_sub2 = data_sub1 - res2.best_fit
-
-    res3 = self.make_sine_fit(x_axis=x_axis, data=data_sub2, estimator=self.estimate_sine)
-
-    # Fill the parameter dict:
-    params['s1_amplitude'].set(value=res1.params['amplitude'].value)
-    params['s1_frequency'].set(value=res1.params['frequency'].value)
-    params['s1_phase'].set(value=res1.params['phase'].value)
-
-    params['s2_amplitude'].set(value=res2.params['amplitude'].value)
-    params['s2_frequency'].set(value=res2.params['frequency'].value)
-    params['s2_phase'].set(value=res2.params['phase'].value)
-
-    params['s3_amplitude'].set(value=res3.params['amplitude'].value)
-    params['s3_frequency'].set(value=res3.params['frequency'].value)
-    params['s3_phase'].set(value=res3.params['phase'].value)
-
-    params['offset'].set(value=data.mean())
-
-    return error, params
-
-##########################################################################
-# Sum of three individual Sinus with offset and single exponential decay #
-##########################################################################
-
-
-def make_sinetriplewithexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a three sine with one exponential decay offset fit on the provided
-        data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    three_sine_exp_decay_offset, params = self.make_sinetriplewithexpdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params, update_params=add_params)
-    try:
-        result = three_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The sinetriplewithexpdecay fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = three_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['s1_frequency'].value
-    try:
-        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['s2_frequency'].value
-    try:
-        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    period3 = 1 / result.params['s3_frequency'].value
-    try:
-        period3_err = result.params['s3_frequency'].stderr / (result.params['s3_frequency']) ** 2
-    except ZeroDivisionError:
-        period3_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
-                                   'error': period3_err if period3_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
-                                      'error': result.params['s1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
-                                      'error': result.params['s2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 3'] = {'value': result.params['s3_frequency'].value,
-                                      'error': result.params['s3_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
-                                      'error': result.params['s1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
-                                      'error': result.params['s2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 3'] = {'value': result.params['s3_amplitude'].value,
-                                      'error': result.params['s3_amplitude'].stderr,
-                                      'unit': units[1]}
-
-
-    amp_string = 's1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 's2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 's3_amplitude'
-    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
-                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
-                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['s3_phase'].value,
-                                  'error': 180/np.pi*result.params['s3_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
-                                   'error': result.params['lifetime'].stderr,
-                                   'unit': units[0]}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinetriplewithexpdecay(self, x_axis, data, params):
-    """ Provides an estimator for initial values of three sine with offset and
-        exponential decay fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make three consecutive
-    # sine exponential decay with offset fits where for the next fit the
-    # previous is subtracted to delete its contribution in the data.
-
-    res1 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data,
-        estimator=self.estimate_sineexponentialdecay)
-
-    data_sub1 = data - res1.best_fit
-
-    res2 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub1,
-        estimator=self.estimate_sineexponentialdecay)
-
-    data_sub2 = data_sub1 - res2.best_fit
-
-    res3 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub2,
-        estimator=self.estimate_sineexponentialdecay)
-
-    # Fill the parameter dict:
-    params['s1_amplitude'].set(value=res1.params['amplitude'].value)
-    params['s1_frequency'].set(value=res1.params['frequency'].value)
-    params['s1_phase'].set(value=res1.params['phase'].value)
-
-    params['s2_amplitude'].set(value=res2.params['amplitude'].value)
-    params['s2_frequency'].set(value=res2.params['frequency'].value)
-    params['s2_phase'].set(value=res2.params['phase'].value)
-
-    params['s3_amplitude'].set(value=res3.params['amplitude'].value)
-    params['s3_frequency'].set(value=res3.params['frequency'].value)
-    params['s3_phase'].set(value=res3.params['phase'].value)
-
-    lifetime = (res1.params['lifetime'].value + res2.params['lifetime'].value + res3.params['lifetime'].value)/3
-    params['lifetime'].set(value=lifetime,
-                           min=2*(x_axis[1]-x_axis[0]))
-    params['offset'].set(value=data.mean())
-
-    return error, params
-
-#########################################################################
-# Sum of three individual Sinus with offset and three exponential decay #
-#########################################################################
-
-
-def make_sinetriplewiththreeexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
-    """ Perform a three sine with three exponential decay and offset fit on the
-        provided data.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param method estimator: Pointer to the estimator method
-    @param list units: List containing the ['horizontal', 'vertical'] units as strings
-    @param Parameters or dict add_params: optional, additional parameters of
-                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
-                which will be used instead of the values from the estimator.
-
-    @return object result: lmfit.model.ModelFit object, all parameters
-                           provided about the fitting, like: success,
-                           initial fitting values, best fitting values, data
-                           with best fit with given axis,...
-    """
-    three_sine_three_exp_decay_offset, params = self.make_sinetriplewiththreeexpdecay_model()
-
-    error, params = estimator(x_axis, data, params)
-
-    params = self._substitute_params(initial_params=params,
-                                     update_params=add_params)
-    try:
-        result = three_sine_three_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-    except:
-        self.log.warning('The twosinetwoexpdecayoffset fit did not work. '
-                         'Error message: {}'.format(str(result.message)))
-        result = three_sine_three_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
-
-    if units is None:
-        units = ['arb. unit', 'arb. unit']
-
-    result_str_dict = dict()  # create result string for gui or OrderedDict()
-
-    period1 = 1 / result.params['e1_frequency'].value
-    try:
-        period1_err = result.params['e1_frequency'].stderr / (result.params['e1_frequency']) ** 2
-    except ZeroDivisionError:
-        period1_err = np.inf
-
-    period2 = 1 / result.params['e2_frequency'].value
-    try:
-        period2_err = result.params['e2_frequency'].stderr / (result.params['e2_frequency']) ** 2
-    except ZeroDivisionError:
-        period2_err = np.inf
-
-    period3 = 1 / result.params['e3_frequency'].value
-    try:
-        period3_err = result.params['e3_frequency'].stderr / (result.params['e3_frequency']) ** 2
-    except ZeroDivisionError:
-        period3_err = np.inf
-
-    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
-                                   'error': period1_err if period1_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
-                                   'error': period2_err if period2_err else 0.0,
-                                   'unit': units[0]}
-    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
-                                   'error': period3_err if period3_err else 0.0,
-                                   'unit': units[0]}
-
-    result_str_dict['Frequency 1'] = {'value': result.params['e1_frequency'].value,
-                                      'error': result.params['e1_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 2'] = {'value': result.params['e2_frequency'].value,
-                                      'error': result.params['e2_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Frequency 3'] = {'value': result.params['e3_frequency'].value,
-                                      'error': result.params['e3_frequency'].stderr,
-                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
-
-    result_str_dict['Amplitude 1'] = {'value': result.params['e1_amplitude'].value,
-                                      'error': result.params['e1_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 2'] = {'value': result.params['e2_amplitude'].value,
-                                      'error': result.params['e2_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    result_str_dict['Amplitude 3'] = {'value': result.params['e3_amplitude'].value,
-                                      'error': result.params['e3_amplitude'].stderr,
-                                      'unit': units[1]}
-
-    amp_string = 'e1_amplitude'
-    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 'e2_amplitude'
-    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-    amp_string = 'e3_amplitude'
-    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
-                                               (result.params['offset'].value+result.params[amp_string].value)*100),
-                                     'error': (np.abs((2*result.params[amp_string].value) /
-                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
-                                             result.params['offset'].stderr) +
-                                             np.abs((2/(result.params['offset'].value +
-                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
-                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
-                                               result.params[amp_string].stderr))*100,
-                                     'unit': '%'}
-
-
-    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['e1_phase'].value,
-                                  'error': 180/np.pi*result.params['e1_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['e2_phase'].value,
-                                  'error': 180/np.pi*result.params['e2_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['e3_phase'].value,
-                                  'error': 180/np.pi*result.params['e3_phase'].stderr,
-                                  'unit': 'deg'}
-
-    result_str_dict['Lifetime 1'] = {'value': result.params['e1_lifetime'].value,
-                                     'error': result.params['e1_lifetime'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Lifetime 2'] = {'value': result.params['e2_lifetime'].value,
-                                     'error': result.params['e2_lifetime'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Lifetime 3'] = {'value': result.params['e3_lifetime'].value,
-                                     'error': result.params['e3_lifetime'].stderr,
-                                     'unit': units[0]}
-
-    result_str_dict['Offset'] = {'value': result.params['offset'].value,
-                                 'error': result.params['offset'].stderr,
-                                 'unit': units[1]}
-
-    result.result_str_dict = result_str_dict
-    return result
-
-
-def estimate_sinetriplewiththreeexpdecay(self, x_axis, data, params):
-    """ Provides an estimator for initial values of three sine with offset and
-        three exponential decay fitting.
-
-    @param numpy.array x_axis: 1D axis values
-    @param numpy.array data: 1D data, should have the same dimension as x_axis.
-    @param lmfit.Parameters params: object includes parameter dictionary which
-                                    can be set
-
-    @return tuple (error, params):
-
-    Explanation of the return parameter:
-        int error: error code (0:OK, -1:error)
-        Parameters object params: set parameters of initial values
-    """
-
-    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
-
-    # That procedure seems to work extremely reliable: make two consecutive
-    # sine offset fits where for the second the first fit is subtracted to
-    # delete the first sine in the data.
-
-    res1 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data,
-        estimator=self.estimate_sineexponentialdecay)
-    data_sub1 = data - res1.best_fit
-
-    res2 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub1,
-        estimator=self.estimate_sineexponentialdecay)
-    data_sub2 = data_sub1 - res2.best_fit
-
-    res3 = self.make_sineexponentialdecay_fit(
-        x_axis=x_axis,
-        data=data_sub2,
-        estimator=self.estimate_sineexponentialdecay)
-
-    # Fill the parameter dict:
-    params['e1_amplitude'].set(value=res1.params['amplitude'].value)
-    params['e1_frequency'].set(value=res1.params['frequency'].value)
-    params['e1_phase'].set(value=res1.params['phase'].value)
-    params['e1_lifetime'].set(value=res1.params['lifetime'].value,
-                              min=2*(x_axis[1]-x_axis[0]))
-
-    params['e2_amplitude'].set(value=res2.params['amplitude'].value)
-    params['e2_frequency'].set(value=res2.params['frequency'].value)
-    params['e2_phase'].set(value=res2.params['phase'].value)
-    params['e2_lifetime'].set(value=res2.params['lifetime'].value,
-                              min=2*(x_axis[1]-x_axis[0]))
-
-    params['e3_amplitude'].set(value=res3.params['amplitude'].value)
-    params['e3_frequency'].set(value=res3.params['frequency'].value)
-    params['e3_phase'].set(value=res3.params['phase'].value)
-    params['e3_lifetime'].set(value=res3.params['lifetime'].value,
-                              min=2*(x_axis[1]-x_axis[0]))
-
-    params['offset'].set(value=data.mean())
-
-    return error, params
+# -*- coding: utf-8 -*-
+"""
+This file contains methods for sine fitting, these methods
+are imported by class FitLogic.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+import numpy as np
+from lmfit.models import Model
+from scipy import signal
+
+
+def get_ft_windows():
+    """ Retrieve the available windows to be applied on signal data before FT.
+
+    @return: dict with keys being the window name and items being again a dict
+             containing the actual function and the normalization factor to
+             calculate correctly the amplitude spectrum in the Fourier Transform
+
+    To find out the amplitude normalization factor check either the scipy
+    implementation on
+        https://github.com/scipy/scipy/blob/v0.15.1/scipy/signal/windows.py#L336
+    or just perform a sum of the window (oscillating parts of the window should
+    be averaged out and constant offset factor will remain):
+        MM=1000000  # choose a big number
+        print(sum(signal.hanning(MM))/MM)
+    """
+
+    win = {'none': {'func': np.ones, 'ampl_norm': 1.0},
+           'hamming': {'func': signal.hamming, 'ampl_norm': 1.0/0.54},
+           'hann': {'func': signal.hann, 'ampl_norm': 1.0/0.5},
+           'blackman': {'func': signal.blackman, 'ampl_norm': 1.0/0.42},
+           'triang': {'func': signal.triang, 'ampl_norm': 1.0/0.5},
+           'flattop': {'func': signal.flattop, 'ampl_norm': 1.0/0.2156},
+           'bartlett': {'func': signal.bartlett, 'ampl_norm': 1.0/0.5},
+           'parzen': {'func': signal.parzen, 'ampl_norm': 1.0/0.375},
+           'bohman': {'func': signal.bohman, 'ampl_norm': 1.0/0.4052847},
+           'blackmanharris': {'func': signal.blackmanharris, 'ampl_norm': 1.0/0.35875},
+           'nuttall': {'func': signal.nuttall, 'ampl_norm': 1.0/0.3635819},
+           'barthann': {'func': signal.barthann, 'ampl_norm': 1.0/0.5}}
+    return win
+
+
+def compute_ft(x_val, y_val, zeropad_num=0, window='none', base_corr=True, psd=False):
+    """ Compute the Discrete fourier Transform of the power spectral density
+
+    @param numpy.array x_val: 1D array
+    @param numpy.array y_val: 1D array of same size as x_val
+    @param int zeropad_num: optional, zeropadding (adding zeros to the end of
+                            the array). zeropad_num >= 0, the size of the array
+                            which is add to the end of the y_val before
+                            performing the Fourier Transform (FT). The
+                            resulting array will have the length
+                                (len(y_val)/2)*(zeropad_num+1)
+                            Note that zeropadding will not change or add more
+                            information to the dft, it will solely interpolate
+                            between the dft_y values (corresponds to a Sinc
+                            interpolation method).
+                            Set zeropad_num=1 to obtain output arrays which
+                            have the same size as the input arrays.
+                            Default is zeropad_num=0.
+    @param str window: optional, the window function which should be applied to
+                       the y values before Fourier Transform is calculated.
+    @param bool base_corr: Select whether baseline correction shoud be performed
+                           before calculating the FT.
+    @param bool psd: optional, select whether the Discrete Fourier Transform or
+                     the Power Spectral Density (PSD, which is just the FT of
+                     the absolute square of the y-values) should be computed.
+                     Default is psd=False.
+
+    @return: tuple(dft_x, dft_y):
+                be aware that the return arrays' length depend on the zeropad
+                number like
+                    len(dft_x) = len(dft_y) = (len(y_val)/2)*(zeropad_num+1)
+
+    Pay attention that the return values of the FT have only half of the
+    entries compared to the used signal input (if zeropad=0).
+
+    In general, a window function should be applied on the y data before
+    calculating the FT, to reduce spectral leakage. The Hann window for
+    instance is almost never a bad choice. Use it like window='hann'
+
+    Keep always in mind the relation to the Fourier transform space:
+        T = delta_t * N_samples
+    where delta_t is the distance between the time points and N_samples are the
+    amount of points in the time domain. Consequently the sample rate is
+        f_samplerate = T / N_samples
+
+    Keep also in mind that the FT returns value from 0 to f_samplerate, or
+        equivalently -f_samplerate/2 to f_samplerate/2.
+
+    Difference between PSD and DFT:
+    The power spectral density (PSD) describes how the power of your signal is
+    distributed over frequency whilst the DFT shows the spectral content of
+    your signal, i.e. the amplitude and phase of harmonics in your signal.
+    """
+
+    avail_windows = get_ft_windows()
+
+    x_val = np.array(x_val)
+    y_val = np.array(y_val)
+
+    # Make a baseline correction to avoid a constant offset near zero
+    # frequencies. Offset of the y_val from mean corresponds to half the value
+    # at fft_y[0].
+    corrected_y = y_val
+    if base_corr:
+        corrected_y = y_val - y_val.mean()
+
+    ampl_norm_fact = 1.0
+    # apply window to data to account for spectral leakage:
+    if window in avail_windows:
+        window_val = avail_windows[window]['func'](len(y_val))
+        corrected_y = corrected_y * window_val
+        # to get the correct amplitude in the amplitude spectrum
+        ampl_norm_fact = avail_windows[window]['ampl_norm']
+
+    # zeropad for sinc interpolation:
+    zeropad_arr = np.zeros(len(corrected_y)*(zeropad_num+1))
+    zeropad_arr[:len(corrected_y)] = corrected_y
+
+    # Get the amplitude values from the fourier transformed y values.
+    fft_y = np.abs(np.fft.fft(zeropad_arr))
+
+    # Power spectral density (PSD) or just amplitude spectrum of fourier signal:
+    power_value = 1.0
+    if psd:
+        power_value = 2.0
+
+    # The factor 2 accounts for the fact that just the half of the spectrum was
+    # taken. The ampl_norm_fact is the normalization factor due to the applied
+    # window function (the offset value in the window function):
+    fft_y = ((2/len(y_val)) * fft_y * ampl_norm_fact)**power_value
+
+    # Due to the sampling theorem you can only identify frequencies at half
+    # of the sample rate, therefore the FT contains an almost symmetric
+    # spectrum (the asymmetry results from aliasing effects). Therefore take
+    # the half of the values for the display.
+    middle = int((len(zeropad_arr)+1)//2)
+
+    # sample spacing of x_axis, if x is a time axis than it corresponds to a
+    # timestep:
+    x_spacing = np.round(x_val[-1] - x_val[-2], 12)
+
+    # use the helper function of numpy to calculate the x_values for the
+    # fourier space. That function will handle an occuring devision by 0:
+    fft_x = np.fft.fftfreq(len(zeropad_arr), d=x_spacing)
+
+    return abs(fft_x[:middle]), fft_y[:middle]
+
+
+################################################################################
+#                                                                              #
+#                               Defining Sine models                           #
+#                                                                              #
+################################################################################
+
+##################################################
+# Bare sine with unitary amplitude and no offset #
+##################################################
+
+def make_baresine_model(self, prefix=None):
+    """ Create a bare sine model without amplitude and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params)
+
+    Explanation of the objects:
+        object lmfit.model.CompositeModel model:
+            A model the lmfit module will use for that fit. Here a
+            gaussian model. Returns an object of the class
+            lmfit.model.CompositeModel.
+
+        object lmfit.parameter.Parameters params:
+            It is basically an OrderedDict, so a dictionary, with keys
+            denoting the parameters as string names and values which are
+            lmfit.parameter.Parameter (without s) objects, keeping the
+            information about the current value.
+
+        For further information have a look in:
+    http://cars9.uchicago.edu/software/python/lmfit/builtin_models.html#models.GaussianModel
+    """
+
+    def bare_sine_function(x, frequency, phase):
+        """ Function of a bare sine.
+
+        @param numpy.array x: independant variable - e.g. time
+        @param float frequency: frequency
+        @param float phase: phase
+
+        @return: reference to method of a sine function in order to use it as a
+                 model
+        """
+
+        return np.sin(2*np.pi*frequency*x+phase)
+
+    if not isinstance(prefix, str) and prefix is not None:
+        self.log.error('The passed prefix <{0}> of type {1} is not a string and'
+                       'cannot be used as a prefix and will be ignored for now.'
+                       'Correct that!'.format(prefix, type(prefix)))
+        model = Model(bare_sine_function, independent_vars=['x'])
+    else:
+        model = Model(bare_sine_function, independent_vars=['x'], prefix=prefix)
+
+    params = model.make_params()
+
+    return model, params
+
+###############################
+# Centred sine with no offset #
+###############################
+
+
+def make_sinewithoutoffset_model(self, prefix=None):
+    """ Create a model of sine with an amplitude.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+    baresine_model, params = self.make_baresine_model(prefix=prefix)
+    amplitude_model, params = self.make_amplitude_model(prefix=prefix)
+
+    sine_model = amplitude_model*baresine_model
+    params = sine_model.make_params()
+
+    return sine_model, params
+
+############################
+# General sine with offset #
+############################
+
+
+def make_sine_model(self, prefix=None):
+    """ Create a sine model with amplitude and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    sine_offset_model = sine_model + constant_model
+    params = sine_offset_model.make_params()
+
+    return sine_offset_model, params
+
+###############################################
+# Sinus with exponential decay but not offset #
+###############################################
+
+
+def make_sineexpdecaywithoutoffset_model(self, prefix=None):
+    """ Create a model of a sine with exponential decay.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
+    bareexponentialdecay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
+
+    sine_exp_decay_model = sine_model*bareexponentialdecay_model
+    params = sine_exp_decay_model.make_params()
+
+    return sine_exp_decay_model, params
+
+###################################################
+# Sinus with exponential decay and offset fitting #
+###################################################
+
+def make_sineexponentialdecay_model(self, prefix=None):
+    """ Create a model of a sine with exponential decay and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    sine_exp_decay_model, params = self.make_sineexpdecaywithoutoffset_model(prefix=prefix)
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    sine_exp_decay_offset_model = sine_exp_decay_model + constant_model
+    params = sine_exp_decay_offset_model.make_params()
+
+    return sine_exp_decay_offset_model, params
+
+###################################################
+# Sinus with stretched exponential decay fitting  #
+###################################################
+
+def make_sinestretchedexponentialdecay_model(self, prefix=None):
+    """ Create a model of a sine with stretched exponential decay.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    sine_model, params = self.make_sinewithoutoffset_model(prefix=prefix)
+    bare_stretched_exp_decay_model, params = self.make_barestretchedexponentialdecay_model(prefix=prefix)
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    model = sine_model * bare_stretched_exp_decay_model + constant_model
+    params = model.make_params()
+
+    return model, params
+
+###########################################
+# Sum of two individual Sinus with offset #
+###########################################
+
+
+def make_sinedouble_model(self, prefix=None):
+    """ Create a model of two summed sine with an offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
+    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    two_sine_offset = sine_model1 + sine_model2 + constant_model
+    params = two_sine_offset.make_params()
+
+    return two_sine_offset, params
+
+################################################################################
+#    Sum of two individual Sinus with offset and single exponential decay      #
+################################################################################
+
+
+def make_sinedoublewithexpdecay_model(self, prefix=None):
+    """ Create a model of two summed sine with an exponential decay and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
+    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
+    bare_exp_decay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    two_sine_exp_decay_offset = (sine_model1 + sine_model2)*bare_exp_decay_model + constant_model
+    params = two_sine_exp_decay_offset.make_params()
+
+    return two_sine_exp_decay_offset, params
+
+###############################################################
+# Sum of two individual Sinus exponential decays (and offset) #
+###############################################################
+
+
+def make_sinedoublewithtwoexpdecay_model(self, prefix=None):
+    """ Create a model of two summed sine with three exponential decays and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_exp_decay_model1, params = self.make_sineexpdecaywithoutoffset_model(prefix='e1_'+add_text)
+    sine_exp_decay_model2, params = self.make_sineexpdecaywithoutoffset_model(prefix='e2_'+add_text)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    sinedoublewithtwoexpdecay = sine_exp_decay_model1 + sine_exp_decay_model2 + constant_model
+    params = sinedoublewithtwoexpdecay.make_params()
+
+    return sinedoublewithtwoexpdecay, params
+
+#############################################
+# Sum of three individual Sinus with offset #
+#############################################
+
+
+def make_sinetriple_model(self, prefix=None):
+    """ Create a model of three summed sine with an offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
+    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
+    sine_model3, params = self.make_sinewithoutoffset_model(prefix='s3_'+add_text)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    three_sine_offset = sine_model1 + sine_model2 + sine_model3 + constant_model
+    params = three_sine_offset.make_params()
+
+    return three_sine_offset, params
+
+##########################################################################
+# Sum of three individual Sinus with offset and single exponential decay #
+##########################################################################
+
+
+def make_sinetriplewithexpdecay_model(self, prefix=None):
+    """ Create a model of three summed sine with an exponential decay and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_model1, params = self.make_sinewithoutoffset_model(prefix='s1_'+add_text)
+    sine_model2, params = self.make_sinewithoutoffset_model(prefix='s2_'+add_text)
+    sine_model3, params = self.make_sinewithoutoffset_model(prefix='s3_'+add_text)
+    bare_exp_decay_model, params = self.make_bareexponentialdecay_model(prefix=prefix)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    three_sine_exp_decay_offset = (
+        sine_model1 + sine_model2 + sine_model3) * bare_exp_decay_model + constant_model
+    params = three_sine_exp_decay_offset.make_params()
+
+    return three_sine_exp_decay_offset, params
+
+#########################################################################
+# Sum of three individual Sinus with offset and three exponential decay #
+#########################################################################
+
+
+def make_sinetriplewiththreeexpdecay_model(self, prefix=None):
+    """ Create a model of three summed sine with three exponential decays and offset.
+
+    @param str prefix: optional, if multiple models should be used in a
+                       composite way and the parameters of each model should be
+                       distinguished from each other to prevent name collisions.
+
+    @return tuple: (object model, object params), for more description see in
+                   the method make_baresine_model.
+    """
+
+    if prefix is None:
+        add_text = ''
+    else:
+        add_text = prefix
+
+    sine_exp_decay_model1, params = self.make_sineexpdecaywithoutoffset_model(prefix='e1_'+add_text)
+    sine_exp_decay_model2, params = self.make_sineexpdecaywithoutoffset_model(prefix='e2_'+add_text)
+    sine_exp_decay_model3, params = self.make_sineexpdecaywithoutoffset_model(prefix='e3_'+add_text)
+
+    constant_model, params = self.make_constant_model(prefix=prefix)
+
+    three_sine_exp_decay_offset = sine_exp_decay_model1 + sine_exp_decay_model2 + sine_exp_decay_model3 + constant_model
+    params = three_sine_exp_decay_offset.make_params()
+
+    return three_sine_exp_decay_offset, params
+
+################################################################################
+#                                                                              #
+#                        General estimators used later                         #
+#                                                                              #
+################################################################################
+
+
+def estimate_baresine(self, x_axis, data, params):
+    """ Bare sine estimator with a frequency and phase.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        lmfit.Parameters params: derived OrderedDict object contains the initial
+                                 values for the fit.
+    """
+
+    # Convert for safety:
+    x_axis = np.array(x_axis)
+    data = np.array(data)
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # calculate dft with zeropadding to obtain nicer interpolation between the
+    # appearing peaks.
+    dft_x, dft_y = compute_ft(x_axis, data, zeropad_num=1)
+
+    stepsize = x_axis[1]-x_axis[0]  # for frequency axis
+    frequency_max = np.abs(dft_x[np.log(dft_y).argmax()])
+
+    # find minimal distance to the next meas point in the corresponding time value>
+    min_x_diff = np.ediff1d(x_axis).min()
+
+    # How many points are used to sample the estimated frequency with min_x_diff:
+    iter_steps = int(1/(frequency_max*min_x_diff))
+    if iter_steps < 1:
+        iter_steps = 1
+
+    sum_res = np.zeros(iter_steps)
+
+    # Procedure: Create sin waves with different phases and perform a summation.
+    #            The sum shows how well the sine was fitting to the actual data.
+    #            The best fitting sine should be a maximum of the summed time
+    #            trace.
+
+    for iter_s in range(iter_steps):
+        func_val = np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps *2*np.pi)
+        sum_res[iter_s] = np.abs(data - func_val).sum()
+
+    # The minimum indicates where the sine function was fittng the worst,
+    # therefore subtract pi. This will also ensure that the estimated phase will
+    # be in the interval [-pi,pi].
+    phase = sum_res.argmax()/iter_steps *2*np.pi - np.pi
+
+    params['frequency'].set(value=frequency_max, min=0.0, max=1/stepsize*3)
+    params['phase'].set(value=phase, min=-np.pi, max=np.pi)
+
+    return error, params
+
+
+def estimate_sinewithoutoffset(self, x_axis, data, params):
+    """ Sine estimator, with an amplitude, frequency and phase.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        lmfit.Parameters params: derived OrderedDict object contains the initial
+                                 values for the fit.
+    """
+
+    # Convert for safety:
+    x_axis = np.array(x_axis)
+    data = np.array(data)
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # sort the input
+    sorted_indices = x_axis.argsort()
+    x_axis = x_axis[sorted_indices]
+    data = data[sorted_indices]
+
+    # estimate amplitude
+    ampl_val = max(np.abs(data.min()), np.abs(data.max()))
+
+    # calculate dft with zeropadding to obtain nicer interpolation between the
+    # appearing peaks.
+    dft_x, dft_y = compute_ft(x_axis, data, zeropad_num=1)
+
+    stepsize = x_axis[1] - x_axis[0]  # for frequency axis
+
+    # remove the zero values so that it is still possible to take
+    # the logarithm. The logarithm acts as a non linear filter
+    # which decrease the noise in the dft and enhances the
+    # prominent frequencies.
+    indicies = np.where(dft_y > 0.0)
+
+    dft_x_red = dft_x[indicies]
+    dft_y_red = dft_y[indicies]
+
+    frequency_max = np.abs(dft_x_red[np.log(dft_y_red).argmax()])
+
+    # find minimal distance to the next meas point in the corresponding time value>
+    diff_array = np.ediff1d(x_axis)
+    min_x_diff = diff_array.min()
+
+    # if at least two identical values are in the array, then the difference is of course zero,
+    # catch that case.
+    for tries, diff_array_step in enumerate(diff_array):
+        if np.isclose(min_x_diff, 0.0, atol=1e-12):
+            index = np.argmin(diff_array)
+            diff_array = np.delete(diff_array, index)
+            min_x_diff = diff_array.min()
+
+        else:
+            if len(diff_array) == 0:
+                self.log.error(
+                    'The passed x_axis for the sinus estimation contains the same values!'
+                    ' Cannot do the fit!')
+
+                return -1, params
+            else:
+                min_x_diff = diff_array.min()
+            break
+
+    # How many points are used to sample the estimated frequency with min_x_diff:
+    iter_steps = int(1/(frequency_max*min_x_diff))
+    if iter_steps < 1:
+        iter_steps = 1
+
+    sum_res = np.zeros(iter_steps)
+
+    # Procedure: Create sin waves with different phases and perform a summation.
+    #            The sum shows how well the sine was fitting to the actual data.
+    #            The best fitting sine should be a maximum of the summed time
+    #            trace.
+
+    for iter_s in range(iter_steps):
+        func_val = ampl_val * np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps*2*np.pi)
+        sum_res[iter_s] = np.abs(data - func_val).sum()
+
+    # The minimum indicates where the sine function was fitting the worst,
+    # therefore subtract pi. This will also ensure that the estimated phase will
+    # be in the interval [-pi,pi].
+    phase = sum_res.argmax()/iter_steps *2*np.pi - np.pi
+
+    # values and bounds of initial parameters
+    params['amplitude'].set(value=ampl_val)
+    params['frequency'].set(value=frequency_max, min=0.0, max=1/stepsize*3)
+    params['phase'].set(value=phase, min=-np.pi, max=np.pi)
+
+    return error, params
+
+
+################################################################################
+#                                                                              #
+#              Fitting methods and their estimators                            #
+#                                                                              #
+################################################################################
+
+########
+# Sine #
+########
+
+def make_sine_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a sine fit with a constant offset on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+
+    sine, params = self.make_sine_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = sine.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = sine.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.error('The sine fit did not work.\n'
+                       'Error message: {0}\n'.format(result.message))
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()
+
+    period = 1 / result.params['frequency'].value
+    try:
+        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
+    except ZeroDivisionError:
+        period_err = np.inf
+
+    result_str_dict['Period'] = {'value': period if period else 0.0,
+                                 'error': period_err if period_err else 0.0,
+                                 'unit': units[0]}
+
+    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
+                                    'error': result.params['frequency'].stderr,
+                                    'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
+                                'error': 180/np.pi*result.params['phase'].stderr,
+                                'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error':  result.params['amplitude'].stderr,
+                                    'unit': units[1]}
+
+    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
+                                   'error':  (np.abs((2*result.params['amplitude'].value) /
+                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
+                                             result.params['amplitude'].stderr))*100,
+                                   'unit': '%'}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sine(self, x_axis, data, params):
+    """ Provides an estimator to obtain initial values for sine fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # set the offset as the average of the data
+    offset = np.average(data)
+
+    # level data
+    data_level = data - offset
+
+    error, params = self.estimate_sinewithoutoffset(x_axis=x_axis, data=data_level, params=params)
+
+    params['offset'].set(value=offset)
+
+    return error, params
+
+##########################
+# Sine exponential decay #
+##########################
+
+
+def make_sineexponentialdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a sine exponential decay fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    sine_exp_decay_offset, params = self.make_sineexponentialdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+
+        result = sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.error('The sineexponentialdecayoffset fit did not work.\n'
+                       'Error message: {0}'.format(result.message))
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()
+
+    period = 1/result.params['frequency'].value
+    try:
+        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
+    except ZeroDivisionError:
+        period_err = np.inf
+
+    result_str_dict['Period'] = {'value': period if period else 0.0,
+                                 'error': period_err if period_err else 0.0,
+                                 'unit': units[0]}
+
+    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
+                                    'error': result.params['frequency'].stderr,
+                                    'unit': 'Hz' if units[0] == 's' else '1/'+units[0]}
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error': result.params['amplitude'].stderr,
+                                    'unit': units[1]}
+
+    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
+                                   'error':  (np.abs((2*result.params['amplitude'].value) /
+                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
+                                             result.params['amplitude'].stderr))*100,
+                                   'unit': '%'}
+
+    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
+                                'error': 180/np.pi*result.params['phase'].stderr,
+                                'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}
+
+    result_str_dict['Beta'] = {'value': result.params['beta'].value,
+                               'error': result.params['beta'].stderr,
+                               'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sineexponentialdecay(self, x_axis, data, params=None):
+    """ Provide an estimator to obtain initial values for a sine exponential
+        decay with offset function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    # Convert for safety:
+    x_axis = np.array(x_axis)
+    data = np.array(data)
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # set the offset as the mean of the data
+    offset = np.mean(data)
+
+    # level data
+    data_level = data - offset
+
+    # estimate amplitude
+    ampl_val = max(np.abs(data_level.min()), np.abs(data_level.max()))
+
+    dft_x, dft_y = compute_ft(x_axis, data_level, zeropad_num=1)
+
+    stepsize = x_axis[1] - x_axis[0]  # for frequency axis
+
+    frequency_max = np.abs(dft_x[dft_y.argmax()])
+
+    # remove noise
+    a = np.std(dft_y)
+    for i in range(0, len(dft_x)):
+        if dft_y[i] <= a:
+            dft_y[i] = 0
+
+    # calculating the width of the FT peak for the estimation of lifetime
+    s = 0
+    for i in range(0, len(dft_x)):
+        s += dft_y[i]*abs(dft_x[1]-dft_x[0])/max(dft_y)
+    lifetime_val = 0.5/s
+
+    # find minimal distance to the next meas point in the corresponding x value
+    min_x_diff = np.ediff1d(x_axis).min()
+
+    # How many points are used to sample the estimated frequency with min_x_diff:
+    iter_steps = int(1/(frequency_max*min_x_diff))
+    if iter_steps < 1:
+        iter_steps = 1
+
+    sum_res = np.zeros(iter_steps)
+
+    # Procedure: Create sin waves with different phases and perform a summation.
+    #            The sum shows how well the sine was fitting to the actual data.
+    #            The best fitting sine should be a maximum of the summed time
+    #            trace.
+
+    for iter_s in range(iter_steps):
+        func_val = ampl_val * np.sin(2*np.pi*frequency_max*x_axis + iter_s/iter_steps *2*np.pi)
+        sum_res[iter_s] = np.abs(data_level - func_val).sum()
+
+    # The minimum indicates where the sine function was fittng the worst,
+    # therefore subtract pi. This will also ensure that the estimated phase will
+    # be in the interval [-pi,pi].
+    phase = (sum_res.argmax()/iter_steps *2*np.pi - np.pi)%(2*np.pi)
+
+    # values and bounds of initial parameters
+    params['frequency'].set(value=frequency_max,
+                            min=min(0.1 / (x_axis[-1]-x_axis[0]), dft_x[3]),
+                            max=min(0.5 / stepsize, dft_x.max()-abs(dft_x[2]-dft_x[0])))
+    params['phase'].set(value=phase, min=-2*np.pi, max=2*np.pi)
+    params['amplitude'].set(value=ampl_val, min=0)
+    params['offset'].set(value=offset)
+
+    params['lifetime'].set(value=lifetime_val,
+                           min=2*(x_axis[1]-x_axis[0]),
+                           max=1/(abs(dft_x[1]-dft_x[0])*0.5))
+
+    return error, params
+
+###################################################
+# Sinus with stretched exponential decay fitting  #
+###################################################
+
+
+def make_sinestretchedexponentialdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a sine stretched exponential decay fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    sine_stretched_exp_decay, params = self.make_sinestretchedexponentialdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = sine_stretched_exp_decay.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        result = sine_stretched_exp_decay.fit(data, x=x_axis, params=params, **kwargs)
+        self.log.error('The sineexponentialdecay fit did not work.\n'
+                       'Error message: {0}'.format(result.message))
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()
+
+    period = 1 / result.params['frequency'].value
+    try:
+        period_err = result.params['frequency'].stderr / (result.params['frequency'])**2
+    except ZeroDivisionError:
+        period_err = np.inf
+
+    result_str_dict['Period'] = {'value': period if period else 0.0,
+                                 'error': period_err if period_err else 0.0,
+                                 'unit': units[0]}
+
+    result_str_dict['Frequency'] = {'value': result.params['frequency'].value,
+                                    'error': result.params['frequency'].stderr,
+                                    'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude'] = {'value': result.params['amplitude'].value,
+                                    'error': result.params['amplitude'].stderr,
+                                    'unit': units[1]}
+
+    result_str_dict['Contrast'] = {'value': ((2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value+result.params['amplitude'].value)*100),
+                                   'error':  (np.abs((2*result.params['amplitude'].value) /
+                                              (result.params['offset'].value+result.params['amplitude'].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params['amplitude'].value) + (2*result.params['amplitude'].value) /
+                                             (result.params['offset'].value + result.params['amplitude'].value)**2) *
+                                             result.params['amplitude'].stderr))*100,
+                                   'unit': '%'}
+
+    result_str_dict['Phase'] = {'value': 180/np.pi*result.params['phase'].value,
+                                'error': 180/np.pi*result.params['phase'].stderr,
+                                'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}
+
+    result_str_dict['Beta'] = {'value': result.params['beta'].value,
+                               'error': result.params['beta'].stderr,
+                               'unit': ''}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinestretchedexponentialdecay(self, x_axis, data, params):
+    """ Provide a estimation of a initial values for a sine stretched exponential decay function.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param Parameters object params: object includes parameter dictionary which can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error, params = self.estimate_sineexponentialdecay(x_axis, data, params)
+    #TODO: estimate the exponent cleaverly! For now, set the initial value to 2
+    #      since the usual values for our cases are between 1 and 3.
+    params['beta'].set(value=2, min=0.0, max=10)
+
+    return error, params
+
+###########################################
+# Sum of two individual Sinus with offset #
+###########################################
+
+
+def make_sinedouble_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a two sine with offset fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    two_sine_offset, params = self.make_sinedouble_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The twosineexpdecayoffset fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['s1_frequency'].value
+    try:
+        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency'])**2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['s2_frequency'].value
+    try:
+        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency'])**2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
+                                      'error': result.params['s1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
+                                      'error': result.params['s2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
+                                      'error': result.params['s1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
+                                      'error': result.params['s2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    amp_string = 's1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                    'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                   'unit': '%'}
+
+    amp_string = 's2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                             (result.params['offset'].value+result.params[amp_string].value)*100),
+                                   'error':  (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                             (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                             result.params[amp_string].stderr))*100,
+                                   'unit': '%'}
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
+                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
+                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinedouble(self, x_axis, data, params):
+    """ Provides an estimator for initial values of two sines with offset fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make two consecutive
+    # sine offset fits where for the second the first fit is subtracted to
+    # delete the first sine in the data.
+
+    result1 = self.make_sine_fit(x_axis=x_axis, data=data, estimator=self.estimate_sine)
+    data_sub = data - result1.best_fit
+
+    result2 = self.make_sine_fit(x_axis=x_axis, data=data_sub, estimator=self.estimate_sine)
+
+    # Fill the parameter dict:
+    params['s1_amplitude'].set(value=result1.params['amplitude'].value)
+    params['s1_frequency'].set(value=result1.params['frequency'].value)
+    params['s1_phase'].set(value=result1.params['phase'].value)
+
+    params['s2_amplitude'].set(value=result2.params['amplitude'].value)
+    params['s2_frequency'].set(value=result2.params['frequency'].value)
+    params['s2_phase'].set(value=result2.params['phase'].value)
+
+    params['offset'].set(value=data.mean())
+
+    return error, params
+
+################################################################################
+#    Sum of two individual Sinus with offset and single exponential decay      #
+################################################################################
+
+
+def make_sinedoublewithexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a two sine with one exponential decay offset fit on the provided
+        data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    two_sine_exp_decay_offset, params = self.make_sinedoublewithexpdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = two_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The sinedoublewithexpdecay fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = two_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['s1_frequency'].value
+    try:
+        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['s2_frequency'].value
+    try:
+        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
+                                      'error': result.params['s1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
+                                      'error': result.params['s2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
+                                      'error': result.params['s1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
+                                      'error': result.params['s2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    amp_string = 's1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 's2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
+                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
+                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinedoublewithexpdecay(self, x_axis, data, params):
+    """ Provides an estimator for initial values of two sine with offset and
+        exponential decay fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make two consecutive
+    # sine offset fits where for the second the first fit is subtracted to
+    # delete the first sine in the data.
+
+    result1 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data,
+        estimator=self.estimate_sineexponentialdecay)
+    data_sub = data - result1.best_fit
+
+    result2 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub,
+        estimator=self.estimate_sineexponentialdecay)
+
+    # Fill the parameter dict:
+    params['s1_amplitude'].set(value=result1.params['amplitude'].value)
+    params['s1_frequency'].set(value=result1.params['frequency'].value)
+    params['s1_phase'].set(value=result1.params['phase'].value)
+
+    params['s2_amplitude'].set(value=result2.params['amplitude'].value)
+    params['s2_frequency'].set(value=result2.params['frequency'].value)
+    params['s2_phase'].set(value=result2.params['phase'].value)
+
+    lifetime = (result1.params['lifetime'].value + result2.params['lifetime'].value)/2
+    params['lifetime'].set(value=lifetime, min=2*(x_axis[1]-x_axis[0]))
+    params['offset'].set(value=data.mean())
+
+    return error, params
+
+
+###############################################################
+# Sum of two individual Sinus exponential decays (and offset) #
+###############################################################
+# Problem with stderr: x.stderr will always be 0 for this model!
+
+
+def make_sinedoublewithtwoexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a two sine with two exponential decay and offset fit on the
+        provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    two_sine_two_exp_decay_offset, params = self.make_sinedoublewithtwoexpdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = two_sine_two_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The sinedoublewithtwoexpdecay fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = two_sine_two_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['e1_frequency'].value
+    try:
+        period1_err = result.params['e1_frequency'].stderr / (result.params['e1_frequency']) ** 2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['e2_frequency'].value
+    try:
+        period2_err = result.params['e2_frequency'].stderr / (result.params['e2_frequency']) ** 2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['e1_frequency'].value,
+                                      'error': result.params['e1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['e2_frequency'].value,
+                                      'error': result.params['e2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['e1_amplitude'].value,
+                                      'error': result.params['e1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['e2_amplitude'].value,
+                                      'error': result.params['e2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    amp_string = 'e1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 'e2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['e1_phase'].value,
+                                  'error': 180/np.pi*result.params['e1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['e2_phase'].value,
+                                  'error': 180/np.pi*result.params['e2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Lifetime 1'] = {'value': result.params['e1_lifetime'].value,
+                                     'error': result.params['e1_lifetime'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Lifetime 2'] = {'value': result.params['e2_lifetime'].value,
+                                     'error': result.params['e2_lifetime'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinedoublewithtwoexpdecay(self, x_axis, data, params):
+    """ Provides an estimator for initial values of two sine with offset and
+        two exponential decay fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make two consecutive
+    # sine offset fits where for the second the first fit is subtracted to
+    # delete the first sine in the data.
+
+    result1 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data,
+        estimator=self.estimate_sineexponentialdecay)
+    data_sub = data - result1.best_fit
+
+    result2 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub,
+        estimator=self.estimate_sineexponentialdecay)
+
+    # Fill the parameter dict:
+    params['e1_amplitude'].set(value=result1.params['amplitude'].value)
+    params['e1_frequency'].set(value=result1.params['frequency'].value)
+    params['e1_phase'].set(value=result1.params['phase'].value)
+    params['e1_lifetime'].set(value=result1.params['lifetime'].value,
+                              min=2*(x_axis[1]-x_axis[0]))
+
+    params['e2_amplitude'].set(value=result2.params['amplitude'].value)
+    params['e2_frequency'].set(value=result2.params['frequency'].value)
+    params['e2_phase'].set(value=result2.params['phase'].value)
+    params['e2_lifetime'].set(value=result2.params['lifetime'].value,
+                              min=2*(x_axis[1]-x_axis[0]))
+
+    params['offset'].set(value=data.mean())
+
+    return error, params
+
+#############################################
+# Sum of three individual Sinus with offset #
+#############################################
+
+
+def make_sinetriple_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a three sine with offset fit on the provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    two_sine_offset, params = self.make_sinetriple_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The threesineexpdecayoffset fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = two_sine_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['s1_frequency'].value
+    try:
+        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['s2_frequency'].value
+    try:
+        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    period3 = 1 / result.params['s3_frequency'].value
+    try:
+        period3_err = result.params['s3_frequency'].stderr / (result.params['s3_frequency']) ** 2
+    except ZeroDivisionError:
+        period3_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
+                                   'error': period3_err if period3_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
+                                      'error': result.params['s1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
+                                      'error': result.params['s2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 3'] = {'value': result.params['s3_frequency'].value,
+                                      'error': result.params['s3_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
+                                      'error': result.params['s1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
+                                      'error': result.params['s2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 3'] = {'value': result.params['s3_amplitude'].value,
+                                      'error': result.params['s3_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    amp_string = 's1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 's2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 's3_amplitude'
+    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
+                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
+                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['s3_phase'].value,
+                                  'error': 180/np.pi*result.params['s3_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinetriple(self, x_axis, data, params):
+    """ Provides an estimator for initial values of three sines with offset fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make three consecutive
+    # sine offset fits where for the next fit the previous is subtracted to
+    # delete its contribution in the data.
+
+    res1 = self.make_sine_fit(x_axis=x_axis, data=data, estimator=self.estimate_sine)
+    data_sub1 = data - res1.best_fit
+
+    res2 = self.make_sine_fit(x_axis=x_axis, data=data_sub1, estimator=self.estimate_sine)
+    data_sub2 = data_sub1 - res2.best_fit
+
+    res3 = self.make_sine_fit(x_axis=x_axis, data=data_sub2, estimator=self.estimate_sine)
+
+    # Fill the parameter dict:
+    params['s1_amplitude'].set(value=res1.params['amplitude'].value)
+    params['s1_frequency'].set(value=res1.params['frequency'].value)
+    params['s1_phase'].set(value=res1.params['phase'].value)
+
+    params['s2_amplitude'].set(value=res2.params['amplitude'].value)
+    params['s2_frequency'].set(value=res2.params['frequency'].value)
+    params['s2_phase'].set(value=res2.params['phase'].value)
+
+    params['s3_amplitude'].set(value=res3.params['amplitude'].value)
+    params['s3_frequency'].set(value=res3.params['frequency'].value)
+    params['s3_phase'].set(value=res3.params['phase'].value)
+
+    params['offset'].set(value=data.mean())
+
+    return error, params
+
+##########################################################################
+# Sum of three individual Sinus with offset and single exponential decay #
+##########################################################################
+
+
+def make_sinetriplewithexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a three sine with one exponential decay offset fit on the provided
+        data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    three_sine_exp_decay_offset, params = self.make_sinetriplewithexpdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params, update_params=add_params)
+    try:
+        result = three_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The sinetriplewithexpdecay fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = three_sine_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['s1_frequency'].value
+    try:
+        period1_err = result.params['s1_frequency'].stderr / (result.params['s1_frequency']) ** 2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['s2_frequency'].value
+    try:
+        period2_err = result.params['s2_frequency'].stderr / (result.params['s2_frequency']) ** 2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    period3 = 1 / result.params['s3_frequency'].value
+    try:
+        period3_err = result.params['s3_frequency'].stderr / (result.params['s3_frequency']) ** 2
+    except ZeroDivisionError:
+        period3_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
+                                   'error': period3_err if period3_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['s1_frequency'].value,
+                                      'error': result.params['s1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['s2_frequency'].value,
+                                      'error': result.params['s2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 3'] = {'value': result.params['s3_frequency'].value,
+                                      'error': result.params['s3_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['s1_amplitude'].value,
+                                      'error': result.params['s1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['s2_amplitude'].value,
+                                      'error': result.params['s2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 3'] = {'value': result.params['s3_amplitude'].value,
+                                      'error': result.params['s3_amplitude'].stderr,
+                                      'unit': units[1]}
+
+
+    amp_string = 's1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 's2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 's3_amplitude'
+    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['s1_phase'].value,
+                                  'error': 180/np.pi*result.params['s1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['s2_phase'].value,
+                                  'error': 180/np.pi*result.params['s2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['s3_phase'].value,
+                                  'error': 180/np.pi*result.params['s3_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Lifetime'] = {'value': result.params['lifetime'].value,
+                                   'error': result.params['lifetime'].stderr,
+                                   'unit': units[0]}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinetriplewithexpdecay(self, x_axis, data, params):
+    """ Provides an estimator for initial values of three sine with offset and
+        exponential decay fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make three consecutive
+    # sine exponential decay with offset fits where for the next fit the
+    # previous is subtracted to delete its contribution in the data.
+
+    res1 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data,
+        estimator=self.estimate_sineexponentialdecay)
+
+    data_sub1 = data - res1.best_fit
+
+    res2 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub1,
+        estimator=self.estimate_sineexponentialdecay)
+
+    data_sub2 = data_sub1 - res2.best_fit
+
+    res3 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub2,
+        estimator=self.estimate_sineexponentialdecay)
+
+    # Fill the parameter dict:
+    params['s1_amplitude'].set(value=res1.params['amplitude'].value)
+    params['s1_frequency'].set(value=res1.params['frequency'].value)
+    params['s1_phase'].set(value=res1.params['phase'].value)
+
+    params['s2_amplitude'].set(value=res2.params['amplitude'].value)
+    params['s2_frequency'].set(value=res2.params['frequency'].value)
+    params['s2_phase'].set(value=res2.params['phase'].value)
+
+    params['s3_amplitude'].set(value=res3.params['amplitude'].value)
+    params['s3_frequency'].set(value=res3.params['frequency'].value)
+    params['s3_phase'].set(value=res3.params['phase'].value)
+
+    lifetime = (res1.params['lifetime'].value + res2.params['lifetime'].value + res3.params['lifetime'].value)/3
+    params['lifetime'].set(value=lifetime,
+                           min=2*(x_axis[1]-x_axis[0]))
+    params['offset'].set(value=data.mean())
+
+    return error, params
+
+#########################################################################
+# Sum of three individual Sinus with offset and three exponential decay #
+#########################################################################
+
+
+def make_sinetriplewiththreeexpdecay_fit(self, x_axis, data, estimator, units=None, add_params=None, **kwargs):
+    """ Perform a three sine with three exponential decay and offset fit on the
+        provided data.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param method estimator: Pointer to the estimator method
+    @param list units: List containing the ['horizontal', 'vertical'] units as strings
+    @param Parameters or dict add_params: optional, additional parameters of
+                type lmfit.parameter.Parameters, OrderedDict or dict for the fit
+                which will be used instead of the values from the estimator.
+
+    @return object result: lmfit.model.ModelFit object, all parameters
+                           provided about the fitting, like: success,
+                           initial fitting values, best fitting values, data
+                           with best fit with given axis,...
+    """
+    three_sine_three_exp_decay_offset, params = self.make_sinetriplewiththreeexpdecay_model()
+
+    error, params = estimator(x_axis, data, params)
+
+    params = self._substitute_params(initial_params=params,
+                                     update_params=add_params)
+    try:
+        result = three_sine_three_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+    except:
+        self.log.warning('The twosinetwoexpdecayoffset fit did not work. '
+                         'Error message: {}'.format(str(result.message)))
+        result = three_sine_three_exp_decay_offset.fit(data, x=x_axis, params=params, **kwargs)
+
+    if units is None:
+        units = ['arb. unit', 'arb. unit']
+
+    result_str_dict = dict()  # create result string for gui or OrderedDict()
+
+    period1 = 1 / result.params['e1_frequency'].value
+    try:
+        period1_err = result.params['e1_frequency'].stderr / (result.params['e1_frequency']) ** 2
+    except ZeroDivisionError:
+        period1_err = np.inf
+
+    period2 = 1 / result.params['e2_frequency'].value
+    try:
+        period2_err = result.params['e2_frequency'].stderr / (result.params['e2_frequency']) ** 2
+    except ZeroDivisionError:
+        period2_err = np.inf
+
+    period3 = 1 / result.params['e3_frequency'].value
+    try:
+        period3_err = result.params['e3_frequency'].stderr / (result.params['e3_frequency']) ** 2
+    except ZeroDivisionError:
+        period3_err = np.inf
+
+    result_str_dict['Period 1'] = {'value': period1 if period1 else 0.0,
+                                   'error': period1_err if period1_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Period 2'] = {'value': period2 if period2 else 0.0,
+                                   'error': period2_err if period2_err else 0.0,
+                                   'unit': units[0]}
+    result_str_dict['Period 3'] = {'value': period3 if period3 else 0.0,
+                                   'error': period3_err if period3_err else 0.0,
+                                   'unit': units[0]}
+
+    result_str_dict['Frequency 1'] = {'value': result.params['e1_frequency'].value,
+                                      'error': result.params['e1_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 2'] = {'value': result.params['e2_frequency'].value,
+                                      'error': result.params['e2_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Frequency 3'] = {'value': result.params['e3_frequency'].value,
+                                      'error': result.params['e3_frequency'].stderr,
+                                      'unit': 'Hz' if units[0] == 's' else '1/' + units[0]}
+
+    result_str_dict['Amplitude 1'] = {'value': result.params['e1_amplitude'].value,
+                                      'error': result.params['e1_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 2'] = {'value': result.params['e2_amplitude'].value,
+                                      'error': result.params['e2_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    result_str_dict['Amplitude 3'] = {'value': result.params['e3_amplitude'].value,
+                                      'error': result.params['e3_amplitude'].stderr,
+                                      'unit': units[1]}
+
+    amp_string = 'e1_amplitude'
+    result_str_dict['Contrast 1'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 'e2_amplitude'
+    result_str_dict['Contrast 2'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+    amp_string = 'e3_amplitude'
+    result_str_dict['Contrast 3'] = {'value': ((2*result.params[amp_string].value) /
+                                               (result.params['offset'].value+result.params[amp_string].value)*100),
+                                     'error': (np.abs((2*result.params[amp_string].value) /
+                                              (result.params['offset'].value+result.params[amp_string].value)**2 *
+                                             result.params['offset'].stderr) +
+                                             np.abs((2/(result.params['offset'].value +
+                                             result.params[amp_string].value) + (2*result.params[amp_string].value) /
+                                              (result.params['offset'].value + result.params[amp_string].value)**2) *
+                                               result.params[amp_string].stderr))*100,
+                                     'unit': '%'}
+
+
+    result_str_dict['Phase 1'] = {'value': 180/np.pi*result.params['e1_phase'].value,
+                                  'error': 180/np.pi*result.params['e1_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 2'] = {'value': 180/np.pi*result.params['e2_phase'].value,
+                                  'error': 180/np.pi*result.params['e2_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Phase 3'] = {'value': 180/np.pi*result.params['e3_phase'].value,
+                                  'error': 180/np.pi*result.params['e3_phase'].stderr,
+                                  'unit': 'deg'}
+
+    result_str_dict['Lifetime 1'] = {'value': result.params['e1_lifetime'].value,
+                                     'error': result.params['e1_lifetime'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Lifetime 2'] = {'value': result.params['e2_lifetime'].value,
+                                     'error': result.params['e2_lifetime'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Lifetime 3'] = {'value': result.params['e3_lifetime'].value,
+                                     'error': result.params['e3_lifetime'].stderr,
+                                     'unit': units[0]}
+
+    result_str_dict['Offset'] = {'value': result.params['offset'].value,
+                                 'error': result.params['offset'].stderr,
+                                 'unit': units[1]}
+
+    result.result_str_dict = result_str_dict
+    return result
+
+
+def estimate_sinetriplewiththreeexpdecay(self, x_axis, data, params):
+    """ Provides an estimator for initial values of three sine with offset and
+        three exponential decay fitting.
+
+    @param numpy.array x_axis: 1D axis values
+    @param numpy.array data: 1D data, should have the same dimension as x_axis.
+    @param lmfit.Parameters params: object includes parameter dictionary which
+                                    can be set
+
+    @return tuple (error, params):
+
+    Explanation of the return parameter:
+        int error: error code (0:OK, -1:error)
+        Parameters object params: set parameters of initial values
+    """
+
+    error = self._check_1D_input(x_axis=x_axis, data=data, params=params)
+
+    # That procedure seems to work extremely reliable: make two consecutive
+    # sine offset fits where for the second the first fit is subtracted to
+    # delete the first sine in the data.
+
+    res1 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data,
+        estimator=self.estimate_sineexponentialdecay)
+    data_sub1 = data - res1.best_fit
+
+    res2 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub1,
+        estimator=self.estimate_sineexponentialdecay)
+    data_sub2 = data_sub1 - res2.best_fit
+
+    res3 = self.make_sineexponentialdecay_fit(
+        x_axis=x_axis,
+        data=data_sub2,
+        estimator=self.estimate_sineexponentialdecay)
+
+    # Fill the parameter dict:
+    params['e1_amplitude'].set(value=res1.params['amplitude'].value)
+    params['e1_frequency'].set(value=res1.params['frequency'].value)
+    params['e1_phase'].set(value=res1.params['phase'].value)
+    params['e1_lifetime'].set(value=res1.params['lifetime'].value,
+                              min=2*(x_axis[1]-x_axis[0]))
+
+    params['e2_amplitude'].set(value=res2.params['amplitude'].value)
+    params['e2_frequency'].set(value=res2.params['frequency'].value)
+    params['e2_phase'].set(value=res2.params['phase'].value)
+    params['e2_lifetime'].set(value=res2.params['lifetime'].value,
+                              min=2*(x_axis[1]-x_axis[0]))
+
+    params['e3_amplitude'].set(value=res3.params['amplitude'].value)
+    params['e3_frequency'].set(value=res3.params['frequency'].value)
+    params['e3_phase'].set(value=res3.params['phase'].value)
+    params['e3_lifetime'].set(value=res3.params['lifetime'].value,
+                              min=2*(x_axis[1]-x_axis[0]))
+
+    params['offset'].set(value=data.mean())
+
+    return error, params
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/io_handler.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/io_handler.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,342 +1,342 @@
-import ast
-import datetime
-import inspect
-import itertools
-import pickle
-from functools import wraps
-from pathlib import Path
-from typing import Callable
-
-import matplotlib.pyplot as plt
-import numpy as np
-import pandas as pd
-import pySPM
-
-
-class IOHandler:
-    """ Handle all read and write operations. """
-
-    def __init__(self, base_read_path: Path = None, base_write_path: Path = None):
-        super().__init__()
-        self.base_read_path = base_read_path
-        self.base_write_path = base_write_path
-
-    @staticmethod
-    def add_base_read_path(func: Callable) -> Callable:
-        """ Decorator to add the base_read_path to the filepath if it is not None """
-
-        @wraps(func)
-        def wrapper(self, filepath: Path, **kwargs):
-            if self.base_read_path:
-                filepath = self.base_read_path / filepath
-            return func(self, filepath, **kwargs)
-
-        return wrapper
-
-    @staticmethod
-    def add_base_write_path(func: Callable) -> Callable:
-        """ Decorator to add the base_write_path to the filepath if it is not None """
-
-        @wraps(func)
-        def wrapper(self, filepath: Path, **kwargs):
-            if self.base_write_path:
-                filepath = self.base_write_path / filepath
-            filepath.parent.mkdir(exist_ok=True)
-            return func(self, filepath, **kwargs)
-
-        return wrapper
-
-    @staticmethod
-    def check_extension(ext: str) -> Callable:
-        """ Decorator to check the extension of the filepath is correct """
-
-        def decorator(func: Callable) -> Callable:
-            def wrapper(self, filepath: Path, **kwargs) -> Callable:
-                if filepath.suffix == ext:
-                    return func(self, filepath, **kwargs)
-                elif filepath.suffix == "":
-                    return func(self, filepath.with_suffix(ext), **kwargs)
-                else:
-                    raise IOError(f"Invalid extension '{filepath.suffix}' in '{filepath}', extension should be '{ext}'")
-
-            return wrapper
-
-        return decorator
-
-    @add_base_read_path
-    @check_extension(".dat")
-    def read_qudi_parameters(self, filepath: Path) -> dict:
-        """ Extract parameters from a qudi dat file. """
-        params = {}
-        with open(filepath) as file:
-            for line in file:
-                if line == '#=====\n':
-                    break
-                else:
-                    # noinspection PyBroadException
-                    try:
-                        # Remove # from beginning of lines
-                        line = line[1:]
-                        if line.count(":") == 1:
-                            # Add params to dictionary
-                            label, value = line.split(":")
-                            if value != "\n":
-                                params[label] = ast.literal_eval(inspect.cleandoc(value))
-                        elif line.count(":") == 3:
-                            # Handle files with timestamps in them
-                            label = line.split(":")[0]
-                            timestamp_str = "".join(line.split(":")[1:]).strip()
-                            datetime_str = datetime.datetime.strptime(timestamp_str, "%d.%m.%Y %Hh%Mmin%Ss").replace(
-                                tzinfo=datetime.timezone.utc)
-                            params[label] = datetime_str
-                    except Exception as _:
-                        pass
-        return params
-
-    @add_base_read_path
-    @check_extension(".dat")
-    def read_into_dataframe(self, filepath: Path) -> pd.DataFrame:
-        """ Read a qudi data file into a pd DataFrame for analysis. """
-        with open(filepath) as handle:
-            # Generate column names for DataFrame by parsing the file
-            *_comments, names = itertools.takewhile(lambda line: line.startswith('#'), handle)
-            names = names[1:].strip().split("\t")
-        return pd.read_csv(filepath, names=names, comment="#", sep="\t")
-
-    @add_base_read_path
-    def read_csv(self, filepath: Path, **kwargs) -> pd.DataFrame:
-        """ Read a csv file into a pd DataFrame. """
-        return pd.read_csv(filepath, **kwargs)
-
-    @add_base_read_path
-    def read_excel(self, filepath: Path, **kwargs) -> pd.DataFrame:
-        """ Read a csv file into a pd DataFrame. """
-        return pd.read_excel(filepath, **kwargs)
-
-    @add_base_read_path
-    @check_extension(".dat")
-    def read_confocal_into_dataframe(self, filepath: Path) -> pd.DataFrame:
-        confocal_params = self.read_qudi_parameters(filepath)
-        data = self.read_into_ndarray(filepath, delimiter="\t")
-        # Use the confocal parameters to generate the index and columns for the DataFrame
-        index = np.linspace(
-            confocal_params['X image min (m)'],
-            confocal_params['X image max (m)'],
-            data.shape[0]
-        )
-        columns = np.linspace(
-            confocal_params['Y image min'],
-            confocal_params['Y image max'],
-            data.shape[1]
-        )
-        df = pd.DataFrame(data, index=index, columns=columns)
-        # Sort the index to get origin (0, 0) in the lower left corner of the DataFrame
-        df.sort_index(axis=0, ascending=False, inplace=True)
-        return df
-
-    @add_base_read_path
-    def read_into_ndarray(self, filepath: Path, **kwargs) -> np.ndarray:
-        return np.genfromtxt(filepath, **kwargs)
-
-    @add_base_read_path
-    def read_into_ndarray_transposed(self, filepath: Path, **kwargs) -> np.ndarray:
-        return np.genfromtxt(filepath, **kwargs).T
-
-    @add_base_read_path
-    @check_extension(".pys")
-    def read_pys(self, filepath: Path) -> dict:
-        """ Loads raw pys data files. Wraps around numpy.load. """
-        byte_dict = np.load(str(filepath), encoding="bytes", allow_pickle=True)
-        # Convert byte string keys to normal strings
-        return {key.decode('utf8'): byte_dict.get(key) for key in byte_dict.keys()}
-
-    @add_base_read_path
-    @check_extension(".pkl")
-    def read_pkl(self, filepath: Path) -> dict:
-        """ Loads processed pickle files for plotting/further analysis. """
-        with open(filepath, 'rb') as f:
-            file = pickle.load(f)
-        return file
-
-    @add_base_read_path
-    @check_extension(".dat")
-    def read_nanonis_data(self, filepath: Path) -> pd.DataFrame:
-        """ Extract data from a Nanonis dat file. """
-        skip_rows = 0
-        with open(filepath) as dat_file:
-            for num, line in enumerate(dat_file, 1):
-                if "[DATA]" in line:
-                    # Find number of rows to skip when extracting data
-                    skip_rows = num
-                    break
-                if "#=====" in line:
-                    skip_rows = num
-                    break
-        df = pd.read_table(filepath, sep="\t", skiprows=skip_rows)
-        return df
-
-    @add_base_read_path
-    @check_extension(".dat")
-    def read_nanonis_parameters(self, filepath: Path) -> dict:
-        """ Extract parameters from a Nanonis dat file. """
-        parameters = {}
-        with open(filepath) as dat_file:
-            for line in dat_file:
-                if line == "\n":
-                    # Break when reaching empty line
-                    break
-                elif "User" in line or line.split("\t")[0] == "":
-                    # Cleanup excess parameters and skip empty lines
-                    pass
-                else:
-                    label, value, _ = line.split("\t")
-                    try:
-                        # Convert strings to number where possible
-                        value = float(value)
-                    except ValueError:
-                        pass
-                    if "Oscillation Control>" in label:
-                        label = label.replace("Oscillation Control>", "")
-                    parameters[label] = value
-        return parameters
-
-    @add_base_read_path
-    @check_extension(".sxm")
-    def read_nanonis_spm_data(self, filepath: Path) -> pySPM.SXM:
-        """ Read a Nanonis SPM data file. """
-        return pySPM.SXM(filepath)
-
-    @add_base_read_path
-    @check_extension(".001")
-    def read_bruker_spm_data(self, filepath: Path) -> pySPM.Bruker:
-        """ Read a Bruker SPM data file. """
-        return pySPM.Bruker(filepath)
-
-    @add_base_read_path
-    @check_extension(".txt")
-    def read_pfeiffer_data(self, filepath: Path) -> pd.DataFrame:
-        """ Read data stored by Pfeiffer vacuum monitoring software. """
-        # Extract rows including the header
-        df = pd.read_csv(filepath, sep="\t", skiprows=[0, 2, 3, 4])
-        # Combine data and time columns together
-        df["Date"] = df["Date"] + " " + df["Time"]
-        df = df.drop("Time", axis=1)
-        # Infer datetime format and convert to datetime objects
-        df["Date"] = pd.to_datetime(df["Date"], infer_datetime_format=True)
-        # Set datetime as index
-        df = df.set_index("Date", drop=True)
-        return df
-
-    @add_base_read_path
-    @check_extension(".xls")
-    def read_lakeshore_data(self, filepath: Path) -> pd.DataFrame:
-        """ Read data stored by Lakeshore temperature monitor software. """
-        # Extract only the origin timestamp
-        origin = pd.read_excel(filepath, skiprows=1, nrows=1, usecols=[1], header=None)[1][0]
-        # Remove any tzinfo to prevent future exceptions in pandas
-        origin = origin.replace("CET", "")
-        # Parse datetime object from timestamp
-        origin = pd.to_datetime(origin)
-        # Create DataFrame and drop empty cols
-        df = pd.read_excel(filepath, skiprows=3)
-        df = df.dropna(axis=1, how="all")
-        # Add datetimes to DataFrame
-        df["Datetime"] = pd.to_datetime(df["Time"], unit="ms", origin=origin)
-        df = df.drop("Time", axis=1)
-        # Set datetime as index
-        df = df.set_index("Datetime", drop=True)
-        return df
-
-    @add_base_read_path
-    @check_extension(".txt")
-    def read_oceanoptics_data(self, filepath: str) -> pd.DataFrame:
-        """ Read spectrometer data from OceanOptics spectrometer. """
-        df = pd.read_csv(filepath, sep="\t", skiprows=14, names=["wavelength", "intensity"])
-        return df
-
-    @staticmethod
-    def __get_forward_backward_counts(count_rates, num_pixels):
-        split_array = np.split(count_rates, 2 * num_pixels)
-        # Extract forward scan array as every second element
-        forward_counts = np.stack(split_array[::2])
-        # Extract backward scan array as every shifted second element
-        # Flip scan so that backward and forward scans represent the same data
-        backward_counts = np.flip(np.stack(split_array[1::2]), axis=1)
-        return forward_counts, backward_counts
-
-    def read_pixelscanner_data(self, filepath: Path) -> (pySPM.SPM_image, pySPM.SPM_image):
-        df = self.read_into_dataframe(filepath)
-        num_pixels = int(np.sqrt(len(df) // 2))
-
-        if num_pixels ** 2 != len(df) // 2:
-            raise ValueError("Number of pixels does not match data length.")
-
-        try:
-            fwd, bwd = self.__get_forward_backward_counts(df["count_rates"], num_pixels)
-        except KeyError:
-            try:
-                fwd, bwd = self.__get_forward_backward_counts(df["Count Rates (cps)"], num_pixels)
-            except KeyError:
-                # Support old data format
-                fwd = df["forward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
-                bwd = df["backward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
-
-        fwd = pySPM.SPM_image(fwd, channel="Forward", _type="NV-PL")
-        bwd = pySPM.SPM_image(bwd, channel="Backward", _type="NV-PL")
-        return fwd, bwd
-
-    @add_base_write_path
-    @check_extension(".pkl")
-    def save_pkl(self, filepath: Path, obj: object):
-        """ Saves processed pickle files for plotting/further analysis. """
-        with open(filepath, 'wb') as f:
-            pickle.dump(obj, f)
-
-    @add_base_write_path
-    @check_extension(".pys")
-    def save_pys(self, filepath: Path, dictionary: dict):
-        """ Saves processed pickle files for plotting/further analysis. """
-        with open(filepath, 'wb') as f:
-            pickle.dump(dictionary, f, 1)
-
-    @add_base_write_path
-    @check_extension(".pys")
-    def save_df(self, filepath: Path, df: pd.DataFrame):
-        """ Save Dataframe as csv. """
-        df.to_csv(filepath, sep='\t', encoding='utf-8')
-
-    @add_base_write_path
-    def save_figures(self, filepath: Path, fig: plt.Figure, **kwargs):
-        """
-        Saves figures from matplotlib plot data. By default, saves as jpg, png, pdf and svg.
-
-        Parameters
-        ----------
-        fig : matplotlib.figure.Figure
-            Figure to save.
-        filepath : pathlib.Path
-            Path to save figure to. If called with DataHandler, only the filename is required.
-
-        Keyword Arguments
-        -----------------
-        only_jpg : bool
-            If True, only save as jpg. Default is False.
-        only_pdf : bool
-            If True, only save as pdf. Default is False.
-        **kwargs
-            Keyword arguments passed to fig.savefig().
-        """
-        extensions = None
-        if "only_jpg" in kwargs:
-            if kwargs.get("only_jpg"):
-                extensions = [".jpg"]
-            kwargs.pop("only_jpg", None)
-        elif "only_pdf" in kwargs:
-            if kwargs.get("only_pdf"):
-                extensions = [".pdf"]
-            kwargs.pop("only_pdf", None)
-        else:
-            extensions = [".jpg", ".pdf", ".svg", ".png"]
-
-        for ext in extensions:
-            fig.savefig(filepath.with_suffix(ext), dpi=200, **kwargs)
+import ast
+import datetime
+import inspect
+import itertools
+import pickle
+from functools import wraps
+from pathlib import Path
+from typing import Callable
+
+import matplotlib.pyplot as plt
+import numpy as np
+import pandas as pd
+import pySPM
+
+
+class IOHandler:
+    """ Handle all read and write operations. """
+
+    def __init__(self, base_read_path: Path = None, base_write_path: Path = None):
+        super().__init__()
+        self.base_read_path = base_read_path
+        self.base_write_path = base_write_path
+
+    @staticmethod
+    def add_base_read_path(func: Callable) -> Callable:
+        """ Decorator to add the base_read_path to the filepath if it is not None """
+
+        @wraps(func)
+        def wrapper(self, filepath: Path, **kwargs):
+            if self.base_read_path:
+                filepath = self.base_read_path / filepath
+            return func(self, filepath, **kwargs)
+
+        return wrapper
+
+    @staticmethod
+    def add_base_write_path(func: Callable) -> Callable:
+        """ Decorator to add the base_write_path to the filepath if it is not None """
+
+        @wraps(func)
+        def wrapper(self, filepath: Path, **kwargs):
+            if self.base_write_path:
+                filepath = self.base_write_path / filepath
+            filepath.parent.mkdir(exist_ok=True)
+            return func(self, filepath, **kwargs)
+
+        return wrapper
+
+    @staticmethod
+    def check_extension(ext: str) -> Callable:
+        """ Decorator to check the extension of the filepath is correct """
+
+        def decorator(func: Callable) -> Callable:
+            def wrapper(self, filepath: Path, **kwargs) -> Callable:
+                if filepath.suffix == ext:
+                    return func(self, filepath, **kwargs)
+                elif filepath.suffix == "":
+                    return func(self, filepath.with_suffix(ext), **kwargs)
+                else:
+                    raise IOError(f"Invalid extension '{filepath.suffix}' in '{filepath}', extension should be '{ext}'")
+
+            return wrapper
+
+        return decorator
+
+    @add_base_read_path
+    @check_extension(".dat")
+    def read_qudi_parameters(self, filepath: Path) -> dict:
+        """ Extract parameters from a qudi dat file. """
+        params = {}
+        with open(filepath) as file:
+            for line in file:
+                if line == '#=====\n':
+                    break
+                else:
+                    # noinspection PyBroadException
+                    try:
+                        # Remove # from beginning of lines
+                        line = line[1:]
+                        if line.count(":") == 1:
+                            # Add params to dictionary
+                            label, value = line.split(":")
+                            if value != "\n":
+                                params[label] = ast.literal_eval(inspect.cleandoc(value))
+                        elif line.count(":") == 3:
+                            # Handle files with timestamps in them
+                            label = line.split(":")[0]
+                            timestamp_str = "".join(line.split(":")[1:]).strip()
+                            datetime_str = datetime.datetime.strptime(timestamp_str, "%d.%m.%Y %Hh%Mmin%Ss").replace(
+                                tzinfo=datetime.timezone.utc)
+                            params[label] = datetime_str
+                    except Exception as _:
+                        pass
+        return params
+
+    @add_base_read_path
+    @check_extension(".dat")
+    def read_into_dataframe(self, filepath: Path) -> pd.DataFrame:
+        """ Read a qudi data file into a pd DataFrame for analysis. """
+        with open(filepath) as handle:
+            # Generate column names for DataFrame by parsing the file
+            *_comments, names = itertools.takewhile(lambda line: line.startswith('#'), handle)
+            names = names[1:].strip().split("\t")
+        return pd.read_csv(filepath, names=names, comment="#", sep="\t")
+
+    @add_base_read_path
+    def read_csv(self, filepath: Path, **kwargs) -> pd.DataFrame:
+        """ Read a csv file into a pd DataFrame. """
+        return pd.read_csv(filepath, **kwargs)
+
+    @add_base_read_path
+    def read_excel(self, filepath: Path, **kwargs) -> pd.DataFrame:
+        """ Read a csv file into a pd DataFrame. """
+        return pd.read_excel(filepath, **kwargs)
+
+    @add_base_read_path
+    @check_extension(".dat")
+    def read_confocal_into_dataframe(self, filepath: Path) -> pd.DataFrame:
+        confocal_params = self.read_qudi_parameters(filepath)
+        data = self.read_into_ndarray(filepath, delimiter="\t")
+        # Use the confocal parameters to generate the index and columns for the DataFrame
+        index = np.linspace(
+            confocal_params['X image min (m)'],
+            confocal_params['X image max (m)'],
+            data.shape[0]
+        )
+        columns = np.linspace(
+            confocal_params['Y image min'],
+            confocal_params['Y image max'],
+            data.shape[1]
+        )
+        df = pd.DataFrame(data, index=index, columns=columns)
+        # Sort the index to get origin (0, 0) in the lower left corner of the DataFrame
+        df.sort_index(axis=0, ascending=False, inplace=True)
+        return df
+
+    @add_base_read_path
+    def read_into_ndarray(self, filepath: Path, **kwargs) -> np.ndarray:
+        return np.genfromtxt(filepath, **kwargs)
+
+    @add_base_read_path
+    def read_into_ndarray_transposed(self, filepath: Path, **kwargs) -> np.ndarray:
+        return np.genfromtxt(filepath, **kwargs).T
+
+    @add_base_read_path
+    @check_extension(".pys")
+    def read_pys(self, filepath: Path) -> dict:
+        """ Loads raw pys data files. Wraps around numpy.load. """
+        byte_dict = np.load(str(filepath), encoding="bytes", allow_pickle=True)
+        # Convert byte string keys to normal strings
+        return {key.decode('utf8'): byte_dict.get(key) for key in byte_dict.keys()}
+
+    @add_base_read_path
+    @check_extension(".pkl")
+    def read_pkl(self, filepath: Path) -> dict:
+        """ Loads processed pickle files for plotting/further analysis. """
+        with open(filepath, 'rb') as f:
+            file = pickle.load(f)
+        return file
+
+    @add_base_read_path
+    @check_extension(".dat")
+    def read_nanonis_data(self, filepath: Path) -> pd.DataFrame:
+        """ Extract data from a Nanonis dat file. """
+        skip_rows = 0
+        with open(filepath) as dat_file:
+            for num, line in enumerate(dat_file, 1):
+                if "[DATA]" in line:
+                    # Find number of rows to skip when extracting data
+                    skip_rows = num
+                    break
+                if "#=====" in line:
+                    skip_rows = num
+                    break
+        df = pd.read_table(filepath, sep="\t", skiprows=skip_rows)
+        return df
+
+    @add_base_read_path
+    @check_extension(".dat")
+    def read_nanonis_parameters(self, filepath: Path) -> dict:
+        """ Extract parameters from a Nanonis dat file. """
+        parameters = {}
+        with open(filepath) as dat_file:
+            for line in dat_file:
+                if line == "\n":
+                    # Break when reaching empty line
+                    break
+                elif "User" in line or line.split("\t")[0] == "":
+                    # Cleanup excess parameters and skip empty lines
+                    pass
+                else:
+                    label, value, _ = line.split("\t")
+                    try:
+                        # Convert strings to number where possible
+                        value = float(value)
+                    except ValueError:
+                        pass
+                    if "Oscillation Control>" in label:
+                        label = label.replace("Oscillation Control>", "")
+                    parameters[label] = value
+        return parameters
+
+    @add_base_read_path
+    @check_extension(".sxm")
+    def read_nanonis_spm_data(self, filepath: Path) -> pySPM.SXM:
+        """ Read a Nanonis SPM data file. """
+        return pySPM.SXM(filepath)
+
+    @add_base_read_path
+    @check_extension(".001")
+    def read_bruker_spm_data(self, filepath: Path) -> pySPM.Bruker:
+        """ Read a Bruker SPM data file. """
+        return pySPM.Bruker(filepath)
+
+    @add_base_read_path
+    @check_extension(".txt")
+    def read_pfeiffer_data(self, filepath: Path) -> pd.DataFrame:
+        """ Read data stored by Pfeiffer vacuum monitoring software. """
+        # Extract rows including the header
+        df = pd.read_csv(filepath, sep="\t", skiprows=[0, 2, 3, 4])
+        # Combine data and time columns together
+        df["Date"] = df["Date"] + " " + df["Time"]
+        df = df.drop("Time", axis=1)
+        # Infer datetime format and convert to datetime objects
+        df["Date"] = pd.to_datetime(df["Date"], infer_datetime_format=True)
+        # Set datetime as index
+        df = df.set_index("Date", drop=True)
+        return df
+
+    @add_base_read_path
+    @check_extension(".xls")
+    def read_lakeshore_data(self, filepath: Path) -> pd.DataFrame:
+        """ Read data stored by Lakeshore temperature monitor software. """
+        # Extract only the origin timestamp
+        origin = pd.read_excel(filepath, skiprows=1, nrows=1, usecols=[1], header=None)[1][0]
+        # Remove any tzinfo to prevent future exceptions in pandas
+        origin = origin.replace("CET", "")
+        # Parse datetime object from timestamp
+        origin = pd.to_datetime(origin)
+        # Create DataFrame and drop empty cols
+        df = pd.read_excel(filepath, skiprows=3)
+        df = df.dropna(axis=1, how="all")
+        # Add datetimes to DataFrame
+        df["Datetime"] = pd.to_datetime(df["Time"], unit="ms", origin=origin)
+        df = df.drop("Time", axis=1)
+        # Set datetime as index
+        df = df.set_index("Datetime", drop=True)
+        return df
+
+    @add_base_read_path
+    @check_extension(".txt")
+    def read_oceanoptics_data(self, filepath: str) -> pd.DataFrame:
+        """ Read spectrometer data from OceanOptics spectrometer. """
+        df = pd.read_csv(filepath, sep="\t", skiprows=14, names=["wavelength", "intensity"])
+        return df
+
+    @staticmethod
+    def __get_forward_backward_counts(count_rates, num_pixels):
+        split_array = np.split(count_rates, 2 * num_pixels)
+        # Extract forward scan array as every second element
+        forward_counts = np.stack(split_array[::2])
+        # Extract backward scan array as every shifted second element
+        # Flip scan so that backward and forward scans represent the same data
+        backward_counts = np.flip(np.stack(split_array[1::2]), axis=1)
+        return forward_counts, backward_counts
+
+    def read_pixelscanner_data(self, filepath: Path) -> (pySPM.SPM_image, pySPM.SPM_image):
+        df = self.read_into_dataframe(filepath)
+        num_pixels = int(np.sqrt(len(df) // 2))
+
+        if num_pixels ** 2 != len(df) // 2:
+            raise ValueError("Number of pixels does not match data length.")
+
+        try:
+            fwd, bwd = self.__get_forward_backward_counts(df["count_rates"], num_pixels)
+        except KeyError:
+            try:
+                fwd, bwd = self.__get_forward_backward_counts(df["Count Rates (cps)"], num_pixels)
+            except KeyError:
+                # Support old data format
+                fwd = df["forward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
+                bwd = df["backward (cps)"].to_numpy().reshape(num_pixels, num_pixels)
+
+        fwd = pySPM.SPM_image(fwd, channel="Forward", _type="NV-PL")
+        bwd = pySPM.SPM_image(bwd, channel="Backward", _type="NV-PL")
+        return fwd, bwd
+
+    @add_base_write_path
+    @check_extension(".pkl")
+    def save_pkl(self, filepath: Path, obj: object):
+        """ Saves processed pickle files for plotting/further analysis. """
+        with open(filepath, 'wb') as f:
+            pickle.dump(obj, f)
+
+    @add_base_write_path
+    @check_extension(".pys")
+    def save_pys(self, filepath: Path, dictionary: dict):
+        """ Saves processed pickle files for plotting/further analysis. """
+        with open(filepath, 'wb') as f:
+            pickle.dump(dictionary, f, 1)
+
+    @add_base_write_path
+    @check_extension(".pys")
+    def save_df(self, filepath: Path, df: pd.DataFrame):
+        """ Save Dataframe as csv. """
+        df.to_csv(filepath, sep='\t', encoding='utf-8')
+
+    @add_base_write_path
+    def save_figures(self, filepath: Path, fig: plt.Figure, **kwargs):
+        """
+        Saves figures from matplotlib plot data. By default, saves as jpg, png, pdf and svg.
+
+        Parameters
+        ----------
+        fig : matplotlib.figure.Figure
+            Figure to save.
+        filepath : pathlib.Path
+            Path to save figure to. If called with DataHandler, only the filename is required.
+
+        Keyword Arguments
+        -----------------
+        only_jpg : bool
+            If True, only save as jpg. Default is False.
+        only_pdf : bool
+            If True, only save as pdf. Default is False.
+        **kwargs
+            Keyword arguments passed to fig.savefig().
+        """
+        extensions = None
+        if "only_jpg" in kwargs:
+            if kwargs.get("only_jpg"):
+                extensions = [".jpg"]
+            kwargs.pop("only_jpg", None)
+        elif "only_pdf" in kwargs:
+            if kwargs.get("only_pdf"):
+                extensions = [".pdf"]
+            kwargs.pop("only_pdf", None)
+        else:
+            extensions = [".jpg", ".pdf", ".svg", ".png"]
+
+        for ext in extensions:
+            fig.savefig(filepath.with_suffix(ext), dpi=200, **kwargs)
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/measurement_dataclass.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/measurement_dataclass.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,202 +1,202 @@
-from __future__ import annotations
-
-import logging
-import re
-from dataclasses import dataclass, field
-from pathlib import Path
-from typing import TYPE_CHECKING, Callable
-
-import pandas as pd
-
-if TYPE_CHECKING:
-    import datetime
-    import numpy as np
-    from PIL import Image
-
-logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
-
-
-@dataclass
-class PulsedMeasurement:
-    filepath: Path
-    loaders: (Callable, Callable) = field(default=None)
-    __data: pd.DataFrame = field(default=None)
-    __params: dict = field(default=None)
-
-    @property
-    def data(self) -> pd.DataFrame:
-        """ Read measurement data from file into pandas DataFrame """
-        if self.__data is None:
-            self.__data = self.loaders[0](self.filepath)
-        return self.__data
-
-    @property
-    def params(self) -> dict:
-        """ Read measurement params from file into dict """
-        if self.__params is None:
-            self.__params = self.loaders[1](self.filepath)
-        return self.__params
-
-
-@dataclass
-class LaserPulses:
-    filepath: Path
-    loaders: (Callable, Callable) = field(default=None)
-    __data: np.ndarray = field(default=None)
-    __params: dict = field(default=None)
-
-    @property
-    def data(self) -> np.ndarray:
-        """ Read measurement data from file into pandas DataFrame """
-        if self.__data is None:
-            self.__data = self.loaders[0](self.filepath)
-        return self.__data
-
-    @property
-    def params(self) -> dict:
-        """ Read measurement params from file into dict """
-        if self.__params is None:
-            self.__params = self.loaders[1](self.filepath)
-        return self.__params
-
-
-@dataclass
-class RawTimetrace:
-    filepath: Path
-    loaders: (Callable, Callable) = field(default=None)
-    __data: np.ndarray = field(default=None)
-    __params: dict = field(default=None)
-
-    @property
-    def data(self) -> np.ndarray:
-        """ Read measurement data from file into pandas DataFrame """
-        if self.__data is None:
-            self.__data = self.loaders[0](self.filepath)
-        return self.__data
-
-    @property
-    def params(self) -> dict:
-        """ Read measurement params from file into dict """
-        if self.__params is None:
-            self.__params = self.loaders[1](self.filepath)
-        return self.__params
-
-
-@dataclass
-class PulsedMeasurementDataclass:
-    measurement: PulsedMeasurement
-    laser_pulses: LaserPulses = field(default=None)
-    timetrace: RawTimetrace = field(default=None)
-
-    def __post_init__(self):
-        self.base_filename = self.measurement.filepath.name.replace("_pulsed_measurement.dat", "")
-
-    def show_image(self) -> Image:
-        """ Use PIL to open the measurement image saved on the disk """
-        return Image.open(str(self.measurement.filepath).replace(".dat", "_fig.png"))
-
-
-@dataclass
-class MeasurementDataclass:
-    timestamp: datetime.datetime
-    filepath: Path = field(default=None)
-    loaders: (Callable, Callable) = field(default=None)
-    pulsed: PulsedMeasurementDataclass = field(default=None)
-    __data: np.ndarray | pd.DataFrame = field(default=None)
-    __params: dict = field(default=None)
-
-    def __post_init__(self):
-        self.log = logging.getLogger(__name__)
-
-        if self.pulsed:
-            self.filename = self.pulsed.base_filename
-        else:
-            self.filename = self.filepath.name
-
-    def __repr__(self) -> str:
-
-        return f"Measurement(timestamp='{self.timestamp}', filename='{self.filename}')"
-
-    @property
-    def data(self) -> np.ndarray | pd.DataFrame:
-        """ Read measurement data from file into suitable data structure """
-        if self.pulsed:
-            return self.pulsed.measurement.data
-        else:
-            if self.__data is None:
-                self.__data = self.loaders[0](self.filepath)
-            return self.__data
-
-    @property
-    def params(self) -> dict:
-        """ Read measurement params from file into dict """
-        if self.pulsed:
-            return self.pulsed.measurement.params
-        else:
-            if self.__params is None:
-                self.__params = self.loaders[1](self.filepath)
-            return self.__params
-
-    def get_param_from_filename(self, unit: str) -> float | None:
-        """
-        Extract param from filename with format <param><unit>, where param
-        is a float or integer and unit is a string. The param can be negative
-        with keyword 'minus' or a decimal point with keyword 'point'.
-
-        Args:
-            unit: str
-                unit of param to extract, e.g. dBm, mbar, V, etc.
-
-        Returns: float
-            extracted param from filename
-
-        Examples:
-            filename = "rabi_12dBm"
-            >>> get_param_from_filename(unit='dBm')
-            12.0
-
-            filename = "pixelscan_minus100nm"
-            >>> get_param_from_filename(unit='dBm')
-            -100.0
-
-            filename = "rabi_2e-6mbar"
-            >>> get_param_from_filename(unit='mbar')
-            2e-6
-
-            filename = "rabi_2point3uW"
-            >>> get_param_from_filename(unit='uW')
-            2.5
-        """
-        filename = self.filename
-        filename = filename.replace("point", ".")
-        filename = filename.replace("minus", "-")
-        params = re.search(rf"(-?\d+\.?\d*)(?={unit})", filename)
-
-        if params:
-            # Handle exponents in filename
-            if filename[params.start() - 1] == "e":
-                try:
-                    params = re.search(rf"(-?_\d)[^a]+?(?={unit})", filename).group(0)[1:]
-                    return float(params)
-                except AttributeError:
-                    raise Exception(f"Parameter with unit '{unit}' not found in filename '{filename}'")
-            else:
-                return float(params.group(0))
-        else:
-            self.log.warning(f"Unable to extract parameter from filename: {filename}")
-            return None
-
-    def set_datetime_index(self) -> pd.DataFrame:
-        if 'Start counting time' not in self.__params:
-            raise ValueError("'Start counting time' not in params")
-        if not isinstance(self.__data, pd.DataFrame):
-            raise TypeError("data is not of type pd.DataFrame")
-        if "Time (s)" not in self.__data.columns:
-            raise IndexError("Unable to find column 'Time (s)' in DataFrame")
-
-        self.__data['Time (s)'] += self.__params['Start counting time'].timestamp()
-        self.__data["Time"] = pd.to_datetime(self.__data['Time (s)'], unit='s', utc=True)
-        self.__data.set_index(self.__data["Time"], inplace=True)
-        self.__data.tz_convert('Europe/Berlin')
-        self.__data.drop(["Time", "Time (s)"], inplace=True, axis=1)
-        return self.__data
+from __future__ import annotations
+
+import logging
+import re
+from dataclasses import dataclass, field
+from pathlib import Path
+from typing import TYPE_CHECKING, Callable
+
+import pandas as pd
+
+if TYPE_CHECKING:
+    import datetime
+    import numpy as np
+    from PIL import Image
+
+logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
+
+
+@dataclass
+class PulsedMeasurement:
+    filepath: Path
+    loaders: (Callable, Callable) = field(default=None)
+    __data: pd.DataFrame = field(default=None)
+    __params: dict = field(default=None)
+
+    @property
+    def data(self) -> pd.DataFrame:
+        """ Read measurement data from file into pandas DataFrame """
+        if self.__data is None:
+            self.__data = self.loaders[0](self.filepath)
+        return self.__data
+
+    @property
+    def params(self) -> dict:
+        """ Read measurement params from file into dict """
+        if self.__params is None:
+            self.__params = self.loaders[1](self.filepath)
+        return self.__params
+
+
+@dataclass
+class LaserPulses:
+    filepath: Path
+    loaders: (Callable, Callable) = field(default=None)
+    __data: np.ndarray = field(default=None)
+    __params: dict = field(default=None)
+
+    @property
+    def data(self) -> np.ndarray:
+        """ Read measurement data from file into pandas DataFrame """
+        if self.__data is None:
+            self.__data = self.loaders[0](self.filepath)
+        return self.__data
+
+    @property
+    def params(self) -> dict:
+        """ Read measurement params from file into dict """
+        if self.__params is None:
+            self.__params = self.loaders[1](self.filepath)
+        return self.__params
+
+
+@dataclass
+class RawTimetrace:
+    filepath: Path
+    loaders: (Callable, Callable) = field(default=None)
+    __data: np.ndarray = field(default=None)
+    __params: dict = field(default=None)
+
+    @property
+    def data(self) -> np.ndarray:
+        """ Read measurement data from file into pandas DataFrame """
+        if self.__data is None:
+            self.__data = self.loaders[0](self.filepath)
+        return self.__data
+
+    @property
+    def params(self) -> dict:
+        """ Read measurement params from file into dict """
+        if self.__params is None:
+            self.__params = self.loaders[1](self.filepath)
+        return self.__params
+
+
+@dataclass
+class PulsedMeasurementDataclass:
+    measurement: PulsedMeasurement
+    laser_pulses: LaserPulses = field(default=None)
+    timetrace: RawTimetrace = field(default=None)
+
+    def __post_init__(self):
+        self.base_filename = self.measurement.filepath.name.replace("_pulsed_measurement.dat", "")
+
+    def show_image(self) -> Image:
+        """ Use PIL to open the measurement image saved on the disk """
+        return Image.open(str(self.measurement.filepath).replace(".dat", "_fig.png"))
+
+
+@dataclass
+class MeasurementDataclass:
+    timestamp: datetime.datetime
+    filepath: Path = field(default=None)
+    loaders: (Callable, Callable) = field(default=None)
+    pulsed: PulsedMeasurementDataclass = field(default=None)
+    __data: np.ndarray | pd.DataFrame = field(default=None)
+    __params: dict = field(default=None)
+
+    def __post_init__(self):
+        self.log = logging.getLogger(__name__)
+
+        if self.pulsed:
+            self.filename = self.pulsed.base_filename
+        else:
+            self.filename = self.filepath.name
+
+    def __repr__(self) -> str:
+
+        return f"Measurement(timestamp='{self.timestamp}', filename='{self.filename}')"
+
+    @property
+    def data(self) -> np.ndarray | pd.DataFrame:
+        """ Read measurement data from file into suitable data structure """
+        if self.pulsed:
+            return self.pulsed.measurement.data
+        else:
+            if self.__data is None:
+                self.__data = self.loaders[0](self.filepath)
+            return self.__data
+
+    @property
+    def params(self) -> dict:
+        """ Read measurement params from file into dict """
+        if self.pulsed:
+            return self.pulsed.measurement.params
+        else:
+            if self.__params is None:
+                self.__params = self.loaders[1](self.filepath)
+            return self.__params
+
+    def get_param_from_filename(self, unit: str) -> float | None:
+        """
+        Extract param from filename with format <param><unit>, where param
+        is a float or integer and unit is a string. The param can be negative
+        with keyword 'minus' or a decimal point with keyword 'point'.
+
+        Args:
+            unit: str
+                unit of param to extract, e.g. dBm, mbar, V, etc.
+
+        Returns: float
+            extracted param from filename
+
+        Examples:
+            filename = "rabi_12dBm"
+            >>> get_param_from_filename(unit='dBm')
+            12.0
+
+            filename = "pixelscan_minus100nm"
+            >>> get_param_from_filename(unit='dBm')
+            -100.0
+
+            filename = "rabi_2e-6mbar"
+            >>> get_param_from_filename(unit='mbar')
+            2e-6
+
+            filename = "rabi_2point3uW"
+            >>> get_param_from_filename(unit='uW')
+            2.5
+        """
+        filename = self.filename
+        filename = filename.replace("point", ".")
+        filename = filename.replace("minus", "-")
+        params = re.search(rf"(-?\d+\.?\d*)(?={unit})", filename)
+
+        if params:
+            # Handle exponents in filename
+            if filename[params.start() - 1] == "e":
+                try:
+                    params = re.search(rf"(-?_\d)[^a]+?(?={unit})", filename).group(0)[1:]
+                    return float(params)
+                except AttributeError:
+                    raise Exception(f"Parameter with unit '{unit}' not found in filename '{filename}'")
+            else:
+                return float(params.group(0))
+        else:
+            self.log.warning(f"Unable to extract parameter from filename: {filename}")
+            return None
+
+    def set_datetime_index(self) -> pd.DataFrame:
+        if 'Start counting time' not in self.__params:
+            raise ValueError("'Start counting time' not in params")
+        if not isinstance(self.__data, pd.DataFrame):
+            raise TypeError("data is not of type pd.DataFrame")
+        if "Time (s)" not in self.__data.columns:
+            raise IndexError("Unable to find column 'Time (s)' in DataFrame")
+
+        self.__data['Time (s)'] += self.__params['Start counting time'].timestamp()
+        self.__data["Time"] = pd.to_datetime(self.__data['Time (s)'], unit='s', utc=True)
+        self.__data.set_index(self.__data["Time"], inplace=True)
+        self.__data.tz_convert('Europe/Berlin')
+        self.__data.drop(["Time", "Time (s)"], inplace=True, axis=1)
+        return self.__data
```

### Comparing `qudi_hira_analysis-1.4.7/qudi_hira_analysis/qudi_fit_logic.py` & `qudi_hira_analysis-1.4.8/qudi_hira_analysis/qudi_fit_logic.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,427 +1,427 @@
-"""
-This file contains the Qudi FitLogic class, which provides all
-fitting methods imported from the files in logic/fitmethods.
-
-Qudi is free software: you can redistribute it and/or modify
-it under the terms of the GNU General Public License as published by
-the Free Software Foundation, either version 3 of the License, or
-(at your option) any later version.
-
-Qudi is distributed in the hope that it will be useful,
-but WITHOUT ANY WARRANTY; without even the implied warranty of
-MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-GNU General Public License for more details.
-
-You should have received a copy of the GNU General Public License
-along with Qudi. If not, see <http://www.gnu.org/licenses/>.
-
-Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
-top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
-"""
-
-import importlib
-import inspect
-import logging
-import os
-import sys
-from collections import OrderedDict
-from distutils.version import LooseVersion
-
-import lmfit
-import numpy as np
-
-logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
-
-
-class FitLogic:
-    """
-    Documentation to add a new fit model/estimator/function can be found in
-    documentation/how_to_use_fitting.md or in the online documentation at
-    http://qosvn.physik.uni-ulm.de/qudi-docs/fit_logic.html
-
-    This is the fitting class where fit functions are defined and methods are
-    implemented to process the data.
-
-    For clarity reasons the fit function are imported from different files
-    seperated by function type, e.g. gaussianlikemethods, sinemethods, generalmethods
-    """
-
-    # Optional additional paths to import from
-    _additional_methods_import_path = False
-
-    def __init__(self):
-        super().__init__()
-        # locking for thread safety
-
-        filenames = []
-        # for path in directories:
-        path_list = [os.path.join(os.path.dirname(os.path.realpath(__file__)), 'fitmethods')]
-        # adding additional path, to be defined in the config
-        self.log = logging.getLogger(__name__)
-
-        if self._additional_methods_import_path:
-            if isinstance(self._additional_methods_import_path, str):
-                self._additional_methods_import_path = [self._additional_methods_import_path]
-                self.log.info('Adding fit methods path: {}'.format(self._additional_methods_import_path))
-
-            if isinstance(self._additional_methods_import_path, (list, tuple, set)):
-                self.log.info('Adding fit methods path list: {}'.format(self._additional_methods_import_path))
-                for method_import_path in self._additional_methods_import_path:
-                    if not os.path.exists(method_import_path):
-                        self.log.error('Specified path "{0}" for import of additional fit methods '
-                                       'does not exist.'.format(method_import_path))
-                    else:
-                        path_list.append(method_import_path)
-            else:
-                self.log.error('ConfigOption additional_predefined_methods_path needs to either be a string or '
-                               'a list of strings.')
-
-        for path in path_list:
-            for f in os.listdir(path):
-                if os.path.isfile(os.path.join(path, f)) and f.endswith('.py'):
-                    filenames.append(f[:-3])
-                    if path not in sys.path:
-                        sys.path.append(path)
-
-        # A dictionary containing all fit methods and their estimators.
-        self.fit_list = OrderedDict()
-        self.fit_list['1d'] = OrderedDict()
-        self.fit_list['2d'] = OrderedDict()
-        self.fit_list['3d'] = OrderedDict()
-
-        # Go through the fitmethods files and import all methods.
-        # Also determine which methods need to be added to the fit_list dictionary
-        estimators_for_dict = list()
-        models_for_dict = list()
-        fits_for_dict = list()
-
-        for files in filenames:
-            mod = importlib.import_module('{0}'.format(files))
-            for method in dir(mod):
-                ref = getattr(mod, method)
-                if callable(ref) and (inspect.ismethod(ref) or inspect.isfunction(ref)):
-                    method_str = str(method)
-                    try:
-                        # import methods in Fitlogic
-                        setattr(FitLogic, method, ref)
-                        # append method to a list of methods to include in the fit_list dictionary
-                        if method_str.startswith('make_') and method_str.endswith('_fit'):
-                            fits_for_dict.append(method_str.split('_', 1)[1].rsplit('_', 1)[0])
-                        elif method_str.startswith('make_') and method_str.endswith('_model'):
-                            models_for_dict.append(method_str.split('_', 1)[1].rsplit('_', 1)[0])
-                        elif method_str.startswith('estimate_'):
-                            estimators_for_dict.append(method_str.split('_', 1)[1])
-                    except:
-                        self.log.error('Method "{0}" could not be imported to FitLogic.'
-                                       ''.format(str(method)))
-
-        fits_for_dict.sort()
-        models_for_dict.sort()
-        estimators_for_dict.sort()
-        # Now attach the fit, model and estimator methods to the proper dictionary fields
-        for fit_name in fits_for_dict:
-            fit_method = 'make_' + fit_name + '_fit'
-            model_method = 'make_' + fit_name + '_model'
-
-            # Determine fit dimension
-            if 'twoD' in fit_name:
-                dimension = '2d'
-            elif 'threeD' in fit_name:
-                dimension = '3d'
-            else:
-                dimension = '1d'
-
-            # Attach make_*_fit method to fit_list
-            if fit_name not in self.fit_list[dimension]:
-                self.fit_list[dimension][fit_name] = OrderedDict()
-            self.fit_list[dimension][fit_name]['make_fit'] = getattr(self, fit_method)
-
-            # Attach make_*_model method to fit_list
-            if fit_name in models_for_dict:
-                self.fit_list[dimension][fit_name]['make_model'] = getattr(self, model_method)
-            else:
-                self.log.error('No make_*_model method for fit "{0}" found in FitLogic.'
-                               ''.format(fit_name))
-
-            # Attach all estimate_* methods to corresponding fit method in fit_list
-            found_estimator = False
-            for estimator_name in estimators_for_dict:
-                estimator_method = 'estimate_' + estimator_name
-                if fit_name == estimator_name:
-                    self.fit_list[dimension][fit_name]['generic'] = getattr(self, estimator_method)
-                    found_estimator = True
-                elif estimator_name.startswith(fit_name + '_'):
-                    custom_name = estimator_name.split('_', 1)[1]
-                    self.fit_list[dimension][fit_name][custom_name] = getattr(self, estimator_method)
-                    found_estimator = True
-            if not found_estimator:
-                self.log.error('No estimator method for fit "{0}" found in FitLogic.'
-                               ''.format(fit_name))
-
-        # self.log.info('Methods were included to FitLogic, but only if naming is right: check the'
-        #               ' doxygen documentation if you added a new method and it does not show.')
-
-    def on_activate(self):
-        """ Initialisation performed during activation of the module.
-        """
-        # FIXME: load all the fits here, otherwise reloading this module is really questionable
-        fitversion = LooseVersion(lmfit.__version__)
-        if fitversion < LooseVersion('0.9.2'):
-            raise Exception('lmfit needs to be at least version 0.9.2!')
-
-    def on_deactivate(self):
-        """ """
-        pass
-
-    def validate_load_fits(self, fits):
-        """ Take fit names and estimators from a dict and check if they are valid.
-            @param fits dict: dictionary containing fit and estimator description
-
-            @return dict: checked dictionary with references to fit, model and estimator
-
-        The stored dictionary must have the following format.
-        There can be a parameter settings string included at the deepest level.
-        Example:
-        '1d':
-            'Two Lorentzian dips':
-                'fit_function': 'doublelorentzoffset'
-                'estimator': 'dip'
-
-        The returned dictionary has the following format (example):
-        '1d':
-            'Two Lorentzian dips':
-                'fit_name': 'doublelorentzoffset'
-                'est_name': 'dip'
-                'make_fit': function reference to fit function
-                'make_model': function reference to model function
-                'estimator': function reference to estimator function
-                'parameters': lmfit.parameter.Parameters object
-        """
-        user_fits = OrderedDict()
-        for dim, dfits in fits.items():
-            if dim not in ('1d', '2d', '3d'):
-                continue
-            user_fits[dim] = OrderedDict()
-            for name, fit in dfits.items():
-                try:
-                    fname = fit['fit_function']
-                    new_fit = {'fit_name': fname, 'est_name': fit['estimator'],
-                               'make_fit': self.fit_list[dim][fname]['make_fit'],
-                               'make_model': self.fit_list[dim][fname]['make_model'],
-                               'estimator': self.fit_list[dim][fname][fit['estimator']]}
-                    try:
-                        par = lmfit.parameter.Parameters()
-                        par.loads(fit['parameters'])
-                    except KeyError:
-                        model, par = self.fit_list[dim][fname]['make_model']()
-                    new_fit['parameters'] = par
-                    user_fits[dim][name] = new_fit
-                except KeyError:
-                    self.log.exception('Failed to validate fit {0}'.format(name))
-                    continue
-        return user_fits
-
-    def prepare_save_fits(self, fits):
-        """ Convert fit dictionary into a storable form.
-            @param fits dict: fit dictionary with function references and parameter objects
-
-            @return dict: storable fits description dictionary
-
-        For the format of this dictionary, ess validate_load_fits.
-        """
-        save_fits = OrderedDict()
-        for dim, dfits in fits.items():
-            if dim not in ('1d', '2d', '3d'):
-                continue
-            save_fits[dim] = OrderedDict()
-            for name, fit in dfits.items():
-                try:
-                    new_fit = {'fit_function': fit['fit_name'], 'estimator': fit['est_name'],
-                               'parameters': fit['parameters'].dumps()}
-                    save_fits[dim][name] = new_fit
-                except KeyError:
-                    self.log.exception('Error while preparing fit {0} for saving.'.format(name))
-                    continue
-        return save_fits
-
-    def make_fit_container(self, container_name, dimension):
-        """ Creare a fit container object.
-            @param container_name str: user-fiendly name for configurable fit
-            @param dimension str: dimension of fit input data ('1d', '2d' od '3d')
-
-            @return FitContainer: fit container object
-
-        This is a convenience function so you do not have to mess with an extra import in modules
-        using FitLogic.
-        """
-
-        return FitContainer(self, container_name, dimension)
-
-
-class FitContainer():
-    """ A class for managing a single flexible fit setting in a logic module.
-    """
-
-    def __init__(self, fit_logic, name, dimension):
-        """ Create a fit container.
-
-            @param fit_logic FitLogic: reference to a FitLogic instance
-            @param name str: user-friendly name for this container
-            @param dimension str: dimension for fit input in this container, '1d', '2d' or '3d'
-        """
-        super().__init__()
-
-        self.fit_logic = fit_logic
-        self.name = name
-        if dimension == '1d':
-            self.dim = 1
-        elif dimension == '2d':
-            self.dim = 2
-        elif dimension == '3d':
-            self.dim = 3
-        else:
-            raise Exception('Invalid dimension {0}'.format(dimension))
-        self.dimension = dimension
-        self.fit_list = OrderedDict()
-        # variables for fitting
-        self.fit_granularity_fact = 10
-        self.current_fit = 'No Fit'
-        self.current_fit_param = lmfit.parameter.Parameters()
-        self.current_fit_result = None
-        self.use_settings = None
-        self.units = ['independent variable {0}'.format(i + 1) for i in range(self.dim)]
-        self.units.append('dependent variable')
-
-    def set_units(self, units):
-        """ Set units for this fit.
-            @param units list(str): list of units (for x axes and y axis)
-
-            Number of units must be = dimensions + 1
-        """
-        if len(units) == self.dim + 1:
-            self.units = units
-
-    def load_from_dict(self, fit_dict):
-        """ Take a list of fits from a storable dictionary, load to self.fit_list and check.
-            @param fit_dict dict: fit dictionary with function references etc
-
-        """
-        try:
-            self.fit_list = self.fit_logic.validate_load_fits(fit_dict)[self.dimension]
-        except KeyError:
-            self.fit_list = OrderedDict()
-
-    def save_to_dict(self):
-        """ Convert self.fit_list to a storable dictionary.
-
-            @return dict: storable configured fits dictionary
-        """
-        prep = self.fit_logic.prepare_save_fits({self.dimension: self.fit_list})
-        return prep
-
-    def clear_result(self):
-        """ Reset fit result and fit parameters from result for this container.
-        """
-        self.current_fit_param = lmfit.parameter.Parameters()
-        self.current_fit_result = None
-
-    def set_fit_functions(self, fit_functions):
-        """ Set the configured fit functions for this container.
-            @param fit_functions dict: configured fit functions dictionary
-        """
-        self.fit_list = fit_functions
-        self.set_current_fit(self.current_fit)
-
-    def set_current_fit(self, current_fit):
-        """ Check and set the current fit for this container by name.
-            @param current_fit str: name of configured fit to be used as current fit
-
-        If the name given is not in the list of fits, the current fit will be 'No Fit'.
-        This is a reserved name that will do nothing and should not display a fit line if set.
-        """
-        if current_fit not in self.fit_list and current_fit != 'No Fit':
-            self.fit_logic.log.warning('{0} not in {1} fit list!'.format(current_fit, self.name))
-            self.current_fit = 'No Fit'
-        else:
-            self.current_fit = current_fit
-            if current_fit != 'No Fit':
-                use_settings = self.fit_list[self.current_fit]['use_settings']
-                self.use_settings = lmfit.parameter.Parameters()
-                # Update the use parameter dictionary
-                for para in use_settings:
-                    if use_settings[para]:
-                        self.use_settings[para] = self.fit_list[self.current_fit]['parameters'][para]
-            else:
-                self.use_settings = None
-        self.clear_result()
-        return self.current_fit, self.use_settings
-
-    def do_fit(self, x_data, y_data):
-        """Performs the chosen fit on the measured data.
-        @param array x_data: optional, 1D np.array or 1D list with the x values.
-                             If None is passed then the module x values are
-                             taken.
-        @param array y_data: optional, 1D np.array or 1D list with the y values.
-                             If None is passed then the module y values are
-                             taken. If passed, then it should have the same size
-                             as x_data.
-
-        @return: tuple (fit_x, fit_y, str_dict, fit_result)
-            np.array fit_x: 1D array containing the x values of the fit
-            np.array fit_y: 1D array containing the y values of the fit
-            OrderedDict str_dict: a dictionary with the relevant fit
-                                    parameters, i.e. the result of the fit. Each
-                                    entry is again a dict with three entries,
-                                        {'value': ... , 'error': ...., 'unit': '...'}
-                                    The values and the errors are always saved
-                                    in SI units!
-
-            lmfit.model.ModelResult fit_result:
-                            the result object of lmfit. If additional
-                            information is needed from the fit, then they can be
-                            obtained from this object. If no fit is performed
-                            then result is set to None.
-        """
-        self.clear_result()
-
-        fit_x = np.linspace(
-            start=x_data[0],
-            stop=x_data[-1],
-            num=int(len(x_data) * self.fit_granularity_fact))
-
-        # set the keyword arguments, which will be passed to the fit.
-        kwargs = {
-            'x_axis': x_data,
-            'data': y_data,
-            'units': self.units,
-            'add_params': self.use_settings}
-
-        result = None
-
-        if self.current_fit in self.fit_list:
-            result = self.fit_list[self.current_fit]['make_fit'](
-                estimator=self.fit_list[self.current_fit]['estimator'],
-                **kwargs)
-
-        elif self.current_fit == 'No Fit':
-            fit_y = np.zeros(fit_x.shape)
-
-        else:
-            self.fit_logic.log.warning(
-                'The Fit Function "{0}" is not implemented to be used in the ODMR Logic. '
-                'Correct that! Fit Call will be skipped and Fit Function will be set to '
-                '"No Fit".'.format(self.current_fit))
-
-            self.current_fit = 'No Fit'
-
-        if self.current_fit != 'No Fit':
-            # after the fit was performed, retrieve the fitting function and
-            # evaluate the fitted parameters according to the function:
-            model, params = self.fit_list[self.current_fit]['make_model']()
-            fit_y = model.eval(x=fit_x, params=result.params)
-
-        if result is not None:
-            self.current_fit_param = result.params
-            self.current_fit_result = result
-
-        return fit_x, fit_y, result
+"""
+This file contains the Qudi FitLogic class, which provides all
+fitting methods imported from the files in logic/fitmethods.
+
+Qudi is free software: you can redistribute it and/or modify
+it under the terms of the GNU General Public License as published by
+the Free Software Foundation, either version 3 of the License, or
+(at your option) any later version.
+
+Qudi is distributed in the hope that it will be useful,
+but WITHOUT ANY WARRANTY; without even the implied warranty of
+MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License
+along with Qudi. If not, see <http://www.gnu.org/licenses/>.
+
+Copyright (c) the Qudi Developers. See the COPYRIGHT.txt file at the
+top-level directory of this distribution and at <https://github.com/Ulm-IQO/qudi/>
+"""
+
+import importlib
+import inspect
+import logging
+import os
+import sys
+from collections import OrderedDict
+from distutils.version import LooseVersion
+
+import lmfit
+import numpy as np
+
+logging.basicConfig(format='%(name)s :: %(levelname)s :: %(message)s', level=logging.INFO)
+
+
+class FitLogic:
+    """
+    Documentation to add a new fit model/estimator/function can be found in
+    documentation/how_to_use_fitting.md or in the online documentation at
+    http://qosvn.physik.uni-ulm.de/qudi-docs/fit_logic.html
+
+    This is the fitting class where fit functions are defined and methods are
+    implemented to process the data.
+
+    For clarity reasons the fit function are imported from different files
+    seperated by function type, e.g. gaussianlikemethods, sinemethods, generalmethods
+    """
+
+    # Optional additional paths to import from
+    _additional_methods_import_path = False
+
+    def __init__(self):
+        super().__init__()
+        # locking for thread safety
+
+        filenames = []
+        # for path in directories:
+        path_list = [os.path.join(os.path.dirname(os.path.realpath(__file__)), 'fitmethods')]
+        # adding additional path, to be defined in the config
+        self.log = logging.getLogger(__name__)
+
+        if self._additional_methods_import_path:
+            if isinstance(self._additional_methods_import_path, str):
+                self._additional_methods_import_path = [self._additional_methods_import_path]
+                self.log.info('Adding fit methods path: {}'.format(self._additional_methods_import_path))
+
+            if isinstance(self._additional_methods_import_path, (list, tuple, set)):
+                self.log.info('Adding fit methods path list: {}'.format(self._additional_methods_import_path))
+                for method_import_path in self._additional_methods_import_path:
+                    if not os.path.exists(method_import_path):
+                        self.log.error('Specified path "{0}" for import of additional fit methods '
+                                       'does not exist.'.format(method_import_path))
+                    else:
+                        path_list.append(method_import_path)
+            else:
+                self.log.error('ConfigOption additional_predefined_methods_path needs to either be a string or '
+                               'a list of strings.')
+
+        for path in path_list:
+            for f in os.listdir(path):
+                if os.path.isfile(os.path.join(path, f)) and f.endswith('.py'):
+                    filenames.append(f[:-3])
+                    if path not in sys.path:
+                        sys.path.append(path)
+
+        # A dictionary containing all fit methods and their estimators.
+        self.fit_list = OrderedDict()
+        self.fit_list['1d'] = OrderedDict()
+        self.fit_list['2d'] = OrderedDict()
+        self.fit_list['3d'] = OrderedDict()
+
+        # Go through the fitmethods files and import all methods.
+        # Also determine which methods need to be added to the fit_list dictionary
+        estimators_for_dict = list()
+        models_for_dict = list()
+        fits_for_dict = list()
+
+        for files in filenames:
+            mod = importlib.import_module('{0}'.format(files))
+            for method in dir(mod):
+                ref = getattr(mod, method)
+                if callable(ref) and (inspect.ismethod(ref) or inspect.isfunction(ref)):
+                    method_str = str(method)
+                    try:
+                        # import methods in Fitlogic
+                        setattr(FitLogic, method, ref)
+                        # append method to a list of methods to include in the fit_list dictionary
+                        if method_str.startswith('make_') and method_str.endswith('_fit'):
+                            fits_for_dict.append(method_str.split('_', 1)[1].rsplit('_', 1)[0])
+                        elif method_str.startswith('make_') and method_str.endswith('_model'):
+                            models_for_dict.append(method_str.split('_', 1)[1].rsplit('_', 1)[0])
+                        elif method_str.startswith('estimate_'):
+                            estimators_for_dict.append(method_str.split('_', 1)[1])
+                    except:
+                        self.log.error('Method "{0}" could not be imported to FitLogic.'
+                                       ''.format(str(method)))
+
+        fits_for_dict.sort()
+        models_for_dict.sort()
+        estimators_for_dict.sort()
+        # Now attach the fit, model and estimator methods to the proper dictionary fields
+        for fit_name in fits_for_dict:
+            fit_method = 'make_' + fit_name + '_fit'
+            model_method = 'make_' + fit_name + '_model'
+
+            # Determine fit dimension
+            if 'twoD' in fit_name:
+                dimension = '2d'
+            elif 'threeD' in fit_name:
+                dimension = '3d'
+            else:
+                dimension = '1d'
+
+            # Attach make_*_fit method to fit_list
+            if fit_name not in self.fit_list[dimension]:
+                self.fit_list[dimension][fit_name] = OrderedDict()
+            self.fit_list[dimension][fit_name]['make_fit'] = getattr(self, fit_method)
+
+            # Attach make_*_model method to fit_list
+            if fit_name in models_for_dict:
+                self.fit_list[dimension][fit_name]['make_model'] = getattr(self, model_method)
+            else:
+                self.log.error('No make_*_model method for fit "{0}" found in FitLogic.'
+                               ''.format(fit_name))
+
+            # Attach all estimate_* methods to corresponding fit method in fit_list
+            found_estimator = False
+            for estimator_name in estimators_for_dict:
+                estimator_method = 'estimate_' + estimator_name
+                if fit_name == estimator_name:
+                    self.fit_list[dimension][fit_name]['generic'] = getattr(self, estimator_method)
+                    found_estimator = True
+                elif estimator_name.startswith(fit_name + '_'):
+                    custom_name = estimator_name.split('_', 1)[1]
+                    self.fit_list[dimension][fit_name][custom_name] = getattr(self, estimator_method)
+                    found_estimator = True
+            if not found_estimator:
+                self.log.error('No estimator method for fit "{0}" found in FitLogic.'
+                               ''.format(fit_name))
+
+        # self.log.info('Methods were included to FitLogic, but only if naming is right: check the'
+        #               ' doxygen documentation if you added a new method and it does not show.')
+
+    def on_activate(self):
+        """ Initialisation performed during activation of the module.
+        """
+        # FIXME: load all the fits here, otherwise reloading this module is really questionable
+        fitversion = LooseVersion(lmfit.__version__)
+        if fitversion < LooseVersion('0.9.2'):
+            raise Exception('lmfit needs to be at least version 0.9.2!')
+
+    def on_deactivate(self):
+        """ """
+        pass
+
+    def validate_load_fits(self, fits):
+        """ Take fit names and estimators from a dict and check if they are valid.
+            @param fits dict: dictionary containing fit and estimator description
+
+            @return dict: checked dictionary with references to fit, model and estimator
+
+        The stored dictionary must have the following format.
+        There can be a parameter settings string included at the deepest level.
+        Example:
+        '1d':
+            'Two Lorentzian dips':
+                'fit_function': 'doublelorentzoffset'
+                'estimator': 'dip'
+
+        The returned dictionary has the following format (example):
+        '1d':
+            'Two Lorentzian dips':
+                'fit_name': 'doublelorentzoffset'
+                'est_name': 'dip'
+                'make_fit': function reference to fit function
+                'make_model': function reference to model function
+                'estimator': function reference to estimator function
+                'parameters': lmfit.parameter.Parameters object
+        """
+        user_fits = OrderedDict()
+        for dim, dfits in fits.items():
+            if dim not in ('1d', '2d', '3d'):
+                continue
+            user_fits[dim] = OrderedDict()
+            for name, fit in dfits.items():
+                try:
+                    fname = fit['fit_function']
+                    new_fit = {'fit_name': fname, 'est_name': fit['estimator'],
+                               'make_fit': self.fit_list[dim][fname]['make_fit'],
+                               'make_model': self.fit_list[dim][fname]['make_model'],
+                               'estimator': self.fit_list[dim][fname][fit['estimator']]}
+                    try:
+                        par = lmfit.parameter.Parameters()
+                        par.loads(fit['parameters'])
+                    except KeyError:
+                        model, par = self.fit_list[dim][fname]['make_model']()
+                    new_fit['parameters'] = par
+                    user_fits[dim][name] = new_fit
+                except KeyError:
+                    self.log.exception('Failed to validate fit {0}'.format(name))
+                    continue
+        return user_fits
+
+    def prepare_save_fits(self, fits):
+        """ Convert fit dictionary into a storable form.
+            @param fits dict: fit dictionary with function references and parameter objects
+
+            @return dict: storable fits description dictionary
+
+        For the format of this dictionary, ess validate_load_fits.
+        """
+        save_fits = OrderedDict()
+        for dim, dfits in fits.items():
+            if dim not in ('1d', '2d', '3d'):
+                continue
+            save_fits[dim] = OrderedDict()
+            for name, fit in dfits.items():
+                try:
+                    new_fit = {'fit_function': fit['fit_name'], 'estimator': fit['est_name'],
+                               'parameters': fit['parameters'].dumps()}
+                    save_fits[dim][name] = new_fit
+                except KeyError:
+                    self.log.exception('Error while preparing fit {0} for saving.'.format(name))
+                    continue
+        return save_fits
+
+    def make_fit_container(self, container_name, dimension):
+        """ Creare a fit container object.
+            @param container_name str: user-fiendly name for configurable fit
+            @param dimension str: dimension of fit input data ('1d', '2d' od '3d')
+
+            @return FitContainer: fit container object
+
+        This is a convenience function so you do not have to mess with an extra import in modules
+        using FitLogic.
+        """
+
+        return FitContainer(self, container_name, dimension)
+
+
+class FitContainer():
+    """ A class for managing a single flexible fit setting in a logic module.
+    """
+
+    def __init__(self, fit_logic, name, dimension):
+        """ Create a fit container.
+
+            @param fit_logic FitLogic: reference to a FitLogic instance
+            @param name str: user-friendly name for this container
+            @param dimension str: dimension for fit input in this container, '1d', '2d' or '3d'
+        """
+        super().__init__()
+
+        self.fit_logic = fit_logic
+        self.name = name
+        if dimension == '1d':
+            self.dim = 1
+        elif dimension == '2d':
+            self.dim = 2
+        elif dimension == '3d':
+            self.dim = 3
+        else:
+            raise Exception('Invalid dimension {0}'.format(dimension))
+        self.dimension = dimension
+        self.fit_list = OrderedDict()
+        # variables for fitting
+        self.fit_granularity_fact = 10
+        self.current_fit = 'No Fit'
+        self.current_fit_param = lmfit.parameter.Parameters()
+        self.current_fit_result = None
+        self.use_settings = None
+        self.units = ['independent variable {0}'.format(i + 1) for i in range(self.dim)]
+        self.units.append('dependent variable')
+
+    def set_units(self, units):
+        """ Set units for this fit.
+            @param units list(str): list of units (for x axes and y axis)
+
+            Number of units must be = dimensions + 1
+        """
+        if len(units) == self.dim + 1:
+            self.units = units
+
+    def load_from_dict(self, fit_dict):
+        """ Take a list of fits from a storable dictionary, load to self.fit_list and check.
+            @param fit_dict dict: fit dictionary with function references etc
+
+        """
+        try:
+            self.fit_list = self.fit_logic.validate_load_fits(fit_dict)[self.dimension]
+        except KeyError:
+            self.fit_list = OrderedDict()
+
+    def save_to_dict(self):
+        """ Convert self.fit_list to a storable dictionary.
+
+            @return dict: storable configured fits dictionary
+        """
+        prep = self.fit_logic.prepare_save_fits({self.dimension: self.fit_list})
+        return prep
+
+    def clear_result(self):
+        """ Reset fit result and fit parameters from result for this container.
+        """
+        self.current_fit_param = lmfit.parameter.Parameters()
+        self.current_fit_result = None
+
+    def set_fit_functions(self, fit_functions):
+        """ Set the configured fit functions for this container.
+            @param fit_functions dict: configured fit functions dictionary
+        """
+        self.fit_list = fit_functions
+        self.set_current_fit(self.current_fit)
+
+    def set_current_fit(self, current_fit):
+        """ Check and set the current fit for this container by name.
+            @param current_fit str: name of configured fit to be used as current fit
+
+        If the name given is not in the list of fits, the current fit will be 'No Fit'.
+        This is a reserved name that will do nothing and should not display a fit line if set.
+        """
+        if current_fit not in self.fit_list and current_fit != 'No Fit':
+            self.fit_logic.log.warning('{0} not in {1} fit list!'.format(current_fit, self.name))
+            self.current_fit = 'No Fit'
+        else:
+            self.current_fit = current_fit
+            if current_fit != 'No Fit':
+                use_settings = self.fit_list[self.current_fit]['use_settings']
+                self.use_settings = lmfit.parameter.Parameters()
+                # Update the use parameter dictionary
+                for para in use_settings:
+                    if use_settings[para]:
+                        self.use_settings[para] = self.fit_list[self.current_fit]['parameters'][para]
+            else:
+                self.use_settings = None
+        self.clear_result()
+        return self.current_fit, self.use_settings
+
+    def do_fit(self, x_data, y_data):
+        """Performs the chosen fit on the measured data.
+        @param array x_data: optional, 1D np.array or 1D list with the x values.
+                             If None is passed then the module x values are
+                             taken.
+        @param array y_data: optional, 1D np.array or 1D list with the y values.
+                             If None is passed then the module y values are
+                             taken. If passed, then it should have the same size
+                             as x_data.
+
+        @return: tuple (fit_x, fit_y, str_dict, fit_result)
+            np.array fit_x: 1D array containing the x values of the fit
+            np.array fit_y: 1D array containing the y values of the fit
+            OrderedDict str_dict: a dictionary with the relevant fit
+                                    parameters, i.e. the result of the fit. Each
+                                    entry is again a dict with three entries,
+                                        {'value': ... , 'error': ...., 'unit': '...'}
+                                    The values and the errors are always saved
+                                    in SI units!
+
+            lmfit.model.ModelResult fit_result:
+                            the result object of lmfit. If additional
+                            information is needed from the fit, then they can be
+                            obtained from this object. If no fit is performed
+                            then result is set to None.
+        """
+        self.clear_result()
+
+        fit_x = np.linspace(
+            start=x_data[0],
+            stop=x_data[-1],
+            num=int(len(x_data) * self.fit_granularity_fact))
+
+        # set the keyword arguments, which will be passed to the fit.
+        kwargs = {
+            'x_axis': x_data,
+            'data': y_data,
+            'units': self.units,
+            'add_params': self.use_settings}
+
+        result = None
+
+        if self.current_fit in self.fit_list:
+            result = self.fit_list[self.current_fit]['make_fit'](
+                estimator=self.fit_list[self.current_fit]['estimator'],
+                **kwargs)
+
+        elif self.current_fit == 'No Fit':
+            fit_y = np.zeros(fit_x.shape)
+
+        else:
+            self.fit_logic.log.warning(
+                'The Fit Function "{0}" is not implemented to be used in the ODMR Logic. '
+                'Correct that! Fit Call will be skipped and Fit Function will be set to '
+                '"No Fit".'.format(self.current_fit))
+
+            self.current_fit = 'No Fit'
+
+        if self.current_fit != 'No Fit':
+            # after the fit was performed, retrieve the fitting function and
+            # evaluate the fitted parameters according to the function:
+            model, params = self.fit_list[self.current_fit]['make_model']()
+            fit_y = model.eval(x=fit_x, params=result.params)
+
+        if result is not None:
+            self.current_fit_param = result.params
+            self.current_fit_result = result
+
+        return fit_x, fit_y, result
```

### Comparing `qudi_hira_analysis-1.4.7/PKG-INFO` & `qudi_hira_analysis-1.4.8/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,407 +1,37 @@
-Metadata-Version: 2.1
-Name: qudi-hira-analysis
-Version: 1.4.7
-Summary: A Python toolkit to analzye photon timetrace data from qubit sensors
-Home-page: https://github.com/dineshpinto/qudi-hira-analysis
-License: MIT
-Keywords: python,qubit,analysis,nv centers,photon timetrace
-Author: dineshpinto
-Author-email: annual.fallout_0z@icloud.com
-Requires-Python: >=3.10,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: lmfit (>=1.1.0,<2.0.0)
-Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.10,<4.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: pyspm (>=0.3.0,<0.4.0)
-Requires-Dist: tqdm (>=4.64.1,<5.0.0)
-Requires-Dist: xlrd (>=2.0.1,<3.0.0)
-Project-URL: Repository, https://github.com/dineshpinto/qudi-hira-analysis
-Description-Content-Type: text/markdown
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
-[![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)
-[![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)
-[![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)
-[![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)
-[![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)
-[![codecov](https://codecov.io/gh/dineshpinto/qudi-hira-analysis/branch/main/graph/badge.svg?token=FMXDAYW8DW)](https://codecov.io/gh/dineshpinto/qudi-hira-analysis)
+packages = \
+['qudi_hira_analysis', 'qudi_hira_analysis.fitmethods']
 
-# Qudi Hira Analysis
+package_data = \
+{'': ['*']}
 
-This toolkit automates a large portion of the work surrounding data analysis on quantum sensing experiments where the
-primary raw data extracted is photon counts.
+install_requires = \
+['lmfit>=1.1.0,<2.0.0',
+ 'matplotlib>=3.6.2,<4.0.0',
+ 'numpy>=1.24.0,<2.0.0',
+ 'openpyxl>=3.0.10,<4.0.0',
+ 'pandas>=2.0.0,<3.0.0',
+ 'pyspm>=0.3.0,<0.4.0',
+ 'tqdm>=4.64.1,<5.0.0',
+ 'xlrd>=2.0.1,<3.0.0']
+
+setup_kwargs = {
+    'name': 'qudi-hira-analysis',
+    'version': '1.4.8',
+    'description': 'A Python toolkit to analzye photon timetrace data from qubit sensors',
+    'long_description': '[![DOI](https://zenodo.org/badge/288670453.svg)](https://zenodo.org/badge/latestdoi/288670453)\n[![Downloads](https://pepy.tech/badge/qudi-hira-analysis)](https://pepy.tech/project/qudi-hira-analysis)\n[![PyPi version](https://img.shields.io/pypi/v/qudi-hira-analysis)](https://pypi.python.org/pypi/qudi-hira-analysis/)\n[![Python 3.10](https://img.shields.io/badge/python-3.10-orange.svg)](https://www.python.org/downloads/release/python-3100//)\n[![Python 3.11](https://img.shields.io/badge/python-3.11-orange.svg)](https://www.python.org/downloads/release/python-3110//)\n[![codecov](https://codecov.io/gh/dineshpinto/qudi-hira-analysis/branch/main/graph/badge.svg?token=FMXDAYW8DW)](https://codecov.io/gh/dineshpinto/qudi-hira-analysis)\n\n# Qudi Hira Analysis\n\nThis toolkit automates a large portion of the work surrounding data analysis on quantum sensing experiments where the\nprimary raw data extracted is photon counts.\n\nThe high level interface is abstracted, and provides a set of functions to automate data import, handling and analysis.\nIt is designed to be exposed through Jupyter Notebooks, although the abstract interface allows it to be integrated into\nlarger, more general frameworks as well (with only some pain). Using the toolkit itself should only require a\nbeginner-level understanding of Python.\n\nIt also aims to improve transparency and reproducibility in experimental data analysis. In an ideal scenario,\ntwo lines of code are sufficient to recreate all output data.\n\nPython offers some very handy features like dataclasses, which are heavily used by this toolkit. Dataclasses offer a\nfull OOP (object-oriented programming) experience while analyzing complex data sets. They provide a solid and\ntransparent structure to the data to\nreduce errors arising from data fragmentation. This generally comes at a large performance cost, but this is (largely)\nsidestepped by lazy loading data and storing metadata instead wherever possible.\n\n## Installation\n\n```bash\npip install qudi-hira-analysis\n```\n\n### Update to latest version\n\n```bash\npip install --upgrade qudi-hira-analysis\n```\n\n## Citation\n\nIf you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670\n\n## Examples\n\nFirst set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure\nfolders.\n\nEverything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the\nfollowing required arguments:\n\n- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of\n  several sub-folders, each containing the data for a specific measurement\n- `figure_folder` is the folder where the output figures will be saved\n\nOptional arguments:\n\n- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored\n\n```python\nfrom pathlib import Path\nimport matplotlib.pyplot as plt\nimport seaborn as sns\n\nfrom qudi_hira_analysis import DataHandler\n\ndh = DataHandler(\n    data_folder=Path("C:\\\\", "Data"),\n    figure_folder=Path("C:\\\\", "QudiHiraAnalysis"),\n    measurement_folder=Path("20230101_NV1")\n)\n```\n\nTo load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the\nfollowing required arguments:\n\n- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the\n  `data_folder` and `measurement_folder` (if specified)\n\nOptional arguments:\n\n- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)\n- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (\n  default: False)\n- `extension` is the extension of the data files (default: ".dat")\n\nThe `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.\n\n- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.\n\n- The dictionary values are `MeasurementDataclass` objects whose schema is shown\n  visually [here](#measurement-dataclass-schema).\n\n### Example 0: NV-PL measurements\n\n```python\npixel_scanner_measurements = dh.load_measurements(measurement_str="PixelScanner")\n\nfwd, bwd = pixel_scanner_measurements["20230101-0420-00"].data\n\n# If size is known, it can be specified here\nfwd.size["real"] = {"x": 1e-6, "y": 1e-6, "unit": "m"}\n\nfig, ax = plt.subplots()\n\n# Perform (optional) image corrections\nfwd.filter_gaussian(sigma=0.5)\n\n# Add scale bar, color bar and plot the data\nimg = fwd.show(cmap="inferno", ax=ax)\nfwd.add_scale(length=1e-6, ax=ax, height=1)\ncbar = fig.colorbar(img)\ncbar.set_label("NV-PL (kcps)")\n\n# Save the figure to the figure folder specified earlier\ndh.save_figures(filepath="nv_pl_scan", fig=fig, only_jpg=True)\n```\n\n### Example 1: Nanonis AFM measurements\n\n```python\nafm_measurements = dh.load_measurements(measurement_str="Scan", extension=".sxm")\n\nafm = afm_measurements["20230101-0420-00"].data\n\n# Print the channels available in the data\nafm.list_channels()\ntopo = afm.get_channel("Z")\n\nfig, ax = plt.subplots()\n\n# Perform (optional) image corrections\ntopo.correct_lines()\ntopo.correct_plane()\ntopo.filter_lowpass(fft_radius=20)\ntopo.zero_min()\n\n# Add scale bar, color bar and plot the data\nimg = topo.show(cmap="inferno", ax=ax)\ntopo.add_scale(length=1e-6, ax=ax, height=1, fontsize=10)\ncbar = fig.colorbar(img)\ncbar.set_label("Height (nm)")\n\ndh.save_figures(filepath="afm_topo", fig=fig, only_jpg=True)\n``` \n\n### Example 2: Autocorrelation measurements (Antibunching fit)\n\n```python\nautocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")\n\nfig, ax = plt.subplots()\n\nfor autocorrelation in autocorrelation_measurements.values():\n    autocorrelation.data["Time (ns)"] = autocorrelation.data["Time (ps)"] * 1e-3\n    # Plot the data\n    sns.lineplot(data=autocorrelation.data, x="Time (ns)", y="g2(t) norm", ax=ax)\n    # Fit the data using the antibunching function\n    fit_x, fit_y, result = dh.fit(x="Time (ns)", y="g2(t) norm", data=autocorrelation.data,\n                                  fit_function=dh.fit_function.antibunching)\n    # Plot the fit\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")\n\n# Save the figure to the figure folder specified earlier\ndh.save_figures(filepath="autocorrelation_variation", fig=fig)\n```\n\n### Example 3: ODMR measurements (double Lorentzian fit)\n\n```python\nodmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor odmr in odmr_measurements.values():\n    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,\n                                  fit_function=dh.fit_function.lorentziandouble)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")\n\ndh.save_figures(filepath="odmr_variation", fig=fig)\n```\n\n### Example 4: Rabi measurements (sine exponential decay fit)\n\n```python\nrabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)\n\nfig, ax = plt.subplots()\n\nfor rabi in rabi_measurements.values():\n    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)\n    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,\n                                  fit_function=dh.fit_function.sineexponentialdecay)\n    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")\n\ndh.save_figures(filepath="rabi_variation", fig=fig)\n```\n\n### Example 5: Temperature data\n\n```python\ntemperature_measurements = dh.load_measurements(measurement_str="Temperature", qudi=False)\n\ntemperature = pd.concat([t.data for t in temperature_measurements.values()])\n\nfig, ax = plt.subplots()\nsns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)\ndh.save_figures(filepath="temperature_monitoring", fig=fig)\n```\n\n### Example 6: PYS data (pi3diamond compatibility)\n\n```python\npys_measurements = dh.load_measurements(measurement_str="ndmin", extension=".pys", qudi=False)\npys = pys_measurements[list(pys_measurements)[0]].data\n\nfig, ax = plt.subplots()\nsns.lineplot(x=pys["time_bins"], y=pys["counts"], ax=ax)\ndh.save_figures(filepath="pys_measurement", fig=fig)\n```\n\n## Measurement Dataclass Schema\n\n```mermaid\nflowchart LR\n    subgraph Standard Data\n        MeasurementDataclass --o filepath1[filepath: Path];\n        MeasurementDataclass --o data1[data: DataFrame];\n        MeasurementDataclass --o params1[params: dict];\n        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];\n        MeasurementDataclass --o methods1[get_param_from_filename: Callable];\n        MeasurementDataclass --o methods2[set_datetime_index: Callable];\n    end\n    subgraph Pulsed Data\n        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;\n        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;\n        PulsedMeasurement --o filepath2[filepath: Path];\n        PulsedMeasurement --o data2[data: DataFrame];\n        PulsedMeasurement --o params2[params: dict];\n        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;\n        LaserPulses --o filepath3[filepath: Path];\n        LaserPulses --o data3[data: DataFrame];\n        LaserPulses --o params3[params: dict];\n        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;\n        RawTimetrace --o filepath4[filepath: Path];\n        RawTimetrace --o data4[data: DataFrame];\n        RawTimetrace --o params4[params: dict];\n    end\n```\n\n## Supports common fitting routines\n\nTo get the full list of available fit routines, explore the `dh.fit_function` attribute or call `dh.get_all_fits()`. The\nfit functions are:\n\n| Dimension | Fit                           |\n|-----------|-------------------------------|\n| 1d        | decayexponential              |\n|           | biexponential                 |\n|           | decayexponentialstretched     |\n|           | gaussian                      |\n|           | gaussiandouble                |\n|           | gaussianlinearoffset          |\n|           | hyperbolicsaturation          |\n|           | linear                        |\n|           | lorentzian                    |\n|           | lorentziandouble              |\n|           | lorentziantriple              |\n|           | sine                          |\n|           | sinedouble                    |\n|           | sinedoublewithexpdecay        |\n|           | sinedoublewithtwoexpdecay     |\n|           | sineexponentialdecay          |\n|           | sinestretchedexponentialdecay |\n|           | sinetriple                    |\n|           | sinetriplewithexpdecay        |\n|           | sinetriplewiththreeexpdecay   |\n| 2d        | twoDgaussian                  |\n\n## Inbuilt measurement tree visualizer\n\n```ipython\n>>> dh.data_folder_tree()\n\n# Output\n├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv\n├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv\n├── 20211116_NetworkAnalysis_TipOut_UpperPin.csv\n├── ContactTestingMeasurementHead\n│   ├── C2_Reference.txt\n│   ├── C2_SampleLowerPin.txt\n│   ├── C2_SampleUpperPin.txt\n│   ├── C2_TipLowerPin.txt\n│   └── C2_TipUpperPin.txt\n├── Sample_MW_Pin_comparision.png\n├── Tip_MW_Pin_comparision.png\n└── Tip_Sample_MW_Pin_comparision.png\n```\n\n## Overall Schema\n\n```mermaid\nflowchart TD\n    IOHandler <-- Handle IO operations --> DataLoader;\n    DataLoader <-- Map IO callables --> DataHandler;\n    Qudi[Qudi FitLogic] --> AnalysisLogic;\n    AnalysisLogic -- Inject fit functions --> DataHandler;\n    DataHandler -- Fit data --> Plot;\n    DataHandler -- Structure data --> MeasurementDataclass;\n    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];\n    Plot -- Save plotted data --> DataHandler;\n    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5\n```\n\n## License\n\nThis license of this project is located in the top level folder under `LICENSE`. Some specific files contain their\nindividual licenses in the file header docstring.\n\n## Build\n\n### Prerequisites\n\nLatest version of:\n\n- [Poetry](https://python-poetry.org) (recommended) or [conda](https://docs.conda.io/en/latest/miniconda.html) package\n  manager\n- [git](https://git-scm.com/downloads) version control system\n\n### Clone the repository\n\n```shell\ngit clone https://github.com/dineshpinto/qudi-hira-analysis.git\n```\n\n### Installing dependencies with Poetry\n\n```bash\npoetry install\n```\n\n#### Add Poetry environment to Jupyter kernel\n\n```bash\npoetry run python -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### OR installing dependencies with conda\n\n#### Creating the conda environment\n\n```shell\nconda env create -f tools/conda-env-xx.yml\n```\n\nwhere `xx` is either `win10`, `osx-intel` or `osx-apple-silicon`.\n\n#### Activate conda environment\n\n```shell\nconda activate qudi-hira-analysis\n```\n\n#### Add conda environment to Jupyter kernel\n\n```shell\npython -m ipykernel install --user --name=qudi-hira-analysis\n```\n\n### Start the analysis\n\n#### If installed with Poetry\n\n```shell\npoetry run jupyter lab\n```\n\n#### OR with conda\n\n```shell\njupyter lab\n```\n\nDon\'t forget to switch to the `qudi-hira-analysis` kernel in JupyterLab.\n\n## Makefile\n\nThe Makefile located in `notebooks/` is configured to generate a variety of outputs:\n\n+ `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)\n+ `make html`: Converts all notebooks to HTML\n+ `make py`  : Converts all notebooks to Python (can be useful for VCS)\n+ `make all` : Sequentially runs all the notebooks in folder\n\nTo use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then\ninstall make with `choco install make`\n',
+    'author': 'dineshpinto',
+    'author_email': 'annual.fallout_0z@icloud.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'https://github.com/dineshpinto/qudi-hira-analysis',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'python_requires': '>=3.10,<4.0',
+}
 
-The high level interface is abstracted, and provides a set of functions to automate data import, handling and analysis.
-It is designed to be exposed through Jupyter Notebooks, although the abstract interface allows it to be integrated into
-larger, more general frameworks as well (with only some pain). Using the toolkit itself should only require a
-beginner-level understanding of Python.
-
-It also aims to improve transparency and reproducibility in experimental data analysis. In an ideal scenario,
-two lines of code are sufficient to recreate all output data.
-
-Python offers some very handy features like dataclasses, which are heavily used by this toolkit. Dataclasses offer a
-full OOP (object-oriented programming) experience while analyzing complex data sets. They provide a solid and
-transparent structure to the data to
-reduce errors arising from data fragmentation. This generally comes at a large performance cost, but this is (largely)
-sidestepped by lazy loading data and storing metadata instead wherever possible.
-
-## Installation
-
-```bash
-pip install qudi-hira-analysis
-```
-
-## Citation
-
-If you are publishing scientific results, you can cite this work as:  https://doi.org/10.5281/zenodo.7604670
-
-## Examples
-
-First set up the `DataHandler` object (henceforth referred to as `dh`) with the correct paths to the data and figure
-folders.
-
-Everything revolves around the `dh` object. It is the main interface to the toolkit and is initialized with the
-following required arguments:
-
-- `data_folder` is the main folder where all the data is stored, it can be the direct path to the data, or composed of
-  several sub-folders, each containing the data for a specific measurement
-- `figure_folder` is the folder where the output figures will be saved
-
-Optional arguments:
-
-- `measurement_folder` is the specific sub-folder in `data_folder` where the data for a specific measurement is stored
-
-```python
-from pathlib import Path
-import matplotlib.pyplot as plt
-import seaborn as sns
-
-from qudi_hira_analysis import DataHandler
-
-dh = DataHandler(
-    data_folder=Path("C:\\", "Data"),
-    figure_folder=Path("C:\\", "QudiHiraAnalysis"),
-    measurement_folder=Path("20230101_NV1")
-)
-```
-
-To load a specific set of measurements from the data folder, use the `dh.load_measurements()` method, which takes the
-following required arguments:
-
-- `measurement_str` is the string that is used to identify the measurement. It is used to filter the data files in the
-  `data_folder` and `measurement_folder` (if specified)
-
-Optional arguments:
-
-- `qudi` is a boolean. If `True`, the data is assumed to be in the format used by Qudi (default: True)
-- `pulsed` is a boolean. If `True`, the data is assumed to be in the format used by Qudi for pulsed measurements (
-  default: False)
-- `extension` is the extension of the data files (default: ".dat")
-
-The `load_measurements` function returns a dictionary containing the measurement data filtered by `measurement_str`.
-
-- The dictionary keys are measurement timestamps in "(year)(month)(day)-(hour)(minute)-(second)" format.
-
-- The dictionary values are `MeasurementDataclass` objects whose schema is shown
-  visually [here](#measurement-dataclass-schema).
-
-### Example 0: NV-PL measurements
-
-```python
-pixel_scanner_measurements = dh.load_measurements(measurement_str="PixelScanner")
-
-fwd, bwd = pixel_scanner_measurements["20230101-0420-00"].data
-
-# If size is known, it can be specified here
-fwd.size["real"] = {"x": 1e-6, "y": 1e-6, "unit": "m"}
-
-fig, ax = plt.subplots()
-
-# Perform (optional) image corrections
-fwd.filter_gaussian(sigma=0.5)
-
-# Add scale bar, color bar and plot the data
-img = fwd.show(cmap="inferno", ax=ax)
-fwd.add_scale(length=1e-6, ax=ax, height=1)
-cbar = fig.colorbar(img)
-cbar.set_label("NV-PL (kcps)")
-
-# Save the figure to the figure folder specified earlier
-dh.save_figures(filepath="nv_pl_scan", fig=fig, only_jpg=True)
-```
-
-### Example 1: Nanonis AFM measurements
-
-```python
-afm_measurements = dh.load_measurements(measurement_str="Scan", extension=".sxm")
-
-afm = afm_measurements["20230101-0420-00"].data
-
-# Print the channels available in the data
-afm.list_channels()
-topo = afm.get_channel("Z")
-
-fig, ax = plt.subplots()
-
-# Perform (optional) image corrections
-topo.correct_lines()
-topo.correct_plane()
-topo.filter_lowpass(fft_radius=20)
-topo.zero_min()
-
-# Add scale bar, color bar and plot the data
-img = topo.show(cmap="inferno", ax=ax)
-topo.add_scale(length=1e-6, ax=ax, height=1, fontsize=10)
-cbar = fig.colorbar(img)
-cbar.set_label("Height (nm)")
-
-dh.save_figures(filepath="afm_topo", fig=fig, only_jpg=True)
-``` 
-
-### Example 2: Autocorrelation measurements (Antibunching fit)
-
-```python
-autocorrelation_measurements = dh.load_measurements(measurement_str="Autocorrelation")
-
-fig, ax = plt.subplots()
-
-for autocorrelation in autocorrelation_measurements.values():
-  autocorrelation.data["Time (ns)"] = autocorrelation.data["Time (ps)"] * 1e-3
-  # Plot the data
-  sns.lineplot(data=autocorrelation.data, x="Time (ns)", y="g2(t) norm", ax=ax)
-  # Fit the data using the antibunching function
-  fit_x, fit_y, result = dh.fit(x="Time (ns)", y="g2(t) norm", data=autocorrelation.data,
-                                fit_function=dh.fit_function.antibunching)
-  # Plot the fit
-  sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")
-
-# Save the figure to the figure folder specified earlier
-dh.save_figures(filepath="autocorrelation_variation", fig=fig)
-```
-
-### Example 3: ODMR measurements (double Lorentzian fit)
-
-```python
-odmr_measurements = dh.load_measurements(measurement_str="ODMR", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for odmr in odmr_measurements.values():
-    sns.scatterplot(data=odmr.data, x="Controlled variable(Hz)", y="Signal", ax=ax)
-    fit_x, fit_y, result = dh.fit(x="Controlled variable(Hz)", y="Signal", data=odmr.data,
-                                  fit_function=dh.fit_function.lorentziandouble)
-    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")
-
-dh.save_figures(filepath="odmr_variation", fig=fig)
-```
-
-### Example 4: Rabi measurements (sine exponential decay fit)
-
-```python
-rabi_measurements = dh.load_measurements(measurement_str="Rabi", pulsed=True)
-
-fig, ax = plt.subplots()
-
-for rabi in rabi_measurements.values():
-    sns.scatterplot(data=rabi.data, x="Controlled variable(s)", y="Signal", ax=ax)
-    fit_x, fit_y, result = dh.fit(x="Controlled variable(s)", y="Signal", data=rabi.data,
-                                  fit_function=dh.fit_function.sineexponentialdecay)
-    sns.lineplot(x=fit_x, y=fit_y, ax=ax, color="C1")
-
-dh.save_figures(filepath="rabi_variation", fig=fig)
-```
-
-### Example 5: Temperature data
-
-```python
-temperature_measurements = dh.load_measurements(measurement_str="Temperature")
-
-temperature = pd.concat([t.data for t in temperature_measurements.values()])
-
-fig, ax = plt.subplots()
-sns.lineplot(data=temperature, x="Time", y="Temperature", ax=ax)
-dh.save_figures(filepath="temperature_monitoring", fig=fig)
-```
-
-## Measurement Dataclass Schema
-
-```mermaid
-flowchart LR
-    subgraph Standard Data
-        MeasurementDataclass --o filepath1[filepath: Path];
-        MeasurementDataclass --o data1[data: DataFrame];
-        MeasurementDataclass --o params1[params: dict];
-        MeasurementDataclass --o timestamp1[timestamp: datetime.datetime];
-        MeasurementDataclass --o methods1[get_param_from_filename: Callable];
-        MeasurementDataclass --o methods2[set_datetime_index: Callable];
-    end
-    subgraph Pulsed Data
-        MeasurementDataclass -- pulsed --> PulsedMeasurementDataclass;
-        PulsedMeasurementDataclass -- measurement --> PulsedMeasurement;
-        PulsedMeasurement --o filepath2[filepath: Path];
-        PulsedMeasurement --o data2[data: DataFrame];
-        PulsedMeasurement --o params2[params: dict];
-        PulsedMeasurementDataclass -- laser_pulses --> LaserPulses;
-        LaserPulses --o filepath3[filepath: Path];
-        LaserPulses --o data3[data: DataFrame];
-        LaserPulses --o params3[params: dict];
-        PulsedMeasurementDataclass -- timetrace --> RawTimetrace;
-        RawTimetrace --o filepath4[filepath: Path];
-        RawTimetrace --o data4[data: DataFrame];
-        RawTimetrace --o params4[params: dict];
-    end
-```
-
-## Supports common fitting routines
-
-To get the full list of available fit routines, use the `dh.fit_function` attribute. The fit functions are:
-
-| Dimension | Fit                           |
-|-----------|-------------------------------|
-| 1d        | decayexponential              |
-|           | biexponential                 |
-|           | decayexponentialstretched     |
-|           | gaussian                      |
-|           | gaussiandouble                |
-|           | gaussianlinearoffset          |
-|           | hyperbolicsaturation          |
-|           | linear                        |
-|           | lorentzian                    |
-|           | lorentziandouble              |
-|           | lorentziantriple              |
-|           | sine                          |
-|           | sinedouble                    |
-|           | sinedoublewithexpdecay        |
-|           | sinedoublewithtwoexpdecay     |
-|           | sineexponentialdecay          |
-|           | sinestretchedexponentialdecay |
-|           | sinetriple                    |
-|           | sinetriplewithexpdecay        |
-|           | sinetriplewiththreeexpdecay   |
-| 2d        | twoDgaussian                  |
-
-## Inbuilt measurement tree visualizer
-
-```ipython
->>> dh.data_folder_tree()
-
-# Output
-├── 20211116_NetworkAnalysis_SampleIn_UpperPin.csv
-├── 20211116_NetworkAnalysis_SampleOut_UpperPin.csv
-├── 20211116_NetworkAnalysis_TipIn_LowerPin.csv
-├── 20211116_NetworkAnalysis_TipIn_UpperPin.csv
-├── 20211116_NetworkAnalysis_TipOut_LowerPin.csv
-├── 20211116_NetworkAnalysis_TipOut_UpperPin.csv
-├── ContactTestingMeasurementHead
-│   ├── C2_Reference.txt
-│   ├── C2_SampleLowerPin.txt
-│   ├── C2_SampleUpperPin.txt
-│   ├── C2_TipLowerPin.txt
-│   └── C2_TipUpperPin.txt
-├── Sample_MW_Pin_comparision.png
-├── Tip_MW_Pin_comparision.png
-└── Tip_Sample_MW_Pin_comparision.png
-```
-
-## Overall Schema
-
-```mermaid
-flowchart TD
-    IOHandler <-- Handle IO operations --> DataLoader;
-    DataLoader <-- Map IO callables --> DataHandler;
-    Qudi[Qudi FitLogic] --> AnalysisLogic;
-    AnalysisLogic -- Inject fit functions --> DataHandler;
-    DataHandler -- Fit data --> Plot;
-    DataHandler -- Structure data --> MeasurementDataclass;
-    MeasurementDataclass -- Plot data --> Plot[JupyterLab Notebook];
-    Plot -- Save plotted data --> DataHandler;
-    style MeasurementDataclass fill: #bbf, stroke: #f66, stroke-width: 2px, color: #fff, stroke-dasharray: 5 5
-```
-
-## License
-
-This license of this project is located in the top level folder under `LICENSE`. Some specific files contain their
-individual licenses in the file header docstring.
-
-## Build
-
-### Prerequisites
-
-Latest version of:
-
-- [Poetry](https://python-poetry.org) (recommended) or [conda](https://docs.conda.io/en/latest/miniconda.html) package
-  manager
-- [git](https://git-scm.com/downloads) version control system
-
-### Clone the repository
-
-```shell
-git clone https://github.com/dineshpinto/qudi-hira-analysis.git
-```
-
-### Installing dependencies with Poetry
-
-```bash
-poetry install
-```
-
-#### Add Poetry environment to Jupyter kernel
-
-```bash
-poetry run python -m ipykernel install --user --name=qudi-hira-analysis
-```
-
-### OR installing dependencies with conda
-
-#### Creating the conda environment
-
-```shell
-conda env create -f tools/conda-env-xx.yml
-```
-
-where `xx` is either `win10`, `osx-intel` or `osx-apple-silicon`.
-
-#### Activate conda environment
-
-```shell
-conda activate qudi-hira-analysis
-```
-
-#### Add conda environment to Jupyter kernel
-
-```shell
-python -m ipykernel install --user --name=qudi-hira-analysis
-```
-
-### Start the analysis
-
-#### If installed with Poetry
-
-```shell
-poetry run jupyter lab
-```
-
-#### OR with conda
-
-```shell
-jupyter lab
-```
-
-Don't forget to switch to the `qudi-hira-analysis` kernel in JupyterLab.
-
-## Makefile
-
-The Makefile located in `notebooks/` is configured to generate a variety of outputs:
-
-+ `make pdf` : Converts all notebooks to PDF (requires LaTeX backend)
-+ `make html`: Converts all notebooks to HTML
-+ `make py`  : Converts all notebooks to Python (can be useful for VCS)
-+ `make all` : Sequentially runs all the notebooks in folder
-
-To use the `make` command on Windows you can install [Chocolatey](https://chocolatey.org/install), then
-install make with `choco install make`
 
+setup(**setup_kwargs)
```

