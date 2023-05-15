# Comparing `tmp/pssm-promoter-tool-1.0.3.tar.gz` & `tmp/pssm-promoter-tool-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssm-promoter-tool-1.0.3.tar", last modified: Mon May 15 00:03:22 2023, max compression
+gzip compressed data, was "pssm-promoter-tool-1.0.4.tar", last modified: Mon May 15 00:19:59 2023, max compression
```

## Comparing `pssm-promoter-tool-1.0.3.tar` & `pssm-promoter-tool-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:03:22.120520 pssm-promoter-tool-1.0.3/
--rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.3/LICENSE.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.3/MANIFEST.in
--rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:03:22.120356 pssm-promoter-tool-1.0.3/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)     4565 2023-05-15 00:01:39.000000 pssm-promoter-tool-1.0.3/README.md
--rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.3/free_energy_coeffs.npy
--rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.3/model_intercept.npy
--rw-r--r--   0 ellinium   (501) staff       (20)    13075 2023-05-14 03:06:01.000000 pssm-promoter-tool-1.0.3/pssm_promoter_calculator.py
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:03:22.120092 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/
--rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/not-zip-safe
--rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/requires.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/top_level.txt
--rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.3/pyproject.toml
--rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-15 00:03:22.120576 pssm-promoter-tool-1.0.3/setup.cfg
--rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-15 00:02:23.000000 pssm-promoter-tool-1.0.3/setup.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:19:59.655983 pssm-promoter-tool-1.0.4/
+-rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.4/LICENSE.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.4/MANIFEST.in
+-rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:19:59.655809 pssm-promoter-tool-1.0.4/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)     4565 2023-05-15 00:19:10.000000 pssm-promoter-tool-1.0.4/README.md
+-rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.4/free_energy_coeffs.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.4/model_intercept.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)    13075 2023-05-14 03:06:01.000000 pssm-promoter-tool-1.0.4/pssm_promoter_calculator.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:19:59.655454 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/
+-rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/not-zip-safe
+-rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/requires.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-15 00:19:59.000000 pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/top_level.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.4/pyproject.toml
+-rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-15 00:19:59.656034 pssm-promoter-tool-1.0.4/setup.cfg
+-rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-15 00:19:49.000000 pssm-promoter-tool-1.0.4/setup.py
```

### Comparing `pssm-promoter-tool-1.0.3/LICENSE.txt` & `pssm-promoter-tool-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.3/PKG-INFO` & `pssm-promoter-tool-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.3
+Version: 1.0.4
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -41,18 +41,18 @@
 From the folder with the downloaded files run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
 Depending on the result, up to four output CSV files can be generated:
-1) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
-2) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
-3) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
-4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
+1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
+2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
+3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
+4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
 5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
```

### Comparing `pssm-promoter-tool-1.0.3/README.md` & `pssm-promoter-tool-1.0.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 From the folder with the downloaded files run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
 Depending on the result, up to four output CSV files can be generated:
-1) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
-2) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
-3) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
-4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
+1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
+2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
+3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
+4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
 5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
```

### Comparing `pssm-promoter-tool-1.0.3/free_energy_coeffs.npy` & `pssm-promoter-tool-1.0.4/free_energy_coeffs.npy`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.3/pssm_promoter_calculator.py` & `pssm-promoter-tool-1.0.4/pssm_promoter_calculator.py`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/PKG-INFO` & `pssm-promoter-tool-1.0.4/pssm_promoter_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.3
+Version: 1.0.4
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -41,18 +41,18 @@
 From the folder with the downloaded files run:
 ```
 python pssm_promoter_calculator.py <file_name>
 ```
 where 'file_name' is a path to the file with a gene sequence (TXT or FASTA format).
 
 Depending on the result, up to four output CSV files can be generated:
-1) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
-2) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
-3) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
-4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
+1) PSSMPromoterCalculator_MIN_FWD_results.csv - contains promoters to minimise transcription rate (forward strand)
+2) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to minimise transcription rate (reverse strand)
+3) PSSMPromoterCalculator_MAX_FWD_results.csv - contains promoters to maximise transcription rate (forward strand)
+4) PSSMPromoterCalculator_MAX_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
 5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
```

### Comparing `pssm-promoter-tool-1.0.3/setup.py` & `pssm-promoter-tool-1.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pssm-promoter-tool',
-      version='1.0.3',
+      version='1.0.4',
       description='The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ellinium/PSSM_PromoterTool',
       author='Ellina Trofimova',
       author_email='ellina.trofimova@gmail.com',
       license='GNU General Public License',
```

