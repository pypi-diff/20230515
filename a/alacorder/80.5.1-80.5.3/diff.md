# Comparing `tmp/alacorder-80.5.1.tar.gz` & `tmp/alacorder-80.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.5.1.tar", max compression
+gzip compressed data, was "alacorder-80.5.3.tar", max compression
```

## Comparing `alacorder-80.5.1.tar` & `alacorder-80.5.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.1/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.1/README.md
--rw-r--r--   0        0        0      746 2023-05-14 14:16:27.040873 alacorder-80.5.1/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-14 00:21:47.679650 alacorder-80.5.1/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.1/src/alacorder/__init__.py
--rw-r--r--   0        0        0   218348 2023-05-14 14:13:42.945251 alacorder-80.5.1/src/alacorder/__main__.py
--rw-r--r--   0        0        0   218348 2023-05-14 14:12:36.830180 alacorder-80.5.1/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.3/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.3/README.md
+-rw-r--r--   0        0        0      746 2023-05-15 02:30:04.829419 alacorder-80.5.3/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-14 14:20:06.372148 alacorder-80.5.3/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   272869 2023-05-15 02:28:43.447468 alacorder-80.5.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   272869 2023-05-15 02:28:29.605882 alacorder-80.5.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.3/PKG-INFO
```

### Comparing `alacorder-80.5.1/LICENSE` & `alacorder-80.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.1/README.md` & `alacorder-80.5.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.1/pyproject.toml` & `alacorder-80.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.5.1"
+version = "80.5.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.5.1/src/alacorder/.DS_Store` & `alacorder-80.5.3/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.1/src/alacorder/__main__.py` & `alacorder-80.5.3/src/alacorder/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.1"
+version = "80.5.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2274,15 +2274,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2360,27 +2360,1787 @@
                 pl.col("CERVDisqConviction")
                 | pl.col("PardonDisqConviction")
                 | pl.col("PermanentDisqConviction")
             )
             .then((pl.col("TotalBalance") - pl.col("TotalD999")))
             .otherwise(None)
             .alias("PaymentToRestore"),
+            pl.col("RAWDESC").alias("Description"),
+            pl.col("RAWCITE").alias("Cite")
         ]
     )
-    aggch = charges.groupby("CASENONUM").agg("CaseNumber", "RAWCITE", "RAWDESC")
-    aggch = aggch.select(
+    charges = charges.fill_null("")
+        # fix missing PFI3
+    charges = charges.with_columns(
         [
-            pl.col("CASENONUM"),
-            pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
-            pl.col("RAWDESC").arr.get(0).alias("Description"),
-            pl.col("RAWCITE").arr.get(0).alias("Cite"),
+            pl.when(pl.col("Code")=="PFI3")
+            .then("POSSESS FORGED INSTRUMENT 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PFI3")
+            .then("13A-009-006.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing NWNI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="NWNI")
+            .then("NEGOTIATING WORTHLESS INST")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="NWNI")
+            .then("13A-009-013.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDR1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR1")
+            .then("USE/POSSESS DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR1")
+            .then("13A-012-260(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UPCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UPCS")
+            .then("POSS. CONTR. SUBS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UPCS")
+            .then("13A-012-212(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FRCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FRCC")
+            .then("FRAUD USE CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FRCC")
+            .then("13A-012-212(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T003
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T003")
+            .then("NO DRIVERS LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T003")
+            .then("032-006-001(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PMIO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PMIO")
+            .then("PORN POSS MATERIAL MINORS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PMIO")
+            .then("13A-012-192(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UPCC")
+            .then("POSS CONTR SUBS INTENT DISTRIB")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UPCC")
+            .then("013-012-192(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BEMV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BEMV")
+            .then("BREAK/ENTER VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BEMV")
+            .then("13A-008-011(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HARA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HARA")
+            .then("HARASSMENT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HARA")
+            .then("13A-011-008(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TET3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TET3")
+            .then("THEFT OF PROPERTY 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TET3")
+            .then("13A-008-004.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T042
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T042")
+            .then("OVERWEIGHT TRUCK")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T042")
+            .then("032-009-020(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T707
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T707")
+            .then("FAIL DISPLAY INSURANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T707")
+            .then("032-07A-016(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SX12
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SX12")
+            .then("SEX ABUSE-CHILD LESS 12 YOA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SX12")
+            .then("13A-006-069.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRAK
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAK")
+            .then("TRAFFICKING-METHAMPHETAMINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAK")
+            .then("13A-012-231(11)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FCDC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FCDC")
+            .then("FRAUD USE CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FCDC")
+            .then("13A-009-014(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TOD3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOD3")
+            .then("THEFT/DECEPTION 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOD3")
+            .then("13A-008-004.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUV")
+            .then("UNAUTHORIZED USE VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUV")
+            .then("13A-008-011(A)1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T012
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T012")
+            .then("FAIL STOP SIGN")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T012")
+            .then("032-05A-112(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FR3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FR3D")
+            .then("FORGERY 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FR3D")
+            .then("13A-009-003.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HCOM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HCOM")
+            .then("HARASSING COMMUNICATIONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HCOM")
+            .then("13A-011-008(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TP3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TP3D")
+            .then("THEFT OF PROPERTY 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TP3D")
+            .then("13A-008-4.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VPCC")
+            .then("POSS CONTROLLED SUBST BY FRAUD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VPCC")
+            .then("13A-012-212(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FORF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FORF")
+            .then("BOND FORF-FELONY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T012")
+            .then("- -BOND FORT")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T527
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T527")
+            .then("DUI-CONTROLLED SUBSTANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T527")
+            .then("032-05A-191(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA3")
+            .then("BURGLARY 3RD (UNOCCUPIED BLDG)")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA3")
+            .then("13A-007-007(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FMUR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FMUR")
+            .then("FELONY MURDER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FMUR")
+            .then("13A-006-002(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MURR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MURR")
+            .then("MURDER-RECKLESS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MURR")
+            .then("13A-006-002(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FPCC")
+            .then("ILL POSSESS CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FPCC")
+            .then("13A-009-014(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PREC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PREC")
+            .then("POSS/SELL PRECURSOR CHEMICALS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PREC")
+            .then("020-002-190(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing STSA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="STSA")
+            .then("SEXUAL TORTURE/ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="STSA")
+            .then("13A-006-065.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T582
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T582")
+            .then("EXPIRED LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T582")
+            .then("032-006-001(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM02
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM02")
+            .then("MURDER CAPITAL-ROBBERY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM02")
+            .then("13A-005-040(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDR4
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR4")
+            .then("PARAPHERNALIA - SELL/DELIVER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR4")
+            .then("13A-012-260(D)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VAPP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VAPP")
+            .then("POSSESS MARIHUANA 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VAPP")
+            .then("13A-012-213(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing MAN1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAN1")
+            .then("MANSLAUGHTER-RECKLESS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAN1")
+            .then("13A-006-003(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDR1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR1")
+            .then("USE/POSSESS DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR1")
+            .then("13A-012-260(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T755
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T755")
+            .then("NO/IMP TAG LIGHT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T755")
+            .then("032-005-240(C)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRAO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAO")
+            .then("TRAFFICKING-HEROIN")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAO")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FORM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FORM")
+            .then("BOND FORF-MISD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FORM")
+            .then("- -BOND FORT")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing SVIA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SVIA")
+            .then("SALVIA MISDEMEANOR POSSESSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SVIA")
+            .then("13A-012-214.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRAG
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAG")
+            .then("TRAFFICKING-SYNTHETIC DRUGS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAG")
+            .then("13A-012-231(12)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DSF1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DSF1")
+            .then("DISCHARGE GUN OCC BLDG/VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DSF1")
+            .then("13A-011-061(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing MISC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MISC")
+            .then("MISCELLANEOUS FILING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MISC")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA1")
+            .then("BURGLARY 3RD - DWELLING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA1")
+            .then("13A-007-007(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CEM1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CEM1")
+            .then("CHEMICAL ENDANGER MINOR")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CEM1")
+            .then("026-015-3.2(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM04
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM04")
+            .then("MURDER CAPITAL-BURGLARY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM04")
+            .then("13A-005-040(A)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing IPCD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="IPCD")
+            .then("ILL POSSESS CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="IPCD")
+            .then("13A-009-014(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T005
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T005")
+            .then("UNDER INFLUENCE CONT. SUBSTANC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T005")
+            .then("032-05A-191(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T525
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T525")
+            .then("DUI: ANY SUB WHICH IMPAIRS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T525")
+            .then("032-05A-191(A)(5)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM15
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM15")
+            .then("MURDER CAPITAL-UNDER 14 YEARS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM15")
+            .then("13A-005-040(A)(15)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DUIF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DUIF")
+            .then("DUI - FELONY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DUIF")
+            .then("032-05A-191(A)&(H)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T169
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T169")
+            .then("SPEED/ 70+ MPH OR 65+ MPH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T169")
+            .then("032-05A-171(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DUIM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DUIM")
+            .then("DUI - MISD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DUIM")
+            .then("032-05A-191(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T718
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T718")
+            .then("DUI: UNDER INFLU ALCOHOL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T718")
+            .then("032-05A-191(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DVHF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVHF")
+            .then("FELONY DV 3RD HARRASSMENT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVHF")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TROP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TROP")
+            .then("TRAFFICKING-OPIUM")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TROP")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM10
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM10")
+            .then("MURDER CAPITAL-TWO OR MORE PER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM10")
+            .then("13A-005-040(A)(10)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM17
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM17")
+            .then("MURDER CAPITAL-VEH FR OUTSIDE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM17")
+            .then("13A-005-040(A)(17)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM01
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM01")
+            .then("MURDER CAPITAL-KIDNAP")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM01")
+            .then("13A-005-040(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDRU
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRU")
+            .then("TRAFFICKING-MORPHINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRU")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T770
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T770")
+            .then("INOPERABLE BRAKE LIGHTS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T770")
+            .then("032-005-241(B)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing ACAL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ACAL")
+            .then("AGGRAVATED CHILD ABUSE < SIX")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ACAL")
+            .then("025-015-03.1(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDRY
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRY")
+            .then("TRAFFICKING-COCAINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRY")
+            .then("13A-012-231(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRFT
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRFT")
+            .then("TRAFFICKING FENTANYL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRFT")
+            .then("13A-012-231(13)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FNLE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FNLE")
+            .then("GIVING FALSE NAME TO OFF")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FNLE")
+            .then("13A-009-018.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing RS3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="RS3D")
+            .then("REC STOLEN PROP 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="RS3D")
+            .then("13A-008-18.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T806
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T806")
+            .then("NO DRIVERS LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T806")
+            .then("032-006-018(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TOS3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOS3")
+            .then("THEFT OF SERVICES 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOS3")
+            .then("13A-008-010.3")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TSIB
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TSIB")
+            .then("TRAFFICKING STOLEN IDENTITIES")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TSIB")
+            .then("13A-008-193(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T011
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T011")
+            .then("DRIVING WRONG SIDE HWY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T011")
+            .then("032-05A-080(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VAPD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VAPD")
+            .then("POSSESS MARIHUANA 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VAPD")
+            .then("13A-012-213(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T128
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRFT")
+            .then("NO TAG REGIS IN VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRFT")
+            .then("040-012-260(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing BHER
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BHER")
+            .then("BOND HEARING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BHER")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing APPL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="APPL")
+            .then("CASE APPEALED ON")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="APPL")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MRDI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MRDI")
+            .then("MURDER - INTENTIONAL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MRDI")
+            .then("13A-006-002(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUY
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUY")
+            .then("UNAUTHORIZED USE VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUY")
+            .then("13A-008-011(A)3")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T019
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T019")
+            .then("FAILURE TO DIM LIGHTS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T019")
+            .then("032-005-242(C)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T006
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T006")
+            .then("FAIL YIELD ROW")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T006")
+            .then("032-05A-112(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MAN2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAN2")
+            .then("MANSLAUGHTER-INTENT, PASSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAN2")
+            .then("13A-006-003(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM18
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM18")
+            .then("MURDER CAPITAL-FIRED FROM VEHI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM18")
+            .then("13A-005-040(A)(18)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing NUSE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="NUSE")
+            .then("NO USER PERMIT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="NUSE")
+            .then("033-015-007(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FBAP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FBAP")
+            .then("FRAUD BY AUTHORIZED PERSONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FBAP")
+            .then("13A-009-014.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDRO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRO")
+            .then("DRUG PARAPHERNALIA TO MINOR")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRO")
+            .then("13A-012-260(E)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM16
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM16")
+            .then("MURDER CAPITAL-DWELL FR OUTSID")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM16")
+            .then("13A-005-040(A)(16)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing EDCO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="EDCO")
+            .then("ENDG WELFARE CHILD-OCCUPATION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="EDCO")
+            .then("13A-013-006(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T096
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T096")
+            .then("MOVING TRAFFIC VIO")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T096")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing THBV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="THBV")
+            .then("HOMICIDE BY VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="THBV")
+            .then("032-05A-190.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing ASTM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ASTM")
+            .then("ALCOHOL-SALE/PERMIT UNDER AGE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ASTM")
+            .then("028-03A-025(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SAVI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SAVI")
+            .then("SALVIA FELONY POSSESSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SAVI")
+            .then("13A-012-214.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVFC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVFC")
+            .then("FELONY DV CRIM MISCHIEF 2D/3D")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVFC")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T128
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T128")
+            .then("NO TAG REGIS IN VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T128")
+            .then("040-012-260(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T071
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T071")
+            .then("COMBINED INFLUENCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T071")
+            .then("032-05A-191(A)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM07
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM07")
+            .then("MURDER CAPITAL-FOR HIRE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM07")
+            .then("13A-005-040(A)(7)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRBF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRBF")
+            .then("TR-FORT.")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRBF")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T813
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T813")
+            .then("MOVE OVER LAW")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T813")
+            .then("032-05A-058.2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM03
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM03")
+            .then("MURDER CAPITAL-RAPE/SODOMY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM03")
+            .then("13A-005-040(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRMA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRMA")
+            .then("TRAFFICKING-MARIJUANA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRMA")
+            .then("13A-012-231(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T783
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T783")
+            .then("IMPEDING FLOW TRAFFIC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T783")
+            .then("032-05A-080(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T091
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T091")
+            .then("DUI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T091")
+            .then("032-05A-191(A)1/2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T072
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T072")
+            .then("UNDER INFLU - ANY SUBSTANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T072")
+            .then("032-05A-191(A)5")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TOS2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOS2")
+            .then("THEFT OF SERVICES 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOS2")
+            .then("13A-008-010.2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DV36
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DV36")
+            .then("FELONY DV CRIM MISCHIEF 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DV36")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DSF2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DSF2")
+            .then("DISCHARGE GUN UNOCC BLDG/VEH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DSF2")
+            .then("13A-011-061(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM08
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM08")
+            .then("MURDER CAPITAL-SEXUAL ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM08")
+            .then("13A-005-040(A)(8)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DOG1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DOG1")
+            .then("DOG/CAT CRUELTY 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DOG1")
+            .then("13A-011-241(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CEM3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CEM3")
+            .then("CHEMICAL ENDANGER MINOR/DEATH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CEM3")
+            .then("026-015-3.2(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing PACS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PACS")
+            .then("PROHIBITED ACTS-MAIN BLD/DWL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PACS")
+            .then("020-002-071(A)(5)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T097
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T097")
+            .then("OTHER NON MOVING VIO")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T097")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDR2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR2")
+            .then("DEL/SALE DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR2")
+            .then("13A-012-260(E)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA2")
+            .then("BURGLARY 3RD - OCCUPIED BLDG")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA2")
+            .then("13A-007-007(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVFC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVFC")
+            .then("FELONY DV CRIM MISCHIEF 2D/3D")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVFC")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TS3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TS3D")
+            .then("THEFT OF SERVICES 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TS3D")
+            .then("13A-008-010.25")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CODL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CODL")
+            .then("CONTRIBUTING TO THE DELINQUENC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CODL")
+            .then("012-015-111(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HAR2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HAR2")
+            .then("HARASSMENT - THREAT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HAR2")
+            .then("13A-011-008(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T506
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T506")
+            .then("FAIL TO YIELD EMER VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T506")
+            .then("032-05A-115(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HGAR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HGAR")
+            .then("FAILURE TO COMPLY - GARBAGE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HGAR")
+            .then("022-027-003(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRCN
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRCN")
+            .then("TR-CONTEMPT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRCN")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T773
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T773")
+            .then("IMP TAIL LIGHTS-TRAILER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T773")
+            .then("032-005-240(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PCUR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PCUR")
+            .then("FAIL CPLY REPORTS-PRECUR CHEMS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PCUR")
+            .then("020-002-190(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PPRE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PPRE")
+            .then("POSS OF PRE-CURSOR CHEMICALS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PPRE")
+            .then("020-002-181(D)(13)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T507
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T507")
+            .then("FAIL TO YIELD RIGHT OF WAY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T507")
+            .then("032-05A-082(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T081
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T081")
+            .then("NO HDLGTS WHEN REQUIRED")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T081")
+            .then("032-005-240(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PARA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PARA")
+            .then("FAILURE COMPLY PARK CONDITIONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PARA")
+            .then("220-005-013(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MAAL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAAL")
+            .then("ALCOHOL- MINOR/POSS/CONSUME")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAAL")
+            .then("028-03A-025(A)(18)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PCAB
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PCAB")
+            .then("POSS/CONT ALCOHOL-STATE PARK")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PCAB")
+            .then("220-005-016(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DOG2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DOG2")
+            .then("DOG/CAT CRUELTY 2ND DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DOG2")
+            .then("13A-011-241(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SFUF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SFUF")
+            .then("SETTING FIRE-UNCL FOREST/WOOD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SFUF")
+            .then("009-013-011(B)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing OSUA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="OSUA")
+            .then("OMMISSION/MISREP SALE SECURITI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="OSUA")
+            .then("008-006-017(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing OSUA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="OSUA")
+            .then("OMMISSION/MISREP SALE SECURITI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="OSUA")
+            .then("008-006-017(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing EPH7
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="EPH7")
+            .then("ILL PURCHASE EPHEDRINE-INDIVID")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="EPH7")
+            .then("020-002-190(C)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing POBM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="POBM")
+            .then("PORN INTENT TO DISSEMINATE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="POBM")
+            .then("13A-012-192(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HWL2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HWL2")
+            .then("HUNT-W/O NONRESIDENT LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HWL2")
+            .then("009-011-051(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FCPF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FCPF")
+            .then("FIREARM-PERSONS FORBIDDEN/POSS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FCPF")
+            .then("13A-011-072(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HNRL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HNRL")
+            .then("HUNT-LEND RESIDENT LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HNRL")
+            .then("009-011-051(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVAF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVAF")
+            .then("FELONY DV 3RD ASSAULT 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVAF")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
         ]
     )
-    charges = charges.join(aggch, on="CASENONUM")
-    charges = charges.fill_null("")
     charges = charges.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
```

### Comparing `alacorder-80.5.1/src/alacorder/alac.py` & `alacorder-80.5.3/src/alacorder/alac.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.1"
+version = "80.5.3"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -2274,15 +2274,15 @@
             pl.col("SEG_2")
             .str.extract(
                 r"(ALCOHOL|BOND|CONSERVATION|DOCKET|DRUG|GOVERNMENT|HEALTH|MUNICIPAL|OTHER|PERSONAL|PROPERTY|SEX|TRAFFIC)",
                 group_index=1,
             )
             .alias("Category"),
             pl.col("RAWDESC")
-            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP)")
+            .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
                 r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
@@ -2360,27 +2360,1787 @@
                 pl.col("CERVDisqConviction")
                 | pl.col("PardonDisqConviction")
                 | pl.col("PermanentDisqConviction")
             )
             .then((pl.col("TotalBalance") - pl.col("TotalD999")))
             .otherwise(None)
             .alias("PaymentToRestore"),
+            pl.col("RAWDESC").alias("Description"),
+            pl.col("RAWCITE").alias("Cite")
         ]
     )
-    aggch = charges.groupby("CASENONUM").agg("CaseNumber", "RAWCITE", "RAWDESC")
-    aggch = aggch.select(
+    charges = charges.fill_null("")
+        # fix missing PFI3
+    charges = charges.with_columns(
         [
-            pl.col("CASENONUM"),
-            pl.col("CaseNumber").arr.get(0).alias("CaseNumber"),
-            pl.col("RAWDESC").arr.get(0).alias("Description"),
-            pl.col("RAWCITE").arr.get(0).alias("Cite"),
+            pl.when(pl.col("Code")=="PFI3")
+            .then("POSSESS FORGED INSTRUMENT 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PFI3")
+            .then("13A-009-006.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing NWNI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="NWNI")
+            .then("NEGOTIATING WORTHLESS INST")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="NWNI")
+            .then("13A-009-013.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDR1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR1")
+            .then("USE/POSSESS DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR1")
+            .then("13A-012-260(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UPCS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UPCS")
+            .then("POSS. CONTR. SUBS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UPCS")
+            .then("13A-012-212(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FRCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FRCC")
+            .then("FRAUD USE CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FRCC")
+            .then("13A-012-212(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T003
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T003")
+            .then("NO DRIVERS LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T003")
+            .then("032-006-001(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PMIO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PMIO")
+            .then("PORN POSS MATERIAL MINORS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PMIO")
+            .then("13A-012-192(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UPCC")
+            .then("POSS CONTR SUBS INTENT DISTRIB")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UPCC")
+            .then("013-012-192(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BEMV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BEMV")
+            .then("BREAK/ENTER VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BEMV")
+            .then("13A-008-011(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HARA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HARA")
+            .then("HARASSMENT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HARA")
+            .then("13A-011-008(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TET3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TET3")
+            .then("THEFT OF PROPERTY 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TET3")
+            .then("13A-008-004.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T042
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T042")
+            .then("OVERWEIGHT TRUCK")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T042")
+            .then("032-009-020(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T707
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T707")
+            .then("FAIL DISPLAY INSURANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T707")
+            .then("032-07A-016(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SX12
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SX12")
+            .then("SEX ABUSE-CHILD LESS 12 YOA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SX12")
+            .then("13A-006-069.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRAK
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAK")
+            .then("TRAFFICKING-METHAMPHETAMINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAK")
+            .then("13A-012-231(11)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FCDC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FCDC")
+            .then("FRAUD USE CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FCDC")
+            .then("13A-009-014(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TOD3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOD3")
+            .then("THEFT/DECEPTION 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOD3")
+            .then("13A-008-004.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUV")
+            .then("UNAUTHORIZED USE VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUV")
+            .then("13A-008-011(A)1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T012
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T012")
+            .then("FAIL STOP SIGN")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T012")
+            .then("032-05A-112(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FR3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FR3D")
+            .then("FORGERY 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FR3D")
+            .then("13A-009-003.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HCOM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HCOM")
+            .then("HARASSING COMMUNICATIONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HCOM")
+            .then("13A-011-008(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TP3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TP3D")
+            .then("THEFT OF PROPERTY 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TP3D")
+            .then("13A-008-4.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VPCC")
+            .then("POSS CONTROLLED SUBST BY FRAUD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VPCC")
+            .then("13A-012-212(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FORF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FORF")
+            .then("BOND FORF-FELONY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T012")
+            .then("- -BOND FORT")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T527
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T527")
+            .then("DUI-CONTROLLED SUBSTANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T527")
+            .then("032-05A-191(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA3")
+            .then("BURGLARY 3RD (UNOCCUPIED BLDG)")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA3")
+            .then("13A-007-007(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FMUR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FMUR")
+            .then("FELONY MURDER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FMUR")
+            .then("13A-006-002(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MURR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MURR")
+            .then("MURDER-RECKLESS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MURR")
+            .then("13A-006-002(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FPCC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FPCC")
+            .then("ILL POSSESS CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FPCC")
+            .then("13A-009-014(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PREC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PREC")
+            .then("POSS/SELL PRECURSOR CHEMICALS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PREC")
+            .then("020-002-190(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing STSA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="STSA")
+            .then("SEXUAL TORTURE/ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="STSA")
+            .then("13A-006-065.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T582
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T582")
+            .then("EXPIRED LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T582")
+            .then("032-006-001(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM02
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM02")
+            .then("MURDER CAPITAL-ROBBERY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM02")
+            .then("13A-005-040(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDR4
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR4")
+            .then("PARAPHERNALIA - SELL/DELIVER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR4")
+            .then("13A-012-260(D)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VAPP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VAPP")
+            .then("POSSESS MARIHUANA 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VAPP")
+            .then("13A-012-213(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing MAN1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAN1")
+            .then("MANSLAUGHTER-RECKLESS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAN1")
+            .then("13A-006-003(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDR1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR1")
+            .then("USE/POSSESS DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR1")
+            .then("13A-012-260(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T755
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T755")
+            .then("NO/IMP TAG LIGHT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T755")
+            .then("032-005-240(C)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRAO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAO")
+            .then("TRAFFICKING-HEROIN")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAO")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FORM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FORM")
+            .then("BOND FORF-MISD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FORM")
+            .then("- -BOND FORT")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing SVIA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SVIA")
+            .then("SALVIA MISDEMEANOR POSSESSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SVIA")
+            .then("13A-012-214.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRAG
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRAG")
+            .then("TRAFFICKING-SYNTHETIC DRUGS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRAG")
+            .then("13A-012-231(12)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DSF1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DSF1")
+            .then("DISCHARGE GUN OCC BLDG/VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DSF1")
+            .then("13A-011-061(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing MISC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MISC")
+            .then("MISCELLANEOUS FILING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MISC")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA1")
+            .then("BURGLARY 3RD - DWELLING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA1")
+            .then("13A-007-007(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CEM1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CEM1")
+            .then("CHEMICAL ENDANGER MINOR")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CEM1")
+            .then("026-015-3.2(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM04
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM04")
+            .then("MURDER CAPITAL-BURGLARY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM04")
+            .then("13A-005-040(A)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing IPCD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="IPCD")
+            .then("ILL POSSESS CREDIT/DEBIT CARD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="IPCD")
+            .then("13A-009-014(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T005
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T005")
+            .then("UNDER INFLUENCE CONT. SUBSTANC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T005")
+            .then("032-05A-191(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T525
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T525")
+            .then("DUI: ANY SUB WHICH IMPAIRS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T525")
+            .then("032-05A-191(A)(5)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM15
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM15")
+            .then("MURDER CAPITAL-UNDER 14 YEARS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM15")
+            .then("13A-005-040(A)(15)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DUIF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DUIF")
+            .then("DUI - FELONY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DUIF")
+            .then("032-05A-191(A)&(H)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T169
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T169")
+            .then("SPEED/ 70+ MPH OR 65+ MPH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T169")
+            .then("032-05A-171(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DUIM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DUIM")
+            .then("DUI - MISD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DUIM")
+            .then("032-05A-191(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T718
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T718")
+            .then("DUI: UNDER INFLU ALCOHOL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T718")
+            .then("032-05A-191(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DVHF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVHF")
+            .then("FELONY DV 3RD HARRASSMENT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVHF")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TROP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TROP")
+            .then("TRAFFICKING-OPIUM")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TROP")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM10
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM10")
+            .then("MURDER CAPITAL-TWO OR MORE PER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM10")
+            .then("13A-005-040(A)(10)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM17
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM17")
+            .then("MURDER CAPITAL-VEH FR OUTSIDE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM17")
+            .then("13A-005-040(A)(17)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM01
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM01")
+            .then("MURDER CAPITAL-KIDNAP")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM01")
+            .then("13A-005-040(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDRU
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRU")
+            .then("TRAFFICKING-MORPHINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRU")
+            .then("13A-012-231(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T770
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T770")
+            .then("INOPERABLE BRAKE LIGHTS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T770")
+            .then("032-005-241(B)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing ACAL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ACAL")
+            .then("AGGRAVATED CHILD ABUSE < SIX")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ACAL")
+            .then("025-015-03.1(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDRY
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRY")
+            .then("TRAFFICKING-COCAINE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRY")
+            .then("13A-012-231(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRFT
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRFT")
+            .then("TRAFFICKING FENTANYL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRFT")
+            .then("13A-012-231(13)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FNLE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FNLE")
+            .then("GIVING FALSE NAME TO OFF")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FNLE")
+            .then("13A-009-018.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing RS3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="RS3D")
+            .then("REC STOLEN PROP 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="RS3D")
+            .then("13A-008-18.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T806
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T806")
+            .then("NO DRIVERS LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T806")
+            .then("032-006-018(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TOS3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOS3")
+            .then("THEFT OF SERVICES 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOS3")
+            .then("13A-008-010.3")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TSIB
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TSIB")
+            .then("TRAFFICKING STOLEN IDENTITIES")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TSIB")
+            .then("13A-008-193(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T011
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T011")
+            .then("DRIVING WRONG SIDE HWY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T011")
+            .then("032-05A-080(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VAPD
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VAPD")
+            .then("POSSESS MARIHUANA 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VAPD")
+            .then("13A-012-213(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T128
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRFT")
+            .then("NO TAG REGIS IN VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRFT")
+            .then("040-012-260(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing BHER
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BHER")
+            .then("BOND HEARING")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BHER")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing APPL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="APPL")
+            .then("CASE APPEALED ON")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="APPL")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MRDI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MRDI")
+            .then("MURDER - INTENTIONAL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MRDI")
+            .then("13A-006-002(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing UAUY
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="UAUY")
+            .then("UNAUTHORIZED USE VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="UAUY")
+            .then("13A-008-011(A)3")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T019
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T019")
+            .then("FAILURE TO DIM LIGHTS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T019")
+            .then("032-005-242(C)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T006
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T006")
+            .then("FAIL YIELD ROW")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T006")
+            .then("032-05A-112(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MAN2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAN2")
+            .then("MANSLAUGHTER-INTENT, PASSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAN2")
+            .then("13A-006-003(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM18
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM18")
+            .then("MURDER CAPITAL-FIRED FROM VEHI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM18")
+            .then("13A-005-040(A)(18)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing NUSE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="NUSE")
+            .then("NO USER PERMIT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="NUSE")
+            .then("033-015-007(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FBAP
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FBAP")
+            .then("FRAUD BY AUTHORIZED PERSONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FBAP")
+            .then("13A-009-014.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing VDRO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDRO")
+            .then("DRUG PARAPHERNALIA TO MINOR")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDRO")
+            .then("13A-012-260(E)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM16
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM16")
+            .then("MURDER CAPITAL-DWELL FR OUTSID")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM16")
+            .then("13A-005-040(A)(16)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing EDCO
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="EDCO")
+            .then("ENDG WELFARE CHILD-OCCUPATION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="EDCO")
+            .then("13A-013-006(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T096
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T096")
+            .then("MOVING TRAFFIC VIO")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T096")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing THBV
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="THBV")
+            .then("HOMICIDE BY VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="THBV")
+            .then("032-05A-190.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing ASTM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="ASTM")
+            .then("ALCOHOL-SALE/PERMIT UNDER AGE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="ASTM")
+            .then("028-03A-025(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SAVI
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SAVI")
+            .then("SALVIA FELONY POSSESSION")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SAVI")
+            .then("13A-012-214.1")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVFC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVFC")
+            .then("FELONY DV CRIM MISCHIEF 2D/3D")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVFC")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T128
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T128")
+            .then("NO TAG REGIS IN VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T128")
+            .then("040-012-260(B)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T071
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T071")
+            .then("COMBINED INFLUENCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T071")
+            .then("032-05A-191(A)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM07
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM07")
+            .then("MURDER CAPITAL-FOR HIRE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM07")
+            .then("13A-005-040(A)(7)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRBF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRBF")
+            .then("TR-FORT.")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRBF")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T813
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T813")
+            .then("MOVE OVER LAW")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T813")
+            .then("032-05A-058.2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CM03
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM03")
+            .then("MURDER CAPITAL-RAPE/SODOMY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM03")
+            .then("13A-005-040(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing TRMA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRMA")
+            .then("TRAFFICKING-MARIJUANA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRMA")
+            .then("13A-012-231(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T783
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T783")
+            .then("IMPEDING FLOW TRAFFIC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T783")
+            .then("032-05A-080(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T091
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T091")
+            .then("DUI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T091")
+            .then("032-05A-191(A)1/2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing T072
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T072")
+            .then("UNDER INFLU - ANY SUBSTANCE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T072")
+            .then("032-05A-191(A)5")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TOS2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TOS2")
+            .then("THEFT OF SERVICES 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TOS2")
+            .then("13A-008-010.2")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DV36
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DV36")
+            .then("FELONY DV CRIM MISCHIEF 2ND")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DV36")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing DSF2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DSF2")
+            .then("DISCHARGE GUN UNOCC BLDG/VEH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DSF2")
+            .then("13A-011-061(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing CM08
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CM08")
+            .then("MURDER CAPITAL-SEXUAL ABUSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CM08")
+            .then("13A-005-040(A)(8)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DOG1
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DOG1")
+            .then("DOG/CAT CRUELTY 1ST DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DOG1")
+            .then("13A-011-241(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CEM3
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CEM3")
+            .then("CHEMICAL ENDANGER MINOR/DEATH")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CEM3")
+            .then("026-015-3.2(A)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing PACS
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PACS")
+            .then("PROHIBITED ACTS-MAIN BLD/DWL")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PACS")
+            .then("020-002-071(A)(5)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T097
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T097")
+            .then("OTHER NON MOVING VIO")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T097")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )    
+    # fix missing VDR2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="VDR2")
+            .then("DEL/SALE DRUG PARAPHERNALIA")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="VDR2")
+            .then("13A-012-260(E)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing BRA2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="BRA2")
+            .then("BURGLARY 3RD - OCCUPIED BLDG")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="BRA2")
+            .then("13A-007-007(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVFC
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVFC")
+            .then("FELONY DV CRIM MISCHIEF 2D/3D")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVFC")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TS3D
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TS3D")
+            .then("THEFT OF SERVICES 3RD DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TS3D")
+            .then("13A-008-010.25")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing CODL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="CODL")
+            .then("CONTRIBUTING TO THE DELINQUENC")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="CODL")
+            .then("012-015-111(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HAR2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HAR2")
+            .then("HARASSMENT - THREAT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HAR2")
+            .then("13A-011-008(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T506
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T506")
+            .then("FAIL TO YIELD EMER VEHICLE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T506")
+            .then("032-05A-115(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HGAR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HGAR")
+            .then("FAILURE TO COMPLY - GARBAGE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HGAR")
+            .then("022-027-003(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing TRCN
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="TRCN")
+            .then("TR-CONTEMPT")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="TRCN")
+            .then("")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T773
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T773")
+            .then("IMP TAIL LIGHTS-TRAILER")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T773")
+            .then("032-005-240(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PCUR
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PCUR")
+            .then("FAIL CPLY REPORTS-PRECUR CHEMS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PCUR")
+            .then("020-002-190(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PPRE
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PPRE")
+            .then("POSS OF PRE-CURSOR CHEMICALS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PPRE")
+            .then("020-002-181(D)(13)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T507
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T507")
+            .then("FAIL TO YIELD RIGHT OF WAY")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T507")
+            .then("032-05A-082(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing T081
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="T081")
+            .then("NO HDLGTS WHEN REQUIRED")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="T081")
+            .then("032-005-240(A)(1)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PARA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PARA")
+            .then("FAILURE COMPLY PARK CONDITIONS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PARA")
+            .then("220-005-013(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing MAAL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="MAAL")
+            .then("ALCOHOL- MINOR/POSS/CONSUME")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="MAAL")
+            .then("028-03A-025(A)(18)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing PCAB
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="PCAB")
+            .then("POSS/CONT ALCOHOL-STATE PARK")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="PCAB")
+            .then("220-005-016(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DOG2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DOG2")
+            .then("DOG/CAT CRUELTY 2ND DEGREE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DOG2")
+            .then("13A-011-241(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing SFUF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="SFUF")
+            .then("SETTING FIRE-UNCL FOREST/WOOD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="SFUF")
+            .then("009-013-011(B)(3)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing OSUA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="OSUA")
+            .then("OMMISSION/MISREP SALE SECURITI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="OSUA")
+            .then("008-006-017(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing OSUA
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="OSUA")
+            .then("OMMISSION/MISREP SALE SECURITI")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="OSUA")
+            .then("008-006-017(A)(2)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing EPH7
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="EPH7")
+            .then("ILL PURCHASE EPHEDRINE-INDIVID")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="EPH7")
+            .then("020-002-190(C)(4)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing POBM
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="POBM")
+            .then("PORN INTENT TO DISSEMINATE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="POBM")
+            .then("13A-012-192(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HWL2
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HWL2")
+            .then("HUNT-W/O NONRESIDENT LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HWL2")
+            .then("009-011-051(C)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing FCPF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="FCPF")
+            .then("FIREARM-PERSONS FORBIDDEN/POSS")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="FCPF")
+            .then("13A-011-072(A)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing HNRL
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="HNRL")
+            .then("HUNT-LEND RESIDENT LICENSE")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="HNRL")
+            .then("009-011-051(B)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
+        ]
+    )
+    # fix missing DVAF
+    charges = charges.with_columns(
+        [
+            pl.when(pl.col("Code")=="DVAF")
+            .then("FELONY DV 3RD ASSAULT 3RD")
+            .otherwise(pl.col("Description"))
+            .alias("Description"),
+            pl.when(pl.col("Code")=="DVAF")
+            .then("13A-006-132(D)")
+            .otherwise(pl.col("Cite"))
+            .alias("Cite")
         ]
     )
-    charges = charges.join(aggch, on="CASENONUM")
-    charges = charges.fill_null("")
     charges = charges.with_columns(
         [
             pl.concat_str(
                 [
                     pl.col("CaseNumber"),
                     pl.lit(" - "),
                     pl.col("Num"),
```

### Comparing `alacorder-80.5.1/PKG-INFO` & `alacorder-80.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.5.1
+Version: 80.5.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

