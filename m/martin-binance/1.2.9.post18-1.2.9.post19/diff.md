# Comparing `tmp/martin-binance-1.2.9.post18.tar.gz` & `tmp/martin-binance-1.2.9.post19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "martin-binance-1.2.9.post18.tar", last modified: Mon Nov 21 17:29:11 2022, max compression
+gzip compressed data, was "martin-binance-1.2.9.post19.tar", last modified: Mon Nov 21 18:44:42 2022, max compression
```

## Comparing `martin-binance-1.2.9.post18.tar` & `martin-binance-1.2.9.post19.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.2.9.post18/.deepsource.toml
--rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.2.9.post18/.dockerignore
--rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.2.9.post18/.github/FUNDING.yml
--rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post18/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post18/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post18/.gitignore
--rwxr-xr-x   0        0        0    11608 2022-11-21 17:25:24.032003 martin-binance-1.2.9.post18/CHANGELOG.md
--rw-r--r--   0        0        0      586 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post18/Dockerfile
--rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.2.9.post18/LICENSE
--rwxr-xr-x   0        0        0    33890 2022-11-21 17:25:24.032003 martin-binance-1.2.9.post18/README.md
--rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.2.9.post18/doc/Create_strategy.png
--rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.2.9.post18/doc/Model of logarithmic grid.ods
--rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.2.9.post18/doc/Modified martingale.svg
--rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post18/doc/graf1.png
--rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post18/doc/tlg_notify.png
--rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post18/doc/tmux.png
--rw-r--r--   0        0        0     1635 2022-11-21 17:25:24.032003 martin-binance-1.2.9.post18/martin_binance/__init__.py
--rw-r--r--   0        0        0     6303 2022-10-14 19:57:45.663897 martin-binance-1.2.9.post18/martin_binance/cli_10_AAABBB.py.template
--rw-r--r--   0        0        0     6303 2022-10-14 19:57:45.663897 martin-binance-1.2.9.post18/martin_binance/cli_7_BTCUSDT.py.template
--rw-r--r--   0        0        0     4764 2022-10-30 14:53:52.242160 martin-binance-1.2.9.post18/martin_binance/client.py
--rw-r--r--   0        0        0   169231 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post18/martin_binance/executor.py
--rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.2.9.post18/martin_binance/funds_rate.db.template
--rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.2.9.post18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
--rw-r--r--   0        0        0      376 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post18/martin_binance/margin/margin_req.txt
--rw-r--r--   0        0        0    61383 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post18/martin_binance/margin_wrapper.py
--rw-r--r--   0        0        0     1609 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post18/martin_binance/ms_cfg.toml.template
--rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.2.9.post18/martin_binance/service/.tmux.conf
--rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post18/martin_binance/service/funds_export.service
--rwxr-xr-x   0        0        0    15769 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post18/martin_binance/service/funds_rate_exporter.py
--rwxr-xr-x   0        0        0    64172 2022-08-04 15:26:24.539746 martin-binance-1.2.9.post18/martin_binance/service/grafana.json
--rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post18/martin_binance/service/relaunch.py
--rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.2.9.post18/martin_binance/service/relaunch.service
--rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.2.9.post18/martin_binance/service/tmux.service
--rw-r--r--   0        0        0     1090 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post18/pyproject.toml
--rw-r--r--   0        0        0      243 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post18/requirements.txt
--rw-r--r--   0        0        0     2387 2022-06-16 20:37:14.841699 martin-binance-1.2.9.post18/uml/architecture.puml
--rw-r--r--   0        0        0    34919 1970-01-01 00:00:00.000000 martin-binance-1.2.9.post18/PKG-INFO
+-rw-r--r--   0        0        0      154 2022-06-16 20:42:55.292826 martin-binance-1.2.9.post19/.deepsource.toml
+-rw-r--r--   0        0        0       79 2022-09-29 14:39:58.264847 martin-binance-1.2.9.post19/.dockerignore
+-rw-r--r--   0        0        0       68 2022-06-16 20:42:55.292826 martin-binance-1.2.9.post19/.github/FUNDING.yml
+-rw-r--r--   0        0        0      665 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post19/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      604 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post19/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       45 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post19/.gitignore
+-rwxr-xr-x   0        0        0    11686 2022-11-21 18:43:05.756740 martin-binance-1.2.9.post19/CHANGELOG.md
+-rw-r--r--   0        0        0      586 2022-09-29 14:39:58.268851 martin-binance-1.2.9.post19/Dockerfile
+-rw-r--r--   0        0        0     1079 2022-06-16 20:37:23.392898 martin-binance-1.2.9.post19/LICENSE
+-rwxr-xr-x   0        0        0    33890 2022-11-21 17:25:24.032003 martin-binance-1.2.9.post19/README.md
+-rwxr-xr-x   0        0        0    89295 2021-12-09 10:16:46.764494 martin-binance-1.2.9.post19/doc/Create_strategy.png
+-rwxr-xr-x   0        0        0    26452 2021-12-09 10:16:46.764494 martin-binance-1.2.9.post19/doc/Model of logarithmic grid.ods
+-rw-r--r--   0        0        0  5309091 2021-12-09 10:16:46.820491 martin-binance-1.2.9.post19/doc/Modified martingale.svg
+-rwxr-xr-x   0        0        0    79517 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post19/doc/graf1.png
+-rwxr-xr-x   0        0        0    10318 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post19/doc/tlg_notify.png
+-rwxr-xr-x   0        0        0     9332 2021-12-09 10:16:46.824491 martin-binance-1.2.9.post19/doc/tmux.png
+-rw-r--r--   0        0        0     1635 2022-11-21 18:13:49.092191 martin-binance-1.2.9.post19/martin_binance/__init__.py
+-rw-r--r--   0        0        0     6303 2022-10-14 19:57:45.663897 martin-binance-1.2.9.post19/martin_binance/cli_10_AAABBB.py.template
+-rw-r--r--   0        0        0     6303 2022-10-14 19:57:45.663897 martin-binance-1.2.9.post19/martin_binance/cli_7_BTCUSDT.py.template
+-rw-r--r--   0        0        0     4764 2022-10-30 14:53:52.242160 martin-binance-1.2.9.post19/martin_binance/client.py
+-rw-r--r--   0        0        0   169231 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post19/martin_binance/executor.py
+-rw-r--r--   0        0        0   237568 2022-09-29 14:39:58.276860 martin-binance-1.2.9.post19/martin_binance/funds_rate.db.template
+-rwxr-xr-x   0        0        0   337272 2022-09-29 14:39:58.276860 martin-binance-1.2.9.post19/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so
+-rw-r--r--   0        0        0      376 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post19/martin_binance/margin/margin_req.txt
+-rw-r--r--   0        0        0    61383 2022-11-21 17:25:24.036047 martin-binance-1.2.9.post19/martin_binance/margin_wrapper.py
+-rw-r--r--   0        0        0     1609 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post19/martin_binance/ms_cfg.toml.template
+-rw-r--r--   0        0        0      485 2021-12-09 09:06:56.984779 martin-binance-1.2.9.post19/martin_binance/service/.tmux.conf
+-rwxr-xr-x   0        0        0      319 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post19/martin_binance/service/funds_export.service
+-rwxr-xr-x   0        0        0    15769 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post19/martin_binance/service/funds_rate_exporter.py
+-rwxr-xr-x   0        0        0    64172 2022-08-04 15:26:24.539746 martin-binance-1.2.9.post19/martin_binance/service/grafana.json
+-rwxr-xr-x   0        0        0     1276 2022-09-29 14:39:58.280864 martin-binance-1.2.9.post19/martin_binance/service/relaunch.py
+-rwxr-xr-x   0        0        0      271 2022-09-29 14:39:58.284868 martin-binance-1.2.9.post19/martin_binance/service/relaunch.service
+-rwxr-xr-x   0        0        0      372 2021-12-09 09:06:56.984779 martin-binance-1.2.9.post19/martin_binance/service/tmux.service
+-rw-r--r--   0        0        0     1092 2022-11-21 18:13:49.084258 martin-binance-1.2.9.post19/pyproject.toml
+-rw-r--r--   0        0        0      245 2022-11-21 18:13:49.076326 martin-binance-1.2.9.post19/requirements.txt
+-rw-r--r--   0        0        0     2387 2022-06-16 20:37:14.841699 martin-binance-1.2.9.post19/uml/architecture.puml
+-rw-r--r--   0        0        0    34921 1970-01-01 00:00:00.000000 martin-binance-1.2.9.post19/PKG-INFO
```

### Comparing `martin-binance-1.2.9.post18/.github/ISSUE_TEMPLATE/bug_report.md` & `martin-binance-1.2.9.post19/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/.github/ISSUE_TEMPLATE/feature_request.md` & `martin-binance-1.2.9.post19/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/CHANGELOG.md` & `martin-binance-1.2.9.post19/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 ## v1.2.9-18 2022-11-21
+### Update
+* Dependency to exchanges-wrapper 1.2.7-1
+
+## v1.2.9-18 2022-11-21
 ### Fixed
 * #36
 * #37
 
 ## v1.2.9-14 2022-11-11
 ### Fixed
 * After restart from saved state incorrect value for first_run may cause incorrect data to be saved
```

### Comparing `martin-binance-1.2.9.post18/Dockerfile` & `martin-binance-1.2.9.post19/Dockerfile`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/LICENSE` & `martin-binance-1.2.9.post19/LICENSE`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/README.md` & `martin-binance-1.2.9.post19/README.md`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/Create_strategy.png` & `martin-binance-1.2.9.post19/doc/Create_strategy.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/Model of logarithmic grid.ods` & `martin-binance-1.2.9.post19/doc/Model of logarithmic grid.ods`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/Modified martingale.svg` & `martin-binance-1.2.9.post19/doc/Modified martingale.svg`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/graf1.png` & `martin-binance-1.2.9.post19/doc/graf1.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/tlg_notify.png` & `martin-binance-1.2.9.post19/doc/tlg_notify.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/doc/tmux.png` & `martin-binance-1.2.9.post19/doc/tmux.png`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/__init__.py` & `martin-binance-1.2.9.post19/martin_binance/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Free trading system for Binance SPOT API
 """
 __author__ = "Jerry Fedorenko"
 __copyright__ = "Copyright © 2021 Jerry Fedorenko aka VM"
 __license__ = "MIT"
-__version__ = "1.2.9-18"
+__version__ = "1.2.9-19"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 
 from pathlib import Path
 import shutil
 #
 import platform
```

### Comparing `martin-binance-1.2.9.post18/martin_binance/cli_10_AAABBB.py.template` & `martin-binance-1.2.9.post19/martin_binance/cli_10_AAABBB.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/cli_7_BTCUSDT.py.template` & `martin-binance-1.2.9.post19/martin_binance/cli_7_BTCUSDT.py.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/client.py` & `martin-binance-1.2.9.post19/martin_binance/client.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/executor.py` & `martin-binance-1.2.9.post19/martin_binance/executor.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/funds_rate.db.template` & `martin-binance-1.2.9.post19/martin_binance/funds_rate.db.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so` & `martin-binance-1.2.9.post19/martin_binance/margin/_sqlite3.cpython-37m-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/margin_wrapper.py` & `martin-binance-1.2.9.post19/martin_binance/margin_wrapper.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/ms_cfg.toml.template` & `martin-binance-1.2.9.post19/martin_binance/ms_cfg.toml.template`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/service/funds_rate_exporter.py` & `martin-binance-1.2.9.post19/martin_binance/service/funds_rate_exporter.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/service/grafana.json` & `martin-binance-1.2.9.post19/martin_binance/service/grafana.json`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/martin_binance/service/relaunch.py` & `martin-binance-1.2.9.post19/martin_binance/service/relaunch.py`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/pyproject.toml` & `martin-binance-1.2.9.post19/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "exchanges-wrapper==1.2.7",
+    "exchanges-wrapper==1.2.7-1",
     "margin-strategy-sdk==0.0.11",
     "aiohttp==3.8.1",
     "grpcio==1.48.1",
     "grpcio-tools==1.48.1",
     "jsonpickle==2.2.0",
     "psutil==5.9.1",
     "requests==2.28.1",
```

### Comparing `martin-binance-1.2.9.post18/uml/architecture.puml` & `martin-binance-1.2.9.post19/uml/architecture.puml`

 * *Files identical despite different names*

### Comparing `martin-binance-1.2.9.post18/PKG-INFO` & `martin-binance-1.2.9.post19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: martin-binance
-Version: 1.2.9.post18
+Version: 1.2.9.post19
 Summary: Free trading system for Binance SPOT API
 Author-email: Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: exchanges-wrapper==1.2.7
+Requires-Dist: exchanges-wrapper==1.2.7-1
 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.1
 Requires-Dist: grpcio==1.48.1
 Requires-Dist: grpcio-tools==1.48.1
 Requires-Dist: jsonpickle==2.2.0
 Requires-Dist: psutil==5.9.1
 Requires-Dist: requests==2.28.1
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: martin-binance Version: 1.2.9.post18 Summary: Free
+Metadata-Version: 2.1 Name: martin-binance Version: 1.2.9.post19 Summary: Free
 trading system for Binance SPOT API Author-email: Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: exchanges-wrapper==1.2.7 Requires-Dist: margin-strategy-sdk==0.0.11
+Dist: exchanges-wrapper==1.2.7-1 Requires-Dist: margin-strategy-sdk==0.0.11
 Requires-Dist: aiohttp==3.8.1 Requires-Dist: grpcio==1.48.1 Requires-Dist:
 grpcio-tools==1.48.1 Requires-Dist: jsonpickle==2.2.0 Requires-Dist:
 psutil==5.9.1 Requires-Dist: requests==2.28.1 Requires-Dist: simplejson==3.17.6
 Requires-Dist: toml==0.10.2 Requires-Dist: libtmux==0.14.0 Requires-Dist:
 colorama==0.4.5 Requires-Dist: prometheus-client==0.14.1 Project-URL: Source,
 https://github.com/DogsTailFarmer/martin-binance
        [https://github.com/DogsTailFarmer/martin-binance/raw/public/doc/
```

