# Comparing `tmp/gravity_auto_exit-1.71.2-py3-none-any.whl.zip` & `tmp/gravity_auto_exit-1.71.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 5679 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-03 11:23 gravity_auto_exit/__init__.py
 -rw-rw-rw-  2.0 fat      978 b- defN 22-Nov-06 04:54 gravity_auto_exit/logger.py
--rw-rw-rw-  2.0 fat     7449 b- defN 23-Mar-22 11:38 gravity_auto_exit/main.py
+-rw-rw-rw-  2.0 fat     7470 b- defN 23-Mar-24 05:40 gravity_auto_exit/main.py
 -rw-rw-rw-  2.0 fat      327 b- defN 22-Nov-06 04:14 gravity_auto_exit/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-06 04:12 gravity_auto_exit/logs/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Mar-22 11:39 gravity_auto_exit-1.71.2.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      364 b- defN 23-Mar-22 11:39 gravity_auto_exit-1.71.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-22 11:39 gravity_auto_exit-1.71.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-Mar-22 11:39 gravity_auto_exit-1.71.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      861 b- defN 23-Mar-22 11:39 gravity_auto_exit-1.71.2.dist-info/RECORD
-10 files, 11180 bytes uncompressed, 4181 bytes compressed:  62.6%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Mar-24 05:43 gravity_auto_exit-1.71.3.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      364 b- defN 23-Mar-24 05:43 gravity_auto_exit-1.71.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Mar-24 05:43 gravity_auto_exit-1.71.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-Mar-24 05:43 gravity_auto_exit-1.71.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      861 b- defN 23-Mar-24 05:43 gravity_auto_exit-1.71.3.dist-info/RECORD
+10 files, 11201 bytes uncompressed, 4181 bytes compressed:  62.7%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: gravity_auto_exit/settings.py
 Comment: 
 
 Filename: gravity_auto_exit/logs/__init__.py
 Comment: 
 
-Filename: gravity_auto_exit-1.71.2.dist-info/LICENSE
+Filename: gravity_auto_exit-1.71.3.dist-info/LICENSE
 Comment: 
 
-Filename: gravity_auto_exit-1.71.2.dist-info/METADATA
+Filename: gravity_auto_exit-1.71.3.dist-info/METADATA
 Comment: 
 
-Filename: gravity_auto_exit-1.71.2.dist-info/WHEEL
+Filename: gravity_auto_exit-1.71.3.dist-info/WHEEL
 Comment: 
 
-Filename: gravity_auto_exit-1.71.2.dist-info/top_level.txt
+Filename: gravity_auto_exit-1.71.3.dist-info/top_level.txt
 Comment: 
 
-Filename: gravity_auto_exit-1.71.2.dist-info/RECORD
+Filename: gravity_auto_exit-1.71.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gravity_auto_exit/main.py

```diff
@@ -77,14 +77,15 @@
 
     def cad_callback_func(self, data=None):
         logger.debug("=====CAD func started=====")
         if self.simple_callback_func:
             threading.Thread(target=self.simple_callback_func).start()
         if not self.active:
             logger.debug("---It is not active---")
+            return
         if not self.engine.status_ready:
             logger.debug("Engine is not ready!")
             #if self.can_wait_others and not self.wait_started:
             #    self.wait_started = True
             #    logger.debug("But it is a another car in order")
             #    while not self.active:
             #        time.sleep(0.5)
@@ -94,44 +95,44 @@
         #self.active = False
         logger.debug(f'Sleeping before: {self.sleep_before}')
         time.sleep(self.sleep_before)
         #if datetime.datetime.now() - self.last_take > datetime.timedelta(
         #        seconds=self.reload_time):
         logger.debug("Recognise cycle has been started")
         #self.cycle_started = True
-        self.active = False
+        #self.active = False
         for i in range(5):
             if not self.engine.status_ready:
                 logger.info("Cancel cycle for engine is not ready")
                 return
             logger.debug(f"Recognise cycle {i} of 5")
             time.sleep(i + 0.2)
-            #if not self.active:
-                #self.active = True
+            if not self.active:
+                self.active = True
             #    return
             response = self.camera_and_recognise()
             if 'error' in response:
                 logger.error(f"{response['error']}: {response['info']}")
             else:
                 result, photo = response
                 if result:
                     self.last_take = datetime.datetime.now()
                     logger.debug(f"Success recognise. Number {result}")
                     self.can_wait_others = False
                     self.wait_started = False
-                    self.active = True
+                    #self.active = True
                     #self.cycle_started = False
                     return result
                 else:
                     logger.error(
                         f"Unknown Error! Number {result}")
             if self.failed_callback and i == 2:
                 logger.debug(f'Failed callbaсk working photo...')
                 self.failed_callback()
-        self.active = True
+        #self.active = True
         self.wait_started = False
         self.cycle_started = False
         self.can_wait_others = False
 
     def camera_and_recognise(self):
         result = self.try_recognise_plate()
         if 'error' in result:
```

## Comparing `gravity_auto_exit-1.71.2.dist-info/LICENSE` & `gravity_auto_exit-1.71.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gravity_auto_exit-1.71.2.dist-info/RECORD` & `gravity_auto_exit-1.71.3.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 gravity_auto_exit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gravity_auto_exit/logger.py,sha256=fqAx0eDI7R3dEGnnkoIqaTbg2qrcVuRUGAeDFnMQktA,978
-gravity_auto_exit/main.py,sha256=XgymTypbpkyTo3l4Av3y4sfBGYQrhoIDhXIxSA_rjK8,7449
+gravity_auto_exit/main.py,sha256=0VAWUs__L--pUCbBcNQH7WfJrC_xjz7zTzTlHASgbUM,7470
 gravity_auto_exit/settings.py,sha256=W4ZrNBbyEsoDMvEAvRK5AH6Q2DLrK2tCzVX3i069rpE,327
 gravity_auto_exit/logs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gravity_auto_exit-1.71.2.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gravity_auto_exit-1.71.2.dist-info/METADATA,sha256=SjNhyHyWN99FLWqaxs77JkKT_zcC3sZPXNgej2iU8Dk,364
-gravity_auto_exit-1.71.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gravity_auto_exit-1.71.2.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
-gravity_auto_exit-1.71.2.dist-info/RECORD,,
+gravity_auto_exit-1.71.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gravity_auto_exit-1.71.3.dist-info/METADATA,sha256=QQ0De5Llp_sagSUpJ9Xfxx6xGGKb2UlqjV71NWsjTck,364
+gravity_auto_exit-1.71.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gravity_auto_exit-1.71.3.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
+gravity_auto_exit-1.71.3.dist-info/RECORD,,
```

