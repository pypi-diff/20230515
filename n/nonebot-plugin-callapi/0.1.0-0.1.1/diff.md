# Comparing `tmp/nonebot_plugin_callapi-0.1.0.tar.gz` & `tmp/nonebot_plugin_callapi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_callapi-0.1.0.tar", last modified: Sat May  6 20:19:39 2023, max compression
+gzip compressed data, was "nonebot_plugin_callapi-0.1.1.tar", last modified: Mon May 15 19:23:00 2023, max compression
```

## Comparing `nonebot_plugin_callapi-0.1.0.tar` & `nonebot_plugin_callapi-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-06 20:19:26.286293 nonebot_plugin_callapi-0.1.0/LICENSE
--rw-r--r--   0        0        0     4575 2023-05-06 20:19:26.286293 nonebot_plugin_callapi-0.1.0/README.md
--rw-r--r--   0        0        0      304 2023-05-06 20:19:26.286293 nonebot_plugin_callapi-0.1.0/nonebot_plugin_callapi/__init__.py
--rw-r--r--   0        0        0     7944 2023-05-06 20:19:26.286293 nonebot_plugin_callapi-0.1.0/nonebot_plugin_callapi/__main__.py
--rw-r--r--   0        0        0      197 2023-05-06 20:19:26.286293 nonebot_plugin_callapi-0.1.0/nonebot_plugin_callapi/config.py
--rw-r--r--   0        0        0      830 2023-05-06 20:19:39.622483 nonebot_plugin_callapi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5471 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4572 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/README.md
+-rw-r--r--   0        0        0      304 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__init__.py
+-rw-r--r--   0        0        0     8442 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__main__.py
+-rw-r--r--   0        0        0      197 2023-05-15 19:22:49.226889 nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/config.py
+-rw-r--r--   0        0        0      838 2023-05-15 19:23:00.803087 nonebot_plugin_callapi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5476 1970-01-01 00:00:00.000000 nonebot_plugin_callapi-0.1.1/PKG-INFO
```

### Comparing `nonebot_plugin_callapi-0.1.0/LICENSE` & `nonebot_plugin_callapi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_callapi-0.1.0/README.md` & `nonebot_plugin_callapi-0.1.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
-# nonebot-plugin-callapi
+# NoneBot-Plugin-CallAPI
 
 _✨ 使用指令来调用 Bot 的 API ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
@@ -105,17 +105,17 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|    配置项     | 必填 | 默认值 | 说明                                                                                                                                                                          |
-| :-----------: | :--: | :----: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `CALLAPI_PIC` |  否  | `True` | API 调用结果是否生成为图片<br />Tip: 除 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 支持的平台 以及 Telegram 外，<br />调用结果只能发送为纯文本 |
+|    配置项     | 必填 | 默认值 | 说明                                                                                                                                                                       |
+| :-----------: | :--: | :----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `CALLAPI_PIC` |  否  | `True` | API 调用结果是否生成为图片<br />Tip: 只有 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 支持的平台才能发送图片，<br />其他平台只能发送为纯文本 |
 
 ## 🎉 使用
 
 ### 指令
 
 插件指令仅限 `SUPERUSER` 调用
 
@@ -156,8 +156,10 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 修复文本类 Segment 未做转义处理的问题
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
-# nonebot-plugin-callapi _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
+# NoneBot-Plugin-CallAPI _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
                            [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ä½¿ç¨ Bot æä»¤æ¥ç´æ¥è°ç¨ Bot ç API å§ï¼
 æ¬æä»¶çè®ºä¸å¼å®¹ä»»ä½ééå¨~ ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
 ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-callapi ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
@@ -15,19 +15,19 @@
 conda install nonebot-plugin-callapi ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç `plugins`
 é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_callapi" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
 è¯´æ | | :-----------: | :--: | :----: | :-----------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------- | | `CALLAPI_PIC` |
-å¦ | `True` | API è°ç¨ç»ææ¯å¦çæä¸ºå¾ç
-Tip: é¤ [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-
-anywhere) æ¯æçå¹³å° ä»¥å Telegram å¤ï¼
-è°ç¨ç»æåªè½åéä¸ºçº¯ææ¬ | ## ð ä½¿ç¨ ### æä»¤
+------------------------------------------------------- | | `CALLAPI_PIC` | å¦
+| `True` | API è°ç¨ç»ææ¯å¦çæä¸ºå¾ç
+Tip: åªæ [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-
+anywhere) æ¯æçå¹³å°æè½åéå¾çï¼
+å¶ä»å¹³å°åªè½åéä¸ºçº¯ææ¬ | ## ð ä½¿ç¨ ### æä»¤
 æä»¶æä»¤ä»é `SUPERUSER` è°ç¨ ![intro](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/callapi/intro.png) ###
 ææå¾ ![preview](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/
 callapi/preview.png) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ITCraftDevelopmentTeam/XDbot2](https://github.com/
@@ -35,9 +35,9 @@
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
+æªåè½¬ä¹å¤ççé®é¢
```

### Comparing `nonebot_plugin_callapi-0.1.0/nonebot_plugin_callapi/__main__.py` & `nonebot_plugin_callapi-0.1.1/nonebot_plugin_callapi/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import json
 import traceback
 from contextlib import suppress
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Tuple, Union, cast
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union, cast
 
 from bbcode import Parser as BBCodeParser
 from nonebot import on_command, require
-from nonebot.internal.adapter import Bot, Event, Message
+from nonebot.internal.adapter import Bot, Message, MessageSegment
 from nonebot.log import logger
-from nonebot.matcher import Matcher
+from nonebot.matcher import Matcher, current_bot, current_event
 from nonebot.params import CommandArg
 from nonebot.permission import SUPERUSER
 from PIL import Image
 from pil_utils import BuildImage, Text2Image
 from pil_utils.fonts import DEFAULT_FALLBACK_FONTS
 from pydantic import BaseModel
 from pygments import highlight
 from pygments.formatters import BBCodeFormatter
 from pygments.lexers import get_lexer_by_name
 from pygments.style import Style
 
-from .config import config
-
 try:
-    from nonebot.adapters.telegram import Event as TgEvent
+    from nonebot.adapters.telegram.event import MessageEvent as TgMsgEvent
     from nonebot.adapters.telegram.message import File as TgFile
 except ImportError:
     TgEvent = None
 
+from .config import config
+
 require("nonebot_plugin_saa")
 from nonebot_plugin_saa import Image as SAAImage  # noqa: E402
-from nonebot_plugin_saa import MessageFactory, extract_target  # noqa: E402
+from nonebot_plugin_saa import MessageFactory  # noqa: E402
 
 CODE_FONTS = [
     "JetBrains Mono",
     "Cascadia Mono",
     "Segoe UI Mono",
     "Liberation Mono",
     "Menlo",
@@ -100,37 +100,33 @@
 
         if not formatted:
             formatted = item.content
 
     text_img = Text2Image.from_bbcode_text(
         formatted,
         fallback_fonts=CODE_FONTS,
-    ).to_image()
+    )
 
     if not is_codeblock:
-        img = text_img
-
-    else:
-        block_size = (text_img.width + PADDING * 2, text_img.height + PADDING * 2)
-        block_width, block_height = block_size
-
-        build_img = BuildImage.new("RGBA", block_size, (255, 255, 255, 0))
+        return text_img.to_image()
 
-        if background_color:
-            build_img.draw_rounded_rectangle(
-                (0, 0, block_width, block_height),
-                radius=10,
-                fill=background_color,
-            )
+    block_size = (text_img.width + PADDING * 2, text_img.height + PADDING * 2)
+    block_width, block_height = block_size
 
-        build_img.paste(text_img, (PADDING, PADDING), alpha=True)
+    build_img = BuildImage.new("RGBA", block_size, (255, 255, 255, 0))
 
-        img = build_img.image
+    if background_color:
+        build_img.draw_rounded_rectangle(
+            (0, 0, block_width, block_height),
+            radius=10,
+            fill=background_color,
+        )
 
-    return img
+    text_img.draw_on_image(build_img.image, (PADDING, PADDING))
+    return build_img.image
 
 
 def draw_image(items: List[Union[str, Codeblock]]) -> bytes:
     images = [item_to_image(it) for it in items]
 
     width = max(img.width for img in images)
     height = sum(img.height for img in images)
@@ -144,27 +140,45 @@
     for img in images:
         bg.paste(img, (PADDING, y), alpha=True)
         y += img.height
 
     return bg.convert("RGB").save("png").getvalue()
 
 
-async def send_return(bot: Bot, event: Event, items: List[Union[str, Codeblock]]):
+# async def send_return(items: List[Union[str, Codeblock]]):
+#     if config.callapi_pic:
+#         with suppress(Exception):
+#             image = draw_image(items)
+#             await MessageFactory(SAAImage(image)).send(reply=True)
+#             return
+
+#     event = current_event.get()
+#     bot = current_bot.get()
+#     await bot.send(event, format_plain_text(items))
+
+
+async def send_return(items: List[Union[str, Codeblock]]):
+    event = current_event.get()
+    bot = current_bot.get()
+
     if config.callapi_pic:
         with suppress(Exception):
-            if TgEvent and isinstance(event, TgEvent):
+            if TgEvent and isinstance(event, TgMsgEvent):
                 # telegram
                 image = draw_image(items)
-                await bot.send(event, TgFile.photo(image))
+                await bot.send(
+                    event,
+                    TgFile.photo(image),
+                    reply_to_message_id=event.message_id,
+                )
 
             else:
                 # via saa
-                target = extract_target(event)
                 image = draw_image(items)
-                await MessageFactory(SAAImage(image)).send_to(target, bot=bot)
+                await MessageFactory(SAAImage(image)).send(reply=True)
 
             return
 
     await bot.send(event, format_plain_text(items))
 
 
 def cast_param_type(param: str) -> Any:
@@ -201,16 +215,15 @@
 
     return api_name, param_dict
 
 
 HELP_ITEMS = [
     "[b]指令格式：[/b]",
     Codeblock(lang=None, content="callapi <API 名称>\n[传入参数]"),
-    "其中，传入参数可以为一行一个的 name=value 格式的参数，也可以直接写一串 JSON",
-    "详见下面的调用示例",
+    "关于传入参数的格式，请看下面的调用示例",
     "",
     "[b]调用示例：[/b]",
     "使用 name=value 格式（会自动推断类型）：",
     Codeblock(
         lang=None,
         content=(
             "callapi get_stranger_info\n"
@@ -229,19 +242,24 @@
 HELP_TEXT = format_plain_text(HELP_ITEMS)
 
 
 call_api_matcher = on_command("callapi", permission=SUPERUSER)
 
 
 @call_api_matcher.handle()
-async def _(matcher: Matcher, bot: Bot, event: Event, args: Message = CommandArg()):
-    arg_txt = str(args).strip()
+async def _(matcher: Matcher, bot: Bot, args: Message = CommandArg()):
+    arg_txt = "".join(
+        [
+            txt if x.is_text() and (txt := x.data.get("text")) else str(x)
+            for x in cast(Iterable[MessageSegment], args)
+        ],
+    ).strip()
 
     if not arg_txt:
-        await send_return(bot, event, HELP_ITEMS)
+        await send_return(HELP_ITEMS)
         return
 
     try:
         api, params_dict = parse_args(arg_txt)
     except ValueError as e:
         await matcher.finish(e.args[0])
     except Exception:
@@ -280,8 +298,8 @@
         ret_items.append(
             Codeblock(
                 lang="json" if content else None,
                 content=content or str(result),
             ),
         )
 
-    await send_return(bot, event, ret_items)
+    await send_return(ret_items)
```

### Comparing `nonebot_plugin_callapi-0.1.0/PKG-INFO` & `nonebot_plugin_callapi-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-callapi
-Version: 0.1.0
-Summary: Template plugin project
+Version: 0.1.1
+Summary: Use bot command to call its API
 Home-page: https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Author-Email: student_2333 <lgc2333@126.com>
 License: MIT
 Project-URL: Homepage, https://github.com/lgc-NB2Dev/nonebot-plugin-callapi
 Requires-Python: <4.0,>=3.8
 Requires-Dist: nonebot2>=2.0.0-rc.1
 Requires-Dist: nonebot-adapter-onebot>=2.2.0
@@ -30,15 +30,15 @@
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo">
 </a>
 
 <p>
   <img src="https://raw.githubusercontent.com/A-kirami/nonebot-plugin-template/resources/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText">
 </p>
 
-# nonebot-plugin-callapi
+# NoneBot-Plugin-CallAPI
 
 _✨ 使用指令来调用 Bot 的 API ✨_
 
 <img src="https://img.shields.io/badge/python-3.8+-blue.svg" alt="python">
 <a href="https://pdm.fming.dev">
   <img src="https://img.shields.io/badge/pdm-managed-blueviolet" alt="pdm-managed">
 </a>
@@ -129,17 +129,17 @@
 
 </details>
 
 ## ⚙️ 配置
 
 在 nonebot2 项目的 `.env` 文件中添加下表中的必填配置
 
-|    配置项     | 必填 | 默认值 | 说明                                                                                                                                                                          |
-| :-----------: | :--: | :----: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
-| `CALLAPI_PIC` |  否  | `True` | API 调用结果是否生成为图片<br />Tip: 除 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 支持的平台 以及 Telegram 外，<br />调用结果只能发送为纯文本 |
+|    配置项     | 必填 | 默认值 | 说明                                                                                                                                                                       |
+| :-----------: | :--: | :----: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
+| `CALLAPI_PIC` |  否  | `True` | API 调用结果是否生成为图片<br />Tip: 只有 [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-anywhere) 支持的平台才能发送图片，<br />其他平台只能发送为纯文本 |
 
 ## 🎉 使用
 
 ### 指令
 
 插件指令仅限 `SUPERUSER` 调用
 
@@ -180,8 +180,10 @@
 
   ![讨饭](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/imgs/sponsor.png)
 
   </details>
 
 ## 📝 更新日志
 
-芝士刚刚发布的插件，还没有更新日志的说 qwq~
+### 0.1.1
+
+- 修复文本类 Segment 未做转义处理的问题
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.0 Summary:
-Template plugin project Home-page: https://github.com/lgc-NB2Dev/nonebot-
+Metadata-Version: 2.1 Name: nonebot-plugin-callapi Version: 0.1.1 Summary: Use
+bot command to call its API Home-page: https://github.com/lgc-NB2Dev/nonebot-
 plugin-callapi Author-Email: student_2333
 126.com> License: MIT Project-URL: Homepage, https://github.com/lgc-NB2Dev/
 nonebot-plugin-callapi Requires-Python: <4.0,>=3.8 Requires-Dist:
 nonebot2>=2.0.0-rc.1 Requires-Dist: nonebot-adapter-onebot>=2.2.0 Requires-
 Dist: pydantic>=1.10.4 Requires-Dist: Pygments>=2.15.1 Requires-Dist: pil-
 utils>=0.1.7 Requires-Dist: nonebot-plugin-send-anything-anywhere>=0.2.4
 Requires-Dist: pip>=23.0.1; extra == "dev" Requires-Dist: setuptools>=67.6.1;
 extra == "dev" Requires-Dist: nb-cli>=1.0.5; extra == "dev" Requires-Dist:
 black>=23.3.0; extra == "dev" Requires-Dist: ruff>=0.0.260; extra == "dev"
 Requires-Dist: isort>=5.12.0; extra == "dev" Provides-Extra: dev Description-
 Content-Type: text/markdown
                               [NoneBotPluginLogo]
                               [NoneBotPluginText]
-# nonebot-plugin-callapi _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
+# NoneBot-Plugin-CallAPI _â¨ ä½¿ç¨æä»¤æ¥è°ç¨ Bot ç API â¨_ [python]
                            [pdm-managed] [wakatime]
                        [license] [pypi] [pypi_download]
 ## ð ä»ç» ä½¿ç¨ Bot æä»¤æ¥ç´æ¥è°ç¨ Bot ç API å§ï¼
 æ¬æä»¶çè®ºä¸å¼å®¹ä»»ä½ééå¨~ ## ð¿ å®è£ ä»¥ä¸æå°çæ¹æ³
 ä»»é**å¶ä¸** å³å¯  [æ¨è] ä½¿ç¨ nb-cli å®è£ å¨ nonebot2
 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡, è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ ```bash nb
 plugin install nonebot-plugin-callapi ```   ä½¿ç¨åç®¡çå¨å®è£ å¨
@@ -28,19 +28,19 @@
 conda install nonebot-plugin-callapi ```  æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åç `plugins`
 é¡¹éè¿½å åå¥ ```toml [tool.nonebot] plugins = [ # ...
 "nonebot_plugin_callapi" ] ```  ## âï¸ éç½® å¨ nonebot2 é¡¹ç®ç `.env`
 æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« | é»è®¤å¼ |
 è¯´æ | | :-----------: | :--: | :----: | :-----------------------------------
 -------------------------------------------------------------------------------
----------------------------------------------------------- | | `CALLAPI_PIC` |
-å¦ | `True` | API è°ç¨ç»ææ¯å¦çæä¸ºå¾ç
-Tip: é¤ [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-
-anywhere) æ¯æçå¹³å° ä»¥å Telegram å¤ï¼
-è°ç¨ç»æåªè½åéä¸ºçº¯ææ¬ | ## ð ä½¿ç¨ ### æä»¤
+------------------------------------------------------- | | `CALLAPI_PIC` | å¦
+| `True` | API è°ç¨ç»ææ¯å¦çæä¸ºå¾ç
+Tip: åªæ [SAA](https://github.com/felinae98/nonebot-plugin-send-anything-
+anywhere) æ¯æçå¹³å°æè½åéå¾çï¼
+å¶ä»å¹³å°åªè½åéä¸ºçº¯ææ¬ | ## ð ä½¿ç¨ ### æä»¤
 æä»¶æä»¤ä»é `SUPERUSER` è°ç¨ ![intro](https://
 raw.githubusercontent.com/lgc-NB2Dev/readme/main/callapi/intro.png) ###
 ææå¾ ![preview](https://raw.githubusercontent.com/lgc-NB2Dev/readme/main/
 callapi/preview.png) ## ð èç³» QQï¼3076823485 Telegramï¼[@lgc2333]
 (https://t.me/lgc2333) å¹æ°´ç¾¤ï¼[1105946125](https://jq.qq.com/
 ?_wv=1027&k=Z3n1MpEp) é®ç®±ï¼
 126.com> ## ð¡ é¸£è°¢ ### [ITCraftDevelopmentTeam/XDbot2](https://github.com/
@@ -48,9 +48,9 @@
 github.com/MeetWq/pil-utils) è¶å¥½ç¨ç Pillow è¾å©åº ### [felinae98/
 nonebot-plugin-send-anything-anywhere](https://github.com/felinae98/nonebot-
 plugin-send-anything-anywhere)
 å¤ééå¨æ¶æ¯åéæ¯æï¼æ¬æä»¶ç¨æ¥åéå¾çï¼ ## ð° èµå©
 æè°¢å¤§å®¶çèµå©ï¼ä½ ä»¬çèµå©å°æ¯æç»§ç»­åä½çå¨åï¼ -
 [ç±åçµ](https://afdian.net/@lgc2333) -  èµå©äºç»´ç ï¼ç¹å»å±å¼ï¼ !
 [è®¨é¥­](https://raw.githubusercontent.com/lgc2333/ShigureBotMenu/master/src/
-imgs/sponsor.png)  ## ð æ´æ°æ¥å¿
-èå£«åååå¸çæä»¶ï¼è¿æ²¡ææ´æ°æ¥å¿çè¯´ qwq~
+imgs/sponsor.png)  ## ð æ´æ°æ¥å¿ ### 0.1.1 - ä¿®å¤ææ¬ç±» Segment
+æªåè½¬ä¹å¤ççé®é¢
```

