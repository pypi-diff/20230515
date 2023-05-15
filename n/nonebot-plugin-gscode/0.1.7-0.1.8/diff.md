# Comparing `tmp/nonebot_plugin_gscode-0.1.7.tar.gz` & `tmp/nonebot_plugin_gscode-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_gscode-0.1.7.tar", max compression
+gzip compressed data, was "nonebot_plugin_gscode-0.1.8.tar", max compression
```

## Comparing `nonebot_plugin_gscode-0.1.7.tar` & `nonebot_plugin_gscode-0.1.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-05-13 17:01:10.822822 nonebot_plugin_gscode-0.1.7/LICENSE
--rw-r--r--   0        0        0     1950 2023-05-13 17:01:10.822822 nonebot_plugin_gscode-0.1.7/README.md
--rw-r--r--   0        0        0     1032 2023-05-13 17:01:10.822822 nonebot_plugin_gscode-0.1.7/nonebot_plugin_gscode/__init__.py
--rw-r--r--   0        0        0     5219 2023-05-13 17:01:10.822822 nonebot_plugin_gscode-0.1.7/nonebot_plugin_gscode/data_source.py
--rw-r--r--   0        0        0     1739 2023-05-13 17:01:10.822822 nonebot_plugin_gscode-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1950 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/README.md
+-rw-r--r--   0        0        0     1028 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/__init__.py
+-rw-r--r--   0        0        0     6805 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/data_source.py
+-rw-r--r--   0        0        0     1739 2023-05-15 12:04:42.661528 nonebot_plugin_gscode-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2780 1970-01-01 00:00:00.000000 nonebot_plugin_gscode-0.1.8/PKG-INFO
```

### Comparing `nonebot_plugin_gscode-0.1.7/LICENSE` & `nonebot_plugin_gscode-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.1.7/README.md` & `nonebot_plugin_gscode-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_gscode-0.1.7/nonebot_plugin_gscode/__init__.py` & `nonebot_plugin_gscode-0.1.8/nonebot_plugin_gscode/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from nonebot.typing import T_State
 from nonebot.adapters.onebot.v11 import Bot
 from nonebot.plugin import PluginMetadata, on_command
 from nonebot.adapters.onebot.v11.event import MessageEvent, GroupMessageEvent
 
-from .data_source import getCodes
+from .data_source import getMsg
 
 __plugin_meta__ = PluginMetadata(
     name="GsCode",
     description="查询原神前瞻直播兑换码",
     usage="""查询原神前瞻直播兑换码
 注意：经测试，兑换码接口返回与前瞻直播有 2 分钟左右延迟，应为正常现象，请耐心等待。
 /gscode
@@ -17,12 +17,12 @@
 codeMatcher = on_command("gscode", aliases={"兑换码"}, priority=5)
 
 
 @codeMatcher.handle()
 async def _(bot: Bot, event: MessageEvent, state: T_State):
     if str(state["_prefix"]["command_arg"]):
         await codeMatcher.finish()
-    codes = await getCodes()
+    codes = await getMsg()
     if isinstance(event, GroupMessageEvent):
         await bot.send_group_forward_msg(group_id=event.group_id, messages=codes)
     else:
         await bot.send_private_forward_msg(user_id=event.user_id, messages=codes)
```

### Comparing `nonebot_plugin_gscode-0.1.7/pyproject.toml` & `nonebot_plugin_gscode-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nonebot-plugin-gscode"
-version = "0.1.7"
+version = "0.1.8"
 description = "Genshin live codes plugin for NoneBot2"
 authors = ["monsterxcn <monsterxcn@gmail.com>"]
 documentation = "https://github.com/monsterxcn/nonebot-plugin-gscode#readme"
 license = "MIT"
 homepage = "https://github.com/monsterxcn/nonebot-plugin-gscode"
 readme = "README.md"
 keywords = ["nonebot", "nonebot2", "genshin", "live", "code", "redeem"]
```

### Comparing `nonebot_plugin_gscode-0.1.7/PKG-INFO` & `nonebot_plugin_gscode-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-gscode
-Version: 0.1.7
+Version: 0.1.8
 Summary: Genshin live codes plugin for NoneBot2
 Home-page: https://github.com/monsterxcn/nonebot-plugin-gscode
 License: MIT
 Keywords: nonebot,nonebot2,genshin,live,code,redeem
 Author: monsterxcn
 Author-email: monsterxcn@gmail.com
 Requires-Python: >=3.8.1,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-gscode Version: 0.1.8 Summary:
 Genshin live codes plugin for NoneBot2 Home-page: https://github.com/
 monsterxcn/nonebot-plugin-gscode License: MIT Keywords:
 nonebot,nonebot2,genshin,live,code,redeem Author: monsterxcn Author-email:
 monsterxcn@gmail.com Requires-Python: >=3.8.1,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

