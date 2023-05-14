# Comparing `tmp/opengpt4-0.1.3.tar.gz` & `tmp/opengpt4-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opengpt4-0.1.3.tar", max compression
+gzip compressed data, was "opengpt4-0.1.4.tar", max compression
```

## Comparing `opengpt4-0.1.3.tar` & `opengpt4-0.1.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    35149 2023-05-14 21:17:10.604194 opengpt4-0.1.3/LICENSE
--rw-r--r--   0        0        0     4740 2023-05-14 21:17:10.604194 opengpt4-0.1.3/README.md
--rw-r--r--   0        0        0      270 2023-05-14 21:17:10.604194 opengpt4-0.1.3/libraries/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-14 21:17:10.604194 opengpt4-0.1.3/libraries/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2023-05-14 21:17:10.604194 opengpt4-0.1.3/libraries/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2023-05-14 21:17:10.604194 opengpt4-0.1.3/libraries/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2023-05-14 21:17:10.608193 opengpt4-0.1.3/libraries/colorama/win32.py
--rw-r--r--   0        0        0     7168 2023-05-14 21:17:10.608193 opengpt4-0.1.3/libraries/colorama/winterm.py
--rw-r--r--   0        0        0     1691 2023-05-14 21:17:10.608193 opengpt4-0.1.3/libraries/tempmail.py
--rw-r--r--   0        0        0     1097 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/README.md
--rw-r--r--   0        0        0     3355 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/__init__.py
--rw-r--r--   0        0        0      206 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/config.yml
--rw-r--r--   0        0        0      866 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatbase/DOC.md
--rw-r--r--   0        0        0      489 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatbase/README.md
--rw-r--r--   0        0        0     5320 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatbase/model.py
--rw-r--r--   0        0        0      649 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/DOC.md
--rw-r--r--   0        0        0      525 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/README.md
--rw-r--r--   0        0        0     2406 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/model.py
--rw-r--r--   0        0        0      624 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatllama/DOC.md
--rw-r--r--   0        0        0      459 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatllama/README.md
--rw-r--r--   0        0        0     1150 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/chatllama/model.py
--rw-r--r--   0        0        0     6698 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/DOC.md
--rw-r--r--   0        0        0     6460 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/README.md
--rw-r--r--   0        0        0     3788 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/attributes/conversation.py
--rw-r--r--   0        0        0     7505 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/model.py
--rw-r--r--   0        0        0     5818 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/tools/system/email_creation.py
--rw-r--r--   0        0        0      657 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/tools/system/signature.py
--rw-r--r--   0        0        0      446 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/forefront/tools/typing/response.py
--rw-r--r--   0        0        0      842 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/italygpt/DOC.md
--rw-r--r--   0        0        0      321 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/italygpt/README.md
--rw-r--r--   0        0        0     1495 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/italygpt/model.py
--rw-r--r--   0        0        0     1208 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/usesless/DOC.md
--rw-r--r--   0        0        0      769 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/usesless/README.md
--rw-r--r--   0        0        0     1577 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/usesless/model.py
--rw-r--r--   0        0        0      418 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/completion/usesless/tools/typing/response.py
--rw-r--r--   0        0        0     4110 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/image/hotpot/model.py
--rw-r--r--   0        0        0     3012 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/image/hotpot/styles.yml
--rw-r--r--   0        0        0      232 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/image/hotpot/tools/system/id.py
--rw-r--r--   0        0        0      147 2023-05-14 21:17:10.608193 opengpt4-0.1.3/opengpt/models/image/hotpot/tools/typing/response.py
--rw-r--r--   0        0        0      437 2023-05-14 21:17:10.608193 opengpt4-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-14 23:05:32.670989 opengpt4-0.1.4/LICENSE
+-rw-r--r--   0        0        0     4740 2023-05-14 23:05:32.670989 opengpt4-0.1.4/README.md
+-rw-r--r--   0        0        0      270 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/win32.py
+-rw-r--r--   0        0        0     7168 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/colorama/winterm.py
+-rw-r--r--   0        0        0     1691 2023-05-14 23:05:32.670989 opengpt4-0.1.4/libraries/tempmail.py
+-rw-r--r--   0        0        0     1097 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/README.md
+-rw-r--r--   0        0        0     3355 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/__init__.py
+-rw-r--r--   0        0        0      206 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/config.yml
+-rw-r--r--   0        0        0      866 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/DOC.md
+-rw-r--r--   0        0        0      489 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/README.md
+-rw-r--r--   0        0        0     5320 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatbase/model.py
+-rw-r--r--   0        0        0      649 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/DOC.md
+-rw-r--r--   0        0        0      525 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/README.md
+-rw-r--r--   0        0        0     2406 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/model.py
+-rw-r--r--   0        0        0      624 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/DOC.md
+-rw-r--r--   0        0        0      459 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/README.md
+-rw-r--r--   0        0        0     1150 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/chatllama/model.py
+-rw-r--r--   0        0        0     6698 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/DOC.md
+-rw-r--r--   0        0        0     6460 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/README.md
+-rw-r--r--   0        0        0     3788 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/attributes/conversation.py
+-rw-r--r--   0        0        0     7505 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/model.py
+-rw-r--r--   0        0        0     5818 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/email_creation.py
+-rw-r--r--   0        0        0      657 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/signature.py
+-rw-r--r--   0        0        0      446 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/forefront/tools/typing/response.py
+-rw-r--r--   0        0        0      842 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/DOC.md
+-rw-r--r--   0        0        0      321 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/README.md
+-rw-r--r--   0        0        0     1495 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/italygpt/model.py
+-rw-r--r--   0        0        0     1208 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/DOC.md
+-rw-r--r--   0        0        0      769 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/README.md
+-rw-r--r--   0        0        0     1577 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/model.py
+-rw-r--r--   0        0        0      418 2023-05-14 23:05:32.670989 opengpt4-0.1.4/opengpt/models/completion/usesless/tools/typing/response.py
+-rw-r--r--   0        0        0     4110 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/model.py
+-rw-r--r--   0        0        0     3012 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/styles.yml
+-rw-r--r--   0        0        0      232 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/tools/system/id.py
+-rw-r--r--   0        0        0      147 2023-05-14 23:05:32.674989 opengpt4-0.1.4/opengpt/models/image/hotpot/tools/typing/response.py
+-rw-r--r--   0        0        0      414 2023-05-14 23:05:32.674989 opengpt4-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     5459 1970-01-01 00:00:00.000000 opengpt4-0.1.4/PKG-INFO
```

### Comparing `opengpt4-0.1.3/LICENSE` & `opengpt4-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/README.md` & `opengpt4-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/colorama/ansi.py` & `opengpt4-0.1.4/libraries/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/colorama/ansitowin32.py` & `opengpt4-0.1.4/libraries/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/colorama/initialise.py` & `opengpt4-0.1.4/libraries/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/colorama/win32.py` & `opengpt4-0.1.4/libraries/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/colorama/winterm.py` & `opengpt4-0.1.4/libraries/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/libraries/tempmail.py` & `opengpt4-0.1.4/libraries/tempmail.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/README.md` & `opengpt4-0.1.4/opengpt/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/__init__.py` & `opengpt4-0.1.4/opengpt/__init__.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatbase/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/chatbase/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatbase/model.py` & `opengpt4-0.1.4/opengpt/models/completion/chatbase/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/README.md` & `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatgptproxy/model.py` & `opengpt4-0.1.4/opengpt/models/completion/chatgptproxy/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatllama/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/chatllama/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/chatllama/model.py` & `opengpt4-0.1.4/opengpt/models/completion/chatllama/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/forefront/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/README.md` & `opengpt4-0.1.4/opengpt/models/completion/forefront/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/attributes/conversation.py` & `opengpt4-0.1.4/opengpt/models/completion/forefront/attributes/conversation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/model.py` & `opengpt4-0.1.4/opengpt/models/completion/forefront/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/tools/system/email_creation.py` & `opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/email_creation.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/forefront/tools/system/signature.py` & `opengpt4-0.1.4/opengpt/models/completion/forefront/tools/system/signature.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/italygpt/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/italygpt/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/italygpt/model.py` & `opengpt4-0.1.4/opengpt/models/completion/italygpt/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/usesless/DOC.md` & `opengpt4-0.1.4/opengpt/models/completion/usesless/DOC.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/usesless/README.md` & `opengpt4-0.1.4/opengpt/models/completion/usesless/README.md`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/completion/usesless/model.py` & `opengpt4-0.1.4/opengpt/models/completion/usesless/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/image/hotpot/model.py` & `opengpt4-0.1.4/opengpt/models/image/hotpot/model.py`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/opengpt/models/image/hotpot/styles.yml` & `opengpt4-0.1.4/opengpt/models/image/hotpot/styles.yml`

 * *Files identical despite different names*

### Comparing `opengpt4-0.1.3/PKG-INFO` & `opengpt4-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opengpt4
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 License: GPL-3.0
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

