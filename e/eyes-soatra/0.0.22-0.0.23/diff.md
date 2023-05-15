# Comparing `tmp/eyes_soatra-0.0.22.tar.gz` & `tmp/eyes_soatra-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eyes_soatra-0.0.22.tar", last modified: Fri May 12 06:04:23 2023, max compression
+gzip compressed data, was "eyes_soatra-0.0.23.tar", last modified: Mon May 15 03:46:02 2023, max compression
```

## Comparing `eyes_soatra-0.0.22.tar` & `eyes_soatra-0.0.23.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.375082 eyes_soatra-0.0.22/
--rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.22/LICENSE
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-12 06:04:23.374947 eyes_soatra-0.0.22/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.22/README.md
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.370113 eyes_soatra-0.0.22/eyes_soatra/
--rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.22/eyes_soatra/__init__.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.371458 eyes_soatra-0.0.22/eyes_soatra/depends/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.22/eyes_soatra/depends/__init__.py
--rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.22/eyes_soatra/depends/depends_404.py
--rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.22/eyes_soatra/depends/depends_no_data.py
--rw-r--r--   0 soatra     (501) staff       (20)    12728 2023-05-12 06:00:40.000000 eyes_soatra-0.0.22/eyes_soatra/eyes.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.371882 eyes_soatra-0.0.22/eyes_soatra/needs/
--rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.22/eyes_soatra/needs/__init__.py
--rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.22/eyes_soatra/needs/user_agents.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.370940 eyes_soatra-0.0.22/eyes_soatra.egg-info/
--rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-12 06:04:23.000000 eyes_soatra-0.0.22/eyes_soatra.egg-info/PKG-INFO
--rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-12 06:04:23.000000 eyes_soatra-0.0.22/eyes_soatra.egg-info/SOURCES.txt
--rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-12 06:04:23.000000 eyes_soatra-0.0.22/eyes_soatra.egg-info/dependency_links.txt
--rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-12 06:04:23.000000 eyes_soatra-0.0.22/eyes_soatra.egg-info/requires.txt
--rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-12 06:04:23.000000 eyes_soatra-0.0.22/eyes_soatra.egg-info/top_level.txt
--rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-12 06:04:23.375132 eyes_soatra-0.0.22/setup.cfg
--rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-12 01:29:54.000000 eyes_soatra-0.0.22/setup.py
-drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-12 06:04:23.374543 eyes_soatra-0.0.22/test/
--rw-r--r--   0 soatra     (501) staff       (20)     2482 2023-05-12 01:25:06.000000 eyes_soatra-0.0.22/test/test.py
--rw-r--r--   0 soatra     (501) staff       (20)     1372 2023-05-12 05:57:10.000000 eyes_soatra-0.0.22/test/test2.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.021640 eyes_soatra-0.0.23/
+-rw-r--r--   0 soatra     (501) staff       (20)       13 2023-05-02 07:13:47.000000 eyes_soatra-0.0.23/LICENSE
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-15 03:46:02.021514 eyes_soatra-0.0.23/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)       49 2023-05-11 09:42:34.000000 eyes_soatra-0.0.23/README.md
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.016770 eyes_soatra-0.0.23/eyes_soatra/
+-rw-r--r--   0 soatra     (501) staff       (20)       28 2023-05-02 07:14:02.000000 eyes_soatra-0.0.23/eyes_soatra/__init__.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.018021 eyes_soatra-0.0.23/eyes_soatra/depends/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-02 07:07:54.000000 eyes_soatra-0.0.23/eyes_soatra/depends/__init__.py
+-rw-r--r--   0 soatra     (501) staff       (20)     7691 2023-05-11 01:49:20.000000 eyes_soatra-0.0.23/eyes_soatra/depends/depends_404.py
+-rw-r--r--   0 soatra     (501) staff       (20)      276 2023-05-02 03:37:05.000000 eyes_soatra-0.0.23/eyes_soatra/depends/depends_no_data.py
+-rw-r--r--   0 soatra     (501) staff       (20)    13126 2023-05-15 03:20:21.000000 eyes_soatra-0.0.23/eyes_soatra/eyes.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.018369 eyes_soatra-0.0.23/eyes_soatra/needs/
+-rw-r--r--   0 soatra     (501) staff       (20)        0 2023-05-11 07:51:47.000000 eyes_soatra-0.0.23/eyes_soatra/needs/__init__.py
+-rw-rw-r--   0 soatra     (501) staff       (20)  1339531 2023-05-11 09:13:03.000000 eyes_soatra-0.0.23/eyes_soatra/needs/user_agents.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.017494 eyes_soatra-0.0.23/eyes_soatra.egg-info/
+-rw-r--r--   0 soatra     (501) staff       (20)      554 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/PKG-INFO
+-rw-r--r--   0 soatra     (501) staff       (20)      440 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/SOURCES.txt
+-rw-r--r--   0 soatra     (501) staff       (20)        1 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/dependency_links.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       43 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/requires.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       12 2023-05-15 03:46:01.000000 eyes_soatra-0.0.23/eyes_soatra.egg-info/top_level.txt
+-rw-r--r--   0 soatra     (501) staff       (20)       38 2023-05-15 03:46:02.021685 eyes_soatra-0.0.23/setup.cfg
+-rw-r--r--   0 soatra     (501) staff       (20)     1131 2023-05-15 03:45:59.000000 eyes_soatra-0.0.23/setup.py
+drwxr-xr-x   0 soatra     (501) staff       (20)        0 2023-05-15 03:46:02.021035 eyes_soatra-0.0.23/test/
+-rw-r--r--   0 soatra     (501) staff       (20)     2889 2023-05-15 02:48:58.000000 eyes_soatra-0.0.23/test/test.py
+-rw-r--r--   0 soatra     (501) staff       (20)      332 2023-05-15 03:21:33.000000 eyes_soatra-0.0.23/test/test2.py
```

### Comparing `eyes_soatra-0.0.22/PKG-INFO` & `eyes_soatra-0.0.23/eyes_soatra.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes_soatra
-Version: 0.0.22
+Name: eyes-soatra
+Version: 0.0.23
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.22/eyes_soatra/depends/depends_404.py` & `eyes_soatra-0.0.23/eyes_soatra/depends/depends_404.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.22/eyes_soatra/eyes.py` & `eyes_soatra-0.0.23/eyes_soatra/eyes.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,34 @@
 __separator = '\||-|:'
 __header_min_length = 3
 __paragraph_min_length = 7
 __container = 'self::div or self::span or self::table'
 __header_xpaths = [
     '//title',
     '//h1[self::*//text() and last()=1]',
-    '(//h2[self::*//text() and last()=1])[1]'
+    '//h2[self::*//text() and last()=1]'
+]
+__header_xpaths_all = [
+    '//title',
+    '//h1',
+    '//h2',
+    '//h3',
+    '//h4',
+    '//h5',
+    '//h6',
+    '//p',
+    '//a',
+    '//button',
+    
+    '//span',
+    '//div',
+    
+    '//li',
+    '//dt',
+    '//dd'
 ]
 __paragraph_xpaths = [
     '//p[@class="no_data"]',
     '//h1[self::*//text()]/following-sibling::p[1]',
     '//h1[self::*//text()]/following-sibling::*//p[1]',
     f'//*[({__container}) and self::*//h1[self::*//text()] and self::*/*[last()=1]]/following-sibling::*[1][{__container}]//p[1]'
 ]
@@ -54,36 +73,39 @@
     return __re.sub(r'\s+', ' ', text).strip()
 
 def __get_highlight(
     html,
     header_xpath,
     paragraph_xpath,
     content_xpath,
+    allow_all_tags,
 ):
     html = __HTML(html=html)
     highlight = __highlighter(
         html,
         header_xpath,
         paragraph_xpath,
-        content_xpath
+        content_xpath,
+        allow_all_tags,
     )
     
     return highlight
 
 def __highlighter(
     html,
     header_xpath,
     paragraph_xpath,
     content_xpath,
+    allow_all_tags,
 ):
     header_texts = []
     paragraph_texts = []
     content_texts = []
     
-    for xpath in __header_xpaths + (header_xpath if type(header_xpath) == list else []):
+    for xpath in (__header_xpaths_all if allow_all_tags else __header_xpaths) + (header_xpath if type(header_xpath) == list else []):
         header_list = html.xpath(f'({xpath})//text()')
         header = ' '.join(header_list)
         header = __strip(header)
         
         if len(header) >= __header_min_length:
             header_texts.append(header)
     
@@ -248,14 +270,15 @@
     sleep_reject=2,
     tries_timeout=3,
     tries_reject=25,
     header_xpath=None,
     paragraph_xpath=None,
     content_xpath=None,
     allow_redirects=True,
+    allow_all_header_tags=True,
     header_min_point=0.8,
     paragraph_min_point=0.85,
     
     show_highlight = False,
     show_header = False,
     show_paragraph = False,
     show_content = False,
@@ -322,14 +345,15 @@
     
             html = response.content
             highlight = __get_highlight(
                 html,
                 header_xpath,
                 paragraph_xpath,
                 content_xpath,
+                allow_all_header_tags
             )
             
             if not (lang == 'ja' or lang == 'en'):
                 translate = __Translator(from_lang=lang, to_lang='en')
                 
                 for key in highlight:
                     for i in range(0, len(highlight[key])):
```

### Comparing `eyes_soatra-0.0.22/eyes_soatra/needs/user_agents.py` & `eyes_soatra-0.0.23/eyes_soatra/needs/user_agents.py`

 * *Files identical despite different names*

### Comparing `eyes_soatra-0.0.22/eyes_soatra.egg-info/PKG-INFO` & `eyes_soatra-0.0.23/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: eyes-soatra
-Version: 0.0.22
+Name: eyes_soatra
+Version: 0.0.23
 Summary: Eyes
 Author: Soatra
 Author-email: johnsoatra@gmail.com
 Keywords: python,crawler,scanner,requests
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eyes_soatra-0.0.22/setup.py` & `eyes_soatra-0.0.23/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 NAME = 'eyes_soatra'
-VERSION = '0.0.22'
+VERSION = '0.0.23'
 DESCRIPTION = 'Eyes'
 
 AUTHOR_NAME = 'Soatra'
 AUTHOR_EMAIL = 'johnsoatra@gmail.com'
 
 # Setting up
 setup(
```

### Comparing `eyes_soatra-0.0.22/test/test.py` & `eyes_soatra-0.0.23/test/test.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,15 +25,31 @@
     print('\n-------------\n')
 
 def worker(start, end):
     for i in range(start, end):
         url = records[i][0]
         
         try:
-            obj = eyes.view_page(url, show_header=True)
+            obj = eyes.view_page(
+                url,
+                show_header=True,
+                header_xpath=[
+                    '//title',
+                    '//h1',
+                    '//h2',
+                    '//h3',
+                    '//h4',
+                    '//h5',
+                    '//h6',
+                    '//p',
+                    '//a',
+                    '//span',
+                    '//div'
+                ]
+            )
             
             if obj['active']:
                 print(f'--- active {i} --- {url}')
                 
             else:
                 print(f'\n--- inactive {i} --- {url}\n')
                 founds.append(obj)
```

