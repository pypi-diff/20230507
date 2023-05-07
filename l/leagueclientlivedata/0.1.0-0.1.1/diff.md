# Comparing `tmp/leagueclientlivedata-0.1.0.tar.gz` & `tmp/leagueclientlivedata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "leagueclientlivedata-0.1.0.tar", max compression
+gzip compressed data, was "leagueclientlivedata-0.1.1.tar", max compression
```

## Comparing `leagueclientlivedata-0.1.0.tar` & `leagueclientlivedata-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-04-22 12:23:51.085286 leagueclientlivedata-0.1.0/league_client_live_data/__init__.py
--rw-r--r--   0        0        0      194 2023-04-20 18:27:25.791715 leagueclientlivedata-0.1.0/league_client_live_data/config.py
--rw-r--r--   0        0        0       72 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.0/league_client_live_data/config.yaml
--rw-r--r--   0        0        0        0 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/__init__.py
--rw-r--r--   0        0        0      625 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/abilities.py
--rw-r--r--   0        0        0      414 2023-04-22 12:26:05.824869 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/all_game_data.py
--rw-r--r--   0        0        0      974 2023-04-20 18:27:25.793712 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/champion_stata.py
--rw-r--r--   0        0        0     1169 2023-04-20 18:27:25.793712 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/event.py
--rw-r--r--   0        0        0      272 2023-04-20 18:27:25.793712 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/game_data.py
--rw-r--r--   0        0        0     1551 2023-04-22 12:26:58.406265 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/player.py
--rw-r--r--   0        0        0      798 2023-04-20 18:27:25.794710 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/runes.py
--rw-r--r--   0        0        0      419 2023-04-20 18:27:25.794710 leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/summoner_spell.py
--rw-r--r--   0        0        0     5382 2023-04-22 12:29:33.117154 leagueclientlivedata-0.1.0/league_client_live_data/live_client_data.py
--rw-r--r--   0        0        0      510 2023-04-22 12:26:38.402289 leagueclientlivedata-0.1.0/league_client_live_data/utils.py
--rw-r--r--   0        0        0    35823 2023-04-20 18:25:08.094413 leagueclientlivedata-0.1.0/LICENSE
--rw-r--r--   0        0        0      548 2023-04-22 12:39:04.408623 leagueclientlivedata-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1129 2023-04-20 22:15:14.200678 leagueclientlivedata-0.1.0/README.md
--rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 leagueclientlivedata-0.1.0/setup.py
--rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 leagueclientlivedata-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-22 12:23:51.085286 leagueclientlivedata-0.1.1/league_client_live_data/__init__.py
+-rw-r--r--   0        0        0      194 2023-04-20 18:27:25.791715 leagueclientlivedata-0.1.1/league_client_live_data/config.py
+-rw-r--r--   0        0        0       72 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.1/league_client_live_data/config.yaml
+-rw-r--r--   0        0        0        0 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/__init__.py
+-rw-r--r--   0        0        0      625 2023-04-20 18:27:25.792713 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/abilities.py
+-rw-r--r--   0        0        0      414 2023-04-22 12:26:05.824869 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/all_game_data.py
+-rw-r--r--   0        0        0      974 2023-04-20 18:27:25.793712 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/champion_stata.py
+-rw-r--r--   0        0        0     1200 2023-05-06 16:42:38.975582 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/event.py
+-rw-r--r--   0        0        0      272 2023-04-20 18:27:25.793712 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/game_data.py
+-rw-r--r--   0        0        0     1551 2023-04-22 12:26:58.406265 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/player.py
+-rw-r--r--   0        0        0      798 2023-04-20 18:27:25.794710 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/runes.py
+-rw-r--r--   0        0        0      419 2023-04-20 18:27:25.794710 leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/summoner_spell.py
+-rw-r--r--   0        0        0     5382 2023-04-22 12:29:33.117154 leagueclientlivedata-0.1.1/league_client_live_data/live_client_data.py
+-rw-r--r--   0        0        0      510 2023-04-22 12:26:38.402289 leagueclientlivedata-0.1.1/league_client_live_data/utils.py
+-rw-r--r--   0        0        0    35823 2023-04-20 18:25:08.094413 leagueclientlivedata-0.1.1/LICENSE
+-rw-r--r--   0        0        0      548 2023-05-07 15:04:36.647740 leagueclientlivedata-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1129 2023-04-20 22:15:14.200678 leagueclientlivedata-0.1.1/README.md
+-rw-r--r--   0        0        0     1983 1970-01-01 00:00:00.000000 leagueclientlivedata-0.1.1/setup.py
+-rw-r--r--   0        0        0     1725 1970-01-01 00:00:00.000000 leagueclientlivedata-0.1.1/PKG-INFO
```

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/abilities.py` & `leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/abilities.py`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/champion_stata.py` & `leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/champion_stata.py`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/event.py` & `leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/event.py`

 * *Files 23% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Assisters: Optional[List[str]]
     KillerName: Optional[str]
     InhibKilled: Optional[str]
     TurretKilled: Optional[str]
     Stolen: Optional[bool]
     AcingTeam: Optional[str]
     Acer: Optional[str]
+    VictimName: Optional[str]
     InhibRespawningSoon: Optional[str]
 
 
 class Events(BaseModel):
     """
     Represents a list of game events
     """
```

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/player.py` & `leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/player.py`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/endpoint_data/runes.py` & `leagueclientlivedata-0.1.1/league_client_live_data/endpoint_data/runes.py`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/league_client_live_data/live_client_data.py` & `leagueclientlivedata-0.1.1/league_client_live_data/live_client_data.py`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/LICENSE` & `leagueclientlivedata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/pyproject.toml` & `leagueclientlivedata-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "leagueclientlivedata"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["Lukas Mahr <lukas@yousuckatprogramming.de>"]
 readme = "README.md"
 packages = [{ include = "league_client_live_data" }]
 exclude = ["*.pem", "*.db"]
```

### Comparing `leagueclientlivedata-0.1.0/README.md` & `leagueclientlivedata-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `leagueclientlivedata-0.1.0/setup.py` & `leagueclientlivedata-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'pylint>=2.17.2,<3.0.0',
  'pyyaml>=6.0,<7.0',
  'ruff>=0.0.262,<0.0.263',
  'types-pyyaml>=6.0.12.9,<7.0.0.0']
 
 setup_kwargs = {
     'name': 'leagueclientlivedata',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# League Client Live Data Api\nAn async api wrapper for the [game client api](https://developer.riotgames.com/docs/lol#game-client-api) from league of legends.\nFor every endpoint there is a pydantic BaseModel that represents the data from the response of the request. \n# Setup\n## Installation\n\n```bash\ngit clone https://github.com/Plutokekz/LeagueClientLiveDataApi.git\npoetry install\n```\n## Usage\nGet the events from your current game\n````python\nfrom pathlib import Path\n\nfrom live_client_data import LeagueClientLiveDataApi\n\n\nif __name__ == "__main__":\n    config_file = Path("config.yaml")\n    api = LeagueClientLiveDataApi()\n    async def main():\n        while True:\n            data = await api.event_data()\n            print(data)\n    api.loop.run_until_complete(main())\n````\n## Config\n\nthe config file contains currently 2 entries on for the api endpoint and one for the \nssl certificate of riot games. You can download the file from [here](https://developer.riotgames.com/docs/lol#game-client-api). \n\n````yaml\ncert_file: "riotgames.pem"\nurl: "https://127.0.0.1:2999/liveclientdata"\n````\n',
     'author': 'Lukas Mahr',
     'author_email': 'lukas@yousuckatprogramming.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `leagueclientlivedata-0.1.0/PKG-INFO` & `leagueclientlivedata-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: leagueclientlivedata
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Lukas Mahr
 Author-email: lukas@yousuckatprogramming.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: black (>=23.3.0,<24.0.0)
```

