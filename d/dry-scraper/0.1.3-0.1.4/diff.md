# Comparing `tmp/dry_scraper-0.1.3.tar.gz` & `tmp/dry_scraper-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dry_scraper-0.1.3.tar", max compression
+gzip compressed data, was "dry_scraper-0.1.4.tar", max compression
```

## Comparing `dry_scraper-0.1.3.tar` & `dry_scraper-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.3/LICENSE
--rw-r--r--   0        0        0       50 2022-12-05 04:14:04.570059 dry_scraper-0.1.3/README.md
--rw-r--r--   0        0        0      527 2023-01-12 23:02:52.253377 dry_scraper-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2706 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/data_source.py
--rw-r--r--   0        0        0      207 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/__init__.py
--rw-r--r--   0        0        0    16391 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/nhl_api_sources.py
--rw-r--r--   0        0        0      490 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_conferences_api_source.py
--rw-r--r--   0        0        0      848 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py
--rw-r--r--   0        0        0     5323 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py
--rw-r--r--   0        0        0     9928 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py
--rw-r--r--   0        0        0     1558 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py
--rw-r--r--   0        0        0     1140 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_schedule_api_source.py
--rw-r--r--   0        0        0     1830 2023-01-12 22:59:13.590036 dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py
--rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.3/src/dry_scraper/shared.py
--rw-r--r--   0        0        0    35587 2022-12-05 04:14:04.570059 dry_scraper-0.1.3/src/dry_scraper/teams.py
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 dry_scraper-0.1.3/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 dry_scraper-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/LICENSE
+-rw-r--r--   0        0        0       50 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/README.md
+-rw-r--r--   0        0        0      547 2023-05-14 23:37:10.035820 dry_scraper-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2704 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/data_source.py
+-rw-r--r--   0        0        0       87 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/__init__.py
+-rw-r--r--   0        0        0    14305 2023-05-14 23:33:44.497300 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/nhl_api_sources.py
+-rw-r--r--   0        0        0      490 2023-01-14 00:52:26.603584 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_conferences_api_source.py
+-rw-r--r--   0        0        0      848 2023-01-14 00:54:47.040256 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py
+-rw-r--r--   0        0        0     5323 2023-01-14 00:54:44.046922 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py
+-rw-r--r--   0        0        0    11296 2023-05-14 23:33:35.187214 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py
+-rw-r--r--   0        0        0     1558 2023-01-14 00:54:44.046922 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py
+-rw-r--r--   0        0        0     1938 2023-05-14 23:33:35.187214 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_schedule_api_source.py
+-rw-r--r--   0        0        0     1830 2023-01-14 00:52:26.603584 dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py
+-rw-r--r--   0        0        0    20946 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/src/dry_scraper/shared.py
+-rw-r--r--   0        0        0    35587 2022-12-05 04:14:04.570059 dry_scraper-0.1.4/src/dry_scraper/teams.py
+-rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 dry_scraper-0.1.4/PKG-INFO
```

### Comparing `dry_scraper-0.1.3/LICENSE` & `dry_scraper-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/pyproject.toml` & `dry_scraper-0.1.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "dry_scraper"
-version = "0.1.3"
+version = "0.1.4"
 description = "A framework for retrieving and parsing hockey data into useful forms."
 authors = ["cak <chris@cak.co>"]
 license = "GNU General Public License v3.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 beautifulsoup4 = "^4.11.1"
 pandas = "^1.4.3"
 requests = "^2.28.1"
 pydantic = "^1.10.2"
 uuid = "^1.30"
+fastapi = "^0.89.1"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/data_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import requests
 from abc import ABC
-from typing import ClassVar
+from typing import ClassVar, Self
 
 
 class DataSource(ABC):
     """
     Abstract class that represents an online data source.
 
     ...
@@ -55,15 +55,15 @@
     def url_stub(self) -> str:
         return self._url_stub
 
     @property
     def extension(self) -> str:
         return self._extension
 
-    def fetch_content(self):  # -> Self:
+    def fetch_content(self) -> Self:
         """
         Use requests.get to retrieve file at URL and store response in self.content
 
         Returns:
             self
         """
         try:
@@ -76,15 +76,15 @@
             print(errc)
         except requests.exceptions.Timeout as errt:
             print(errt)
         except requests.exceptions.RequestException as err:
             print(err)
         return self
 
-    def write_content(self, path: str, filename: str):  # -> Self:
+    def write_content(self, path: str, filename: str) -> Self:
         """Write content to {path}/{filename}.{self.extension}
 
         Args:
             filename (str): desired filename
             path (str): path to save location
         """
         full_path = os.path.join(path, f"{filename}.{self.extension}")
```

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_divisions_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_content_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_game_live_feed_api_source.py`

 * *Files 15% similar despite different names*

```diff
@@ -334,7 +334,59 @@
 
 class LiveFeed(BaseModel):
     game_pk: int = Field(alias="gamePk")
     link: LiveFeedLink
     metadata: Metadata = Field(alias="metaData")
     game_data: GameData = Field(alias="gameData")
     live_data: LiveData = Field(alias="liveData")
+
+
+pbp_df_model = {
+    "season": "int",
+    "gamePk": "int",
+    "home_team_id": "int",
+    "home_team_name": "str",
+    "home_team_tricode": "str",
+    "away_team_id": "int",
+    "away_team_name": "str",
+    "away_team_tricode": "str",
+    "event_idx": "int",
+    "event_id": "int",
+    "event": "str",
+    "event_code": "str",
+    "event_type_id": "str",
+    "description": "str",
+    "secondary_type": "str",
+    "game_winning_goal": "str",
+    "empty_net": "str",
+    "period": "int",
+    "period_type": "str",
+    "ordinal_num": "str",
+    "period_time": "str",
+    "period_time_remaining": "str",
+    "date_time": "str",
+    "goals_home": "int",
+    "goals_away": "int",
+    "coordinates_x": "int",
+    "coordinates_y": "int",
+    "strength_code": "str",
+    "strength_name": "str",
+    "player0_id": "int",
+    "player0_full_name": "str",
+    "player0_player_type": "str",
+    "player0_season_total": "int",
+    "player1_id": "int",
+    "player1_full_name": "str",
+    "player1_player_type": "str",
+    "player1_season_total": "int",
+    "player2_id": "int",
+    "player2_full_name": "str",
+    "player2_player_type": "str",
+    "player2_season_total": "int",
+    "player3_id": "int",
+    "player3_full_name": "str",
+    "player3_player_type": "str",
+    "player3_season_total": "int",
+    "team_id": "int",
+    "team_name": "str",
+    "team_tricode": "str",
+}
```

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_people_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py` & `dry_scraper-0.1.4/src/dry_scraper/data_sources/nhl/pydantic_models/nhl_teams_api_source.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/src/dry_scraper/shared.py` & `dry_scraper-0.1.4/src/dry_scraper/shared.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/src/dry_scraper/teams.py` & `dry_scraper-0.1.4/src/dry_scraper/teams.py`

 * *Files identical despite different names*

### Comparing `dry_scraper-0.1.3/PKG-INFO` & `dry_scraper-0.1.4/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: dry-scraper
-Version: 0.1.3
+Version: 0.1.4
 Summary: A framework for retrieving and parsing hockey data into useful forms.
 License: GNU General Public License v3.0
 Author: cak
 Author-email: chris@cak.co
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: fastapi (>=0.89.1,<0.90.0)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.2,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: uuid (>=1.30,<2.0)
 Description-Content-Type: text/markdown
 
 # dry_scraper
```

