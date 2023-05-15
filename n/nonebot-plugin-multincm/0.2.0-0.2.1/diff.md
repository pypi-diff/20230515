# Comparing `tmp/nonebot_plugin_multincm-0.2.0.tar.gz` & `tmp/nonebot_plugin_multincm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.2.0.tar", last modified: Mon May 15 17:48:35 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.2.1.tar", last modified: Mon May 15 18:07:45 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.2.0.tar` & `nonebot_plugin_multincm-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/LICENSE
--rw-r--r--   0        0        0     5488 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/README.md
--rw-r--r--   0        0        0      769 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0     7284 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0     4553 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0     9924 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0     2495 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/lrc_parser.py
--rw-r--r--   0        0        0   212591 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     1688 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      874 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      830 2023-05-15 17:48:35.217791 nonebot_plugin_multincm-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/LICENSE
+-rw-r--r--   0        0        0     5548 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/README.md
+-rw-r--r--   0        0        0      769 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0     7284 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0     4553 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0     9924 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2573 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0   212591 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     1688 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      874 2023-05-15 18:07:31.427900 nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      826 2023-05-15 18:07:45.920101 nonebot_plugin_multincm-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6449 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.1/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.2.0/LICENSE` & `nonebot_plugin_multincm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/README.md` & `nonebot_plugin_multincm-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -167,11 +167,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.1
+
+- 删除歌词尾部的空行与多余分割线
+
 ### 0.2.0
 
 - 新增了三个指令 `解析`、`歌词`、`链接`
 - 点歌指令支持直接输入音乐 ID
```

#### html2text {}

```diff
@@ -49,9 +49,10 @@
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.1 -
+å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__init__.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.plugin import PluginMetadata
 
 from . import __main__ as __main__
 from .config import ConfigModel
 
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __plugin_meta__ = PluginMetadata(
     "MultiNCM",
     "网易云多选点歌",
     (
         "指令：\n"
         "▷ 点歌 [歌曲名 / 音乐 ID]\n"
         "▷ 解析 <回复 音乐卡片 / 链接>（获取该音乐的播放链接并使用自定义卡片发送）\n"
```

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__main__.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/__main__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/draw.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/lrc_parser.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/lrc_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,19 @@
 
     parsed.sort(key=lambda x: x.time)
     return parsed
 
 
 def merge(*lyrics: List[LrcLine], threshold: int = 20) -> List[List[LrcLine]]:
     lyrics = tuple(x.copy() for x in lyrics)
+
+    for lrc in lyrics:
+        while not lrc[-1].lrc:
+            lrc.pop()
+
     main_lyric = lyrics[0]
     sub_lyrics = lyrics[1:]
 
     for x in main_lyric:
         if not x.lrc:
             x.lrc = "--------"
```

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/types.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.2.1/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.2.0/pyproject.toml` & `nonebot_plugin_multincm-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.2.0"
-description = "网易云多选点歌"
+version = "0.2.1"
+description = "NCM Song Searcher"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
     "pydantic>=1.10.4",
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nonebot_plugin_multincm-0.2.0/PKG-INFO` & `nonebot_plugin_multincm-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.2.0
-Summary: 网易云多选点歌
+Version: 0.2.1
+Summary: NCM Song Searcher
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
@@ -192,11 +192,15 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
+### 0.2.1
+
+- 删除歌词尾部的空行与多余分割线
+
 ### 0.2.0
 
 - 新增了三个指令 `解析`、`歌词`、`链接`
 - 点歌指令支持直接输入音乐 ID
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.0 Summary:
-ç½æäºå¤éç¹æ­ Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-
-multincm Author-Email: student_2333
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.1 Summary: NCM
+Song Searcher Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
+Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
 anyio>=3.6.2 Requires-Dist: pip>=23.0.1; extra == "dev" Requires-Dist:
 setuptools>=67.6.1; extra == "dev" Requires-Dist: nb-cli>=1.0.5; extra == "dev"
@@ -62,9 +62,10 @@
 èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
 [1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.1 -
+å é¤æ­è¯å°¾é¨çç©ºè¡ä¸å¤ä½åå²çº¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
 `è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

