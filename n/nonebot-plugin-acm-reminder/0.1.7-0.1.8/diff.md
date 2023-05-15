# Comparing `tmp/nonebot-plugin-acm-reminder-0.1.7.tar.gz` & `tmp/nonebot-plugin-acm-reminder-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.7.tar", last modified: Sat Apr 29 14:08:23 2023, max compression
+gzip compressed data, was "nonebot-plugin-acm-reminder-0.1.8.tar", last modified: Mon May 15 11:31:06 2023, max compression
```

## Comparing `nonebot-plugin-acm-reminder-0.1.7.tar` & `nonebot-plugin-acm-reminder-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.7/LICENSE
--rw-r--r--   0        0        0     3028 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/__init__.py
--rw-r--r--   0        0        0      228 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/config.py
--rw-r--r--   0        0        0     3706 2023-04-29 14:08:14.618792 nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/data_source.py
--rw-r--r--   0        0        0      636 2023-04-29 14:08:14.618792 nonebot-plugin-acm-reminder-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.7/README.md
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-01-15 11:05:12.918513 nonebot-plugin-acm-reminder-0.1.8/LICENSE
+-rw-r--r--   0        0        0     3353 2023-05-15 11:29:35.875350 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-30 14:06:17.044896 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/config.py
+-rw-r--r--   0        0        0     4017 2023-05-15 11:25:53.437244 nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/data_source.py
+-rw-r--r--   0        0        0      636 2023-05-15 11:30:58.511125 nonebot-plugin-acm-reminder-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      852 2023-04-06 15:33:46.324195 nonebot-plugin-acm-reminder-0.1.8/README.md
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 nonebot-plugin-acm-reminder-0.1.8/PKG-INFO
```

### Comparing `nonebot-plugin-acm-reminder-0.1.7/LICENSE` & `nonebot-plugin-acm-reminder-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/__init__.py` & `nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from typing import List
-from httpx import URL
 from nonebot.adapters.onebot.v11 import MessageEvent, MessageSegment
 from nonebot.plugin import on_command, PluginMetadata
-from nonebot import get_driver, require
+from nonebot import get_driver, logger, require
 
 
 from .config import Config
 from .data_source import ContestType, req_get, html_parse_cf, html_parse_nc
 
 require("nonebot_plugin_apscheduler")
 require("nonebot_plugin_htmlrender")
@@ -39,31 +38,40 @@
     更新比赛信息
     """
     contest_data.clear()
     contest_data.extend(html_parse_cf(await req_get("https://codeforces.com/contests")))
     contest_data.extend(html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=13")))
     contest_data.extend(html_parse_nc(await req_get("https://ac.nowcoder.com/acm/contest/vip-index?topCategoryFilter=14")))
 
-
 @scheduler.scheduled_job('interval', minutes=plugin_config.update_time, id="update_contest")
 async def update_contest():
-    await update()
+    try:
+        await update()
+    except Exception as e:
+        logger.warning("拉取竞赛信息更新失败!")
+        logger.warning(e)
 
 
 @driver.on_startup
 async def startup():
-    await update()
+    try:
+        await update()
+    except Exception as e:
+        logger.warning("拉取竞赛信息更新失败!")
+        logger.warning(e)
     # 防止因为网络问题导致机器人启动失败
 
 
 @contest_update.handle()
 async def update_handle(event: MessageEvent):
     try:
         await update()
     except Exception as e:
+        logger.warning("拉取竞赛信息更新失败!")
+        logger.warning(e)
         await contest_update.finish(MessageSegment.image(await md_to_pic(f"更新失败 {e}")))
 
     await contest_update.finish("更新成功")
 
 
 @contest_list.handle()
 async def get_list(event: MessageEvent):
```

### Comparing `nonebot-plugin-acm-reminder-0.1.7/nonebot_plugin_acm_reminder/data_source.py` & `nonebot-plugin-acm-reminder-0.1.8/nonebot_plugin_acm_reminder/data_source.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from json import loads
-from time import strptime, mktime
+from time import strptime, mktime, struct_time
 from html import unescape
-from typing import Literal, Optional, TypedDict, List
-from httpx import AsyncClient
+from typing import Any, Dict, Literal, Optional, TypedDict, List, Union
+from httpx import AsyncClient, Response
 from httpx._types import URLTypes, ProxiesTypes
-from bs4 import BeautifulSoup, ResultSet
+from bs4 import BeautifulSoup, NavigableString, ResultSet, Tag
 
 class ContestType(TypedDict):
     id: int  # 竞赛ID
     name: str  # 竞赛名称
     writes: List[str]  # 竞赛主办方
     length: int  # 竞赛时长 [分钟]
     time: float  # 竞赛开始时间戳
@@ -22,15 +22,15 @@
     Args:
         url (URLTypes): 对应的URL
 
     Returns:
         str: URL对应的HTML
     """
     async with AsyncClient(proxies=proxies) as client:
-        r = await client.get(url)
+        r: Response = await client.get(url)
     return r.content.decode("utf-8")
 
 def html_parse_cf(content: str) -> List[ContestType]:
     """
     处理Codeforces的竞赛列表
 
     Args:
@@ -38,30 +38,30 @@
 
     Returns:
         list: 竞赛列表
     """
     contest_data: List[ContestType] = []
     
     soup = BeautifulSoup(content, 'html.parser')
-    datatable = soup.find('div', class_='datatable')  # 获取到数据表
-    if datatable is None:
+    datatable: Union[Tag,NavigableString,None] = soup.find('div', class_='datatable')  # 获取到数据表
+    if not isinstance(datatable,Tag):
         return contest_data
 
     # 解析竞赛信息
-    contest_list = datatable.find_all("tr")  # type: ignore
+    contest_list: ResultSet[Any] = datatable.find_all("tr") 
     for contest in contest_list:
-        cdata = contest.find_all("td")
+        cdata: ResultSet[Any] = contest.find_all("td")
         if cdata:
-            cwriters = [i.string for i in cdata[1].find_all("a")] #获得主办方
-            ctime = mktime(strptime(cdata[2].find("span").string, "%b/%d/%Y %H:%M")) #获得开始时间戳
+            cwriters: List[str] = [i.string for i in cdata[1].find_all("a")] #获得主办方
+            ctime: float = mktime(strptime(cdata[2].find("span").string, "%b/%d/%Y %H:%M")) #获得开始时间戳
             ctime+=5*60*60
             try:
-                clength = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M")
+                clength: struct_time = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M")
             except:
-                clength = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M:%S")
+                clength: struct_time = strptime(str(cdata[3].string).strip("\n").strip(), "%H:%M:%S")
             contest_data.append({"name": str(cdata[0].string).strip("\n").strip(), 
                                 "writes": cwriters, 
                                 "time": ctime, 
                                 "length": clength.tm_hour * 60 + clength.tm_min, 
                                 "platform": "Codeforces", 
                                 "id": contest.get("data-contestid")})
     return contest_data
@@ -71,20 +71,23 @@
     处理牛客的竞赛列表 
 
     Args:
         content (str): HTML
 
     Returns:
         list: 竞赛列表
-    """
+    """ 
     contest_data: List[ContestType] = []
     soup = BeautifulSoup(content, 'html.parser')
-    datatable: ResultSet = soup.find('div', class_='platform-mod js-current').find_all('div', class_='platform-item js-item') #type: ignore
+    find_item: Union[Tag,NavigableString,None] = soup.find('div', class_='platform-mod js-current')
+    if not isinstance(find_item, Tag):
+        return contest_data
+    datatable: ResultSet = find_item.find_all('div', class_='platform-item js-item')
     for contest in datatable:
-        cdata = loads(unescape(contest.get("data-json")))
+        cdata: Dict[str, Any] = loads(unescape(contest.get("data-json")))
         if cdata:
             contest_data.append({"name": cdata["contestName"], 
                                 "writes": [cdata["settingInfo"]["organizerName"]], 
                                 "time":  cdata["contestStartTime"] / 1000, 
                                 "length": cdata["contestDuration"] / 1000 / 60, 
                                 "platform": "Nowcoder", 
                                 "id": cdata["contestId"]})
```

### Comparing `nonebot-plugin-acm-reminder-0.1.7/pyproject.toml` & `nonebot-plugin-acm-reminder-0.1.8/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "nonebot_plugin_acm_reminder"
-version = "0.1.7"
+version = "0.1.8"
 description = "A subscribe CodeForces/NowCoder contest info plugin for nonebot2"
 authors = [
     { name = "BigOrangeQWQ", email = "2284086963@qq.com" },
 ]
 dependencies = [
     "BeautifulSoup4>=4.11.2",
     "nonebot2>=2.0.0b5",
```

### Comparing `nonebot-plugin-acm-reminder-0.1.7/README.md` & `nonebot-plugin-acm-reminder-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-acm-reminder-0.1.7/PKG-INFO` & `nonebot-plugin-acm-reminder-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_acm_reminder
-Version: 0.1.7
+Version: 0.1.8
 Summary: A subscribe CodeForces/NowCoder contest info plugin for nonebot2
 License: MIT
 Author-email: BigOrangeQWQ <2284086963@qq.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.7 Summary:
+Metadata-Version: 2.1 Name: nonebot_plugin_acm_reminder Version: 0.1.8 Summary:
 A subscribe CodeForces/NowCoder contest info plugin for nonebot2 License: MIT
 Author-email: BigOrangeQWQ <2284086963@qq.com> Requires-Python: >=3.8
 Description-Content-Type: text/markdown
    # ACMReminder ä¸æ¬¾å¯æ¥è¯¢ä¸è®¢éçå®¢/CFç«èµçæä»¶ [Download]
 ## å®è£ ``` pip install nonebot-plugin-acm-reminder nb plugin install
 nonebot-plugin-acm-reminder ``` ## éç½®é¡¹ *
 æåç«èµåè¡¨çæ´æ°æ¶é´(åé) ``` update_time = 720 ``` ## ç¨æ³
```

