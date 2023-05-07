# Comparing `tmp/onvif-zeep-async-3.0.0.tar.gz` & `tmp/onvif-zeep-async-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-3.0.0.tar", last modified: Sun May  7 01:05:28 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.0.1.tar", last modified: Sun May  7 01:21:57 2023, max compression
```

## Comparing `onvif-zeep-async-3.0.0.tar` & `onvif-zeep-async-3.0.1.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618925 onvif-zeep-async-3.0.0/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.0/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.0/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:05:28.618984 onvif-zeep-async-3.0.0/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.612363 onvif-zeep-async-3.0.0/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.613187 onvif-zeep-async-3.0.0/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    39635 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1882 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/onvif/util.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:05:09.000000 onvif-zeep-async-3.0.0/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.617982 onvif-zeep-async-3.0.0/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.0/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618724 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 01:05:28.619230 onvif-zeep-async-3.0.0/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618821 onvif-zeep-async-3.0.0/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.995086 onvif-zeep-async-3.0.1/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.1/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.1/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:21:57.995136 onvif-zeep-async-3.0.1/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.988413 onvif-zeep-async-3.0.1/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.989166 onvif-zeep-async-3.0.1/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    39420 2023-05-07 01:21:33.000000 onvif-zeep-async-3.0.1/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1882 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.1/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:21:38.000000 onvif-zeep-async-3.0.1/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994053 onvif-zeep-async-3.0.1/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.1/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994855 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:21:57.000000 onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 01:21:57.995361 onvif-zeep-async-3.0.1/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.1/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:21:57.994984 onvif-zeep-async-3.0.1/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.1/tests/test.py
```

### Comparing `onvif-zeep-async-3.0.0/.gitignore` & `onvif-zeep-async-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/.pre-commit-config.yaml` & `onvif-zeep-async-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/LICENSE` & `onvif-zeep-async-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/Makefile` & `onvif-zeep-async-3.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/PKG-INFO` & `onvif-zeep-async-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.0
+Version: 3.0.1
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.0/README.rst` & `onvif-zeep-async-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/examples/events.py` & `onvif-zeep-async-3.0.1/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/examples/rotate_image.py` & `onvif-zeep-async-3.0.1/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/examples/streaming.py` & `onvif-zeep-async-3.0.1/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/__init__.py` & `onvif-zeep-async-3.0.1/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/client.py` & `onvif-zeep-async-3.0.1/onvif/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -411,67 +411,56 @@
         self._cancel_subscription_renew: asyncio.TimerHandle | None = None
 
     @property
     def closed(self) -> bool:
         """Return True if the manager is closed."""
         return not self._subscription or self._subscription.transport.client.is_closed
 
-    @abstractmethod
-    async def _start(self) -> float:
-        """Setup the processor.
-
-        Returns the next renewal call at time.
-
-        """
-
-    async def _set_synchronization_point(self, service: ONVIFService) -> float:
-        """Set the synchronization point."""
-        try:
-            await service.SetSynchronizationPoint()
-        except (Fault, asyncio.TimeoutError, TransportError, TypeError):
-            logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
-
     async def start(self) -> None:
-        """Setup the notification processor."""
+        """Setup the manager."""
         renewal_call_at = await self._start()
         self._schedule_subscription_renew(renewal_call_at)
         return self._subscription
 
     def pause(self) -> None:
-        """Pause the notification processor."""
+        """Pause the manager."""
         self._cancel_renewals()
 
     def resume(self) -> None:
-        """Resume the notification processor."""
+        """Resume the manager."""
         self._schedule_subscription_renew(self._loop.time())
 
     async def stop(self) -> None:
-        """Stop the notification processor."""
+        """Stop the manager."""
         logger.debug("%s: Stop the notification manager", self._device.host)
         self._cancel_renewals()
         assert self._subscription, "Call start first"
         await self._subscription.Unsubscribe()
 
     async def shutdown(self) -> None:
-        """Shutdown the notification processor."""
+        """Shutdown the manager.
+
+        This method is irreversible.
+        """
         self._shutdown = True
         if self._restart_or_renew_task:
             self._restart_or_renew_task.cancel()
         logger.debug("%s: Shutdown the notification manager", self._device.host)
         await self.stop()
 
-    async def renew(self) -> float:
-        """Renew the notification subscription."""
-        device = self._device
-        logger.debug("%s: Renew the notification manager", device.host)
-        return self._calculate_next_renewal_call_at(
-            await self._subscription.Renew(
-                device.get_next_termination_time(self._interval)
-            )
-        )
+    @abstractmethod
+    async def _start(self) -> float:
+        """Setup the processor. Returns the next renewal call at time."""
+
+    async def _set_synchronization_point(self, service: ONVIFService) -> float:
+        """Set the synchronization point."""
+        try:
+            await service.SetSynchronizationPoint()
+        except (Fault, asyncio.TimeoutError, TransportError, TypeError):
+            logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
 
     def _cancel_renewals(self) -> None:
         """Cancel any pending renewals."""
         if self._cancel_subscription_renew:
             self._cancel_subscription_renew.cancel()
             self._cancel_subscription_renew = None
 
@@ -512,15 +501,21 @@
         """Restart the notify subscription assuming the camera rebooted."""
         self._cancel_renewals()
         return await self._start()
 
     @retry_connection_error()
     async def _call_subscription_renew(self) -> float:
         """Call notify subscription Renew."""
-        return await self.renew()
+        device = self._device
+        logger.debug("%s: Renew the notification manager", device.host)
+        return self._calculate_next_renewal_call_at(
+            await self._subscription.Renew(
+                device.get_next_termination_time(self._interval)
+            )
+        )
 
     async def _renew_subscription(self) -> float | None:
         """Renew notify subscription."""
         if self.closed or self._shutdown:
             return None
         try:
             return await self._call_subscription_renew()
@@ -529,17 +524,15 @@
             logger.debug(
                 "%s: Failed to renew notify subscription %s",
                 self._device.host,
                 stringify_onvif_error(err),
             )
         return None
 
-    async def _renew_or_restart_subscription(
-        self, now: dt.datetime | None = None
-    ) -> None:
+    async def _renew_or_restart_subscription(self) -> None:
         """Renew or start notify subscription."""
         if self._shutdown:
             return
         renewal_call_at = None
         try:
             renewal_call_at = (
                 await self._renew_subscription() or await self._restart_subscription()
```

### Comparing `onvif-zeep-async-3.0.0/onvif/definition.py` & `onvif-zeep-async-3.0.1/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/exceptions.py` & `onvif-zeep-async-3.0.1/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/util.py` & `onvif-zeep-async-3.0.1/onvif/util.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-3.0.1/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/addressing` & `onvif-zeep-async-3.0.1/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/envelope` & `onvif-zeep-async-3.0.1/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.0.1/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.0.1/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.0.1/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 3.0.0
+Version: 3.0.1
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
```

### Comparing `onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.0.1/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/pylintrc` & `onvif-zeep-async-3.0.1/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/setup.py` & `onvif-zeep-async-3.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-3.0.0/tests/test.py` & `onvif-zeep-async-3.0.1/tests/test.py`

 * *Files identical despite different names*

