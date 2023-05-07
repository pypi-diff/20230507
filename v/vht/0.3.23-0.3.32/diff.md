# Comparing `tmp/vht-0.3.23.tar.gz` & `tmp/vht-0.3.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vht-0.3.23.tar", last modified: Tue Apr 25 21:55:30 2023, max compression
+gzip compressed data, was "vht-0.3.32.tar", last modified: Sun May  7 09:57:25 2023, max compression
```

## Comparing `vht-0.3.23.tar` & `vht-0.3.32.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.300751 vht-0.3.23/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2022-12-31 13:17:54.000000 vht-0.3.23/LICENSE
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2022-12-31 13:17:54.000000 vht-0.3.23/MANIFEST.in
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-04-25 21:55:30.300751 vht-0.3.23/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1255 2023-04-25 21:49:33.000000 vht-0.3.23/README.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.280752 vht-0.3.23/data/
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.280752 vht-0.3.23/data/bank/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2022-12-31 13:17:54.000000 vht-0.3.23/data/bank/10-gm1
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2022-12-31 13:17:54.000000 vht-0.3.23/data/bank/20-gm2
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      290 2022-12-31 13:17:54.000000 vht-0.3.23/data/com.github.rdybka.vht.desktop
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.280752 vht-0.3.23/data/ctrl/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2022-12-31 13:17:54.000000 vht-0.3.23/data/ctrl/10-gm
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2022-12-31 13:17:54.000000 vht-0.3.23/data/ctrl/20-zyn
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2022-12-31 13:17:54.000000 vht-0.3.23/data/mandy.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2022-12-31 13:17:54.000000 vht-0.3.23/data/menu.ui
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2022-12-31 13:17:54.000000 vht-0.3.23/data/vht.png
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2022-12-31 13:17:54.000000 vht-0.3.23/data/vht.svg
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.280752 vht-0.3.23/doc/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2367 2023-03-23 02:01:12.000000 vht-0.3.23/doc/vht.1.gz
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4642 2023-03-23 02:01:02.000000 vht-0.3.23/doc/vht.1.md
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.292751 vht-0.3.23/libvht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/ctrlrow.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/ctrlrow.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7095 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/envelope.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/envelope.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1960 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/jack_process.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/jack_process.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19730 2023-01-30 08:50:38.000000 vht-0.3.23/libvht/libcvht.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31881 2023-04-25 21:49:54.000000 vht-0.3.23/libvht/libcvht.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   477234 2023-04-25 21:49:54.000000 vht-0.3.23/libvht/libcvht_wrap.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8287 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/libvht.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34606 2023-03-21 11:13:05.000000 vht-0.3.23/libvht/mandy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2023-03-31 14:55:44.000000 vht-0.3.23/libvht/mandy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/mandy_pix_scan.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/mandy_pix_scan.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/mandy_trk_disp.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/mandy_trk_disp.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    16444 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/midi_client.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4381 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/midi_client.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/midi_event.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/midi_event.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15439 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/module.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3151 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/module.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3036 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/row.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/row.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28715 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/sequence.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4464 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/sequence.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29202 2023-03-23 02:07:54.000000 vht-0.3.23/libvht/timeline.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2022-12-31 13:17:54.000000 vht-0.3.23/libvht/timeline.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41059 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/track.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2023-01-30 08:43:51.000000 vht-0.3.23/libvht/track.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2023-03-21 08:03:40.000000 vht-0.3.23/libvht/tracy.c
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2023-03-20 13:26:10.000000 vht-0.3.23/libvht/tracy.h
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtcolumn.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtctrl.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtctrllist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtctrlrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtextras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtmandy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21012 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtmodule.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3283 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtport.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtports.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtquicklist.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhtrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10811 2023-03-31 15:37:38.000000 vht-0.3.23/libvht/vhtsequence.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimeline.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelinechange.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelinechanges.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelineloop.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelineslices.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelinestrip.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelinestrips.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttimelineticks.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttrack.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2023-03-21 08:03:58.000000 vht-0.3.23/libvht/vhttracy.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1693 2023-04-25 21:33:50.000000 vht-0.3.23/pyproject.toml
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      108 2023-04-25 21:55:30.300751 vht-0.3.23/setup.cfg
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1796 2023-03-23 02:00:37.000000 vht-0.3.23/setup.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.300751 vht-0.3.23/vht/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2022-12-31 13:17:54.000000 vht-0.3.23/vht/__init__.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2023-03-21 08:04:15.000000 vht-0.3.23/vht/autoexec.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2023-03-21 08:04:15.000000 vht-0.3.23/vht/bankcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2023-03-21 08:04:15.000000 vht-0.3.23/vht/capturebutton.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23674 2023-03-23 01:55:40.000000 vht-0.3.23/vht/configuration.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2023-03-21 08:04:15.000000 vht-0.3.23/vht/console.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2023-03-21 08:04:15.000000 vht-0.3.23/vht/controllereditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2023-03-21 08:04:15.000000 vht-0.3.23/vht/controllersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5705 2023-03-21 08:04:15.000000 vht-0.3.23/vht/controllersviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2023-03-21 08:04:15.000000 vht-0.3.23/vht/controllerundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2023-03-21 08:04:15.000000 vht-0.3.23/vht/ctrlcfg.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2023-03-21 08:04:15.000000 vht-0.3.23/vht/extras.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2023-03-21 08:04:15.000000 vht-0.3.23/vht/filerotator.py
--rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11440 2023-03-21 08:08:37.000000 vht-0.3.23/vht/main.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18385 2023-03-21 08:04:15.000000 vht-0.3.23/vht/mainwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2023-03-21 08:04:15.000000 vht-0.3.23/vht/mandymenu.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17970 2023-03-21 08:04:15.000000 vht-0.3.23/vht/mandyview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2023-03-21 08:04:15.000000 vht-0.3.23/vht/midimapview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2023-03-21 08:04:15.000000 vht-0.3.23/vht/midimapviewrow.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2023-03-21 08:04:15.000000 vht-0.3.23/vht/notebooklabel.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2023-03-21 12:19:49.000000 vht-0.3.23/vht/poormanspiano.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2023-03-21 08:04:15.000000 vht-0.3.23/vht/portconfig.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2023-03-21 08:04:15.000000 vht-0.3.23/vht/portconfigpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7557 2023-03-21 08:04:15.000000 vht-0.3.23/vht/portconfigview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23391 2023-03-21 08:04:15.000000 vht-0.3.23/vht/preferenceswin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2023-03-21 08:04:15.000000 vht-0.3.23/vht/probeditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2023-03-21 08:04:15.000000 vht-0.3.23/vht/propview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2023-03-21 08:04:15.000000 vht-0.3.23/vht/pulsar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2023-03-21 08:04:15.000000 vht-0.3.23/vht/randomcomposer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7264 2023-03-21 08:04:15.000000 vht-0.3.23/vht/renderer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9217 2023-03-21 08:04:15.000000 vht-0.3.23/vht/renderwin.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2023-03-21 08:04:15.000000 vht-0.3.23/vht/sequencelistview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7775 2023-03-21 12:19:50.000000 vht-0.3.23/vht/sequencelistviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2023-03-21 08:04:15.000000 vht-0.3.23/vht/sequencepropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2023-03-21 12:19:50.000000 vht-0.3.23/vht/sequencetriggersview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37127 2023-03-21 09:35:06.000000 vht-0.3.23/vht/sequenceview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6678 2023-03-21 08:04:15.000000 vht-0.3.23/vht/shortcutmayhem.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19284 2023-03-21 08:04:15.000000 vht-0.3.23/vht/sidetrackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2023-03-31 15:37:39.000000 vht-0.3.23/vht/statusbar.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2023-03-21 08:04:15.000000 vht-0.3.23/vht/thumbmanager.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2023-03-21 08:04:15.000000 vht-0.3.23/vht/timelineview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2023-03-21 08:04:15.000000 vht-0.3.23/vht/timeshifteditor.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2023-03-21 08:04:15.000000 vht-0.3.23/vht/trackpropview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2023-03-21 08:04:15.000000 vht-0.3.23/vht/trackpropviewpopover.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2023-03-21 08:04:15.000000 vht-0.3.23/vht/trackundobuffer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    95800 2023-03-23 02:00:08.000000 vht-0.3.23/vht/trackview.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2023-03-21 08:04:15.000000 vht-0.3.23/vht/trackviewpointer.py
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2023-03-21 08:04:15.000000 vht-0.3.23/vht/velocityeditor.py
-drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-04-25 21:55:30.300751 vht-0.3.23/vht.egg-info/
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-04-25 21:55:30.000000 vht-0.3.23/vht.egg-info/PKG-INFO
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2458 2023-04-25 21:55:30.000000 vht-0.3.23/vht.egg-info/SOURCES.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2023-04-25 21:55:30.000000 vht-0.3.23/vht.egg-info/dependency_links.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2023-04-25 21:55:30.000000 vht-0.3.23/vht.egg-info/entry_points.txt
--rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2023-04-25 21:55:30.000000 vht-0.3.23/vht.egg-info/top_level.txt
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.477701 vht-0.3.32/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    35148 2022-12-31 13:17:54.000000 vht-0.3.32/LICENSE
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       49 2022-12-31 13:17:54.000000 vht-0.3.32/MANIFEST.in
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-05-07 09:57:25.477701 vht-0.3.32/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1255 2023-04-25 21:49:33.000000 vht-0.3.32/README.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.453700 vht-0.3.32/data/
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.453700 vht-0.3.32/data/bank/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2430 2022-12-31 13:17:54.000000 vht-0.3.32/data/bank/10-gm1
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4875 2022-12-31 13:17:54.000000 vht-0.3.32/data/bank/20-gm2
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      290 2022-12-31 13:17:54.000000 vht-0.3.32/data/com.github.rdybka.vht.desktop
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.453700 vht-0.3.32/data/ctrl/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      294 2022-12-31 13:17:54.000000 vht-0.3.32/data/ctrl/10-gm
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      166 2022-12-31 13:17:54.000000 vht-0.3.32/data/ctrl/20-zyn
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4550 2022-12-31 13:17:54.000000 vht-0.3.32/data/mandy.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1246 2022-12-31 13:17:54.000000 vht-0.3.32/data/menu.ui
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11176 2022-12-31 13:17:54.000000 vht-0.3.32/data/vht.png
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4458 2022-12-31 13:17:54.000000 vht-0.3.32/data/vht.svg
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.453700 vht-0.3.32/doc/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2359 2023-05-07 09:52:48.000000 vht-0.3.32/doc/vht.1.gz
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4640 2023-05-07 09:51:47.000000 vht-0.3.32/doc/vht.1.md
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.461700 vht-0.3.32/libvht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       75 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1538 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/ctrlrow.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1416 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/ctrlrow.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7095 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/envelope.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1612 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/envelope.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1960 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/jack_process.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1212 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/jack_process.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19730 2023-01-30 08:50:38.000000 vht-0.3.32/libvht/libcvht.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31881 2023-05-07 09:55:00.000000 vht-0.3.32/libvht/libcvht.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)   477234 2023-05-07 09:55:00.000000 vht-0.3.32/libvht/libcvht_wrap.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8287 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/libvht.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    34606 2023-04-28 01:37:45.000000 vht-0.3.32/libvht/mandy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6088 2023-03-31 14:55:44.000000 vht-0.3.32/libvht/mandy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2354 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/mandy_pix_scan.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1001 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/mandy_pix_scan.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7405 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/mandy_trk_disp.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      986 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/mandy_trk_disp.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    16444 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/midi_client.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4381 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/midi_client.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3496 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/midi_event.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1540 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/midi_event.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15439 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/module.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3151 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/module.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3036 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/row.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1670 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/row.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    28715 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/sequence.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4464 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/sequence.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    29202 2023-03-23 02:07:54.000000 vht-0.3.32/libvht/timeline.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4538 2022-12-31 13:17:54.000000 vht-0.3.32/libvht/timeline.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    41059 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/track.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4153 2023-01-30 08:43:51.000000 vht-0.3.32/libvht/track.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2023-03-21 08:03:40.000000 vht-0.3.32/libvht/tracy.c
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2370 2023-03-20 13:26:10.000000 vht-0.3.32/libvht/tracy.h
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1882 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtcolumn.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2639 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtctrl.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2012 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtctrllist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3639 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtctrlrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtextras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6566 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtmandy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    21012 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtmodule.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3283 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtport.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2404 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtports.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1922 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtquicklist.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5623 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhtrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    10811 2023-03-31 15:37:38.000000 vht-0.3.32/libvht/vhtsequence.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3751 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimeline.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1887 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelinechange.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2204 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelinechanges.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1686 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelineloop.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1913 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelineslices.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5262 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelinestrip.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3637 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelinestrips.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1454 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttimelineticks.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9143 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttrack.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2270 2023-03-21 08:03:58.000000 vht-0.3.32/libvht/vhttracy.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1693 2023-05-07 09:48:35.000000 vht-0.3.32/pyproject.toml
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      108 2023-05-07 09:57:25.477701 vht-0.3.32/setup.cfg
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)     1796 2023-05-07 09:50:58.000000 vht-0.3.32/setup.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.477701 vht-0.3.32/vht/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)      124 2022-12-31 13:17:54.000000 vht-0.3.32/vht/__init__.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1088 2023-03-21 08:04:15.000000 vht-0.3.32/vht/autoexec.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3531 2023-03-21 08:04:15.000000 vht-0.3.32/vht/bankcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1688 2023-03-21 08:04:15.000000 vht-0.3.32/vht/capturebutton.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23674 2023-03-23 01:55:40.000000 vht-0.3.32/vht/configuration.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5836 2023-03-21 08:04:15.000000 vht-0.3.32/vht/console.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    55124 2023-03-21 08:04:15.000000 vht-0.3.32/vht/controllereditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6976 2023-03-21 08:04:15.000000 vht-0.3.32/vht/controllersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     5705 2023-03-21 08:04:15.000000 vht-0.3.32/vht/controllersviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4560 2023-03-21 08:04:15.000000 vht-0.3.32/vht/controllerundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2909 2023-03-21 08:04:15.000000 vht-0.3.32/vht/ctrlcfg.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1910 2023-03-21 08:04:15.000000 vht-0.3.32/vht/extras.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1298 2023-03-21 08:04:15.000000 vht-0.3.32/vht/filerotator.py
+-rwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)    11440 2023-03-21 08:08:37.000000 vht-0.3.32/vht/main.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    18385 2023-03-21 08:04:15.000000 vht-0.3.32/vht/mainwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    14192 2023-03-21 08:04:15.000000 vht-0.3.32/vht/mandymenu.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    17970 2023-03-21 08:04:15.000000 vht-0.3.32/vht/mandyview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2401 2023-03-21 08:04:15.000000 vht-0.3.32/vht/midimapview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4176 2023-03-21 08:04:15.000000 vht-0.3.32/vht/midimapviewrow.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1299 2023-03-21 08:04:15.000000 vht-0.3.32/vht/notebooklabel.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4675 2023-03-21 12:19:49.000000 vht-0.3.32/vht/poormanspiano.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2677 2023-03-21 08:04:15.000000 vht-0.3.32/vht/portconfig.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3547 2023-03-21 08:04:15.000000 vht-0.3.32/vht/portconfigpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7557 2023-03-21 08:04:15.000000 vht-0.3.32/vht/portconfigview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    23391 2023-03-21 08:04:15.000000 vht-0.3.32/vht/preferenceswin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6623 2023-03-21 08:04:15.000000 vht-0.3.32/vht/probeditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     4996 2023-03-21 08:04:15.000000 vht-0.3.32/vht/propview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1035 2023-03-21 08:04:15.000000 vht-0.3.32/vht/pulsar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1100 2023-03-21 08:04:15.000000 vht-0.3.32/vht/randomcomposer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7264 2023-03-21 08:04:15.000000 vht-0.3.32/vht/renderer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9217 2023-03-21 08:04:15.000000 vht-0.3.32/vht/renderwin.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    15715 2023-03-21 08:04:15.000000 vht-0.3.32/vht/sequencelistview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     7775 2023-03-21 12:19:50.000000 vht-0.3.32/vht/sequencelistviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    11262 2023-03-21 08:04:15.000000 vht-0.3.32/vht/sequencepropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    12223 2023-03-21 12:19:50.000000 vht-0.3.32/vht/sequencetriggersview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    37127 2023-03-21 09:35:06.000000 vht-0.3.32/vht/sequenceview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6678 2023-03-21 08:04:15.000000 vht-0.3.32/vht/shortcutmayhem.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19284 2023-03-21 08:04:15.000000 vht-0.3.32/vht/sidetrackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    19612 2023-03-31 15:37:39.000000 vht-0.3.32/vht/statusbar.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2879 2023-03-21 08:04:15.000000 vht-0.3.32/vht/thumbmanager.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    51601 2023-03-21 08:04:15.000000 vht-0.3.32/vht/timelineview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     6308 2023-03-21 08:04:15.000000 vht-0.3.32/vht/timeshifteditor.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    22027 2023-03-21 08:04:15.000000 vht-0.3.32/vht/trackpropview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    31965 2023-03-21 08:04:15.000000 vht-0.3.32/vht/trackpropviewpopover.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     3229 2023-03-21 08:04:15.000000 vht-0.3.32/vht/trackundobuffer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)    95777 2023-05-07 09:38:51.000000 vht-0.3.32/vht/trackview.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     9212 2023-03-21 08:04:15.000000 vht-0.3.32/vht/trackviewpointer.py
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     8127 2023-03-21 08:04:15.000000 vht-0.3.32/vht/velocityeditor.py
+drwxrwxr-x   0 mal1ce    (1000) mal1ce    (1000)        0 2023-05-07 09:57:25.477701 vht-0.3.32/vht.egg-info/
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     1973 2023-05-07 09:57:25.000000 vht-0.3.32/vht.egg-info/PKG-INFO
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)     2458 2023-05-07 09:57:25.000000 vht-0.3.32/vht.egg-info/SOURCES.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)        1 2023-05-07 09:57:25.000000 vht-0.3.32/vht.egg-info/dependency_links.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       37 2023-05-07 09:57:25.000000 vht-0.3.32/vht.egg-info/entry_points.txt
+-rw-rw-r--   0 mal1ce    (1000) mal1ce    (1000)       27 2023-05-07 09:57:25.000000 vht-0.3.32/vht.egg-info/top_level.txt
```

### Comparing `vht-0.3.23/LICENSE` & `vht-0.3.32/LICENSE`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/PKG-INFO` & `vht-0.3.32/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.23
+Version: 0.3.32
 Summary: vahatraker - a live MIDI sequencer for JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `vht-0.3.23/README.md` & `vht-0.3.32/README.md`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/bank/10-gm1` & `vht-0.3.32/data/bank/10-gm1`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/bank/20-gm2` & `vht-0.3.32/data/bank/20-gm2`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/mandy.png` & `vht-0.3.32/data/mandy.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/menu.ui` & `vht-0.3.32/data/menu.ui`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/vht.png` & `vht-0.3.32/data/vht.png`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/data/vht.svg` & `vht-0.3.32/data/vht.svg`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/doc/vht.1.md` & `vht-0.3.32/doc/vht.1.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-% VHT(1) vht 0.3.23
+% VHT(1) vht 0.3.32
 % Remigiusz Dybka
-% April 2022
+% May 2023
 
 # NAME
 **vht** - a minimalistic MIDI sequencer for JACK/GNOME
 
 # SYNOPSIS
 **vht** [file]
```

### Comparing `vht-0.3.23/libvht/ctrlrow.c` & `vht-0.3.32/libvht/ctrlrow.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/ctrlrow.h` & `vht-0.3.32/libvht/ctrlrow.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/envelope.c` & `vht-0.3.32/libvht/envelope.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/envelope.h` & `vht-0.3.32/libvht/envelope.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/jack_process.c` & `vht-0.3.32/libvht/jack_process.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/jack_process.h` & `vht-0.3.32/libvht/jack_process.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/libcvht.h` & `vht-0.3.32/libvht/libcvht.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/libcvht.py` & `vht-0.3.32/libvht/libcvht.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/libcvht_wrap.c` & `vht-0.3.32/libvht/libcvht_wrap.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/libvht.c` & `vht-0.3.32/libvht/libvht.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy.c` & `vht-0.3.32/libvht/mandy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy.h` & `vht-0.3.32/libvht/mandy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy_pix_scan.c` & `vht-0.3.32/libvht/mandy_pix_scan.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy_pix_scan.h` & `vht-0.3.32/libvht/mandy_pix_scan.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy_trk_disp.c` & `vht-0.3.32/libvht/mandy_trk_disp.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/mandy_trk_disp.h` & `vht-0.3.32/libvht/mandy_trk_disp.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/midi_client.c` & `vht-0.3.32/libvht/midi_client.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/midi_client.h` & `vht-0.3.32/libvht/midi_client.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/midi_event.c` & `vht-0.3.32/libvht/midi_event.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/midi_event.h` & `vht-0.3.32/libvht/midi_event.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/module.c` & `vht-0.3.32/libvht/module.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/module.h` & `vht-0.3.32/libvht/module.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/row.c` & `vht-0.3.32/libvht/row.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/row.h` & `vht-0.3.32/libvht/row.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/sequence.c` & `vht-0.3.32/libvht/sequence.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/sequence.h` & `vht-0.3.32/libvht/sequence.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/timeline.c` & `vht-0.3.32/libvht/timeline.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/timeline.h` & `vht-0.3.32/libvht/timeline.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/track.c` & `vht-0.3.32/libvht/track.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/track.h` & `vht-0.3.32/libvht/track.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/tracy.c` & `vht-0.3.32/libvht/tracy.c`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/tracy.h` & `vht-0.3.32/libvht/tracy.h`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtcolumn.py` & `vht-0.3.32/libvht/vhtcolumn.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtctrl.py` & `vht-0.3.32/libvht/vhtctrl.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtctrllist.py` & `vht-0.3.32/libvht/vhtctrllist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtctrlrow.py` & `vht-0.3.32/libvht/vhtctrlrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtextras.py` & `vht-0.3.32/libvht/vhtextras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtmandy.py` & `vht-0.3.32/libvht/vhtmandy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtmodule.py` & `vht-0.3.32/libvht/vhtmodule.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtport.py` & `vht-0.3.32/libvht/vhtport.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtports.py` & `vht-0.3.32/libvht/vhtports.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtquicklist.py` & `vht-0.3.32/libvht/vhtquicklist.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtrow.py` & `vht-0.3.32/libvht/vhtrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhtsequence.py` & `vht-0.3.32/libvht/vhtsequence.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimeline.py` & `vht-0.3.32/libvht/vhttimeline.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelinechange.py` & `vht-0.3.32/libvht/vhttimelinechange.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelinechanges.py` & `vht-0.3.32/libvht/vhttimelinechanges.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelineloop.py` & `vht-0.3.32/libvht/vhttimelineloop.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelineslices.py` & `vht-0.3.32/libvht/vhttimelineslices.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelinestrip.py` & `vht-0.3.32/libvht/vhttimelinestrip.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelinestrips.py` & `vht-0.3.32/libvht/vhttimelinestrips.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttimelineticks.py` & `vht-0.3.32/libvht/vhttimelineticks.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttrack.py` & `vht-0.3.32/libvht/vhttrack.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/libvht/vhttracy.py` & `vht-0.3.32/libvht/vhttracy.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/pyproject.toml` & `vht-0.3.32/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [metadata]
 name = "vht"
-version = "0.3.23"
+version = "0.3.32"
 description = "vahatraker - a live MIDI sequencer for JACK"
 author = "Remigiusz Dybka"
 author_email = "remigiusz.dybka@gmail.com"
 license = "GPLv3+"
 url = "https://github.com/rdybka/vht"
 long_description = "file: README.md"
 long_description_content_type = "text/markdown"
```

### Comparing `vht-0.3.23/setup.py` & `vht-0.3.32/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, Extension
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name = "vht",
-	version = "0.3.23",
+	version = "0.3.32",
 	description = "vahatraker - a live MIDI sequencer for JACK",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	author = "Remigiusz Dybka",
 	author_email = "remigiusz.dybka@gmail.com",
 	url = "https://github.com/rdybka/vht",
 	license = 'GPLv3+',
```

### Comparing `vht-0.3.23/vht/autoexec.py` & `vht-0.3.32/vht/autoexec.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/bankcfg.py` & `vht-0.3.32/vht/bankcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/capturebutton.py` & `vht-0.3.32/vht/capturebutton.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/configuration.py` & `vht-0.3.32/vht/configuration.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/console.py` & `vht-0.3.32/vht/console.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/controllereditor.py` & `vht-0.3.32/vht/controllereditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/controllersview.py` & `vht-0.3.32/vht/controllersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/controllersviewrow.py` & `vht-0.3.32/vht/controllersviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/controllerundobuffer.py` & `vht-0.3.32/vht/controllerundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/ctrlcfg.py` & `vht-0.3.32/vht/ctrlcfg.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/extras.py` & `vht-0.3.32/vht/extras.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/filerotator.py` & `vht-0.3.32/vht/filerotator.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/main.py` & `vht-0.3.32/vht/main.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/mainwin.py` & `vht-0.3.32/vht/mainwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/mandymenu.py` & `vht-0.3.32/vht/mandymenu.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/mandyview.py` & `vht-0.3.32/vht/mandyview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/midimapview.py` & `vht-0.3.32/vht/midimapview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/midimapviewrow.py` & `vht-0.3.32/vht/midimapviewrow.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/notebooklabel.py` & `vht-0.3.32/vht/notebooklabel.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/poormanspiano.py` & `vht-0.3.32/vht/poormanspiano.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/portconfig.py` & `vht-0.3.32/vht/portconfig.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/portconfigpopover.py` & `vht-0.3.32/vht/portconfigpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/portconfigview.py` & `vht-0.3.32/vht/portconfigview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/preferenceswin.py` & `vht-0.3.32/vht/preferenceswin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/probeditor.py` & `vht-0.3.32/vht/probeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/propview.py` & `vht-0.3.32/vht/propview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/pulsar.py` & `vht-0.3.32/vht/pulsar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/randomcomposer.py` & `vht-0.3.32/vht/randomcomposer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/renderer.py` & `vht-0.3.32/vht/renderer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/renderwin.py` & `vht-0.3.32/vht/renderwin.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sequencelistview.py` & `vht-0.3.32/vht/sequencelistview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sequencelistviewpopover.py` & `vht-0.3.32/vht/sequencelistviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sequencepropviewpopover.py` & `vht-0.3.32/vht/sequencepropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sequencetriggersview.py` & `vht-0.3.32/vht/sequencetriggersview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sequenceview.py` & `vht-0.3.32/vht/sequenceview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/shortcutmayhem.py` & `vht-0.3.32/vht/shortcutmayhem.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/sidetrackview.py` & `vht-0.3.32/vht/sidetrackview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/statusbar.py` & `vht-0.3.32/vht/statusbar.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/thumbmanager.py` & `vht-0.3.32/vht/thumbmanager.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/timelineview.py` & `vht-0.3.32/vht/timelineview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/timeshifteditor.py` & `vht-0.3.32/vht/timeshifteditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/trackpropview.py` & `vht-0.3.32/vht/trackpropview.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/trackpropviewpopover.py` & `vht-0.3.32/vht/trackpropviewpopover.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/trackundobuffer.py` & `vht-0.3.32/vht/trackundobuffer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/trackview.py` & `vht-0.3.32/vht/trackview.py`

 * *Files 0% similar despite different names*

```diff
@@ -2033,16 +2033,14 @@
 
             if event.state & Gdk.ModifierType.CONTROL_MASK:
                 ctrl = True
 
             if event.state & Gdk.ModifierType.MOD1_MASK:
                 alt = True
 
-        shift = False
-
         if cfg.key["exit_edit"].matches(event):
             self.leave_all()
             return True
 
         if self.velocity_editor:
             self.velocity_editor.on_key_press(widget, event)
```

### Comparing `vht-0.3.23/vht/trackviewpointer.py` & `vht-0.3.32/vht/trackviewpointer.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht/velocityeditor.py` & `vht-0.3.32/vht/velocityeditor.py`

 * *Files identical despite different names*

### Comparing `vht-0.3.23/vht.egg-info/PKG-INFO` & `vht-0.3.32/vht.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vht
-Version: 0.3.23
+Version: 0.3.32
 Summary: vahatraker - a live MIDI sequencer for JACK
 Home-page: https://github.com/rdybka/vht
 Author: Remigiusz Dybka
 Author-email: remigiusz.dybka@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: GTK
```

### Comparing `vht-0.3.23/vht.egg-info/SOURCES.txt` & `vht-0.3.32/vht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

