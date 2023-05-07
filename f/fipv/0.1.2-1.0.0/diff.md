# Comparing `tmp/fipv-0.1.2.tar.gz` & `tmp/fipv-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fipv-0.1.2.tar", last modified: Thu Oct  7 16:10:43 2021, max compression
+gzip compressed data, was "fipv-1.0.0.tar", last modified: Sun May  7 14:43:16 2023, max compression
```

## Comparing `fipv-0.1.2.tar` & `fipv-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 16:10:43.219663 fipv-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-10-07 16:10:39.000000 fipv-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       62 2021-10-07 16:10:39.000000 fipv-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-10-07 16:10:43.219663 fipv-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    10457 2021-10-07 16:10:39.000000 fipv-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-10-07 16:10:39.000000 fipv-0.1.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 16:10:43.215663 fipv-0.1.2/fipv/
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-10-07 16:10:39.000000 fipv-0.1.2/fipv/fipv.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 16:10:43.215663 fipv-0.1.2/fipv/fipv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11329 2021-10-07 16:10:43.000000 fipv-0.1.2/fipv/fipv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      332 2021-10-07 16:10:43.000000 fipv-0.1.2/fipv/fipv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-07 16:10:43.000000 fipv-0.1.2/fipv/fipv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-10-07 16:10:43.000000 fipv-0.1.2/fipv/fipv.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 16:10:43.219663 fipv-0.1.2/include/
--rw-r--r--   0 runner    (1001) docker     (121)     2317 2021-10-07 16:10:39.000000 fipv-0.1.2/include/split.h
--rw-r--r--   0 runner    (1001) docker     (121)      321 2021-10-07 16:10:39.000000 fipv-0.1.2/include/types.h
--rw-r--r--   0 runner    (1001) docker     (121)     2550 2021-10-07 16:10:39.000000 fipv-0.1.2/include/utils.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-07 16:10:43.219663 fipv-0.1.2/include/validators/
--rw-r--r--   0 runner    (1001) docker     (121)     1909 2021-10-07 16:10:39.000000 fipv-0.1.2/include/validators/ipv4.h
--rw-r--r--   0 runner    (1001) docker     (121)     2977 2021-10-07 16:10:39.000000 fipv-0.1.2/include/validators/ipv6.h
--rw-r--r--   0 runner    (1001) docker     (121)     1796 2021-10-07 16:10:39.000000 fipv-0.1.2/include/xalloc.h
--rw-r--r--   0 runner    (1001) docker     (121)      110 2021-10-07 16:10:39.000000 fipv-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      941 2021-10-07 16:10:43.219663 fipv-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      282 2021-10-07 16:10:39.000000 fipv-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:43:16.063375 fipv-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-07 14:43:14.000000 fipv-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-07 14:43:14.000000 fipv-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-07 14:43:16.063375 fipv-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-05-07 14:43:14.000000 fipv-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-07 14:43:14.000000 fipv-1.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:43:16.059375 fipv-1.0.0/fipv/
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-07 14:43:14.000000 fipv-1.0.0/fipv/fipv.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:43:16.063375 fipv-1.0.0/fipv/fipv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11619 2023-05-07 14:43:16.000000 fipv-1.0.0/fipv/fipv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-07 14:43:16.000000 fipv-1.0.0/fipv/fipv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 14:43:16.000000 fipv-1.0.0/fipv/fipv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-07 14:43:16.000000 fipv-1.0.0/fipv/fipv.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:43:16.063375 fipv-1.0.0/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-07 14:43:14.000000 fipv-1.0.0/include/split.h
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-07 14:43:14.000000 fipv-1.0.0/include/types.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-05-07 14:43:14.000000 fipv-1.0.0/include/utils.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 14:43:16.063375 fipv-1.0.0/include/validators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-07 14:43:14.000000 fipv-1.0.0/include/validators/ipv4.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-07 14:43:14.000000 fipv-1.0.0/include/validators/ipv6.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-07 14:43:14.000000 fipv-1.0.0/include/xalloc.h
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-07 14:43:14.000000 fipv-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-07 14:43:16.063375 fipv-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-07 14:43:14.000000 fipv-1.0.0/setup.py
```

### Comparing `fipv-0.1.2/LICENSE` & `fipv-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fipv-0.1.2/PKG-INFO` & `fipv-1.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 Metadata-Version: 2.1
 Name: fipv
-Version: 0.1.2
+Version: 1.0.0
 Summary: Fast IP validator for bulk IP data.
 Home-page: https://github.com/eredotpkfr/fipv
 Author: eredotpkfr
 Author-email: erdoganyoksul3@gmail.com
 License: MIT
+Project-URL: Documentation, https://www.erdoganyoksul.com/fipv/
 Project-URL: Bug Reports, https://github.com/eredotpkfr/fipv/issues
 Project-URL: Say Thanks (star the project), https://github.com/eredotpkfr/fipv
 Keywords: fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr
-Platform: UNKNOWN
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# fipv
 [![Test](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml/badge.svg)](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml)
 [![PyPI](https://img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/)
+[![Github Pages](https://img.shields.io/badge/github-pages-orange.svg)](https://www.erdoganyoksul.com/fipv/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fipv)
 [![License: MIT](https://img.shields.io/badge/license-MIT-informational.svg)](https://opensource.org/licenses/MIT)
 [![Stars](https://img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers)
 
-# fipv
 `fipv` (fast ip validator) is a python package build with `C` language. Simply it includes basic IP address validator functions as a `C` function, so works faster than others. Following `C` functions avaliable on this package:
 - ipv4
 - ipv4_cidr
 - ipv6
 - ipv6_cidr
 
-Can be used on bulk IP data. You can find detailed test benchmark at below.
+Can be used on bulk IP data. You can find detailed test benchmark at below. Also see [github pages](https://www.erdoganyoksul.com/fipv/) for full package reference and documentation.
 
 ## Installation
-`fipv` can be installed easly with `pip3`. It requires `Python 3.7+`
+`fipv` can be installed easily with `pip3`. It requires `Python 3.9+`
 ```sh
 $ pip3 install fipv
 ```
 ## Usage
 ```python
-#!/usr/bin/python3
-
 import fipv
 
 # Basic C validation functions
 print(
-    fipv.ipv4('127.0.0.1'),  # True
-    fipv.ipv4_cidr('127.0.0.1/44'),  # False
-    fipv.ipv6('::1'),  # True
-    fipv.ipv6_cidr('::1/129'),  # False
+    fipv.ipv4("127.0.0.1"),
+    fipv.ipv4_cidr("127.0.0.1/44"),
+    fipv.ipv6("::1"),
+    fipv.ipv6_cidr("::1/129"),
 )
+```
+```
+True False True False
+```
+<hr/>
+
+```python
+import fipv
 
 # Validate bulk IPv4 data
 ips = ['127.0.0.1'] * 1000000
 valids = [ip for ip in ips if fipv.ipv4(ip)]
-print(len(valids))  # 1000000
+print(len(valids))
+```
+```
+1000000
 ```
 
-## Test Benchmark
+## Test Benchmark (2021-10-07)
 In this test, it was tested validation speed and average RAM usage with different python validators and different data types. Finally results saved to below table.
 
 <b>Test Duration:</b> Used linux `time` command for determine execution time of script.<br/>
 <b>Avr. RAM Usage:</b> Used linux `ps` command every `0.1` second and calculated RAM average.
 
 :green_circle: Valid :red_circle: Invalid
 <table>
@@ -321,9 +331,7 @@
     </tr>
   </tbody>
 </table>
 
 ## Contact
 Blog - [erdoganyoksul.com](https://www.erdoganyoksul.com)<br/>
 Mail - erdoganyoksul3@gmail.com
-
-
```

#### html2text {}

```diff
@@ -1,40 +1,46 @@
-Metadata-Version: 2.1 Name: fipv Version: 0.1.2 Summary: Fast IP validator for
+Metadata-Version: 2.1 Name: fipv Version: 1.0.0 Summary: Fast IP validator for
 bulk IP data. Home-page: https://github.com/eredotpkfr/fipv Author: eredotpkfr
-Author-email: erdoganyoksul3@gmail.com License: MIT Project-URL: Bug Reports,
-https://github.com/eredotpkfr/fipv/issues Project-URL: Say Thanks (star the
-project), https://github.com/eredotpkfr/fipv Keywords:
-fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr Platform:
-UNKNOWN Classifier: Programming Language :: C Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/markdown License-File: LICENSE [![Test](https://github.com/
-eredotpkfr/fipv/actions/workflows/python-package-test.yml/badge.svg)](https://
-github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml) [![PyPI]
-(https://img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/fipv) [![License: MIT]
-(https://img.shields.io/badge/license-MIT-informational.svg)](https://
-opensource.org/licenses/MIT) [![Stars](https://img.shields.io/github/stars/
-eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers) #
-fipv `fipv` (fast ip validator) is a python package build with `C` language.
-Simply it includes basic IP address validator functions as a `C` function, so
-works faster than others. Following `C` functions avaliable on this package: -
-ipv4 - ipv4_cidr - ipv6 - ipv6_cidr Can be used on bulk IP data. You can find
-detailed test benchmark at below. ## Installation `fipv` can be installed easly
-with `pip3`. It requires `Python 3.7+` ```sh $ pip3 install fipv ``` ## Usage
-```python #!/usr/bin/python3 import fipv # Basic C validation functions print
-( fipv.ipv4('127.0.0.1'), # True fipv.ipv4_cidr('127.0.0.1/44'), # False
-fipv.ipv6('::1'), # True fipv.ipv6_cidr('::1/129'), # False ) # Validate bulk
-IPv4 data ips = ['127.0.0.1'] * 1000000 valids = [ip for ip in ips if fipv.ipv4
-(ip)] print(len(valids)) # 1000000 ``` ## Test Benchmark In this test, it was
-tested validation speed and average RAM usage with different python validators
-and different data types. Finally results saved to below table. Test Duration:
-Used linux `time` command for determine execution time of script.
+Author-email: erdoganyoksul3@gmail.com License: MIT Project-URL: Documentation,
+https://www.erdoganyoksul.com/fipv/ Project-URL: Bug Reports, https://
+github.com/eredotpkfr/fipv/issues Project-URL: Say Thanks (star the project),
+https://github.com/eredotpkfr/fipv Keywords:
+fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr Classifier:
+Programming Language :: C Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE # fipv [![Test](https://github.com/eredotpkfr/
+fipv/actions/workflows/python-package-test.yml/badge.svg)](https://github.com/
+eredotpkfr/fipv/actions/workflows/python-package-test.yml) [![PyPI](https://
+img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/) [![Github Pages]
+(https://img.shields.io/badge/github-pages-orange.svg)](https://
+www.erdoganyoksul.com/fipv/) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fipv) [![License: MIT](https://img.shields.io/badge/license-
+MIT-informational.svg)](https://opensource.org/licenses/MIT) [![Stars](https://
+img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/
+eredotpkfr/fipv/stargazers) `fipv` (fast ip validator) is a python package
+build with `C` language. Simply it includes basic IP address validator
+functions as a `C` function, so works faster than others. Following `C`
+functions avaliable on this package: - ipv4 - ipv4_cidr - ipv6 - ipv6_cidr Can
+be used on bulk IP data. You can find detailed test benchmark at below. Also
+see [github pages](https://www.erdoganyoksul.com/fipv/) for full package
+reference and documentation. ## Installation `fipv` can be installed easily
+with `pip3`. It requires `Python 3.9+` ```sh $ pip3 install fipv ``` ## Usage
+```python import fipv # Basic C validation functions print( fipv.ipv4
+("127.0.0.1"), fipv.ipv4_cidr("127.0.0.1/44"), fipv.ipv6("::1"), fipv.ipv6_cidr
+("::1/129"), ) ``` ``` True False True False ```
+===============================================================================
+```python import fipv # Validate bulk IPv4 data ips = ['127.0.0.1'] * 1000000
+valids = [ip for ip in ips if fipv.ipv4(ip)] print(len(valids)) ``` ``` 1000000
+``` ## Test Benchmark (2021-10-07) In this test, it was tested validation speed
+and average RAM usage with different python validators and different data
+types. Finally results saved to below table. Test Duration: Used linux `time`
+command for determine execution time of script.
 Avr. RAM Usage: Used linux `ps` command every `0.1` second and calculated RAM
 average. :green_circle: Valid :red_circle: Invalid
 Test ID   Test Data Count  Total Data Type   Project  Validation  Avr. RAM
                            Data                        Duration  Usage (MB)
               :       500K                 validators 0m12,975s       85M
     1   green_circle:        1M     IPv4
         :red_circle:  500K                 ipaddress   0m2,007s       80M
```

### Comparing `fipv-0.1.2/README.md` & `fipv-1.0.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,48 +1,58 @@
+# fipv
 [![Test](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml/badge.svg)](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml)
 [![PyPI](https://img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/)
+[![Github Pages](https://img.shields.io/badge/github-pages-orange.svg)](https://www.erdoganyoksul.com/fipv/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fipv)
 [![License: MIT](https://img.shields.io/badge/license-MIT-informational.svg)](https://opensource.org/licenses/MIT)
 [![Stars](https://img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers)
 
-# fipv
 `fipv` (fast ip validator) is a python package build with `C` language. Simply it includes basic IP address validator functions as a `C` function, so works faster than others. Following `C` functions avaliable on this package:
 - ipv4
 - ipv4_cidr
 - ipv6
 - ipv6_cidr
 
-Can be used on bulk IP data. You can find detailed test benchmark at below.
+Can be used on bulk IP data. You can find detailed test benchmark at below. Also see [github pages](https://www.erdoganyoksul.com/fipv/) for full package reference and documentation.
 
 ## Installation
-`fipv` can be installed easly with `pip3`. It requires `Python 3.7+`
+`fipv` can be installed easily with `pip3`. It requires `Python 3.9+`
 ```sh
 $ pip3 install fipv
 ```
 ## Usage
 ```python
-#!/usr/bin/python3
-
 import fipv
 
 # Basic C validation functions
 print(
-    fipv.ipv4('127.0.0.1'),  # True
-    fipv.ipv4_cidr('127.0.0.1/44'),  # False
-    fipv.ipv6('::1'),  # True
-    fipv.ipv6_cidr('::1/129'),  # False
+    fipv.ipv4("127.0.0.1"),
+    fipv.ipv4_cidr("127.0.0.1/44"),
+    fipv.ipv6("::1"),
+    fipv.ipv6_cidr("::1/129"),
 )
+```
+```
+True False True False
+```
+<hr/>
+
+```python
+import fipv
 
 # Validate bulk IPv4 data
 ips = ['127.0.0.1'] * 1000000
 valids = [ip for ip in ips if fipv.ipv4(ip)]
-print(len(valids))  # 1000000
+print(len(valids))
+```
+```
+1000000
 ```
 
-## Test Benchmark
+## Test Benchmark (2021-10-07)
 In this test, it was tested validation speed and average RAM usage with different python validators and different data types. Finally results saved to below table.
 
 <b>Test Duration:</b> Used linux `time` command for determine execution time of script.<br/>
 <b>Avr. RAM Usage:</b> Used linux `ps` command every `0.1` second and calculated RAM average.
 
 :green_circle: Valid :red_circle: Invalid
 <table>
```

#### html2text {}

```diff
@@ -1,29 +1,33 @@
-[![Test](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-
-test.yml/badge.svg)](https://github.com/eredotpkfr/fipv/actions/workflows/
-python-package-test.yml) [![PyPI](https://img.shields.io/pypi/v/fipv)](https://
-pypi.org/project/fipv/) ![PyPI - Python Version](https://img.shields.io/pypi/
-pyversions/fipv) [![License: MIT](https://img.shields.io/badge/license-MIT-
-informational.svg)](https://opensource.org/licenses/MIT) [![Stars](https://
-img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/
-eredotpkfr/fipv/stargazers) # fipv `fipv` (fast ip validator) is a python
-package build with `C` language. Simply it includes basic IP address validator
-functions as a `C` function, so works faster than others. Following `C`
-functions avaliable on this package: - ipv4 - ipv4_cidr - ipv6 - ipv6_cidr Can
-be used on bulk IP data. You can find detailed test benchmark at below. ##
-Installation `fipv` can be installed easly with `pip3`. It requires `Python
-3.7+` ```sh $ pip3 install fipv ``` ## Usage ```python #!/usr/bin/python3
-import fipv # Basic C validation functions print( fipv.ipv4('127.0.0.1'), #
-True fipv.ipv4_cidr('127.0.0.1/44'), # False fipv.ipv6('::1'), # True
-fipv.ipv6_cidr('::1/129'), # False ) # Validate bulk IPv4 data ips =
-['127.0.0.1'] * 1000000 valids = [ip for ip in ips if fipv.ipv4(ip)] print(len
-(valids)) # 1000000 ``` ## Test Benchmark In this test, it was tested
-validation speed and average RAM usage with different python validators and
-different data types. Finally results saved to below table. Test Duration: Used
-linux `time` command for determine execution time of script.
+# fipv [![Test](https://github.com/eredotpkfr/fipv/actions/workflows/python-
+package-test.yml/badge.svg)](https://github.com/eredotpkfr/fipv/actions/
+workflows/python-package-test.yml) [![PyPI](https://img.shields.io/pypi/v/
+fipv)](https://pypi.org/project/fipv/) [![Github Pages](https://img.shields.io/
+badge/github-pages-orange.svg)](https://www.erdoganyoksul.com/fipv/) ![PyPI -
+Python Version](https://img.shields.io/pypi/pyversions/fipv) [![License: MIT]
+(https://img.shields.io/badge/license-MIT-informational.svg)](https://
+opensource.org/licenses/MIT) [![Stars](https://img.shields.io/github/stars/
+eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers)
+`fipv` (fast ip validator) is a python package build with `C` language. Simply
+it includes basic IP address validator functions as a `C` function, so works
+faster than others. Following `C` functions avaliable on this package: - ipv4 -
+ipv4_cidr - ipv6 - ipv6_cidr Can be used on bulk IP data. You can find detailed
+test benchmark at below. Also see [github pages](https://www.erdoganyoksul.com/
+fipv/) for full package reference and documentation. ## Installation `fipv` can
+be installed easily with `pip3`. It requires `Python 3.9+` ```sh $ pip3 install
+fipv ``` ## Usage ```python import fipv # Basic C validation functions print
+( fipv.ipv4("127.0.0.1"), fipv.ipv4_cidr("127.0.0.1/44"), fipv.ipv6("::1"),
+fipv.ipv6_cidr("::1/129"), ) ``` ``` True False True False ```
+===============================================================================
+```python import fipv # Validate bulk IPv4 data ips = ['127.0.0.1'] * 1000000
+valids = [ip for ip in ips if fipv.ipv4(ip)] print(len(valids)) ``` ``` 1000000
+``` ## Test Benchmark (2021-10-07) In this test, it was tested validation speed
+and average RAM usage with different python validators and different data
+types. Finally results saved to below table. Test Duration: Used linux `time`
+command for determine execution time of script.
 Avr. RAM Usage: Used linux `ps` command every `0.1` second and calculated RAM
 average. :green_circle: Valid :red_circle: Invalid
 Test ID   Test Data Count  Total Data Type   Project  Validation  Avr. RAM
                            Data                        Duration  Usage (MB)
               :       500K                 validators 0m12,975s       85M
     1   green_circle:        1M     IPv4
         :red_circle:  500K                 ipaddress   0m2,007s       80M
```

### Comparing `fipv-0.1.2/fipv/fipv.c` & `fipv-1.0.0/fipv/fipv.c`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-/*
+/**
  * Author: eredotpkfr
  * Purpose: Implementing fast IP validators with C language.
  * Language:  C
  *
  * Main C API source file for fipv module.
  */
 
@@ -14,50 +14,98 @@
 
 static PyObject *ipv4(PyObject *self, PyObject *args);
 static PyObject *ipv4_cidr(PyObject *self, PyObject *args);
 static PyObject *ipv6(PyObject *self, PyObject *args);
 static PyObject *ipv6_cidr(PyObject *self, PyObject *args);
 PyMODINIT_FUNC PyInit_fipv(void);
 
+/**
+ * Module function for validating IPv4 values.
+ *
+ * Args:
+ *     self(PyObject *): the module itself
+ *     args(PyObject *): function arguments as a python object
+ *
+ * Returns:
+ *     Python boolean object, ``True`` if value is a valid IPv4
+ *         otherwise returns ``False``
+ *
+ */
 static PyObject *ipv4(PyObject *self, PyObject *args) {
   char *ipv4_addr;
 
   if (!PyArg_ParseTuple(args, "s", &ipv4_addr))
     return NULL;
 
   if (is_ipv4(ipv4_addr))
     Py_RETURN_TRUE;
 
   Py_RETURN_FALSE;
 }
 
+/**
+ * Module function for validating IPv4 CIDR values.
+ *
+ * Args:
+ *     self(PyObject *): the module itself
+ *     args(PyObject *): function arguments as a python object
+ *
+ * Returns:
+ *     Python boolean object, ``True`` if value is a valid IPv4 CIDR
+ *         otherwise returns ``False``
+ *
+ */
 static PyObject *ipv4_cidr(PyObject *self, PyObject *args) {
   char *ipv4_addr_cidr;
 
   if (!PyArg_ParseTuple(args, "s", &ipv4_addr_cidr))
     return NULL;
 
   if (is_ipv4_cidr(ipv4_addr_cidr))
     Py_RETURN_TRUE;
 
   Py_RETURN_FALSE;
 }
 
+/**
+ * Module function for validating IPv6 values.
+ *
+ * Args:
+ *     self(PyObject *): the module itself
+ *     args(PyObject *): function arguments as a python object
+ *
+ * Returns:
+ *     Python boolean object, ``True`` if value is a valid IPv6
+ *         otherwise returns ``False``
+ *
+ */
 static PyObject *ipv6(PyObject *self, PyObject *args) {
   char *ipv6_addr;
 
   if (!PyArg_ParseTuple(args, "s", &ipv6_addr))
     return NULL;
 
   if (is_ipv6(ipv6_addr))
     Py_RETURN_TRUE;
 
   Py_RETURN_FALSE;
 }
 
+/**
+ * Module function for validating IPv6 CIDR values.
+ *
+ * Args:
+ *     self(PyObject *): the module itself
+ *     args(PyObject *): function arguments as a python object
+ *
+ * Returns:
+ *     Python boolean object, ``True`` if value is a valid IPv6 CIDR
+ *         otherwise returns ``False``
+ *
+ */
 static PyObject *ipv6_cidr(PyObject *self, PyObject *args) {
   char *ipv6_addr_cidr;
 
   if (!PyArg_ParseTuple(args, "s", &ipv6_addr_cidr))
     return NULL;
 
   if (is_ipv6_cidr(ipv6_addr_cidr))
```

### Comparing `fipv-0.1.2/fipv/fipv.egg-info/PKG-INFO` & `fipv-1.0.0/fipv/fipv.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,71 +1,81 @@
 Metadata-Version: 2.1
 Name: fipv
-Version: 0.1.2
+Version: 1.0.0
 Summary: Fast IP validator for bulk IP data.
 Home-page: https://github.com/eredotpkfr/fipv
 Author: eredotpkfr
 Author-email: erdoganyoksul3@gmail.com
 License: MIT
+Project-URL: Documentation, https://www.erdoganyoksul.com/fipv/
 Project-URL: Bug Reports, https://github.com/eredotpkfr/fipv/issues
 Project-URL: Say Thanks (star the project), https://github.com/eredotpkfr/fipv
 Keywords: fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr
-Platform: UNKNOWN
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+# fipv
 [![Test](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml/badge.svg)](https://github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml)
 [![PyPI](https://img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/)
+[![Github Pages](https://img.shields.io/badge/github-pages-orange.svg)](https://www.erdoganyoksul.com/fipv/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/fipv)
 [![License: MIT](https://img.shields.io/badge/license-MIT-informational.svg)](https://opensource.org/licenses/MIT)
 [![Stars](https://img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers)
 
-# fipv
 `fipv` (fast ip validator) is a python package build with `C` language. Simply it includes basic IP address validator functions as a `C` function, so works faster than others. Following `C` functions avaliable on this package:
 - ipv4
 - ipv4_cidr
 - ipv6
 - ipv6_cidr
 
-Can be used on bulk IP data. You can find detailed test benchmark at below.
+Can be used on bulk IP data. You can find detailed test benchmark at below. Also see [github pages](https://www.erdoganyoksul.com/fipv/) for full package reference and documentation.
 
 ## Installation
-`fipv` can be installed easly with `pip3`. It requires `Python 3.7+`
+`fipv` can be installed easily with `pip3`. It requires `Python 3.9+`
 ```sh
 $ pip3 install fipv
 ```
 ## Usage
 ```python
-#!/usr/bin/python3
-
 import fipv
 
 # Basic C validation functions
 print(
-    fipv.ipv4('127.0.0.1'),  # True
-    fipv.ipv4_cidr('127.0.0.1/44'),  # False
-    fipv.ipv6('::1'),  # True
-    fipv.ipv6_cidr('::1/129'),  # False
+    fipv.ipv4("127.0.0.1"),
+    fipv.ipv4_cidr("127.0.0.1/44"),
+    fipv.ipv6("::1"),
+    fipv.ipv6_cidr("::1/129"),
 )
+```
+```
+True False True False
+```
+<hr/>
+
+```python
+import fipv
 
 # Validate bulk IPv4 data
 ips = ['127.0.0.1'] * 1000000
 valids = [ip for ip in ips if fipv.ipv4(ip)]
-print(len(valids))  # 1000000
+print(len(valids))
+```
+```
+1000000
 ```
 
-## Test Benchmark
+## Test Benchmark (2021-10-07)
 In this test, it was tested validation speed and average RAM usage with different python validators and different data types. Finally results saved to below table.
 
 <b>Test Duration:</b> Used linux `time` command for determine execution time of script.<br/>
 <b>Avr. RAM Usage:</b> Used linux `ps` command every `0.1` second and calculated RAM average.
 
 :green_circle: Valid :red_circle: Invalid
 <table>
@@ -321,9 +331,7 @@
     </tr>
   </tbody>
 </table>
 
 ## Contact
 Blog - [erdoganyoksul.com](https://www.erdoganyoksul.com)<br/>
 Mail - erdoganyoksul3@gmail.com
-
-
```

#### html2text {}

```diff
@@ -1,40 +1,46 @@
-Metadata-Version: 2.1 Name: fipv Version: 0.1.2 Summary: Fast IP validator for
+Metadata-Version: 2.1 Name: fipv Version: 1.0.0 Summary: Fast IP validator for
 bulk IP data. Home-page: https://github.com/eredotpkfr/fipv Author: eredotpkfr
-Author-email: erdoganyoksul3@gmail.com License: MIT Project-URL: Bug Reports,
-https://github.com/eredotpkfr/fipv/issues Project-URL: Say Thanks (star the
-project), https://github.com/eredotpkfr/fipv Keywords:
-fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr Platform:
-UNKNOWN Classifier: Programming Language :: C Classifier: Programming Language
-:: Python :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: License :: OSI Approved :: MIT License Classifier:
-Operating System :: OS Independent Requires-Python: >=3.7 Description-Content-
-Type: text/markdown License-File: LICENSE [![Test](https://github.com/
-eredotpkfr/fipv/actions/workflows/python-package-test.yml/badge.svg)](https://
-github.com/eredotpkfr/fipv/actions/workflows/python-package-test.yml) [![PyPI]
-(https://img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/) ![PyPI -
-Python Version](https://img.shields.io/pypi/pyversions/fipv) [![License: MIT]
-(https://img.shields.io/badge/license-MIT-informational.svg)](https://
-opensource.org/licenses/MIT) [![Stars](https://img.shields.io/github/stars/
-eredotpkfr/fipv?style=social)](https://github.com/eredotpkfr/fipv/stargazers) #
-fipv `fipv` (fast ip validator) is a python package build with `C` language.
-Simply it includes basic IP address validator functions as a `C` function, so
-works faster than others. Following `C` functions avaliable on this package: -
-ipv4 - ipv4_cidr - ipv6 - ipv6_cidr Can be used on bulk IP data. You can find
-detailed test benchmark at below. ## Installation `fipv` can be installed easly
-with `pip3`. It requires `Python 3.7+` ```sh $ pip3 install fipv ``` ## Usage
-```python #!/usr/bin/python3 import fipv # Basic C validation functions print
-( fipv.ipv4('127.0.0.1'), # True fipv.ipv4_cidr('127.0.0.1/44'), # False
-fipv.ipv6('::1'), # True fipv.ipv6_cidr('::1/129'), # False ) # Validate bulk
-IPv4 data ips = ['127.0.0.1'] * 1000000 valids = [ip for ip in ips if fipv.ipv4
-(ip)] print(len(valids)) # 1000000 ``` ## Test Benchmark In this test, it was
-tested validation speed and average RAM usage with different python validators
-and different data types. Finally results saved to below table. Test Duration:
-Used linux `time` command for determine execution time of script.
+Author-email: erdoganyoksul3@gmail.com License: MIT Project-URL: Documentation,
+https://www.erdoganyoksul.com/fipv/ Project-URL: Bug Reports, https://
+github.com/eredotpkfr/fipv/issues Project-URL: Say Thanks (star the project),
+https://github.com/eredotpkfr/fipv Keywords:
+fast,validation,validator,validate,ipv4,ipv6,ipv6_cidr,ipv4_cidr Classifier:
+Programming Language :: C Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Requires-Python: >=3.9 Description-Content-Type: text/
+markdown License-File: LICENSE # fipv [![Test](https://github.com/eredotpkfr/
+fipv/actions/workflows/python-package-test.yml/badge.svg)](https://github.com/
+eredotpkfr/fipv/actions/workflows/python-package-test.yml) [![PyPI](https://
+img.shields.io/pypi/v/fipv)](https://pypi.org/project/fipv/) [![Github Pages]
+(https://img.shields.io/badge/github-pages-orange.svg)](https://
+www.erdoganyoksul.com/fipv/) ![PyPI - Python Version](https://img.shields.io/
+pypi/pyversions/fipv) [![License: MIT](https://img.shields.io/badge/license-
+MIT-informational.svg)](https://opensource.org/licenses/MIT) [![Stars](https://
+img.shields.io/github/stars/eredotpkfr/fipv?style=social)](https://github.com/
+eredotpkfr/fipv/stargazers) `fipv` (fast ip validator) is a python package
+build with `C` language. Simply it includes basic IP address validator
+functions as a `C` function, so works faster than others. Following `C`
+functions avaliable on this package: - ipv4 - ipv4_cidr - ipv6 - ipv6_cidr Can
+be used on bulk IP data. You can find detailed test benchmark at below. Also
+see [github pages](https://www.erdoganyoksul.com/fipv/) for full package
+reference and documentation. ## Installation `fipv` can be installed easily
+with `pip3`. It requires `Python 3.9+` ```sh $ pip3 install fipv ``` ## Usage
+```python import fipv # Basic C validation functions print( fipv.ipv4
+("127.0.0.1"), fipv.ipv4_cidr("127.0.0.1/44"), fipv.ipv6("::1"), fipv.ipv6_cidr
+("::1/129"), ) ``` ``` True False True False ```
+===============================================================================
+```python import fipv # Validate bulk IPv4 data ips = ['127.0.0.1'] * 1000000
+valids = [ip for ip in ips if fipv.ipv4(ip)] print(len(valids)) ``` ``` 1000000
+``` ## Test Benchmark (2021-10-07) In this test, it was tested validation speed
+and average RAM usage with different python validators and different data
+types. Finally results saved to below table. Test Duration: Used linux `time`
+command for determine execution time of script.
 Avr. RAM Usage: Used linux `ps` command every `0.1` second and calculated RAM
 average. :green_circle: Valid :red_circle: Invalid
 Test ID   Test Data Count  Total Data Type   Project  Validation  Avr. RAM
                            Data                        Duration  Usage (MB)
               :       500K                 validators 0m12,975s       85M
     1   green_circle:        1M     IPv4
         :red_circle:  500K                 ipaddress   0m2,007s       80M
```

### Comparing `fipv-0.1.2/include/utils.h` & `fipv-1.0.0/include/utils.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,98 @@
-/*
- * Some helpful functions listed in this header file.
- *
- * Function: is_digit
- * ----------------------------
- * Checks if the given string is a digit.
- *
- * target_str: target string to be checked (char *)
- * returns: true if string is a digit otherwise false (bool)
- *
- * Function: is_xdigit
- * ----------------------------
- * Checks if the given string is a hexadecimal.
- *
- * target_str: target string to be checked (char *)
- * returns: true if string is a hexadecimal otherwise false (bool)
- *
- * Function: blanks
- * ----------------------------
- * Definition of "blank" is python empty string (''). If you split ".."
- * with "." in python, you get 3 empty string (['', '', ''])
- * simply blanks function counts these empty strings.
- *
- * target_str: target string (char *)
- * delimiter: delimiter character (char)
- * returns: returns count of empty strings (int)
- *
- * Function: startswith
- * ----------------------------
- * Returns true if the given string startswith given character
- *
- * target_str: target string (char *)
- * chr: comparing character (char)
- * returns: returns true if target_str startswith chr (bool)
- *
- * Function: endswith
- * ----------------------------
- * Returns true if the given string endswith given character
- *
- * target_str: target string (char *)
- * chr: comparing character (char)
- * returns: returns true if target_str endswith chr (bool)
- */
-
 #ifndef _UTILS_H_
 #define _UTILS_H_
 
 #include <ctype.h> /* for isdigit and isxdigit */
 
 bool is_digit(char *target_str);
 bool is_xdigit(char *target_str);
 bool startswith(char *target_str, char chr);
 bool endswith(char *target_str, char chr);
 int blanks(char *target_str, char delimiter);
 
+/**
+ * Returns ``true`` if the given string startswith given character.
+ *
+ * Args:
+ *     target_str(char *): target string
+ *     chr(char): comparing character
+ *
+ * Returns:
+ *     ``true`` if ``target_str`` startswith ``chr``
+ */
 bool startswith(char *target_str, char chr) {
   if (!target_str)
     return false;
 
   return target_str[0] == chr;
 }
 
+/**
+ * Returns ``true`` if the given string endswith given character.
+ *
+ * Args:
+ *     target_str(char *): target string
+ *     chr(char): comparing character
+ *
+ * Returns:
+ *     ``true`` if ``target_str`` endswith ``chr``
+ */
 bool endswith(char *target_str, char chr) {
   if (!target_str)
     return false;
 
   return target_str[strlen(target_str) - 1] == chr;
 }
 
+/**
+ * Checks if the given string is a digit.
+ *
+ * Args:
+ *     target_str(char *): target string to be checked
+ *
+ * Returns:
+ *     ``true`` if string is a digit otherwise ``false``
+ */
 bool is_digit(char *target_str) {
   for (size_t i = 0; i < strlen(target_str); i++) {
     if (!isdigit(target_str[i]))
       return false;
   }
   return true;
 }
 
+/**
+ * Checks if the given string is a hexadecimal.
+ *
+ * Args:
+ *     target_str(char *): target string to be checked
+ *
+ * Returns:
+ *     ``true`` if string is a hexadecimal otherwise ``false``
+ */
 bool is_xdigit(char *target_str) {
   for (size_t i = 0; i < strlen(target_str); i++) {
     if (!isxdigit(target_str[i]))
       return false;
   }
   return true;
 }
 
+/**
+ * Definition of `blank` is python empty string (``''``). If you split ``..``
+ *     with ``.`` in python, you get 3 empty string (``['', '', '']``)
+ *     simply blanks function counts these empty strings.
+ *
+ * Args:
+ *     target_str(char *): target string to count blanks
+ *     delimiter(char): delimiter character
+ *
+ * Returns:
+ *     count of empty strings
+ */
 int blanks(char *target_str, char delimiter) {
   int counter = 0;
 
   for (size_t i = 0; i < strlen(target_str); i++) {
     if (target_str[i] != delimiter)
       continue;
```

### Comparing `fipv-0.1.2/include/validators/ipv6.h` & `fipv-1.0.0/include/validators/ipv6.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-/*
- * IPv6 validator functions definition.
- *
- * Function: is_ipv6
- * ----------------------------
- * Returns true if given string is a IPv6 otherwise false.
- *
- * ipv6_addr: target string to be validated (char *)
- * returns: true if given address is a IPv6 address (bool)
- *
- * Function: is_ipv6_cidr
- * ----------------------------
- * Returns true if given string is a IPv6CIDR otherwise false.
- *
- * ipv6_addr_cidr: target string to be validated (char *)
- * returns: true if given address is a IPv6CIDR (bool)
- */
-
 #ifndef _IPV6_H_
 #define _IPV6_H_
 
 #define HEX_BASE 16
 #define IP_CIDR_DELIMITER "/"
 #define IPV4_DELIMITER "."
 #define IPV6_DELIMITER ":"
@@ -27,14 +9,23 @@
 
 #include "split.h"
 #include "utils.h"
 
 bool is_ipv6(char *ipv6_addr);
 bool is_ipv6_cidr(char *ipv6_addr_cidr);
 
+/**
+ * Returns ``true`` if given string is a IPv6 otherwise ``false``.
+ *
+ * Args:
+ *     ipv6_addr(char *): target string to be validated
+ *
+ * Returns:
+ *     ``true`` if given address is a IPv6 address
+ */
 bool is_ipv6(char *ipv6_addr) {
   struct split_t ipv6_groups;
   struct split_t ipv4_groups;
 
   char *ipv4_part;
   int blankctr, number;
   bool is_freed_ipv4;
@@ -100,14 +91,23 @@
 
   if (!is_freed_ipv4)
     free_split(&ipv4_groups);
 
   return free_split_r(&ipv6_groups, false);
 }
 
+/**
+ * Returns ``true`` if given string is a IPv6CIDR otherwise ``false``.
+ *
+ * Args:
+ *     ipv6_addr_cidr(char *): target string to be validated
+ *
+ * Returns:
+ *     ``true`` if given address is a IPv6CIDR
+ */
 bool is_ipv6_cidr(char *ipv6_addr_cidr) {
   struct split_t splitted = split(ipv6_addr_cidr, IP_CIDR_DELIMITER);
 
   if (splitted.length != 2)
     return free_split_r(&splitted, false);
 
   char *prefix = splitted.tokens[0];
```

### Comparing `fipv-0.1.2/include/xalloc.h` & `fipv-1.0.0/include/xalloc.h`

 * *Files 19% similar despite different names*

```diff
@@ -1,73 +1,76 @@
-/*
- * Header file for managing memory allocations
- * and allocation exceptions.
- *
- * Function: xmem_err
- * ----------------------------
- * Throw exception and exit program if p is NULL pointer.
- *
- * p: target pointer (void *)
- * returns: returns p if p is not NULL (void *)
- *
- * Function: xmalloc
- * ----------------------------
- * Allocate memory from heap and initialize with zero values.
- *
- * size: allocation byte size (size_t)
- * returns: returns head of allocated address (void *)
- *
- * Function: xrealloc
- * ----------------------------
- * Reallocate given pointer address.
- *
- * target: target pointer to be reallocated (void *)
- * new_size: new allocation size (size_t)
- * returns: returns head of reallocated address (void *)
- *
- * Function: xcalloc
- * ----------------------------
- * Allocate memory from heap with count and
- * automatic initialize with zero values.
- *
- * count: allocation count (size_t)
- * size: allocation size (size_t)
- * returns: returns head of allocated address (void *)
- */
-
 #ifndef _XALLOC_H_
 #define _XALLOC_H_
 
 // printed error message when allocation is failed.
 #define MEMORY_ERR "Out of memory!\n"
 
 #include <stdlib.h> /* for allocating operations */
 
 void *xmem_err(void *p);
 void *xmalloc(size_t size);
 void *xrealloc(void *target, size_t new_size);
 void *xcalloc(size_t count, size_t size);
 
+/**
+ * Throw exception and exit program if p is ``NULL`` pointer.
+ *
+ * Args:
+ *     p(void *): target pointer
+ *
+ * Returns:
+ *     ``p`` if ``p`` is not ``NULL``
+ */
 void *xmem_err(void *p) {
   if (!p) {
     fprintf(stderr, MEMORY_ERR);
     exit(EXIT_FAILURE); /* 1 */
   }
   return p;
 }
 
+/**
+ * Allocate memory from heap and initialize with zero values.
+ *
+ * Args:
+ *     size(size_t): allocation byte size
+ *
+ * Returns:
+ *     head of allocated address
+ */
 void *xmalloc(size_t size) {
   void *pointer = xmem_err(malloc(size));
   memset(pointer, 0, size); /* set zero values */
 
   return pointer;
 }
 
+/**
+ * Reallocate given pointer address.
+ *
+ * Args:
+ *     target(void *): target pointer to be reallocated
+ *     new_size(size_t): new allocation size
+ *
+ * Returns:
+ *     head of reallocated address
+ */
 void *xrealloc(void *target, size_t new_size) {
   return xmem_err(realloc(target, new_size));
 }
 
+/**
+ * Allocate memory from heap with count and
+ *     automatic initialize with zero values.
+ *
+ * Args:
+ *     count(size_t): allocation count
+ *     size(size_t): allocation size
+ *
+ * Returns:
+ *     head of allocated address
+ */
 void *xcalloc(size_t count, size_t size) {
   return xmem_err(calloc(count, size));
 }
 
 #endif
```

### Comparing `fipv-0.1.2/setup.cfg` & `fipv-1.0.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,28 @@
 author = eredotpkfr
 author_email = erdoganyoksul3@gmail.com
 description = Fast IP validator for bulk IP data.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/eredotpkfr/fipv
 project_urls = 
+	Documentation = https://www.erdoganyoksul.com/fipv/
 	Bug Reports = https://github.com/eredotpkfr/fipv/issues
 	Say Thanks (star the project) = https://github.com/eredotpkfr/fipv
 classifiers = 
 	Programming Language :: C
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.7
-	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.9
 packages = find:
 package_dir = 
 	= fipv
 
 [options.packages.find]
 where = fipv
```

