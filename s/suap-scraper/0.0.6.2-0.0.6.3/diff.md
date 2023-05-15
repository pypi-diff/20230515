# Comparing `tmp/suap_scraper-0.0.6.2.tar.gz` & `tmp/suap_scraper-0.0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suap_scraper-0.0.6.2.tar", last modified: Mon May 15 16:47:49 2023, max compression
+gzip compressed data, was "suap_scraper-0.0.6.3.tar", last modified: Mon May 15 20:54:07 2023, max compression
```

## Comparing `suap_scraper-0.0.6.2.tar` & `suap_scraper-0.0.6.3.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/
--rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.2/LICENSE.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.2/README.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      638 2023-05-15 16:47:05.000000 suap_scraper-0.0.6.2/pyproject.toml
--rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/setup.cfg
--rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6.2/setup.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.346771 suap_scraper-0.0.6.2/suap_scraper/
--rw-rw-r--   0 dom       (1000) dom       (1000)     4081 2023-05-15 16:39:57.000000 suap_scraper-0.0.6.2/suap_scraper/SUAP.py
--rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6.2/suap_scraper/__init__.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-05-06 18:49:43.000000 suap_scraper-0.0.6.2/suap_scraper/config.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1043 2023-05-07 11:07:39.000000 suap_scraper-0.0.6.2/suap_scraper/envio.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1085 2023-05-14 23:34:55.000000 suap_scraper-0.0.6.2/suap_scraper/sla.py
--rw-rw-r--   0 dom       (1000) dom       (1000)      385 2023-05-15 14:06:00.000000 suap_scraper-0.0.6.2/suap_scraper/teste.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     2730 2023-05-15 16:39:57.000000 suap_scraper-0.0.6.2/suap_scraper/utils.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.366771 suap_scraper-0.0.6.2/suap_scraper.egg-info/
--rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)      378 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       17 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/requires.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 20:54:07.105275 suap_scraper-0.0.6.3/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.3/LICENSE.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 20:54:07.105275 suap_scraper-0.0.6.3/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.3/README.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      638 2023-05-15 20:48:58.000000 suap_scraper-0.0.6.3/pyproject.toml
+-rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-15 20:54:07.105275 suap_scraper-0.0.6.3/setup.cfg
+-rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6.3/setup.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 20:54:07.093275 suap_scraper-0.0.6.3/suap_scraper/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     3447 2023-05-15 20:41:04.000000 suap_scraper-0.0.6.3/suap_scraper/SUAP.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6.3/suap_scraper/__init__.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1693 2023-05-15 20:43:19.000000 suap_scraper-0.0.6.3/suap_scraper/config.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     2730 2023-05-15 18:25:38.000000 suap_scraper-0.0.6.3/suap_scraper/utils.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 20:54:07.101275 suap_scraper-0.0.6.3/suap_scraper.egg-info/
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 20:54:07.000000 suap_scraper-0.0.6.3/suap_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)      314 2023-05-15 20:54:07.000000 suap_scraper-0.0.6.3/suap_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-15 20:54:07.000000 suap_scraper-0.0.6.3/suap_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       17 2023-05-15 20:54:07.000000 suap_scraper-0.0.6.3/suap_scraper.egg-info/requires.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-15 20:54:07.000000 suap_scraper-0.0.6.3/suap_scraper.egg-info/top_level.txt
```

### Comparing `suap_scraper-0.0.6.2/LICENSE.md` & `suap_scraper-0.0.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.2/PKG-INFO` & `suap_scraper-0.0.6.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap_scraper
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `suap_scraper-0.0.6.2/pyproject.toml` & `suap_scraper-0.0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "suap_scraper"
-version = "0.0.6.2"
+version = "0.0.6.3"
 authors = [
   { name="Jao42", email="cavalcante.joao@protonmail.ch" },
 ]
 description = "Um scraper para o SUAP do IFPB"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `suap_scraper-0.0.6.2/suap_scraper/SUAP.py` & `suap_scraper-0.0.6.3/suap_scraper/SUAP.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import httpx
 import asyncio
+from selectolax.parser import HTMLParser
 import sys
 from suap_scraper.utils import parsear_boletim
 import json
-import time
 import os
 from suap_scraper.config import *
 
 
 class LoginError(Exception):
   """
   Gerar mensagens de erro ao n conseguir logar
@@ -97,39 +97,18 @@
 
     return [ session_id, csrf ]
 
   async def __getBoletimPage(self):
     if self.matricula is None:
       logged = await self.__getInitialPage()
       self.matricula = logged.headers.get('user')
-    req_json = REQ_JSON_BOLETIM
-    req_json["referrer"] = (LINK_SUAP + "/edu/aluno/"
-    + str(self.matricula)
-    + "/?tab=boletim"
-    )
-
-    req = self.session.build_request("GET",
-                           LINK_SUAP + "/edu/aluno/"
-                           +str(self.matricula)
-                           +"/?tab=boletim",
-                           cookies={
-                             'sessionid': self.session_id,
-                             'csrftoken': self.csrf
-                           },
-                           headers=HEADER_BOLETIM,
-                           json=req_json
-                           )
-    res = ''
-    html_content = ''
-    while req is not None:
-      res = await self.session.send(req)
-      req = res.next_request
-    html_content = res.text
 
-    return html_content
+    res = await self.session.get(LINK_SUAP + "/edu/aluno/" + str(self.matricula) +"/?tab=boletim")
+    boletim_html = res.text
+    return boletim_html
 
   async def __createBoletimJSON(self, html_content):
     dic_materias = await parsear_boletim(html_content, self.session)
     boletim_json = json.dumps(
       dic_materias, sort_keys=True, indent=2, ensure_ascii=False
     )
```

### Comparing `suap_scraper-0.0.6.2/suap_scraper/config.py` & `suap_scraper-0.0.6.3/suap_scraper/config.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-UA_PADRAO = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/58.0.3029.110 Safari/537.36.'}
+UA_PADRAO = {'User-Agent': 'Oi, eu sou um bot que raspa o SUAP do IFPB. Disponivel em: https://github.com/Jao42/suap-scraper'}
 
 HEADER_LOGIN = {
   "accept": "text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9",
   "accept-language": "pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7",
   "cache-control": "max-age=0",
   "content-type": "application/x-www-form-urlencoded",
   "sec-fetch-dest": "document",
```

### Comparing `suap_scraper-0.0.6.2/suap_scraper/utils.py` & `suap_scraper-0.0.6.3/suap_scraper/utils.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.2/suap_scraper.egg-info/PKG-INFO` & `suap_scraper-0.0.6.3/suap_scraper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap-scraper
-Version: 0.0.6.2
+Version: 0.0.6.3
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

