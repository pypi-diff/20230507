# Comparing `tmp/valo_api_official-1.0.0.tar.gz` & `tmp/valo_api_official-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api_official-1.0.0.tar", max compression
+gzip compressed data, was "valo_api_official-1.0.1.tar", max compression
```

## Comparing `valo_api_official-1.0.0.tar` & `valo_api_official-1.0.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0     1083 2023-01-05 23:57:21.847830 valo_api_official-1.0.0/LICENSE
--rw-r--r--   0        0        0     2420 2023-01-05 23:57:21.847830 valo_api_official-1.0.0/README.md
--rw-r--r--   0        0        0     2794 2023-01-05 23:57:21.847830 valo_api_official-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      228 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/__init__.py
--rw-r--r--   0        0        0      577 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/config.py
--rw-r--r--   0        0        0     1302 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/__init__.py
--rw-r--r--   0        0        0     3577 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/account.py
--rw-r--r--   0        0        0     1889 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/active_shards.py
--rw-r--r--   0        0        0     1866 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/content.py
--rw-r--r--   0        0        0     3128 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/leaderboard.py
--rw-r--r--   0        0        0     2371 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/match_details.py
--rw-r--r--   0        0        0     2310 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/match_history.py
--rw-r--r--   0        0        0     2573 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/recent_matches.py
--rw-r--r--   0        0        0     1992 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints/status.py
--rw-r--r--   0        0        0     1878 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/exceptions/__init__.py
--rw-r--r--   0        0        0      448 2023-01-05 23:57:21.867830 valo_api_official-1.0.0/valo_api_official/exceptions/rate_limit.py
--rw-r--r--   0        0        0     1685 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/__init__.py
--rw-r--r--   0        0        0      104 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/account.py
--rw-r--r--   0        0        0      109 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/active_shards.py
--rw-r--r--   0        0        0      823 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/content.py
--rw-r--r--   0        0        0      251 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/error_response.py
--rw-r--r--   0        0        0      689 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/leaderboard.py
--rw-r--r--   0        0        0     2861 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/match_details.py
--rw-r--r--   0        0        0      216 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/match_history.py
--rw-r--r--   0        0        0      130 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/recent_matches.py
--rw-r--r--   0        0        0      827 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/responses/status.py
--rw-r--r--   0        0        0        0 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/utils/__init__.py
--rw-r--r--   0        0        0     2237 2023-01-05 23:57:21.871830 valo_api_official-1.0.0/valo_api_official/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3287 1970-01-01 00:00:00.000000 valo_api_official-1.0.0/setup.py
--rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 valo_api_official-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-05-07 09:45:16.001202 valo_api_official-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2420 2023-05-07 09:45:16.001202 valo_api_official-1.0.1/README.md
+-rw-r--r--   0        0        0     2795 2023-05-07 09:45:16.005202 valo_api_official-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      228 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/config.py
+-rw-r--r--   0        0        0     1302 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/__init__.py
+-rw-r--r--   0        0        0     3577 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/account.py
+-rw-r--r--   0        0        0     1889 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/active_shards.py
+-rw-r--r--   0        0        0     1866 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/content.py
+-rw-r--r--   0        0        0     3128 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/leaderboard.py
+-rw-r--r--   0        0        0     2371 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/match_details.py
+-rw-r--r--   0        0        0     2310 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/match_history.py
+-rw-r--r--   0        0        0     2573 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/recent_matches.py
+-rw-r--r--   0        0        0     1992 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints/status.py
+-rw-r--r--   0        0        0     1878 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/exceptions/__init__.py
+-rw-r--r--   0        0        0      448 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     1685 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/account.py
+-rw-r--r--   0        0        0      109 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/active_shards.py
+-rw-r--r--   0        0        0      823 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/content.py
+-rw-r--r--   0        0        0      251 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/error_response.py
+-rw-r--r--   0        0        0      689 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/leaderboard.py
+-rw-r--r--   0        0        0     2950 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/match_details.py
+-rw-r--r--   0        0        0      216 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/match_history.py
+-rw-r--r--   0        0        0      130 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/recent_matches.py
+-rw-r--r--   0        0        0      827 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/responses/status.py
+-rw-r--r--   0        0        0        0 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/utils/__init__.py
+-rw-r--r--   0        0        0     2237 2023-05-07 09:45:16.025202 valo_api_official-1.0.1/valo_api_official/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3586 1970-01-01 00:00:00.000000 valo_api_official-1.0.1/PKG-INFO
```

### Comparing `valo_api_official-1.0.0/LICENSE` & `valo_api_official-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/README.md` & `valo_api_official-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/pyproject.toml` & `valo_api_official-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api_official"
-version = "1.0.0"
+version = "1.0.1"
 description = "Valorant API Wrapper"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPIOfficial"
 homepage = "https://github.com/raimannma/ValorantAPIOfficial"
 
@@ -23,46 +23,46 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
-msgspec = "^0.12.0"
+msgspec = ">=0.12,<0.15"
 
 [tool.poetry.dev-dependencies]
-bandit = "^1.7.4"
+bandit = "^1.7.5"
 black = {version = "^22.12.0", allow-prereleases = true}
 darglint = "^1.8.1"
-isort = {extras = ["colors"], version = "^5.11.4"}
-mypy = "^0.991"
-mypy-extensions = "^0.4.3"
-pre-commit = "^2.21.0"
-pydocstyle = "^6.2.2"
-pylint = "^2.15.9"
-pytest = "^7.2.0"
-hypothesis = "^6.61.0"
-pyupgrade = "^3.3.1"
+isort = {extras = ["colors"], version = "^5.12.0"}
+mypy = "^1.2"
+mypy-extensions = "^1.0.0"
+pre-commit = "^3.3.1"
+pydocstyle = "^6.3.0"
+pylint = "^2.17.4"
+pytest = "^7.3.1"
+hypothesis = "^6.75.2"
+pyupgrade = "^3.4.0"
 safety = "^2.3.5"
 pytest-html = "^3.2.0"
 pytest-cov = "^4.0.0"
-Sphinx = "^5.3.0"
-sphinxcontrib-applehelp = "^1.0.2"
+Sphinx = "^6.2.1"
+sphinxcontrib-applehelp = "^1.0.4"
 sphinxcontrib-devhelp = "^1.0.2"
-sphinxcontrib-htmlhelp = "^2.0.0"
+sphinxcontrib-htmlhelp = "^2.0.1"
 sphinxcontrib-jsmath = "^1.0.1"
 sphinxcontrib-qthelp = "^1.0.3"
 sphinxcontrib-serializinghtml = "^1.1.5"
-sphinx-rtd-theme = "^1.1.1"
-sphinx-autodoc-typehints = "^1.19.5"
-autodocsumm = "^0.2.8"
-responses = "^0.22.0"
+sphinx-rtd-theme = "^1.2.0"
+sphinx-autodoc-typehints = "^1.23"
+autodocsumm = "^0.2.11"
+responses = "^0.23.1"
 pytest-parallel = "^0.1.1"
-pytest-split = "^0.8.0"
-tomlkit = "<0.11.7"
+pytest-split = "^0.8.1"
+tomlkit = "<0.11.9"
 colorama = "^0.4.6"
 
 
 [tool.black]
 target-version = ["py38"]
 line-length = 88
 color = true
```

### Comparing `valo_api_official-1.0.0/valo_api_official/config.py` & `valo_api_official-1.0.1/valo_api_official/config.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/__init__.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/account.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/account.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/active_shards.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/active_shards.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/content.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/content.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/leaderboard.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/match_details.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/match_details.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/match_history.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/recent_matches.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/recent_matches.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints/status.py` & `valo_api_official-1.0.1/valo_api_official/endpoints/status.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/endpoints_config.py` & `valo_api_official-1.0.1/valo_api_official/endpoints_config.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/exceptions/valo_api_exception.py` & `valo_api_official-1.0.1/valo_api_official/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/responses/content.py` & `valo_api_official-1.0.1/valo_api_official/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/responses/leaderboard.py` & `valo_api_official-1.0.1/valo_api_official/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/responses/match_details.py` & `valo_api_official-1.0.1/valo_api_official/responses/match_details.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from msgspec import Struct
 
 
 class MatchInfo(Struct):
     matchId: str
     mapId: str
     gameVersion: str
-    gameLengthMillis: int
     gameStartMillis: int
     isCompleted: bool
     customGameName: str
     gameMode: str
     isRanked: bool
     seasonId: str
     queueId: Optional[str] = None
     provisioningFlowID: Optional[str] = None
+    gameLengthMillis: Optional[int] = None
 
 
 class PlayerAbilityCasts(Struct):
     grenadeCasts: int
     ability1Casts: int
     ability2Casts: int
     ultimateCasts: int
@@ -37,19 +37,20 @@
 
 class MatchPlayers(Struct):
     puuid: str
     gameName: str
     tagLine: str
     teamId: str
     partyId: str
-    characterId: str
-    stats: PlayerStats
     competitiveTier: int
     playerCard: str
     playerTitle: str
+    isObserver: Optional[bool] = None
+    characterId: Optional[str] = None
+    stats: Optional[PlayerStats] = None
 
 
 class MatchTeam(Struct):
     teamId: str
     won: bool
     roundsPlayed: int
     roundsWon: int
```

### Comparing `valo_api_official-1.0.0/valo_api_official/responses/status.py` & `valo_api_official-1.0.1/valo_api_official/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/valo_api_official/utils/fetch_endpoint.py` & `valo_api_official-1.0.1/valo_api_official/utils/fetch_endpoint.py`

 * *Files identical despite different names*

### Comparing `valo_api_official-1.0.0/setup.py` & `valo_api_official-1.0.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,67 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: valo-api-official
+Version: 1.0.1
+Summary: Valorant API Wrapper
+Home-page: https://github.com/raimannma/ValorantAPIOfficial
+License: MIT
+Author: Manuel Raimann
+Author-email: raimannma@outlook.de
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: msgspec (>=0.12,<0.15)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Project-URL: Repository, https://github.com/raimannma/ValorantAPIOfficial
+Description-Content-Type: text/markdown
+
+# valo_api_official
+
+<div align="center">
+
+[![Build status](https://github.com/raimannma/ValorantAPIOfficial/workflows/build/badge.svg?branch=master&event=push)](https://github.com/raimannma/ValorantAPIOfficial/actions?query=workflow%3Abuild)
+[![Python Version](https://img.shields.io/pypi/pyversions/valo_api_official.svg)](https://pypi.org/project/valo_api_official/)
+[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/raimannma/ValorantAPI/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)
+
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/raimannma/ValorantAPIOfficial/blob/master/.pre-commit-config.yaml)
+[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/raimannma/ValorantAPIOfficial/releases)
+[![License](https://img.shields.io/github/license/raimannma/ValorantAPIOfficial)](https://github.com/raimannma/ValorantAPIOfficial/blob/master/LICENSE)
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/3b23d2a3b1694356bc95255a2edb83e6)](https://www.codacy.com/gh/raimannma/ValorantAPIOfficial/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=raimannma/ValorantAPIOfficial&amp;utm_campaign=Badge_Grade)
+[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/3b23d2a3b1694356bc95255a2edb83e6)](https://www.codacy.com/gh/raimannma/ValorantAPIOfficial/dashboard?utm_source=github.com&utm_medium=referral&utm_content=raimannma/ValorantAPIOfficial&utm_campaign=Badge_Coverage)
+[![Downloads](https://pepy.tech/badge/valo-api-official)](https://pepy.tech/project/valo-api-official)
+
+Valorant API Wrapper
+
+</div>
+
+## Installation
+
+    pip install valo-api-official
+
+## Documentation
+
+### Hosted
+
+The documentation is hosted here: https://raimannma.github.io/ValorantAPIOfficial/
 
-packages = \
-['valo_api_official',
- 'valo_api_official.endpoints',
- 'valo_api_official.exceptions',
- 'valo_api_official.responses',
- 'valo_api_official.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['msgspec>=0.12.0,<0.13.0', 'requests>=2.28.1,<3.0.0']
-
-setup_kwargs = {
-    'name': 'valo-api-official',
-    'version': '1.0.0',
-    'description': 'Valorant API Wrapper',
-    'long_description': '# valo_api_official\n\n<div align="center">\n\n[![Build status](https://github.com/raimannma/ValorantAPIOfficial/workflows/build/badge.svg?branch=master&event=push)](https://github.com/raimannma/ValorantAPIOfficial/actions?query=workflow%3Abuild)\n[![Python Version](https://img.shields.io/pypi/pyversions/valo_api_official.svg)](https://pypi.org/project/valo_api_official/)\n[![Dependencies Status](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)](https://github.com/raimannma/ValorantAPI/pulls?utf8=%E2%9C%93&q=is%3Apr%20author%3Aapp%2Fdependabot)\n\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)\n[![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/raimannma/ValorantAPIOfficial/blob/master/.pre-commit-config.yaml)\n[![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/raimannma/ValorantAPIOfficial/releases)\n[![License](https://img.shields.io/github/license/raimannma/ValorantAPIOfficial)](https://github.com/raimannma/ValorantAPIOfficial/blob/master/LICENSE)\n[![Codacy Badge](https://app.codacy.com/project/badge/Grade/3b23d2a3b1694356bc95255a2edb83e6)](https://www.codacy.com/gh/raimannma/ValorantAPIOfficial/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=raimannma/ValorantAPIOfficial&amp;utm_campaign=Badge_Grade)\n[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/3b23d2a3b1694356bc95255a2edb83e6)](https://www.codacy.com/gh/raimannma/ValorantAPIOfficial/dashboard?utm_source=github.com&utm_medium=referral&utm_content=raimannma/ValorantAPIOfficial&utm_campaign=Badge_Coverage)\n[![Downloads](https://pepy.tech/badge/valo-api-official)](https://pepy.tech/project/valo-api-official)\n\nValorant API Wrapper\n\n</div>\n\n## Installation\n\n    pip install valo-api-official\n\n## Documentation\n\n### Hosted\n\nThe documentation is hosted here: https://raimannma.github.io/ValorantAPIOfficial/\n\n### From Source\n\nAfter installing the package dependencies `pip install -r requirements.txt`, you can use the following commands to get the documentation:\n\n    cd docs/ && make html\n\nOpen the index.html file in the docs/_build/html/ directory.\n',
-    'author': 'Manuel Raimann',
-    'author_email': 'raimannma@outlook.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/raimannma/ValorantAPIOfficial',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+### From Source
 
+After installing the package dependencies `pip install -r requirements.txt`, you can use the following commands to get the documentation:
+
+    cd docs/ && make html
+
+Open the index.html file in the docs/_build/html/ directory.
 
-setup(**setup_kwargs)
```

