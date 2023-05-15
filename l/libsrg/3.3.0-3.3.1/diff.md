# Comparing `tmp/libsrg-3.3.0-py3-none-any.whl.zip` & `tmp/libsrg-3.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,26 +1,26 @@
-Zip file size: 30820 bytes, number of entries: 24
+Zip file size: 30819 bytes, number of entries: 24
 -rw-r--r--  2.0 unx      196 b- defN 23-Jan-24 15:50 libsrg/Info.py
 -rw-r--r--  2.0 unx     3532 b- defN 23-Jan-31 15:26 libsrg/LevelBanner.py
 -rw-r--r--  2.0 unx     1492 b- defN 23-Jan-18 20:30 libsrg/LoggerGUIProxy.py
 -rw-r--r--  2.0 unx     5511 b- defN 23-Jan-31 15:26 libsrg/LoggingAppBase.py
 -rw-r--r--  2.0 unx     5733 b- defN 23-Jan-31 15:30 libsrg/LoggingCounter.py
 -rw-r--r--  2.0 unx      413 b- defN 23-Jan-31 15:26 libsrg/LoggingUtils.py
 -rw-r--r--  2.0 unx     1376 b- defN 23-Jan-08 15:03 libsrg/LoggingWatcher.py
 -rw-r--r--  2.0 unx     2680 b- defN 23-Jan-31 15:30 libsrg/NagiosBase.py
--rw-r--r--  2.0 unx    14015 b- defN 23-Jan-31 15:35 libsrg/ReZFS.py
+-rw-r--r--  2.0 unx    14015 b- defN 23-May-01 17:29 libsrg/ReZFS.py
 -rw-r--r--  2.0 unx     4193 b- defN 23-Feb-02 14:45 libsrg/Runner.py
 -rw-r--r--  2.0 unx     4015 b- defN 23-Jan-31 15:30 libsrg/Runner2.py
 -rw-r--r--  2.0 unx     6947 b- defN 23-Feb-09 18:22 libsrg/Stage0.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-31 16:52 libsrg/__init__.py
 -rw-r--r--  2.0 unx    17506 b- defN 23-Feb-06 00:12 libsrg/ztool.py
 -rw-r--r--  2.0 unx     2214 b- defN 23-Feb-05 15:02 libsrg/TKGUI/GuiBase.py
 -rw-r--r--  2.0 unx      447 b- defN 22-Mar-14 16:04 libsrg/TKGUI/GuiRequest.py
 -rw-r--r--  2.0 unx     3414 b- defN 23-Feb-05 15:22 libsrg/TKGUI/GuiRequestQueue.py
 -rw-r--r--  2.0 unx    10535 b- defN 23-Jan-19 14:02 libsrg/TKGUI/LoggerGUI.py
 -rw-r--r--  2.0 unx        1 b- defN 23-Jan-31 17:16 libsrg/TKGUI/__init__.py
--rw-rw-rw-  2.0 unx     1069 b- defN 23-Feb-09 18:23 libsrg-3.3.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     3357 b- defN 23-Feb-09 18:23 libsrg-3.3.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-09 18:23 libsrg-3.3.0.dist-info/WHEEL
--rw-rw-rw-  2.0 unx        7 b- defN 23-Feb-09 18:23 libsrg-3.3.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1860 b- defN 23-Feb-09 18:23 libsrg-3.3.0.dist-info/RECORD
-24 files, 90605 bytes uncompressed, 27860 bytes compressed:  69.3%
+-rw-rw-rw-  2.0 unx     1069 b- defN 23-May-01 17:29 libsrg-3.3.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3357 b- defN 23-May-01 17:29 libsrg-3.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-01 17:29 libsrg-3.3.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx        7 b- defN 23-May-01 17:29 libsrg-3.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1860 b- defN 23-May-01 17:29 libsrg-3.3.1.dist-info/RECORD
+24 files, 90605 bytes uncompressed, 27859 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -51,23 +51,23 @@
 
 Filename: libsrg/TKGUI/LoggerGUI.py
 Comment: 
 
 Filename: libsrg/TKGUI/__init__.py
 Comment: 
 
-Filename: libsrg-3.3.0.dist-info/LICENSE.txt
+Filename: libsrg-3.3.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: libsrg-3.3.0.dist-info/METADATA
+Filename: libsrg-3.3.1.dist-info/METADATA
 Comment: 
 
-Filename: libsrg-3.3.0.dist-info/WHEEL
+Filename: libsrg-3.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: libsrg-3.3.0.dist-info/top_level.txt
+Filename: libsrg-3.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: libsrg-3.3.0.dist-info/RECORD
+Filename: libsrg-3.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## libsrg/ReZFS.py

```diff
@@ -77,15 +77,15 @@
         self.parser.add_argument('--patch', help="patch repo file for N-1, then install (even if current repo exists)",
                                  dest='mode', action='store_const', const=Mode.PATCH)
         self.parser.add_argument('--unpatch', help="revert to unpatched repo file, then install", dest='mode',
                                  action='store_const', const=Mode.UNPATCH)
         self.parser.add_argument('--osrelease', help='OS Release file (/etc/os-release)', dest='osrelease',
                                  type=str, default="/etc/os-release")
         self.parser.add_argument('--zfsrel', help='ZFS release url prefix', dest='zfsrel',
-                                 type=str, default="https://zfsonlinux.org/fedora/zfs-release-2-2")
+                                 type=str, default="https://zfsonlinux.org/fedora/zfs-release-2-3")
         self.parser.add_argument('--zfsrel2', help='ZFS release url suffix', dest='zfsrel2',
                                  type=str, default=".noarch.rpm")
         self.parser.add_argument('--remove', help='removed prior install', dest='remove',
                                  action='store_true', default=False)
 
         self.parser.description = "rezfs.py is a tool to update zfs installation across updates of Fedora"
         self.parser.prog = "rezfs.py"
```

## Comparing `libsrg-3.3.0.dist-info/LICENSE.txt` & `libsrg-3.3.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `libsrg-3.3.0.dist-info/METADATA` & `libsrg-3.3.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libsrg
-Version: 3.3.0
+Version: 3.3.1
 Summary: Base class for logging apps, Nagios, utilities
 Home-page: https://gitlab.com/SRG_gitlab/libsrg
 Author: Steven Goncalo
 Author-email: srg_pypi@ice9mail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
```

## Comparing `libsrg-3.3.0.dist-info/RECORD` & `libsrg-3.3.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 libsrg/LevelBanner.py,sha256=k2JC41LkQz9_bPCiGhejqkd7SO7_fiuBmo4Y_ETW9H4,3532
 libsrg/LoggerGUIProxy.py,sha256=qrgLnB0Gtmu5IXP9EzBpIpKWYphcVVQOmIpqWOH9Y6k,1492
 libsrg/LoggingAppBase.py,sha256=JCeaLFPTwQjVS2YnIHOh5ciK54u1lLXt_dwGP7hv-r0,5511
 libsrg/LoggingCounter.py,sha256=fL3E_lErmjSQDy9TPDn-m0_PASoOM7wlf3VQs2R4AEM,5733
 libsrg/LoggingUtils.py,sha256=brhP-2YaCd69vI0CKWTFUZtiTRhj1ud4i-tApP4FWg0,413
 libsrg/LoggingWatcher.py,sha256=tZ803wbw_qvW8tSRDwAbBRQSCrMzhz-FIJsf_hCNIFo,1376
 libsrg/NagiosBase.py,sha256=5FniCUJ8ywFX8oM2q0gKQX2Wvz6J6yt0HT_WYfPniik,2680
-libsrg/ReZFS.py,sha256=9OLy3Mqvo6ZZrdYVC3OBn8996CeohukmSMdqCC2OH0U,14015
+libsrg/ReZFS.py,sha256=8SInGf72nnju_MRpYqNPtf6VHAqesuZr50_wy7iPE_c,14015
 libsrg/Runner.py,sha256=CeZLOhBiIUZ60MgBxktQnaWB5NsLhJE8wNJISd23TtM,4193
 libsrg/Runner2.py,sha256=bZqvmyw9O-2XQconsWQTvtUHy7QYzQrNfoSBKMc3XXA,4015
 libsrg/Stage0.py,sha256=gMPTzSn7ZE0RaO85zmvwZbik4zPUsuwnNITUsD1iXWE,6947
 libsrg/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 libsrg/ztool.py,sha256=PCGHW1WghwegWXyR8rhYocsJ2HyDfjGSd5-gcvjIhJY,17506
 libsrg/TKGUI/GuiBase.py,sha256=MG4D10voRxszQvglABmHG8GHqRNXNo6gWZmY77fpkGU,2214
 libsrg/TKGUI/GuiRequest.py,sha256=ZrUBxrpkAV8ITqbcr7br0-sX9iK69bx1_Fu7COKB5uc,447
 libsrg/TKGUI/GuiRequestQueue.py,sha256=SLoT-PdXgK4JgU-WcESlRwehZIEPBwRgPORn0Tm8Mws,3414
 libsrg/TKGUI/LoggerGUI.py,sha256=2OCiCii4aejdPrgfVRq7FWSdefTiArnmv7mUKyytNSs,10535
 libsrg/TKGUI/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-libsrg-3.3.0.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
-libsrg-3.3.0.dist-info/METADATA,sha256=80cm_RSRCiTMqvVKRcL3lZu33uGhs-rjYr_LApuv8W4,3357
-libsrg-3.3.0.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-libsrg-3.3.0.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
-libsrg-3.3.0.dist-info/RECORD,,
+libsrg-3.3.1.dist-info/LICENSE.txt,sha256=ACwmltkrXIz5VsEQcrqljq-fat6ZXAMepjXGoe40KtE,1069
+libsrg-3.3.1.dist-info/METADATA,sha256=B-RPowk9CZbhhynNZXrmWbW7hTJq03SarzQxBz2XXSA,3357
+libsrg-3.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+libsrg-3.3.1.dist-info/top_level.txt,sha256=NYEOHhvqWFavgb_q4ADmjraMpsan8oFEQPXmMMHGvZ0,7
+libsrg-3.3.1.dist-info/RECORD,,
```

