# Comparing `tmp/nonebot_plugin_multincm-0.1.0.tar.gz` & `tmp/nonebot_plugin_multincm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_multincm-0.1.0.tar", last modified: Sun May 14 20:42:52 2023, max compression
+gzip compressed data, was "nonebot_plugin_multincm-0.2.0.tar", last modified: Mon May 15 17:48:35 2023, max compression
```

## Comparing `nonebot_plugin_multincm-0.1.0.tar` & `nonebot_plugin_multincm-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1069 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/LICENSE
--rw-r--r--   0        0        0     4951 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/README.md
--rw-r--r--   0        0        0      316 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/__init__.py
--rw-r--r--   0        0        0     4138 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/__main__.py
--rw-r--r--   0        0        0      512 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/config.py
--rw-r--r--   0        0        0     3868 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/data_source.py
--rw-r--r--   0        0        0     8031 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/draw.py
--rw-r--r--   0        0        0   212591 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/res/bg.jpg
--rw-r--r--   0        0        0     1311 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/types.py
--rw-r--r--   0        0        0      874 2023-05-14 20:42:34.894505 nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/utils.py
--rw-r--r--   0        0        0      830 2023-05-14 20:42:52.178719 nonebot_plugin_multincm-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5856 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5488 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/README.md
+-rw-r--r--   0        0        0      769 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__init__.py
+-rw-r--r--   0        0        0     7284 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/__main__.py
+-rw-r--r--   0        0        0      512 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/config.py
+-rw-r--r--   0        0        0     4553 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/data_source.py
+-rw-r--r--   0        0        0     9924 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/draw.py
+-rw-r--r--   0        0        0     2495 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/lrc_parser.py
+-rw-r--r--   0        0        0   212591 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/res/bg.jpg
+-rw-r--r--   0        0        0     1688 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/types.py
+-rw-r--r--   0        0        0      874 2023-05-15 17:48:22.949869 nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/utils.py
+-rw-r--r--   0        0        0      830 2023-05-15 17:48:35.217791 nonebot_plugin_multincm-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6393 1970-01-01 00:00:00.000000 nonebot_plugin_multincm-0.2.0/PKG-INFO
```

### Comparing `nonebot_plugin_multincm-0.1.0/LICENSE` & `nonebot_plugin_multincm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.1.0/README.md` & `nonebot_plugin_multincm-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -125,15 +125,28 @@
 |   `NCM_LIST_LIMIT`   |  否  |  `20`  |         歌曲列表每页的最大数量          |
 |   `NCM_LIST_FONT`    |  否  |   无   |         渲染歌曲列表使用的字体          |
 |  `NCM_MAX_NAME_LEN`  |  否  | `600`  | 歌曲列表中歌名列的最大文本宽度（像素）  |
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
-发送 `点歌 [歌曲名]` 即可
+### 指令
+
+- 点歌 [歌曲名 / 音乐 ID]
+  - 别名：`网易云`、`wyy`
+- 解析 <回复 音乐卡片 / 链接>（获取该音乐的播放链接并使用自定义卡片发送）
+  - 别名：`resolve`、`parse`、`get`
+- 歌词 <回复 音乐卡片 / 链接>（获取该音乐的歌词）
+  - 别名：`lrc`、`lyric`、`lyrics`
+- 链接 <回复 音乐卡片 / 链接>（获取该音乐的网易云链接）
+  - 别名：`link`
+
+### Tip
+
+- 点击 Bot 发送的音乐卡片可以跳转直链，可以直接下载该音乐
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -154,8 +167,11 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.0
+
+- 新增了三个指令 `解析`、`歌词`、`链接`
+- 点歌指令支持直接输入音乐 ID
```

#### html2text {}

```diff
@@ -33,18 +33,25 @@
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
-æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨
-åé `ç¹æ­ [æ­æ²å]` å³å¯ ## ð èç³» QQï¼3076823485 Telegramï¼
-[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
-?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
+æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] - å«åï¼`ç½æäº`ã`wyy` - è§£æ
+<åå¤ é³ä¹å¡ç /
+é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåéï¼ -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç /
+é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ - å«åï¼`lrc`ã`lyric`ã`lyrics` -
+é¾æ¥ <åå¤ é³ä¹å¡ç / é¾æ¥>ï¼è·åè¯¥é³ä¹çç½æäºé¾æ¥ï¼ -
+å«åï¼`link` ### Tip - ç¹å» Bot
+åéçé³ä¹å¡çå¯ä»¥è·³è½¬ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½è¯¥é³ä¹ ## ð
+èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
+[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/config.py` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/config.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/data_source.py` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/data_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,18 +13,18 @@
 from pyncm.apis.cloudsearch import GetSearchResult
 from pyncm.apis.login import (
     GetCurrentLoginStatus,
     LoginViaAnonymousAccount,
     LoginViaCellphone,
     LoginViaEmail,
 )
-from pyncm.apis.track import GetTrackAudio
+from pyncm.apis.track import GetTrackAudio, GetTrackDetail, GetTrackLyrics
 
 from .config import config
-from .types import SongSearchResult, TrackAudio
+from .types import LyricData, Privilege, Song, SongSearchResult, TrackAudio
 from .utils import awaitable
 
 DATA_PATH = Path().cwd() / "data" / "multincm"
 if not DATA_PATH.exists():
     DATA_PATH.mkdir(parents=True)
 
 SESSION_FILE = DATA_PATH / "session.cache"
@@ -48,20 +48,41 @@
         offset=offset,
         **kwargs,
     )
     return SongSearchResult(**res["result"])
 
 
 async def get_track_audio(
-    song_ids: list,
+    song_ids: List[int],
     bit_rate: int = 320000,
     **kwargs,
 ) -> List[TrackAudio]:
     res = await ncm_request(GetTrackAudio, song_ids, bitrate=bit_rate, **kwargs)
-    return [TrackAudio(**x) for x in cast(List[dict], res["data"])] if res else []
+    return [TrackAudio(**x) for x in cast(List[dict], res["data"])]
+
+
+async def get_track_info(ids: List[int], **kwargs) -> List[Song]:
+    res = await ncm_request(GetTrackDetail, ids, **kwargs)
+    privileges = {y.id: y for y in [Privilege(**x) for x in res["privileges"]]}
+    return [
+        Song(
+            **x,
+            privilege=(
+                privileges[song_id]
+                if (song_id := x["id"]) in privileges
+                else Privilege(id=song_id, pl=128000, plLevel="standard")
+            ),
+        )
+        for x in res["songs"]
+    ]
+
+
+async def get_track_lrc(song_id: int) -> LyricData:
+    res = await ncm_request(GetTrackLyrics, song_id)
+    return LyricData(**res)
 
 
 async def login(retry=True):
     if SESSION_FILE.exists():
         logger.info(f"使用缓存登录态 ({str(SESSION_FILE)})")
         SetCurrentSession(
             LoadSessionFromString(
```

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/draw.py` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/draw.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from dataclasses import dataclass
 from io import BytesIO
 from math import ceil
 from pathlib import Path
-from typing import List, Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union, cast
 
 from pil_utils import BuildImage, Text2Image
 from pil_utils.types import ColorType, HAlignType
 
+from . import lrc_parser
 from .config import config
-from .types import SongSearchResult
+from .types import Lyric, LyricData, SongSearchResult, User
 from .utils import format_alias, format_artists, format_time
 
 BACKGROUND = BuildImage.open(Path(__file__).parent / "res" / "bg.jpg")
 
 
 @dataclass()
 class TableHead:
@@ -259,7 +260,76 @@
     )
     footer_txt.draw_on_image(
         bg.image,
         ((width - footer_txt.width) // 2, height - table_padding - footer_txt.height),
     )
 
     return bg.save_jpg()
+
+
+def format_lrc(lrc: LyricData) -> Optional[str]:
+    def fmt_usr(usr: User) -> str:
+        return f"{usr.nickname} [{usr.userid}]"
+
+    raw = lrc.lrc
+    if (not raw) or (not (raw_lrc := raw.lyric)):
+        return None
+
+    lyrics = [
+        lrc_parser.parse(x.lyric)
+        for x in cast(List[Optional[Lyric]], [raw, lrc.romalrc, lrc.tlyric])
+        if x
+    ]
+    lyrics = [x for x in lyrics if x]
+
+    lines = []
+    if not lyrics:
+        lines.append("[i]该歌曲没有滚动歌词[/i]")
+        lines.append("")
+        lines.append("--------")
+        lines.append("")
+        lines.append(raw_lrc)
+
+    else:
+        if lyrics[0][-1].time >= 5940000:
+            return None  # 纯音乐
+
+        only_one = len(lyrics) == 1
+        for li in lrc_parser.merge(*lyrics):
+            if not only_one:
+                lines.append("")
+            lines.append(f"[b]{li[0].lrc}[/b]")
+            lines.extend([f"{x.lrc}" for x in li[1:]])
+
+    if lrc.lyricUser or lrc.transUser:
+        lines.append("")
+        lines.append("--------")
+        lines.append("")
+
+        if usr := lrc.lyricUser:
+            lines.append(f"歌词贡献者：{fmt_usr(usr)}")
+        if usr := lrc.transUser:
+            lines.append(f"翻译贡献者：{fmt_usr(usr)}")
+
+    return "\n".join(lines).strip()
+
+
+def str_to_pic(
+    txt: str,
+    padding: int = 20,
+    font_color: ColorType = (241, 246, 249),
+    bg_color: ColorType = (33, 42, 62),
+    **kwargs,
+) -> BytesIO:
+    txt2img = Text2Image.from_bbcode_text(
+        txt,
+        fontname=config.ncm_list_font or "",
+        fill=font_color,
+        **kwargs,
+    )
+    img = BuildImage.new(
+        "RGBA",
+        (txt2img.width + padding * 2, txt2img.height + padding * 2),
+        bg_color,
+    )
+    txt2img.draw_on_image(img.image, (padding, padding))
+    return img.save_jpg()
```

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/res/bg.jpg` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/res/bg.jpg`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/types.py` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List, Literal, Optional
 
 from pydantic import BaseModel
 
-BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard"]
+BrLevel = Literal["hires", "lossless", "exhigh", "higher", "standard", "none"]
 
 
 class Artist(BaseModel):
     id: int  # noqa: A003
     name: str
     tns: List[str]
     alias: List[str]
@@ -16,14 +16,15 @@
     id: int  # noqa: A003
     name: str
     picUrl: str  # noqa: N815
     tns: List[str]
 
 
 class Privilege(BaseModel):
+    id: int  # noqa: A003
     pl: int
     plLevel: BrLevel  # noqa: N815
 
 
 class Song(BaseModel):
     name: str
     id: int  # noqa: A003
@@ -60,7 +61,26 @@
     url: str
     br: int
     size: int
     md5: str
     level: str
     encodeType: str  # noqa: N815
     time: int
+
+
+class User(BaseModel):
+    id: int  # noqa: A003
+    userid: int
+    nickname: str
+
+
+class Lyric(BaseModel):
+    version: int
+    lyric: str
+
+
+class LyricData(BaseModel):
+    transUser: Optional[User]  # noqa: N815
+    lyricUser: Optional[User]  # noqa: N815
+    lrc: Optional[Lyric]
+    tlyric: Optional[Lyric]
+    romalrc: Optional[Lyric]
```

### Comparing `nonebot_plugin_multincm-0.1.0/nonebot_plugin_multincm/utils.py` & `nonebot_plugin_multincm-0.2.0/nonebot_plugin_multincm/utils.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_multincm-0.1.0/pyproject.toml` & `nonebot_plugin_multincm-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-multincm"
-version = "0.1.0"
+version = "0.2.0"
 description = "网易云多选点歌"
 authors = [
     { name = "student_2333", email = "lgc2333@126.com" },
 ]
 dependencies = [
     "nonebot2>=2.0.0-rc.1",
     "nonebot-adapter-onebot>=2.2.0",
```

### Comparing `nonebot_plugin_multincm-0.1.0/PKG-INFO` & `nonebot_plugin_multincm-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-multincm
-Version: 0.1.0
+Version: 0.2.0
 Summary: 网易云多选点歌
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-multincm
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
@@ -150,15 +150,28 @@
 |   `NCM_LIST_LIMIT`   |  否  |  `20`  |         歌曲列表每页的最大数量          |
 |   `NCM_LIST_FONT`    |  否  |   无   |         渲染歌曲列表使用的字体          |
 |  `NCM_MAX_NAME_LEN`  |  否  | `600`  | 歌曲列表中歌名列的最大文本宽度（像素）  |
 | `NCM_MAX_ARTIST_LEN` |  否  | `400`  | 歌曲列表中歌手列的最大文本宽度（像素）  |
 
 ## 🎉 使用
 
-发送 `点歌 [歌曲名]` 即可
+### 指令
+
+- 点歌 [歌曲名 / 音乐 ID]
+  - 别名：`网易云`、`wyy`
+- 解析 <回复 音乐卡片 / 链接>（获取该音乐的播放链接并使用自定义卡片发送）
+  - 别名：`resolve`、`parse`、`get`
+- 歌词 <回复 音乐卡片 / 链接>（获取该音乐的歌词）
+  - 别名：`lrc`、`lyric`、`lyrics`
+- 链接 <回复 音乐卡片 / 链接>（获取该音乐的网易云链接）
+  - 别名：`link`
+
+### Tip
+
+- 点击 Bot 发送的音乐卡片可以跳转直链，可以直接下载该音乐
 
 ## 📞 联系
 
 QQ：3076823485  
 Telegram：[@lgc2333](https://t.me/lgc2333)  
 吹水群：[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp)  
 邮箱：<lgc2333@126.com>
@@ -179,8 +192,11 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.2.0
+
+- 新增了三个指令 `解析`、`歌词`、`链接`
+- 点歌指令支持直接输入音乐 ID
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.1.0 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-multincm Version: 0.2.0 Summary:
 ç½æäºå¤éç¹æ­ Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-
 multincm Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-multincm Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: pil-utils>=0.1.7 Requires-Dist:
 pyncm>=1.6.8.9.1 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
@@ -46,18 +46,25 @@
 å¸å·ææå¯ç ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | | `NCM_PASSWORD_HASH` |
 å¦ | æ  | å¸å·å¯ç  MD5 åå¸ï¼é®ç®±ç»å½æ¶ä¸ºé®ç®±å¯ç  | |
 `NCM_LIST_LIMIT` | å¦ | `20` | æ­æ²åè¡¨æ¯é¡µçæå¤§æ°é | |
 `NCM_LIST_FONT` | å¦ | æ  | æ¸²ææ­æ²åè¡¨ä½¿ç¨çå­ä½ | |
 `NCM_MAX_NAME_LEN` | å¦ | `600` |
 æ­æ²åè¡¨ä¸­æ­ååçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | |
 `NCM_MAX_ARTIST_LEN` | å¦ | `400` |
-æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨
-åé `ç¹æ­ [æ­æ²å]` å³å¯ ## ð èç³» QQï¼3076823485 Telegramï¼
-[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
-?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
+æ­æ²åè¡¨ä¸­æ­æåçæå¤§ææ¬å®½åº¦ï¼åç´ ï¼ | ## ð ä½¿ç¨ ###
+æä»¤ - ç¹æ­ [æ­æ²å / é³ä¹ ID] - å«åï¼`ç½æäº`ã`wyy` - è§£æ
+<åå¤ é³ä¹å¡ç /
+é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­æ¾é¾æ¥å¹¶ä½¿ç¨èªå®ä¹å¡çåéï¼ -
+å«åï¼`resolve`ã`parse`ã`get` - æ­è¯ <åå¤ é³ä¹å¡ç /
+é¾æ¥>ï¼è·åè¯¥é³ä¹çæ­è¯ï¼ - å«åï¼`lrc`ã`lyric`ã`lyrics` -
+é¾æ¥ <åå¤ é³ä¹å¡ç / é¾æ¥>ï¼è·åè¯¥é³ä¹çç½æäºé¾æ¥ï¼ -
+å«åï¼`link` ### Tip - ç¹å» Bot
+åéçé³ä¹å¡çå¯ä»¥è·³è½¬ç´é¾ï¼å¯ä»¥ç´æ¥ä¸è½½è¯¥é³ä¹ ## ð
+èç³» QQï¼3076823485 Telegramï¼[@lgc2333](https://t.me/lgc2333) å¹æ°´ç¾¤ï¼
+[1105946125](https://jq.qq.com/?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [MeetWq/pil-utils](https://github.com/MeetWq/pil-
 utils) è¶å¥½ç¨ç Pillow è¾å©åº ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.2.0 - æ°å¢äºä¸ä¸ªæä»¤
+`è§£æ`ã`æ­è¯`ã`é¾æ¥` - ç¹æ­æä»¤æ¯æç´æ¥è¾å¥é³ä¹ ID
```

