# Comparing `tmp/icalstatus-0.0.6-py3-none-any.whl.zip` & `tmp/icalstatus-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 6439 bytes, number of entries: 9
+Zip file size: 6438 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 icalstatus/__init__.py
 -rw-r--r--  2.0 unx     1234 b- defN 80-Jan-01 00:00 icalstatus/date.py
 -rwxr-xr-x  2.0 unx     1036 b- defN 80-Jan-01 00:00 icalstatus/parse.py
 -rw-r--r--  2.0 unx     4691 b- defN 80-Jan-01 00:00 icalstatus/status.py
--rw-r--r--  2.0 unx      770 b- defN 80-Jan-01 00:00 icalstatus-0.0.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     3318 b- defN 80-Jan-01 00:00 icalstatus-0.0.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 icalstatus-0.0.6.dist-info/WHEEL
--rw-r--r--  2.0 unx      123 b- defN 80-Jan-01 00:00 icalstatus-0.0.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      708 b- defN 16-Jan-01 00:00 icalstatus-0.0.6.dist-info/RECORD
-9 files, 11968 bytes uncompressed, 5221 bytes compressed:  56.4%
+-rw-r--r--  2.0 unx      770 b- defN 80-Jan-01 00:00 icalstatus-0.0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3318 b- defN 80-Jan-01 00:00 icalstatus-0.0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 icalstatus-0.0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx      123 b- defN 80-Jan-01 00:00 icalstatus-0.0.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      708 b- defN 16-Jan-01 00:00 icalstatus-0.0.7.dist-info/RECORD
+9 files, 11968 bytes uncompressed, 5220 bytes compressed:  56.4%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: icalstatus/parse.py
 Comment: 
 
 Filename: icalstatus/status.py
 Comment: 
 
-Filename: icalstatus-0.0.6.dist-info/LICENSE
+Filename: icalstatus-0.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: icalstatus-0.0.6.dist-info/METADATA
+Filename: icalstatus-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: icalstatus-0.0.6.dist-info/WHEEL
+Filename: icalstatus-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: icalstatus-0.0.6.dist-info/entry_points.txt
+Filename: icalstatus-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: icalstatus-0.0.6.dist-info/RECORD
+Filename: icalstatus-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## icalstatus/status.py

```diff
@@ -142,15 +142,15 @@
         begin_str = humanize(begin.timestamp() - now.timestamp())
     else:
         begin_str = f"@{begin.strftime('%H:%M')}"
 
     return Event(
         name=next.get("SUMMARY", "Unknown").strip(),
         begin=begin_str,
-        alert=now - timedelta(seconds=config.alert_sec_before) > begin,
+        alert=now + timedelta(seconds=config.alert_sec_before) > begin,
     )
 
 
 def status() -> None:
     """main"""
 
     event = upcoming_event()
```

## Comparing `icalstatus-0.0.6.dist-info/LICENSE` & `icalstatus-0.0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `icalstatus-0.0.6.dist-info/METADATA` & `icalstatus-0.0.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icalstatus
-Version: 0.0.6
+Version: 0.0.7
 Summary: icalstatus
 Home-page: https://github.com/frbor/icalstatus
 License: ISC
 Author: Fredrik Borg
 Author-email: fredrikb.borg@gmail.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

## Comparing `icalstatus-0.0.6.dist-info/RECORD` & `icalstatus-0.0.7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 icalstatus/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 icalstatus/date.py,sha256=Uu7VJn_f9H9Q0RIqcexdTMrgCb27Fr8J9jNHhfCBdiQ,1234
 icalstatus/parse.py,sha256=jXnFHzFDAYnjTCD0Rfj9yilcQ6Vozd9h4VDq3jpEerA,1036
-icalstatus/status.py,sha256=0QQ6sM_B3tWLrVT2GkPeoLmmVGMC0pKCH1R_clF2LWc,4691
-icalstatus-0.0.6.dist-info/LICENSE,sha256=4DFZPzsHvBwvMFiW1m_3QilusGT6jMBlP6zHFNhQ7A8,770
-icalstatus-0.0.6.dist-info/METADATA,sha256=1-7EBB5lM3NOoIzSWgMxp-zW4m3XXS8zNBev0F6qdzM,3318
-icalstatus-0.0.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-icalstatus-0.0.6.dist-info/entry_points.txt,sha256=V4B_F6lqqyg1AL-OIRmQ9hj3lJO5mkI_6xUCvrtjTJY,123
-icalstatus-0.0.6.dist-info/RECORD,,
+icalstatus/status.py,sha256=9OLGEgC0ZOwOZSEhq4UPAiWqJxQw5etdh-0wqtewu3Q,4691
+icalstatus-0.0.7.dist-info/LICENSE,sha256=4DFZPzsHvBwvMFiW1m_3QilusGT6jMBlP6zHFNhQ7A8,770
+icalstatus-0.0.7.dist-info/METADATA,sha256=5tjrysCDMZIEs-4nwKwtJ1eDXFmpa_auTj-zU3X93OI,3318
+icalstatus-0.0.7.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+icalstatus-0.0.7.dist-info/entry_points.txt,sha256=V4B_F6lqqyg1AL-OIRmQ9hj3lJO5mkI_6xUCvrtjTJY,123
+icalstatus-0.0.7.dist-info/RECORD,,
```

