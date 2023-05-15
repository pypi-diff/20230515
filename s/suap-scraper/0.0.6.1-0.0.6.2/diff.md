# Comparing `tmp/suap_scraper-0.0.6.1.tar.gz` & `tmp/suap_scraper-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suap_scraper-0.0.6.1.tar", last modified: Mon May 15 01:15:19 2023, max compression
+gzip compressed data, was "suap_scraper-0.0.6.2.tar", last modified: Mon May 15 16:47:49 2023, max compression
```

## Comparing `suap_scraper-0.0.6.1.tar` & `suap_scraper-0.0.6.2.tar`

### file list

```diff
@@ -1,24 +1,21 @@
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/
--rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.1/LICENSE.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.1/README.md
--rw-rw-r--   0 dom       (1000) dom       (1000)      642 2023-05-15 01:14:39.000000 suap_scraper-0.0.6.1/pyproject.toml
--rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-15 01:15:19.100239 suap_scraper-0.0.6.1/setup.cfg
--rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6.1/setup.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.088239 suap_scraper-0.0.6.1/suap_scraper/
--rw-rw-r--   0 dom       (1000) dom       (1000)     4067 2023-05-15 01:05:45.000000 suap_scraper-0.0.6.1/suap_scraper/SUAP.py
--rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6.1/suap_scraper/__init__.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-05-06 18:49:43.000000 suap_scraper-0.0.6.1/suap_scraper/config.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1043 2023-05-07 11:07:39.000000 suap_scraper-0.0.6.1/suap_scraper/envio.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1025 2023-05-15 00:55:36.000000 suap_scraper-0.0.6.1/suap_scraper/mensagem.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1755 2023-05-15 00:46:26.000000 suap_scraper-0.0.6.1/suap_scraper/novas_notas.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     1085 2023-05-14 23:34:55.000000 suap_scraper-0.0.6.1/suap_scraper/sla.py
--rw-rw-r--   0 dom       (1000) dom       (1000)      293 2023-05-14 23:22:25.000000 suap_scraper-0.0.6.1/suap_scraper/teste.py
--rw-rw-r--   0 dom       (1000) dom       (1000)      966 2023-05-07 20:07:58.000000 suap_scraper-0.0.6.1/suap_scraper/teste_async.py
--rw-rw-r--   0 dom       (1000) dom       (1000)     2807 2023-05-15 01:05:45.000000 suap_scraper-0.0.6.1/suap_scraper/utils.py
-drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 01:15:19.096239 suap_scraper-0.0.6.1/suap_scraper.egg-info/
--rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/PKG-INFO
--rw-rw-r--   0 dom       (1000) dom       (1000)      459 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/SOURCES.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/dependency_links.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       21 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/requires.txt
--rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-15 01:15:18.000000 suap_scraper-0.0.6.1/suap_scraper.egg-info/top_level.txt
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1080 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.2/LICENSE.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)       15 2023-04-30 15:51:56.000000 suap_scraper-0.0.6.2/README.md
+-rw-rw-r--   0 dom       (1000) dom       (1000)      638 2023-05-15 16:47:05.000000 suap_scraper-0.0.6.2/pyproject.toml
+-rw-rw-r--   0 dom       (1000) dom       (1000)       38 2023-05-15 16:47:49.370771 suap_scraper-0.0.6.2/setup.cfg
+-rw-rw-r--   0 dom       (1000) dom       (1000)       69 2023-04-30 22:38:11.000000 suap_scraper-0.0.6.2/setup.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.346771 suap_scraper-0.0.6.2/suap_scraper/
+-rw-rw-r--   0 dom       (1000) dom       (1000)     4081 2023-05-15 16:39:57.000000 suap_scraper-0.0.6.2/suap_scraper/SUAP.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)       36 2023-05-01 00:09:59.000000 suap_scraper-0.0.6.2/suap_scraper/__init__.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1713 2023-05-06 18:49:43.000000 suap_scraper-0.0.6.2/suap_scraper/config.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1043 2023-05-07 11:07:39.000000 suap_scraper-0.0.6.2/suap_scraper/envio.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     1085 2023-05-14 23:34:55.000000 suap_scraper-0.0.6.2/suap_scraper/sla.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)      385 2023-05-15 14:06:00.000000 suap_scraper-0.0.6.2/suap_scraper/teste.py
+-rw-rw-r--   0 dom       (1000) dom       (1000)     2730 2023-05-15 16:39:57.000000 suap_scraper-0.0.6.2/suap_scraper/utils.py
+drwxrwxr-x   0 dom       (1000) dom       (1000)        0 2023-05-15 16:47:49.366771 suap_scraper-0.0.6.2/suap_scraper.egg-info/
+-rw-rw-r--   0 dom       (1000) dom       (1000)      532 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/PKG-INFO
+-rw-rw-r--   0 dom       (1000) dom       (1000)      378 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/SOURCES.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)        1 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/dependency_links.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       17 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/requires.txt
+-rw-rw-r--   0 dom       (1000) dom       (1000)       13 2023-05-15 16:47:49.000000 suap_scraper-0.0.6.2/suap_scraper.egg-info/top_level.txt
```

### Comparing `suap_scraper-0.0.6.1/LICENSE.md` & `suap_scraper-0.0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.1/PKG-INFO` & `suap_scraper-0.0.6.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap_scraper
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `suap_scraper-0.0.6.1/pyproject.toml` & `suap_scraper-0.0.6.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "suap_scraper"
-version = "0.0.6.1"
+version = "0.0.6.2"
 authors = [
   { name="Jao42", email="cavalcante.joao@protonmail.ch" },
 ]
 description = "Um scraper para o SUAP do IFPB"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
     "httpx",
-    "beautifulsoup4",
+    "selectolax",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `suap_scraper-0.0.6.1/suap_scraper/SUAP.py` & `suap_scraper-0.0.6.2/suap_scraper/SUAP.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import httpx
 import asyncio
 import sys
-from bs4 import BeautifulSoup
 from suap_scraper.utils import parsear_boletim
 import json
 import time
 import os
 from suap_scraper.config import *
 
 
@@ -16,38 +15,38 @@
 
 
 class SUAP:
   def __init__(self, user_agent=UA_PADRAO):
     self.user_agent = user_agent
     self.session = httpx.AsyncClient()
     self.session.headers.update(user_agent)
+    self.session_id = None
+    self.matricula = None
+    self.csrf = None
+    self.senha = None
 
   async def loginCredenciais(self, matricula, senha, user_agent=UA_PADRAO):
     self.matricula = matricula
     self.senha = senha
     self.session_id, self.csrf = await self.__loginSUAP()
 
   async def loginSessionId(self, session_id, user_agent=UA_PADRAO):
     self.session_id = session_id
     self.session.cookies['sessionid'] = self.session_id
-    logged = await self.__getInitialPage()
-    self.matricula = logged.headers.get('user')
-    self.csrf = ''
-    self.senha = ''
 
   async def __getInitialPage(self):
     res = await self.session.get(LINK_SUAP)
     return res
 
   def __getCookiesInitialPage(self, initial_page):
-    soup = BeautifulSoup(initial_page.text, 'html.parser')
-    middleware_csrf = soup.find(
-      'input',
-      attrs = {'name': 'csrfmiddlewaretoken'}
-      )['value']
+    tree = HTMLParser(initial_page.text)
+    middleware_csrf = (
+      tree.css('input[name="csrfmiddlewaretoken"]')
+      .attributes['value']
+    )
 
     csrf = initial_page.cookies['csrftoken']
     session_id = initial_page.cookies['sessionid']
 
     return [ middleware_csrf, csrf, session_id ]
 
 
@@ -78,31 +77,34 @@
                         )
 
     res = await self.session.send(req)
 
     try:
       session_id = res.cookies['sessionid']
     except KeyError:
-      soup = BeautifulSoup(res.text, 'html.parser')
-      erro = soup.find(class_="errornote")
-      if erro == None:
+      tree = HTMLParser(res.text)
+      erro = tree.css(".errornote")
+      if not erro:
         raise LoginError("Não foi possivel logar no SUAP")
       msg_erro = erro.get_text().strip()
       try:
         raise LoginError(MSGS_ERRO[msg_erro])
       except KeyError:
         raise LoginError(msg_erro)
     try:
       csrf = res.cookies['csrftoken']
     except:
       pass
 
     return [ session_id, csrf ]
 
   async def __getBoletimPage(self):
+    if self.matricula is None:
+      logged = await self.__getInitialPage()
+      self.matricula = logged.headers.get('user')
     req_json = REQ_JSON_BOLETIM
     req_json["referrer"] = (LINK_SUAP + "/edu/aluno/"
     + str(self.matricula)
     + "/?tab=boletim"
     )
 
     req = self.session.build_request("GET",
@@ -133,7 +135,8 @@
 
     return boletim_json
 
   async def getBoletim(self):
     html_boletim = await self.__getBoletimPage()
     boletim = await self.__createBoletimJSON(html_boletim)
     return boletim
+
```

### Comparing `suap_scraper-0.0.6.1/suap_scraper/config.py` & `suap_scraper-0.0.6.2/suap_scraper/config.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.1/suap_scraper/envio.py` & `suap_scraper-0.0.6.2/suap_scraper/envio.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.1/suap_scraper/sla.py` & `suap_scraper-0.0.6.2/suap_scraper/sla.py`

 * *Files identical despite different names*

### Comparing `suap_scraper-0.0.6.1/suap_scraper/utils.py` & `suap_scraper-0.0.6.2/suap_scraper/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-from bs4 import BeautifulSoup
+from selectolax.parser import HTMLParser
 import sys
 import json
 import asyncio
 from suap_scraper.config import *
 
 def tratar_notas_detalhar(html_detalhar):
   notas = {}
-  soup = BeautifulSoup(html_detalhar, 'html.parser')
-  trs_soups = soup.tbody.find_all('tr')
-  for tr_soup in trs_soups:
-    tr_tds = tr_soup.find_all('td')
-    nota = tr_tds[4].get_text()
-    sigla_av = tr_tds[0].get_text()
+  tree = HTMLParser(html_detalhar)
+  trs_nodes = tree.css('tbody > tr')
+  for tr_node in trs_nodes:
+    tr_tds = tr_node.css('td')
+    nota = tr_tds[4].text()
+    sigla_av = tr_tds[0].text()
     notas[sigla_av] = None if nota == '-' else int(nota)
 
   return notas
 
 async def tratar_etapas_tds(materia_etapas_tds, session):
   etapas = {}
   tasks = []
   etapas_com_link = []
   etapas_td = zip(LABELS_NOTAS_TABLE, materia_etapas_tds)
   for etapa, td in etapas_td:
-    link = td.a
-    texto_td = td.get_text().strip()
+    link = td.css_first('a')
+    texto_td = td.text().strip()
     notas = texto_td
     if link is not None:
       etapas_com_link.append(etapa)
-      tasks.append(asyncio.create_task(session.get(LINK_SUAP + link['href'])))
+      tasks.append(asyncio.create_task(session.get(LINK_SUAP + link.attributes['href'])))
     etapas[etapa] = notas if notas != '-' else None
 
   responses = await asyncio.gather(*tasks)
   for i in range(len(etapas_com_link)):
     html_detalhar = responses[i].text
     notas = tratar_notas_detalhar(html_detalhar)
     etapas[etapas_com_link[i]] = notas
   return etapas
 
 
 def tem_colspan(tag):
-  return tag.has_attr('colspan')
-
+  return ('colspan' in list(tag.attributes.keys()))
 
 def criar_indices_colspan(indices_notas, indices_colspans):
   indices_notas_materia = indices_notas[::]
   for i in indices_colspans:
     for j in range(len(indices_notas)):
       if indices_notas_materia[j] > i:
         indices_notas_materia[j] -= 1
   return indices_notas_materia
 
 
 def materias_etapas_tds(boletim_html):
 
-  soup = BeautifulSoup(boletim_html, 'html.parser')
-  corpo_tabela_soup = soup.tbody
-  materias_html = corpo_tabela_soup.find_all('tr')
-
+  tree = HTMLParser(boletim_html)
+  materias_tr = tree.css('.borda > tbody > tr')
   materias = {}
 
-  for i in range(len(materias_html)):
+  for i in range(len(materias_tr)):
 
-    soup = BeautifulSoup(str(materias_html[i]), 'html.parser')
-    materia_tds = soup.find_all('td')
+    materia_tr = materias_tr[i]
+    materia_tds = materia_tr.css('td')
 
-    disciplina_soup = materia_tds[1]
-    disciplina = (disciplina_soup
-    .get_text()
+    disciplina_node = materia_tds[1]
+    disciplina = (disciplina_node
+    .text()
     .replace('\n', '')
     .strip()
     .replace('  ', ''))
 
     indices_colspan = [
       i for i in range(len(materia_tds)) if tem_colspan(materia_tds[i])
     ]
@@ -97,8 +94,7 @@
       session
       )
     ))
   responses = await asyncio.gather(*tasks)
   for i in range(len(disciplinas)):
     boletim[list(disciplinas)[i]] = responses[i]
   return boletim
-
```

### Comparing `suap_scraper-0.0.6.1/suap_scraper.egg-info/PKG-INFO` & `suap_scraper-0.0.6.2/suap_scraper.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suap-scraper
-Version: 0.0.6.1
+Version: 0.0.6.2
 Summary: Um scraper para o SUAP do IFPB
 Author-email: Jao42 <cavalcante.joao@protonmail.ch>
 Project-URL: Homepage, https://github.com/Jao42/suap-scraper
 Project-URL: Bug Tracker, https://github.com/Jao42/suap-scraper/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

