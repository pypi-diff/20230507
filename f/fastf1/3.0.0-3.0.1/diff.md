# Comparing `tmp/fastf1-3.0.0.tar.gz` & `tmp/fastf1-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastf1-3.0.0.tar", last modified: Tue May  2 20:43:31 2023, max compression
+gzip compressed data, was "fastf1-3.0.1.tar", last modified: Sun May  7 21:37:40 2023, max compression
```

## Comparing `fastf1-3.0.0.tar` & `fastf1-3.0.1.tar`

### file list

```diff
@@ -1,41 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-02 20:43:19.000000 fastf1-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-02 20:43:19.000000 fastf1-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-02 20:43:31.091595 fastf1-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-02 20:43:19.000000 fastf1-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/api.py
--rw-r--r--   0 runner    (1001) docker     (123)   132755 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/ergast/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/sphinx.py
--rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/ergast/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/livetiming/
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/livetiming/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/req.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1/signalr_aio/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/signalr_aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/signalr_aio/_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-02 20:43:19.000000 fastf1-3.0.0/fastf1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 20:43:31.091595 fastf1-3.0.0/fastf1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-02 20:43:31.000000 fastf1-3.0.0/fastf1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-02 20:43:30.000000 fastf1-3.0.0/fastf1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-02 20:43:19.000000 fastf1-3.0.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-02 20:43:31.091595 fastf1-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-02 20:43:19.000000 fastf1-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-07 21:37:25.000000 fastf1-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-07 21:37:25.000000 fastf1-3.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-07 21:37:40.955927 fastf1-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-07 21:37:25.000000 fastf1-3.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.951927 fastf1-3.0.1/fastf1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68847 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132755 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/ergast/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61147 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/sphinx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17410 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/ergast/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38668 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/livetiming/
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/livetiming/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5429 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15509 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24975 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/req.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/events/_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/hubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/hubs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/hubs/_hub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.955927 fastf1-3.0.1/fastf1/signalr_aio/transports/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_queue_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3588 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/signalr_aio/transports/_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-07 21:37:25.000000 fastf1-3.0.1/fastf1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 21:37:40.951927 fastf1-3.0.1/fastf1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 21:37:40.000000 fastf1-3.0.1/fastf1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-07 21:37:25.000000 fastf1-3.0.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-07 21:37:40.955927 fastf1-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-07 21:37:25.000000 fastf1-3.0.1/setup.py
```

### Comparing `fastf1-3.0.0/LICENSE` & `fastf1-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/README.rst` & `fastf1-3.0.1/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,96 +1,107 @@
-00000000: 3d3d 3d3d 3d3d 0a46 6173 7446 310a 3d3d  ======.FastF1.==
-00000010: 3d3d 3d3d 0a0a 4661 7374 4631 2069 7320  ====..FastF1 is 
-00000020: 6120 7079 7468 6f6e 2070 6163 6b61 6765  a python package
-00000030: 2066 6f72 2061 6363 6573 7369 6e67 2061   for accessing a
-00000040: 6e64 2061 6e61 6c79 7a69 6e67 2046 6f72  nd analyzing For
-00000050: 6d75 6c61 2031 2072 6573 756c 7473 2c0a  mula 1 results,.
-00000060: 7363 6865 6475 6c65 732c 2074 696d 696e  schedules, timin
-00000070: 6720 6461 7461 2061 6e64 2074 656c 656d  g data and telem
-00000080: 6574 7279 2e0a 0a2e 2e20 696d 6167 653a  etry..... image:
-00000090: 3a20 646f 6373 2f5f 7374 6174 6963 2f72  : docs/_static/r
-000000a0: 6561 646d 652e 706e 670a 2020 2020 3a74  eadme.png.    :t
-000000b0: 6172 6765 743a 2064 6f63 732f 5f73 7461  arget: docs/_sta
-000000c0: 7469 632f 7265 6164 6d65 2e70 6e67 0a0a  tic/readme.png..
-000000d0: 0a4d 6169 6e20 4665 6174 7572 6573 0a3d  .Main Features.=
-000000e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a 2d20  ============..- 
-000000f0: 4163 6365 7373 2074 6f20 4631 2074 696d  Access to F1 tim
-00000100: 696e 6720 6461 7461 2c20 7465 6c65 6d65  ing data, teleme
-00000110: 7472 792c 2073 6573 7369 6f6e 7320 7265  try, sessions re
-00000120: 7375 6c74 7320 616e 6420 6d6f 7265 0a2d  sults and more.-
-00000130: 2046 756c 6c20 7375 7070 6f72 7420 666f   Full support fo
-00000140: 7220 6045 7267 6173 7420 3c68 7474 703a  r `Ergast <http:
-00000150: 2f2f 6572 6761 7374 2e63 6f6d 2f6d 7264  //ergast.com/mrd
-00000160: 2f3e 605f 2074 6f20 6163 6365 7373 2063  />`_ to access c
-00000170: 7572 7265 6e74 2061 6e64 0a20 2068 6973  urrent and.  his
-00000180: 746f 7269 6361 6c20 4631 2064 6174 610a  torical F1 data.
-00000190: 2d20 416c 6c20 6461 7461 2069 7320 7072  - All data is pr
-000001a0: 6f76 6964 6564 2069 6e20 7468 6520 666f  ovided in the fo
-000001b0: 726d 206f 6620 6578 7465 6e64 6564 2050  rm of extended P
-000001c0: 616e 6461 7320 4461 7461 4672 616d 6573  andas DataFrames
-000001d0: 2074 6f20 6d61 6b65 0a20 2077 6f72 6b69   to make.  worki
-000001e0: 6e67 2077 6974 6820 7468 6520 6461 7461  ng with the data
-000001f0: 2065 6173 7920 7768 696c 6520 6861 7669   easy while havi
-00000200: 6e67 2070 6f77 6572 6675 6c20 746f 6f6c  ng powerful tool
-00000210: 7320 6176 6169 6c61 626c 650a 2d20 4164  s available.- Ad
-00000220: 6473 2063 7573 746f 6d20 6675 6e63 7469  ds custom functi
-00000230: 6f6e 7320 746f 2074 6865 2050 616e 6461  ons to the Panda
-00000240: 7320 6f62 6a65 6374 7320 7370 6563 6966  s objects specif
-00000250: 6963 616c 6c79 2074 6f20 6d61 6b65 2077  ically to make w
-00000260: 6f72 6b69 6e67 0a20 2077 6974 6820 4631  orking.  with F1
-00000270: 2064 6174 6120 7175 6963 6b20 616e 6420   data quick and 
-00000280: 7369 6d70 6c65 0a2d 2049 6e74 6567 7261  simple.- Integra
-00000290: 7469 6f6e 2077 6974 6820 4d61 7470 6c6f  tion with Matplo
-000002a0: 746c 6962 2074 6f20 6661 6369 6c69 7461  tlib to facilita
-000002b0: 7465 2064 6174 6120 7669 7375 616c 697a  te data visualiz
-000002c0: 6174 696f 6e0a 2d20 496d 706c 656d 656e  ation.- Implemen
-000002d0: 7473 2063 6163 6869 6e67 2066 6f72 2061  ts caching for a
-000002e0: 6c6c 2041 5049 2072 6571 7565 7374 7320  ll API requests 
-000002f0: 746f 2073 7065 6564 2075 7020 796f 7572  to speed up your
-00000300: 2073 6372 6970 7473 0a0a 0a49 6e73 7461   scripts...Insta
-00000310: 6c6c 6174 696f 6e0a 3d3d 3d3d 3d3d 3d3d  llation.========
-00000320: 3d3d 3d3d 0a0a 4974 2069 7320 7265 636f  ====..It is reco
-00000330: 6d6d 656e 6465 6420 746f 2069 6e73 7461  mmended to insta
-00000340: 6c6c 2046 6173 7446 3120 7573 696e 6720  ll FastF1 using 
-00000350: 6070 6970 603a 0a0a 2e2e 2063 6f64 652d  `pip`:.... code-
-00000360: 626c 6f63 6b3a 3a20 6261 7368 0a0a 2020  block:: bash..  
-00000370: 2070 6970 2069 6e73 7461 6c6c 2066 6173   pip install fas
-00000380: 7466 310a 0a4e 6f74 6520 7468 6174 2050  tf1..Note that P
-00000390: 7974 686f 6e20 332e 3820 6f72 2068 6967  ython 3.8 or hig
-000003a0: 6865 7220 6973 2072 6571 7569 7265 642e  her is required.
-000003b0: 0a0a 416c 7465 726e 6174 6976 656c 792c  ..Alternatively,
-000003c0: 2061 2077 6865 656c 206f 7220 6120 736f   a wheel or a so
-000003d0: 7572 6365 2064 6973 7472 6962 7574 696f  urce distributio
-000003e0: 6e20 6361 6e20 6265 2064 6f77 6e6c 6f61  n can be downloa
-000003f0: 6465 6420 6672 6f6d 2050 7970 692e 0a0a  ded from Pypi...
-00000400: 596f 7520 6361 6e20 616c 736f 2069 6e73  You can also ins
-00000410: 7461 6c6c 2075 7369 6e67 2060 636f 6e64  tall using `cond
-00000420: 6160 3a0a 0a2e 2e20 636f 6465 2d62 6c6f  a`:.... code-blo
-00000430: 636b 3a3a 2062 6173 680a 0a20 2063 6f6e  ck:: bash..  con
-00000440: 6461 2069 6e73 7461 6c6c 202d 6320 636f  da install -c co
-00000450: 6e64 612d 666f 7267 6520 6661 7374 6631  nda-forge fastf1
-00000460: 0a0a 0a44 6f63 756d 656e 7461 7469 6f6e  ...Documentation
-00000470: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0a0a  .=============..
-00000480: 5468 6520 6f66 6669 6369 616c 2064 6f63  The official doc
-00000490: 756d 656e 7461 7469 6f6e 2063 616e 2062  umentation can b
-000004a0: 6520 666f 756e 6420 6865 7265 3a0a 6068  e found here:.`h
-000004b0: 7474 7073 3a2f 2f74 6865 6f65 6872 6c79  ttps://theoehrly
-000004c0: 2e67 6974 6875 622e 696f 2f46 6173 742d  .github.io/Fast-
-000004d0: 4631 2f20 3c68 7474 7073 3a2f 2f74 6865  F1/ <https://the
-000004e0: 6f65 6872 6c79 2e67 6974 6875 622e 696f  oehrly.github.io
-000004f0: 2f46 6173 742d 4631 2f3e 605f 0a0a 0a4e  /Fast-F1/>`_...N
-00000500: 6f74 6963 650a 3d3d 3d3d 3d3d 0a0a 4661  otice.======..Fa
-00000510: 7374 4631 2061 6e64 2074 6869 7320 7765  stF1 and this we
-00000520: 6273 6974 6520 6172 6520 756e 6f66 6669  bsite are unoffi
-00000530: 6369 616c 2061 6e64 2061 7265 206e 6f74  cial and are not
-00000540: 2061 7373 6f63 6961 7465 6420 696e 2061   associated in a
-00000550: 6e79 2077 6179 2077 6974 680a 7468 6520  ny way with.the 
-00000560: 466f 726d 756c 6120 3120 636f 6d70 616e  Formula 1 compan
-00000570: 6965 732e 2046 312c 2046 4f52 4d55 4c41  ies. F1, FORMULA
-00000580: 204f 4e45 2c20 464f 524d 554c 4120 312c   ONE, FORMULA 1,
-00000590: 2046 4941 2046 4f52 4d55 4c41 204f 4e45   FIA FORMULA ONE
-000005a0: 2057 4f52 4c44 0a43 4841 4d50 494f 4e53   WORLD.CHAMPIONS
-000005b0: 4849 502c 2047 5241 4e44 2050 5249 5820  HIP, GRAND PRIX 
-000005c0: 616e 6420 7265 6c61 7465 6420 6d61 726b  and related mark
-000005d0: 7320 6172 6520 7472 6164 6520 6d61 726b  s are trade mark
-000005e0: 7320 6f66 2046 6f72 6d75 6c61 204f 6e65  s of Formula One
-000005f0: 0a4c 6963 656e 7369 6e67 2042 2e56 2e0a  .Licensing B.V..
+00000000: 2320 4661 7374 4631 0a0a 4661 7374 4631  # FastF1..FastF1
+00000010: 2069 7320 6120 7079 7468 6f6e 2070 6163   is a python pac
+00000020: 6b61 6765 2066 6f72 2061 6363 6573 7369  kage for accessi
+00000030: 6e67 2061 6e64 2061 6e61 6c79 7a69 6e67  ng and analyzing
+00000040: 2046 6f72 6d75 6c61 2031 2072 6573 756c   Formula 1 resul
+00000050: 7473 2c0a 7363 6865 6475 6c65 732c 2074  ts,.schedules, t
+00000060: 696d 696e 6720 6461 7461 2061 6e64 2074  iming data and t
+00000070: 656c 656d 6574 7279 2e0a 0a21 5b5d 2864  elemetry...![](d
+00000080: 6f63 732f 5f73 7461 7469 632f 7265 6164  ocs/_static/read
+00000090: 6d65 2e70 6e67 2022 6261 6e6e 6572 2229  me.png "banner")
+000000a0: 0a0a 0a23 2320 4d61 696e 2046 6561 7475  ...## Main Featu
+000000b0: 7265 730a 0a2d 2041 6363 6573 7320 746f  res..- Access to
+000000c0: 2046 3120 7469 6d69 6e67 2064 6174 612c   F1 timing data,
+000000d0: 2074 656c 656d 6574 7279 2c20 7365 7373   telemetry, sess
+000000e0: 696f 6e73 2072 6573 756c 7473 2061 6e64  ions results and
+000000f0: 206d 6f72 650a 2d20 4675 6c6c 2073 7570   more.- Full sup
+00000100: 706f 7274 2066 6f72 205b 4572 6761 7374  port for [Ergast
+00000110: 5d28 6874 7470 3a2f 2f65 7267 6173 742e  ](http://ergast.
+00000120: 636f 6d2f 6d72 642f 2920 746f 2061 6363  com/mrd/) to acc
+00000130: 6573 7320 6375 7272 656e 7420 616e 640a  ess current and.
+00000140: 2020 6869 7374 6f72 6963 616c 2046 3120    historical F1 
+00000150: 6461 7461 0a2d 2041 6c6c 2064 6174 6120  data.- All data 
+00000160: 6973 2070 726f 7669 6465 6420 696e 2074  is provided in t
+00000170: 6865 2066 6f72 6d20 6f66 2065 7874 656e  he form of exten
+00000180: 6465 6420 5061 6e64 6173 2044 6174 6146  ded Pandas DataF
+00000190: 7261 6d65 7320 746f 206d 616b 650a 2020  rames to make.  
+000001a0: 776f 726b 696e 6720 7769 7468 2074 6865  working with the
+000001b0: 2064 6174 6120 6561 7379 2077 6869 6c65   data easy while
+000001c0: 2068 6176 696e 6720 706f 7765 7266 756c   having powerful
+000001d0: 2074 6f6f 6c73 2061 7661 696c 6162 6c65   tools available
+000001e0: 0a2d 2041 6464 7320 6375 7374 6f6d 2066  .- Adds custom f
+000001f0: 756e 6374 696f 6e73 2074 6f20 7468 6520  unctions to the 
+00000200: 5061 6e64 6173 206f 626a 6563 7473 2073  Pandas objects s
+00000210: 7065 6369 6669 6361 6c6c 7920 746f 206d  pecifically to m
+00000220: 616b 6520 776f 726b 696e 670a 2020 7769  ake working.  wi
+00000230: 7468 2046 3120 6461 7461 2071 7569 636b  th F1 data quick
+00000240: 2061 6e64 2073 696d 706c 650a 2d20 496e   and simple.- In
+00000250: 7465 6772 6174 696f 6e20 7769 7468 204d  tegration with M
+00000260: 6174 706c 6f74 6c69 6220 746f 2066 6163  atplotlib to fac
+00000270: 696c 6974 6174 6520 6461 7461 2076 6973  ilitate data vis
+00000280: 7561 6c69 7a61 7469 6f6e 0a2d 2049 6d70  ualization.- Imp
+00000290: 6c65 6d65 6e74 7320 6361 6368 696e 6720  lements caching 
+000002a0: 666f 7220 616c 6c20 4150 4920 7265 7175  for all API requ
+000002b0: 6573 7473 2074 6f20 7370 6565 6420 7570  ests to speed up
+000002c0: 2079 6f75 7220 7363 7269 7074 730a 0a0a   your scripts...
+000002d0: 2323 2049 6e73 7461 6c6c 6174 696f 6e0a  ## Installation.
+000002e0: 0a49 7420 6973 2072 6563 6f6d 6d65 6e64  .It is recommend
+000002f0: 6564 2074 6f20 696e 7374 616c 6c20 4661  ed to install Fa
+00000300: 7374 4631 2075 7369 6e67 2060 7069 7060  stF1 using `pip`
+00000310: 3a0a 0a60 6060 636f 6d6d 616e 646c 696e  :..```commandlin
+00000320: 650a 7069 7020 696e 7374 616c 6c20 6661  e.pip install fa
+00000330: 7374 6631 0a60 6060 0a0a 4e6f 7465 2074  stf1.```..Note t
+00000340: 6861 7420 5079 7468 6f6e 2033 2e38 206f  hat Python 3.8 o
+00000350: 7220 6869 6768 6572 2069 7320 7265 7175  r higher is requ
+00000360: 6972 6564 2e0a 0a41 6c74 6572 6e61 7469  ired...Alternati
+00000370: 7665 6c79 2c20 6120 7768 6565 6c20 6f72  vely, a wheel or
+00000380: 2061 2073 6f75 7263 6520 6469 7374 7269   a source distri
+00000390: 6275 7469 6f6e 2063 616e 2062 6520 646f  bution can be do
+000003a0: 776e 6c6f 6164 6564 2066 726f 6d20 5079  wnloaded from Py
+000003b0: 7069 2e0a 0a59 6f75 2063 616e 2061 6c73  pi...You can als
+000003c0: 6f20 696e 7374 616c 6c20 7573 696e 6720  o install using 
+000003d0: 6063 6f6e 6461 603a 0a0a 6060 6063 6f6d  `conda`:..```com
+000003e0: 6d61 6e64 6c69 6e65 0a63 6f6e 6461 2069  mandline.conda i
+000003f0: 6e73 7461 6c6c 202d 6320 636f 6e64 612d  nstall -c conda-
+00000400: 666f 7267 6520 6661 7374 6631 0a60 6060  forge fastf1.```
+00000410: 0a0a 2323 2044 6f63 756d 656e 7461 7469  ..## Documentati
+00000420: 6f6e 0a0a 5468 6520 6f66 6669 6369 616c  on..The official
+00000430: 2064 6f63 756d 656e 7461 7469 6f6e 2063   documentation c
+00000440: 616e 2062 6520 666f 756e 6420 6865 7265  an be found here
+00000450: 3a0a 5b64 6f63 732e 6661 7374 6631 2e64  :.[docs.fastf1.d
+00000460: 6576 5d28 6874 7470 733a 2f2f 646f 6373  ev](https://docs
+00000470: 2e66 6173 7466 312e 6465 7629 0a0a 0a23  .fastf1.dev)...#
+00000480: 2320 5375 7070 6f72 7469 6e67 2074 6865  # Supporting the
+00000490: 2050 726f 6a65 6374 0a0a 4966 2079 6f75   Project..If you
+000004a0: 2077 616e 7420 746f 2073 7570 706f 7274   want to support
+000004b0: 2074 6865 2063 6f6e 7469 6e75 6f75 7320   the continuous 
+000004c0: 6465 7665 6c6f 706d 656e 7420 6f66 2046  development of F
+000004d0: 6173 7446 312c 2079 6f75 2063 616e 2062  astF1, you can b
+000004e0: 7579 206d 650a 6120 636f 6666 6565 2e0a  uy me.a coffee..
+000004f0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00000500: 2f2f 7777 772e 6275 796d 6561 636f 6666  //www.buymeacoff
+00000510: 6565 2e63 6f6d 2f66 6173 7466 3122 2074  ee.com/fastf1" t
+00000520: 6172 6765 743d 225f 626c 616e 6b22 3e3c  arget="_blank"><
+00000530: 696d 6720 7372 633d 2268 7474 7073 3a2f  img src="https:/
+00000540: 2f63 646e 2e62 7579 6d65 6163 6f66 6665  /cdn.buymeacoffe
+00000550: 652e 636f 6d2f 6275 7474 6f6e 732f 6465  e.com/buttons/de
+00000560: 6661 756c 742d 6f72 616e 6765 2e70 6e67  fault-orange.png
+00000570: 2220 616c 743d 2242 7579 204d 6520 4120  " alt="Buy Me A 
+00000580: 436f 6666 6565 2220 6865 6967 6874 3d22  Coffee" height="
+00000590: 3431 2220 7769 6474 683d 2231 3734 223e  41" width="174">
+000005a0: 3c2f 613e 0a0a 0a23 2320 4e6f 7469 6365  </a>...## Notice
+000005b0: 0a0a 4661 7374 4631 2061 6e64 2074 6869  ..FastF1 and thi
+000005c0: 7320 7765 6273 6974 6520 6172 6520 756e  s website are un
+000005d0: 6f66 6669 6369 616c 2061 6e64 2061 7265  official and are
+000005e0: 206e 6f74 2061 7373 6f63 6961 7465 6420   not associated 
+000005f0: 696e 2061 6e79 2077 6179 2077 6974 680a  in any way with.
+00000600: 7468 6520 466f 726d 756c 6120 3120 636f  the Formula 1 co
+00000610: 6d70 616e 6965 732e 2046 312c 2046 4f52  mpanies. F1, FOR
+00000620: 4d55 4c41 204f 4e45 2c20 464f 524d 554c  MULA ONE, FORMUL
+00000630: 4120 312c 2046 4941 2046 4f52 4d55 4c41  A 1, FIA FORMULA
+00000640: 204f 4e45 2057 4f52 4c44 0a43 4841 4d50   ONE WORLD.CHAMP
+00000650: 494f 4e53 4849 502c 2047 5241 4e44 2050  IONSHIP, GRAND P
+00000660: 5249 5820 616e 6420 7265 6c61 7465 6420  RIX and related 
+00000670: 6d61 726b 7320 6172 6520 7472 6164 6520  marks are trade 
+00000680: 6d61 726b 7320 6f66 2046 6f72 6d75 6c61  marks of Formula
+00000690: 204f 6e65 0a4c 6963 656e 7369 6e67 2042   One.Licensing B
+000006a0: 2e56 2e0a                                .V..
```

### Comparing `fastf1-3.0.0/fastf1/__init__.py` & `fastf1-3.0.1/fastf1/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/_api.py` & `fastf1-3.0.1/fastf1/_api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/api.py` & `fastf1-3.0.1/fastf1/api.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/core.py` & `fastf1-3.0.1/fastf1/core.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/ergast/interface.py` & `fastf1-3.0.1/fastf1/ergast/interface.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/ergast/legacy.py` & `fastf1-3.0.1/fastf1/ergast/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/ergast/sphinx.py` & `fastf1-3.0.1/fastf1/ergast/sphinx.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/ergast/structure.py` & `fastf1-3.0.1/fastf1/ergast/structure.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/events.py` & `fastf1-3.0.1/fastf1/events.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/legacy.py` & `fastf1-3.0.1/fastf1/legacy.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/livetiming/__init__.py` & `fastf1-3.0.1/fastf1/livetiming/__init__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/livetiming/__main__.py` & `fastf1-3.0.1/fastf1/livetiming/__main__.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/livetiming/client.py` & `fastf1-3.0.1/fastf1/livetiming/client.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/livetiming/data.py` & `fastf1-3.0.1/fastf1/livetiming/data.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/logger.py` & `fastf1-3.0.1/fastf1/logger.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/plotting.py` & `fastf1-3.0.1/fastf1/plotting.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/req.py` & `fastf1-3.0.1/fastf1/req.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/signalr_aio/_connection.py` & `fastf1-3.0.1/fastf1/signalr_aio/_connection.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/fastf1/utils.py` & `fastf1-3.0.1/fastf1/utils.py`

 * *Files identical despite different names*

### Comparing `fastf1-3.0.0/setup.cfg` & `fastf1-3.0.1/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 [options]
 zip_safe = False
 packages = 
 	fastf1
 	fastf1.ergast
 	fastf1.livetiming
 	fastf1.signalr_aio
+	fastf1.signalr_aio.events
+	fastf1.signalr_aio.hubs
+	fastf1.signalr_aio.transports
 python_requires = >= 3.8
 install_requires = 
 	requests-cache>=0.8.0
 	pandas>=1.2.4
 	numpy>=1.20.3
 	scipy>=1.6.3
 	thefuzz
```

