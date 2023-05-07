# Comparing `tmp/tahoma-2.2.5.tar.gz` & `tmp/tahoma-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahoma-2.2.5.tar", last modified: Thu May  4 12:16:30 2023, max compression
+gzip compressed data, was "tahoma-2.2.6.tar", last modified: Sun May  7 16:50:58 2023, max compression
```

## Comparing `tahoma-2.2.5.tar` & `tahoma-2.2.6.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.318843 tahoma-2.2.5/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.5/LICENSE
--rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.5/MANIFEST.in
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6416 2023-05-04 12:16:30.319178 tahoma-2.2.5/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5754 2023-05-04 11:36:22.000000 tahoma-2.2.5/PYPI_README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5753 2023-05-04 11:36:20.000000 tahoma-2.2.5/README.md
--rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.5/pyproject.toml
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.5/requirements.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-04 12:16:30.320181 tahoma-2.2.5/setup.cfg
--rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.5/setup.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.309385 tahoma-2.2.5/tahoma/
--rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.5/tahoma/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-04 12:16:06.000000 tahoma-2.2.5/tahoma/__version__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)     5469 2023-04-05 15:40:09.000000 tahoma-2.2.5/tahoma/get_devices_url.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.315569 tahoma-2.2.5/tahoma/icons/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.5/tahoma/icons/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.5/tahoma/icons/connected_house.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.5/tahoma/icons/water heater.png
--rwxrwx---   0 neptune   (1000) neptune   (1000)      668 2023-02-21 09:02:06.000000 tahoma-2.2.5/tahoma/install_tahoma.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)    36253 2023-05-04 11:44:29.000000 tahoma-2.2.5/tahoma/tahoma.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.316598 tahoma-2.2.5/tahoma/temp/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.5/tahoma/temp/__init__.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.318192 tahoma-2.2.5/tahoma/test/
--rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.5/tahoma/test/__init__.py
--rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.5/tahoma/test/test.py
-drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-04 12:16:30.313018 tahoma-2.2.5/tahoma.egg-info/
--rwxrwx---   0 neptune   (1000) neptune   (1000)     6416 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/PKG-INFO
--rwxrwx---   0 neptune   (1000) neptune   (1000)      542 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/SOURCES.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/dependency_links.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/entry_points.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/requires.txt
--rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-04 12:16:30.000000 tahoma-2.2.5/tahoma.egg-info/top_level.txt
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.616933 tahoma-2.2.6/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1070 2023-02-18 00:22:37.000000 tahoma-2.2.6/LICENSE
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      142 2023-02-21 14:35:21.000000 tahoma-2.2.6/MANIFEST.in
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6437 2023-05-07 16:50:58.617046 tahoma-2.2.6/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5775 2023-05-07 16:40:31.000000 tahoma-2.2.6/PYPI_README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     5753 2023-05-04 11:36:20.000000 tahoma-2.2.6/README.md
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     1201 2023-02-21 21:29:00.000000 tahoma-2.2.6/pyproject.toml
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-02-21 17:24:01.000000 tahoma-2.2.6/requirements.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       38 2023-05-07 16:50:58.617379 tahoma-2.2.6/setup.cfg
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      125 2023-02-15 20:31:23.000000 tahoma-2.2.6/setup.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.611462 tahoma-2.2.6/tahoma/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      134 2023-02-21 18:24:33.000000 tahoma-2.2.6/tahoma/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       22 2023-05-07 16:41:10.000000 tahoma-2.2.6/tahoma/__version__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6121 2023-05-07 16:43:55.000000 tahoma-2.2.6/tahoma/get_devices_url.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.615305 tahoma-2.2.6/tahoma/icons/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.6/tahoma/icons/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    21160 2023-02-15 08:39:56.000000 tahoma-2.2.6/tahoma/icons/connected_house.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    29722 2023-02-15 17:48:11.000000 tahoma-2.2.6/tahoma/icons/water heater.png
+-rwxrwx---   0 neptune   (1000) neptune   (1000)    38624 2023-05-07 16:50:10.000000 tahoma-2.2.6/tahoma/tahoma.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.615824 tahoma-2.2.6/tahoma/temp/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:32:54.000000 tahoma-2.2.6/tahoma/temp/__init__.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.616627 tahoma-2.2.6/tahoma/test/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        5 2023-02-18 00:33:06.000000 tahoma-2.2.6/tahoma/test/__init__.py
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       23 2021-07-13 15:25:04.000000 tahoma-2.2.6/tahoma/test/test.py
+drwxrwx---   0 neptune   (1000) neptune   (1000)        0 2023-05-07 16:50:58.613891 tahoma-2.2.6/tahoma.egg-info/
+-rwxrwx---   0 neptune   (1000) neptune   (1000)     6437 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/PKG-INFO
+-rwxrwx---   0 neptune   (1000) neptune   (1000)      517 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/SOURCES.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        1 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/dependency_links.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       46 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/entry_points.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)       41 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/requires.txt
+-rwxrwx---   0 neptune   (1000) neptune   (1000)        7 2023-05-07 16:50:58.000000 tahoma-2.2.6/tahoma.egg-info/top_level.txt
```

### Comparing `tahoma-2.2.5/LICENSE` & `tahoma-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.5/PKG-INFO` & `tahoma-2.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.5
+Version: 2.2.6
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -110,15 +110,15 @@
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
+For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -180,15 +180,15 @@
 
 
 By doing this, instead of taping `python3 '/place/of/the/folder/tahoma/tahoma.py open shutter kitchen'`,
 
  you will be able to directly tape in the terminal : `tahoma open shutter kitchen`.
 
 
-Then execute tahoma just like this : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office` and that's all !
+Then execute tahoma just like this : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning` and that's all !
 
 
 
 
 
 
 For :
```

### Comparing `tahoma-2.2.5/PYPI_README.md` & `tahoma-2.2.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
 For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
 
-
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
 - `tahoma --list-actions` or `tahoma -la`
```

### Comparing `tahoma-2.2.5/README.md` & `tahoma-2.2.6/PYPI_README.md`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,16 @@
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
+For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
+
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
 Open a terminal and type :
@@ -164,15 +165,15 @@
 
 
 By doing this, instead of taping `python3 '/place/of/the/folder/tahoma/tahoma.py open shutter kitchen'`,
 
  you will be able to directly tape in the terminal : `tahoma open shutter kitchen`.
 
 
-Then execute tahoma just like this : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office` and that's all !
+Then execute tahoma just like this : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning` and that's all !
 
 
 
 
 
 
 For :
```

### Comparing `tahoma-2.2.5/pyproject.toml` & `tahoma-2.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.5/tahoma/get_devices_url.py` & `tahoma-2.2.6/tahoma/get_devices_url.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,25 +11,27 @@
 import re
 from getpass import getpass
 import time
 from pyoverkiz.const import SUPPORTED_SERVERS
 from pyoverkiz.client import OverkizClient
 from pyoverkiz.enums import OverkizCommand
 from pyoverkiz.models import Command
+from pyoverkiz.models import Scenario
 
 async def main() -> None:
 
     passwd_file = os.path.dirname(os.path.abspath(__file__))+'/temp/identifier_file.txt'
     list_of_tahoma_devices = os.path.dirname(os.path.abspath(__file__))+'/temp/list_of_tahoma_devices.txt'
     list_of_tahoma_shutters = os.path.dirname(os.path.abspath(__file__))+'/temp/shutters.txt'
     list_of_tahoma_heaters = os.path.dirname(os.path.abspath(__file__))+'/temp/heaters.txt'
     list_of_tahoma_alarms = os.path.dirname(os.path.abspath(__file__))+'/temp/alarms.txt'
     list_of_tahoma_spotalarms = os.path.dirname(os.path.abspath(__file__))+'/temp/spotalarms.txt'
     list_of_tahoma_plugs = os.path.dirname(os.path.abspath(__file__))+'/temp/plugs.txt'
     list_of_tahoma_sunscreens = os.path.dirname(os.path.abspath(__file__))+'/temp/sunscreens.txt'
+    list_of_tahoma_scenes = os.path.dirname(os.path.abspath(__file__))+'/temp/scenarios.txt'
 
     server_choosen =  os.path.dirname(os.path.abspath(__file__))+'/temp/server_choosen.txt'
 
     try :
         f = open(server_choosen, 'r')
         serverchoice = f.read()
         f.close()
@@ -39,14 +41,15 @@
     f2 = open(list_of_tahoma_devices, 'w')
     f3 = open(list_of_tahoma_shutters, 'w')
     f4 = open(list_of_tahoma_heaters, 'w')
     f5 = open(list_of_tahoma_alarms, 'w')
     f6 = open(list_of_tahoma_spotalarms, 'w')
     f7 = open(list_of_tahoma_plugs, 'w')
     f8 = open(list_of_tahoma_sunscreens, 'w')
+    f9 = open(list_of_tahoma_scenes, 'w')
 
     parser = argparse.ArgumentParser()
     parser.add_argument("-u", "--username")
     parser.add_argument("-p", "--password")
     parser.add_argument("-g", action='store_true') #store_true for not asking argument
     parser.add_argument("--getlist", action='store_true') #store_true for not asking argument
     args = parser.parse_args()
@@ -71,48 +74,60 @@
     async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
         try:
             await client.login()
         except Exception as exception:  # pylint: disable=broad-except
             print(exception)
             return
         devices = await client.get_devices()
+        scenarios = await client.get_scenarios()
     try :
+        f2.write(f"Devices :\n")
         for device in devices:
             print(f"\n{device.label},{device.id},{device.widget}")
             f2.write(f"{device.label},{device.id},{device.widget},{device.ui_class},{device.controllable_name}\n")
             if "Shutter" in device.widget or "PositionableTiltedScreen" in device.widget:
                 f3.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_shutters)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_shutters)
             elif "Heater" in device.widget :
                 f4.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_heaters)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_heaters)
             elif "MyFoxAlarm" in device.widget :
                 f5.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_alarms)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_alarms)
             elif "StatefulOnOffLight" in device.widget :
                 f6.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_spotalarms)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_spotalarms)
             elif "StatelessOnOff" in device.widget :
                 f7.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_plugs)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_plugs)
             elif "PositionableScreen" in device.widget or "PositionableHorizontalAwning" in device.widget:
                 f8.write(device.label+","+device.id+","+device.widget+"\n")
-                print( "Device "+device.label+" controled by tahoma. Added to "+list_of_tahoma_sunscreens)
+                print( "Device "+device.label+" controled by tahoma. Added to : "+list_of_tahoma_sunscreens)
             else :
                 print( "Device '"+device.label+"' NOT controlled by tahoma yet")
     except Exception as e :
         print(e)
-    
+    print("\nScenes :\n")
+    try :
+        f2.write(f"\nScenes :\n")
+        for scenario in scenarios:
+            f2.write(f"{scenario.label},{scenario.oid}\n")
+            f9.write(f"{scenario.label},{scenario.oid}\n")
+            print( 'Scene : "'+scenario.label+'" controled by tahoma. Added to : '+list_of_tahoma_scenes)
+    except Exception as e :
+        print(e)
+
     f2.close()
     f3.close()
     f4.close()
     f5.close()
     f6.close()
     f7.close()
     f8.close()
+    f9.close()
     
     print( "\nIf you want to add a device you have found in this list but which is not controlled by tahoma yet, please provide info about this device from this file at \nhttps://github.com/pzim-devdata/tahoma/issues and I will update the plugin ;-).")
     print( "\nThe list of devices has been succesfully imported to the file : "+list_of_tahoma_devices+"\n" )
 
 try:
     asyncio.run(main())
     exit(0)
```

### Comparing `tahoma-2.2.5/tahoma/icons/connected_house.png` & `tahoma-2.2.6/tahoma/icons/connected_house.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.5/tahoma/icons/water heater.png` & `tahoma-2.2.6/tahoma/icons/water heater.png`

 * *Files identical despite different names*

### Comparing `tahoma-2.2.5/tahoma/tahoma.py` & `tahoma-2.2.6/tahoma/tahoma.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import re
 from getpass import getpass
 import time
 from pyoverkiz.const import SUPPORTED_SERVERS
 from pyoverkiz.client import OverkizClient
 from pyoverkiz.enums import OverkizCommand
 from pyoverkiz.models import Command
+from pyoverkiz.models import Scenario
 from tahoma import __version__
 
 
 def main():
     version ='tahoma - Version '+ str(__version__.__version__)+' - by @pzim-devdata'
 
     icon_app = os.path.dirname(os.path.abspath(__file__))+'/icons/connected_house.png'
@@ -33,23 +34,24 @@
     list_of_tahoma_devices = os.path.dirname(os.path.abspath(__file__))+'/temp/list_of_tahoma_devices.txt'
     list_of_tahoma_shutters = os.path.dirname(os.path.abspath(__file__))+'/temp/shutters.txt'
     list_of_tahoma_heaters = os.path.dirname(os.path.abspath(__file__))+'/temp/heaters.txt'
     list_of_tahoma_alarms = os.path.dirname(os.path.abspath(__file__))+'/temp/alarms.txt'
     list_of_tahoma_spotalarms = os.path.dirname(os.path.abspath(__file__))+'/temp/spotalarms.txt'
     list_of_tahoma_plugs = os.path.dirname(os.path.abspath(__file__))+'/temp/plugs.txt'
     list_of_tahoma_sunscreens = os.path.dirname(os.path.abspath(__file__))+'/temp/sunscreens.txt'
+    list_of_tahoma_scenes = os.path.dirname(os.path.abspath(__file__))+'/temp/scenarios.txt'
 
     notification_consent = os.path.dirname(os.path.abspath(__file__))+'/temp/consent_notification.txt'
 
     server_choosen =  os.path.dirname(os.path.abspath(__file__))+'/temp/server_choosen.txt'
 
-    list_categories = ['shutter','spotalarm','plug','alarm','heater','sunscreen']
-    list_categories_french = ['volet','spotalarme','prise','alarme','chauffage','rideau']
-    list_actions = ['[open,close,stop,my,NUMBER]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my,NUMBER]']
-    list_actions_french = ['[ouvrir,fermer,stop,my,NOMBRE]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my,NOMBRE]']
+    list_categories = ['shutter','spotalarm','plug','alarm','heater','sunscreen','scene']
+    list_categories_french = ['volet','spotalarme','prise','alarme','chauffage','rideau','scenario']
+    list_actions = ['[open,close,stop,my,NUMBER]','[on,off]','[on,off]','[arm,disarm,partial,arm_night,arm_away]','[comfort,comfort-1,comfort-2,eco,off]','[open,close,stop,my,NUMBER]','[on,activate,launch,execute]']
+    list_actions_french = ['[ouvrir,fermer,stop,my,NOMBRE]','[allumer,eteindre]','[allumer,eteindre]','[activer,desactiver,partiel,activer_nuit,activer_parti]','[confort,confort-1,confort-2,eco,eteindre]','[ouvrir,fermer,stop,my,NOMBRE]','[lancer,activer,executer]']
 
     try :
         f = open(notification_consent, 'r')
         notification = f.read()
         f.close()
     except FileNotFoundError:
         notification = 'n'
@@ -151,15 +153,15 @@
 
     for arg in sys.argv :
         if arg == '-i' or arg == '--info' :
             info()
             exit()
 
     for arg in sys.argv :
-        if arg == '-c' or arg == '--configure' :
+        if arg == '-c' or arg == '--configure' or arg == '--config' :
             print("Do you want to show desktop notifications ? (Only for Linux users) (Y/n)")
             notification = input()
             if notification.lower() == 'y'or notification.lower() == 'yes':
                 f = open(notification_consent, 'w')
                 f.write('Yes')
                 f.close()
             else :
@@ -552,27 +554,67 @@
                 fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['off'])
             else :
                 print( "\n'"+action+"'"+" is not a valide action.\n")
                 print("Please provide one of this argument as action : [comfort comfort-1 comfort-2 eco off]")
                 exit()
             str1 = " "
             print("Output action : "+remove_accent(action).lower()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
+
+        ##########################SCENES
+
+        elif remove_accent(category) == 'scene' or remove_accent(category) == 'scenario':
+            f = open(list_of_tahoma_scenes, 'r')
+            content = f.read()
+            f.close()
+            try:
+                master_list = content.split("\n")
+                master_list.remove('')
+            except ValueError:
+                print("\nDid you downloaded the list of Tahoma's scenes ?.\nExecute tahoma --getlist \nFor more info execute tahoma -h or tahoma --info")
+                exit()
+            for i in master_list :
+                bad_name.append(i.split(",")[0])
+                if remove_accent(i.split(",")[0]) in remove_accent(str(name)) or remove_accent(str(name)) in remove_accent(i.split(",")[0]) :
+                     url.append(i.split(",")[1])
+                     too_many_urls.append(i.split(",")[0])
+                     good_name.append(i.split(",")[0])
+            if len(url)== 0 :
+                print("There is no match. The <NAME> you gave is not exact. Did you mean : "+str(bad_name)+" ? Choose a UNIQUE part of word from this results as <NAME> argument\nIf you don't find your device in this results try tahoma --getlist\nSee tahoma --list-names for help.")
+                exit()
+            if len(url) > 1 :
+                print("There is more than one match. The <NAME> you gave is not exact. Choose a UNIQUE part of word from this results as <NAME> argument : "+str(too_many_urls)+"\nSee tahoma --list-names for help.")
+                exit()
+
             
+            #fonction = Command(OverkizCommand.SET_HEATING_LEVEL,['comfort'])
+            #exec_id = await client.execute_scenario(device_url)
+
+            str1 = " "
+            print("Output action : "+remove_accent(action).lower()+" "+remove_accent(category)+" "+str1.join(good_name)+ " \nwith url : "+str1.join(url))
+
+        ##########################
+
         else :
             print( "\nThe <CATEGORY> you have entered doesn't exist.\nChoose one of this category : "+str(list_categories)+"\nUse tahoma --help-categories or tahoma --list-categories for info")
 
+
     ##########################MAIN FUNCTION
 
         try:
             async def main() -> None:
                 async with OverkizClient(USERNAME, PASSWORD, SUPPORTED_SERVERS[serverchoice]) as client:
                     await client.login()
                     try :
                         for device_url in url :
-                            exec_id = await client.execute_command( device_url, fonction )
+                            try :
+                                exec_id = await client.execute_command( device_url, fonction )
+                            except : pass
+                            try :
+                                exec_id = await client.execute_scenario(device_url)
+                            except : pass
                     except Exception as e:
                         print(e) 
                         try:
                             if notification.lower() == 'y'or notification.lower() == 'yes':
                                 os.system("notify-send -i "+icon_app+" -t 150000 Tahoma "+"'Program failed. Here is the error message :\n\n "+str(e)+"'")
                         except:pass
                         exit()
```

### Comparing `tahoma-2.2.5/tahoma.egg-info/PKG-INFO` & `tahoma-2.2.6/tahoma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahoma
-Version: 2.2.5
+Version: 2.2.6
 Summary: This is a very easy API for controlling Somfy Tahoma's devices written in Python3, thanks to the pyoverkiz API. You just need a three-word input to control a device
 Author-email: Pzim-devdata <contact@pzim.fr>
 Project-URL: Homepage, https://github.com/pzim-devdata/tahoma
 Project-URL: Bug Tracker, https://github.com/pzim-devdata/tahoma/issues
 Keywords: tahoma,somfy,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -110,15 +110,15 @@
 
 For instance : `tahoma open shutter kitchen` or `tahoma ouvrir volet cuisine`
 
 You can also close a shutter or a sunscreen to a specific level. For example, to close to 25%, you can use the commands : `tahoma 25 shutter kitchen` or `tahoma 25 sunscreen kitchen`. Please note that this feature only works with IO protocols and not with RTS.
 
 You can also run many commands during the same process without restarting tahoma ;
 
-For instance : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office 25 sunscreen kitchen`
+For instance : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning`
 
 
 # But first you need to retrieve your PERSONALS commands :
 
 
 ## Get a list of all possibles [ACTIONS] for each [CATEGORIES] : 
 
@@ -180,15 +180,15 @@
 
 
 By doing this, instead of taping `python3 '/place/of/the/folder/tahoma/tahoma.py open shutter kitchen'`,
 
  you will be able to directly tape in the terminal : `tahoma open shutter kitchen`.
 
 
-Then execute tahoma just like this : `tahoma arm alarm garden open shutter kitchen close shutter room6 confort heater dining off plug office` and that's all !
+Then execute tahoma just like this : `tahoma arm alarm garden close shutter room6 confort heater dining off plug office 25 sunscreen kitchen launch scene morning` and that's all !
 
 
 
 
 
 
 For :
```

