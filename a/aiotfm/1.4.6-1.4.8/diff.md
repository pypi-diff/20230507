# Comparing `tmp/aiotfm-1.4.6.tar.gz` & `tmp/aiotfm-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiotfm-1.4.6.tar", last modified: Wed Jul 13 19:12:09 2022, max compression
+gzip compressed data, was "dist/aiotfm-1.4.8.tar", last modified: Sun May  7 19:36:41 2023, max compression
```

## Comparing `aiotfm-1.4.6.tar` & `aiotfm-1.4.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:12:09.000000 aiotfm-1.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      572 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-07-13 19:11:35.000000 aiotfm-1.4.6/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-07-13 19:11:35.000000 aiotfm-1.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-13 19:11:35.000000 aiotfm-1.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4695 2022-07-13 19:12:09.000000 aiotfm-1.4.6/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm/
--rw-r--r--   0 runner    (1001) docker     (121)    12735 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/shop.py
--rw-r--r--   0 runner    (1001) docker     (121)      643 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/packet.py
--rw-r--r--   0 runner    (1001) docker     (121)    12823 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/inventory.py
--rw-r--r--   0 runner    (1001) docker     (121)     5298 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/tribe.py
--rw-r--r--   0 runner    (1001) docker     (121)     7461 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/player.py
--rw-r--r--   0 runner    (1001) docker     (121)    48498 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4983 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/friend.py
--rw-r--r--   0 runner    (1001) docker     (121)     2061 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     4212 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     7597 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/room.py
--rw-r--r--   0 runner    (1001) docker     (121)     3647 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-13 19:12:09.000000 aiotfm-1.4.6/aiotfm/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2934 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/utils/locale.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/utils/shakikoo.py
--rw-r--r--   0 runner    (1001) docker     (121)      655 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (121)     2817 2022-07-13 19:11:35.000000 aiotfm-1.4.6/aiotfm/utils/get_keys.py
--rw-r--r--   0 runner    (1001) docker     (121)      133 2022-07-13 19:12:09.000000 aiotfm-1.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-07-13 19:11:35.000000 aiotfm-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:36:41.000000 aiotfm-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-07 19:36:27.000000 aiotfm-1.4.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-07 19:36:41.000000 aiotfm-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-07 19:36:27.000000 aiotfm-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:36:41.000000 aiotfm-1.4.8/aiotfm/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48498 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2061 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/friend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12823 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12735 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/shop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/tribe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:36:41.000000 aiotfm-1.4.8/aiotfm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/utils/get_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/utils/locale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-07 19:36:27.000000 aiotfm-1.4.8/aiotfm/utils/shakikoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 19:36:41.000000 aiotfm-1.4.8/aiotfm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-05-07 19:36:40.000000 aiotfm-1.4.8/aiotfm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-07 19:36:40.000000 aiotfm-1.4.8/aiotfm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 19:36:40.000000 aiotfm-1.4.8/aiotfm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-07 19:36:40.000000 aiotfm-1.4.8/aiotfm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 19:36:40.000000 aiotfm-1.4.8/aiotfm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-07 19:36:27.000000 aiotfm-1.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-07 19:36:41.000000 aiotfm-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-07 19:36:27.000000 aiotfm-1.4.8/setup.py
```

### Comparing `aiotfm-1.4.6/aiotfm.egg-info/SOURCES.txt` & `aiotfm-1.4.8/aiotfm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm.egg-info/PKG-INFO` & `aiotfm-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotfm
-Version: 1.4.6
+Version: 1.4.8
 Summary: An asynchronous event based client for Transformice.
 Home-page: https://github.com/Athesdrake/aiotfm
 Author: Athesdrake
 License: UNKNOWN
 Description: # aiotfm
         
         aiotfm is an asynchronous Client implementation of [Transformice](https://www.transformice.com/) that allows developers to make bots easily.
```

### Comparing `aiotfm-1.4.6/README.md` & `aiotfm-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/PKG-INFO` & `aiotfm-1.4.8/aiotfm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotfm
-Version: 1.4.6
+Version: 1.4.8
 Summary: An asynchronous event based client for Transformice.
 Home-page: https://github.com/Athesdrake/aiotfm
 Author: Athesdrake
 License: UNKNOWN
 Description: # aiotfm
         
         aiotfm is an asynchronous Client implementation of [Transformice](https://www.transformice.com/) that allows developers to make bots easily.
```

### Comparing `aiotfm-1.4.6/aiotfm/shop.py` & `aiotfm-1.4.8/aiotfm/shop.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/__init__.py` & `aiotfm-1.4.8/aiotfm/__init__.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/packet.py` & `aiotfm-1.4.8/aiotfm/packet.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/inventory.py` & `aiotfm-1.4.8/aiotfm/inventory.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/tribe.py` & `aiotfm-1.4.8/aiotfm/tribe.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/player.py` & `aiotfm-1.4.8/aiotfm/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -185,27 +185,29 @@
 		All badges unlocked by the player and their number.
 	stats: `Stats`
 		The player's stats.
 	equippedOrb: `int`
 		The equipped orb of the player.
 	orbs: `set`
 		The list of unlocked orbs.
+	isOnline: `bool`
+		Whether or not the player is online. See [#31](https://github.com/Athesdrake/aiotfm/pull/31#issuecomment-1537433271).
 	adventurePoints: `int`
 		Number of adventure points the player has.
 	"""
 	def __init__(self, packet: Packet):
 		self.username = packet.readUTF()
 		self.id = packet.read32()
 
 		self.registration_date = packet.read32()
 		self.privLevel = packet.read8()
 		self.gender = packet.read8()
 		self.tribe = packet.readUTF() or None
 		self.soulmate = packet.readUTF() or None
-		stats = [packet.read32() for i in range(7)]
+		stats = [packet.read32() for i in range(10)]
 		self.title = packet.read16()
 
 		self.titles = set()
 		self.titles_stars = {}
 		for _ in range(packet.read16()):
 			title_id, stars = packet.read16(), packet.read8()
 			self.titles.add(title_id)
@@ -226,15 +228,15 @@
 		self.stats = Stats(stats, modeStats)
 
 		self.equippedOrb = packet.read8()
 		self.orbs = set()
 		for _ in range(packet.read8()):
 			self.orbs.add(packet.read8())
 
-		packet.readBool()
+		self.isOnline = packet.readBool()
 		self.adventurePoints = packet.read32()
 
 
 class Stats:
 	"""Represents the statistics of a player.
 
 	Attributes
@@ -252,18 +254,27 @@
 	gatheredCheese: `int`
 		Total number of gathered cheese.
 	bootcamps: `int`
 		Number of bootcamp.
 	modeStats: `list`
 		A list of tuples that represents the stats in different mode.
 		(id, progress, progressLimit, imageId)
+	noSkillNormalModeSaves: `int`
+		Number of shaman saves in normal mode without skills.
+	noSkillHardModeSaves: `int`
+		Number of shaman saves in hard mode without skills.
+	noSkillDivineModeSaves: `int`
+		Number of shaman saves in divine mode without skills.
 	"""
 	def __init__(self, stats, modeStats):
 		self.normalModeSaves = stats[0]
 		self.hardModeSaves = stats[4]
 		self.divineModeSaves = stats[6]
 		self.shamanCheese = stats[1]
 		self.firsts = stats[2]
 		self.gatheredCheese = stats[3]
 		self.bootcamps = stats[5]
+		self.noSkillNormalModeSaves = stats[7]
+		self.noSkillHardModeSaves = stats[8]
+		self.noSkillDivineModeSaves = stats[9]
 
 		self.modeStats = modeStats # id, progress, progressLimit, imageId
```

### Comparing `aiotfm-1.4.6/aiotfm/client.py` & `aiotfm-1.4.8/aiotfm/client.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/errors.py` & `aiotfm-1.4.8/aiotfm/errors.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/__version__.py` & `aiotfm-1.4.8/aiotfm/__version__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'aiotfm'
 __description__ = "An asynchronous event based client for Transformice."
 __url__ = 'https://github.com/Athesdrake/aiotfm'
 
-__version__ = '1.4.6'
+__version__ = '1.4.8'
 __author__ = 'Athesdrake'
 __credits__ = [
 	'Tocutoeltuco', 'https://github.com/Tocutoeltuco/transfromage',
 	'Lautenschlager-id', 'https://github.com/Lautenschlager-id/Transfromage'
 ]
 
 __license__ = """MIT License
```

### Comparing `aiotfm-1.4.6/aiotfm/friend.py` & `aiotfm-1.4.8/aiotfm/friend.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/enums.py` & `aiotfm-1.4.8/aiotfm/enums.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/message.py` & `aiotfm-1.4.8/aiotfm/message.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/room.py` & `aiotfm-1.4.8/aiotfm/room.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/connection.py` & `aiotfm-1.4.8/aiotfm/connection.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/utils/locale.py` & `aiotfm-1.4.8/aiotfm/utils/locale.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 	Attributes
 	----------
 	locales: :class:`dict`[:class:`aiotfm.locale.Locale`]
 		Cached locales.
 	locale: :class:`str`
 		The locale name.
 	"""
-	BASE_URL = 'http://transformice.com/langues/tfz_{}'
+	BASE_URL = 'http://transformice.com/langues/tfm-{}.gz'
 
 	def __init__(self, locale='en'):
 		self._locale = locale
 		self.locales = {}
 
 	def __getitem__(self, key):
 		"""Return the translation of a key.
```

### Comparing `aiotfm-1.4.6/aiotfm/utils/shakikoo.py` & `aiotfm-1.4.8/aiotfm/utils/shakikoo.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/utils/date.py` & `aiotfm-1.4.8/aiotfm/utils/date.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/aiotfm/utils/get_keys.py` & `aiotfm-1.4.8/aiotfm/utils/get_keys.py`

 * *Files identical despite different names*

### Comparing `aiotfm-1.4.6/setup.py` & `aiotfm-1.4.8/setup.py`

 * *Files identical despite different names*

