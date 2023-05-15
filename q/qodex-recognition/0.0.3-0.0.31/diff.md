# Comparing `tmp/qodex_recognition-0.0.3-py3-none-any.whl.zip` & `tmp/qodex_recognition-0.0.31-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3709 bytes, number of entries: 9
+Zip file size: 3724 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 06:47 qodex_recognition/__init__.py
--rw-rw-rw-  2.0 fat     2119 b- defN 23-May-12 12:20 qodex_recognition/main.py
+-rw-rw-rw-  2.0 fat     2181 b- defN 23-May-12 12:29 qodex_recognition/main.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-12 09:02 qodex_recognition/tests/__init__.py
 -rw-rw-rw-  2.0 fat      432 b- defN 23-May-12 09:07 qodex_recognition/tests/main_tests.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-12 12:21 qodex_recognition-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      266 b- defN 23-May-12 12:21 qodex_recognition-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-12 12:21 qodex_recognition-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       18 b- defN 23-May-12 12:21 qodex_recognition-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      782 b- defN 23-May-12 12:21 qodex_recognition-0.0.3.dist-info/RECORD
-9 files, 4800 bytes uncompressed, 2333 bytes compressed:  51.4%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-15 08:11 qodex_recognition-0.0.31.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      267 b- defN 23-May-15 08:11 qodex_recognition-0.0.31.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-15 08:11 qodex_recognition-0.0.31.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       18 b- defN 23-May-15 08:11 qodex_recognition-0.0.31.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      787 b- defN 23-May-15 08:11 qodex_recognition-0.0.31.dist-info/RECORD
+9 files, 4868 bytes uncompressed, 2338 bytes compressed:  52.0%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: qodex_recognition/tests/__init__.py
 Comment: 
 
 Filename: qodex_recognition/tests/main_tests.py
 Comment: 
 
-Filename: qodex_recognition-0.0.3.dist-info/LICENSE
+Filename: qodex_recognition-0.0.31.dist-info/LICENSE
 Comment: 
 
-Filename: qodex_recognition-0.0.3.dist-info/METADATA
+Filename: qodex_recognition-0.0.31.dist-info/METADATA
 Comment: 
 
-Filename: qodex_recognition-0.0.3.dist-info/WHEEL
+Filename: qodex_recognition-0.0.31.dist-info/WHEEL
 Comment: 
 
-Filename: qodex_recognition-0.0.3.dist-info/top_level.txt
+Filename: qodex_recognition-0.0.31.dist-info/top_level.txt
 Comment: 
 
-Filename: qodex_recognition-0.0.3.dist-info/RECORD
+Filename: qodex_recognition-0.0.31.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qodex_recognition/main.py

```diff
@@ -66,14 +66,16 @@
             return {'error': 'Car number is not found'}
         return labels['labels'][0]
 
 
 class MailNumberRecognitionRus(MailNumberRecognition):
     def parse_result(self, result):
         response = super().parse_result(result)
+        if 'error' in response:
+            return response
         if 'rus' in response:
             return response['rus']
```

## Comparing `qodex_recognition-0.0.3.dist-info/LICENSE` & `qodex_recognition-0.0.31.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qodex_recognition-0.0.3.dist-info/RECORD` & `qodex_recognition-0.0.31.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 qodex_recognition/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-qodex_recognition/main.py,sha256=rwujhhcLOmDBNOTyH8ZQfWYG0n733NYVnVbouJDAU0s,2119
+qodex_recognition/main.py,sha256=Gxe2RuAmp84DltuLxJ7sbuZu063onNLF3VlEwjabFMU,2181
 qodex_recognition/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qodex_recognition/tests/main_tests.py,sha256=fCDiM0Sm7rI2dn4dIAQ0JqS0DLMWar4XpinU_hP-SDM,432
-qodex_recognition-0.0.3.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
-qodex_recognition-0.0.3.dist-info/METADATA,sha256=iAjMcHesxq6v6tv2gf9vkkDBCNB2XM02zlgb8SiUzA4,266
-qodex_recognition-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-qodex_recognition-0.0.3.dist-info/top_level.txt,sha256=uwnIlOnugV2jqvu_vR2T1f0zn3Nl2UE2tdrxJoiUfPk,18
-qodex_recognition-0.0.3.dist-info/RECORD,,
+qodex_recognition-0.0.31.dist-info/LICENSE,sha256=6kbiFSfobTZ7beWiKnHpN902HgBx-Jzgcme0SvKqhKY,1091
+qodex_recognition-0.0.31.dist-info/METADATA,sha256=-mqDx-Hfff_PCZE31WMyzKcnsUnLWOcW5cQ9NFj9ldY,267
+qodex_recognition-0.0.31.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+qodex_recognition-0.0.31.dist-info/top_level.txt,sha256=uwnIlOnugV2jqvu_vR2T1f0zn3Nl2UE2tdrxJoiUfPk,18
+qodex_recognition-0.0.31.dist-info/RECORD,,
```

