# Comparing `tmp/spotcrates-0.6.2.tar.gz` & `tmp/spotcrates-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotcrates-0.6.2.tar", max compression
+gzip compressed data, was "spotcrates-0.6.3.tar", max compression
```

## Comparing `spotcrates-0.6.2.tar` & `spotcrates-0.6.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2022-12-15 22:50:22.212154 spotcrates-0.6.2/LICENSE
--rw-r--r--   0        0        0    11842 2023-03-22 02:23:26.155732 spotcrates-0.6.2/README.md
--rw-r--r--   0        0        0      792 2023-05-06 22:13:03.687615 spotcrates-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-04 22:49:46.694616 spotcrates-0.6.2/spotcrates/__init__.py
--rw-r--r--   0        0        0     9579 2023-03-22 02:53:53.625880 spotcrates-0.6.2/spotcrates/cli.py
--rw-r--r--   0        0        0     2601 2023-05-06 22:08:20.007380 spotcrates-0.6.2/spotcrates/common.py
--rw-r--r--   0        0        0     9738 2023-03-20 16:44:29.264590 spotcrates-0.6.2/spotcrates/filters.py
--rw-r--r--   0        0        0    16392 2023-03-20 21:08:56.572940 spotcrates-0.6.2/spotcrates/playlists.py
--rw-r--r--   0        0        0      401 2022-12-15 22:03:25.519119 spotcrates-0.6.2/spotcrates/templates/auth_index.html
--rw-r--r--   0        0        0      173 2022-12-15 22:03:25.523119 spotcrates-0.6.2/spotcrates/templates/base.html
--rw-r--r--   0        0        0      150 2022-12-15 22:03:25.523119 spotcrates-0.6.2/spotcrates/templates/index.html
--rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 spotcrates-0.6.2/setup.py
--rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 spotcrates-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-12-15 22:50:22.212154 spotcrates-0.6.3/LICENSE
+-rw-r--r--   0        0        0    11842 2023-03-22 02:23:26.155732 spotcrates-0.6.3/README.md
+-rw-r--r--   0        0        0      792 2023-05-07 03:32:40.794955 spotcrates-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-04 22:49:46.694616 spotcrates-0.6.3/spotcrates/__init__.py
+-rw-r--r--   0        0        0     9738 2023-05-06 22:40:36.400846 spotcrates-0.6.3/spotcrates/cli.py
+-rw-r--r--   0        0        0     2601 2023-05-06 22:08:20.007380 spotcrates-0.6.3/spotcrates/common.py
+-rw-r--r--   0        0        0     9738 2023-03-20 16:44:29.264590 spotcrates-0.6.3/spotcrates/filters.py
+-rw-r--r--   0        0        0    16392 2023-03-20 21:08:56.572940 spotcrates-0.6.3/spotcrates/playlists.py
+-rw-r--r--   0        0        0      401 2022-12-15 22:03:25.519119 spotcrates-0.6.3/spotcrates/templates/auth_index.html
+-rw-r--r--   0        0        0      173 2022-12-15 22:03:25.523119 spotcrates-0.6.3/spotcrates/templates/base.html
+-rw-r--r--   0        0        0      150 2022-12-15 22:03:25.523119 spotcrates-0.6.3/spotcrates/templates/index.html
+-rw-r--r--   0        0        0    13098 1970-01-01 00:00:00.000000 spotcrates-0.6.3/setup.py
+-rw-r--r--   0        0        0    12594 1970-01-01 00:00:00.000000 spotcrates-0.6.3/PKG-INFO
```

### Comparing `spotcrates-0.6.2/LICENSE` & `spotcrates-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.2/README.md` & `spotcrates-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.2/pyproject.toml` & `spotcrates-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spotcrates"
-version = "0.6.2"
+version = "0.6.3"
 description = ""
 authors = ["Chris Mayes <cmayes@cmay.es>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jinja2 = "^3.1.2"
```

### Comparing `spotcrates-0.6.2/spotcrates/cli.py` & `spotcrates-0.6.3/spotcrates/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 import tomli_w
 
 from spotcrates.common import BaseLookup, truncate_long_value
 from spotcrates.filters import FieldName
 
 import tomli
 
+import importlib.metadata
+
+__version__ = importlib.metadata.version('spotcrates')
+
 __author__ = "cmayes"
 
 from pathlib import Path
 
 import spotipy
 
 from spotcrates.playlists import Playlists, PlaylistResult
@@ -225,14 +229,15 @@
     parser = argparse.ArgumentParser()
     parser.add_argument("-c", "--config_file",
                         help=f"The location of the config file (default: {DEFAULT_CONFIG_FILE})",
                         default=DEFAULT_CONFIG_FILE, type=Path)
     parser.add_argument("-s", "--sort_fields", help="The fields to sort against, applied in order")
     parser.add_argument("-f", "--filters", help="Filters to apply to the list")
     parser.add_argument("-r", "--randomize", help="Randomize the target list", action='store_true')
+    parser.add_argument('--version', action='version', version=__version__)
     parser.add_argument("-t", "--target",
                         help="Specify the target name of the operation (overrides any default value)")
     parser.add_argument("command", metavar="COMMAND",
                         help=f"The command to run (one of {','.join(COMMANDS)})")
     parser.add_argument("arguments", metavar='ARGUMENTS', nargs='*',
                         help="the arguments to the command")
     args = None
```

### Comparing `spotcrates-0.6.2/spotcrates/common.py` & `spotcrates-0.6.3/spotcrates/common.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.2/spotcrates/filters.py` & `spotcrates-0.6.3/spotcrates/filters.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.2/spotcrates/playlists.py` & `spotcrates-0.6.3/spotcrates/playlists.py`

 * *Files identical despite different names*

### Comparing `spotcrates-0.6.2/setup.py` & `spotcrates-0.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'types-appdirs>=1.4.3.5,<2.0.0.0']
 
 entry_points = \
 {'console_scripts': ['spotcrates = spotcrates.cli:main']}
 
 setup_kwargs = {
     'name': 'spotcrates',
-    'version': '0.6.2',
+    'version': '0.6.3',
     'description': '',
     'long_description': '# Spotcrates\n## A set of tools for finding and managing music on Spotify\n\n![Code Coverage](https://img.shields.io/endpoint?url=https://gist.githubusercontent.com/cmayes/3c8214e2bd942821496440b93acd3582/raw/covbadge.json)\n\n# Installation\n\n## Requirements\n\nSpotcrates requires [Python](https://www.python.org/) 10 or newer. You will also need a Spotify account.\n\n## Install from PyPI\n\n```shell\npip install spotcrates\n```\n\n## Configuration\n\nSpotcrates will need, at minimum, credentials for accessing your Spotify account. You may also specify\nplaylists to subscribe to, among other settings.\n\n### Initial Configuration File\n\nSpotcrates can create an initial configuration file for itself. It will write to the specified configuration file\nlocation, i.e. what you configure with `-c` or `--config_file`. If you don\'t specify anything, Spotcrates will use\na platform-specific configuration file location, e.g. `/home/$USER/.config/spotcrates/spotcrates_config.toml` \non Linux. The output of `spotcrates -h` includes the default location for your configuration file.\n\n```shell\nspotcrates init-config\n```\n\n### Spotify API Credentials\n\nThis bit is not terribly user-friendly as it\'s assumed that developers will be the ones creating these credentials.\nSince this app runs as a script on your own machine, you\'ll need to create your own credentials. You will need\na `Client ID` and a `Client Secret`. The process is a little involved, and the \n[Spotify docs on the subject](https://developer.spotify.com/documentation/general/guides/authorization/app-settings/) \nare a bit opaque for the casual user (as I very recently was). These pages do a pretty good job describing \nthe process:\n\n- https://support.heateor.com/get-spotify-client-id-client-secret/\n- https://cran.r-project.org/web/packages/spotidy/vignettes/Connecting-with-the-Spotify-API.html\n\nNote that these projects are mainly interested in extracting data for their respective applications, so the \ninstructions are geared to that end.\n\nOnce you have your client ID and client secret, paste them into your Spotcrates configuration file in the `[spotify]`\nsection:\n\n```toml\n[spotify]\nclient_id = "(your ID here)"\nclient_secret = "(your secret here)"\n```\n\n#### Testing Your Credentials\n\nSpotcrates will request and cache authorization info the first time you use your Spotify credentials. The cache location\nis platform-specific. On Linux, it\'s usually at `/home/$USER/.cache/spotcrates/spotcrates_auth_cache`.\n\nTo trigger this step, you can try listing your playlists:\n\n`spotcrates list-playlists`\n\nSpotcrates will initiate an authorization process with Spotify via your default browser. If the authorization\nsucceeds, the browser tab will close itself, and your playlists will be listed on the command line.\n\n### Customizable Settings for Spotify\n\nThese settings can be changed from their defaults, though you won\'t usually need to do so. They are defined\nunder the `[spotify]` config file heading.\n\n- `auth_cache`: The location of the Spotify authorization cache. This defaults to your platform\'s default cache\n    location base, plus `spotcrates/spotcrates_auth_cache`.\n- `auth_scopes`: A list of authorization scopes that Spotcrates requests. The default scopes are\n    `["playlist-modify-private", "playlist-read-private"]`.\n\n## Playlists\n\nThese settings control playlist-related commands like [daily](#daily) or [randomize](#randomize). They\ncan be customized under the [playlists] heading in the configuration file.\n\n- `daily_mix_target`: The name of the playlist to target, which is created if it does not exist. Defaults to "Now."\n- `daily_mix_prefix`: The prefix of the "Daily Mix" playlists to be aggregated. Defaults to "Daily Mix."\n- `daily_mix_excludes`: The prefix of the playlists that contain tracks to exclude. Defaults to "Overplayed."\n\n## Subscriptions\n\nThese settings are for the [subscriptions](#subscriptions) command. They can be configured under the `[subscriptions]` \nconfiguration file heading. \n\n- `subscriptions_target`: The name of the playlists where the new subscriptions will be appended. Created if \n    the playlist does not exist. Defaults to `NewSubscriptions`.\n- `max_age`: The maximum age of a track in a playlist for it to be considered "new." Values can be English\n    expressions like `2 weeks` or `96 hours`. Defaults to `3 days`.\n\n### Subscription Playlists\n\nThese are the playlist groups used by [subscriptions](#subscriptions) and related commands. All groups are included\nby default. The values are the "spotify IDs" listed in the [list-playlists](#list-playlists) command. These playlist \ngroups are configured under the [subscriptions.playlists] section of the configuration file.\n\n\n```toml\n[subscriptions.playlists]\n# IRL ANGEL, Twin Peaks Vibes, Folk Fabrique,\n# FADO PORTUGAL, While You Work\nquiet = ["37i9dQZF1DX7Ocjwy96xTX", "38rrtWgflrw7grB37aMlsO", "37i9dQZF1DX62XscWX9t6h",\n"67waO0NR8HTySxtB7wfMBZ", "6bUIofrj5PWNIeb67DbUqf"]\n# Japanese Shoegaze, Modern Psychedelia, Adrenaline Coding\nnoisy = ["2uiYiQFpynkWCpIXcBGir9", "37i9dQZF1DX8gDIpdqp1XJ", "3JEvwuKbVKoggEA75gWqET"]\n# State of Jazz, Jazz-Funk, Jazz Funk (Instrumental),\n# Jazz Funk & Groove\njazz = ["37i9dQZF1DX7YCknf2jT6s", "37i9dQZF1DWUb0uBnlJuTi", "4xRrCdkn4r5lrDOElek5oC",\n"2puFFdGTID0iJdQtjLvhal"]\n```\n\n# Commands\n\nThe installation script puts the command `spotcrates` in your Python environment\n(e.g. `/.pyenv/shims/spotcrates`). The command `spotcrates commands` lists all of the \ncommands available along with a short description of each.\n\nNote that Spotcrates will accept the shortest unique command substring, so for example you can run\n`spotcrates sub` for the `subscriptions` command.\n\n## daily\n`spotcrates daily` collects the contents of the "Daily Mix" playlists, filters them \nagainst an exclusion list ("Overplayed" by default), and adds them to the end of \na target list ("Now" by default).\n\n## subscriptions\n`spotcrates subscriptions` adds new tracks from configured playlists to the target playlist, \nfiltering for excluded entries. Three days is the default maximum age for a track to be \nconsidered "new."\n\n## list-playlists\n`spotcrates list-playlists` lists playlists\' name, owner, track count, and description.\nThe command accepts `-f` for filter expressions and `-s` for sort expressions. (TODO: \nadd description of filter and search expressions and link to it here)\n\n### Search Patterns\n\nThe command `list-playlists` accepts search filters passed via the `-f` option. Multiple\nfilter expressions are separated by commas.\n\n#### Search Examples\n\n`spotcrates li -f jazz`\n\nList playlists where any field contains the string "jazz" (case-insensitive)\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nAcid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets\nJazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          \nAcid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          \nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nInstrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nJazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          \nFaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma\n```\n\n`spotcrates li -f o:spotify,n:rise`\n\nList playlists where the owner contains `spotify` and name contains `rise`.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nRise                             230   37i9dQZF1DWUOhRIDwDB7M   spotify          Positive and uplifting ambient instrumental tracks.\n```\n\n`spotcrates li -f n:ends:villains`\n\nList playlists where name ends with `villains`.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nclassical music for villains     66    0zkl7eKzuUit1QRPVKtga2   225uye2hek5id23t \n```\n\n#### Search Fields\n\nThe default search field is `all`.\n\n- spotify_id\n- playlist_name\n- size\n- owner\n- playlist_description\n- all: Search any/all of the above fields.\n\n#### Search Types\n\nThe default search type is `contains`.\n\n- contains\n- equals\n- starts\n- ends\n- greater\n- less\n- greater_equal\n- less_equal\n\n### Sort Patterns\n\nThe command `list-playlists` accepts sort filters passed via the `-s` option. Multiple\nsort expressions are separated by commas.\n\n#### Sort Examples\n\n`spotcrates li -f n:jazz -s name`\n\nName contains `jazz`; sort by name ascending.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nAcid Jazz                        90    37i9dQZF1DWXHghfFFOaS6   spotify          Where hip-hop and soul meets jazz. Cover: Digable Planets\nAcid Jazz                        3     1h6rEPX9qRpBCBbjuAysMz   cmayes3          \nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nInstrumental Acid Jazz Mix       50    37i9dQZF1EIgnEnn8SKPjM   spotify          Instrumental Acid Jazz music picked just for you\nJazz                             1     6VH2cw8n115fbQ7Ls2wzdR   cmayes3          \nJazz Funk                        6     61Q9DgzF3f1ULr3i1uRyUy   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\n```\n\n`spotcrates li -f jazz,size:ge:100 -s size:desc`\n\nAny field contains `jazz`; size is greater than or equal to 100, sort by size descending.\n\n```\nPLAYLIST NAME                    SIZE  ID                       OWNER            DESCRIPTION\nFaLaLaLaLa GREAT BIG Christmas V 4051  6A2Kj9cWUpuu0UcEbWVf5E   kingofjingaling  Over 170 hours of classic Christmas music. The focus is on classic Christma\nGeneral Jazz                     513   1j6ndSnyYn6oUlnwpGiRWc   cmayes3          \nJazz Funk (Instrumental)         272   4xRrCdkn4r5lrDOElek5oC   1226030890       \nJazz-Funk                        200   37i9dQZF1DWUb0uBnlJuTi   spotify          Jazz. But funky. Cover: Takuya Kuroda\nJazz Piano Classics              100   37i9dQZF1DX5q7wCXFrkHh   spotify          The classic piano recordings in Jazz. Cover: Oscar Peterson\nState of Jazz                    100   37i9dQZF1DX7YCknf2jT6s   spotify          New jazz for open minds. Cover: Walter Smith III\n```\n\n#### Sort Types\n\nThe default sort type is `ascending`, i.e. a-z.\n\n- ascending\n- descending\n\n## randomize\n`spotcrates randomize (playlist1) (playlist2)...` randomizes the playlists with the given names, \nIDs, or in the given collections. \n\n## copy\n`spotcrates copy (source) (dest)` copies a playlist into a new playlist. You may optionally specify \na destination playlist name; the default is to name the destination based on the source name with\nthe general form `f"{source_name}-{count:02d}"`.\n\n## commands\n`spotcrates commands` displays a summary of the available commands.',
     'author': 'Chris Mayes',
     'author_email': 'cmayes@cmay.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spotcrates-0.6.2/PKG-INFO` & `spotcrates-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotcrates
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 Author: Chris Mayes
 Author-email: cmayes@cmay.es
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

