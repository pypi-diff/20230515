# Comparing `tmp/t2c-0.0.4.tar.gz` & `tmp/t2c-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "t2c-0.0.4.tar", last modified: Sun May 14 16:26:39 2023, max compression
+gzip compressed data, was "t2c-0.0.5.tar", last modified: Mon May 15 17:01:24 2023, max compression
```

## Comparing `t2c-0.0.4.tar` & `t2c-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.947018 t2c-0.0.4/
--rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.4/LICENSE
--rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 16:26:39.946854 t2c-0.0.4/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      550 2023-05-14 16:25:57.000000 t2c-0.0.4/README.md
--rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-14 16:26:39.947061 t2c-0.0.4/setup.cfg
--rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-14 16:26:04.000000 t2c-0.0.4/setup.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.945848 t2c-0.0.4/t2c/
--rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-14 16:26:08.000000 t2c-0.0.4/t2c/__init__.py
--rw-r--r--   0 iguangyu   (502) staff       (20)     6755 2023-05-14 16:25:03.000000 t2c-0.0.4/t2c/text2cron.py
-drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-14 16:26:39.946680 t2c-0.0.4/t2c.egg-info/
--rw-r--r--   0 iguangyu   (502) staff       (20)     1088 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/PKG-INFO
--rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/SOURCES.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/dependency_links.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/requires.txt
--rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-14 16:26:39.000000 t2c-0.0.4/t2c.egg-info/top_level.txt
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.248734 t2c-0.0.5/
+-rw-r--r--   0 iguangyu   (502) staff       (20)    11356 2023-05-13 17:09:56.000000 t2c-0.0.5/LICENSE
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1257 2023-05-15 17:01:24.248562 t2c-0.0.5/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      719 2023-05-15 17:00:47.000000 t2c-0.0.5/README.md
+-rw-r--r--   0 iguangyu   (502) staff       (20)       38 2023-05-15 17:01:24.248775 t2c-0.0.5/setup.cfg
+-rw-r--r--   0 iguangyu   (502) staff       (20)      918 2023-05-15 17:00:53.000000 t2c-0.0.5/setup.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.247324 t2c-0.0.5/t2c/
+-rw-r--r--   0 iguangyu   (502) staff       (20)       86 2023-05-15 17:01:12.000000 t2c-0.0.5/t2c/__init__.py
+-rw-r--r--   0 iguangyu   (502) staff       (20)     7505 2023-05-15 16:59:33.000000 t2c-0.0.5/t2c/text2cron.py
+drwxr-xr-x   0 iguangyu   (502) staff       (20)        0 2023-05-15 17:01:24.248343 t2c-0.0.5/t2c.egg-info/
+-rw-r--r--   0 iguangyu   (502) staff       (20)     1257 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/PKG-INFO
+-rw-r--r--   0 iguangyu   (502) staff       (20)      193 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/SOURCES.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        1 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/dependency_links.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)       15 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/requires.txt
+-rw-r--r--   0 iguangyu   (502) staff       (20)        4 2023-05-15 17:01:24.000000 t2c-0.0.5/t2c.egg-info/top_level.txt
```

### Comparing `t2c-0.0.4/LICENSE` & `t2c-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `t2c-0.0.4/setup.py` & `t2c-0.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 # Get the long description from the relevant file
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='t2c',
-    version='0.0.4',
+    version='0.0.5',
     description='A Python Library that converts human readable text to Cron Expression.',
     long_description=long_description,
     url='https://github.com/iguangyu/text2cron',
     author='iguangyu',
     author_email='oofheaven7@gmail.com',
     license='MIT',
     classifiers=[
```

### Comparing `t2c-0.0.4/t2c/text2cron.py` & `t2c-0.0.5/t2c/text2cron.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import re
 import json
 import requests
 import pendulum
 import cn2an
 
 class Text2Cron(object):
-    now = pendulum.now()
-    current_datetime = f"{now.hour}时{now.minute}分"
     re_dict = {
         ' ': '',
         '号': '日',
         "日": "天",
         "星期": "周",
         "礼拜": "周",
         "小时": "时",
@@ -23,53 +21,66 @@
         "天半": ".5天",
         "半时":"30分",
         "半个时":"30分",
         "半个小时":"30分",
         "半":"30分",
         "一刻": "15分",
         "minute": "分",
-        "这时候": current_datetime,
-        "这个时候": current_datetime
     }
     period = r'(每个?|下[^午]|这个?)?'
     day = r'(今.|明[天]?|后[天]?|周[天1234567]?|月\d+天|[天周月年])?'
     aopm = r'(早.|上.|中.|下.|晚.)?'
     hour = r'(\d+)?' + r'[点时：:]?'
     minute = r'([0-5]?[0-9]|半|一刻)?'
     
     full_pattern = period + day + aopm + hour + minute 
     short_term = r'(\d+\.?5?)?个?([分时天周月年])之?后'
     day_pattern = r'周(\d|天)|月(\d+)天|(今.)|(明.)|(大*后.)'
     
     
-    def __init__(self, text: str, usegpt = False) -> None:
-        self.text = text
-        # print(self.full_pattern)
-        if not usegpt:
-            text = text.replace('\n','')
-            for key, value in self.re_dict.items():
-                text = text.replace(key, value)
-            self.text = cn2an.transform(text)
-        
-    def __to_cron(self) -> list:
-        l, isshort = self.__find_util(self.text)
+    def __init__(self, usegpt=False, apikey='', language=None) -> None:
+        self.usegpt = usegpt
+        self.apikey = apikey
+        self.language = language
+
+                
+    def __to_text(self, text: str):
+        self.now = pendulum.now()
+        current_datetime = f"{self.now.hour}时{self.now.minute}分"
+        self.re_dict["这时候"] = current_datetime
+        self.re_dict["这个时候"] = current_datetime
+        text = text.replace('\n','')
+        for key, value in self.re_dict.items():
+            text = text.replace(key, value)
+        text = cn2an.transform(text)
+        return text
+    
+    def __to_cron(self, text: str) -> list:
+        if self.language is not None:
+            import googletrans
+            from googletrans import Translator
+            self.translater = Translator()
+            out = self.translater.translate(text, dest='zh-cn', src=self.language)
+            text = out.text
+        text = self.__to_text(text)
+        l, isshort = self.__find_util(text)
         if isshort:
             digit = float(l[0])
             offset = {
                 '年': self.now.add(years=int(digit)), 
                 '月': self.now.add(months=int(digit)),
                 '周': self.now.add(weeks=digit),
                 '天': self.now.add(days=digit),
                 '时': self.now.add(hours=digit),
                 '分': self.now.add(minutes=digit)
             }
             self.now = offset[l[1]]
             return [
-                0, self.now.minute, self.now.hour, 
-                self.now.day, self.now.month, '?', self.now.year,
+                self.now.minute, self.now.hour, 
+                self.now.day, self.now.month, '?',
             ]
         else:
             period, day, aopm, hour, minute = l
             everyday = False
             # period_matches = re.search(self.period_pattern, period)
             day_matches = re.search(self.day_pattern, day)
             if day_matches is not None:
@@ -105,46 +116,51 @@
             return [
                 self.now.minute, self.now.hour, 
                 self.now.day if not everyday else '*', 
                 self.now.month if not everyday else '*',
                 '?',
             ]
 
-    def show_args(self):
-        l, _ = self.__find_util(self.text)
+    def show_args(self, text: str):
+        text = self.__to_text(text)
+        l, _ = self.__find_util(text)
         return l
 
-    def cron(self) -> str:
-        cron_list = self.__to_cron()
+    def cron(self, text: str) -> str:
+        
+        cron_list = self.__to_cron(text)
         return ' '.join([str(i) for i in cron_list])
     
     
     def __find_util(self, text: str) -> list[tuple, bool]:
         long_term = max(re.findall(pattern=self.full_pattern, string=text),
             key=lambda tup: sum(1 for val in tup if val != ''))
         short_term = re.findall(pattern=self.short_term, string=text)
         short_term = () if len(short_term) == 0 else short_term[0]
         if sum(1 for val in short_term if val != '') == 2:
             return short_term, True
         term = max([long_term, short_term],
             key=lambda tup: sum(1 for val in tup if val != ''))
         return term, term == short_term
 
-    def gpt(self, apikey: str) -> str:        
+    def gpt(self, text: str) -> str:
+        if not self.usegpt or self.apikey == '':
+            raise ValueError('set the `usegpt` = True and set the correct apikey')    
         try:
             import openai
-            openai.api_key = apikey
+            openai.api_key = self.apikey
+            self.now = pendulum.now()
             res = openai.ChatCompletion.create(
             model="gpt-3.5-turbo",
             messages=[{
                     "role": "system",
                     "content": "You are a helpful webapp that provides users with cron expressions"
                 },{
                     "role": "user",
-                    "content": f"Write a cron expression for the following and please just output the answer, say nothing else and don't explain 'current time is {self.now.to_datetime_string} {self.text}'"
+                    "content": f"Write a cron expression for the following and please just output the answer, say nothing else and don't explain 'current time is {self.now.to_datetime_string} {text}'"
                 }]
             )
             return res.choices[0].message.content
         except ImportError as e:
             print('You need to install openai module to use gpt\npip install openai')
         
 
@@ -157,20 +173,22 @@
     parser.add_argument('--gpt', '-g', type=str, default=None, help="使用gpt")
     
     args = parser.parse_args()
     text = args.time
     if args.gpt is not None:
         res = Text2Cron(text, usegpt=True, apikey='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').gpt()
     else: 
-        res = Text2Cron(text).cron()
+        print(text)
+        # res = Text2Cron(language='en').cron(text)
+        res = Text2Cron(language='en').cron('two minutes later')
         print(res)
 
     if args.cron is not None:
         print('= cron表达式如下 =')
         cron_exp = ' '.join([str(c) for c in res])
         res = requests.get('http://cron.ciding.cc/getCornTimes?cronExpression='+cron_exp+'&time=5')
         print('\n'.join(json.loads(res.text)['datas']))
 
     # import pendulum
-    now = pendulum.now()
-    now.add()
+    # now = pendulum.now()
+    # now.add()
```

