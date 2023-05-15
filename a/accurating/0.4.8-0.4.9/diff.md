# Comparing `tmp/accurating-0.4.8.tar.gz` & `tmp/accurating-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accurating-0.4.8.tar", max compression
+gzip compressed data, was "accurating-0.4.9.tar", max compression
```

## Comparing `accurating-0.4.8.tar` & `accurating-0.4.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.8/LICENSE
--rw-r--r--   0        0        0     6369 2023-05-14 19:51:52.513579 accurating-0.4.8/README.md
--rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.8/accurating/__init__.py
--rw-r--r--   0        0        0     8420 2023-05-14 19:49:50.236990 accurating-0.4.8/accurating/model.py
--rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.8/accurating/tests/__init__.py
--rw-r--r--   0        0        0     3135 2023-05-14 19:49:25.928871 accurating-0.4.8/accurating/tests/model_test.py
--rw-r--r--   0        0        0      648 2023-05-14 19:52:44.021823 accurating-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 accurating-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-04-16 18:25:22.173292 accurating-0.4.9/LICENSE
+-rw-r--r--   0        0        0     6369 2023-05-14 19:51:52.513579 accurating-0.4.9/README.md
+-rw-r--r--   0        0        0      231 2023-04-17 04:07:09.502903 accurating-0.4.9/accurating/__init__.py
+-rw-r--r--   0        0        0     9316 2023-05-15 00:36:02.306450 accurating-0.4.9/accurating/model.py
+-rw-r--r--   0        0        0        0 2023-04-16 18:25:22.173292 accurating-0.4.9/accurating/tests/__init__.py
+-rw-r--r--   0        0        0     3131 2023-05-15 00:37:22.194706 accurating-0.4.9/accurating/tests/model_test.py
+-rw-r--r--   0        0        0      648 2023-05-15 00:37:53.362805 accurating-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     6977 1970-01-01 00:00:00.000000 accurating-0.4.9/PKG-INFO
```

### Comparing `accurating-0.4.8/LICENSE` & `accurating-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `accurating-0.4.8/README.md` & `accurating-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `accurating-0.4.8/accurating/model.py` & `accurating-0.4.9/accurating/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 def log_win_prob(rating, opp_rating):
     # return jnp.log2(win_prob(rating, opp_rating))
     diff = opp_rating - rating
     return -jnp.log2(1.0 + jnp.exp2(diff))
 
 
 def log_data_prob(p1_ratings, p2_ratings, p1_win_probs, p2_win_probs):
-    winner_win_prob_log = p1_win_probs * \
-        log_win_prob(p1_ratings, p2_ratings) + p2_win_probs * \
-        log_win_prob(p2_ratings, p1_ratings)
-    mean_log_data_prob = jnp.mean(winner_win_prob_log)
-    return mean_log_data_prob
+    log_data_prov_values = (
+        p1_win_probs * log_win_prob(p1_ratings, p2_ratings) +
+        p2_win_probs * log_win_prob(p2_ratings, p1_ratings)
+    )
+    return jnp.mean(log_data_prov_values)
 
 
 @dataclasses.dataclass
 class MatchResultArrays:
     """Match data for AccuRating in numpy arrays.
     All attributes have a shape (match_count,).
     """
@@ -76,14 +76,19 @@
     Setting smoothing to 1.0 ignorse match result would rely on player pairing only.
 
     Typically, in the absence of data ratings assume a prior that the skill of a player some fixed value like 1000.
     This allows the rating to not escape to infinity when only losses or only wins are available.
     Smoothing essentially allows to specify that the looser (in every match) had a small chance of winning.
     This is also known as 'label smoothing'."""
 
+    winner_prior_rating: float = 1000.0
+    loser_prior_rating: float = 1000.0
+    winner_prior_match_count: float = 0.0
+    loser_prior_match_count: float = 0.0
+
     max_steps: int = 1_000_000
     """Limits the number of passes over the dataset."""
 
     do_log: bool = False
     """Enables additional logging."""
 
     initial_lr: float = 10000.0
@@ -101,46 +106,58 @@
 def fit(
     data: MatchResultArrays,
     config: Config,
 ) -> Model:
     """Fits the model to data according to config.
     The time complexity is O(match_count * player_count * max(season) * steps)
     """
+    if config.do_log:
+        print(config)
     p1_win_probs = data.p1_win_prob
     p1s = data.p1
     p2s = data.p2
     seasons = data.season
 
     p1_win_probs = (1 - config.smoothing) * \
         p1_win_probs + config.smoothing * 0.5
     p2_win_probs = 1.0 - p1_win_probs
 
-    player_count = jnp.maximum(jnp.max(p1s), jnp.max(p2s)) + 1
-    season_count = jnp.max(seasons) + 1
+    player_count = int(jnp.maximum(jnp.max(p1s), jnp.max(p2s)) + 1)
+    season_count = int(jnp.max(seasons) + 1)
 
     (data_size,) = p1s.shape
     assert seasons.shape == (data_size,)
     assert p1s.shape == (data_size,)
     assert p2s.shape == (data_size,)
     assert p1_win_probs.shape == (data_size,)
 
     def model(params):
+        log_likelihood = 0.0
         ratings = params['rating']
         assert ratings.shape == (player_count, season_count)
         p1_ratings = ratings[p1s, seasons]
         p2_ratings = ratings[p2s, seasons]
 
         assert p1_ratings.shape == (data_size,)
         assert p2_ratings.shape == (data_size,)
-        mean_log_data_prob = log_data_prob(
-            p1_ratings, p2_ratings, p1_win_probs, p2_win_probs)
-        rating_season_divergence = config.season_rating_stability * \
-            jnp.mean((ratings[:, 1:] - ratings[:, :-1])**2)
+
+        mean_log_data_prob = log_data_prob(p1_ratings, p2_ratings, p1_win_probs, p2_win_probs)
+        log_likelihood += mean_log_data_prob
+
+        if config.season_rating_stability > 0.0:
+            log_likelihood -= config.season_rating_stability * jnp.mean((ratings[:, 1:] - ratings[:, :-1])**2)
+
+        if config.winner_prior_match_count > 0.0:
+            log_likelihood += log_data_prob(ratings, config.winner_prior_rating, 0.0, config.winner_prior_match_count)
+
+        if config.loser_prior_match_count > 0.0:
+            log_likelihood += log_data_prob(ratings, config.loser_prior_rating, config.loser_prior_match_count, 0.0)
+
         geomean_data_prob = jnp.exp2(mean_log_data_prob)
-        return mean_log_data_prob - rating_season_divergence, geomean_data_prob
+        return log_likelihood, geomean_data_prob
 
         # TODO: This is an experiment trying to evaluate ELO playing consistency. Try again and delete if does not work.
         # cons = params['consistency']
         # p1_cons = jnp.take(cons, p1s)
         # p2_cons = jnp.take(cons, p2s)
         # winner_win_prob_log = 0.0
         # winner_win_prob_log += p1_win_probs * log_win_prob_diff(diff/jnp.exp(p1_cons)) + p2_win_probs * log_win_prob_diff(-diff/jnp.exp(p1_cons))
@@ -195,19 +212,26 @@
         if max_d_rating < 1e-15:
             break
 
         lr *= 1.5 ** (1.0 / 12)
 
     def postprocess():
         rating = {}
+        last_rating = []
         for id, name in enumerate(data.player_name):
             rating[name] = {}
             for season in range(season_count):
-                rating[name][season] = float(
-                    params['rating'][id, season]) * 100.0
+                rating[name][season] = float(params['rating'][id, season]) * 100.0
+            last_rating.append((rating[name][season_count - 1], name))
+        if config.do_log:
+            last_rating.sort(reverse=True)
+            print("Top 10 last season:")
+            for i in range(min(len(last_rating), 10)):
+                print(f'{last_rating[i][1]:30}: {last_rating[i][0]: 8.1f}')
+
         ret = Model(rating=rating)
         return ret
 
     return postprocess()
 
 
 def data_from_dicts(matches) -> MatchResultArrays:
```

### Comparing `accurating-0.4.8/accurating/tests/model_test.py` & `accurating-0.4.9/accurating/tests/model_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,18 +19,18 @@
                 p2s.append(p2)
                 p1_win_prob = accurating.win_prob(
                     true_elos[p1][season], true_elos[p2][season])
                 p1_win_probs.append(p1_win_prob)
                 seasons.append(season)
 
     return accurating.MatchResultArrays(
-        p1=jnp.array(p1s),
-        p2=jnp.array(p2s),
-        p1_win_prob=jnp.array(p1_win_probs),
-        season=jnp.array(seasons),
+        p1=np.array(p1s),
+        p2=np.array(p2s),
+        p1_win_prob=np.array(p1_win_probs),
+        season=np.array(seasons),
         player_name=[f'p{i}' for i in range(player_count)],
     )
 
 
 def test_fit():
     true_elos = jnp.array([[8.0, 4.0], [2.0, 3.0], [0.0, 0.0],])
     test_data = get_test_data(true_elos)
```

### Comparing `accurating-0.4.8/pyproject.toml` & `accurating-0.4.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AccuRating"
-version = "0.4.8"
+version = "0.4.9"
 description = "AccuRating is a library for accurate player ranking based on match results."
 authors = ["Lukasz Lew <lukasz.lew@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/lukaszlew/accurating"
 documentation = "https://lukaszlew.github.io/accurating/"
 
 [tool.poetry.dependencies]
```

### Comparing `accurating-0.4.8/PKG-INFO` & `accurating-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accurating
-Version: 0.4.8
+Version: 0.4.9
 Summary: AccuRating is a library for accurate player ranking based on match results.
 Home-page: https://github.com/lukaszlew/accurating
 Author: Lukasz Lew
 Author-email: lukasz.lew@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

