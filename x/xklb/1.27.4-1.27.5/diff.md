# Comparing `tmp/xklb-1.27.4.tar.gz` & `tmp/xklb-1.27.5.tar.gz`

## Comparing `xklb-1.27.4.tar` & `xklb-1.27.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.4/.gitattributes
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.4/TODO
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.4/Windows.md
--rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.4/pdm.lock
--rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.4/readme.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/FUNDING.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.4/.github/workflows/push.yaml
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.4/sql/transfer.sql
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/__init__.py
--rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/av.py
--rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/books.py
--rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/consts.py
--rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/db.py
--rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/dl_config.py
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/dl_extract.py
--rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/fs_extract.py
--rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/gui.py
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/hn_extract.py
--rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/lb.py
--rw-r--r--   0        0        0    35208 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/play_actions.py
--rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/playback.py
--rw-r--r--   0        0        0    27136 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/player.py
--rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/praw_extract.py
--rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/stats.py
--rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/subtitle.py
--rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tabs_actions.py
--rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tabs_extract.py
--rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tube_backend.py
--rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/tube_extract.py
--rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/utils.py
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/bigdirs.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/christen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/dedupe.py
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/move_list.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/relmv.py
--rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/data.py
--rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.4/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.4/assets/kotobago.png
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.4/.gitignore
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.4/LICENSE
--rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.4/README.md
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.4/pyproject.toml
--rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.4/PKG-INFO
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 xklb-1.27.5/.gitattributes
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 xklb-1.27.5/TODO
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 xklb-1.27.5/Windows.md
+-rw-r--r--   0        0        0   416092 2020-02-02 00:00:00.000000 xklb-1.27.5/pdm.lock
+-rw-r--r--   0        0        0    16847 2020-02-02 00:00:00.000000 xklb-1.27.5/readme.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 xklb-1.27.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 xklb-1.27.5/sql/transfer.sql
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/__init__.py
+-rw-r--r--   0        0        0     6996 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/av.py
+-rw-r--r--   0        0        0     6866 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/books.py
+-rw-r--r--   0        0        0     7698 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/consts.py
+-rw-r--r--   0        0        0     8450 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/db.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/dl_config.py
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/dl_extract.py
+-rw-r--r--   0        0        0    14486 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/fs_extract.py
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/gui.py
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/hn_extract.py
+-rw-r--r--   0        0        0     9635 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/lb.py
+-rw-r--r--   0        0        0    35208 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/play_actions.py
+-rw-r--r--   0        0        0     4545 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/playback.py
+-rw-r--r--   0        0        0    28867 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/player.py
+-rw-r--r--   0        0        0    14733 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/praw_extract.py
+-rw-r--r--   0        0        0    16161 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/stats.py
+-rw-r--r--   0        0        0     4109 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/subtitle.py
+-rw-r--r--   0        0        0    12091 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     3639 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    21920 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tube_backend.py
+-rw-r--r--   0        0        0     6378 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/tube_extract.py
+-rw-r--r--   0        0        0    28274 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/utils.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/bigdirs.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/christen.py
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0     8267 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/dedupe.py
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     4022 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7013 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/relmv.py
+-rw-r--r--   0        0        0    17200 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2712 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/data.py
+-rw-r--r--   0        0        0     1938 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2777 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 xklb-1.27.5/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-1.27.5/assets/kotobago.png
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 xklb-1.27.5/.gitignore
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-1.27.5/LICENSE
+-rw-r--r--   0        0        0    40521 2020-02-02 00:00:00.000000 xklb-1.27.5/README.md
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 xklb-1.27.5/pyproject.toml
+-rw-r--r--   0        0        0    44035 2020-02-02 00:00:00.000000 xklb-1.27.5/PKG-INFO
```

### Comparing `xklb-1.27.4/Windows.md` & `xklb-1.27.5/Windows.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/pdm.lock` & `xklb-1.27.5/pdm.lock`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/readme.py` & `xklb-1.27.5/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/.github/ISSUE_TEMPLATE/bug_report.md` & `xklb-1.27.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/.github/ISSUE_TEMPLATE/feature_request.md` & `xklb-1.27.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/.github/workflows/push.yaml` & `xklb-1.27.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/sql/transfer.sql` & `xklb-1.27.5/sql/transfer.sql`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/av.py` & `xklb-1.27.5/xklb/av.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/books.py` & `xklb-1.27.5/xklb/books.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/consts.py` & `xklb-1.27.5/xklb/consts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/db.py` & `xklb-1.27.5/xklb/db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/dl_config.py` & `xklb-1.27.5/xklb/dl_config.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/dl_extract.py` & `xklb-1.27.5/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/fs_extract.py` & `xklb-1.27.5/xklb/fs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/gui.py` & `xklb-1.27.5/xklb/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/hn_extract.py` & `xklb-1.27.5/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/lb.py` & `xklb-1.27.5/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/play_actions.py` & `xklb-1.27.5/xklb/play_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/playback.py` & `xklb-1.27.5/xklb/playback.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/player.py` & `xklb-1.27.5/xklb/player.py`

 * *Files 3% similar despite different names*

```diff
@@ -575,14 +575,54 @@
         return False
     elif display.width > display.height:  # wide
         return False
     else:  # tall or square: prefer horizontal split
         return True
 
 
+def modify_display_size_for_taskbar(display):
+    try:
+        if platform.system() == "Windows":
+            import win32gui
+
+            taskbar_window_handle = win32gui.FindWindow("Shell_TrayWnd", None)
+            if taskbar_window_handle == 0:
+                taskbar_window_handle = win32gui.FindWindow("Shell_SecondaryTrayWnd", None)
+            if taskbar_window_handle == 0:
+                return display
+
+            work_area = win32gui.GetMonitorInfo(taskbar_window_handle)["rcWork"]
+
+            _taskbar_height = display.height - work_area[3]
+            display.height = work_area[3] - work_area[1]
+            display.width = work_area[2] - work_area[0]
+
+        elif platform.system() == "Linux":
+            xprop_output = subprocess.check_output("xprop -root _NET_WORKAREA".split()).decode().strip()
+            work_area = [int(x) for x in xprop_output.split(" = ")[1].split(",")]
+
+            _taskbar_height = display.height - work_area[3]
+            display.height = work_area[3] - work_area[1]
+            display.width = work_area[2] - work_area[0]
+
+        elif platform.system() == "Darwin":
+            dock_height = int(subprocess.check_output(["defaults", "read", "com.apple.dock", "tilesize"]).strip())
+            dock_position = (
+                subprocess.check_output(["defaults", "read", "com.apple.dock", "orientation"]).decode().strip()
+            )
+            if dock_position == "left" or dock_position == "right":
+                display.width -= dock_height
+            else:
+                display.height -= dock_height
+
+        return display
+    except:
+        return display
+
+
 def get_multiple_player_template(args) -> List[str]:
     import screeninfo
 
     displays = screeninfo.get_monitors()
     if args.screen_name:
         displays = get_display_by_name(displays, args.screen_name)
 
@@ -593,14 +633,17 @@
     elif args.multiple_playback < len(displays):
         # play videos on supporting screens but not active one
         displays = [d for d in displays if not d.is_primary]
         displays = displays[: len(args.multiple_playback)]
 
     min_media_per_screen, remainder = divmod(args.multiple_playback, len(displays))
 
+    if min_media_per_screen > 1:
+        displays[0] = modify_display_size_for_taskbar(displays[0])
+
     displays.sort(key=lambda d: d.width * d.height, reverse=True)
     players = []
     for d_idx, display in enumerate(displays):
         qty = min_media_per_screen
         if remainder > 0 and d_idx == 0:
             qty += remainder
```

### Comparing `xklb-1.27.4/xklb/praw_extract.py` & `xklb-1.27.5/xklb/praw_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/stats.py` & `xklb-1.27.5/xklb/stats.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/subtitle.py` & `xklb-1.27.5/xklb/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/tabs_actions.py` & `xklb-1.27.5/xklb/tabs_actions.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/tabs_extract.py` & `xklb-1.27.5/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/tube_backend.py` & `xklb-1.27.5/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/tube_extract.py` & `xklb-1.27.5/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/utils.py` & `xklb-1.27.5/xklb/utils.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/__init__.py` & `xklb-1.27.5/xklb/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/bigdirs.py` & `xklb-1.27.5/xklb/scripts/bigdirs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/christen.py` & `xklb-1.27.5/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/copy_play_counts.py` & `xklb-1.27.5/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/dedupe.py` & `xklb-1.27.5/xklb/scripts/dedupe.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/merge_dbs.py` & `xklb-1.27.5/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/merge_online_local.py` & `xklb-1.27.5/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/move_list.py` & `xklb-1.27.5/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/optimize_db.py` & `xklb-1.27.5/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/redownload.py` & `xklb-1.27.5/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/relmv.py` & `xklb-1.27.5/xklb/scripts/relmv.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/scatter.py` & `xklb-1.27.5/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/streaming_tab_loader.py` & `xklb-1.27.5/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/mining/data.py` & `xklb-1.27.5/xklb/scripts/mining/data.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/mining/extract_links.py` & `xklb-1.27.5/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/mining/nouns.py` & `xklb-1.27.5/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/mining/pushshift.py` & `xklb-1.27.5/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/xklb/scripts/mining/reddit_selftext.py` & `xklb-1.27.5/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/assets/kotobago.png` & `xklb-1.27.5/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/.gitignore` & `xklb-1.27.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/LICENSE` & `xklb-1.27.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/README.md` & `xklb-1.27.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.004)
+    xk media library subcommands (v1.27.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

### Comparing `xklb-1.27.4/pyproject.toml` & `xklb-1.27.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-1.27.4/PKG-INFO` & `xklb-1.27.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xklb
-Version: 1.27.4
+Version: 1.27.5
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library/wiki/Usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library/
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -99,15 +99,15 @@
     pip install xklb
 
 ## Examples
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v1.27.004)
+    xk media library subcommands (v1.27.005)
 
     local media:
       lb fsadd                 Create a local media database; Add folders
       lb fsupdate              Refresh database: add new files, mark deleted
 
       lb listen                Listen to local and online media
       lb watch                 Watch local and online media
```

