# Comparing `tmp/circuitpython-bmp581-0.1.0.tar.gz` & `tmp/circuitpython-bmp581-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-bmp581-0.1.0.tar", last modified: Tue May  2 23:38:22 2023, max compression
+gzip compressed data, was "circuitpython-bmp581-0.1.1.tar", last modified: Sun May  7 18:29:21 2023, max compression
```

## Comparing `circuitpython-bmp581-0.1.0.tar` & `circuitpython-bmp581-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.657098 circuitpython-bmp581-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/bmp581.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-02 23:38:22.000000 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-02 23:38:22.000000 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 23:38:22.000000 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-02 23:38:22.000000 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 23:38:22.000000 circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/examples/bmp581_power_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/examples/bmp581_pressure_oversample_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/examples/bmp581_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/examples/bmp581_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-02 23:38:15.000000 circuitpython-bmp581-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-02 23:38:05.000000 circuitpython-bmp581-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 23:38:22.661098 circuitpython-bmp581-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.750778 circuitpython-bmp581-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3239 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/bmp581.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 18:29:21.000000 circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_output_data_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_power_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/examples/bmp581_temperature_oversample_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-07 18:29:14.000000 circuitpython-bmp581-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-07 18:29:06.000000 circuitpython-bmp581-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 18:29:21.754778 circuitpython-bmp581-0.1.1/setup.cfg
```

### Comparing `circuitpython-bmp581-0.1.0/.github/workflows/build.yml` & `circuitpython-bmp581-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/.github/workflows/release_gh.yml` & `circuitpython-bmp581-0.1.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/.gitignore` & `circuitpython-bmp581-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/.pre-commit-config.yaml` & `circuitpython-bmp581-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/.pylintrc` & `circuitpython-bmp581-0.1.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/LICENSE` & `circuitpython-bmp581-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/PKG-INFO` & `circuitpython-bmp581-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp581
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the Bosch BMP581 pressure sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP581
 Keywords: sensor,blinka,circuitpython,micropython,bmp581,pressure,temperature,bosch,sensor,BMP581
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bmp581-0.1.0/README.rst` & `circuitpython-bmp581-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/bmp581.py` & `circuitpython-bmp581-0.1.1/bmp581.py`

 * *Files 24% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from adafruit_register.i2c_bits import RWBits, ROBits
 
 try:
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_BMP581.git"
 
 _REG_WHOAMI = const(0x01)
 _OSR_CONF = const(0x36)
 _ODR_CONFIG = const(0x37)
 
 
@@ -45,14 +45,24 @@
 OSR4 = const(0x02)
 OSR8 = const(0x03)
 OSR16 = const(0x04)
 OSR32 = const(0x05)
 OSR64 = const(0x06)
 OSR128 = const(0x07)
 pressure_oversample_rate_values = (OSR1, OSR2, OSR4, OSR8, OSR16, OSR32, OSR64, OSR128)
+temperature_oversample_rate_values = (
+    OSR1,
+    OSR2,
+    OSR4,
+    OSR8,
+    OSR16,
+    OSR32,
+    OSR64,
+    OSR128,
+)
 
 
 class BMP581:
     """Driver for the BMP581 Sensor connected over I2C.
 
     :param ~busio.I2C i2c_bus: The I2C bus the BMP581 is connected to.
     :param int address: The I2C device address. Defaults to :const:`0x47`
@@ -83,15 +93,17 @@
         press = bmp.pressure
 
     """
 
     _device_id = ROUnaryStruct(_REG_WHOAMI, "B")
 
     _power_mode = RWBits(2, _ODR_CONFIG, 0)
+    _temperature_oversample_rate = RWBits(3, _OSR_CONF, 0)
     _pressure_oversample_rate = RWBits(3, _OSR_CONF, 3)
+    _output_data_rate = RWBits(5, _ODR_CONFIG, 2)
 
     _temperature = ROBits(24, 0x1D, 0, 3)
     _pressure = ROBits(24, 0x20, 0, 3)
 
     def __init__(self, i2c_bus: I2C, address: int = 0x47) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
 
@@ -171,14 +183,74 @@
     @pressure_oversample_rate.setter
     def pressure_oversample_rate(self, value: int) -> None:
         if value not in pressure_oversample_rate_values:
             raise ValueError("Value must be a valid pressure_oversample_rate setting")
         self._pressure_oversample_rate = value
 
     @property
+    def temperature_oversample_rate(self) -> str:
+        """
+        Sensor temperature_oversample_rate
+
+        +---------------------------+------------------+
+        | Mode                      | Value            |
+        +===========================+==================+
+        | :py:const:`bmp581.OSR1`   | :py:const:`0x00` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR2`   | :py:const:`0x01` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR4`   | :py:const:`0x02` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR8`   | :py:const:`0x03` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR16`  | :py:const:`0x04` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR32`  | :py:const:`0x05` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR64`  | :py:const:`0x06` |
+        +---------------------------+------------------+
+        | :py:const:`bmp581.OSR128` | :py:const:`0x07` |
+        +---------------------------+------------------+
+        """
+        values = (
+            "OSR1",
+            "OSR2",
+            "OSR4",
+            "OSR8",
+            "OSR16",
+            "OSR32",
+            "OSR64",
+            "OSR128",
+        )
+        return values[self._temperature_oversample_rate]
+
+    @temperature_oversample_rate.setter
+    def temperature_oversample_rate(self, value: int) -> None:
+        if value not in temperature_oversample_rate_values:
+            raise ValueError(
+                "Value must be a valid temperature_oversample_rate setting"
+            )
+        self._temperature_oversample_rate = value
+
+    @property
+    def output_data_rate(self) -> int:
+        """
+        Sensor output_data_rate. for a complete list of values please see the datasheet
+
+        """
+
+        return self._output_data_rate
+
+    @output_data_rate.setter
+    def output_data_rate(self, value: int) -> None:
+        if value not in range(0, 32, 1):
+            raise ValueError("Value must be a valid output_data_rate setting")
+        self._output_data_rate = value
+
+    @property
     def temperature(self) -> float:
         """
         The temperature sensor in C
         :return: Temperature
         """
         raw_temp = self._temperature
```

### Comparing `circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/PKG-INFO` & `circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-bmp581
-Version: 0.1.0
+Version: 0.1.1
 Summary: CircuitPython Driver for the Bosch BMP581 pressure sensor
 Author-email: "Jose D. Montoya" <jlib@mailmeto.mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_BMP581
 Keywords: sensor,blinka,circuitpython,micropython,bmp581,pressure,temperature,bosch,sensor,BMP581
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-bmp581-0.1.0/circuitpython_bmp581.egg-info/SOURCES.txt` & `circuitpython-bmp581-0.1.1/circuitpython_bmp581.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -23,11 +23,13 @@
 docs/requirements.txt
 docs/_static/Logo.png
 docs/_static/Logo.png.license
 docs/_static/extra_css.css
 docs/_static/extra_css.css.license
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
+examples/bmp581_output_data_rate.py
 examples/bmp581_power_mode.py
 examples/bmp581_pressure_oversample_rate.py
 examples/bmp581_simpletest.py
-examples/bmp581_temperature.py
+examples/bmp581_temperature.py
+examples/bmp581_temperature_oversample_rate.py
```

### Comparing `circuitpython-bmp581-0.1.0/docs/_static/Logo.png` & `circuitpython-bmp581-0.1.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/docs/_static/favicon.ico` & `circuitpython-bmp581-0.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/docs/conf.py` & `circuitpython-bmp581-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/docs/examples.rst` & `circuitpython-bmp581-0.1.1/docs/examples.rst`

 * *Files 20% similar despite different names*

```diff
@@ -29,7 +29,25 @@
 ----------------------------------
 
 Example showing the Power Mode setting
 
 .. literalinclude:: ../examples/bmp581_power_mode.py
     :caption: examples/bmp581_power_mode.py
     :linenos:
+
+Temperature oversample rate settings
+-------------------------------------
+
+Example showing the Temperature oversample rate setting
+
+.. literalinclude:: ../examples/bmp581_temperature_oversample_rate.py
+    :caption: examples/bmp581_temperature_oversample_rate.py
+    :linenos:
+
+Output data rate settings
+--------------------------
+
+Example showing the Output data rate setting
+
+.. literalinclude:: ../examples/bmp581_output_data_rate.py
+    :caption: examples/bmp581_output_data_rate.py
+    :linenos:
```

### Comparing `circuitpython-bmp581-0.1.0/examples/bmp581_power_mode.py` & `circuitpython-bmp581-0.1.1/examples/bmp581_power_mode.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/examples/bmp581_pressure_oversample_rate.py` & `circuitpython-bmp581-0.1.1/examples/bmp581_pressure_oversample_rate.py`

 * *Files identical despite different names*

### Comparing `circuitpython-bmp581-0.1.0/pyproject.toml` & `circuitpython-bmp581-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-bmp581"
 description = "CircuitPython Driver for the Bosch BMP581 pressure sensor"
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.rst"
 authors = [
     {name = "Jose D. Montoya", email = "jlib@mailmeto.mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_BMP581"}
 keywords = [
     "sensor",
```

