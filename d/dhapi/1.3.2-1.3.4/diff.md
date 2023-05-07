# Comparing `tmp/dhapi-1.3.2.tar.gz` & `tmp/dhapi-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.3.2.tar", last modified: Sun Apr 30 12:25:38 2023, max compression
+gzip compressed data, was "dhapi-1.3.4.tar", last modified: Sun May  7 15:10:52 2023, max compression
```

## Comparing `dhapi-1.3.2.tar` & `dhapi-1.3.4.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176642 dhapi-1.3.2/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.2/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     1160 2023-04-30 12:25:38.176519 dhapi-1.3.2/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      505 2023-04-19 16:05:26.000000 dhapi-1.3.2/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-19 16:05:26.000000 dhapi-1.3.2/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-04-30 12:25:38.176673 dhapi-1.3.2/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-04-30 12:24:58.000000 dhapi-1.3.2/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.173391 dhapi-1.3.2/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.174504 dhapi-1.3.2/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175318 dhapi-1.3.2/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4657 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175570 dhapi-1.3.2/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3393 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175802 dhapi-1.3.2/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2372 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176129 dhapi-1.3.2/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3919 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      463 2023-04-30 11:41:52.000000 dhapi-1.3.2/src/dhapi/router/router.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.176353 dhapi-1.3.2/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.2/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-04-30 12:25:38.175114 dhapi-1.3.2/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     1160 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      669 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       54 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/requires.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-04-30 12:25:38.000000 dhapi-1.3.2/src/dhapi.egg-info/top_level.txt
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227639 dhapi-1.3.4/
+-rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.4/LICENSE.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:10:52.227515 dhapi-1.3.4/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)     1245 2023-05-07 14:36:29.000000 dhapi-1.3.4/README.md
+-rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-30 18:03:10.000000 dhapi-1.3.4/pyproject.toml
+-rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-05-07 15:10:52.227670 dhapi-1.3.4/setup.cfg
+-rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-07 15:06:57.000000 dhapi-1.3.4/setup.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.222521 dhapi-1.3.4/src/
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.223639 dhapi-1.3.4/src/dhapi/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/__init__.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226194 dhapi-1.3.4/src/dhapi/client/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/client/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     4804 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/client/lottery_client.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226405 dhapi-1.3.4/src/dhapi/domain_object/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/domain_object/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     3313 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/main.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.226598 dhapi-1.3.4/src/dhapi/purchase/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/purchase/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     2410 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/purchase/lotto645_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227073 dhapi-1.3.4/src/dhapi/router/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/router/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)     5132 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/router/arg_parser.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-07 15:04:37.000000 dhapi-1.3.4/src/dhapi/router/router.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-07 15:10:00.000000 dhapi-1.3.4/src/dhapi/router/version_checker.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.227306 dhapi-1.3.4/src/dhapi/user_info/
+-rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/user_info/__init__.py
+-rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.4/src/dhapi/user_info/user_info_controller.py
+drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:10:52.225989 dhapi-1.3.4/src/dhapi.egg-info/
+-rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/PKG-INFO
+-rw-r--r--   0 roeniss    (501) staff       (20)      705 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/SOURCES.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/dependency_links.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/entry_points.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)       72 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/requires.txt
+-rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-05-07 15:10:52.000000 dhapi-1.3.4/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.3.2/LICENSE.txt` & `dhapi-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.2/setup.py` & `dhapi-1.3.4/setup.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.2/src/dhapi/client/lottery_client.py` & `dhapi-1.3.4/src/dhapi/client/lottery_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import json
+import logging
 import requests
 from bs4 import BeautifulSoup
 
 from dhapi.domain_object.lotto645_buy_request import Lotto645BuyRequest
 
+logger = logging.getLogger(__name__)
+
 
 # TODO : LotteryClient 를 한번만 만들어 쓰도록 Singleton/DI 적용
 class LotteryClient:
     _default_session_url = "https://dhlottery.co.kr/gameResult.do?method=byWin&wiselog=H_C_1_1"
     _system_under_check_url = "https://dhlottery.co.kr/index_check.html"
     _main_url = "https://dhlottery.co.kr/common.do?method=main"
     _login_request_url = "https://www.dhlottery.co.kr/userSsl.do?method=login"
@@ -34,24 +37,26 @@
         }
         self._set_default_session()
 
     # 로그인을 시도하면 새로운 JSESSIONID 값이 내려오는데,
     #  이 값으로 갱신하면 로그인이 풀리는 듯하여 헤더를 갱신하지 않음
     def _set_default_session(self):
         resp = requests.get(LotteryClient._default_session_url, timeout=10)
+        logger.debug(f"resp.status_code: {resp.status_code}")
+        logger.debug(f"resp.headers: {resp.headers}")
 
         if resp.url == LotteryClient._system_under_check_url:
-            raise FileNotFoundError("동행복권 사이트가 현재 시스템 점검중입니다.")
+            raise RuntimeError("동행복권 사이트가 현재 시스템 점검중입니다.")
 
         for cookie in resp.cookies:
             if cookie.name == "JSESSIONID":
                 self._headers["Cookie"] = f"JSESSIONID={cookie.value}"
                 break
         else:
-            raise KeyError("JSESSIONID cookie is not set in response")
+            raise RuntimeError("JSESSIONID 쿠키가 정상적으로 세팅되지 않았습니다.")
 
     def login(self, user_id: str, user_pw: str):
         resp = requests.post(
             LotteryClient._login_request_url,
             headers=self._headers,
             data={
                 "returnUrl": LotteryClient._main_url,
@@ -60,15 +65,15 @@
                 "checkSave": "off",
                 "newsEventYn": "",
             },
             timeout=10,
         )
         soup = BeautifulSoup(resp.text, "html5lib")
         if soup.find("a", {"class": "btn_common"}) is not None:
-            raise ValueError("로그인에 실패했습니다. \n아이디 또는 비밀번호를 확인해주세요.\n아이디는 대소문자를 구분합니다.")
+            raise RuntimeError("로그인에 실패했습니다. 아이디 또는 비밀번호를 확인해주세요.")
 
     def _get_round(self):
         resp = requests.get(self._round_info_url, timeout=10)
         soup = BeautifulSoup(resp.text, "html5lib")  # 'html5lib' : in case that the html don't have clean tag pairs
         last_drawn_round = int(soup.find("strong", id="lottoDrwNo").text)
         return last_drawn_round + 1
```

### Comparing `dhapi-1.3.2/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-1.3.4/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,69 @@
 import json
 
 
 class Lotto645BuyRequest:
     def __init__(self, games=None):
         """
-        :param 게임은 다섯 개의 list 로 이루어져 있다. 각 게임은 여섯 칸 짜리 list 로 이루어져 있다. 각 칸은 1~45 의 숫자 또는 '자동'을 의미하는 "*" 를 사용한다.
-         Asterisk("*") can be to indicate auto mode for that position.
-         e.g. [["*", "*", "*", "*", "*"], ["*"], [1, 2, 3, 4, 15, 45], None, [3, 5, "*", "*", "*"]]
+        :param 게임은 다섯 개의 list 로 이루어져 있다. 각 게임은 여섯 칸 짜리 list 로 이루어져 있다. 각 칸은 1~45 의 숫자 또는 '자동'을 의미하는 "x" 를 사용한다.
+         e.g. [["x", "x", "x", "x", "x"], ["x"], [1, 2, 3, 4, 15, 45], None, [3, 5, "x", "x", "x"]]
          - This example shows two auto games, one manual game, one half-auto game and forth game is not used.
         """
         self._games = games
 
         if not self._is_correct_games(games):
-            raise ValueError(f"비정상적인 입력값입니다. {self.format()}")
+            raise RuntimeError(f"비정상적인 구매 요청입니다.\n{self.format()}")
 
     def _is_correct_games(self, games):
         return isinstance(games, list) and len(games) == 5 and all(map(lambda x: self._is_correct_game(x), games))
 
     def _is_correct_game(self, game):
         return game is None or (
             isinstance(game, list)
             and (len(game) == 6 or len(game) == 1)
-            and (len(set(filter(lambda x: x != "*", game))) == len(list(filter(lambda x: x != "*", game))))
-            and all(map(lambda x: x == "*" or 1 <= x <= 45, game))
+            and (len(set(filter(lambda x: x != "x", game))) == len(list(filter(lambda x: x != "x", game))))
+            and all(map(lambda x: x == "x" or 1 <= x <= 45, game))
         )
 
     def has_auto_game(self):
         return any(filter(lambda game: self._is_auto_game(game), self._filter_used_games()))
 
     def _is_auto_game(self, game):
-        return self._get_auto_count_in_game(game) == 6
+        return (len(game) == 6 and self._get_auto_count_in_game(game) == 6) or (len(game) == 1 and self._get_auto_count_in_game(game) == 1)
 
     def has_half_auto_game(self):
         return any(filter(lambda game: self._is_half_auto_game(game), self._filter_used_games()))
 
     def _is_half_auto_game(self, game):
-        return 0 < self._get_auto_count_in_game(game) < 6 and (self._get_auto_count_in_game(game) != 1)
+        return len(game) == 6 and 0 < self._get_auto_count_in_game(game) < 6 and (self._get_auto_count_in_game(game) != 1)
 
     def has_manual_game(self):
         return any(filter(lambda game: self._is_manual_game(game), self._filter_used_games()))
 
     def _is_manual_game(self, game):
         return self._get_auto_count_in_game(game) == 0
 
     def _get_auto_count_in_game(self, game):
         """한 게임 내에서의 자동번호 개수를 반환한다. 사용하지 않는 게임(None)에 대해선 사용할 수 없다."""
-        return len(list(filter(lambda x: x == "*", game)))
+        return len(list(filter(lambda x: x == "x", game)))
 
     def get_game_count(self):
         return len(self._filter_used_games())
 
     def _filter_used_games(self):
         return list(filter(lambda x: x is not None, self._games))
 
     def format(self):
-        return (
-            f"""
-[Lotto645 Buy Request]
-Input: {self._games}            
-"""
-            if self._games is None
-            else f"""
-[Lotto645 Buy Request]
+        return f"""[Lotto645 Buy Request]
 Game A: {self._games[0]}
 Game B: {self._games[1]}
 Game C: {self._games[2]}
 Game D: {self._games[3]}
 Game E: {self._games[4]}
-"""
-        )
+----------------------"""
 
     def create_dhlottery_request_param(self):
         params = []
         slots = ["A", "B", "C", "D", "E"]
 
         for i, game in enumerate(self._games):
             slot = slots[i]
```

### Comparing `dhapi-1.3.2/src/dhapi/purchase/lotto645_controller.py` & `dhapi-1.3.4/src/dhapi/purchase/lotto645_controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,70 @@
+import logging
+
 from dhapi.client.lottery_client import LotteryClient
 from dhapi.domain_object.lotto645_buy_request import Lotto645BuyRequest
 
+logger = logging.getLogger(__name__)
+
 
 class Lotto645Controller:
     def __init__(self, user_id, user_pw):
         self.client = LotteryClient()
         self.client.login(user_id, user_pw)
 
     def buy(self, req: Lotto645BuyRequest, quiet: bool):
-        if req.has_manual_game():
-            raise NotImplementedError("수동 번호 입력은 아직 구현되지 않았습니다. 필요하시면 이슈를 남겨주세요.")
         if req.has_half_auto_game():
             raise NotImplementedError("반자동 입력은 아직 구현되지 않았습니다. 필요하시면 이슈를 남겨주세요.")
 
         if not self._confirm_purchase(req, quiet):
-            print("구매를 취소했습니다.")
+            print("✅ 구매를 취소했습니다.")
         else:
             result = self.client.buy_lotto645(req)
             self._show_result(result)
 
     def _confirm_purchase(self, req, quiet):
         print(
             f"""{req.format()}
-위와 같이 구매하시겠습니까? [[Y]/n] """,
+❓ 위와 같이 구매하시겠습니까? [Y/n] """,
             end="",
         )
 
         if quiet:
-            print("\nquiet 플래그가 주어져 자동으로 구매를 진행합니다.")
+            print("yes\n✅ --quiet 플래그가 주어져 자동으로 구매를 진행합니다.")
             return True
         else:
             answer = input().strip().lower()
             return answer in ["y", "yes", ""]
 
     # ID가 다른 경우 loginYn이 N으로 나옴
     def _show_result(self, body: dict) -> None:
         result = body.get("result", {})
         if result.get("resultMsg", "FAILURE").upper() != "SUCCESS":
-            print(f'Fail to purchase (reason: {result.get("resultMsg", f"Unknown (resultMsg field is empty. full response: {body})")})')
-            return
+            logger.debug(f"d: {body}")
+            raise RuntimeError(f'구매에 실패했습니다: {result.get("resultMsg", "resultMsg is empty")}')
+
+        logger.debug(f"response body: {body}")
 
         print(
-            f"""Success to purchase
+            f"""✅ 구매를 완료하였습니다.
+[Lotto645 Buy Response]
 ------------------
-Round: {result["buyRound"]}
-Barcode: {result["barCode1"]} {result["barCode2"]} {result["barCode3"]} {result["barCode4"]} {result["barCode5"]} {result["barCode6"]}
-Cost : {result["nBuyAmount"]}
-Numbers: \n{self._format_lotto_numbers(result["arrGameChoiceNum"])}
-Result Message: {result["resultMsg"]}
-Body: {body}
-------------------"""
+Round:\t\t{result["buyRound"]}
+Barcode:\t{result["barCode1"]} {result["barCode2"]} {result["barCode3"]} {result["barCode4"]} {result["barCode5"]} {result["barCode6"]}
+Cost:\t\t{result["nBuyAmount"]}
+Numbers:\n{self._format_lotto_numbers(result["arrGameChoiceNum"])}
+Message:\t{result["resultMsg"]}
+----------------------"""
         )
 
-    def _format_lotto_numbers(self, numbers: list) -> None:
-        # Manual : 1, Combine : 2, Automatic : 3
-        tabbed_numbers = ["\t\t" + number for number in numbers]
-        linebroken_tabbed_numbers = "\n".join(tabbed_numbers)
-        return linebroken_tabbed_numbers
+    def _format_lotto_numbers(self, lines: list) -> None:
+        modes = {
+            "1": "수동",
+            "2": "반자동",
+            "3": "자동",
+        }
+
+        tabbed_lines = []
+        for _, line in enumerate(lines):
+            tabbed_lines.append(f"\t\t{line[:-1]} ({modes[line[-1]]})")
+
+        return "\n".join(tabbed_lines)
```

### Comparing `dhapi-1.3.2/src/dhapi/router/arg_parser.py` & `dhapi-1.3.4/src/dhapi/router/arg_parser.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,102 +1,131 @@
 import argparse
+import pathlib
 import getpass
+import os
 import sys
 
+from dhapi.router.version_checker import get_versions
 from dhapi.domain_object.lotto645_buy_request import Lotto645BuyRequest
 
 
 class HelpOnErrorParser(argparse.ArgumentParser):
     def error(self, message):
-        sys.stderr.write(f"error: {message}\n")
-        self.print_help()
-        sys.exit(2)
+        sys.stderr.write(f"🚨 입력 파라미터 에러 발생: {message}\n")
+        sys.exit(1)
+
+
+def _exit(message):
+    obj = HelpOnErrorParser()
+    obj.error(message)
 
 
 class ArgParser:
     def __init__(self):
         parser = HelpOnErrorParser(description="동행복권 비공식 API", formatter_class=argparse.RawTextHelpFormatter)
-        parser.add_argument("-v", "--version", action="version", version="%(prog)s 1.3.1")
+        installed_version, _ = get_versions()
+        parser.add_argument("-v", "--version", action="version", version="%(prog)s " + installed_version)
 
         command_subparser = parser.add_subparsers(title="명령어 구분", dest="command", required=True)
 
         buy_lotto645 = command_subparser.add_parser(
             "buy_lotto645",
             help="로또6/45 구매",
             epilog="""
- 
+
 [buy_lotto645 명령어 사용 예시]
-    
-dhapi buy_lotto645 -u $USER_ID -q  # 확인 절차 없이 자동으로 5장 구매
-dhapi buy_lotto645 -u $USER_ID -p $USER_PW -g *,*,*,*,*,*  # 자동으로 1장 구매
-dhapi buy_lotto645 -u $USER_ID -p $USER_PW -g *  # 자동으로 1장 구매 (단축형)
-dhapi buy_lotto645 -u $USER_ID -g 1,2,3,4,5,6 -g 5,6,7,*,*,* -g *,*,*,*,*,* -g *  # 1장 수동, 1장 반자동, 2장 자동 - 총 4장 구매
+
+dhapi buy_lotto645
+\t\t\t# ~/.dhapi_profile 을 읽어 ID/PW 를 자동으로 입력받고, 확인 후 자동모드로 5장 구매 (프로필 파일 포맷은 README.md 참고)
+dhapi buy_lotto645 -q
+\t\t\t# 확인 절차 없이 자동모드로 5장 구매
+dhapi buy_lotto645 -u $USER_ID
+\t\t\t# ID/PW 를 직접 입력받아 자동모드로 5장 구매 (deprecated)
+dhapi buy_lotto645 -g x,x,x,x,x,x
+\t\t\t# 자동모드로 1장 구매 (1 game)
+dhapi buy_lotto645 -g x
+\t\t\t# 자동모드로 1장 구매 (단축형)
+dhapi buy_lotto645 -g 1,2,3,4,5,6 -g 5,6,7,x,x,x -g x,x,x,x,x,x -g x
+\t\t\t# 1장 수동모드, 1장 반자동모드, 2장 자동모드
+
 """,
         )
 
         buy_lotto645.formatter_class = argparse.RawTextHelpFormatter
 
-        buy_lotto645.add_argument("-u", "--username", required=True, help="동행복권 아이디")
-        buy_lotto645.add_argument(
-            "-p",
-            "--password",
-            required=False,
-            help="동행복권 비밀번호 (값을 입력하지 않으면 실행 후 비밀번호를 입력받음)",
-        )
-        buy_lotto645.add_argument("-q", "--quiet", action="store_true", help="플래그 설정 시 구매 전 확인 절차를 스킵합니다")  # "store_true" means "set default to False"
+        buy_lotto645.add_argument("-u", "--username", required=False, help="동행복권 아이디입니다. (deprecated; -p 옵션 사용 권장)")
+        buy_lotto645.add_argument("-q", "--quiet", action="store_true", help="플래그 설정 시 구매 전 확인 절차를 스킵합니다.")  # "store_true" means "set default to False"
         buy_lotto645.add_argument(
             "-g",
             "--game",
             required=False,
             action="append",
             dest="games",
             help="""
 구매할 번호 6개를 콤마로 구분해 입력합니다.
 옵션을 여러번 사용하여 여러 게임을 구매할 수 있습니다 (매주 최대 5 게임).
-'-g *,*,*,*,*,*' 또는 '-g *' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드). 
-특정 숫자 대신 '*'를 입력해 해당 값만 자동으로 구매할 수 있습니다 (반자동 모드).
+'-g x,x,x,x,x,x' 또는 '-g x' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드).
+특정 숫자 대신 'x'를 입력해 해당 값만 자동으로 구매할 수 있습니다 (반자동 모드).
 옵션을 아예 입력하지 않으면 '자동으로 5장 구매'를 수행합니다.""",
         )
-
+        buy_lotto645.add_argument(
+            "-p",
+            "--profile",
+            required=False,
+            nargs=1,
+            default="~/.dhapi_profile",
+            help="프로필 파일 절대경로입니다. (default: ~/.dhapi_profile; 포맷은 README.md 참고)",
+        )
+        buy_lotto645.add_argument("-d", "--debug", action="store_true", help="로그 출력 레벨을 debug로 세팅합니다.")  # "store_true" means "set default to False"
         self._args = parser.parse_args()
 
-        if self._args.password is None:
+        if not self._args.username is None:
             self._args.password = getpass.getpass("비밀번호를 입력하세요: ")
+        else:
+            profile_path = pathlib.Path(self._args.profile).expanduser()
+            if not (os.path.exists(profile_path) and os.path.isfile(profile_path)):
+                _exit(f"{self._args.profile} 파일이 존재하지 않습니다")
+
+            with open(profile_path, encoding="utf-8") as f:
+                self._args.username, self._args.password = f.read().splitlines()
 
         if self.is_buylotto645():
             self.normalize_games_for_lotto645()
 
+    def get_is_debug(self):
+        return self._args.debug
+
     def get_user_id(self):
         return self._args.username
 
     def get_user_pw(self):
         return self._args.password
 
     def is_quiet(self):
         return self._args.quiet
 
     def is_buylotto645(self):
         return self._args.command == "buy_lotto645"
 
     def normalize_games_for_lotto645(self):
         if self._args.games is None:
-            self._args.games = ["*,*,*,*,*,*" for _ in range(5)]
+            self._args.games = ["x,x,x,x,x,x" for _ in range(5)]
         else:
             while len(self._args.games) < 5:
                 self._args.games.append(None)
 
         req_bucket = []
         for game in self._args.games:
             if game is None:
                 req_bucket.append(game)
             else:
                 req_slot = []
                 nums_and_asterisks = game.split(",")
                 for i in nums_and_asterisks:
-                    if i == "*":
+                    if i == "x":
                         req_slot.append(i)
                     else:
                         req_slot.append(int(i))
                 req_bucket.append(req_slot)
 
         self._args.games = req_bucket
```

### Comparing `dhapi-1.3.2/src/dhapi.egg-info/SOURCES.txt` & `dhapi-1.3.4/src/dhapi.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -15,9 +15,10 @@
 src/dhapi/domain_object/__init__.py
 src/dhapi/domain_object/lotto645_buy_request.py
 src/dhapi/purchase/__init__.py
 src/dhapi/purchase/lotto645_controller.py
 src/dhapi/router/__init__.py
 src/dhapi/router/arg_parser.py
 src/dhapi/router/router.py
+src/dhapi/router/version_checker.py
 src/dhapi/user_info/__init__.py
 src/dhapi/user_info/user_info_controller.py
```

