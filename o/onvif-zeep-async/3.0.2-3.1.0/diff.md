# Comparing `tmp/onvif-zeep-async-3.0.2.tar.gz` & `tmp/onvif-zeep-async-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.0.2.tar", last modified: Sun May  7 02:32:29 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.0.tar", last modified: Sun May  7 03:14:14 2023, max compression
```

## Comparing `onvif-zeep-async-3.0.2.tar` & `onvif-zeep-async-3.1.0.tar`

### file list

```diff
@@ -1,72 +1,77 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844544 onvif-zeep-async-3.0.2/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.2/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.2/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 02:32:29.844625 onvif-zeep-async-3.0.2/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.837935 onvif-zeep-async-3.0.2/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.838856 onvif-zeep-async-3.0.2/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    39421 2023-05-07 02:32:09.000000 onvif-zeep-async-3.0.2/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2453 2023-05-07 02:32:09.000000 onvif-zeep-async-3.0.2/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 02:32:13.000000 onvif-zeep-async-3.0.2/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.843569 onvif-zeep-async-3.0.2/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.2/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844306 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 02:32:29.000000 onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 02:32:29.844874 onvif-zeep-async-3.0.2/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.2/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 02:32:29.844427 onvif-zeep-async-3.0.2/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.2/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.586204 onvif-zeep-async-3.1.0/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.0/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 03:14:14.586255 onvif-zeep-async-3.1.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.579240 onvif-zeep-async-3.1.0/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.580553 onvif-zeep-async-3.1.0/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    23745 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    12140 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 03:13:47.000000 onvif-zeep-async-3.1.0/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.0/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.585116 onvif-zeep-async-3.1.0/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.585894 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1538 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 03:14:14.000000 onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 03:14:14.586484 onvif-zeep-async-3.1.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.1.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 03:14:14.586105 onvif-zeep-async-3.1.0/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.0/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.0/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.0.2/.gitignore` & `onvif-zeep-async-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/LICENSE` & `onvif-zeep-async-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/Makefile` & `onvif-zeep-async-3.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/PKG-INFO` & `onvif-zeep-async-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.2
+Version: 3.1.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.2/README.rst` & `onvif-zeep-async-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/examples/events.py` & `onvif-zeep-async-3.1.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/examples/rotate_image.py` & `onvif-zeep-async-3.1.0/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/examples/streaming.py` & `onvif-zeep-async-3.1.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/__init__.py` & `onvif-zeep-async-3.1.0/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/definition.py` & `onvif-zeep-async-3.1.0/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/exceptions.py` & `onvif-zeep-async-3.1.0/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.0/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.0/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.0/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.0/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.0/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.2
+Version: 3.1.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.2/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.0/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -12,19 +12,23 @@
 setup.cfg
 setup.py
 examples/events.py
 examples/rotate_image.py
 examples/streaming.py
 onvif/__init__.py
 onvif/client.py
+onvif/const.py
 onvif/definition.py
 onvif/exceptions.py
+onvif/managers.py
+onvif/settings.py
+onvif/transport.py
 onvif/util.py
 onvif/version.txt
-onvif/wsdl/.events.wsdl.swn
+onvif/wrappers.py
 onvif/wsdl/__init__.py
 onvif/wsdl/accesscontrol.wsdl
 onvif/wsdl/actionengine.wsdl
 onvif/wsdl/addressing
 onvif/wsdl/advancedsecurity.wsdl
 onvif/wsdl/analytics.wsdl
 onvif/wsdl/analyticsdevice.wsdl
@@ -58,8 +62,9 @@
 onvif_zeep_async.egg-info/PKG-INFO
 onvif_zeep_async.egg-info/SOURCES.txt
 onvif_zeep_async.egg-info/dependency_links.txt
 onvif_zeep_async.egg-info/entry_points.txt
 onvif_zeep_async.egg-info/not-zip-safe
 onvif_zeep_async.egg-info/requires.txt
 onvif_zeep_async.egg-info/top_level.txt
-tests/test.py
+tests/test.py
+tests/test_util.py
```

### Comparing `onvif-zeep-async-3.0.2/pylintrc` & `onvif-zeep-async-3.1.0/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/setup.py` & `onvif-zeep-async-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.2/tests/test.py` & `onvif-zeep-async-3.1.0/tests/test.py`

 * *Files identical despite different names*

