# Comparing `tmp/suap_scraper-0.0.6.tar.gz` & `tmp/suap_scraper-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suap_scraper-0.0.6.tar", last modified: Mon May  1 00:12:05 2023, max compression
+gzip compressed data, was "suap_scraper-0.0.6.1.tar", last modified: Mon May 15 01:15:19 2023, max compression
```

## Comparing `suap_scraper-0.0.6.tar` & `suap_scraper-0.0.6.1.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.838954 suap_scraper-0.0.6/
--rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6/LICENSE.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-05-01 00:12:05.834954 suap_scraper-0.0.6/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6/README.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      643 2023-05-01 00:10:46.000000 suap_scraper-0.0.6/pyproject.toml
--rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-01 00:12:05.838954 suap_scraper-0.0.6/setup.cfg
--rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6/setup.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.822954 suap_scraper-0.0.6/suap_scraper/
--rw-rw-r--   0 dom       (1000) dom       (1000)     3898 2023-04-30 23:47:13.000000 suap_scraper-0.0.6/suap_scraper/SUAP.py
--rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6/suap_scraper/__init__.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-04-30 18:34:44.000000 suap_scraper-0.0.6/suap_scraper/config.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     2289 2023-04-30 23:48:10.000000 suap_scraper-0.0.6/suap_scraper/utils.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-01 00:12:05.834954 suap_scraper-0.0.6/suap_scraper.egg-info/
--rw-rw-r--   0 dom       (1000) dom       (1000)      530 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)      314 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       24 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/requires.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-01 00:12:05.000000 suap_scraper-0.0.6/suap_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.1/LICENSE.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.1/README.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      642 2023-05-15 01:14:39.000000 suap_scraper-0.0.6.1/pyproject.toml
+-rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-15 01:15:19.100239 suap_scraper-0.0.6.1/setup.cfg
+-rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6.1/setup.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.088239 suap_scraper-0.0.6.1/suap_scraper/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     4067 2023-05-15 01:05:45.000000 suap_scraper-0.0.6.1/suap_scraper/SUAP.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6.1/suap_scraper/__init__.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-05-06 18:49:43.000000 suap_scraper-0.0.6.1/suap_scraper/config.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1043 2023-05-07 11:07:39.000000 suap_scraper-0.0.6.1/suap_scraper/envio.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1025 2023-05-15 00:55:36.000000 suap_scraper-0.0.6.1/suap_scraper/mensagem.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1755 2023-05-15 00:46:26.000000 suap_scraper-0.0.6.1/suap_scraper/novas_notas.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1085 2023-05-14 23:34:55.000000 suap_scraper-0.0.6.1/suap_scraper/sla.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)      293 2023-05-14 23:22:25.000000 suap_scraper-0.0.6.1/suap_scraper/teste.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)      966 2023-05-07 20:07:58.000000 suap_scraper-0.0.6.1/suap_scraper/teste_async.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     2807 2023-05-15 01:05:45.000000 suap_scraper-0.0.6.1/suap_scraper/utils.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/suap_scraper.egg-info/
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)      459 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       21 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/requires.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/top_level.txt
```

### Comparing `suap_scraper-0.0.6/LICENSE.md` & `suap_scraper-0.0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6/PKG-INFO` & `suap_scraper-0.0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap_scraper
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `suap_scraper-0.0.6/pyproject.toml` & `suap_scraper-0.0.6.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "suap_scraper"
-version = "0.0.6"
+version = "0.0.6.1"
 authors = [
   { name="Jao42", email="cavalcante.joao@protonmail.ch" },
 ]
 description = "Um scraper para o SUAP do IFPB"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
-    "requests",
+    "httpx",
     "beautifulsoup4",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `suap_scraper-0.0.6/suap_scraper/SUAP.py` & `suap_scraper-0.0.6.1/suap_scraper/SUAP.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import requests
+import httpx
+import asyncio
 import sys
 from bs4 import BeautifulSoup
 from suap_scraper.utils import parsear_boletim
 import json
 import time
 import os
 from suap_scraper.config import *
@@ -13,32 +14,32 @@
   Gerar mensagens de erro ao n conseguir logar
   """
 
 
 class SUAP:
   def __init__(self, user_agent=UA_PADRAO):
     self.user_agent = user_agent
-    self.session = requests.Session()
+    self.session = httpx.AsyncClient()
     self.session.headers.update(user_agent)
 
-  def loginCredenciais(self, matricula, senha, user_agent=UA_PADRAO):
+  async def loginCredenciais(self, matricula, senha, user_agent=UA_PADRAO):
     self.matricula = matricula
     self.senha = senha
-    self.session_id, self.csrf = self.__loginSUAP()
+    self.session_id, self.csrf = await self.__loginSUAP()
 
-  def loginSessionId(self, session_id, user_agent=UA_PADRAO):
+  async def loginSessionId(self, session_id, user_agent=UA_PADRAO):
     self.session_id = session_id
     self.session.cookies['sessionid'] = self.session_id
-    logged = self.__getInitialPage()
+    logged = await self.__getInitialPage()
     self.matricula = logged.headers.get('user')
     self.csrf = ''
     self.senha = ''
 
-  def __getInitialPage(self):
-    res = self.session.get(LINK_SUAP)
+  async def __getInitialPage(self):
+    res = await self.session.get(LINK_SUAP)
     return res
 
   def __getCookiesInitialPage(self, initial_page):
     soup = BeautifulSoup(initial_page.text, 'html.parser')
     middleware_csrf = soup.find(
       'input',
       attrs = {'name': 'csrfmiddlewaretoken'}
@@ -46,42 +47,41 @@
 
     csrf = initial_page.cookies['csrftoken']
     session_id = initial_page.cookies['sessionid']
 
     return [ middleware_csrf, csrf, session_id ]
 
 
-  def __loginSUAP(self, campo_captcha=False):
-    initial_page = self.__getInitialPage()
+  async def __loginSUAP(self, campo_captcha=False):
+    initial_page = await self.__getInitialPage()
     middleware_csrf, csrf, session_id = self.__getCookiesInitialPage(
       initial_page
     )
 
     body = ("csrfmiddlewaretoken=" + middleware_csrf +
     "&username=" + str(self.matricula) +
     "&password=" + self.senha +
     "&this_is_the_login_form=1&next="
     )
 
     if campo_captcha:
       body += "&g-recaptcha-response="
 
-    req = requests.Request("POST",
+    req = session.build_request("POST",
                            LINK_SUAP + "/accounts/login/?next=/",
                            headers=HEADER_LOGIN,
                            data=body,
                            json=REQ_JSON_LOGIN,
                            cookies={
                             'csrftoken': csrf,
                             'sessionid': session_id
                           }
                         )
 
-    req = req.prepare()
-    res = self.session.send(req)
+    res = await self.session.send(req)
 
     try:
       session_id = res.cookies['sessionid']
     except KeyError:
       soup = BeautifulSoup(res.text, 'html.parser')
       erro = soup.find(class_="errornote")
       if erro == None:
@@ -94,43 +94,46 @@
     try:
       csrf = res.cookies['csrftoken']
     except:
       pass
 
     return [ session_id, csrf ]
 
-  def __getBoletimPage(self):
+  async def __getBoletimPage(self):
     req_json = REQ_JSON_BOLETIM
     req_json["referrer"] = (LINK_SUAP + "/edu/aluno/"
     + str(self.matricula)
     + "/?tab=boletim"
     )
 
-    req = requests.Request("GET",
+    req = self.session.build_request("GET",
                            LINK_SUAP + "/edu/aluno/"
                            +str(self.matricula)
                            +"/?tab=boletim",
                            cookies={
                              'sessionid': self.session_id,
                              'csrftoken': self.csrf
                            },
                            headers=HEADER_BOLETIM,
                            json=req_json
                            )
-    req = req.prepare()
-    res = self.session.send(req)
+    res = ''
+    html_content = ''
+    while req is not None:
+      res = await self.session.send(req)
+      req = res.next_request
     html_content = res.text
 
     return html_content
 
-  def __createBoletimJSON(self, html_content):
-    dic_materias = parsear_boletim(html_content, self.session)
+  async def __createBoletimJSON(self, html_content):
+    dic_materias = await parsear_boletim(html_content, self.session)
     boletim_json = json.dumps(
       dic_materias, sort_keys=True, indent=2, ensure_ascii=False
     )
 
     return boletim_json
 
-  def getBoletim(self):
-    html_boletim = self.__getBoletimPage()
-    boletim = self.__createBoletimJSON(html_boletim)
+  async def getBoletim(self):
+    html_boletim = await self.__getBoletimPage()
+    boletim = await self.__createBoletimJSON(html_boletim)
     return boletim
```

### Comparing `suap_scraper-0.0.6/suap_scraper/config.py` & `suap_scraper-0.0.6.1/suap_scraper/config.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6/suap_scraper/utils.py` & `suap_scraper-0.0.6.1/suap_scraper/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,44 @@
 from bs4 import BeautifulSoup
 import sys
 import json
+import asyncio
 from suap_scraper.config import *
 
-def notas_detalhar(html_detalhar):
+def tratar_notas_detalhar(html_detalhar):
   notas = {}
   soup = BeautifulSoup(html_detalhar, 'html.parser')
   trs_soups = soup.tbody.find_all('tr')
   for tr_soup in trs_soups:
     tr_tds = tr_soup.find_all('td')
     nota = tr_tds[4].get_text()
     sigla_av = tr_tds[0].get_text()
     notas[sigla_av] = None if nota == '-' else int(nota)
 
   return notas
 
-def tratar_etapas_tds(materia_etapas_tds, session):
+async def tratar_etapas_tds(materia_etapas_tds, session):
   etapas = {}
+  tasks = []
+  etapas_com_link = []
   etapas_td = zip(LABELS_NOTAS_TABLE, materia_etapas_tds)
   for etapa, td in etapas_td:
     link = td.a
     texto_td = td.get_text().strip()
-    notas = texto_td if link is None else notas_detalhar(
-      session.get(
-        LINK_SUAP + link['href']
-        ).text
-      )
+    notas = texto_td
+    if link is not None:
+      etapas_com_link.append(etapa)
+      tasks.append(asyncio.create_task(session.get(LINK_SUAP + link['href'])))
     etapas[etapa] = notas if notas != '-' else None
+
+  responses = await asyncio.gather(*tasks)
+  for i in range(len(etapas_com_link)):
+    html_detalhar = responses[i].text
+    notas = tratar_notas_detalhar(html_detalhar)
+    etapas[etapas_com_link[i]] = notas
   return etapas
 
 
 def tem_colspan(tag):
   return tag.has_attr('colspan')
 
 
@@ -71,17 +79,26 @@
       indices_colspan
     )
     materia_etapas_tds = [materia_tds[i] for i in indices_notas_materia]
 
     materias[disciplina] = materia_etapas_tds
   return materias
 
-def parsear_boletim(boletim_html, session):
+async def parsear_boletim(boletim_html, session):
   materias = materias_etapas_tds(boletim_html)
+  tasks = []
   boletim = {}
+  disciplinas = materias.keys()
+
   for disciplina, materia_etapas_tds in materias.items():
-    boletim[disciplina] = tratar_etapas_tds(
+    tasks.append(
+      asyncio.create_task(
+        tratar_etapas_tds(
       materia_etapas_tds,
       session
-    )
+      )
+    ))
+  responses = await asyncio.gather(*tasks)
+  for i in range(len(disciplinas)):
+    boletim[list(disciplinas)[i]] = responses[i]
   return boletim
```

### Comparing `suap_scraper-0.0.6/suap_scraper.egg-info/PKG-INFO` & `suap_scraper-0.0.6.1/suap_scraper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap-scraper
-Version: 0.0.6
+Version: 0.0.6.1
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

