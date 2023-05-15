# Comparing `tmp/pssm-promoter-tool-1.0.2.tar.gz` & `tmp/pssm-promoter-tool-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssm-promoter-tool-1.0.2.tar", last modified: Wed Apr 26 23:49:59 2023, max compression
+gzip compressed data, was "pssm-promoter-tool-1.0.3.tar", last modified: Mon May 15 00:03:22 2023, max compression
```

## Comparing `pssm-promoter-tool-1.0.2.tar` & `pssm-promoter-tool-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 23:49:59.218442 pssm-promoter-tool-1.0.2/
--rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.2/LICENSE.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.2/MANIFEST.in
--rw-r--r--   0 ellinium   (501) staff       (20)     4883 2023-04-26 23:49:59.218274 pssm-promoter-tool-1.0.2/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)     4426 2023-04-26 23:48:38.000000 pssm-promoter-tool-1.0.2/README.md
--rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.2/free_energy_coeffs.npy
--rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.2/model_intercept.npy
--rw-r--r--   0 ellinium   (501) staff       (20)    12158 2023-04-26 05:57:16.000000 pssm-promoter-tool-1.0.2/pssm_promoter_calculator.py
-drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-04-26 23:49:59.218063 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/
--rw-r--r--   0 ellinium   (501) staff       (20)     4883 2023-04-26 23:49:59.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/PKG-INFO
--rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-04-26 23:49:59.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/SOURCES.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 23:49:59.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/dependency_links.txt
--rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/not-zip-safe
--rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-04-26 23:49:59.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/requires.txt
--rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-04-26 23:49:59.000000 pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/top_level.txt
--rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.2/pyproject.toml
--rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-04-26 23:49:59.218492 pssm-promoter-tool-1.0.2/setup.cfg
--rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-04-26 23:49:45.000000 pssm-promoter-tool-1.0.2/setup.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:03:22.120520 pssm-promoter-tool-1.0.3/
+-rw-r--r--   0 ellinium   (501) staff       (20)     1513 2023-04-26 02:33:30.000000 pssm-promoter-tool-1.0.3/LICENSE.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       13 2023-04-26 03:55:14.000000 pssm-promoter-tool-1.0.3/MANIFEST.in
+-rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:03:22.120356 pssm-promoter-tool-1.0.3/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)     4565 2023-05-15 00:01:39.000000 pssm-promoter-tool-1.0.3/README.md
+-rw-r--r--   0 ellinium   (501) staff       (20)     2872 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.3/free_energy_coeffs.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)      136 2023-01-27 19:33:45.000000 pssm-promoter-tool-1.0.3/model_intercept.npy
+-rw-r--r--   0 ellinium   (501) staff       (20)    13075 2023-05-14 03:06:01.000000 pssm-promoter-tool-1.0.3/pssm_promoter_calculator.py
+drwxr-xr-x   0 ellinium   (501) staff       (20)        0 2023-05-15 00:03:22.120092 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/
+-rw-r--r--   0 ellinium   (501) staff       (20)     5022 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/PKG-INFO
+-rw-r--r--   0 ellinium   (501) staff       (20)      378 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)        1 2023-04-26 03:59:34.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/not-zip-safe
+-rw-r--r--   0 ellinium   (501) staff       (20)      242 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/requires.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)       25 2023-05-15 00:03:22.000000 pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/top_level.txt
+-rw-r--r--   0 ellinium   (501) staff       (20)      103 2023-04-26 02:26:58.000000 pssm-promoter-tool-1.0.3/pyproject.toml
+-rw-r--r--   0 ellinium   (501) staff       (20)       38 2023-05-15 00:03:22.120576 pssm-promoter-tool-1.0.3/setup.cfg
+-rw-r--r--   0 ellinium   (501) staff       (20)     1246 2023-05-15 00:02:23.000000 pssm-promoter-tool-1.0.3/setup.py
```

### Comparing `pssm-promoter-tool-1.0.2/LICENSE.txt` & `pssm-promoter-tool-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.2/PKG-INFO` & `pssm-promoter-tool-1.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -51,36 +51,37 @@
 4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
-5) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element
-6) hex35 -  an upstream 6-nucleotide site called the −35 motif
-7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif
-8) AA_hex35 - an amino acid sequence for the -35 motif
-9) spacer - a spacer region that separates the −10 and −35 motifs
-10) hex10 - a downstream 6-nucleotide site called the −10 motif
-11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif
-12) AA_hex10 - an amino acid sequence for the -10 motif
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) dG_total - total Gibbs free energy for the sequence
-16) dG_10 - -10 motif Gibbs free energy
-17) dG_35 - -35 motif Gibbs free energy
-18) dG_disc - a discriminator Gibbs free energy
-19) dG_ITR - an ITR Gibbs free energy
-20) dG_ext10 −10 extended motif Gibbs free energy
-21) dG_spacer - a spacer Gibbs free energy
-22) dG_UP - an UP Gibbs free energy
-23) dG_bind - binding Gibbs free energy
-24) UP_position - a position of the UP element
-25) hex35_position - a position of the -35 motif
-26) spacer_position - a position of the spacer
-27) hex10_position - a position of the -10 motif
-28) disc_position - a position of the discriminator
+5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
+9) AA_hex35 - an amino acid sequence for the -35 motif 
+10) spacer - a spacer region that separates the −10 and −35 motifs 
+11) hex10 - a downstream 6-nucleotide site called the −10 motif 
+12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+13) AA_hex10 - an amino acid sequence for the -10 motif 
+14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+16) dG_total - total Gibbs free energy for the sequence 
+17) dG_10 - -10 motif Gibbs free energy 
+18) dG_35 - -35 motif Gibbs free energy 
+19) dG_disc - a discriminator Gibbs free energy 
+20) dG_ITR - an ITR Gibbs free energy 
+21) dG_ext10 −10 extended motif Gibbs free energy 
+22) dG_spacer - a spacer Gibbs free energy 
+23) dG_UP - an UP Gibbs free energy 
+24) dG_bind - binding Gibbs free energy 
+25) UP_position - a position of the UP element 
+26) hex35_position - a position of the -35 motif 
+27) spacer_position - a position of the spacer 
+28) hex10_position - a position of the -10 motif 
+29) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.2/README.md` & `pssm-promoter-tool-1.0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -39,36 +39,37 @@
 4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
-5) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element
-6) hex35 -  an upstream 6-nucleotide site called the −35 motif
-7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif
-8) AA_hex35 - an amino acid sequence for the -35 motif
-9) spacer - a spacer region that separates the −10 and −35 motifs
-10) hex10 - a downstream 6-nucleotide site called the −10 motif
-11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif
-12) AA_hex10 - an amino acid sequence for the -10 motif
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) dG_total - total Gibbs free energy for the sequence
-16) dG_10 - -10 motif Gibbs free energy
-17) dG_35 - -35 motif Gibbs free energy
-18) dG_disc - a discriminator Gibbs free energy
-19) dG_ITR - an ITR Gibbs free energy
-20) dG_ext10 −10 extended motif Gibbs free energy
-21) dG_spacer - a spacer Gibbs free energy
-22) dG_UP - an UP Gibbs free energy
-23) dG_bind - binding Gibbs free energy
-24) UP_position - a position of the UP element
-25) hex35_position - a position of the -35 motif
-26) spacer_position - a position of the spacer
-27) hex10_position - a position of the -10 motif
-28) disc_position - a position of the discriminator
+5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
+9) AA_hex35 - an amino acid sequence for the -35 motif 
+10) spacer - a spacer region that separates the −10 and −35 motifs 
+11) hex10 - a downstream 6-nucleotide site called the −10 motif 
+12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+13) AA_hex10 - an amino acid sequence for the -10 motif 
+14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+16) dG_total - total Gibbs free energy for the sequence 
+17) dG_10 - -10 motif Gibbs free energy 
+18) dG_35 - -35 motif Gibbs free energy 
+19) dG_disc - a discriminator Gibbs free energy 
+20) dG_ITR - an ITR Gibbs free energy 
+21) dG_ext10 −10 extended motif Gibbs free energy 
+22) dG_spacer - a spacer Gibbs free energy 
+23) dG_UP - an UP Gibbs free energy 
+24) dG_bind - binding Gibbs free energy 
+25) UP_position - a position of the UP element 
+26) hex35_position - a position of the -35 motif 
+27) spacer_position - a position of the spacer 
+28) hex10_position - a position of the -10 motif 
+29) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.2/free_energy_coeffs.npy` & `pssm-promoter-tool-1.0.3/free_energy_coeffs.npy`

 * *Files identical despite different names*

### Comparing `pssm-promoter-tool-1.0.2/pssm_promoter_calculator.py` & `pssm-promoter-tool-1.0.3/pssm_promoter_calculator.py`

 * *Files 4% similar despite different names*

```diff
@@ -170,64 +170,74 @@
     new_max_rev_Tx_rate_df = res_final_df_max_rev_df.sort_values(by='Tx_rate', ascending=False)
     new_max_rev_Tx_rate = new_max_rev_Tx_rate_df['Tx_rate'].head(1).values[0]
 
     res_final_df_min_rev_df = res_final_df_min.loc[res_final_df_min["direction"] == 'rev']
     new_min_rev_Tx_rate_df = res_final_df_min_rev_df.sort_values(by='Tx_rate', ascending=False)
     new_min_rev_Tx_rate = new_min_rev_Tx_rate_df['Tx_rate'].tail(1).values[0]
 
-    column_list = ["new_gene_sequence", "promoter_sequence", "TSS", "Tx_rate", "UP", "hex35", "PSSM_hex35", "AA_hex35", "spacer", "hex10", "PSSM_hex10", "AA_hex10", "disc", "ITR", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
+    column_list = ["new_gene_sequence", "promoter_sequence", "TSS", "Tx_rate", "Tx_rate_FoldChange", "UP", "hex35", "PSSM_hex35", "AA_hex35", "spacer", "hex10", "PSSM_hex10", "AA_hex10", "disc", "ITR", "dG_total", "dG_10", "dG_35", "dG_disc", "dG_ITR", "dG_ext10", "dG_spacer", "dG_UP", "dG_bind",  "UP_position", "hex35_position", "spacer_position", "hex10_position", "disc_position"]
+
+    ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float)
+    ##max_fwd_TSS_df = fwd_res_df_max.loc[fwd_res_df_max['Tx_rate'].astype(float) >= float(def_fwd_max_tx_rate)]
 
     print("\n")
     print("The minimum transcription rate for the sequence (forward) is " + str(def_fwd_min_tx_rate))
     if len(res_final_df_min_fwd_df) > 1:
         min_fwd_output_file = OUTPUT_FILE_NAME + "_MIN_FWD_results.csv"
         if float(new_min_fwd_Tx_rate) < float(def_fwd_min_tx_rate):
             print ("can be decreased up to " + str(new_min_fwd_Tx_rate))
             print("using the promoters in the " + min_fwd_output_file)
-            res_final_df_max_fwd_df.to_csv(min_fwd_output_file, columns = column_list)
+            #res_final_df_min_fwd_df['Tx_rate_FoldChange'] = res_final_df_min_fwd_df['Tx_rate'].copy()/def_fwd_min_tx_rate.astype(float)
+            res_final_df_min_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_fwd_df,def_fwd_min_tx_rate)
+            res_final_df_min_fwd_df.to_csv(min_fwd_output_file, columns = column_list, float_format='%.2f')
 
             ##files.download(min_fwd_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\n")
     print("The minimum transcription rate for the sequence (reverse) is " + str(def_rev_min_tx_rate))
     if len(res_final_df_min_rev_df) > 1:
         min_rev_output_file = OUTPUT_FILE_NAME + "_MIN_REV_results.csv"
         if float(new_min_rev_Tx_rate) < float(def_rev_min_tx_rate):
             print ("can be decreased up to " + str(new_min_rev_Tx_rate))
             print("using the promoters in the " + min_rev_output_file)
-            res_final_df_max_fwd_df.to_csv(min_rev_output_file, columns = column_list)
+            res_final_df_min_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_min_rev_df,def_rev_min_tx_rate)
+            res_final_df_min_rev_df.to_csv(min_rev_output_file, columns = column_list, float_format='%.2f')
 
             ##files.download(min_rev_output_file)
 
     else:
         print(" cannot be further decreased")
 
     print("\n")
     print("The maximum transcription rate for the sequence (forward) is " + str(def_fwd_max_tx_rate))
     if len(res_final_df_max_fwd_df) > 1:
         max_fwd_output_file = OUTPUT_FILE_NAME + "_MAX_FWD_results.csv"
         if float(new_max_fwd_Tx_rate) > float(def_fwd_max_tx_rate):
             print ("can be increased up to " + str(new_max_fwd_Tx_rate))
             print("using the promoters in the " + max_fwd_output_file)
-            res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list)
+            res_final_df_max_fwd_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_fwd_df,def_fwd_max_tx_rate)
+
+            res_final_df_max_fwd_df.to_csv(max_fwd_output_file, columns = column_list, float_format='%.2f')
             ##files.download(max_fwd_output_file)
 
     else:
         print(" cannot be further increased")
     print("\n")
     print("The maximum transcription rate for the sequence (reverse) is " + str(def_rev_max_tx_rate))
     if len(res_final_df_max_rev_df) > 1:
         max_rev_output_file = OUTPUT_FILE_NAME + "_MAX_REV_results.csv"
         if float(new_max_rev_Tx_rate) > float(def_rev_max_tx_rate):
             print ("can be increased up to " + str(new_max_rev_Tx_rate))
             print("using the promoters in the " + max_rev_output_file)
-            res_final_df_max_fwd_df.to_csv(max_rev_output_file, columns = column_list)
+            res_final_df_max_rev_df = pssm_util.add_txrate_foldchange_col(res_final_df_max_rev_df,def_rev_max_tx_rate)
+
+            res_final_df_max_rev_df.to_csv(max_rev_output_file, columns = column_list, float_format='%.2f')
             ##files.download(max_rev_output_file)
 
     else:
         print(" cannot be further increased")
 
     end_time = datetime.now()
     print('Duration: {}'.format(end_time - start_time))
```

### Comparing `pssm-promoter-tool-1.0.2/pssm_promoter_tool.egg-info/PKG-INFO` & `pssm-promoter-tool-1.0.3/pssm_promoter_tool.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pssm-promoter-tool
-Version: 1.0.2
+Version: 1.0.3
 Summary: The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence
 Home-page: https://github.com/ellinium/PSSM_PromoterTool
 Author: Ellina Trofimova
 Author-email: ellina.trofimova@gmail.com
 License: GNU General Public License
 Keywords: promoter prediction transcription rate
 Description-Content-Type: text/markdown
@@ -51,36 +51,37 @@
 4) PSSMPromoterCalculator_MIN_REV_results.csv - contains promoters to maximise transcription rate (reverse strand).
 
 The output file fields in the CSV files contain data from Salis' Promoter calculator and additional fields:
 1) new_sequence - contains a gene sequence (nt) with substituted promoters. Empty for the original promoters.
 2) promoter_sequence - contains -35 motif, spacer and - 10 motif
 3) TSS -  transcriptional start site
 4) Tx_rate - transcription initiation rate
-5) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element
-6) hex35 -  an upstream 6-nucleotide site called the −35 motif
-7) PSSM_hex35 - position-specific scoring matrix value for the -35 motif
-8) AA_hex35 - an amino acid sequence for the -35 motif
-9) spacer - a spacer region that separates the −10 and −35 motifs
-10) hex10 - a downstream 6-nucleotide site called the −10 motif
-11) PSSM_hex10 - position-specific scoring matrix value for the -10 motif
-12) AA_hex10 - an amino acid sequence for the -10 motif
-13) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
-14) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
-15) dG_total - total Gibbs free energy for the sequence
-16) dG_10 - -10 motif Gibbs free energy
-17) dG_35 - -35 motif Gibbs free energy
-18) dG_disc - a discriminator Gibbs free energy
-19) dG_ITR - an ITR Gibbs free energy
-20) dG_ext10 −10 extended motif Gibbs free energy
-21) dG_spacer - a spacer Gibbs free energy
-22) dG_UP - an UP Gibbs free energy
-23) dG_bind - binding Gibbs free energy
-24) UP_position - a position of the UP element
-25) hex35_position - a position of the -35 motif
-26) spacer_position - a position of the spacer
-27) hex10_position - a position of the -10 motif
-28) disc_position - a position of the discriminator
+5) Tx_rate_FoldChange - the fold change between the original transcription rate and re-calculated with PSSM primers
+6) UP - a 20-nucleotide region that appears upstream of the −35 motif, called the UP element 
+7) hex35 -  an upstream 6-nucleotide site called the −35 motif 
+8) PSSM_hex35 - position-specific scoring matrix value for the -35 motif \
+9) AA_hex35 - an amino acid sequence for the -35 motif 
+10) spacer - a spacer region that separates the −10 and −35 motifs 
+11) hex10 - a downstream 6-nucleotide site called the −10 motif 
+12) PSSM_hex10 - position-specific scoring matrix value for the -10 motif 
+13) AA_hex10 - an amino acid sequence for the -10 motif 
+14) disc - a typically 6-nucleotide region in between the −10 motif and TSS, called the discriminator (Disc)
+15) ITR - the first 20 transcribed nucleotides, called the initial transcribed region (ITR)
+16) dG_total - total Gibbs free energy for the sequence 
+17) dG_10 - -10 motif Gibbs free energy 
+18) dG_35 - -35 motif Gibbs free energy 
+19) dG_disc - a discriminator Gibbs free energy 
+20) dG_ITR - an ITR Gibbs free energy 
+21) dG_ext10 −10 extended motif Gibbs free energy 
+22) dG_spacer - a spacer Gibbs free energy 
+23) dG_UP - an UP Gibbs free energy 
+24) dG_bind - binding Gibbs free energy 
+25) UP_position - a position of the UP element 
+26) hex35_position - a position of the -35 motif 
+27) spacer_position - a position of the spacer 
+28) hex10_position - a position of the -10 motif 
+29) disc_position - a position of the discriminator
 
 References:
 
 1. Logel DY, Trofimova E, Jaschke PR. Codon-Restrained Method for Both Eliminating and Creating Intragenic Bacterial Promoters. ACS Synth Biol. 2022 Jan 19;acssynbio.1c00359. Available from https://pubs.acs.org/doi/10.1021/acssynbio.1c00359. doi: 10.1021/acssynbio.1c00359
 2. LaFleur TL, Hossain A, Salis HM. Automated model-predictive design of synthetic promoters to control transcriptional profiles in bacteria. Nat Commun. 2022 Sep 2;13(1):5159. Available from https://www.nature.com/articles/s41467-022-32829-5. doi: 10.1038/s41467-022-32829-5
```

### Comparing `pssm-promoter-tool-1.0.2/setup.py` & `pssm-promoter-tool-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='pssm-promoter-tool',
-      version='1.0.2',
+      version='1.0.3',
       description='The tool applies direct and inverted Codon Restrained Promoter Silencing method to the provided gene sequence',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/ellinium/PSSM_PromoterTool',
       author='Ellina Trofimova',
       author_email='ellina.trofimova@gmail.com',
       license='GNU General Public License',
```

