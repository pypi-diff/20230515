# Comparing `tmp/dhapi-1.3.5.tar.gz` & `tmp/dhapi-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhapi-1.3.5.tar", last modified: Sun May  7 15:13:47 2023, max compression
+gzip compressed data, was "dhapi-1.4.0.tar", last modified: Mon May 15 00:50:10 2023, max compression
```

## Comparing `dhapi-1.3.5.tar` & `dhapi-1.4.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.163349 dhapi-1.3.5/
--rw-r--r--   0 roeniss    (501) staff       (20)    11356 2023-04-19 16:05:26.000000 dhapi-1.3.5/LICENSE.txt
--rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:13:47.163217 dhapi-1.3.5/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)     1245 2023-05-07 14:36:29.000000 dhapi-1.3.5/README.md
--rw-r--r--   0 roeniss    (501) staff       (20)       51 2023-04-30 18:03:10.000000 dhapi-1.3.5/pyproject.toml
--rw-r--r--   0 roeniss    (501) staff       (20)       38 2023-05-07 15:13:47.163387 dhapi-1.3.5/setup.cfg
--rw-r--r--   0 roeniss    (501) staff       (20)     1271 2023-05-07 15:06:57.000000 dhapi-1.3.5/setup.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.157468 dhapi-1.3.5/src/
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.158573 dhapi-1.3.5/src/dhapi/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/__init__.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.161861 dhapi-1.3.5/src/dhapi/client/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/client/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     4804 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/client/lottery_client.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162066 dhapi-1.3.5/src/dhapi/configuration/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-05-07 15:12:24.000000 dhapi-1.3.5/src/dhapi/configuration/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      862 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/configuration/logger.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162249 dhapi-1.3.5/src/dhapi/domain_object/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/domain_object/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     3313 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/domain_object/lotto645_buy_request.py
--rw-r--r--   0 roeniss    (501) staff       (20)      120 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/main.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162445 dhapi-1.3.5/src/dhapi/purchase/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/purchase/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     2410 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/purchase/lotto645_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.162839 dhapi-1.3.5/src/dhapi/router/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/router/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)     5132 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/router/arg_parser.py
--rw-r--r--   0 roeniss    (501) staff       (20)      518 2023-05-07 15:04:37.000000 dhapi-1.3.5/src/dhapi/router/router.py
--rw-r--r--   0 roeniss    (501) staff       (20)      953 2023-05-07 15:10:00.000000 dhapi-1.3.5/src/dhapi/router/version_checker.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.163035 dhapi-1.3.5/src/dhapi/user_info/
--rw-r--r--   0 roeniss    (501) staff       (20)        0 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/user_info/__init__.py
--rw-r--r--   0 roeniss    (501) staff       (20)      202 2023-04-19 16:05:26.000000 dhapi-1.3.5/src/dhapi/user_info/user_info_controller.py
-drwxr-xr-x   0 roeniss    (501) staff       (20)        0 2023-05-07 15:13:47.161670 dhapi-1.3.5/src/dhapi.egg-info/
--rw-r--r--   0 roeniss    (501) staff       (20)     1900 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/PKG-INFO
--rw-r--r--   0 roeniss    (501) staff       (20)      775 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/SOURCES.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        1 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/dependency_links.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       42 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/entry_points.txt
--rw-r--r--   0 roeniss    (501) staff       (20)       72 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/requires.txt
--rw-r--r--   0 roeniss    (501) staff       (20)        6 2023-05-07 15:13:47.000000 dhapi-1.3.5/src/dhapi.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    11356 2023-05-15 00:45:36.000000 dhapi-1.4.0/LICENSE.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2615 2023-05-15 00:50:10.086488 dhapi-1.4.0/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1960 2023-05-15 00:45:36.000000 dhapi-1.4.0/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       51 2023-05-15 00:45:36.000000 dhapi-1.4.0/pyproject.toml
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-15 00:50:10.086488 dhapi-1.4.0/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1271 2023-05-15 00:45:36.000000 dhapi-1.4.0/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.078488 dhapi-1.4.0/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/__init__.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/client/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/client/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4804 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/client/lottery_client.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/configuration/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/configuration/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      862 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/configuration/logger.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi/domain_object/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/domain_object/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3954 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/domain_object/lotto645_buy_request.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      120 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/main.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/purchase/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/purchase/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2231 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/purchase/lotto645_controller.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/router/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/router/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4616 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/arg_parser.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      518 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/router.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      953 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/router/version_checker.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.086488 dhapi-1.4.0/src/dhapi/user_info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:46:17.000000 dhapi-1.4.0/src/dhapi/user_info/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      202 2023-05-15 00:45:36.000000 dhapi-1.4.0/src/dhapi/user_info/user_info_controller.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-15 00:50:10.082488 dhapi-1.4.0/src/dhapi.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2615 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      775 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       42 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       72 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        6 2023-05-15 00:50:10.000000 dhapi-1.4.0/src/dhapi.egg-info/top_level.txt
```

### Comparing `dhapi-1.3.5/LICENSE.txt` & `dhapi-1.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.5/setup.py` & `dhapi-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.5/src/dhapi/client/lottery_client.py` & `dhapi-1.4.0/src/dhapi/client/lottery_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         last_drawn_round = int(soup.find("strong", id="lottoDrwNo").text)
         return last_drawn_round + 1
 
     def buy_lotto645(self, req: Lotto645BuyRequest):
         """
         :param first 첫 번째 복권 게임을 의미한다. 다음 두 가지 형태 중 하나를 가진다.
          - 일반 숫자 5개와 보너스 숫자를 포함하는 list ([1, 2, 3, 4, 5, 6]) (각각 1~45)
-         - 자동 또는 반자동을 의미하는 str ("AUTO", "HALF_AUTO")
+         - 자동 또는 반자동을 의미하는 str ("AUTO", "SEMI_AUTO")
          위 내용은 second, third, fourth, fifth 파라미터에도 적용된다.
         """
 
         resp = requests.post(
             self._buy_lotto645_url,
             headers=self._headers,
             data={
```

### Comparing `dhapi-1.3.5/src/dhapi/configuration/logger.py` & `dhapi-1.4.0/src/dhapi/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.5/src/dhapi/domain_object/lotto645_buy_request.py` & `dhapi-1.4.0/src/dhapi/domain_object/lotto645_buy_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,116 @@
+import enum
 import json
+import os
+import string
+
+
+class Lotto645GameType(enum.IntEnum):
+    AUTO = 0
+    MANUAL = 1
+    SEMIAUTO = 2
 
 
 class Lotto645BuyRequest:
-    def __init__(self, games=None):
+    MAX_NUMBER_COUNT_IN_GAME = 6
+    MAX_GAME_COUNT = 5
+
+    def __init__(self, games):
         """
-        :param 게임은 다섯 개의 list 로 이루어져 있다. 각 게임은 여섯 칸 짜리 list 로 이루어져 있다. 각 칸은 1~45 의 숫자 또는 '자동'을 의미하는 "x" 를 사용한다.
-         e.g. [["x", "x", "x", "x", "x"], ["x"], [1, 2, 3, 4, 15, 45], None, [3, 5, "x", "x", "x"]]
-         - This example shows two auto games, one manual game, one half-auto game and forth game is not used.
+        :param 게임은 다섯 개 이하의 list 로 이루어져 있다.
+        각 게임은 여섯 칸 이하의 list 로 이루어져 있다. 각 칸은 1~45 의 숫자를 사용한다.
+        - 숫자가 없는 list는 자동을 의미한다.
+        - 여섯개의 숫자를 갖는 list는 수동을 의미한다.
+        - 한개 이상 여섯개 미만의 숫자를 갖는 list는 반자동을 의미한다.
+        e.g. [[], [], [], [1, 2], [1, 2, 3, 4, 15, 45]]
+        - This example shows three auto games, one semi-auto game and one manual game.
         """
         self._games = games
 
         if not self._is_correct_games(games):
             raise RuntimeError(f"비정상적인 구매 요청입니다.\n{self.format()}")
 
     def _is_correct_games(self, games):
-        return isinstance(games, list) and len(games) == 5 and all(map(lambda x: self._is_correct_game(x), games))
+        # fmt: off
+        return (isinstance(games, list)
+            and len(games) <= self.MAX_GAME_COUNT
+            and all(map(lambda x: self._is_correct_game(x), games)))
+        # fmt: on
 
     def _is_correct_game(self, game):
-        return game is None or (
-            isinstance(game, list)
-            and (len(game) == 6 or len(game) == 1)
-            and (len(set(filter(lambda x: x != "x", game))) == len(list(filter(lambda x: x != "x", game))))
-            and all(map(lambda x: x == "x" or 1 <= x <= 45, game))
-        )
+        # fmt: off
+        return (isinstance(game, list)
+            and len(game) <= self.MAX_NUMBER_COUNT_IN_GAME
+            and all(map(lambda x: isinstance(x, int) and 1 <= x <= 45, game))
+            and len(game) == len(set(game)))
+        # fmt: on
 
     def has_auto_game(self):
         return any(filter(lambda game: self._is_auto_game(game), self._filter_used_games()))
 
     def _is_auto_game(self, game):
-        return (len(game) == 6 and self._get_auto_count_in_game(game) == 6) or (len(game) == 1 and self._get_auto_count_in_game(game) == 1)
+        return self._get_manual_count_in_game(game) == 0
 
-    def has_half_auto_game(self):
-        return any(filter(lambda game: self._is_half_auto_game(game), self._filter_used_games()))
+    def has_semi_auto_game(self):
+        return any(filter(lambda game: self._is_semi_auto_game(game), self._filter_used_games()))
 
-    def _is_half_auto_game(self, game):
-        return len(game) == 6 and 0 < self._get_auto_count_in_game(game) < 6 and (self._get_auto_count_in_game(game) != 1)
+    def _is_semi_auto_game(self, game):
+        return 0 < self._get_manual_count_in_game(game) < self.MAX_NUMBER_COUNT_IN_GAME
 
     def has_manual_game(self):
         return any(filter(lambda game: self._is_manual_game(game), self._filter_used_games()))
 
     def _is_manual_game(self, game):
-        return self._get_auto_count_in_game(game) == 0
+        return self._get_manual_count_in_game(game) == self.MAX_NUMBER_COUNT_IN_GAME
 
     def _get_auto_count_in_game(self, game):
-        """한 게임 내에서의 자동번호 개수를 반환한다. 사용하지 않는 게임(None)에 대해선 사용할 수 없다."""
-        return len(list(filter(lambda x: x == "x", game)))
+        return self.MAX_NUMBER_COUNT_IN_GAME - len(game)
+
+    def _get_manual_count_in_game(self, game):
+        return len(game)
 
     def get_game_count(self):
         return len(self._filter_used_games())
 
     def _filter_used_games(self):
         return list(filter(lambda x: x is not None, self._games))
 
+    def _get_game_type(self, game):
+        if self._is_auto_game(game):
+            return Lotto645GameType.AUTO
+        if self._is_manual_game(game):
+            return Lotto645GameType.MANUAL
+        if self._is_semi_auto_game(game):
+            return Lotto645GameType.SEMIAUTO
+
+        raise RuntimeError("지원하지 않는 게임 타입입니다.")
+
+    def _get_gen_type(self, game_type):
+        if not isinstance(game_type, Lotto645GameType):
+            raise RuntimeError("지원하지 않는 게임 타입입니다.")
+
+        return str(game_type)
+
+    def _encode_game(self, slot, game):
+        game_type = self._get_game_type(game)
+        # fmt: off
+        return {
+            "genType": self._get_gen_type(game_type),
+            "arrGameChoiceNum": ",".join(map(str, game)) if game_type != Lotto645GameType.AUTO else None,
+            "alpabet": slot
+        }
+        # fmt: on
+
     def format(self):
-        return f"""[Lotto645 Buy Request]
-Game A: {self._games[0]}
-Game B: {self._games[1]}
-Game C: {self._games[2]}
-Game D: {self._games[3]}
-Game E: {self._games[4]}
-----------------------"""
+        return f"""
+[Lotto645 Buy Request]
+{os.linesep.join(f'Game {string.ascii_uppercase[i]}: {game}' for i, game in enumerate(self._games))}
+"""
 
     def create_dhlottery_request_param(self):
         params = []
-        slots = ["A", "B", "C", "D", "E"]
 
         for i, game in enumerate(self._games):
-            slot = slots[i]
-            if game is None:
-                continue
-            elif self._is_auto_game(game):
-                params.append({"genType": "0", "arrGameChoiceNum": None, "alpabet": slot})
-            elif self._is_half_auto_game(game):
-                raise NotImplementedError("반자동 모드는 아직 구현되지 않았습니다.")
-            else:
-                params.append({"genType": "0", "arrGameChoiceNum": game, "alpabet": slot})
+            slot = string.ascii_uppercase[i]
+            params.append(self._encode_game(slot, sorted(game)))
 
         return json.dumps(params)
```

### Comparing `dhapi-1.3.5/src/dhapi/purchase/lotto645_controller.py` & `dhapi-1.4.0/src/dhapi/purchase/lotto645_controller.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,17 +8,14 @@
 
 class Lotto645Controller:
     def __init__(self, user_id, user_pw):
         self.client = LotteryClient()
         self.client.login(user_id, user_pw)
 
     def buy(self, req: Lotto645BuyRequest, quiet: bool):
-        if req.has_half_auto_game():
-            raise NotImplementedError("반자동 입력은 아직 구현되지 않았습니다. 필요하시면 이슈를 남겨주세요.")
-
         if not self._confirm_purchase(req, quiet):
             print("✅ 구매를 취소했습니다.")
         else:
             result = self.client.buy_lotto645(req)
             self._show_result(result)
 
     def _confirm_purchase(self, req, quiet):
```

### Comparing `dhapi-1.3.5/src/dhapi/router/arg_parser.py` & `dhapi-1.4.0/src/dhapi/router/arg_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,19 +36,17 @@
 
 dhapi buy_lotto645
 \t\t\t# ~/.dhapi_profile 을 읽어 ID/PW 를 자동으로 입력받고, 확인 후 자동모드로 5장 구매 (프로필 파일 포맷은 README.md 참고)
 dhapi buy_lotto645 -q
 \t\t\t# 확인 절차 없이 자동모드로 5장 구매
 dhapi buy_lotto645 -u $USER_ID
 \t\t\t# ID/PW 를 직접 입력받아 자동모드로 5장 구매 (deprecated)
-dhapi buy_lotto645 -g x,x,x,x,x,x
+dhapi buy_lotto645 -g
 \t\t\t# 자동모드로 1장 구매 (1 game)
-dhapi buy_lotto645 -g x
-\t\t\t# 자동모드로 1장 구매 (단축형)
-dhapi buy_lotto645 -g 1,2,3,4,5,6 -g 5,6,7,x,x,x -g x,x,x,x,x,x -g x
+dhapi buy_lotto645 -g 1,2,3,4,5,6 -g 5,6,7 -g -g
 \t\t\t# 1장 수동모드, 1장 반자동모드, 2장 자동모드
 
 """,
         )
 
         buy_lotto645.formatter_class = argparse.RawTextHelpFormatter
 
@@ -56,19 +54,21 @@
         buy_lotto645.add_argument("-q", "--quiet", action="store_true", help="플래그 설정 시 구매 전 확인 절차를 스킵합니다.")  # "store_true" means "set default to False"
         buy_lotto645.add_argument(
             "-g",
             "--game",
             required=False,
             action="append",
             dest="games",
+            nargs="?",
+            const=None,
             help="""
 구매할 번호 6개를 콤마로 구분해 입력합니다.
 옵션을 여러번 사용하여 여러 게임을 구매할 수 있습니다 (매주 최대 5 게임).
-'-g x,x,x,x,x,x' 또는 '-g x' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드).
-특정 숫자 대신 'x'를 입력해 해당 값만 자동으로 구매할 수 있습니다 (반자동 모드).
+'-g' 형태로 제시하면 해당 게임의 모든 번호를 자동으로 선택합니다 (자동 모드).
+6개 미만의 번호를 입력하면 나머지 번호는 자동으로 구매할 수 있습니다 (반자동 모드).
 옵션을 아예 입력하지 않으면 '자동으로 5장 구매'를 수행합니다.""",
         )
         buy_lotto645.add_argument(
             "-p",
             "--profile",
             required=False,
             nargs=1,
@@ -104,30 +104,17 @@
         return self._args.quiet
 
     def is_buylotto645(self):
         return self._args.command == "buy_lotto645"
 
     def normalize_games_for_lotto645(self):
         if self._args.games is None:
-            self._args.games = ["x,x,x,x,x,x" for _ in range(5)]
-        else:
-            while len(self._args.games) < 5:
-                self._args.games.append(None)
+            self._args.games = [None for _ in range(5)]
 
         req_bucket = []
         for game in self._args.games:
-            if game is None:
-                req_bucket.append(game)
-            else:
-                req_slot = []
-                nums_and_asterisks = game.split(",")
-                for i in nums_and_asterisks:
-                    if i == "x":
-                        req_slot.append(i)
-                    else:
-                        req_slot.append(int(i))
-                req_bucket.append(req_slot)
+            req_bucket.append([] if game is None else [*map(int, game.split(","))])
 
         self._args.games = req_bucket
 
     def create_lotto645_req(self):
         return Lotto645BuyRequest(self._args.games)
```

### Comparing `dhapi-1.3.5/src/dhapi/router/router.py` & `dhapi-1.4.0/src/dhapi/router/router.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.5/src/dhapi/router/version_checker.py` & `dhapi-1.4.0/src/dhapi/router/version_checker.py`

 * *Files identical despite different names*

### Comparing `dhapi-1.3.5/src/dhapi.egg-info/SOURCES.txt` & `dhapi-1.4.0/src/dhapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

