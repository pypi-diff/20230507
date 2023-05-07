# Comparing `tmp/onvif-zeep-async-3.0.1.tar.gz` & `tmp/onvif-zeep-async-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.0.1.tar", last modified: Sun May  7 01:21:57 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.0.2.tar", last modified: Sun May  7 02:32:29 2023, max compression
```

## Comparing `onvif-zeep-async-3.0.1.tar` & `onvif-zeep-async-3.0.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.995086 onvif-zeep-async-3.0.1/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.1/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:21:57.995136 onvif-zeep-async-3.0.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.988413 onvif-zeep-async-3.0.1/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.989166 onvif-zeep-async-3.0.1/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    39420 2023-05-07 01:21:33.000000 onvif-zeep-async-3.0.1/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1882 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.1/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:21:38.000000 onvif-zeep-async-3.0.1/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994053 onvif-zeep-async-3.0.1/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.1/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994855 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 01:21:57.995361 onvif-zeep-async-3.0.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994984 onvif-zeep-async-3.0.1/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844544 onvif-zeep-async-3.0.2/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.2/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.2/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 02:32:29.844625 onvif-zeep-async-3.0.2/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.837935 onvif-zeep-async-3.0.2/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.838856 onvif-zeep-async-3.0.2/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    39421 2023-05-07 02:32:09.000000 onvif-zeep-async-3.0.2/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2453 2023-05-07 02:32:09.000000 onvif-zeep-async-3.0.2/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 02:32:13.000000 onvif-zeep-async-3.0.2/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.843569 onvif-zeep-async-3.0.2/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.2/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844306 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 02:32:29.844874 onvif-zeep-async-3.0.2/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.2/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844427 onvif-zeep-async-3.0.2/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/tests/test.py
```

### Comparing `onvif-zeep-async-3.0.1/.gitignore` & `onvif-zeep-async-3.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/.pre-commit-config.yaml` & `onvif-zeep-async-3.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/LICENSE` & `onvif-zeep-async-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/Makefile` & `onvif-zeep-async-3.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/PKG-INFO` & `onvif-zeep-async-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.1
+Version: 3.0.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.1/README.rst` & `onvif-zeep-async-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/examples/events.py` & `onvif-zeep-async-3.0.2/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/examples/rotate_image.py` & `onvif-zeep-async-3.0.2/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/examples/streaming.py` & `onvif-zeep-async-3.0.2/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/__init__.py` & `onvif-zeep-async-3.0.2/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/client.py` & `onvif-zeep-async-3.0.2/onvif/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from zeep.wsdl import Document
 from zeep.wsdl.bindings.soap import SoapOperation
 from zeep.wsse.username import UsernameToken
 
 from onvif.definition import SERVICES
 from onvif.exceptions import ONVIFAuthError, ONVIFError, ONVIFTimeoutError
 
-from .util import extract_subcodes_as_strings, is_auth_error, stringify_onvif_error
+from .util import normalize_url, stringify_onvif_error
 
 logger = logging.getLogger("onvif")
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
 _DEFAULT_SETTINGS = Settings()
 _DEFAULT_SETTINGS.strict = False
@@ -573,15 +573,15 @@
                 "InitialTerminationTime": time_str,
                 "ConsumerReference": {"Address": self._address},
             }
         )
         # pylint: disable=protected-access
         device.xaddrs[
             "http://www.onvif.org/ver10/events/wsdl/NotificationConsumer"
-        ] = result.SubscriptionReference.Address._value_1
+        ] = normalize_url(result.SubscriptionReference.Address._value_1)
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
@@ -653,15 +653,15 @@
                     self._interval
                 ),
             }
         )
         # pylint: disable=protected-access
         device.xaddrs[
             "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
-        ] = result.SubscriptionReference.Address._value_1
+        ] = normalize_url(result.SubscriptionReference.Address._value_1)
         # Create subscription manager
         self._subscription = await device.create_subscription_service(
             "PullPointSubscription"
         )
         # Create the service that will be used to pull messages from the device.
         self._service = await device.create_pullpoint_service()
         if device.has_broken_relative_time(
```

### Comparing `onvif-zeep-async-3.0.1/onvif/definition.py` & `onvif-zeep-async-3.0.2/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/exceptions.py` & `onvif-zeep-async-3.0.2/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-3.0.2/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/addressing` & `onvif-zeep-async-3.0.2/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/envelope` & `onvif-zeep-async-3.0.2/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.0.2/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.0.2/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.0.2/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.1
+Version: 3.0.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/pylintrc` & `onvif-zeep-async-3.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/setup.py` & `onvif-zeep-async-3.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.1/tests/test.py` & `onvif-zeep-async-3.0.2/tests/test.py`

 * *Files identical despite different names*

