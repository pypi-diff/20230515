# Comparing `tmp/gravity_auto_exit-1.8.0-py3-none-any.whl.zip` & `tmp/gravity_auto_exit-1.8.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5871 bytes, number of entries: 11
+Zip file size: 5895 bytes, number of entries: 11
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Feb-03 11:23 gravity_auto_exit/__init__.py
 -rw-rw-rw-  2.0 fat      978 b- defN 22-Nov-06 04:54 gravity_auto_exit/logger.py
--rw-rw-rw-  2.0 fat     7486 b- defN 23-May-12 12:17 gravity_auto_exit/main.py
+-rw-rw-rw-  2.0 fat     7568 b- defN 23-May-15 07:10 gravity_auto_exit/main.py
 -rw-rw-rw-  2.0 fat      172 b- defN 23-Apr-27 06:33 gravity_auto_exit/mixins.py
 -rw-rw-rw-  2.0 fat      327 b- defN 22-Nov-06 04:14 gravity_auto_exit/settings.py
 -rw-rw-rw-  2.0 fat        0 b- defN 22-Nov-06 04:12 gravity_auto_exit/logs/__init__.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-12 12:38 gravity_auto_exit-1.8.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      407 b- defN 23-May-12 12:38 gravity_auto_exit-1.8.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 12:38 gravity_auto_exit-1.8.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-12 12:38 gravity_auto_exit-1.8.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      939 b- defN 23-May-12 12:38 gravity_auto_exit-1.8.0.dist-info/RECORD
-11 files, 11510 bytes uncompressed, 4253 bytes compressed:  63.0%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-15 08:12 gravity_auto_exit-1.8.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      408 b- defN 23-May-15 08:12 gravity_auto_exit-1.8.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 08:12 gravity_auto_exit-1.8.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-15 08:12 gravity_auto_exit-1.8.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      939 b- defN 23-May-15 08:12 gravity_auto_exit-1.8.1.dist-info/RECORD
+11 files, 11593 bytes uncompressed, 4277 bytes compressed:  63.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: gravity_auto_exit/settings.py
 Comment: 
 
 Filename: gravity_auto_exit/logs/__init__.py
 Comment: 
 
-Filename: gravity_auto_exit-1.8.0.dist-info/LICENSE
+Filename: gravity_auto_exit-1.8.1.dist-info/LICENSE
 Comment: 
 
-Filename: gravity_auto_exit-1.8.0.dist-info/METADATA
+Filename: gravity_auto_exit-1.8.1.dist-info/METADATA
 Comment: 
 
-Filename: gravity_auto_exit-1.8.0.dist-info/WHEEL
+Filename: gravity_auto_exit-1.8.1.dist-info/WHEEL
 Comment: 
 
-Filename: gravity_auto_exit-1.8.0.dist-info/top_level.txt
+Filename: gravity_auto_exit-1.8.1.dist-info/top_level.txt
 Comment: 
 
-Filename: gravity_auto_exit-1.8.0.dist-info/RECORD
+Filename: gravity_auto_exit-1.8.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gravity_auto_exit/main.py

```diff
@@ -73,22 +73,22 @@
     def cad_callback_func(self, data=None):
         logger.debug("=====CAD func started=====")
         if self.simple_callback_func:
             threading.Thread(target=self.simple_callback_func).start()
         if not self.active:
             logger.debug("---It is not active---")
             return
-        if not self.engine.status_ready:
+        if self.engine and not self.engine.status_ready:
             logger.debug("Engine is not ready!")
             return
         logger.debug(f'Sleeping before: {self.sleep_before}')
         time.sleep(self.sleep_before)
         logger.debug("Recognise cycle has been started")
         for i in range(5):
-            if not self.engine.status_ready:
+            if self.engine and not self.engine.status_ready:
                 logger.info("Cancel cycle for engine is not ready")
                 return
             logger.debug(f"Recognise cycle {i} of 5")
             time.sleep(i + 0.2)
             if not self.active:
                 self.active = True
             #    return
@@ -187,22 +187,24 @@
 
 if __name__ == '__main__':
     def engine_callback(*args, **kwargs):
         print('MAIN')
 
 
     inst = CADRecogniseMail(  #
-        'http://192.168.60.107',
-        # 'http://172.16.6.176',
+        #'http://192.168.60.107',
+         #'http://172.16.6.176',
+        "http://127.0.0.1",
         'admin',
         'Assa+123',
         debug=True,
         #        cam_port=80,
         # 1920*1080
-        cam_port=80,
+        cam_port=82,
         neurocore_login='admin',
         neurocore_password='admin',
         engine_callback=engine_callback
     )
     inst.set_token(os.environ.get("mail_token"))
-    res = inst.try_recognise_plate()
-    print(res['number'])
+    inst.start()
+    #res = inst.try_recognise_plate()
+    #print(res['number'])
```

## Comparing `gravity_auto_exit-1.8.0.dist-info/LICENSE` & `gravity_auto_exit-1.8.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `gravity_auto_exit-1.8.0.dist-info/RECORD` & `gravity_auto_exit-1.8.1.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 gravity_auto_exit/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 gravity_auto_exit/logger.py,sha256=fqAx0eDI7R3dEGnnkoIqaTbg2qrcVuRUGAeDFnMQktA,978
-gravity_auto_exit/main.py,sha256=1iKkej-k4IRl9PlucvGrg5iWv7HBR7Ief8HoHgm5Is8,7486
+gravity_auto_exit/main.py,sha256=NSsQzITZTRwbvArb0ZXotchTXVVZo1jqBZpfohwZrKk,7568
 gravity_auto_exit/mixins.py,sha256=zzTClSits8whf-zHfeQwZANFAAymMSsL3oK539L_yz0,172
 gravity_auto_exit/settings.py,sha256=W4ZrNBbyEsoDMvEAvRK5AH6Q2DLrK2tCzVX3i069rpE,327
 gravity_auto_exit/logs/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gravity_auto_exit-1.8.0.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-gravity_auto_exit-1.8.0.dist-info/METADATA,sha256=aQrNTi6HAcuiqeBJI_R8U3obMlmQn3uvoCvNDwqM6Yc,407
-gravity_auto_exit-1.8.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gravity_auto_exit-1.8.0.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
-gravity_auto_exit-1.8.0.dist-info/RECORD,,
+gravity_auto_exit-1.8.1.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+gravity_auto_exit-1.8.1.dist-info/METADATA,sha256=-2uwK-33FPuenzZalUNEZuSyhelUbi40JF2cgyNwEY4,408
+gravity_auto_exit-1.8.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gravity_auto_exit-1.8.1.dist-info/top_level.txt,sha256=O896kTA32MK0-JQ_QK-QUsag8oA7wVEeEJGjgZiBpt4,18
+gravity_auto_exit-1.8.1.dist-info/RECORD,,
```

