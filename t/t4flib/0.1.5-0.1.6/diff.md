# Comparing `tmp/t4flib-0.1.5-py2.py3-none-any.whl.zip` & `tmp/t4flib-0.1.6-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 7994 bytes, number of entries: 10
+Zip file size: 8014 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-11 18:20 t4flib/__init__.py
 -rw-rw-r--  2.0 unx      892 b- defN 23-May-11 18:20 t4flib/config.py
--rw-rw-r--  2.0 unx     6029 b- defN 23-May-12 18:55 t4flib/file_helper.py
+-rw-rw-r--  2.0 unx     6097 b- defN 23-May-15 14:56 t4flib/file_helper.py
 -rw-rw-r--  2.0 unx     4508 b- defN 23-May-11 18:20 t4flib/filetransfer_helper.py
 -rw-rw-r--  2.0 unx     3259 b- defN 23-May-11 18:20 t4flib/gcloud_helper.py
 -rw-rw-r--  2.0 unx      753 b- defN 23-May-11 18:20 t4flib/log_helper.py
--rw-rw-r--  2.0 unx     1747 b- defN 23-May-12 19:00 t4flib-0.1.5.dist-info/METADATA
--rw-rw-r--  2.0 unx      110 b- defN 23-May-12 19:00 t4flib-0.1.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-12 19:00 t4flib-0.1.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      758 b- defN 23-May-12 19:00 t4flib-0.1.5.dist-info/RECORD
-10 files, 18063 bytes uncompressed, 6710 bytes compressed:  62.9%
+-rw-rw-r--  2.0 unx     1747 b- defN 23-May-15 15:10 t4flib-0.1.6.dist-info/METADATA
+-rw-rw-r--  2.0 unx      110 b- defN 23-May-15 15:10 t4flib-0.1.6.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-15 15:10 t4flib-0.1.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      758 b- defN 23-May-15 15:10 t4flib-0.1.6.dist-info/RECORD
+10 files, 18131 bytes uncompressed, 6730 bytes compressed:  62.9%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: t4flib/gcloud_helper.py
 Comment: 
 
 Filename: t4flib/log_helper.py
 Comment: 
 
-Filename: t4flib-0.1.5.dist-info/METADATA
+Filename: t4flib-0.1.6.dist-info/METADATA
 Comment: 
 
-Filename: t4flib-0.1.5.dist-info/WHEEL
+Filename: t4flib-0.1.6.dist-info/WHEEL
 Comment: 
 
-Filename: t4flib-0.1.5.dist-info/top_level.txt
+Filename: t4flib-0.1.6.dist-info/top_level.txt
 Comment: 
 
-Filename: t4flib-0.1.5.dist-info/RECORD
+Filename: t4flib-0.1.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## t4flib/file_helper.py

```diff
@@ -71,16 +71,19 @@
     logger('INFO', 'Début de la concaténation des fichiers CSV')
 
     try:
 
         # obtenir la liste de tous les fichiers .csv dans le dossier source
         file_list = get_all_file_by_filemask(source_dir, '*.csv')
 
-        if len(file_list) > 0:
-            liste_data = []
+        if len(file_list) == 0:
+            logger('WARNING', 'Pas de données CSV à concaténer')
+            return
+
+        liste_data = []
 
         # Parcourez la liste des fichiers et lisez chaque fichier CSV
         for fichier in file_list:
             # Lisez le fichier CSV dans un DataFrame
             donnees = pd.read_csv(str(fichier.absolute()), delimiter=';')
 
             # Ajoutez les données du fichier actuel au DataFrame global
@@ -165,12 +168,12 @@
 def copy_files_by_filemask(source_dir, dest_dir, filemask):
     logger('INFO', f'Copie des ficher du dossier {source_dir} vers {dest_dir}')
 
     try:
         files = get_all_file_by_filemask(source_dir, filemask)
 
         for file in files:
-            shutil.copyfile(str(file.absolute()), f'{dest_dir}/{file.name}')
+            shutil.copyfile(str(file.absolute()), dest_dir)
     except Exception as e:
         logger('ERROR', str(e))
         raise
     logger('INFO', 'L\'ensemble des fichiers ont été copiés')
```

## Comparing `t4flib-0.1.5.dist-info/METADATA` & `t4flib-0.1.6.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: t4flib
-Version: 0.1.5
+Version: 0.1.6
 Summary: Librairie de fonction utiles pour T4F
 Home-page: http://gitlab.dev.fr.auchan.com/tech4finance/t4flib.git
 Author: Corentin DEVROUETE
 Author-email: cdevrouete@advanced-schema.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `t4flib-0.1.5.dist-info/RECORD` & `t4flib-0.1.6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 t4flib/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 t4flib/config.py,sha256=fHt2THXtajPzzV_gnHPZNVmez09ODLfIFrt4cTXgZsE,892
-t4flib/file_helper.py,sha256=aXMnpS1zcXR70_YN99tJZ1g-ViOi3I5Hp83e2qiD5Ew,6029
+t4flib/file_helper.py,sha256=VBJPdJwoAyQzwtpUFRJGo9JvEd7qQe_NfgqPnKbN2ZE,6097
 t4flib/filetransfer_helper.py,sha256=mbi_R4cahDFTnPGO4zD_7txD8t1_SQrxPIIRSJvxCdg,4508
 t4flib/gcloud_helper.py,sha256=Y4u_y4fy4zDjXKEmwBV91Yl4x9FNJsSmDLEKLwzDqJ0,3259
 t4flib/log_helper.py,sha256=uRHKVgfhq6V4PY64lrRnrjzoA99OcyKI-bcr0vUnv_I,753
-t4flib-0.1.5.dist-info/METADATA,sha256=Pyv6VuOan3Y_5AMyVcXz_zLVHHn-U_7gvTPNrepYNAs,1747
-t4flib-0.1.5.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-t4flib-0.1.5.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
-t4flib-0.1.5.dist-info/RECORD,,
+t4flib-0.1.6.dist-info/METADATA,sha256=qliOYX_0DBv9qiyrUgGePVUPFwMt2t1Ef4J7hwyDlmw,1747
+t4flib-0.1.6.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+t4flib-0.1.6.dist-info/top_level.txt,sha256=-05r3tdNDBMHneiATbWVqDQI7djLF9N83J6mAMcxbp8,7
+t4flib-0.1.6.dist-info/RECORD,,
```

