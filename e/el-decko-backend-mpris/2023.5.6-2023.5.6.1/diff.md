# Comparing `tmp/el_decko_backend_mpris-2023.5.6.tar.gz` & `tmp/el_decko_backend_mpris-2023.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "el_decko_backend_mpris-2023.5.6.tar", last modified: Sat May  6 21:02:10 2023, max compression
+gzip compressed data, was "el_decko_backend_mpris-2023.5.6.1.tar", last modified: Sat May  6 21:58:37 2023, max compression
```

## Comparing `el_decko_backend_mpris-2023.5.6.tar` & `el_decko_backend_mpris-2023.5.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:02:10.827598 el_decko_backend_mpris-2023.5.6/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-05-06 18:26:55.000000 el_decko_backend_mpris-2023.5.6/LICENSE
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2153 2023-05-06 21:02:10.827598 el_decko_backend_mpris-2023.5.6/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1654 2023-05-06 20:52:40.000000 el_decko_backend_mpris-2023.5.6/README.md
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      972 2023-05-06 20:45:05.000000 el_decko_backend_mpris-2023.5.6/pyproject.toml
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-06 21:02:10.827598 el_decko_backend_mpris-2023.5.6/setup.cfg
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:02:10.823598 el_decko_backend_mpris-2023.5.6/src/
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:02:10.827598 el_decko_backend_mpris-2023.5.6/src/edb_mpris/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     6116 2023-05-06 20:51:47.000000 el_decko_backend_mpris-2023.5.6/src/edb_mpris/__init__.py
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1755 2023-05-06 20:05:23.000000 el_decko_backend_mpris-2023.5.6/src/edb_mpris/event.py
-drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:02:10.827598 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2153 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/PKG-INFO
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      383 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/SOURCES.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/dependency_links.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      142 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/entry_points.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       47 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/requires.txt
--rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       10 2023-05-06 21:02:10.000000 el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/top_level.txt
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)    35149 2023-05-06 18:26:55.000000 el_decko_backend_mpris-2023.5.6.1/LICENSE
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2131 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1630 2023-05-06 21:40:05.000000 el_decko_backend_mpris-2023.5.6.1/README.md
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      929 2023-05-06 21:39:46.000000 el_decko_backend_mpris-2023.5.6.1/pyproject.toml
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       38 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/setup.cfg
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/src/
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/src/edb_mpris/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     6821 2023-05-06 21:52:32.000000 el_decko_backend_mpris-2023.5.6.1/src/edb_mpris/__init__.py
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     1755 2023-05-06 20:05:23.000000 el_decko_backend_mpris-2023.5.6.1/src/edb_mpris/event.py
+drwxr-xr-x   0 vortexacherontic  (1000) vortexacherontic  (1000)        0 2023-05-06 21:58:37.617135 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)     2131 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/PKG-INFO
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      383 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/SOURCES.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)        1 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/dependency_links.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)      142 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/entry_points.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       25 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/requires.txt
+-rw-r--r--   0 vortexacherontic  (1000) vortexacherontic  (1000)       10 2023-05-06 21:58:37.000000 el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/top_level.txt
```

### Comparing `el_decko_backend_mpris-2023.5.6/LICENSE` & `el_decko_backend_mpris-2023.5.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `el_decko_backend_mpris-2023.5.6/PKG-INFO` & `el_decko_backend_mpris-2023.5.6.1/src/el_decko_backend_mpris.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: el_decko_backend_mpris
-Version: 2023.5.6
+Name: el-decko-backend-mpris
+Version: 2023.5.6.1
 Summary: El Decko backend to control MPRIS2 compatible media players
 Author-email: Imo 'Vortex Acherontic' Hester <vortex@z-ray.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_backend_mpris
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_backend_mpris/issues
 Platform: Linux
 Requires-Python: >=3.8
@@ -65,9 +65,8 @@
 ### Python
 Python >= 3.8  
 pympris
 dbus-python  
 cmake  
 dbus-1-devel  
 glib2-devel  
-python3**-devel  
-python3**-gobject-Gdk
+python3**-devel
```

### Comparing `el_decko_backend_mpris-2023.5.6/README.md` & `el_decko_backend_mpris-2023.5.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -52,9 +52,8 @@
 ### Python
 Python >= 3.8  
 pympris
 dbus-python  
 cmake  
 dbus-1-devel  
 glib2-devel  
-python3**-devel  
-python3**-gobject-Gdk
+python3**-devel
```

### Comparing `el_decko_backend_mpris-2023.5.6/pyproject.toml` & `el_decko_backend_mpris-2023.5.6.1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 dynamic = ["version"]
 readme = "README.md"
 description = "El Decko backend to control MPRIS2 compatible media players"
 license = { text = "GPL-3" }
 requires-python = ">=3.8"
 dependencies = [
     "pympris",
-    "PyGObject",
-    "pycairo",
-    "pgi",
     "dbus-python>=1.0"
 ]
 
 [project.entry-points."eldecko.backend"]
 init = "edb_mpris:edb_init"
 stop = "edb_mpris:edb_stop"
 fire = "edb_mpris:edb_fire_event"
```

### Comparing `el_decko_backend_mpris-2023.5.6/src/edb_mpris/__init__.py` & `el_decko_backend_mpris-2023.5.6.1/src/edb_mpris/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pympris
 import dbus
 from dbus.mainloop.glib import DBusGMainLoop
+from pympris import PyMPRISException
 
 from edb_mpris.event import EventType
 
-VERSION = "2023.5.6"
+VERSION = "2023.5.6.1"
 dbus_loop = DBusGMainLoop()
 bus = dbus.SessionBus(mainloop=dbus_loop)
 player_volumes = []
 
 
 def edb_init():
     pass
@@ -30,17 +31,19 @@
 def __make_request(event_type: EventType, player_ids, event_parameters: dict = None):
     player_name = ""
     if event_parameters and "player" in event_parameters:
         player_name = event_parameters["player"]
 
     match event_type:
         case EventType.MUTE.value:
-            pass
+            __unmute(player_ids, player_name)
         case EventType.UNMUTE.value:
-            pass
+            __mute(player_ids, player_name)
+        case EventType.TOGGLE_MUTE.value:
+            __toggle_mute(player_ids, player_name)
         case EventType.PREV.value:
             __prev(player_ids, player_name)
         case EventType.NEXT.value:
             __next(player_ids, player_name)
         case EventType.PAUSE.value:
             __pause(player_ids, player_name)
         case EventType.PLAY.value:
@@ -117,50 +120,59 @@
         for player in player_ids:
             media_player = pympris.MediaPlayer(player, bus)
             if media_player.player.CanGoPrevious:
                 media_player.player.Previous()
 
 
 def __mute(player_ids, player_name):
-    if player_name != "":
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            if player_name.lower() in str(media_player.root.Identity).lower():
+    try:
+        if player_name != "":
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
+                if player_name.lower() in str(media_player.root.Identity).lower():
+                    player_volumes[media_player.root.Identity] = media_player.player.Volume
+                    media_player.player.Volume = 0
+        else:
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
                 player_volumes[media_player.root.Identity] = media_player.player.Volume
                 media_player.player.Volume = 0
-    else:
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            player_volumes[media_player.root.Identity] = media_player.player.Volume
-            media_player.player.Volume = 0
+    except PyMPRISException:
+        print("WARN: Player " + player_name + " does not support interface Volume!")
 
 
 def __unmute(player_ids, player_name):
-    if player_name != "":
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            if player_name.lower() in str(media_player.root.Identity).lower():
+    try:
+        if player_name != "":
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
+                if player_name.lower() in str(media_player.root.Identity).lower():
+                    media_player.player.Volume = player_volumes[media_player.root.Identity]
+        else:
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
                 media_player.player.Volume = player_volumes[media_player.root.Identity]
-    else:
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            media_player.player.Volume = player_volumes[media_player.root.Identity]
+    except PyMPRISException:
+        print("WARN: Player " + player_name + " does not support interface Volume!")
 
 
 def __toggle_mute(player_ids, player_name):
-    if player_name != "":
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            if player_name.lower() in str(media_player.root.Identity).lower():
+    try:
+        if player_name != "":
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
+                if player_name.lower() in str(media_player.root.Identity).lower():
+                    if media_player.player.Volume == 0:
+                        media_player.player.Volume = player_volumes[media_player.root.Identity]
+                    else:
+                        player_volumes[media_player.root.Identity] = media_player.player.Volume
+                        media_player.player.Volume = 0
+        else:
+            for player in player_ids:
+                media_player = pympris.MediaPlayer(player, bus)
                 if media_player.player.Volume == 0:
                     media_player.player.Volume = player_volumes[media_player.root.Identity]
                 else:
                     player_volumes[media_player.root.Identity] = media_player.player.Volume
                     media_player.player.Volume = 0
-    else:
-        for player in player_ids:
-            media_player = pympris.MediaPlayer(player, bus)
-            if media_player.player.Volume == 0:
-                media_player.player.Volume = player_volumes[media_player.root.Identity]
-            else:
-                player_volumes[media_player.root.Identity] = media_player.player.Volume
-                media_player.player.Volume = 0
+    except PyMPRISException:
+        print("WARN: Player " + player_name + " does not support interface Volume!")
```

### Comparing `el_decko_backend_mpris-2023.5.6/src/edb_mpris/event.py` & `el_decko_backend_mpris-2023.5.6.1/src/edb_mpris/event.py`

 * *Files identical despite different names*

### Comparing `el_decko_backend_mpris-2023.5.6/src/el_decko_backend_mpris.egg-info/PKG-INFO` & `el_decko_backend_mpris-2023.5.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: el-decko-backend-mpris
-Version: 2023.5.6
+Name: el_decko_backend_mpris
+Version: 2023.5.6.1
 Summary: El Decko backend to control MPRIS2 compatible media players
 Author-email: Imo 'Vortex Acherontic' Hester <vortex@z-ray.de>
 License: GPL-3
 Project-URL: Homepage, https://github.com/Z-Ray-Entertainment/el_decko_backend_mpris
 Project-URL: Bug Tracker, https://github.com/Z-Ray-Entertainment/el_decko_backend_mpris/issues
 Platform: Linux
 Requires-Python: >=3.8
@@ -65,9 +65,8 @@
 ### Python
 Python >= 3.8  
 pympris
 dbus-python  
 cmake  
 dbus-1-devel  
 glib2-devel  
-python3**-devel  
-python3**-gobject-Gdk
+python3**-devel
```

