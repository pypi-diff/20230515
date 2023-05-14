# Comparing `tmp/athletes_unlimited_py-0.0.4.tar.gz` & `tmp/athletes_unlimited_py-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "athletes_unlimited_py-0.0.4.tar", last modified: Wed May 10 18:15:50 2023, max compression
+gzip compressed data, was "athletes_unlimited_py-0.0.5.tar", last modified: Sun May 14 22:07:23 2023, max compression
```

## Comparing `athletes_unlimited_py-0.0.4.tar` & `athletes_unlimited_py-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:15:50.887481 athletes_unlimited_py-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-10 18:15:50.887481 athletes_unlimited_py-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:15:50.887481 athletes_unlimited_py-0.0.4/athetes_unlimited_py/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25042 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/aux_softball.py
--rw-r--r--   0 runner    (1001) docker     (123)    31448 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/basketball.py
--rw-r--r--   0 runner    (1001) docker     (123)    30883 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/lacrosse.py
--rw-r--r--   0 runner    (1001) docker     (123)    47203 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/softball.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21428 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/athetes_unlimited_py/volleyball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 18:15:50.887481 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-10 18:15:50.000000 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-10 18:15:50.000000 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 18:15:50.000000 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 18:15:50.000000 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 18:15:50.000000 athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-10 18:15:28.000000 athletes_unlimited_py-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 18:15:50.887481 athletes_unlimited_py-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/athetes_unlimited_py/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26277 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/aux_softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31440 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/basketball.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30879 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/lacrosse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47197 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/softball.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30686 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/athetes_unlimited_py/volleyball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-14 22:07:23.000000 athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-14 22:06:53.000000 athletes_unlimited_py-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 22:07:23.595607 athletes_unlimited_py-0.0.5/setup.cfg
```

### Comparing `athletes_unlimited_py-0.0.4/LICENSE` & `athletes_unlimited_py-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.4/PKG-INFO` & `athletes_unlimited_py-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes_unlimited_py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.4/README.md` & `athletes_unlimited_py-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/aux_softball.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/aux_softball.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,89 +6,93 @@
 import requests
 from tqdm import tqdm
 
 from athetes_unlimited_py.softball import get_au_softball_game_stats, get_au_softball_pbp
 from athetes_unlimited_py.utils import raise_html_status_code
 
 
-def get_aux_softball_season_id(season:int) -> int:
+def get_aux_softball_season_id(season: int) -> int:
     """
     Given a season, `get_au_softball_season_id()` returns the proper season ID for the Athletes Unlimited softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The season you want a season ID for softball. 
         If there isn't a season ID for the inputted `season`, a `ValueError()` exception will be raised.
-    
+
     Returns
     ----------
     The proper season ID corresponding to an Athletes Unlimited softball season.
     """
     seasonId = 0
-    
+
     if season == 2022:
         seasonId = 39
-        return seasonId 
+        return seasonId
     elif season == 2023:
         seasonId = 106
-        return seasonId 
+        return seasonId
     else:
-        raise ValueError(f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season}')
+        raise ValueError(
+            f'[season] can only be 2022 or 2023 at this time for softball.\nYou entered :\n\t{season}')
 
 
 ############################################################################################################################################################################################################################################################
 ##
-## Season Functions
+# Season Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_aux_softball_season_pbp(season:int) -> pd.DataFrame():
+def get_aux_softball_season_pbp(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all play-by-play (PBP) data for an AU softball season.
-    
+
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want PBP data from.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data from a AU season.
 
     """
     season_pbp_df = pd.DataFrame()
     seasonId = get_aux_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_pbp(seasonId,j)
+                game_df = get_au_softball_pbp(seasonId, j)
 
-                season_pbp_df = pd.concat([season_pbp_df,game_df],ignore_index=True)
+                season_pbp_df = pd.concat(
+                    [season_pbp_df, game_df], ignore_index=True)
                 del game_df
 
     return season_pbp_df
 
-def get_aux_softball_season_player_box(season:int) -> pd.DataFrame():
+
+def get_aux_softball_season_player_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all box-score game stats for an AU softball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -98,41 +102,45 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     seasonId = get_aux_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+            for j in tqdm(range(1, len_game_ids+1)):
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=False)
+                game_df = get_au_softball_game_stats(
+                    seasonId, j, get_team_stats=False)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     season_stats_df['sport'] = 'aux_softball'
     return season_stats_df
 
-def get_aux_softball_season_team_box(season:int) -> pd.DataFrame():
+
+def get_aux_softball_season_team_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get and parse all box-score game stats for an AU softball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -142,66 +150,70 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     seasonId = get_aux_softball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/softball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+            for j in tqdm(range(1, len_game_ids+1)):
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=True)
+                game_df = get_au_softball_game_stats(
+                    seasonId, j, get_team_stats=True)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     season_stats_df['sport'] = 'aux_softball'
 
     return season_stats_df
 
 ############################################################################################################################################################################################################################################################
 ##
-## Season Stats
+# Season Stats
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_aux_softball_season_player_stats(season:int) -> pd.DataFrame():
+
+def get_aux_softball_season_player_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get all season player stats for an AU softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want season player stats from.
 
     Returns
     ----------
     A pandas DataFrame containing season player stats a AU season.
 
     """
     game_stats_df = get_aux_softball_season_player_box(season)
-    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber', 
-    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',    
+    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber',
+    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',
     #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
-    #    'first_name', 'last_name', 'full_name', 'week', 'game_num', 
+    #    'first_name', 'last_name', 'full_name', 'week', 'game_num',
     #    'season_type', 'G', 'GS', 'batting_PA', 'batting_AB', 'batting_R',
     #    'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
     #    'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
     #    'batting_CS', 'batting_BA', 'batting_OBP', 'batting_SLG', 'batting_TB',
     #    'batting_SF', 'batting_SH', 'AU_POINTS', 'pitching_W', 'pitching_L',
     #    'pitching_ERA', 'pitching_SHO', 'pitching_CG', 'pitching_SV',
     #    'pitching_IP_str', 'pitching_IP', 'pitching_H', 'pitching_R',
@@ -210,130 +222,153 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId', 
-        'first_name', 'last_name', 'full_name'],as_index=False)[[
-        'G', 'GS', 'AU_POINTS',
-        'batting_PA', 'batting_AB', 'batting_R',
-        'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
-        'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
-        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 
-        'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
-        'pitching_SV', 'pitching_IP', 
-        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 
-        'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
-        'pitching_PI_strikes',
-        'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
-        'fielding_CS', 'fielding_TC'
-    ]].sum()
+    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                             'G', 'GS', 'AU_POINTS',
+                                             'batting_PA', 'batting_AB', 'batting_R',
+                                             'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
+                                             'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
+                                             'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
+                                             'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
+                                             'pitching_SV', 'pitching_IP',
+                                             'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
+                                             'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
+                                             'pitching_PI_strikes',
+                                             'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
+                                             'fielding_CS', 'fielding_TC'
+                                         ]].sum()
 
-    finished_df[['G', 'GS', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']] = finished_df[['G', 'GS', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV','pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']].astype('int')
+    finished_df[['G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+        'G', 'GS', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
     finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    ## Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1, 'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+    # Batting
+    finished_df.loc[finished_df['batting_AB'] >= 1,
+                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
     finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
     finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
     finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
     finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
 
     finished_df['batting_OPS+'] = None
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SecA'] = (finished_df['batting_BB'] + (finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
     finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
     finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
     finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_ISO'] = (finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
     finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
     finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
 
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0),'batting_PSN'] = (2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
     finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
 
-    ## Pitching
-    finished_df['pitching_ERA'] = 9 * (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+    # Pitching
+    finished_df['pitching_ERA'] = 9 * \
+        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
     finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
 
     finished_df['pitching_ERA+'] = None
     finished_df['pitching_FIP'] = None
     finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_WHIP'] = (
+        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
 
-    finished_df['pitching_H9'] = (9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_H9'] = (
+        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
 
-    finished_df['pitching_HR9'] = (9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+    finished_df['pitching_HR9'] = (
+        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
     finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
 
-    finished_df['pitching_BB9'] = (9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+    finished_df['pitching_BB9'] = (
+        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
     finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
 
-    finished_df['pitching_SO9'] = (9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+    finished_df['pitching_SO9'] = (
+        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
     finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
 
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / finished_df['pitching_BB']
+    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+        finished_df['pitching_BB']
     finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
 
-    finished_df['pitching_RA9'] = 9 * (finished_df['pitching_R'] / finished_df['pitching_IP'])
+    finished_df['pitching_RA9'] = 9 * \
+        (finished_df['pitching_R'] / finished_df['pitching_IP'])
     finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-    
-    ## Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+
+    # Fielding
+    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
     finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
 
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E']
+    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+        finished_df['fielding_A'] + finished_df['fielding_E']
     finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
 
-    #finished_df['fielding_CS%'] = 0
-    #finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+    # finished_df['fielding_CS%'] = 0
+    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
 
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] + finished_df['fielding_A'])) / finished_df['fielding_IP']
+    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
     finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
 
     # finished_df.to_csv('test.csv')
     # print(finished_df)
     # print(game_stats_df.columns)
     return finished_df
 
-def get_aux_softball_season_team_stats(season:int) -> pd.DataFrame():
+
+def get_aux_softball_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) softball season, get all season team stats for an AU softball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU softball season you want season player stats from.
 
     Returns
     ----------
     A pandas DataFrame containing season player stats a AU season.
 
     """
     game_stats_df = get_aux_softball_season_player_box(season)
-    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber', 
-    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',    
+    # ['sport', 'api_version', 'season', 'seasonId', 'weekNumber',
+    #    'gameNumber', 'seasonType', 'playerId', 'uniformNumber',
     #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
-    #    'first_name', 'last_name', 'full_name', 'week', 'game_num', 
+    #    'first_name', 'last_name', 'full_name', 'week', 'game_num',
     #    'season_type', 'G', 'GS', 'batting_PA', 'batting_AB', 'batting_R',
     #    'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
     #    'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
     #    'batting_CS', 'batting_BA', 'batting_OBP', 'batting_SLG', 'batting_TB',
     #    'batting_SF', 'batting_SH', 'AU_POINTS', 'pitching_W', 'pitching_L',
     #    'pitching_ERA', 'pitching_SHO', 'pitching_CG', 'pitching_SV',
     #    'pitching_IP_str', 'pitching_IP', 'pitching_H', 'pitching_R',
@@ -342,102 +377,124 @@
     #    'pitching_HR9', 'pitching_BB9', 'pitching_SO9', 'pitching_SO/BB',
     #    'pitching_RA9', 'pitching_PI', 'pitching_PI_balls',
     #    'pitching_PI_strikes', 'fielding_position', 'fielding_IP_str',
     #    'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
     #    'fielding_FLD%', 'fielding_CS', 'fielding_CS%', 'fielding_TC',
     #    'fielding_CH', 'fielding_RF/9']
 
-    finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId','teamId'],as_index=False)[[
+    finished_df = game_stats_df.groupby(['sport', 'api_version', 'season', 'seasonId', 'teamId'], as_index=False)[[
         'G', 'AU_POINTS',
         'batting_PA', 'batting_AB', 'batting_R',
         'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI',
         'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA',
-        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 
+        'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH',
         'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS',
-        'pitching_SV', 'pitching_IP', 
-        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 
+        'pitching_SV', 'pitching_IP',
+        'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB',
         'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls',
         'pitching_PI_strikes',
         'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP',
         'fielding_CS', 'fielding_TC'
     ]].sum()
 
-    finished_df[['G',  'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']] = finished_df[['G', 'AU_POINTS','batting_PA', 'batting_AB', 'batting_R','batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI','batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA','batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS','pitching_SV','pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls','pitching_PI_strikes','fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP','fielding_CS', 'fielding_TC']].astype('int')
+    finished_df[['G',  'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']] = finished_df[[
+        'G', 'AU_POINTS', 'batting_PA', 'batting_AB', 'batting_R', 'batting_H', 'batting_2B', 'batting_3B', 'batting_HR', 'batting_RBI', 'batting_BB', 'batting_HBP', 'batting_K', 'batting_SB', 'batting_SBA', 'batting_CS', 'batting_TB', 'batting_SF', 'batting_SH', 'pitching_W', 'pitching_L', 'pitching_SHO', 'pitching_CG', 'pitching_QS', 'pitching_SV', 'pitching_H', 'pitching_R', 'pitching_ER', 'pitching_HR', 'pitching_BB', 'pitching_SO', 'pitching_HBP', 'pitching_WP', 'pitching_PI', 'pitching_PI_balls', 'pitching_PI_strikes', 'fielding_IP', 'fielding_PO', 'fielding_A', 'fielding_E', 'fielding_DP', 'fielding_CS', 'fielding_TC']].astype('int')
     finished_df['pitching_IP'] = finished_df['pitching_IP'].astype('float')
-    ## Batting
-    finished_df.loc[finished_df['batting_AB'] >= 1, 'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
+    # Batting
+    finished_df.loc[finished_df['batting_AB'] >= 1,
+                    'batting_BA'] = finished_df['batting_H'] / finished_df['batting_AB']
     finished_df['batting_BA'] = finished_df['batting_BA'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_OBP'] = (finished_df['batting_H'] + finished_df['batting_BB'] + finished_df['batting_HBP']) / (
+        finished_df['batting_AB'] + finished_df['batting_BB'] + finished_df['batting_HBP'] + finished_df['batting_SF'])
     finished_df['batting_OBP'] = finished_df['batting_OBP'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_SLG'] = finished_df['batting_TB'] / finished_df['batting_AB']
     finished_df['batting_SLG'] = finished_df['batting_SLG'].round(3)
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
+    finished_df.loc[finished_df['batting_AB'] > 0,
+                    'batting_OPS'] = finished_df['batting_OBP'] + finished_df['batting_SLG']
     finished_df['batting_OPS'] = finished_df['batting_OPS'].round(3)
 
     finished_df['batting_OPS+'] = None
 
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_SecA'] = (finished_df['batting_BB'] + (finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_SecA'] = (finished_df['batting_BB'] + (
+        finished_df['batting_TB'] - finished_df['batting_H']) + (finished_df['batting_SB'] - finished_df['batting_CS'])) / finished_df['batting_AB']
     finished_df['batting_SecA'] = finished_df['batting_SecA'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_BB%'] = finished_df['batting_BB'] / finished_df['batting_PA']
     finished_df['batting_BB%'] = finished_df['batting_BB%'].round(3)
 
-    finished_df.loc[finished_df['batting_PA'] > 0,'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
+    finished_df.loc[finished_df['batting_PA'] > 0,
+                    'batting_K%'] = finished_df['batting_K'] / finished_df['batting_PA']
     finished_df['batting_K%'] = finished_df['batting_K%'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_ISO'] = (finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_ISO'] = (
+        finished_df['batting_TB'] - finished_df['batting_H']) / finished_df['batting_AB']
     finished_df['batting_ISO'] = finished_df['batting_ISO'].round(3)
-    
-    finished_df.loc[finished_df['batting_AB'] > 0,'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
+
+    finished_df.loc[finished_df['batting_AB'] > 0, 'batting_BABIP'] = (finished_df['batting_H'] + finished_df['batting_HR']) / (
+        finished_df['batting_AB'] - finished_df['batting_K'] - finished_df['batting_HR'] + finished_df['batting_SF'])
     finished_df['batting_BABIP'] = finished_df['batting_BABIP'].round(3)
 
-    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0),'batting_PSN'] = (2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
+    finished_df.loc[(finished_df['batting_SB'] > 0) | (finished_df['batting_HR'] > 0), 'batting_PSN'] = (
+        2 * finished_df['batting_HR'] * finished_df['batting_SB']) / (finished_df['batting_HR'] * finished_df['batting_SB'])
     finished_df['batting_PSN'] = finished_df['batting_PSN'].round(3)
 
-    ## Pitching
-    finished_df['pitching_ERA'] = 9 * (finished_df['pitching_ER'] / finished_df['pitching_IP'])
+    # Pitching
+    finished_df['pitching_ERA'] = 9 * \
+        (finished_df['pitching_ER'] / finished_df['pitching_IP'])
     finished_df['pitching_ERA'] = finished_df['pitching_ERA'].round(3)
 
     finished_df['pitching_ERA+'] = None
     finished_df['pitching_FIP'] = None
     finished_df['pitching_FIP-'] = None
-    finished_df['pitching_WHIP'] = (finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_WHIP'] = (
+        finished_df['pitching_BB'] + finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_WHIP'] = finished_df['pitching_WHIP'].round(3)
 
-    finished_df['pitching_H9'] = (9 * finished_df['pitching_H']) / finished_df['pitching_IP']
+    finished_df['pitching_H9'] = (
+        9 * finished_df['pitching_H']) / finished_df['pitching_IP']
     finished_df['pitching_H9'] = finished_df['pitching_H9'].round(3)
 
-    finished_df['pitching_HR9'] = (9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
+    finished_df['pitching_HR9'] = (
+        9 * finished_df['pitching_HR']) / finished_df['pitching_IP']
     finished_df['pitching_HR9'] = finished_df['pitching_HR9'].round(3)
 
-    finished_df['pitching_BB9'] = (9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
+    finished_df['pitching_BB9'] = (
+        9 * finished_df['pitching_BB']) / finished_df['pitching_IP']
     finished_df['pitching_BB9'] = finished_df['pitching_BB9'].round(3)
 
-    finished_df['pitching_SO9'] = (9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
+    finished_df['pitching_SO9'] = (
+        9 * finished_df['pitching_SO']) / finished_df['pitching_IP']
     finished_df['pitching_SO9'] = finished_df['pitching_SO9'].round(3)
 
-    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / finished_df['pitching_BB']
+    finished_df['pitching_SO/BB'] = finished_df['pitching_SO'] / \
+        finished_df['pitching_BB']
     finished_df['pitching_SO/BB'] = finished_df['pitching_SO/BB'].round(3)
 
-    finished_df['pitching_RA9'] = 9 * (finished_df['pitching_R'] / finished_df['pitching_IP'])
+    finished_df['pitching_RA9'] = 9 * \
+        (finished_df['pitching_R'] / finished_df['pitching_IP'])
     finished_df['pitching_RA9'] = finished_df['pitching_RA9'].round(3)
-    
-    ## Fielding
-    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
+
+    # Fielding
+    finished_df['fielding_FLD%'] = (finished_df['fielding_PO'] + finished_df['fielding_A']) / (
+        finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E'])
     finished_df['fielding_FLD%'] = finished_df['fielding_FLD%'].round(3)
 
-    finished_df['fielding_CH'] = finished_df['fielding_PO'] + finished_df['fielding_A'] + finished_df['fielding_E']
+    finished_df['fielding_CH'] = finished_df['fielding_PO'] + \
+        finished_df['fielding_A'] + finished_df['fielding_E']
     finished_df['fielding_CH'] = finished_df['fielding_CH'].round(3)
 
-    #finished_df['fielding_CS%'] = 0
-    #finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
+    # finished_df['fielding_CS%'] = 0
+    # finished_df['fielding_CS%'] = finished_df['fielding_CS%'].round(3)
 
-    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] + finished_df['fielding_A'])) / finished_df['fielding_IP']
+    finished_df['fielding_RF/9'] = (9 * (finished_df['fielding_PO'] +
+                                    finished_df['fielding_A'])) / finished_df['fielding_IP']
     finished_df['fielding_RF/9'] = finished_df['fielding_RF/9'].round(3)
 
     # finished_df.to_csv('test.csv')
     # print(finished_df)
     # print(game_stats_df.columns)
     return finished_df
```

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/basketball.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/basketball.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
 
     for i in tqdm(sport_json_data['data']):
         # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_basketball_pbp(season, j)
@@ -479,15 +479,15 @@
     sport_json_data = json.loads(response.text)
 
     for i in sport_json_data['data']:
         # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1, len_game_ids+1)):
+            for j in tqdm(range(1, len_game_ids)):
                 # print(f'\nOn game ID {j} for the {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
@@ -526,15 +526,15 @@
 
     for i in tqdm(sport_json_data['data']):
         # print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1, len_game_ids+1)):
-                # print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_basketball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_basketball_game_stats(
```

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/lacrosse.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/lacrosse.py`

 * *Files 2% similar despite different names*

```diff
@@ -464,15 +464,15 @@
 
     for i in sport_json_data['data']:
         # print(i)
         if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1, len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_lacrosse_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_lacrosse_game_stats(season_id, j)
@@ -510,15 +510,15 @@
 
     for i in sport_json_data['data']:
         # print(i)
         if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1, len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_lacrosse_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_lacrosse_game_stats(
@@ -533,15 +533,15 @@
 ############################################################################################################################################################################################################################################################
 ##
 # Season Stats
 ##
 ############################################################################################################################################################################################################################################################
 
 
-def get_au_softball_season_player_stats(season: int) -> pd.DataFrame():
+def get_au_lacrosse_season_player_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) lacrosse season, get all season player stats for an AU lacrosse season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU lacrosse season you want season player stats from.
@@ -607,15 +607,15 @@
     finished_df['goalie_savePct'] = finished_df['goalie_goalsAgainst'] / \
         finished_df['goalie_shotsFaced']
     finished_df['goalie_savePct'] = finished_df['goalie_savePct'].round(3)
 
     return finished_df
 
 
-def get_au_softball_season_team_stats(season: int) -> pd.DataFrame():
+def get_au_lacrosse_season_team_stats(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) lacrosse season, get all season team stats for an AU lacrosse season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The AU lacrosse season you want season team stats from.
```

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/softball.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/softball.py`

 * *Files 0% similar despite different names*

```diff
@@ -518,15 +518,15 @@
     
     for i in sport_json_data['data']:
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(i['gameIds']):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_softball_pbp(seasonId,j)
@@ -561,15 +561,15 @@
     
     for i in sport_json_data['data']:
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=False)
@@ -604,15 +604,15 @@
     
     for i in sport_json_data['data']:
         #print(i)
         if i['seasonId'] == seasonId:
             len_game_ids = len(i['gameIds'])
 
             for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_softball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
                 game_df = get_au_softball_game_stats(seasonId,j,get_team_stats=True)
```

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/utils.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/utils.py`

 * *Files identical despite different names*

### Comparing `athletes_unlimited_py-0.0.4/athetes_unlimited_py/volleyball.py` & `athletes_unlimited_py-0.0.5/athetes_unlimited_py/volleyball.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,168 +1,178 @@
 import json
 import time
-#from urllib.request import urlopen
+# from urllib.request import urlopen
 
 import pandas as pd
 import requests
 from tqdm import tqdm
 
 from athetes_unlimited_py.utils import raise_html_status_code
 
 ############################################################################################################################################################################################################################################################
 ##
-## Volleyball-only utilities
+# Volleyball-only utilities
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_volleyball_season(season_id:int) -> int:
+
+def get_au_volleyball_season(season_id: int) -> int:
     """
     Given a season ID, `get_au_volleyball_season()` returns the proper season for the corresponding Athletes Unlimited volleyball season.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The season ID you want a season for in Athletes Unlimited volleyball. 
         If there isn't a season for the inputted `season_id`, a `ValueError()` exception will be raised.
-    
+
     Returns
     ----------
     The proper season corresponding to an Athletes Unlimited volleyball season ID.
     """
     season = 0
-    
+
     if season_id == 3:
         season = 2021
-        return season 
+        return season
     elif season_id == 11:
         season = 2022
         return season
     elif season_id == 138:
         season = 2023
-        return season 
+        return season
     else:
-        raise ValueError(f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
+        raise ValueError(
+            f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
 
-def get_au_volleyball_season_id(season:int) -> int:
+
+def get_au_volleyball_season_id(season: int) -> int:
     """
     Given a season, `get_au_volleyball_season_id()` returns the proper season ID for the Athletes Unlimited volleyball season.
 
     Parameters
     ----------
     `season` (int, mandatory):
         The season you want a season ID for volleyball. 
         If there isn't a season ID for the inputted `season`, a `ValueError()` exception will be raised.
-    
+
     Returns
     ----------
     The proper season ID corresponding to an Athletes Unlimited volleyball season.
     """
     seasonId = 0
-    
+
     if season == 2021:
         seasonId = 3
-        return seasonId 
+        return seasonId
     elif season == 2022:
         seasonId = 11
-        return seasonId 
+        return seasonId
     elif season == 2023:
         seasonId = 138
-        return seasonId 
+        return seasonId
     else:
-        raise ValueError(f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
+        raise ValueError(
+            f'[season] can only be 2021, 2022, or 2023 at this time for volleyball.\nYou entered :\n\t{season}')
 
 ############################################################################################################################################################################################################################################################
 ##
-## Game Functions
+# Game Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_volleyball_game_stats(season_id:int,game_num:int,get_team_stats=False,get_player_and_team_stats=False,rename_cols=False) -> pd.DataFrame():
+
+def get_au_volleyball_game_stats(season_id: int, game_num: int, get_team_stats=False, get_player_and_team_stats=False, rename_cols=False) -> pd.DataFrame():
     """
     Retrieves the player and/or team game stats for an Atheltes Unlimited (AU) volleyball game.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The AU volleyball season ID you want a game from.
-    
+
     `game_num` (int, mandatory):
         The game number you want player and/or team stats from.
         This is not the game ID!
         A `ValueError` will be raised if `game_num` is set to less than 1.
-    
+
     `get_team_stats` (bool, optional) = False:
         Optional boolean argument. 
         If set to `True`, the pandas DataFrame returned by `get_volleyball_game_stats()` will only return team stats for that game, 
         and will not return player stats, unless `get_player_and_team_stats` is set to `True` if `get_team_stats` is set to `True`.
-    
+
     `get_player_and_team_stats` (bool, optional) = False:
 
     `rename_cols` (bool, optional) = False:
         NOT IMPLEMENTED YET!
         `get_volleyball_game_stats()` will have no change in functionality at this time if `rename_cols` is set to `True`.
-        
+
 
     Returns
     ----------
     A pandas DataFrame containing player and/or team stats for a given AU game within a given AU season ID.
     """
 
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     player_stats_df = pd.DataFrame()
     team_stats_df = pd.DataFrame()
     row_df = pd.DataFrame()
 
     if game_num < 1:
         raise ValueError('`game_num` cannot be less than 0.')
-    
-    key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+
+    # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+    key = int(time.time())
     url = f"https://auprosports.com/proxy.php?request=/api/stats/volleyball/v1/{season_id}/by-game/{game_num}?statType=volleyball%26k={key}"
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     raise_html_status_code(response.status_code)
-    
+
     json_data = json.loads(response.text)
 
     sport = json_data['metaSport']['sport']
     api_version = json_data['metaSport']['version']
 
     for i in tqdm(json_data['data']):
-        row_df = pd.DataFrame({'sport':sport,'api_version':api_version},index=[0])
-        
+        row_df = pd.DataFrame(
+            {'sport': sport, 'api_version': api_version}, index=[0])
+
         ##############################################################################################################################
-        ## Player/Team info
+        # Player/Team info
         ##############################################################################################################################
         row_df['season'] = get_au_volleyball_season(i['seasonId'])
         row_df['seasonId'] = i['seasonId']
-        row_df['weekNumber'] = 0
-        row_df['gameNumber'] = 0
-        row_df['seasonType'] = ""
+        row_df['week_number'] = 0
+        row_df['game_number'] = 0
+        row_df['season_type'] = ""
 
         row_df['playerId'] = i['playerId']
         row_df['uniformNumber'] = i['uniformNumber']
         row_df['uniformNumberDisplay'] = str(i['uniformNumberDisplay'])
-        
+
         row_df['primaryPositionLk'] = i['primaryPositionLk']
         row_df['secondaryPositionLk'] = i['secondaryPositionLk']
-        row_df['first_name'] = str(i['firstName']).replace('\u2019','\'')
-        row_df['last_name'] = str(i['lastName']).replace('\u2019','\'')
-        row_df['full_name'] = f"{i['firstName']} {i['lastName']}".replace('\u2019','\'')
+        row_df['first_name'] = str(i['firstName']).replace('\u2019', '\'')
+        row_df['last_name'] = str(i['lastName']).replace('\u2019', '\'')
+        row_df['full_name'] = f"{i['firstName']} {i['lastName']}".replace(
+            '\u2019', '\'')
 
         ##############################################################################################################################
-        ## Player/Team stats
+        # Player/Team stats
         ##############################################################################################################################
         row_df['player_id'] = i['stats'][0]['playerId']
         row_df['first_name'] = i['stats'][0]['firstName']
         row_df['last_name'] = i['stats'][0]['lastName']
         row_df['uniform_number'] = i['stats'][0]['uniformNumber']
-        row_df['uniform_number_display'] = str(i['stats'][0]['uniformNumberDisplay'])
+        row_df['uniform_number_display'] = str(
+            i['stats'][0]['uniformNumberDisplay'])
         row_df['primary_position_lk'] = i['stats'][0]['primaryPositionLk']
         row_df['secondary_position_lk'] = i['stats'][0]['secondaryPositionLk']
-        row_df['team_id'] = i['stats'][0]['teamId']
+        row_df['team_id'] = i['teamId']
         row_df['sets_played'] = i['stats'][0]['setsPlayed']
         row_df['player_id'] = i['stats'][0]['playerId']
         row_df['kills'] = i['stats'][0]['kills']
         row_df['kills_per_set'] = i['stats'][0]['killsPerSet']
         row_df['attack_errors'] = i['stats'][0]['attackErrors']
         row_df['attack_attempts'] = i['stats'][0]['attackAttempts']
         row_df['attack_percentage'] = i['stats'][0]['attackPercentage']
@@ -180,96 +190,101 @@
         row_df['blocks'] = i['stats'][0]['blocks']
         row_df['blocks_per_set'] = i['stats'][0]['blocksPerSet']
         row_df['au_total_points'] = i['stats'][0]['auTotalPoints']
         row_df['week_number'] = i['stats'][0]['weekNumber']
         row_df['game_number'] = i['stats'][0]['gameNumber']
         row_df['season_type'] = i['stats'][0]['seasonType']
 
-
         ##############################################################################################################################
-        ## Save the data to the correct DataFrame
+        # Save the data to the correct DataFrame
         ##############################################################################################################################
 
         if i['type'] == "Team":
-            team_stats_df = pd.concat([team_stats_df,row_df],ignore_index=True)
+            team_stats_df = pd.concat(
+                [team_stats_df, row_df], ignore_index=True)
         else:
-            player_stats_df = pd.concat([player_stats_df,row_df],ignore_index=True)
+            player_stats_df = pd.concat(
+                [player_stats_df, row_df], ignore_index=True)
 
         row_df['type'] = i['type']
         row_df['teamId'] = i['teamId']
 
         if i['homeTeamFlg'] == True:
             row_df['homeTeamFlg'] = 1
         else:
             row_df['homeTeamFlg'] = 0
 
         del row_df
 
     ##############################################################################################################################
-    ## Once we're done, return the correct dataframe.
+    # Once we're done, return the correct dataframe.
     ##############################################################################################################################
-    
+
     if get_player_and_team_stats == True:
-        stats_df = pd.concat([player_stats_df,team_stats_df],ignore_index=True)
-        del player_stats_df,team_stats_df
+        stats_df = pd.concat(
+            [player_stats_df, team_stats_df], ignore_index=True)
+        del player_stats_df, team_stats_df
         return stats_df
-    elif get_team_stats == True:        
+    elif get_team_stats == True:
         del player_stats_df
         return team_stats_df
     else:
         del team_stats_df
         return player_stats_df
 
-def get_au_volleyball_pbp(season_id:int,game_id:int,return_participation_data=False) -> pd.DataFrame():
+
+def get_au_volleyball_pbp(season_id: int, game_id: int, return_participation_data=False) -> pd.DataFrame():
     """
     Retrieves the play-by-play (PBP) data for an Atheltes Unlimited (AU) volleyball game.
 
     Parameters
     ----------
     `season_id` (int, mandatory):
         The AU volleyball season ID you want a game from.
-    
+
     `game_id` (int, mandatory):
         The AU volleyball game ID you want PBP data from.
-    
+
     `return_participation_data` (bool, optional) = `False`:
         Optional argument. 
         If set to `True`, `get_au_volleyball_pbp()` will return a secondary pandas DataFrame
         containing roster information for this AU volleyball game.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data for a given AU game ID within a given AU season ID.
     If `return_participation_data` is set to `True`, an additional pandas DataFrame containing roster data for this game will be returned as well.
     """
 
     # season_id = get_au_volleyball_season_id(season)
     season = get_au_volleyball_season(season_id)
 
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
     game_pbp_df = pd.DataFrame()
     roster_df = pd.DataFrame()
     row_df = pd.DataFrame()
-        
+
     if game_id < 1:
         raise ValueError('`game_id` cannot be less than 0.')
-    
-    key = int(time.time()) # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+
+    # Yes, the key is literaly the int of the Epoch time at the time of the GET request.
+    key = int(time.time())
     url = f"https://auprosports.com/proxy.php?request=/api/play-by-play/volleyball/v1/event/{season_id}/game/{game_id}?k={key}"
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     raise_html_status_code(response.status_code)
-    
 
     json_data = json.loads(response.text)
 
     del headers, key
-    #print(json_data)
+    # print(json_data)
     for i in tqdm(json_data['data'][0]['plays']):
-        row_df = pd.DataFrame({'season':season,'game_id':game_id},index=[0])
+        row_df = pd.DataFrame(
+            {'season': season, 'game_id': game_id}, index=[0])
 
         row_df['game_number'] = i['gameNumber']
         row_df['game_id'] = i['gameId']
         row_df['play_seq_num'] = i['playSeqno']
         row_df['narrative_formatted'] = i['narrativeFormatted']
         row_df['start_time'] = i['startTime']
         row_df['end_time'] = i['endTime']
@@ -297,33 +312,33 @@
         row_df['set_continue'] = i['setContinue']
         row_df['home_team_id'] = i['homeTeamId']
         row_df['home_team_score'] = i['homeTeamScore']
         row_df['away_team_id'] = i['awayTeamId']
         row_df['away_team_Score'] = i['awayTeamScore']
         row_df['scoring_team_id'] = i['scoringTeamId']
 
-        game_pbp_df = pd.concat([game_pbp_df,row_df])
+        game_pbp_df = pd.concat([game_pbp_df, row_df])
         del row_df
-    
+
     if return_participation_data == True:
-        
+
         for i in json_data['data'][0]['competitors']:
 
             competitor_id = i['competitorId']
             competitor_color = i['color']
             competitor_name = i['name']
-            
+
             for j in i['players']:
                 row_df = pd.DataFrame({
-                        'season':season,
-                        'game_id':game_id,
-                        'competitor_id':competitor_id,
-                        'competitor_color':competitor_color,
-                        'competitor_name':competitor_name
-                    },
+                    'season': season,
+                    'game_id': game_id,
+                    'competitor_id': competitor_id,
+                    'competitor_color': competitor_color,
+                    'competitor_name': competitor_name
+                },
                     index=[0]
                 )
 
                 row_df['competitor_id'] = j['competitorId']
                 row_df['player_id'] = j['playerId']
                 row_df['captain_flag'] = j['captainFlg']
                 row_df['display_name'] = j['displayName']
@@ -338,73 +353,77 @@
                 row_df['has_voted_flag'] = j['hasVotedFlg']
                 row_df['uniform_number'] = str(j['uniformNumber'])
                 row_df['is_nominated_flag'] = j['isNominatedFlg']
                 row_df['nominated_flag'] = j['nominatedFlg']
                 row_df['player_url'] = j['resourceUrl']
                 row_df['image_url'] = j['imageResource']['imageUrl']
 
-                roster_df = pd.concat([roster_df,row_df],ignore_index=True)
+                roster_df = pd.concat([roster_df, row_df], ignore_index=True)
             del row_df
 
         del json_data
-        return game_pbp_df,roster_df
-    
+        return game_pbp_df, roster_df
+
     else:
         del json_data, roster_df
         return game_pbp_df
 
 ############################################################################################################################################################################################################################################################
 ##
-## Season Functions
+# Season Functions
 ##
 ############################################################################################################################################################################################################################################################
 
-def get_au_volleyball_season_pbp(season:int) -> pd.DataFrame():
+
+def get_au_volleyball_season_pbp(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) volleyball season, get and parse all play-by-play (PBP) data for an AU volleyball season.
-    
+
     Parameters
     ----------
     `season` (int, mandatory):
         The AU volleyball season you want PBP data from.
 
     Returns
     ----------
     A pandas DataFrame containing PBP data from a AU season.
 
     """
     season_pbp_df = pd.DataFrame()
     season_id = get_au_volleyball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/111.0.0.0 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == season_id:
             # len_game_ids = len(i['gameIds'])
 
             for j in tqdm(i['gameIds']):
                 print(f'\nOn game ID {j} in {season}.')
                 # try:
                 #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_volleyball_pbp(season_id,j)
+                game_df = get_au_volleyball_pbp(season_id, j)
 
-                season_pbp_df = pd.concat([season_pbp_df,game_df],ignore_index=True)
+                season_pbp_df = pd.concat(
+                    [season_pbp_df, game_df], ignore_index=True)
                 del game_df
 
     return season_pbp_df
 
-def get_au_volleyball_season_player_box(season:int) -> pd.DataFrame():
+
+def get_au_volleyball_season_player_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) volleyball season, get and parse all box-score game stats for an AU volleyball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -414,40 +433,43 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     season_id = get_au_volleyball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+            for j in tqdm(range(1, len_game_ids+1)):
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_volleyball_game_stats(season_id,j)
+                game_df = get_au_volleyball_game_stats(season_id, j)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     return season_stats_df
 
-def get_au_volleyball_season_team_box(season:int) -> pd.DataFrame():
+
+def get_au_volleyball_season_team_box(season: int) -> pd.DataFrame():
     """
     Given an Atheltes Unlimited (AU) volleyball season, get and parse all box-score game stats for an AU volleyball season.
     This returns all player game stats, and does not return season stats or game averages.
 
     Parameters
     ----------
     `season` (int, mandatory):
@@ -457,32 +479,212 @@
     ----------
     A pandas DataFrame containing player box score stats a AU season.
 
     """
     season_stats_df = pd.DataFrame()
     season_id = get_au_volleyball_season_id(season)
     url = "https://auprosports.com/proxy.php?request=api/seasons/volleyball/v1"
-    headers = {"User-Agent":"Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
+    headers = {
+        "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_4) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/83.0.4103.97 Safari/537.36"}
 
-    response = requests.get(url,headers=headers)
+    response = requests.get(url, headers=headers)
     sport_json_data = json.loads(response.text)
-    
+
     for i in sport_json_data['data']:
-        #print(i)
+        # print(i)
         if i['seasonId'] == season_id:
             len_game_ids = len(i['gameIds'])
 
-            for j in tqdm(range(1,len_game_ids+1)):
-                print(f'\nOn game {j} of {len_game_ids+1} for {season}.')
+            for j in tqdm(range(1, len_game_ids+1)):
+                print(f'\nOn game {j} of {len_game_ids} for {season}.')
                 # try:
                 #     game_df = get_volleyball_game_stats(season,j)
                 # except:
                 #     print(f'Couldn\'t parse game stats for game #{j}.')
                 #     time.sleep(10)
 
-                game_df = get_au_volleyball_game_stats(season_id,j,get_team_stats=True)
+                game_df = get_au_volleyball_game_stats(
+                    season_id, j, get_team_stats=True)
 
-                season_stats_df = pd.concat([season_stats_df,game_df],ignore_index=True)
+                season_stats_df = pd.concat(
+                    [season_stats_df, game_df], ignore_index=True)
                 del game_df
 
     return season_stats_df
 
+############################################################################################################################################################################################################################################################
+##
+# Season Stats
+##
+############################################################################################################################################################################################################################################################
+
+
+def get_au_volleyball_season_player_stats(season: int) -> pd.DataFrame():
+    """
+    Given an Atheltes Unlimited (AU) volleyball season, get all season player stats for an AU volleyball season.
+
+    Parameters
+    ----------
+    `season` (int, mandatory):
+        The AU volleyball season you want season player stats from.
+
+    Returns
+    ----------
+    A pandas DataFrame containing season player stats a AU season.
+
+    """
+    game_stats_df = get_au_volleyball_season_player_box(season)
+    # ['sport', 'api_version', 'season', 'seasonId', 'week_number',
+    #    'game_number', 'season_type', 'playerId', 'uniformNumber',
+    #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
+    #    'first_name', 'last_name', 'full_name', 'player_id', 'uniform_number',
+    #    'uniform_number_display', 'primary_position_lk',
+    #    'secondary_position_lk', 'team_id', 'sets_played', 'kills',
+    #    'kills_per_set', 'attack_errors', 'attack_attempts',
+    #    'attack_percentage', 'assists', 'assists_per_set', 'setting_errors',
+    #    'service_errors', 'service_aces', 'service_aces_per_set',
+    #    'total_reception_attempts', 'reception_errors',
+    #    'positive_reception_pct', 'digs', 'digs_per_set', 'blocks',
+    #    'blocks_per_set', 'au_total_points']
+
+    game_stats_df.loc[game_stats_df['sets_played'] > 0, 'G'] = 1
+
+    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'playerId',
+                                         'first_name', 'last_name', 'full_name'], as_index=False)[[
+                                             'G', 'sets_played', 'kills',
+                                             'attack_errors', 'attack_attempts',
+                                             'assists', 'setting_errors',
+                                             'service_errors', 'service_aces',
+                                             'total_reception_attempts', 'reception_errors',
+                                             'digs', 'blocks',
+                                             'au_total_points']].sum()
+
+    finished_df[['G', 'sets_played', 'kills',
+                 'attack_errors', 'attack_attempts',
+                 'assists', 'setting_errors',
+                 'service_errors', 'service_aces',
+                 'total_reception_attempts', 'reception_errors',
+                 'digs', 'blocks',
+                 'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
+                                                    'attack_errors', 'attack_attempts',
+                                                    'assists', 'setting_errors',
+                                                    'service_errors', 'service_aces',
+                                                    'total_reception_attempts', 'reception_errors',
+                                                    'digs', 'blocks',
+                                                    'au_total_points']].astype('int')
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
+        finished_df['kills']) / finished_df['sets_played']
+    finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
+
+    finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
+        finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
+    finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
+        3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
+        finished_df['assists']) / finished_df['sets_played']
+    finished_df['assists_per_set'] = finished_df['assists_per_set'].round(3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
+        finished_df['service_aces']) / finished_df['sets_played']
+    finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
+        3)
+
+    # finished_df['positive_reception_pct'] = 0
+    # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
+    #     3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
+        finished_df['digs']) / finished_df['sets_played']
+    finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
+        finished_df['blocks']) / finished_df['sets_played']
+    finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
+
+    return finished_df
+
+
+def get_au_volleyball_season_team_stats(season: int) -> pd.DataFrame():
+    """
+    Given an Atheltes Unlimited (AU) volleyball season, get all season team stats for an AU volleyball season.
+
+    Parameters
+    ----------
+    `season` (int, mandatory):
+        The AU volleyball season you want season team stats from.
+
+    Returns
+    ----------
+    A pandas DataFrame containing season team stats a AU season.
+
+    """
+    game_stats_df = get_au_volleyball_season_team_box(season)
+    # ['sport', 'api_version', 'season', 'seasonId', 'week_number',
+    #    'game_number', 'season_type', 'playerId', 'uniformNumber',
+    #    'uniformNumberDisplay', 'primaryPositionLk', 'secondaryPositionLk',
+    #    'first_name', 'last_name', 'full_name', 'player_id', 'uniform_number',
+    #    'uniform_number_display', 'primary_position_lk',
+    #    'secondary_position_lk', 'team_id', 'sets_played', 'kills',
+    #    'kills_per_set', 'attack_errors', 'attack_attempts',
+    #    'attack_percentage', 'assists', 'assists_per_set', 'setting_errors',
+    #    'service_errors', 'service_aces', 'service_aces_per_set',
+    #    'total_reception_attempts', 'reception_errors',
+    #    'positive_reception_pct', 'digs', 'digs_per_set', 'blocks',
+    #    'blocks_per_set', 'au_total_points']
+    game_stats_df['G'] = 1
+
+    finished_df = game_stats_df.groupby(['sport', 'season', 'seasonId', 'team_id'], as_index=False)[[
+        'G', 'sets_played', 'kills',
+        'attack_errors', 'attack_attempts',
+        'assists', 'setting_errors',
+        'service_errors', 'service_aces',
+        'total_reception_attempts', 'reception_errors',
+        'digs', 'blocks',
+        'au_total_points']].sum()
+
+    finished_df[['G', 'sets_played', 'kills',
+                 'attack_errors', 'attack_attempts',
+                 'assists', 'setting_errors',
+                 'service_errors', 'service_aces',
+                 'total_reception_attempts', 'reception_errors',
+                 'digs', 'blocks',
+                 'au_total_points']] = finished_df[['G', 'sets_played', 'kills',
+                                                    'attack_errors', 'attack_attempts',
+                                                    'assists', 'setting_errors',
+                                                    'service_errors', 'service_aces',
+                                                    'total_reception_attempts', 'reception_errors',
+                                                    'digs', 'blocks',
+                                                    'au_total_points']].astype('int')
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'kills_per_set'] = (
+        finished_df['kills']) / finished_df['sets_played']
+    finished_df['kills_per_set'] = finished_df['kills_per_set'].round(3)
+
+    finished_df.loc[finished_df['attack_attempts'] > 0, 'attack_percentage'] = (
+        finished_df['kills'] - finished_df['attack_errors']) / finished_df['attack_attempts']
+    finished_df['attack_percentage'] = finished_df['attack_percentage'].round(
+        3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'assists_per_set'] = (
+        finished_df['assists']) / finished_df['sets_played']
+    finished_df['assists_per_set'] = finished_df['assists_per_set'].round(3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'service_aces_per_set'] = (
+        finished_df['service_aces']) / finished_df['sets_played']
+    finished_df['service_aces_per_set'] = finished_df['service_aces_per_set'].round(
+        3)
+
+    # finished_df['positive_reception_pct'] = 0
+    # finished_df['positive_reception_pct'] = finished_df['positive_reception_pct'].round(
+    #     3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'digs_per_set'] = (
+        finished_df['digs']) / finished_df['sets_played']
+    finished_df['digs_per_set'] = finished_df['digs_per_set'].round(3)
+
+    finished_df.loc[finished_df['sets_played'] > 0, 'blocks_per_set'] = (
+        finished_df['blocks']) / finished_df['sets_played']
+    finished_df['blocks_per_set'] = finished_df['blocks_per_set'].round(3)
+
+    return finished_df
```

### Comparing `athletes_unlimited_py-0.0.4/athletes_unlimited_py.egg-info/PKG-INFO` & `athletes_unlimited_py-0.0.5/athletes_unlimited_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: athletes-unlimited-py
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python package for the Athletes Unlimited sports organization, and for the various sports it hosts.
 Author-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 Maintainer-email: Joseph Armstrong <armstrongjoseph08@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/armstjc/athletes-unlimited-py
 Project-URL: documentation, https://github.com/armstjc/athletes-unlimited-py/wiki
 Project-URL: repository, https://github.com/armstjc/athletes-unlimited-py.git
```

### Comparing `athletes_unlimited_py-0.0.4/pyproject.toml` & `athletes_unlimited_py-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools","wheel","pyarrow","pandas","tqdm","requests","lxml"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "athletes_unlimited_py"
-version = "0.0.4"
+version = "0.0.5"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "MIT"}
 
 authors = [
     {name = "Joseph Armstrong", email="armstrongjoseph08@gmail.com"}
 ]
```

