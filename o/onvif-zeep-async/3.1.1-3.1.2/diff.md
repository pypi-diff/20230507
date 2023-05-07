# Comparing `tmp/onvif-zeep-async-3.1.1.tar.gz` & `tmp/onvif-zeep-async-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.1.1.tar", last modified: Sun May  7 13:03:21 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.1.2.tar", last modified: Sun May  7 21:02:36 2023, max compression
```

## Comparing `onvif-zeep-async-3.1.1.tar` & `onvif-zeep-async-3.1.2.tar`

### file list

```diff
@@ -1,76 +1,77 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.871146 onvif-zeep-async-3.1.1/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.1/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.1/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 13:03:21.871226 onvif-zeep-async-3.1.1/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.862677 onvif-zeep-async-3.1.1/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.863886 onvif-zeep-async-3.1.1/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    23775 2023-05-07 13:02:47.000000 onvif-zeep-async-3.1.1/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/const.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)    12140 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/managers.py
--rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/settings.py
--rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/transport.py
--rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 13:02:52.000000 onvif-zeep-async-3.1.1/onvif/version.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.1/onvif/wrappers.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.870196 onvif-zeep-async-3.1.1/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.870930 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1519 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 13:03:21.000000 onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 13:03:21.871465 onvif-zeep-async-3.1.1/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.1.1/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 13:03:21.871024 onvif-zeep-async-3.1.1/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.1/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.078361 onvif-zeep-async-3.1.2/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.2/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.1.2/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 21:02:36.078411 onvif-zeep-async-3.1.2/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.067025 onvif-zeep-async-3.1.2/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.069189 onvif-zeep-async-3.1.2/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    23775 2023-05-07 13:02:47.000000 onvif-zeep-async-3.1.2/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      104 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.2/onvif/const.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    11738 2023-05-07 21:02:14.000000 onvif-zeep-async-3.1.2/onvif/managers.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      157 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.2/onvif/settings.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      563 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.2/onvif/transport.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     3613 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.2/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 21:02:20.000000 onvif-zeep-async-3.1.2/onvif/version.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     2331 2023-05-07 03:13:34.000000 onvif-zeep-async-3.1.2/onvif/wrappers.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.076806 onvif-zeep-async-3.1.2/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.077822 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 21:02:35.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1538 2023-05-07 21:02:36.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 21:02:35.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 21:02:35.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 21:02:35.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 21:02:35.000000 onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 21:02:36.078651 onvif-zeep-async-3.1.2/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.1.2/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 21:02:36.078050 onvif-zeep-async-3.1.2/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.1.2/tests/test.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      291 2023-05-07 02:28:47.000000 onvif-zeep-async-3.1.2/tests/test_util.py
```

### Comparing `onvif-zeep-async-3.1.1/.gitignore` & `onvif-zeep-async-3.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/.pre-commit-config.yaml` & `onvif-zeep-async-3.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/LICENSE` & `onvif-zeep-async-3.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/Makefile` & `onvif-zeep-async-3.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/PKG-INFO` & `onvif-zeep-async-3.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.1
+Version: 3.1.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.1/README.rst` & `onvif-zeep-async-3.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/examples/events.py` & `onvif-zeep-async-3.1.2/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/examples/rotate_image.py` & `onvif-zeep-async-3.1.2/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/examples/streaming.py` & `onvif-zeep-async-3.1.2/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/__init__.py` & `onvif-zeep-async-3.1.2/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/client.py` & `onvif-zeep-async-3.1.2/onvif/client.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/definition.py` & `onvif-zeep-async-3.1.2/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/exceptions.py` & `onvif-zeep-async-3.1.2/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/managers.py` & `onvif-zeep-async-3.1.2/onvif/managers.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,15 @@
         self._interval = interval
         self._subscription: ONVIFService | None = None
         self._restart_or_renew_task: asyncio.Task | None = None
         self._loop = asyncio.get_event_loop()
         self._shutdown = False
         self._subscription_lost_callback = subscription_lost_callback
         self._cancel_subscription_renew: asyncio.TimerHandle | None = None
+        self._service: ONVIFService | None = None
 
     @property
     def closed(self) -> bool:
         """Return True if the manager is closed."""
         return not self._subscription or self._subscription.transport.client.is_closed
 
     async def start(self) -> None:
@@ -90,18 +91,18 @@
         logger.debug("%s: Shutdown the notification manager", self._device.host)
         await self.stop()
 
     @abstractmethod
     async def _start(self) -> float:
         """Setup the processor. Returns the next renewal call at time."""
 
-    async def _set_synchronization_point(self, service: ONVIFService) -> float:
+    async def set_synchronization_point(self) -> float:
         """Set the synchronization point."""
         try:
-            await service.SetSynchronizationPoint()
+            await self._service.SetSynchronizationPoint()
         except (Fault, asyncio.TimeoutError, TransportError, TypeError):
             logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
 
     def _cancel_renewals(self) -> None:
         """Cancel any pending renewals."""
         if self._cancel_subscription_renew:
             self._cancel_subscription_renew.cancel()
@@ -225,20 +226,20 @@
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
-        service = await self._device.create_onvif_service(
+        self._service = await self._device.create_onvif_service(
             "pullpoint", port_type="NotificationConsumer"
         )
-        self._operation = service.document.bindings[service.binding_name].get(
-            "PullMessages"
-        )
+        self._operation = self._service.document.bindings[
+            self._service.binding_name
+        ].get("PullMessages")
         self._subscription = await device.create_subscription_service(
             "NotificationConsumer"
         )
         if device.has_broken_relative_time(
             self._interval,
             result.CurrentTime,
             result.TerminationTime,
@@ -246,15 +247,14 @@
             # If we determine the device has broken relative timestamps, we switch
             # to using absolute timestamps and renew the subscription.
             result = await self._subscription.Renew(
                 device.get_next_termination_time(self._interval)
             )
         renewal_call_at = self._calculate_next_renewal_call_at(result)
         logger.debug("%s: Start the notification manager", self._device.host)
-        await self._set_synchronization_point(service)
         return renewal_call_at
 
     def process(self, content: bytes) -> Any | None:
         """Process a notification message."""
         if not self._operation:
             logger.debug("%s: Notifications not setup", self._device.host)
             return
@@ -269,24 +269,14 @@
             return None
         return self._operation.process_reply(envelope)
 
 
 class PullPointManager(BaseManager):
     """Manager for PullPoint."""
 
-    def __init__(
-        self,
-        device: ONVIFCamera,
-        interval: dt.timedelta,
-        subscription_lost_callback: Callable[[], None],
-    ) -> None:
-        """Initialize the PullPoint processor."""
-        super().__init__(device, interval, subscription_lost_callback)
-        self._service: ONVIFService | None = None
-
     async def _start(self) -> float:
         """Start the PullPoint manager.
 
         Returns the next renewal call at time.
         """
         device = self._device
         logger.debug("%s: Setup the PullPoint manager", device.host)
@@ -314,13 +304,12 @@
             # If we determine the device has broken relative timestamps, we switch
             # to using absolute timestamps and renew the subscription.
             result = await self._subscription.Renew(
                 device.get_next_termination_time(self._interval)
             )
         renewal_call_at = self._calculate_next_renewal_call_at(result)
         logger.debug("%s: Start the notification manager", self._device.host)
-        await self._set_synchronization_point(self._service)
         return renewal_call_at
 
     def get_service(self) -> ONVIFService:
         """Return the pullpoint service."""
         return self._service
```

### Comparing `onvif-zeep-async-3.1.1/onvif/transport.py` & `onvif-zeep-async-3.1.2/onvif/transport.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/util.py` & `onvif-zeep-async-3.1.2/onvif/util.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wrappers.py` & `onvif-zeep-async-3.1.2/onvif/wrappers.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/addressing` & `onvif-zeep-async-3.1.2/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/envelope` & `onvif-zeep-async-3.1.2/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.1.2/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.1.2/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.1.2/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.1.1
+Version: 3.1.2
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.1.1/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.1.2/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -62,8 +62,9 @@
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

### Comparing `onvif-zeep-async-3.1.1/pylintrc` & `onvif-zeep-async-3.1.2/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/setup.py` & `onvif-zeep-async-3.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.1.1/tests/test.py` & `onvif-zeep-async-3.1.2/tests/test.py`

 * *Files identical despite different names*

