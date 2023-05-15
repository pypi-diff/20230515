# Comparing `tmp/SantorinAI-1.2.5.tar.gz` & `tmp/SantorinAI-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SantorinAI-1.2.5.tar", last modified: Sun May 14 21:07:07 2023, max compression
+gzip compressed data, was "SantorinAI-1.2.6.tar", last modified: Mon May 15 07:26:41 2023, max compression
```

## Comparing `SantorinAI-1.2.5.tar` & `SantorinAI-1.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.165980 SantorinAI-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 21:07:07.165980 SantorinAI-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.161980 SantorinAI-1.2.5/SantorinAI.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-14 21:07:07.000000 SantorinAI-1.2.5/SantorinAI.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-14 21:07:07.000000 SantorinAI-1.2.5/SantorinAI.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:07:07.000000 SantorinAI-1.2.5/SantorinAI.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 21:07:07.000000 SantorinAI-1.2.5/SantorinAI.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 21:07:07.000000 SantorinAI-1.2.5/SantorinAI.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.161980 SantorinAI-1.2.5/santorinai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/board.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.161980 SantorinAI-1.2.5/santorinai/board_displayer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/board_displayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/board_displayer/board_displayer.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/pawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/player.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.161980 SantorinAI-1.2.5/santorinai/player_examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/player_examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/player_examples/first_choice_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/player_examples/random_player.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/santorinai/tester.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 21:07:07.165980 SantorinAI-1.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:07:07.165980 SantorinAI-1.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/test/test_board.py
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-14 21:06:56.000000 SantorinAI-1.2.5/test/test_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/SantorinAI.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5191 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-15 07:26:41.000000 SantorinAI-1.2.6/SantorinAI.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18107 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/board_displayer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board_displayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/board_displayer/board_displayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/pawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/santorinai/player_examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/first_choice_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/player_examples/random_player.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/santorinai/tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:41.389600 SantorinAI-1.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21019 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/test_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-15 07:26:30.000000 SantorinAI-1.2.6/test/test_tester.py
```

### Comparing `SantorinAI-1.2.5/LICENSE` & `SantorinAI-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/PKG-INFO` & `SantorinAI-1.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.5/README.md` & `SantorinAI-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/SantorinAI.egg-info/PKG-INFO` & `SantorinAI-1.2.6/SantorinAI.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SantorinAI
-Version: 1.2.5
+Version: 1.2.6
 Summary: A Python library for the Santorini board game
 Home-page: https://github.com/tomansion/santorinai
 Author: Tom Mansion
 Author-email: tomansion@yahoo.fr
 Keywords: santorini,ai,boardgame
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `SantorinAI-1.2.5/SantorinAI.egg-info/SOURCES.txt` & `SantorinAI-1.2.6/SantorinAI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/board.py` & `SantorinAI-1.2.6/santorinai/board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/board_displayer/board_displayer.py` & `SantorinAI-1.2.6/santorinai/board_displayer/board_displayer.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/pawn.py` & `SantorinAI-1.2.6/santorinai/pawn.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/player.py` & `SantorinAI-1.2.6/santorinai/player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/player_examples/first_choice_player.py` & `SantorinAI-1.2.6/santorinai/player_examples/first_choice_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/player_examples/random_player.py` & `SantorinAI-1.2.6/santorinai/player_examples/random_player.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/santorinai/tester.py` & `SantorinAI-1.2.6/santorinai/tester.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,9 +134,17 @@
                 self.display_message("Draw")
             else:
                 self.display_message(f"Player {players[winer_number - 1].name()} wins!")
                 nb_victories[winer_number - 1] += 1
 
         # Display the results
         print(f"\nResults:")
-        print(f"Player {players[0].name()} won {nb_victories[0]} times")
-        print(f"Player {players[1].name()} won {nb_victories[1]} times")
+        print(
+            f"Player {players[0].name()} won {nb_victories[0]} times ("
+            + str(round(nb_victories[0] / nb_games * 100, 2))
+            + "%)"
+        )
+        print(
+            f"Player {players[1].name()} won {nb_victories[1]} times ("
+            + str(round(nb_victories[1] / nb_games * 100, 2))
+            + "%)"
+        )
```

### Comparing `SantorinAI-1.2.5/setup.py` & `SantorinAI-1.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="SantorinAI",
-    version="1.2.5",
+    version="1.2.6",
     author="Tom Mansion",
     author_email="tomansion@yahoo.fr",
     description="A Python library for the Santorini board game",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/tomansion/santorinai",
     packages=find_packages(),
```

### Comparing `SantorinAI-1.2.5/test/test_board.py` & `SantorinAI-1.2.6/test/test_board.py`

 * *Files identical despite different names*

### Comparing `SantorinAI-1.2.5/test/test_tester.py` & `SantorinAI-1.2.6/test/test_tester.py`

 * *Files identical despite different names*

