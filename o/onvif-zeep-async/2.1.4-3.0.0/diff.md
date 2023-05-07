# Comparing `tmp/onvif-zeep-async-2.1.4.tar.gz` & `tmp/onvif-zeep-async-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onvif-zeep-async-2.1.4.tar", last modified: Sat May  6 21:24:12 2023, max compression
+gzip compressed data, was "onvif-zeep-async-3.0.0.tar", last modified: Sun May  7 01:05:28 2023, max compression
```

## Comparing `onvif-zeep-async-2.1.4.tar` & `onvif-zeep-async-3.0.0.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893273 onvif-zeep-async-2.1.4/
--rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/.gitignore
--rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/.pre-commit-config.yaml
--rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.4/CHANGES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-2.1.4/LICENSE
--rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/MANIFEST.in
--rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/Makefile
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:24:12.893325 onvif-zeep-async-2.1.4/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/README.rst
--rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/bandit.yaml
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.886771 onvif-zeep-async-2.1.4/examples/
--rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/events.py
--rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/rotate_image.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/examples/streaming.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.887355 onvif-zeep-async-2.1.4/onvif/
--rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    28963 2023-05-06 21:23:49.000000 onvif-zeep-async-2.1.4/onvif/client.py
--rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/definition.py
--rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/exceptions.py
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:23:52.000000 onvif-zeep-async-2.1.4/onvif/version.txt
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.892233 onvif-zeep-async-2.1.4/onvif/wsdl/
--rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-2.1.4/onvif/wsdl/.events.wsdl.swn
--rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/__init__.py
--rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/accesscontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/actionengine.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/addressing
--rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/advancedsecurity.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/analytics.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/analyticsdevice.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/b-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/bf-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/bw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/deviceio.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/devicemgmt.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/display.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/doorcontrol.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/envelope
--rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/events.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/imaging.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/include
--rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/media.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/onvif.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ptz.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/r-2.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/receiver.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/recording.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/remotediscovery.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/replay.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/rw-2.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/search.wsdl
--rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/t-1.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/types.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ws-addr.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/ws-discovery.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/xml.xsd
--rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/onvif/wsdl/xmlmime
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893061 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/
--rw-r--r--   0 bdraco     (501) staff       (20)     5290 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/PKG-INFO
--rw-r--r--   0 bdraco     (501) staff       (20)     1445 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/SOURCES.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/dependency_links.txt
--rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/entry_points.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/not-zip-safe
--rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/requires.txt
--rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-06 21:24:12.000000 onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/top_level.txt
--rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/pylintrc
--rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/pyproject.toml
--rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/requirements.txt
--rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-06 21:24:12.893556 onvif-zeep-async-2.1.4/setup.cfg
--rw-r--r--   0 bdraco     (501) staff       (20)     1801 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/setup.py
-drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-06 21:24:12.893172 onvif-zeep-async-2.1.4/tests/
--rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-2.1.4/tests/test.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618925 onvif-zeep-async-3.0.0/
+-rw-r--r--   0 bdraco     (501) staff       (20)      724 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/.gitignore
+-rw-r--r--   0 bdraco     (501) staff       (20)     1139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/.pre-commit-config.yaml
+-rw-r--r--   0 bdraco     (501) staff       (20)        0 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.0/CHANGES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1087 2023-03-23 19:23:45.000000 onvif-zeep-async-3.0.0/LICENSE
+-rw-r--r--   0 bdraco     (501) staff       (20)      100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/MANIFEST.in
+-rw-r--r--   0 bdraco     (501) staff       (20)     1053 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/Makefile
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:05:28.618984 onvif-zeep-async-3.0.0/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     4926 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/README.rst
+-rw-r--r--   0 bdraco     (501) staff       (20)      188 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/bandit.yaml
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.612363 onvif-zeep-async-3.0.0/examples/
+-rw-r--r--   0 bdraco     (501) staff       (20)     1497 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/events.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1264 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/rotate_image.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2459 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/examples/streaming.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.613187 onvif-zeep-async-3.0.0/onvif/
+-rw-r--r--   0 bdraco     (501) staff       (20)      599 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    39635 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/onvif/client.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     2190 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/definition.py
+-rw-r--r--   0 bdraco     (501) staff       (20)      886 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/exceptions.py
+-rw-r--r--   0 bdraco     (501) staff       (20)     1882 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/onvif/util.py
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:05:09.000000 onvif-zeep-async-3.0.0/onvif/version.txt
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.617982 onvif-zeep-async-3.0.0/onvif/wsdl/
+-rw-r--r--   0 bdraco     (501) staff       (20)    16384 2023-04-16 04:45:10.000000 onvif-zeep-async-3.0.0/onvif/wsdl/.events.wsdl.swn
+-rw-r--r--   0 bdraco     (501) staff       (20)       26 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/__init__.py
+-rw-r--r--   0 bdraco     (501) staff       (20)    38072 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/accesscontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    57255 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/actionengine.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     7263 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/addressing
+-rw-r--r--   0 bdraco     (501) staff       (20)    79284 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/advancedsecurity.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24131 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/analytics.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    31976 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/analyticsdevice.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    23300 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/b-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5100 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/bf-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    20498 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/bw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    60231 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/deviceio.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   163209 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/devicemgmt.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    24593 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/display.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    53648 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/doorcontrol.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     6249 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/envelope
+-rw-r--r--   0 bdraco     (501) staff       (20)    37870 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/events.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    17998 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/imaging.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)      511 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/include
+-rw-r--r--   0 bdraco     (501) staff       (20)   174812 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/media.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)   363349 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/onvif.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    54058 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ptz.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3660 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/r-2.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    17214 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/receiver.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    40704 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/recording.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     5596 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/remotediscovery.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    10581 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/replay.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     3727 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/rw-2.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)    43139 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/search.wsdl
+-rw-r--r--   0 bdraco     (501) staff       (20)     8960 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/t-1.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     3738 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/types.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     5849 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ws-addr.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)    10455 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/ws-discovery.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     8836 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/xml.xsd
+-rw-r--r--   0 bdraco     (501) staff       (20)     1639 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/onvif/wsdl/xmlmime
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618724 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/
+-rw-r--r--   0 bdraco     (501) staff       (20)     5292 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/PKG-INFO
+-rw-r--r--   0 bdraco     (501) staff       (20)     1459 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/SOURCES.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/dependency_links.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)       45 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/entry_points.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        1 2023-03-23 19:28:21.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/not-zip-safe
+-rw-r--r--   0 bdraco     (501) staff       (20)       47 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/requires.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)        6 2023-05-07 01:05:28.000000 onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/top_level.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)     1741 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/pylintrc
+-rw-r--r--   0 bdraco     (501) staff       (20)       77 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/pyproject.toml
+-rw-r--r--   0 bdraco     (501) staff       (20)      224 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/requirements.txt
+-rw-r--r--   0 bdraco     (501) staff       (20)      409 2023-05-07 01:05:28.619230 onvif-zeep-async-3.0.0/setup.cfg
+-rw-r--r--   0 bdraco     (501) staff       (20)     1803 2023-05-07 01:05:04.000000 onvif-zeep-async-3.0.0/setup.py
+drwxr-xr-x   0 bdraco     (501) staff       (20)        0 2023-05-07 01:05:28.618821 onvif-zeep-async-3.0.0/tests/
+-rw-r--r--   0 bdraco     (501) staff       (20)     4133 2023-04-30 15:25:07.000000 onvif-zeep-async-3.0.0/tests/test.py
```

### Comparing `onvif-zeep-async-2.1.4/.gitignore` & `onvif-zeep-async-3.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/.pre-commit-config.yaml` & `onvif-zeep-async-3.0.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/LICENSE` & `onvif-zeep-async-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/Makefile` & `onvif-zeep-async-3.0.0/Makefile`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/PKG-INFO` & `onvif-zeep-async-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.4
+Version: 3.0.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
 Keywords: ONVIF,Camera,IPC
-Requires-Python: >=3
+Requires-Python: >=3.9
 License-File: LICENSE
 
 python-onvif-zeep-async
 =======================
 
 ONVIF Client Implementation in Python 3
```

### Comparing `onvif-zeep-async-2.1.4/README.rst` & `onvif-zeep-async-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/examples/events.py` & `onvif-zeep-async-3.0.0/examples/events.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/examples/rotate_image.py` & `onvif-zeep-async-3.0.0/examples/rotate_image.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/examples/streaming.py` & `onvif-zeep-async-3.0.0/examples/streaming.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/__init__.py` & `onvif-zeep-async-3.0.0/onvif/__init__.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/client.py` & `onvif-zeep-async-3.0.0/onvif/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,65 @@
 """ONVIF Client."""
+from __future__ import annotations
+
+from abc import abstractmethod
 import asyncio
+from collections.abc import Awaitable
 import contextlib
 import datetime as dt
-from functools import lru_cache
+from functools import lru_cache, partial
 import logging
 import os.path
 import ssl
-from typing import Any, Awaitable, Callable, Dict, Optional, ParamSpec, Tuple, TypeVar
+from typing import Any, Callable, Dict, Optional, ParamSpec, Tuple, TypeVar
 
 import httpx
 from httpx import AsyncClient, BasicAuth, DigestAuth, TransportError
 from zeep.cache import SqliteCache
 from zeep.client import AsyncClient as BaseZeepAsyncClient, Settings
-from zeep.exceptions import Fault, XMLSyntaxError
+from zeep.exceptions import Fault, XMLParseError, XMLSyntaxError
 import zeep.helpers
 from zeep.loader import parse_xml
 from zeep.proxy import AsyncServiceProxy
 from zeep.transports import AsyncTransport, Transport
 from zeep.wsa import WsAddressingPlugin
 from zeep.wsdl import Document
 from zeep.wsdl.bindings.soap import SoapOperation
 from zeep.wsse.username import UsernameToken
 
 from onvif.definition import SERVICES
 from onvif.exceptions import ONVIFAuthError, ONVIFError, ONVIFTimeoutError
 
+from .util import extract_subcodes_as_strings, is_auth_error, stringify_onvif_error
+
 logger = logging.getLogger("onvif")
 logging.basicConfig(level=logging.INFO)
 logging.getLogger("zeep.client").setLevel(logging.CRITICAL)
 
 _DEFAULT_SETTINGS = Settings()
 _DEFAULT_SETTINGS.strict = False
 _DEFAULT_SETTINGS.xml_huge_tree = True
 
 _WSDL_PATH = os.path.join(os.path.dirname(os.path.dirname(__file__)), "wsdl")
 
-_DEFAULT_TIMEOUT = 30
-_PULLPOINT_TIMEOUT = 80
+_DEFAULT_TIMEOUT = 90
+_PULLPOINT_TIMEOUT = 90
 _CONNECT_TIMEOUT = 30
-_READ_TIMEOUT = 30
-_WRITE_TIMEOUT = 30
+_READ_TIMEOUT = 90
+_WRITE_TIMEOUT = 90
 
+_RENEWAL_PERCENTAGE = 0.8
 
 KEEPALIVE_EXPIRY = 4
 BACKOFF_TIME = KEEPALIVE_EXPIRY + 0.5
 HTTPX_LIMITS = httpx.Limits(keepalive_expiry=4)
 
+SUBSCRIPTION_ERRORS = (Fault, asyncio.TimeoutError, TransportError)
+RENEW_ERRORS = (ONVIFError, httpx.RequestError, XMLParseError, *SUBSCRIPTION_ERRORS)
+SUBSCRIPTION_RESTART_INTERVAL_ON_ERROR = dt.timedelta(seconds=40)
 
 DEFAULT_ATTEMPTS = 2
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
 
@@ -238,25 +248,24 @@
         device_service.SetHostname(params)
     """
 
     @safe_func
     def __init__(
         self,
         xaddr: str,
-        user: Optional[str],
-        passwd: Optional[str],
+        user: str | None,
+        passwd: str | None,
         url: str,
         encrypt=True,
         no_cache=False,
         dt_diff=None,
         binding_name="",
         binding_key="",
-        read_timeout: Optional[int] = None,
-        write_timeout: Optional[int] = None,
-        enable_wsa: bool = False,
+        read_timeout: int | None = None,
+        write_timeout: int | None = None,
     ) -> None:
         if not _path_isfile(url):
             raise ONVIFError("%s doesn`t exist!" % url)
 
         self.url = url
         self.xaddr = xaddr
         self.binding_key = binding_key
@@ -286,52 +295,47 @@
         self.transport = (
             AsyncTransport(client=client, wsdl_client=wsdl_client)
             if no_cache
             else AsyncTransport(
                 client=client, wsdl_client=wsdl_client, cache=SqliteCache()
             )
         )
-        self.document: Optional[Document] = None
-        self.zeep_client_authless: Optional[ZeepAsyncClient] = None
-        self.ws_client_authless: Optional[AsyncServiceProxy] = None
-        self.zeep_client: Optional[ZeepAsyncClient] = None
-        self.ws_client: Optional[AsyncServiceProxy] = None
-        self.create_type: Optional[Callable] = None
+        self.document: Document | None = None
+        self.zeep_client_authless: ZeepAsyncClient | None = None
+        self.ws_client_authless: AsyncServiceProxy | None = None
+        self.zeep_client: ZeepAsyncClient | None = None
+        self.ws_client: AsyncServiceProxy | None = None
+        self.create_type: Callable | None = None
         self.loop = asyncio.get_event_loop()
-        self._enable_wsa = enable_wsa
 
     async def setup(self):
         """Setup the transport."""
         settings = _DEFAULT_SETTINGS
         binding_name = self.binding_name
         wsse = UsernameDigestTokenDtDiff(
             self.user, self.passwd, dt_diff=self.dt_diff, use_digest=self.encrypt
         )
         self.document = await self.loop.run_in_executor(
             None, _cached_document, self.url
         )
-        # Some cameras never return a response to GetCapabilities if WS-Addressing is enabled
-        # but some cameras require WS-Addressing to be enabled for PullPoint or events to work
-        # so we have a flag to enable/disable it which can be changed per service.
-        plugins = [WsAddressingPlugin()] if self._enable_wsa else []
         self.zeep_client_authless = ZeepAsyncClient(
             wsdl=self.document,
             transport=self.transport,
             settings=settings,
-            plugins=plugins,
+            plugins=[WsAddressingPlugin()],
         )
         self.ws_client_authless = self.zeep_client_authless.create_service(
             binding_name, self.xaddr
         )
         self.zeep_client = ZeepAsyncClient(
             wsdl=self.document,
             wsse=wsse,
             transport=self.transport,
             settings=settings,
-            plugins=plugins,
+            plugins=[WsAddressingPlugin()],
         )
         self.ws_client = self.zeep_client.create_service(binding_name, self.xaddr)
         namespace = binding_name[binding_name.find("{") + 1 : binding_name.find("}")]
         available_ns = self.zeep_client.namespaces
         active_ns = (
             list(available_ns.keys())[list(available_ns.values()).index(namespace)]
             or "ns0"
@@ -381,60 +385,242 @@
         if builtin:
             return self.__dict__[name]
         if name.startswith("authless_"):
             return service_wrapper(getattr(self.ws_client_authless, name.split("_")[1]))
         return service_wrapper(getattr(self.ws_client, name))
 
 
-class NotificationManager:
-    """Manager to process notifications."""
+class BaseManager:
+    """Base class for notification and pull point managers."""
 
-    def __init__(self, device: "ONVIFCamera", config: Dict[str, Any]) -> None:
+    def __init__(
+        self,
+        device: ONVIFCamera,
+        interval: dt.timedelta,
+        subscription_lost_callback: Callable[[], None],
+    ) -> None:
         """Initialize the notification processor."""
-        self._service: Optional[ONVIFService] = None
-        self._operation: Optional[SoapOperation] = None
+        self._operation: SoapOperation | None = None
         self._device = device
-        self._config = config
+        self._interval = interval
+        self._renew_lock = asyncio.Lock()
+        self._subscription: ONVIFService | None = None
+        self._restart_or_renew_task: asyncio.Task | None = None
+        self._loop = asyncio.get_event_loop()
+        self._shutdown = False
+        self._subscription_lost_callback = subscription_lost_callback
+        self._cancel_subscription_renew: asyncio.TimerHandle | None = None
+
+    @property
+    def closed(self) -> bool:
+        """Return True if the manager is closed."""
+        return not self._subscription or self._subscription.transport.client.is_closed
+
+    @abstractmethod
+    async def _start(self) -> float:
+        """Setup the processor.
+
+        Returns the next renewal call at time.
+
+        """
+
+    async def _set_synchronization_point(self, service: ONVIFService) -> float:
+        """Set the synchronization point."""
+        try:
+            await service.SetSynchronizationPoint()
+        except (Fault, asyncio.TimeoutError, TransportError, TypeError):
+            logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
 
-    async def setup(self) -> ONVIFService:
+    async def start(self) -> None:
         """Setup the notification processor."""
-        notify_service = await self._device.create_notification_service()
-        notify_subscribe = await notify_service.Subscribe(self._config)
+        renewal_call_at = await self._start()
+        self._schedule_subscription_renew(renewal_call_at)
+        return self._subscription
+
+    def pause(self) -> None:
+        """Pause the notification processor."""
+        self._cancel_renewals()
+
+    def resume(self) -> None:
+        """Resume the notification processor."""
+        self._schedule_subscription_renew(self._loop.time())
+
+    async def stop(self) -> None:
+        """Stop the notification processor."""
+        logger.debug("%s: Stop the notification manager", self._device.host)
+        self._cancel_renewals()
+        assert self._subscription, "Call start first"
+        await self._subscription.Unsubscribe()
+
+    async def shutdown(self) -> None:
+        """Shutdown the notification processor."""
+        self._shutdown = True
+        if self._restart_or_renew_task:
+            self._restart_or_renew_task.cancel()
+        logger.debug("%s: Shutdown the notification manager", self._device.host)
+        await self.stop()
+
+    async def renew(self) -> float:
+        """Renew the notification subscription."""
+        device = self._device
+        logger.debug("%s: Renew the notification manager", device.host)
+        return self._calculate_next_renewal_call_at(
+            await self._subscription.Renew(
+                device.get_next_termination_time(self._interval)
+            )
+        )
+
+    def _cancel_renewals(self) -> None:
+        """Cancel any pending renewals."""
+        if self._cancel_subscription_renew:
+            self._cancel_subscription_renew.cancel()
+            self._cancel_subscription_renew = None
+
+    def _calculate_next_renewal_call_at(self, result: Any | None) -> float:
+        """Calculate the next renewal call_at."""
+        current_time: dt.datetime | None = result.CurrentTime
+        termination_time: dt.datetime | None = result.TerminationTime
+        if termination_time and current_time:
+            delay = termination_time - current_time
+        else:
+            delay = self._interval
+        delay_seconds = delay.total_seconds() * _RENEWAL_PERCENTAGE
+        logger.debug(
+            "%s: Renew notification subscription in %s seconds",
+            self._device.host,
+            delay_seconds,
+        )
+        return self._loop.time() + delay_seconds
+
+    def _schedule_subscription_renew(self, when: float) -> None:
+        """Schedule notify subscription renewal."""
+        self._cancel_renewals()
+        self._cancel_subscription_renew = self._loop.call_at(
+            when,
+            self._run_restart_or_renew,
+        )
+
+    def _run_restart_or_renew(self) -> None:
+        """Create a background task."""
+        if self._restart_or_renew_task and not self._restart_or_renew_task.done():
+            logger.debug("%s: Notify renew already in progress", self._device.host)
+            return
+        self._restart_or_renew_task = asyncio.create_task(
+            self._renew_or_restart_subscription()
+        )
+
+    async def _restart_subscription(self) -> bool:
+        """Restart the notify subscription assuming the camera rebooted."""
+        self._cancel_renewals()
+        return await self._start()
+
+    @retry_connection_error()
+    async def _call_subscription_renew(self) -> float:
+        """Call notify subscription Renew."""
+        return await self.renew()
+
+    async def _renew_subscription(self) -> float | None:
+        """Renew notify subscription."""
+        if self.closed or self._shutdown:
+            return None
+        try:
+            return await self._call_subscription_renew()
+        except RENEW_ERRORS as err:
+            self._subscription_lost_callback()
+            logger.debug(
+                "%s: Failed to renew notify subscription %s",
+                self._device.host,
+                stringify_onvif_error(err),
+            )
+        return None
+
+    async def _renew_or_restart_subscription(
+        self, now: dt.datetime | None = None
+    ) -> None:
+        """Renew or start notify subscription."""
+        if self._shutdown:
+            return
+        renewal_call_at = None
+        try:
+            renewal_call_at = (
+                await self._renew_subscription() or await self._restart_subscription()
+            )
+        finally:
+            self._schedule_subscription_renew(
+                renewal_call_at
+                or self._loop.time()
+                + SUBSCRIPTION_RESTART_INTERVAL_ON_ERROR.total_seconds()
+            )
+
+
+class NotificationManager(BaseManager):
+    """Manager to process notifications."""
+
+    def __init__(
+        self,
+        device: ONVIFCamera,
+        address: str,
+        interval: dt.timedelta,
+        subscription_lost_callback: Callable[[], None],
+    ) -> None:
+        """Initialize the notification processor."""
+        self._address = address
+        super().__init__(device, interval, subscription_lost_callback)
+
+    async def _start(self) -> float:
+        """Start the notification processor.
+
+        Returns the next renewal call at time.
+        """
+        device = self._device
+        logger.debug("%s: Setup the notification manager", device.host)
+        notify_service = await device.create_notification_service()
+        time_str = device.get_next_termination_time(self._interval)
+        result = await notify_service.Subscribe(
+            {
+                "InitialTerminationTime": time_str,
+                "ConsumerReference": {"Address": self._address},
+            }
+        )
         # pylint: disable=protected-access
-        self._device.xaddrs[
+        device.xaddrs[
             "http://www.onvif.org/ver10/events/wsdl/NotificationConsumer"
-        ] = notify_subscribe.SubscriptionReference.Address._value_1
+        ] = result.SubscriptionReference.Address._value_1
         # Create subscription manager
         # 5.2.3 BASIC NOTIFICATION INTERFACE - NOTIFY
         # Call SetSynchronizationPoint to generate a notification message
         # to ensure the webhooks are working.
         #
         # If this fails this is OK as it just means we will switch
         # to webhook later when the first notification is received.
-        #
-        # WSAs not enabled on this service per
-        # https://github.com/home-assistant/core/issues/92308
         service = await self._device.create_onvif_service(
             "pullpoint", port_type="NotificationConsumer"
         )
         self._operation = service.document.bindings[service.binding_name].get(
             "PullMessages"
         )
-        self._service = service
-        return await self._device.create_subscription_service("NotificationConsumer")
-
-    async def start(self) -> None:
-        """Start the notification processor."""
-        assert self._service, "Call setup first"
-        try:
-            await self._service.SetSynchronizationPoint()
-        except (Fault, asyncio.TimeoutError, TransportError, TypeError):
-            logger.debug("%s: SetSynchronizationPoint failed", self._service.url)
+        self._subscription = await device.create_subscription_service(
+            "NotificationConsumer"
+        )
+        if device.has_broken_relative_time(
+            self._interval,
+            result.CurrentTime,
+            result.TerminationTime,
+        ):
+            # If we determine the device has broken relative timestamps, we switch
+            # to using absolute timestamps and renew the subscription.
+            result = await self._subscription.Renew(
+                device.get_next_termination_time(self._interval)
+            )
+        renewal_call_at = self._calculate_next_renewal_call_at(result)
+        logger.debug("%s: Start the notification manager", self._device.host)
+        await self._set_synchronization_point(service)
+        return renewal_call_at
 
-    def process(self, content: bytes) -> Optional[Any]:
+    def process(self, content: bytes) -> Any | None:
         """Process a notification message."""
         if not self._operation:
             logger.debug("%s: Notifications not setup", self._device.host)
             return
         try:
             envelope = parse_xml(
                 content,  # type: ignore[arg-type]
@@ -443,14 +629,73 @@
             )
         except XMLSyntaxError as exc:
             logger.error("Received invalid XML: %s", exc)
             return None
         return self._operation.process_reply(envelope)
 
 
+class PullPointManager(BaseManager):
+    """Manager for PullPoint."""
+
+    def __init__(
+        self,
+        device: ONVIFCamera,
+        interval: dt.timedelta,
+        subscription_lost_callback: Callable[[], None],
+    ) -> None:
+        """Initialize the PullPoint processor."""
+        super().__init__(device, interval, subscription_lost_callback)
+        self._service: ONVIFService | None = None
+
+    async def _start(self) -> float:
+        """Start the PullPoint manager.
+
+        Returns the next renewal call at time.
+        """
+        device = self._device
+        logger.debug("%s: Setup the PullPoint manager", device.host)
+        events_service = await device.create_events_service()
+        result = await events_service.CreatePullPointSubscription(
+            {
+                "InitialTerminationTime": device.get_next_termination_time(
+                    self._interval
+                ),
+            }
+        )
+        # pylint: disable=protected-access
+        device.xaddrs[
+            "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
+        ] = result.SubscriptionReference.Address._value_1
+        # Create subscription manager
+        self._subscription = await device.create_subscription_service(
+            "PullPointSubscription"
+        )
+        # Create the service that will be used to pull messages from the device.
+        self._service = await device.create_pullpoint_service()
+        if device.has_broken_relative_time(
+            self._interval, result.CurrentTime, result.TerminationTime
+        ):
+            # If we determine the device has broken relative timestamps, we switch
+            # to using absolute timestamps and renew the subscription.
+            result = await self._subscription.Renew(
+                device.get_next_termination_time(self._interval)
+            )
+        renewal_call_at = self._calculate_next_renewal_call_at(result)
+        logger.debug("%s: Start the notification manager", self._device.host)
+        await self._set_synchronization_point(self._service)
+        return renewal_call_at
+
+    def get_service(self) -> ONVIFService:
+        """Return the pullpoint service."""
+        return self._service
+
+
+_utcnow: partial[dt.datetime] = partial(dt.datetime.now, dt.timezone.utc)
+
+
 class ONVIFCamera:
     """
     Python Implementation ONVIF compliant device
     This class integrates onvif services
 
     adjust_time parameter allows authentication on cameras without being time synchronized.
     Please note that using NTP on both end is the recommended solution,
@@ -468,16 +713,16 @@
     >>> ptz_service.GetConfiguration()
     """
 
     def __init__(
         self,
         host: str,
         port: int,
-        user: Optional[str],
-        passwd: Optional[str],
+        user: str | None,
+        passwd: str | None,
         wsdl_dir: str = _WSDL_PATH,
         encrypt=True,
         no_cache=False,
         adjust_time=False,
     ) -> None:
         os.environ.pop("http_proxy", None)
         os.environ.pop("https_proxy", None)
@@ -487,25 +732,26 @@
         self.passwd = passwd
         self.wsdl_dir = wsdl_dir
         self.encrypt = encrypt
         self.no_cache = no_cache
         self.adjust_time = adjust_time
         self.dt_diff = None
         self.xaddrs = {}
-        self._capabilities: Optional[Dict[str, Any]] = None
+        self._has_broken_relative_timestamps: bool = False
+        self._capabilities: dict[str, Any] | None = None
 
         # Active service client container
-        self.services: Dict[Tuple[str, Optional[str]], ONVIFService] = {}
+        self.services: dict[tuple[str, str | None], ONVIFService] = {}
 
         self.to_dict = ONVIFService.to_dict
 
         self._snapshot_uris = {}
         self._snapshot_client = AsyncClient(verify=_NO_VERIFY_SSL_CONTEXT)
 
-    async def get_capabilities(self) -> Dict[str, Any]:
+    async def get_capabilities(self) -> dict[str, Any]:
         """Get device capabilities."""
         if self._capabilities is None:
             await self.update_xaddrs()
         return self._capabilities
 
     async def update_xaddrs(self):
         """Update xaddrs for services."""
@@ -543,34 +789,95 @@
             except Exception:
                 logger.exception("Unexpected service type")
         try:
             self._capabilities = self.to_dict(capabilities)
         except Exception:
             logger.exception("Failed to parse capabilities")
 
-    async def create_pullpoint_subscription(
-        self, config: Optional[Dict[str, Any]] = None
+    def has_broken_relative_time(
+        self,
+        expected_interval: dt.timedelta,
+        current_time: dt.datetime | None,
+        termination_time: dt.datetime | None,
     ) -> bool:
-        """Create a pullpoint subscription."""
-        try:
-            events = await self.create_events_service()
-            pullpoint = await events.CreatePullPointSubscription(config or {})
-            # pylint: disable=protected-access
-            self.xaddrs[
-                "http://www.onvif.org/ver10/events/wsdl/PullPointSubscription"
-            ] = pullpoint.SubscriptionReference.Address._value_1
-        except Fault:
+        """Mark timestamps as broken if a subscribe request returns an unexpected result."""
+        logger.debug(
+            "%s: Checking for broken relative timestamps: expected_interval: %s, current_time: %s, termination_time: %s",
+            self.host,
+            expected_interval,
+            current_time,
+            termination_time,
+        )
+        if not current_time:
+            logger.debug("%s: Device returned no current time", self.host)
+            return False
+        if not termination_time:
+            logger.debug("%s: Device returned no current time", self.host)
             return False
-        return True
+        if current_time.tzinfo is None:
+            logger.debug(
+                "%s: Device returned no timezone info for current time", self.host
+            )
+            return False
+        if termination_time.tzinfo is None:
+            logger.debug(
+                "%s: Device returned no timezone info for termination time", self.host
+            )
+            return False
+        actual_interval = termination_time - current_time
+        if abs(actual_interval.total_seconds()) < (
+            expected_interval.total_seconds() / 2
+        ):
+            logger.debug(
+                "%s: Broken relative timestamps detected, switching to absolute timestamps: expected interval: %s, actual interval: %s",
+                self.host,
+                expected_interval,
+                actual_interval,
+            )
+            self._has_broken_relative_timestamps = True
+            return True
+        logger.debug(
+            "%s: Relative timestamps OK: expected interval: %s, actual interval: %s",
+            self.host,
+            expected_interval,
+            actual_interval,
+        )
+        return False
+
+    def get_next_termination_time(self, duration: dt.timedelta) -> str:
+        """Calculate subscription absolute termination time."""
+        if not self._has_broken_relative_timestamps:
+            return f"PT{int(duration.total_seconds())}S"
+        absolute_time: dt.datetime = _utcnow() + duration
+        if dt_diff := self.dt_diff:
+            absolute_time += dt_diff
+        return absolute_time.isoformat(timespec="seconds").replace("+00:00", "Z")
 
-    def create_notification_manager(
-        self, config: Optional[Dict[str, Any]] = None
+    async def create_pullpoint_manager(
+        self,
+        interval: dt.timedelta,
+        subscription_lost_callback: Callable[[], None],
+    ) -> PullPointManager:
+        """Create a pullpoint manager."""
+        manager = PullPointManager(self, interval, subscription_lost_callback)
+        await manager.start()
+        return manager
+
+    async def create_notification_manager(
+        self,
+        address: str,
+        interval: dt.timedelta,
+        subscription_lost_callback: Callable[[], None],
     ) -> NotificationManager:
         """Create a notification manager."""
-        return NotificationManager(self, config)
+        manager = NotificationManager(
+            self, address, interval, subscription_lost_callback
+        )
+        await manager.start()
+        return manager
 
     async def close(self) -> None:
         """Close all transports."""
         await self._snapshot_client.aclose()
         for service in self.services.values():
             await service.close()
 
@@ -584,15 +891,15 @@
             result = await media_service.GetSnapshotUri(req)
             uri = result.Uri
             self._snapshot_uris[profile_token] = uri
         return uri
 
     async def get_snapshot(
         self, profile_token: str, basic_auth: bool = False
-    ) -> Optional[bytes]:
+    ) -> bytes | None:
         """Get a snapshot image from the camera."""
         uri = await self.get_snapshot_uri(profile_token)
         if uri is None:
             return None
 
         auth = None
         if self.user and self.passwd:
@@ -613,16 +920,16 @@
 
         if response.status_code < 300:
             return response.content
 
         return None
 
     def get_definition(
-        self, name: str, port_type: Optional[str] = None
-    ) -> Tuple[str, str, str]:
+        self, name: str, port_type: str | None = None
+    ) -> tuple[str, str, str]:
         """Returns xaddr and wsdl of specified service"""
         # Check if the service is supported
         if name not in SERVICES:
             raise ONVIFError("Unknown service %s" % name)
         wsdl_file = SERVICES[name]["wsdl"]
         namespace = SERVICES[name]["ns"]
 
@@ -651,18 +958,17 @@
             raise ONVIFError("Device doesn`t support service: %s" % name)
 
         return xaddr, wsdlpath, binding_name
 
     async def create_onvif_service(
         self,
         name: str,
-        port_type: Optional[str] = None,
-        read_timeout: Optional[int] = None,
-        write_timeout: Optional[int] = None,
-        enable_wsa: bool = False,
+        port_type: str | None = None,
+        read_timeout: int | None = None,
+        write_timeout: int | None = None,
     ) -> ONVIFService:
         """Create ONVIF service client"""
         name = name.lower()
         # Don't re-create bindings if the xaddr remains the same.
         # The xaddr can change when a new PullPointSubscription is created.
         binding_key = (name, port_type)
 
@@ -693,15 +999,14 @@
             self.encrypt,
             no_cache=self.no_cache,
             dt_diff=self.dt_diff,
             binding_name=binding_name,
             binding_key=binding_key,
             read_timeout=read_timeout,
             write_timeout=write_timeout,
-            enable_wsa=enable_wsa,
         )
         await service.setup()
 
         self.services[binding_key] = service
 
         return service
 
@@ -722,19 +1027,15 @@
         return await self.create_onvif_service("imaging")
 
     async def create_deviceio_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("deviceio")
 
     async def create_events_service(self) -> ONVIFService:
-        """Service creation helper.
-
-        WSAs not enabled on this service per
-        https://github.com/home-assistant/core/issues/92308
-        """
+        """Service creation helper."""
         return await self.create_onvif_service("events")
 
     async def create_analytics_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("analytics")
 
     async def create_recording_service(self) -> ONVIFService:
@@ -746,42 +1047,28 @@
         return await self.create_onvif_service("search")
 
     async def create_replay_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("replay")
 
     async def create_pullpoint_service(self) -> ONVIFService:
-        """Service creation helper.
-
-        WSAs not enabled on this service per
-        https://github.com/home-assistant/core/issues/92308
-        """
+        """Service creation helper."""
         return await self.create_onvif_service(
             "pullpoint",
             port_type="PullPointSubscription",
             read_timeout=_PULLPOINT_TIMEOUT,
             write_timeout=_PULLPOINT_TIMEOUT,
         )
 
     async def create_notification_service(self) -> ONVIFService:
-        """Service creation helper.
-
-        WSAs not enabled on this service per
-        https://github.com/home-assistant/core/issues/92308
-        """
+        """Service creation helper."""
         return await self.create_onvif_service("notification")
 
     async def create_subscription_service(
-        self, port_type: Optional[str] = None
+        self, port_type: str | None = None
     ) -> ONVIFService:
-        """Service creation helper.
-
-        WSAs enabled per
-        https://github.com/home-assistant/core/issues/83524 https://github.com/home-assistant/core/issues/45513
-        """
-        return await self.create_onvif_service(
-            "subscription", port_type=port_type, enable_wsa=True
-        )
+        """Service creation helper."""
+        return await self.create_onvif_service("subscription", port_type=port_type)
 
     async def create_receiver_service(self) -> ONVIFService:
         """Service creation helper."""
         return await self.create_onvif_service("receiver")
```

### Comparing `onvif-zeep-async-2.1.4/onvif/definition.py` & `onvif-zeep-async-3.0.0/onvif/definition.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/exceptions.py` & `onvif-zeep-async-3.0.0/onvif/exceptions.py`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/.events.wsdl.swn` & `onvif-zeep-async-3.0.0/onvif/wsdl/.events.wsdl.swn`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/accesscontrol.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/accesscontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/actionengine.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/actionengine.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/addressing` & `onvif-zeep-async-3.0.0/onvif/wsdl/addressing`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/advancedsecurity.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/advancedsecurity.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/analytics.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/analytics.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/analyticsdevice.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/analyticsdevice.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/b-2.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/b-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/bf-2.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/bf-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/bw-2.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/bw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/deviceio.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/deviceio.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/devicemgmt.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/devicemgmt.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/display.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/display.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/doorcontrol.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/doorcontrol.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/envelope` & `onvif-zeep-async-3.0.0/onvif/wsdl/envelope`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/events.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/events.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/imaging.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/imaging.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/media.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/media.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/onvif.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/onvif.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/ptz.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/ptz.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/r-2.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/r-2.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/receiver.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/receiver.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/recording.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/recording.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/remotediscovery.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/remotediscovery.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/replay.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/replay.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/rw-2.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/rw-2.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/search.wsdl` & `onvif-zeep-async-3.0.0/onvif/wsdl/search.wsdl`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/t-1.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/t-1.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/types.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/types.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/ws-addr.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/ws-addr.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/ws-discovery.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/ws-discovery.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/xml.xsd` & `onvif-zeep-async-3.0.0/onvif/wsdl/xml.xsd`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif/wsdl/xmlmime` & `onvif-zeep-async-3.0.0/onvif/wsdl/xmlmime`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/PKG-INFO` & `onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: onvif-zeep-async
-Version: 2.1.4
+Version: 3.0.0
 Summary: Async Python Client for ONVIF Camera
 Home-page: http://github.com/hunterjm/python-onvif-zeep-async
 Author: Cherish Chen
 Author-email: sinchb128@gmail.com
 Maintainer: sinchb
 Maintainer-email: sinchb128@gmail.com
 License: MIT
 Keywords: ONVIF,Camera,IPC
-Requires-Python: >=3
+Requires-Python: >=3.9
 License-File: LICENSE
 
 python-onvif-zeep-async
 =======================
 
 ONVIF Client Implementation in Python 3
```

### Comparing `onvif-zeep-async-2.1.4/onvif_zeep_async.egg-info/SOURCES.txt` & `onvif-zeep-async-3.0.0/onvif_zeep_async.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 examples/events.py
 examples/rotate_image.py
 examples/streaming.py
 onvif/__init__.py
 onvif/client.py
 onvif/definition.py
 onvif/exceptions.py
+onvif/util.py
 onvif/version.txt
 onvif/wsdl/.events.wsdl.swn
 onvif/wsdl/__init__.py
 onvif/wsdl/accesscontrol.wsdl
 onvif/wsdl/actionengine.wsdl
 onvif/wsdl/addressing
 onvif/wsdl/advancedsecurity.wsdl
```

### Comparing `onvif-zeep-async-2.1.4/pylintrc` & `onvif-zeep-async-3.0.0/pylintrc`

 * *Files identical despite different names*

### Comparing `onvif-zeep-async-2.1.4/setup.py` & `onvif-zeep-async-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     author_email="sinchb128@gmail.com",
     maintainer="sinchb",
     maintainer_email="sinchb128@gmail.com",
     license="MIT",
     keywords=["ONVIF", "Camera", "IPC"],
     url="http://github.com/hunterjm/python-onvif-zeep-async",
     zip_safe=False,
-    python_requires=">=3",
+    python_requires=">=3.9",
     packages=find_packages(exclude=["docs", "examples", "tests"]),
     install_requires=requires,
     package_data={
         "": ["*.txt", "*.rst"],
         "onvif": ["*.wsdl", "*.xsd", "*xml*", "envelope", "include", "addressing"],
         "onvif.wsdl": ["*.wsdl", "*.xsd", "*xml*", "envelope", "include", "addressing"],
     },
```

### Comparing `onvif-zeep-async-2.1.4/tests/test.py` & `onvif-zeep-async-3.0.0/tests/test.py`

 * *Files identical despite different names*

