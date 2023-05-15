# Comparing `tmp/tsp-1.4.9-py3-none-any.whl.zip` & `tmp/tsp-1.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,88 @@
-Zip file size: 1522692 bytes, number of entries: 55
--rw-r--r--  2.0 unx      368 b- defN 23-Jan-31 16:27 tsp/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 23-Jan-31 16:28 tsp/__meta__.py
--rw-r--r--  2.0 unx    30354 b- defN 23-Jan-31 16:27 tsp/core.py
--rw-r--r--  2.0 unx     3991 b- defN 23-Jan-31 16:27 tsp/gtnp.py
--rw-r--r--  2.0 unx      107 b- defN 23-Jan-31 16:27 tsp/misc.py
--rw-r--r--  2.0 unx     2877 b- defN 23-Jan-31 16:27 tsp/physics.py
--rw-r--r--  2.0 unx    16726 b- defN 23-Jan-31 16:27 tsp/readers.py
--rw-r--r--  2.0 unx     1379 b- defN 23-Jan-31 16:27 tsp/time.py
--rw-r--r--  2.0 unx     2956 b- defN 23-Jan-31 16:27 tsp/utils.py
--rw-rw-rw-  2.0 unx      171 b- defN 23-Jan-31 16:27 tsp/data/2023-01-06_755-test-Dataset_2031-Constant_Over_Interval-Hourly-Ground_Temperature-Thermistor_Automated.timeserie.csv
--rw-rw-rw-  2.0 unx     5686 b- defN 23-Jan-31 16:27 tsp/data/2023-01-06_755-test.metadata.txt
--rw-rw-rw-  2.0 unx   262289 b- defN 23-Jan-31 16:27 tsp/data/example_geotop.csv
--rw-rw-rw-  2.0 unx   191812 b- defN 23-Jan-31 16:27 tsp/data/example_gtnp.csv
--rw-r--r--  2.0 unx     1777 b- defN 23-Jan-31 16:27 tsp/dataloggers/AbstractReader.py
--rw-r--r--  2.0 unx     2947 b- defN 23-Jan-31 16:27 tsp/dataloggers/FG2.py
--rw-r--r--  2.0 unx     2975 b- defN 23-Jan-31 16:27 tsp/dataloggers/GP5W.py
--rw-r--r--  2.0 unx      916 b- defN 23-Jan-31 16:27 tsp/dataloggers/Geoprecision.py
--rw-r--r--  2.0 unx    33472 b- defN 23-Jan-31 16:27 tsp/dataloggers/HOBO.py
--rw-r--r--  2.0 unx      410 b- defN 23-Jan-31 16:27 tsp/dataloggers/__init__.py
--rw-r--r--  2.0 unx     2665 b- defN 23-Jan-31 16:27 tsp/dataloggers/logr.py
--rw-rw-rw-  2.0 unx   648322 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/FG2_399.csv
--rw-rw-rw-  2.0 unx    36948 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/GP5W.csv
--rw-rw-rw-  2.0 unx    68696 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/GP5W_260.csv
--rw-rw-rw-  2.0 unx   147550 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/GP5W_270.csv
--rw-rw-rw-  2.0 unx    37920 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/H08-030-08_HOBOware.csv
--rw-rw-rw-  2.0 unx    82735 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/RBR_01.dat
--rw-rw-rw-  2.0 unx   242142 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/RBR_02.dat
--rw-rw-rw-  2.0 unx   470085 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/RSTDT2055.csv
--rw-rw-rw-  2.0 unx    55854 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/U23-001_HOBOware.csv
--rw-rw-rw-  2.0 unx   247057 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-negative-2.txt
--rw-rw-rw-  2.0 unx   221034 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-negative-3.txt
--rw-rw-rw-  2.0 unx    36089 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-positive-number-1.txt
--rw-rw-rw-  2.0 unx    38331 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-positive-number-2.csv
--rw-rw-rw-  2.0 unx    47776 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-positive-number-3.csv
--rw-rw-rw-  2.0 unx    53444 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo-positive-number-4.csv
--rw-rw-rw-  2.0 unx   531384 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo2.csv
--rw-rw-rw-  2.0 unx      408 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB.config.json
--rw-rw-rw-  2.0 unx   958834 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB.csv
--rw-rw-rw-  2.0 unx     4333 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_Details.txt
--rw-rw-rw-  2.0 unx   168846 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_classic.csv
--rw-rw-rw-  2.0 unx   987910 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_defaults.csv
--rw-rw-rw-  2.0 unx    48977 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_minimal.txt
--rw-rw-rw-  2.0 unx    65536 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_raw.hobo
--rw-rw-rw-  2.0 unx   142070 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_var2.csv
--rw-rw-rw-  2.0 unx    92381 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/hobo_1_AB_var3.csv
--rw-rw-rw-  2.0 unx    21966 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/logR_ULogC16-32_1.csv
--rw-rw-rw-  2.0 unx    19066 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/logR_ULogC16-32_2.csv
--rw-rw-rw-  2.0 unx   734009 b- defN 23-Jan-31 16:27 tsp/dataloggers/test_files/mon_3_Ta_2010-08-18_2013-02-08.txt
--rw-r--r--  2.0 unx       71 b- defN 23-Jan-31 16:27 tsp/plots/__init__.py
--rw-r--r--  2.0 unx     9448 b- defN 23-Jan-31 16:27 tsp/plots/static.py
--rw-rw-rw-  2.0 unx    35149 b- defN 23-Jan-31 16:28 tsp-1.4.9.dist-info/LICENSE
--rw-r--r--  2.0 unx     2731 b- defN 23-Jan-31 16:28 tsp-1.4.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-31 16:28 tsp-1.4.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       30 b- defN 23-Jan-31 16:28 tsp-1.4.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     5081 b- defN 23-Jan-31 16:28 tsp-1.4.9.dist-info/RECORD
-55 files, 6826276 bytes uncompressed, 1514554 bytes compressed:  77.8%
+Zip file size: 3035565 bytes, number of entries: 86
+-rw-r--r--  2.0 unx      380 b- defN 23-May-15 21:38 tsp/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 23-May-15 21:38 tsp/__meta__.py
+-rw-r--r--  2.0 unx    30720 b- defN 23-May-15 21:38 tsp/core.py
+-rw-r--r--  2.0 unx     3991 b- defN 23-May-15 21:38 tsp/gtnp.py
+-rw-r--r--  2.0 unx      107 b- defN 23-May-15 21:38 tsp/misc.py
+-rw-r--r--  2.0 unx     2699 b- defN 23-May-15 21:38 tsp/physics.py
+-rw-r--r--  2.0 unx    18520 b- defN 23-May-15 21:38 tsp/readers.py
+-rw-r--r--  2.0 unx     1379 b- defN 23-May-15 21:38 tsp/time.py
+-rw-r--r--  2.0 unx     2932 b- defN 23-May-15 21:38 tsp/utils.py
+-rw-rw-rw-  2.0 unx      171 b- defN 23-May-15 21:38 tsp/data/2023-01-06_755-test-Dataset_2031-Constant_Over_Interval-Hourly-Ground_Temperature-Thermistor_Automated.timeserie.csv
+-rw-rw-rw-  2.0 unx     5686 b- defN 23-May-15 21:38 tsp/data/2023-01-06_755-test.metadata.txt
+-rw-rw-rw-  2.0 unx   262289 b- defN 23-May-15 21:38 tsp/data/example_geotop.csv
+-rw-rw-rw-  2.0 unx   191812 b- defN 23-May-15 21:38 tsp/data/example_gtnp.csv
+-rw-r--r--  2.0 unx     1777 b- defN 23-May-15 21:38 tsp/dataloggers/AbstractReader.py
+-rw-r--r--  2.0 unx     3281 b- defN 23-May-15 21:38 tsp/dataloggers/FG2.py
+-rw-r--r--  2.0 unx     3312 b- defN 23-May-15 21:38 tsp/dataloggers/GP5W.py
+-rw-r--r--  2.0 unx      916 b- defN 23-May-15 21:38 tsp/dataloggers/Geoprecision.py
+-rw-r--r--  2.0 unx    33472 b- defN 23-May-15 21:38 tsp/dataloggers/HOBO.py
+-rw-r--r--  2.0 unx     8538 b- defN 23-May-15 21:38 tsp/dataloggers/RBRXL800.py
+-rw-r--r--  2.0 unx    13908 b- defN 23-May-15 21:38 tsp/dataloggers/RBRXR420.py
+-rw-r--r--  2.0 unx      410 b- defN 23-May-15 21:38 tsp/dataloggers/__init__.py
+-rw-r--r--  2.0 unx     2665 b- defN 23-May-15 21:38 tsp/dataloggers/logr.py
+-rw-rw-rw-  2.0 unx   201018 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/004448.DAT
+-rw-rw-rw-  2.0 unx   331292 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/004531.DAT
+-rw-rw-rw-  2.0 unx   118535 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/004531.HEX
+-rw-rw-rw-  2.0 unx   118531 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/004534.HEX
+-rw-rw-rw-  2.0 unx   171935 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/010252.dat
+-rw-rw-rw-  2.0 unx    84712 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/010252.hex
+-rw-rw-rw-  2.0 unx    62720 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/010274.hex
+-rw-rw-rw-  2.0 unx   173117 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/010278.hex
+-rw-rw-rw-  2.0 unx   127062 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/012064.dat
+-rw-rw-rw-  2.0 unx    62921 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/012064.hex
+-rw-rw-rw-  2.0 unx   172576 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/012081.hex
+-rw-rw-rw-  2.0 unx  1007616 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/062834_20220904_2351.rsk
+-rw-rw-rw-  2.0 unx   308908 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/062834_20220904_2351.xlsx
+-rw-rw-rw-  2.0 unx   107655 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/07B1592.DAT
+-rw-rw-rw-  2.0 unx    59683 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/07B1592.HEX
+-rw-rw-rw-  2.0 unx   162502 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/07B4450.DAT
+-rw-rw-rw-  2.0 unx    84576 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/07B4450.HEX
+-rw-rw-rw-  2.0 unx   648322 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/FG2_399.csv
+-rw-rw-rw-  2.0 unx    36948 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/GP5W.csv
+-rw-rw-rw-  2.0 unx    68696 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/GP5W_260.csv
+-rw-rw-rw-  2.0 unx   147550 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/GP5W_270.csv
+-rw-rw-rw-  2.0 unx    37920 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/H08-030-08_HOBOware.csv
+-rw-rw-rw-  2.0 unx    82735 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/RBR_01.dat
+-rw-rw-rw-  2.0 unx   242142 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/RBR_02.dat
+-rw-rw-rw-  2.0 unx   470085 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/RSTDT2055.csv
+-rw-rw-rw-  2.0 unx    55854 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/U23-001_HOBOware.csv
+-rw-rw-rw-  2.0 unx   247057 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-negative-2.txt
+-rw-rw-rw-  2.0 unx   221034 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-negative-3.txt
+-rw-rw-rw-  2.0 unx    36089 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-positive-number-1.txt
+-rw-rw-rw-  2.0 unx    38331 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-positive-number-2.csv
+-rw-rw-rw-  2.0 unx    47776 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-positive-number-3.csv
+-rw-rw-rw-  2.0 unx    53444 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo-positive-number-4.csv
+-rw-rw-rw-  2.0 unx   531384 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo2.csv
+-rw-rw-rw-  2.0 unx      408 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB.config.json
+-rw-rw-rw-  2.0 unx   958834 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB.csv
+-rw-rw-rw-  2.0 unx     4333 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_Details.txt
+-rw-rw-rw-  2.0 unx   168846 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_classic.csv
+-rw-rw-rw-  2.0 unx   987910 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_defaults.csv
+-rw-rw-rw-  2.0 unx    48977 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_minimal.txt
+-rw-rw-rw-  2.0 unx    65536 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_raw.hobo
+-rw-rw-rw-  2.0 unx   142070 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_var2.csv
+-rw-rw-rw-  2.0 unx    92381 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/hobo_1_AB_var3.csv
+-rw-rw-rw-  2.0 unx    21966 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/logR_ULogC16-32_1.csv
+-rw-rw-rw-  2.0 unx    19066 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/logR_ULogC16-32_2.csv
+-rw-rw-rw-  2.0 unx   734009 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/mon_3_Ta_2010-08-18_2013-02-08.txt
+-rw-rw-rw-  2.0 unx   111570 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_001.dat
+-rw-rw-rw-  2.0 unx    55293 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_001.hex
+-rw-rw-rw-  2.0 unx   111547 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_001_no_comment.dat
+-rw-rw-rw-  2.0 unx    55270 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_001_no_comment.hex
+-rw-rw-rw-  2.0 unx    93525 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_002.dat
+-rw-rw-rw-  2.0 unx    57536 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_002.hex
+-rw-rw-rw-  2.0 unx    62703 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_003.hex
+-rw-rw-rw-  2.0 unx   263680 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_003.xls
+-rw-rw-rw-  2.0 unx    80057 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_xl_001.DAT
+-rw-rw-rw-  2.0 unx    81601 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_xl_002.DAT
+-rw-rw-rw-  2.0 unx   221656 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_xl_003.DAT
+-rw-rw-rw-  2.0 unx   118459 b- defN 23-May-15 21:38 tsp/dataloggers/test_files/rbr_xl_003.HEX
+-rw-r--r--  2.0 unx       71 b- defN 23-May-15 21:38 tsp/plots/__init__.py
+-rw-r--r--  2.0 unx     9448 b- defN 23-May-15 21:38 tsp/plots/static.py
+-rw-rw-rw-  2.0 unx    35149 b- defN 23-May-15 21:38 tsp-1.5.3.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2835 b- defN 23-May-15 21:38 tsp-1.5.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-15 21:38 tsp-1.5.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       30 b- defN 23-May-15 21:38 tsp-1.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     8102 b- defN 23-May-15 21:38 tsp-1.5.3.dist-info/RECORD
+86 files, 11522744 bytes uncompressed, 3022659 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -48,20 +48,77 @@
 
 Filename: tsp/dataloggers/Geoprecision.py
 Comment: 
 
 Filename: tsp/dataloggers/HOBO.py
 Comment: 
 
+Filename: tsp/dataloggers/RBRXL800.py
+Comment: 
+
+Filename: tsp/dataloggers/RBRXR420.py
+Comment: 
+
 Filename: tsp/dataloggers/__init__.py
 Comment: 
 
 Filename: tsp/dataloggers/logr.py
 Comment: 
 
+Filename: tsp/dataloggers/test_files/004448.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/004531.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/004531.HEX
+Comment: 
+
+Filename: tsp/dataloggers/test_files/004534.HEX
+Comment: 
+
+Filename: tsp/dataloggers/test_files/010252.dat
+Comment: 
+
+Filename: tsp/dataloggers/test_files/010252.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/010274.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/010278.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/012064.dat
+Comment: 
+
+Filename: tsp/dataloggers/test_files/012064.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/012081.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/062834_20220904_2351.rsk
+Comment: 
+
+Filename: tsp/dataloggers/test_files/062834_20220904_2351.xlsx
+Comment: 
+
+Filename: tsp/dataloggers/test_files/07B1592.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/07B1592.HEX
+Comment: 
+
+Filename: tsp/dataloggers/test_files/07B4450.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/07B4450.HEX
+Comment: 
+
 Filename: tsp/dataloggers/test_files/FG2_399.csv
 Comment: 
 
 Filename: tsp/dataloggers/test_files/GP5W.csv
 Comment: 
 
 Filename: tsp/dataloggers/test_files/GP5W_260.csv
@@ -138,29 +195,65 @@
 
 Filename: tsp/dataloggers/test_files/logR_ULogC16-32_2.csv
 Comment: 
 
 Filename: tsp/dataloggers/test_files/mon_3_Ta_2010-08-18_2013-02-08.txt
 Comment: 
 
+Filename: tsp/dataloggers/test_files/rbr_001.dat
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_001.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_001_no_comment.dat
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_001_no_comment.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_002.dat
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_002.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_003.hex
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_003.xls
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_xl_001.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_xl_002.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_xl_003.DAT
+Comment: 
+
+Filename: tsp/dataloggers/test_files/rbr_xl_003.HEX
+Comment: 
+
 Filename: tsp/plots/__init__.py
 Comment: 
 
 Filename: tsp/plots/static.py
 Comment: 
 
-Filename: tsp-1.4.9.dist-info/LICENSE
+Filename: tsp-1.5.3.dist-info/LICENSE
 Comment: 
 
-Filename: tsp-1.4.9.dist-info/METADATA
+Filename: tsp-1.5.3.dist-info/METADATA
 Comment: 
 
-Filename: tsp-1.4.9.dist-info/WHEEL
+Filename: tsp-1.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: tsp-1.4.9.dist-info/top_level.txt
+Filename: tsp-1.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: tsp-1.4.9.dist-info/RECORD
+Filename: tsp-1.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tsp/__init__.py

```diff
@@ -1,9 +1,10 @@
 from tsp.core import TSP, IndexedTSP
 from tsp.misc import _is_depth_column
+
 from tsp.plots.static import trumpet_curve, time_series, colour_contour
-from tsp.readers import read_gtnp, read_geotop, read_geoprecision, read_hoboware, read_ntgs, read_logr, read_csv
+from tsp.readers import read_gtnp, read_geotop, read_geoprecision, read_hoboware, read_ntgs, read_logr, read_csv, read_rbr
 from tsp.utils import resolve_duplicate_times
 
 #TSP.__module__ = "teaspoon"
 
-__all__ = ["TSP", "IndexedTSP"]
+__all__ = ["TSP", "IndexedTSP"]
```

## tsp/__meta__.py

```diff
@@ -1,3 +1,3 @@
 # Automatically created. Please do not edit.
-__version__ = '1.4.9'
+__version__ = '1.5.3'
 __author__ = 'Nick Brown'
```

## tsp/core.py

```diff
@@ -8,18 +8,18 @@
 
 try:
     import netCDF4 as nc
 
     try:
         from pfit.pfnet_standard import make_temperature_base
     except ModuleNotFoundError:
-        warnings.warn("Missing pfit library. Some functionality will be limited.")
+        warnings.warn("Missing pfit library. Some functionality will be limited.", stacklevel=2)
 
 except ModuleNotFoundError:
-    warnings.warn("Missing netCDF4 library. Some functionality will be limited.")
+    warnings.warn("Missing netCDF4 library. Some functionality will be limited.", stacklevel=2)
 
 from typing import Union, Optional
 from datetime import datetime, tzinfo, timezone, timedelta
 
 import tsp
 from tsp.physics import analytical_fourier
 from tsp.plots.static import trumpet_curve, colour_contour, time_series
@@ -77,15 +77,15 @@
                  latitude: Optional[float]=None, 
                  longitude: Optional[float]=None,
                  site_id: Optional[str]=None,
                  metadata: dict={}):
 
         self._times = handle_incoming_times(times)
         if self._times.duplicated().any():
-            warnings.warn(f"Duplicate timestamps found: {self._times[np.where(self._times.duplicated())[0]]}. That's bad.")
+            warnings.warn(f"Duplicate timestamps found: {self._times[np.where(self._times.duplicated())[0]]}. That's bad.", stacklevel=2)
         
         if self.utc_offset:
             self._output_utc_offset = self.utc_offset
         else:
             self._output_utc_offset = None
         
         self._depths = np.atleast_1d(depths)
@@ -299,15 +299,15 @@
         index = data['time'].dt.strftime(freq_fmt)
         grouped = data.groupby([index, "depth"])
 
         # calculate data
         agg_avg = grouped['temperature_in_ground'].mean().unstack()
         agg_counts = grouped['number_of_observations'].sum().unstack() 
         times = pd.to_datetime(agg_avg.index, format=freq_fmt)
-        
+
         # apply masks
         count_mask = _observation_count_mask(number_of_observations=agg_counts,
                                              min_count=min_count)
         interval_mask = _temporal_gap_mask(grouped, max_gap, min_span)
         mask = np.logical_or(count_mask, interval_mask)
         values = np.ma.masked_array(agg_avg, mask=mask)
 
@@ -439,14 +439,21 @@
             Minimum total data range (in seconds) to be consiered a valid average, defaults to 64800 (18 hours)
         
         Returns
         -------
         TSP
             A TSP object with data aggregated to daily averages
         """
+        # if the data is already daily +/- 1min , just return it
+        if np.all(np.isclose(np.diff(self.times).astype('float64'), 
+                            8.64e13,
+                            atol=8.64e13 / (24 * 60 ))):
+            
+            return self
+        
         t = self.__nly(freq_fmt="%Y%m%d", 
                          min_count=min_count,
                          max_gap=max_gap,
                          min_span=min_span)
         
         return t
 
@@ -583,15 +590,15 @@
         df.to_csv(filename, index=False)
 
     def to_netcdf(self, file: str) -> None:
         """  Write the data as a netcdf"""
         try:
             ncf = make_temperature_base(file, len(self.depths))
         except NameError:
-            warnings.warn("Missing required packages. Try installing with `pip install tsp[nc]`")
+            warnings.warn("Missing required packages. Try installing with `pip install tsp[nc]`", stacklevel=2)
             return
         
         with nc.Dataset(ncf, 'a') as ncd:
             pytime = self.times.to_pydatetime()
 
             ncd['depth_below_ground_surface'][:] = self.depths
 
@@ -606,15 +613,15 @@
             if self.site_id:
                 ncd['site_name'] = self.site_id
             
             for key, value in self.metadata:
                 try:
                     ncd.setncattr(key, value)
                 except Exception:
-                    warnings.warn(f"Could not set metadata item: {key}")
+                    warnings.warn(f"Could not set metadata item: {key}", stacklevel=2)
 
     def to_json(self, file: str) -> None:
         """ Write the data to a serialized json file """
         with open(file, 'w') as f:
             f.write(self._to_json())
 
     def _to_json(self) -> str:
@@ -766,15 +773,15 @@
         """Depth indices 
 
         Returns
         -------
         numpy.ndarray
             An array of depth indices
         """
-        warnings.warn("This TSP uses indices (1,2,3,...) instad of depths. Use set_depths() to use measured depths.")
+        warnings.warn("This TSP uses indices (1,2,3,...) instad of depths. Use set_depths() to use measured depths.", stacklevel=2)
         return self._depths
 
     @depths.setter
     def depths(self, value):
         TSP.depths.__set__(self, value)
 
     def set_depths(self, depths: np.ndarray):
@@ -804,15 +811,15 @@
         minimum data range (beginning to end) in seconds. 
 
     Returns
     -------
     numpy.ndarray
         boolean array with ``True`` where measurement spacing or range in group does not satisfy tolerances
     """    
-    max_diff = grouped.time.apply(np.diff).apply(lambda x: np.max(x, initial=0)).apply(lambda x: x.total_seconds())
+    max_diff = grouped.time.apply(np.diff).apply(lambda x: np.max(x, initial=np.timedelta64(0))).apply(lambda x: x.total_seconds())
     max_diff = max_diff.unstack().to_numpy()
     diff_mask = np.where((max_diff == 0) | (max_diff >= max_gap), True, False)
     
     total_span = grouped.time.apply(np.ptp).apply(lambda x: x.total_seconds()).unstack().to_numpy()
     span_mask = np.where(total_span < min_span, True, False)
 
     mask = diff_mask * span_mask
```

## tsp/physics.py

```diff
@@ -1,17 +1,17 @@
 import numpy as np
 from typing import Optional
 
 
 def analytical_fourier(depths: "np.ndarray", times: "np.ndarray",
-              Q:"Optional[float]"=0.2, 
-              c:"Optional[float]"=1.6e6,
-              k:"Optional[float]"=2.5,
-              A:"Optional[float]"=6,
-              MAGST:"Optional[float]"=-0.5) -> "np.ndarray":
+              Q:float=0.2, 
+              c:float=1.6e6,
+              k:float=2.5,
+              A:float=6,
+              MAGST:float=-0.5) -> "np.ndarray":
     """Create sinusoidal synthetic data for examples and testing
 
     Parameters
     ----------
     depths : np.ndarray
         array of depths in m
     times : np.ndarray
@@ -28,21 +28,16 @@
         mean annual ground surface temperature [C], by default -0.5
 
     Returns
     -------
     TSP
         _description_
     """
-    Q = 0.2  # [W m-2]
-    c = 1.6e6  # J m-3 K-1
-    k = 2.5  # [W m-1 K-1]
     tau = 31536000  # [s]
     w = 2 * np.pi / tau  # []
-    A = 6  # [C]
-    MAGST = -0.5  # [C]
     alpha = k / c
 
     initial = initial_analytic(MAGST, Q, k, depths) 
     initial = np.repeat(initial[np.newaxis, :], len(times), axis=0) 
     
     T = initial + delta_analytic(A0=A, z=depths, w=w, alpha=alpha, t=times)
```

## tsp/readers.py

```diff
@@ -11,14 +11,16 @@
 
 from pathlib import Path
 from typing import Union, Optional
 
 from tsp.dataloggers.Geoprecision import detect_geoprecision_type
 from tsp.dataloggers.HOBO import HOBO, HOBOProperties
 from tsp.dataloggers.logr import LogR, guessed_depths_ok
+from tsp.dataloggers.RBRXL800 import RBRXL800
+from tsp.dataloggers.RBRXR420 import RBRXR420
 
 from tsp.core import TSP, IndexedTSP
 from tsp.misc import _is_depth_column
 from tsp.gtnp import GtnpMetadata
 
 def read_csv(filepath: str,
               datecol: "Union[str, int]",
@@ -157,15 +159,29 @@
                    na_values=[-9999.0],
                    datecol="^(Date.*)",
                    datefmt=r"%d/%m/%Y %H:%M",
                    depth_pattern=r"^(-?[0-9\.]+)$")
     
     t._depths *= 0.001  # Convert to [m]
 
-    return t
+    # Only use last simulation period 
+    # TODO: this could be improved
+    raw = pd.read_csv(file)
+    last_run = np.logical_and(raw['Simulation_Period'] == max( raw['Simulation_Period'] ),
+               raw['Run'] == max( raw['Run'] ))
+    
+    last = TSP(times = t.times[last_run],
+               depths = t.depths,
+               values = t.values[last_run, :],
+               metadata={"Simulation_Period": max(raw['Simulation_Period']),
+                         "Run": max( raw['Run'] )
+                         }
+    )
+
+    return last
 
 
 def read_gtpem(file: str) -> "list[TSP]":
     output = list()
     try:
         with nc.Dataset(file) as ncdf:
             n_sim = len(ncdf['geotop']['sitename'][:])
@@ -339,24 +355,25 @@
         Path to file.
 
     Returns
     -------
     IndexedTSP
         An IndexedTSP
     """
-    reader = detect_geoprecision_type(filepath)
+    Reader = detect_geoprecision_type(filepath)
     
-    if reader is None:
+    if Reader is None:
         raise RuntimeError("Could not detect type of geoprecision file (GP5W or FG2 missing from header")
-
-    data = reader().read(filepath)
-
+    reader = Reader()
+    
+    data = reader.read(filepath)
     t = IndexedTSP(times=data['TIME'].dt.to_pydatetime(),
                      values=data.drop("TIME", axis=1).values)
 
+    t.metadata = reader.META
     return t
 
 
 def read_logr(filepath: str) -> "Union[IndexedTSP,TSP]":
     """Read a LogR datalogger export (text file)
 
     Reads LogR ULogC16-32 files.
@@ -472,7 +489,48 @@
 
     t = IndexedTSP(times=time, values=temp, latitude=lat, longitude=lon)
     
     if init_file:
         t.set_depths(depths)
 
     return t
+
+
+def read_rbr(file_path: str) -> IndexedTSP:
+    """
+
+    Parameters
+    ----------
+    filepath
+
+    Returns
+    -------
+
+    """
+    file_extention = Path(file_path).suffix.lower()
+    if file_extention in [".dat", ".hex"]:
+        with open(file_path, "r") as f:
+            first_line = f.readline()
+            model = first_line.split()[1]
+            if model == "XL-800":
+                r = RBRXL800()
+            elif model in ["XR-420", "XR-420-T8"]:
+                r = RBRXR420()
+            else:
+                raise ValueError(f"logger model {model} unsupported")
+            data = r.read(file_path)
+    elif file_extention in [".xls", ".xlsx", ".rsk"]:
+        r = RBRXR420()
+        data = r.read(file_path)
+    else:
+        raise IOError("File is not .dat, .hex, .xls, .xlsx, or .rsk")
+
+    times = data['TIME'].dt.to_pydatetime()
+    channels = pd.Series(data.columns).str.match("^ch")
+    values = data.loc[:, channels.to_numpy()]
+
+    t = IndexedTSP(times=times, values=values.values)
+    if "utc offset" in list(r.META.keys()):
+        t.set_utc_offset(r.META["utc offset"])
+
+    return t
+
```

## tsp/utils.py

```diff
@@ -81,15 +81,15 @@
     
     return t_new
 
 
 def _average_duplicate_time(t: TSP):
     singleton = t.wide[~t.wide.index.duplicated(keep=False)]
     duplicated = t.wide[t.wide.index.duplicated(keep=False)].drop(['time'], axis=1).reset_index()
-    averaged = duplicated.groupby(duplicated['index']).apply(lambda x: x[~x.isna()].mean())  # TODO: replace with newer pandas .mean()
+    averaged = duplicated.groupby(duplicated['index']).apply(lambda x: x[~x.isna()].mean(numeric_only=True))  
     averaged.insert(0, 'time',averaged.index)
 
     df = pd.concat([singleton, averaged], ignore_index=False).sort_index()
 
     time = df.index
     values = df.drop(['time'], axis=1).values
     depths = df.drop(['time'], axis=1).columns
```

## tsp/dataloggers/FG2.py

```diff
@@ -71,14 +71,16 @@
                 warnings.warn("Could not successfully convert all data to numeric. Some data may be missing")
                 self.DATA[col] = pd.to_numeric(self.DATA[col], errors='coerce')
 
         self.DATA["TIME"] = pd.to_datetime(self.DATA["TIME"], format=self.DATEFMT)
         self.DATA = self.DATA.drop(["NO"], axis=1)
         self.DATA = self.drop_hk(self.DATA)
 
+        self.META.update(parse_fg2_meta_lines(self.META['raw']))
+
         return self.DATA
 
     def _is_metadata(self, line) -> bool:
         match = re.search("^<.*>$", line)
         return bool(match)
 
     def _is_observation(self, line: str) -> bool:
@@ -92,7 +94,18 @@
     def _is_hk(self, name: str) -> bool:
         if self.HK.match(name):
             return True
         return False
 
     def drop_hk(self, df: "pd.DataFrame") -> "pd.DataFrame":
         return df.drop([c for c in df if self._is_hk(c)], axis=1)
+
+
+def parse_fg2_meta_lines(meta: "list[str]") -> dict:
+    parsed = dict()
+    serial = re.compile(r"LOGGER: \$([\w]{6})")
+
+    for line in meta:
+        if serial.match(line):
+            parsed["logger_serial_number"] = serial.match(line).group(1)
+
+    return parsed
```

## tsp/dataloggers/GP5W.py

```diff
@@ -79,14 +79,16 @@
 
         self.DATA["Time"] = pd.to_datetime(self.DATA["Time"], format=self.DATEFMT)
         self.DATA.rename(columns={"Time":"TIME"}, inplace=True)
 
         self.DATA = self.DATA.drop(["No"], axis=1)
         self.DATA = self.drop_hk(self.DATA)
 
+        self.META.update(parse_gp5w_meta_lines(self.META['raw']))
+
         return self.DATA
 
     def _is_observation(self, line: str) -> bool:
         match = re.search(r"\d*,\d{2}\.\d{2}\.\d{4}", line)
         return bool(match)
 
     def __is_header(self, line: str) -> bool:
@@ -95,8 +97,19 @@
 
     def _is_hk(self, name: str) -> bool:
         if self.HK.match(name):
             return True
         return False
 
     def drop_hk(self, df: "pd.DataFrame") -> "pd.DataFrame":
-        return df.drop([c for c in df if self._is_hk(c)], axis=1)
+        return df.drop([c for c in df if self._is_hk(c)], axis=1)
+
+
+def parse_gp5w_meta_lines(meta: "list[str]") -> dict:
+    parsed = dict()
+    serial = re.compile(r"Logger: \#([\w]{6})")
+
+    for line in meta:
+        if serial.match(line):
+            parsed["logger_serial_number"] = serial.match(line).group(1)
+
+    return parsed
```

## Comparing `tsp-1.4.9.dist-info/LICENSE` & `tsp-1.5.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tsp-1.4.9.dist-info/METADATA` & `tsp-1.5.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tsp
-Version: 1.4.9
+Version: 1.5.3
 Summary: Making permafrost data effortless
 Home-page: https://gitlab.com/permafrostnet/teaspoon
 Author: Nick Brown
 Author-email: nick.brown@carleton.ca
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -24,14 +24,17 @@
 Requires-Dist: mock ; extra == 'dev'
 Provides-Extra: nc
 Requires-Dist: netCDF4 ; extra == 'nc'
 Requires-Dist: pfit (==0.2.1) ; extra == 'nc'
 Provides-Extra: plotting
 Requires-Dist: matplotlib ; extra == 'plotting'
 Requires-Dist: scipy ; extra == 'plotting'
+Provides-Extra: rbr
+Requires-Dist: pyrsktools ; extra == 'rbr'
+Requires-Dist: openpyxl ; extra == 'rbr'
 
 # Teaspoon
 
 ## See the full documentation on the [ReadTheDocs Pages](https://permafrostnet.gitlab.io/teaspoon/source/about.html)
 
 ## [What is it?](https://permafrostnet.gitlab.io/teaspoon/source/about.html)
 `tsp` ('teaspoon') is a python library designed to make working with permafrost ground temperature time series data more straightforward, efficient, and reproduceable. Some of the features include:
```

## Comparing `tsp-1.4.9.dist-info/RECORD` & `tsp-1.5.3.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,46 @@
-tsp/__init__.py,sha256=txeQiOv87P8Jsartlzx8o6yGhgLMzmLshJiqj-7m4BU,368
-tsp/__meta__.py,sha256=aJoYzKMTLxsj_ebew1nK76WJBzXRkt7Vr9-d6GBJABw,93
-tsp/core.py,sha256=zVITPQPYLeEh5_-DlqN9PzcJRkja0gADBvkrbFFm8IY,30354
+tsp/__init__.py,sha256=Ye8YN7QIbwkk6qMB_D0gB_F39JHY7WHsKKpNmE41g-U,380
+tsp/__meta__.py,sha256=YRWJbWvRef7F7Aeph-Cv-keq14LjWDj1ytAoDCkHp58,93
+tsp/core.py,sha256=zXIxGnQE8BIbGbAq672aFiIOOhp2RRx59Uf0R9fVefk,30720
 tsp/gtnp.py,sha256=kIxhLq_ve_cxU9v4_nDebc8jy6l7KQ87MOg8vK8lih4,3991
 tsp/misc.py,sha256=18w41G-umRi69lswXhpvJwrx4hqQ6r3bsvnmeKtpMU4,107
-tsp/physics.py,sha256=vUVsZdQOYaaWJ65VcHm1piuTem0I7xg4MtsJm8Uf33w,2877
-tsp/readers.py,sha256=2Z1tdvzgllbjSmqQtwFme6SNGmSrR3YFzu3R9kRtni8,16726
+tsp/physics.py,sha256=hgVOGU0Bj1g-gxBNhLEl7Gm3VXJKIHHu35uPvgVMOxE,2699
+tsp/readers.py,sha256=AR2__iJIDW4MGUd11B9RF3kPCEZAQ0xzNOHSrpgd-yM,18520
 tsp/time.py,sha256=82h7nxM-iXs2XwetF-alLtNvUm0qRtAA111gTMp5SY4,1379
-tsp/utils.py,sha256=ilJebXiiKcLhL7FQMJxU8TjnSpKoRtN_WrK1_peQfAQ,2956
+tsp/utils.py,sha256=sOJSZLmfv7sh4X971_gNgtZvXtS8ZwGmUdqnUybcVE4,2932
 tsp/data/2023-01-06_755-test-Dataset_2031-Constant_Over_Interval-Hourly-Ground_Temperature-Thermistor_Automated.timeserie.csv,sha256=Q3Ssnoo_kiSn9_orZHjtMxQ02YbrjCAEQKs5sHPFJCg,171
 tsp/data/2023-01-06_755-test.metadata.txt,sha256=Ux1YGqmAmRQmMIqqK8-OloQXflg4Y45FRwdT-WgCg8c,5686
 tsp/data/example_geotop.csv,sha256=rgVP7_tGEvUtn1K_KI98VVgm275D7qt8YegKMe3Vjw4,262289
 tsp/data/example_gtnp.csv,sha256=E5km06-cWlWMwzF-Qo7v0ZrlAvCTpyWIKY6hpzln4sc,191812
 tsp/dataloggers/AbstractReader.py,sha256=YsmESWrmH2jdL-Oli9pwjaFmPCEfJxjm4wx16FoRxpY,1777
-tsp/dataloggers/FG2.py,sha256=Qud2aAEEF8EBvUiluVJDk3REJUF2wJFVEfyxKmJCEY0,2947
-tsp/dataloggers/GP5W.py,sha256=q3yqxLtHCnW_SOIE40Vw-WIC2yuFwRdFiVJ1KvgrnNs,2975
+tsp/dataloggers/FG2.py,sha256=kvfjMQtoSs5ZzV7hc1lJ_SaDuSOOTONfI_nw2VaihO8,3281
+tsp/dataloggers/GP5W.py,sha256=dJ7I-P4_bIDDGb9zIdOf9vbxbxlcT3ZJ09HKLfRA6a0,3312
 tsp/dataloggers/Geoprecision.py,sha256=pDljZDasj7PNdiI5lOEpHZ9n7CZJ1aGlX96rN4cuPHI,916
 tsp/dataloggers/HOBO.py,sha256=xr5PvdMh_AO4CSsqdGLvtdVgfphc91Nl34Qs-AiP-wQ,33472
+tsp/dataloggers/RBRXL800.py,sha256=NjS6g_-grnC8BmLLW7qUppeOBYAOUJODNR-GwahnI7Y,8538
+tsp/dataloggers/RBRXR420.py,sha256=PIY46cjJnngul3OI4mZQ1TtlcFNTJmXmyxmex6TEEeI,13908
 tsp/dataloggers/__init__.py,sha256=4QcIctP5hoVfraU3PwhkTIca-4JIWH9u6-j4CQWoW1g,410
 tsp/dataloggers/logr.py,sha256=4IaqP6debop3QYnKWAyCzRxgve25txcr1itmtCciKkY,2665
+tsp/dataloggers/test_files/004448.DAT,sha256=1eJg5PtOrwlbzitp1XB5uE64ksqQHIIjTNgKIDn7zkI,201018
+tsp/dataloggers/test_files/004531.DAT,sha256=8Pag_PnR-3dK4rhr7os6kyQXVe8i1N5w1_ACefT9G4s,331292
+tsp/dataloggers/test_files/004531.HEX,sha256=0qJio9SvecR2MS4-nkjcZwqLh8h0sKdB6js_6yKqy5k,118535
+tsp/dataloggers/test_files/004534.HEX,sha256=cWMHCZ7JOu08RM2sjqay2aZiud35LY7NSsmBhjheGRI,118531
+tsp/dataloggers/test_files/010252.dat,sha256=_f9rvVq6U3ms3YQlN05doiy46PaNwqjeDlVCZK9NeU0,171935
+tsp/dataloggers/test_files/010252.hex,sha256=3o-A8c7v-KyQr0OR1CftJW1e7c6tyvY16MsZb_s0N74,84712
+tsp/dataloggers/test_files/010274.hex,sha256=4nB6jBzsP3XsraXZ_87IZZbZCqLQRtWcQ2mvR4R1c0I,62720
+tsp/dataloggers/test_files/010278.hex,sha256=8IOkmg1EC5mTj6vLECc9_t-Nb66Yp_dxcFCs6YzkCqo,173117
+tsp/dataloggers/test_files/012064.dat,sha256=LgwK9p0uzV0f7Gt1kIJWQSZWmG25i3vOJmTaG2jQ9gM,127062
+tsp/dataloggers/test_files/012064.hex,sha256=O2VReAh3xW-Rg-z8EJ0cR7aoVqvEfL6TpPkt5FXfagY,62921
+tsp/dataloggers/test_files/012081.hex,sha256=MwCQT5VLWiUVCmQGlzAMjZMwvdKolPAgtIIIvB2Z4sU,172576
+tsp/dataloggers/test_files/062834_20220904_2351.rsk,sha256=2DJa-wnrms1N_fJ9QmvcNFH5JMIBdBhcb-nXtUMp70k,1007616
+tsp/dataloggers/test_files/062834_20220904_2351.xlsx,sha256=z2sE1P--zcQJ1FoVJu43kXoxs1wIhwXGBukwzt1nIbc,308908
+tsp/dataloggers/test_files/07B1592.DAT,sha256=KalPKVVgzKTJrVQU8_3pmIJbEV1QJgXDUcJVwHnyYrY,107655
+tsp/dataloggers/test_files/07B1592.HEX,sha256=Eav6F_ExQ7qfg-mBMkZqrsASgWLM1RafNW43o8H4vEE,59683
+tsp/dataloggers/test_files/07B4450.DAT,sha256=1CpQviX4xhtkXL6wHENMmNvmJNarOAm6UcGL2G4AMZ8,162502
+tsp/dataloggers/test_files/07B4450.HEX,sha256=MyjYMf9EwWi7c91JwrNd4n0cPyAYZT1w719MygMQWO4,84576
 tsp/dataloggers/test_files/FG2_399.csv,sha256=Uonw_fFY3TUZ1O-XFtjRrV1yLr2iqUyBOlJM_wdZQGA,648322
 tsp/dataloggers/test_files/GP5W.csv,sha256=2mQl3YfzFVtvi3pdkEfyw9Cam3TzeHqAMnY06JSU6co,36948
 tsp/dataloggers/test_files/GP5W_260.csv,sha256=AbLBA12XLQLlNXpvht7Jy_DrvCUqhC1cQdFGnNYVXg0,68696
 tsp/dataloggers/test_files/GP5W_270.csv,sha256=ApqjqasC9eu1Na9R-tUrF-4S4vG-iq3trAhuVKjOaFY,147550
 tsp/dataloggers/test_files/H08-030-08_HOBOware.csv,sha256=uih-ZCFZRN9IF69RRVElvHfMGnaQ2-INljAsg_1x0BM,37920
 tsp/dataloggers/test_files/RBR_01.dat,sha256=TAZxbVzZTEWoOAizBPgTHWyk01Ca6VVv7yU6NzUaFlU,82735
 tsp/dataloggers/test_files/RBR_02.dat,sha256=xT8Q0F5D2wc2fxet1E7_dbb-BRbKK4rqT9bd6wInxEM,242142
@@ -42,14 +61,26 @@
 tsp/dataloggers/test_files/hobo_1_AB_minimal.txt,sha256=od_uIEWzk383rgAJ_LqXjplMICfY1kZ4Ly9qLOWyZQE,48977
 tsp/dataloggers/test_files/hobo_1_AB_raw.hobo,sha256=0YYlDKQZCNkR1K6UiPAnsuZycmT4pxeDrhOSi4Fflm0,65536
 tsp/dataloggers/test_files/hobo_1_AB_var2.csv,sha256=GfKmzq-QVLZq42ka7mX5cLCXrXyyZc71pI5b2qlTvbw,142070
 tsp/dataloggers/test_files/hobo_1_AB_var3.csv,sha256=xwtPv3llA-LReippxcOUE20cBb_DBLJz_vOX0kd5tkY,92381
 tsp/dataloggers/test_files/logR_ULogC16-32_1.csv,sha256=0HcCjf_jEBDpgpyTqiJC1oIoJsnt5Qdk4qV_s_KfuTQ,21966
 tsp/dataloggers/test_files/logR_ULogC16-32_2.csv,sha256=MU58RvTSwFrhJIbaKPSSKf51tPyZC9_ZXgPCCfk9p4M,19066
 tsp/dataloggers/test_files/mon_3_Ta_2010-08-18_2013-02-08.txt,sha256=Sqv23n-r1KLLdSsjjVeDvS-sX061Ivklhv5sDwRMwpA,734009
+tsp/dataloggers/test_files/rbr_001.dat,sha256=pS1QV_he33ccbfUpZMWm54AYDekez5us4MxS917wh0g,111570
+tsp/dataloggers/test_files/rbr_001.hex,sha256=HNrSlP05Y2LUqtvlzX_5O7rQrTGItUlZpMswra-dJpc,55293
+tsp/dataloggers/test_files/rbr_001_no_comment.dat,sha256=s_-tc-ShQfYqc4ObMh35xr8tQBHDxwjuBLDftX6Pc9U,111547
+tsp/dataloggers/test_files/rbr_001_no_comment.hex,sha256=HKG-sl7kw1A_Z3melKKT2xgVEAayv2fvCKzCFNM4LXA,55270
+tsp/dataloggers/test_files/rbr_002.dat,sha256=tUIX8InqQHObWzDVZrv1vTmY02zpIeepbKDpv4p5cpA,93525
+tsp/dataloggers/test_files/rbr_002.hex,sha256=W29e__jot7deVVC2XDtXwAgqfmvHzU7qi-7yQb4_mz0,57536
+tsp/dataloggers/test_files/rbr_003.hex,sha256=cjUaYWGm39WthiPvdzQKaOQ5FEKj3U9rCIe_0my7v2M,62703
+tsp/dataloggers/test_files/rbr_003.xls,sha256=PRxsKD88dTQEYOqz5z1FrkPox1jCkYyiBBZK0Kg-7tQ,263680
+tsp/dataloggers/test_files/rbr_xl_001.DAT,sha256=yZXKaClXMtYWDCs1cD2xTVdGj6LBMLKSjKnTgB4qPio,80057
+tsp/dataloggers/test_files/rbr_xl_002.DAT,sha256=JQNHL6X9z4Rp6IDqDBYx8vWsUU6oigl8nC23rMa3Enk,81601
+tsp/dataloggers/test_files/rbr_xl_003.DAT,sha256=ZEKheCvB1CiubY2kMngigY0NNhWTYAiC_hmQhzODPYw,221656
+tsp/dataloggers/test_files/rbr_xl_003.HEX,sha256=sunCD5C1t8l5y4p1b9iiHNsZUznYIuBLz4uwoGkZh3E,118459
 tsp/plots/__init__.py,sha256=i5AhpNwyuT6il7uk2Vtc4YBjVnZ0ifvHNXw19rvDtsM,71
 tsp/plots/static.py,sha256=hH-FkazPMKgqI74NtGUn_D_avo6ts9ZmzWgov2GLmEU,9448
-tsp-1.4.9.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-tsp-1.4.9.dist-info/METADATA,sha256=_iyP8WbiCvHDWsbxi1F7AJrqE5f328G1F_qXLJo-JZg,2731
-tsp-1.4.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-tsp-1.4.9.dist-info/top_level.txt,sha256=7tOR6y7BarphfWD2D7QFi_3F1jxagUZpHG8zwJIw4ck,30
-tsp-1.4.9.dist-info/RECORD,,
+tsp-1.5.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+tsp-1.5.3.dist-info/METADATA,sha256=nObnySvS_vS3145_sZ9CBKEB5gSMeaxx72A5y2amAeU,2835
+tsp-1.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tsp-1.5.3.dist-info/top_level.txt,sha256=7tOR6y7BarphfWD2D7QFi_3F1jxagUZpHG8zwJIw4ck,30
+tsp-1.5.3.dist-info/RECORD,,
```

