# Comparing `tmp/pdivas-1.0.0.tar.gz` & `tmp/pdivas-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pdivas-1.0.0.tar", last modified: Thu Apr 20 09:02:53 2023, max compression
+gzip compressed data, was "pdivas-1.1.0.tar", last modified: Mon May 15 01:46:39 2023, max compression
```

## Comparing `pdivas-1.0.0.tar` & `pdivas-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1088 2023-04-20 06:40:12.000000 pdivas-1.0.0/LICENSE
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       25 2023-04-20 06:44:18.000000 pdivas-1.0.0/MANIFEST.in
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-04-20 09:02:53.000000 pdivas-1.0.0/PKG-INFO
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1910 2023-04-20 06:40:12.000000 pdivas-1.0.0/README.md
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)      221 2023-04-20 09:01:00.000000 pdivas-1.0.0/pdivas/__init__.py
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     7315 2023-04-20 09:00:17.000000 pdivas-1.0.0/pdivas/__main__.py
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas/model/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)  1897567 2023-04-20 06:40:12.000000 pdivas-1.0.0/pdivas/model/PDIVAS.sav
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     4316 2023-04-20 06:40:12.000000 pdivas-1.0.0/pdivas/scoring_to_vcf.py
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2111 2023-04-20 08:31:42.000000 pdivas-1.0.0/pdivas/vcf2tsv.py
-drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-04-20 09:02:53.000000 pdivas-1.0.0/pdivas.egg-info/
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/PKG-INFO
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)      342 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/SOURCES.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)        1 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/dependency_links.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       48 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/entry_points.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       40 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/requires.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)        7 2023-04-20 09:02:52.000000 pdivas-1.0.0/pdivas.egg-info/top_level.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       44 2023-04-20 06:44:18.000000 pdivas-1.0.0/requirements.txt
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)       38 2023-04-20 09:02:53.000000 pdivas-1.0.0/setup.cfg
--rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1650 2023-04-20 07:56:35.000000 pdivas-1.0.0/setup.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-05-15 01:46:39.768249 pdivas-1.1.0/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1088 2023-04-20 06:40:12.000000 pdivas-1.1.0/LICENSE
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       25 2023-04-20 06:44:18.000000 pdivas-1.1.0/MANIFEST.in
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-05-15 01:46:39.766252 pdivas-1.1.0/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1910 2023-04-20 06:40:12.000000 pdivas-1.1.0/README.md
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-05-15 01:46:39.667921 pdivas-1.1.0/pdivas/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      221 2023-05-15 01:45:45.000000 pdivas-1.1.0/pdivas/__init__.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     7222 2023-05-15 01:45:33.000000 pdivas-1.1.0/pdivas/__main__.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-05-15 01:46:39.739241 pdivas-1.1.0/pdivas/model/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)  1897567 2023-04-20 06:40:12.000000 pdivas-1.1.0/pdivas/model/PDIVAS.sav
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     4316 2023-04-20 06:40:12.000000 pdivas-1.1.0/pdivas/scoring_to_vcf.py
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2146 2023-05-15 01:40:31.000000 pdivas-1.1.0/pdivas/vcf2tsv.py
+drwxrwxrwx   0 shiro     (1000) shiro     (1000)        0 2023-05-15 01:46:39.724709 pdivas-1.1.0/pdivas.egg-info/
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     2233 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/PKG-INFO
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)      342 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        1 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       48 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/entry_points.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       40 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/requires.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)        7 2023-05-15 01:46:39.000000 pdivas-1.1.0/pdivas.egg-info/top_level.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       44 2023-04-20 06:44:18.000000 pdivas-1.1.0/requirements.txt
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)       38 2023-05-15 01:46:39.769249 pdivas-1.1.0/setup.cfg
+-rwxrwxrwx   0 shiro     (1000) shiro     (1000)     1650 2023-04-20 07:56:35.000000 pdivas-1.1.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pdivas-1.0.0/LICENSE` & `pdivas-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdivas-1.0.0/PKG-INFO` & `pdivas-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdivas
-Version: 1.0.0
+Version: 1.1.0
 Summary: PDIVAS: Pathogenicity predictor for Deep-Intronic Variants causing Aberrant Splicing
 Home-page: https://github.com/shiro-kur/PDIVAS
 Author: Ryo Kurosawa
 Author-email: a0160561@yahoo.co.jp
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pdivas-1.0.0/README.md` & `pdivas-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pdivas-1.0.0/pdivas/__main__.py` & `pdivas-1.1.0/pdivas/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,18 +11,14 @@
 import csv
 
 from .__init__ import __cur_path__, __version__
 from pdivas.scoring_to_vcf import scoring_to_vcf
 from pdivas.vcf2tsv import vep_editor
 from pdivas.vcf2tsv import vep_ai_matcher
 
-#https://qiita.com/kzkadc/items/e4fc7bc9c003de1eb6d0
-#http://www.yamamo10.jp/yamamoto/comp/Python/library/argparse/sample/prog/index.html
-#https://qiita.com/tanabe13f/items/6c09f8f71eb2efb1ac75
-
 def get_options():
     parser = argparse.ArgumentParser(
         prog="pdivas",
         formatter_class=argparse.RawDescriptionHelpFormatter,
         description=(
                 " ========================================================================================\n"
                 "|| PDIVAS: Pathogenicity predictor for Deep-Intronic Variants causing Aberrant Splicing ||\n"
@@ -168,21 +164,21 @@
     uniq_annots = set([])
     uniq_vars = set([])
 
     for var in vcf:
         itera += 1
         
         if (var.INFO.get("CSQ") is None) :
-            print(var.INFO["CSQ"])
-            filt_csq += 1
+            print(var.CHROM, var.start, var.end, var.ID)
+            filt_vep_error += 1
             continue
 
         if (var.INFO.get("SpliceAI") is None) :
             filt_ai_error += 1
-            elem = vep_editor(var,vep_info_index)
+            elem = vep_editor(var,vep_info_index,spliceai_info_index,PD_info_index)
         
         else :
             elem = vep_ai_matcher(var,vep_info_index,spliceai_info_index,PD_info_index)
             
         if len(elem) == 0 :
             print("Output error")
             break
@@ -191,32 +187,33 @@
             var_ID = ":".join([str(k) for k in [var.CHROM,var.start+1,var.REF,var.ALT[0]]])
             uniq_vars.add(var_ID)
 
         for gen in range(len(elem)) :
             annot_ID = ":".join([str(k) for k in [var.CHROM,var.start+1,var.REF,var.ALT[0],elem[gen][12]]])
             if annot_ID in uniq_annots :
                 print("duplication detected @",annot_ID)
+                oup_list = elem[gen]
+                csv_writer.writerow(oup_list)
                 continue
+
             uniq_annots.add(annot_ID)
             
             oup_list = elem[gen]
             csv_writer.writerow(oup_list)
 
 
     vcf.close()
     csvfile.close()
 
     print("# of input variants : ",itera)
     print("# of VEP-lacked variants :",filt_vep_error,";",round(100*filt_vep_error/itera,2),"(%)")
     print("# of AI-lacked variants :",filt_ai_error,";",round(100*filt_ai_error/itera,2),"(%)")
-    print("# of output variants :",len(uniq_vars),";",round(100*len(uniq_vars)/itera,2),"(%)")
-    print("# of output annotations : ",len(uniq_annots))
-
+    print("# of output unique variants :",len(uniq_vars),";",round(100*len(uniq_vars)/itera,2),"(%)")
+    print("# of output unique annotations : ",len(uniq_annots))
 
-#https://www.javadrive.jp/python/userfunc/index5.html
 def main(args=None):
     args,parser = get_options()
     if hasattr(args, 'handler'):
         args.handler(args)
     else:
         # show help for unknown subcommands
         parser.print_help()
```

### Comparing `pdivas-1.0.0/pdivas/model/PDIVAS.sav` & `pdivas-1.1.0/pdivas/model/PDIVAS.sav`

 * *Files identical despite different names*

### Comparing `pdivas-1.0.0/pdivas/scoring_to_vcf.py` & `pdivas-1.1.0/pdivas/scoring_to_vcf.py`

 * *Files identical despite different names*

### Comparing `pdivas-1.0.0/pdivas/vcf2tsv.py` & `pdivas-1.1.0/pdivas/vcf2tsv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from cyvcf2 import VCF, Writer
 import csv
 import sys
 
-def vep_editor(var,vep_info_index):
+def vep_editor(var,vep_info_index,spliceai_info_index,PD_info_index):
     vep_annot = {dict(zip(vep_info_index, x.strip().split("|")))["Gene"]:
                         x.strip().split("|")
                         for x in var.INFO["CSQ"].strip().split(",")}
     
     base_anno = [var.CHROM,var.start+1,var.ID,var.REF,var.ALT[0],var.QUAL,(var.FILTER or "PASS")]
     oup_list = []
     
@@ -44,8 +44,8 @@
                 oup_list += [base_anno+vep_annot[gene_id]+\
                              spliceai_annot[gene_id]+list(PD_annot.values())[0]]
 
         else :
             oup_list += [base_anno+vep_annot[gene_id]+\
                          ["." for i in range(len(spliceai_info_index))]+["." for i in range(len(PD_info_index))]]     
 
-    return oup_list
+    return oup_list
```

### Comparing `pdivas-1.0.0/pdivas.egg-info/PKG-INFO` & `pdivas-1.1.0/pdivas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdivas
-Version: 1.0.0
+Version: 1.1.0
 Summary: PDIVAS: Pathogenicity predictor for Deep-Intronic Variants causing Aberrant Splicing
 Home-page: https://github.com/shiro-kur/PDIVAS
 Author: Ryo Kurosawa
 Author-email: a0160561@yahoo.co.jp
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pdivas-1.0.0/setup.py` & `pdivas-1.1.0/setup.py`

 * *Files identical despite different names*

