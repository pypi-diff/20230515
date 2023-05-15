# Comparing `tmp/biocartograph-0.4.2.tar.gz` & `tmp/biocartograph-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.4.2.tar", last modified: Mon May  1 18:13:15 2023, max compression
+gzip compressed data, was "biocartograph-0.5.0.tar", last modified: Mon May 15 11:33:34 2023, max compression
```

## Comparing `biocartograph-0.4.2.tar` & `biocartograph-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.505048 biocartograph-0.4.2/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-05-01 17:36:58.000000 biocartograph-0.4.2/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7211 2023-05-01 18:13:15.505048 biocartograph-0.4.2/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-05-01 17:36:58.000000 biocartograph-0.4.2/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7211 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-01 18:13:15.505048 biocartograph-0.4.2/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-01 17:37:01.000000 biocartograph-0.4.2/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-05-01 17:36:58.000000 biocartograph-0.4.2/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-05-01 17:36:58.000000 biocartograph-0.4.2/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    18799 2023-05-01 18:09:12.000000 biocartograph-0.4.2/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14707 2023-05-01 17:37:01.000000 biocartograph-0.4.2/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.206115 biocartograph-0.5.0/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.5.0/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-15 11:33:34.206115 biocartograph-0.5.0/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.5.0/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.204115 biocartograph-0.5.0/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-15 11:33:34.000000 biocartograph-0.5.0/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-15 11:33:34.206115 biocartograph-0.5.0/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-15 11:06:59.000000 biocartograph-0.5.0/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.203115 biocartograph-0.5.0/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-15 11:33:34.205115 biocartograph-0.5.0/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.5.0/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.5.0/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    19918 2023-05-15 11:06:59.000000 biocartograph-0.5.0/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    25243 2023-05-15 11:06:59.000000 biocartograph-0.5.0/src/biocartograph/special.py
```

### Comparing `biocartograph-0.4.2/LICENSE` & `biocartograph-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.4.2/PKG-INFO` & `biocartograph-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biocartograph
@@ -145,7 +147,9 @@
 Blood Cells:
 [blood cells](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/200153c58767d8b5162e66688ff4d669/raw/cfb74069d5cc9fc58e3558c753caaa60d4ba5e9b/index.html)
 [biocartograph gfa enrichment](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/42ec85df088a0c40de339a78322594bd/raw/0725bea467b0c153298655e3a0555670a812e80f/index.html)
 [biocartograph treemap cluster 2](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/d754528cf594087e509fe44fa071c178/raw/a78a82066e3d6aa2971aba2a64543a4018241372/index.html)
 
 [TCGA-BRCA](https://gdc.cancer.gov/) :
 Calculated using the biocartograph and a [TCGA derived data set](https://zenodo.org/record/3407557) with the results for [Breast Cancer mRNA-seq](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/ea18ac756d5142ac98219d45960583d4/raw/7cba81abb8af89416d11a682a2e0d19a311c954f/index.html)
+
+
```

### Comparing `biocartograph-0.4.2/README.md` & `biocartograph-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.4.2/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.5.0/biocartograph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.4.2
+Version: 0.5.0
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biocartograph
@@ -145,7 +147,9 @@
 Blood Cells:
 [blood cells](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/200153c58767d8b5162e66688ff4d669/raw/cfb74069d5cc9fc58e3558c753caaa60d4ba5e9b/index.html)
 [biocartograph gfa enrichment](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/42ec85df088a0c40de339a78322594bd/raw/0725bea467b0c153298655e3a0555670a812e80f/index.html)
 [biocartograph treemap cluster 2](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/d754528cf594087e509fe44fa071c178/raw/a78a82066e3d6aa2971aba2a64543a4018241372/index.html)
 
 [TCGA-BRCA](https://gdc.cancer.gov/) :
 Calculated using the biocartograph and a [TCGA derived data set](https://zenodo.org/record/3407557) with the results for [Breast Cancer mRNA-seq](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/ea18ac756d5142ac98219d45960583d4/raw/7cba81abb8af89416d11a682a2e0d19a311c954f/index.html)
+
+
```

### Comparing `biocartograph-0.4.2/setup.py` & `biocartograph-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.4.2",
+    version      = "0.5.0",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.4.2/src/biocartograph/enrichment.py` & `biocartograph-0.5.0/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.4.2/src/biocartograph/quantification.py` & `biocartograph-0.5.0/src/biocartograph/quantification.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     col_label_prefix = 'UMAP.'
     if bUseTDA :
         from sklearn import ensemble , preprocessing, manifold
         import kmapper as km
         model   = ensemble.IsolationForest( random_state=1337 )
         model   .fit( Xf )
         lens1   = model.decision_function( Xf )
-        P	= (lens1*Xf.T).T
+        P	= (lens1*Xf.T).T # FOR LENS1 ORDER TO BE CORRECT. SYMEMTRY => DOESN'T MATTER FOR P
         print ( 'WARNING: THIS IS A HIGHLY DEVELOPMENTAL FEATURE. TDA => KMAP' )
         mapper  = km.KeplerMapper( verbose=0 )
         Uf      = pd.DataFrame( mapper.fit_transform( Xf , projection = [a for a in range(int(umap_dimension)) ] ) )
         col_label_prefix = 'TDA.'
     else :
         Uf = pd.DataFrame( umap.UMAP( local_connectivity	= local_connectivity	,
                                   n_components		= int(umap_dimension)	,
@@ -122,14 +122,15 @@
         umap_dimension:int = 2 , umap_n_neighbors:int = 20 , umap_local_connectivity:float = 20. ,
         umap_seed:int = 42 , hierarchy_cmd:str = 'ward' , divergence = lambda r : np.exp(r) ,
         add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None , bRemoveCurse:bool=False ,
         n_projections:int = 2 , directory:str = './' , bQN:int = None ,
         nNeighborFilter:list[int] = None , heal_symmetry_break_method:str = 'average' ,
         epls_ownership:str = 'angle' , bNonEuclideanBackprojection:bool = False ,
         Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False , bUseTDA:bool = False ,
+        consensus_function = lambda x:np.sum(x) , consensus_labels:list[str] = None ,
         contraction_quantile:float = None   ,
         contraction_depth:float    = None   ) -> tuple[pd.DataFrame] :
     #
     import biocartograph.special as biox
     #
     if bVerbose :
         print ( "TO DISABLE WRITING OF RESULTS TO", directory )
@@ -152,27 +153,32 @@
         'umap_dimension:int':umap_dimension , 'umap_n_neighbors:int':umap_n_neighbors , 'umap_local_connectivity:float':umap_local_connectivity ,
         'umap_seed:int':umap_seed , 'hierarchy_cmd:str':hierarchy_cmd , 'divergence:lambda function': divergence ,
         'add_labels:list[str]':add_labels , 'sample_label:str':sample_label , 'alignment_label:str':alignment_label ,
         'bRemoveCurse:bool':bRemoveCurse , 'n_projections:int':n_projections , 'directory:str':directory , 'bQN:int':bQN ,
         'nNeighborFilter:list[int]':nNeighborFilter , 'heal_symmetry_break_method:str':heal_symmetry_break_method ,
         'epls_ownership:str':epls_ownership , 'bNonEuclideanBackprojection:bool':bNonEuclideanBackprojection ,
         'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA':bUseTDA ,
+        'consensus_function':consensus_function , 'consensus_labels:list[str]':consensus_labels ,
 	'contraction_quantile:float': contraction_quantile , ' contraction_depth:float': contraction_depth }
             ofile = open ( header_str + runinfo_file , 'w' )
             for item in run_dict.items():
                 if 'list' in str(type(item[1])):
                     print ( item[0],'\t=\t [', ','.join([str(i) for i in item[1]]) ,']', file=ofile )
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
             print ( 'PYTHON GLOBALS:\n ',
 			'\n'.join([ '\t=\t '.join([str(i) for i in item if not i is None]) for item in globals().items() if not item is None ] ),
 			file = ofile )
     #
+    if bVerbose:
+        print ( "BEGIN WARNINGS : ISSUED HERE MEANS THAT SOME ITEMS WITH ZERO STANDARD DEVIATION ARE DROPPED")
     adf = adf.iloc[ np.inf != np.abs( 1.0/np.std(adf.values,1) ) ,
                     np.inf != np.abs( 1.0/np.std(adf.values,0) ) ].copy().apply(pd.to_numeric)
+    if bVerbose:
+        print ( "END STD WARNINGS")
     #
     comp_df = None
     if not jdf is None :
         if not ( alignment_label is None ) :
             if bVerbose :
                 print ( "CONDUCTING COMPOSITIONAL ANALYSIS" )
             comp_df = biox.calculate_compositions ( adf , jdf, label = alignment_label , bAddPies=bAddPies )
@@ -212,14 +218,27 @@
         MF_f = u*s	# EQUIV TO : np.dot(u,np.diag(s))
         MF_s = vt.T*s
         if 'absolute' in distance_type.split('secondary[')[0] :
             MF_f = np.abs( MF_f )
         if 'absolute' in distance_type.split('secondary[')[0] :
             MF_s = np.abs( MF_s )
     #
+    # CONSENSUS CONDENSATION IS NOT DONE FOR SAMPLE SPACE
+    # THIS WILL AFFECT THE UMAP NOT THE CLUSTERING DISTANCES IF
+    # NOT THE bUseUMAP IS SET TRUE
+    if not consensus_labels is None :
+        if 'list' in str(type(consensus_labels)) :
+            for label in consensus_labels :
+                if 'str' in str(type(label)) :
+                    if label in jdf.index :
+                        gdf = adf.T.groupby(jdf.loc[label]).apply( consensus_function ).T
+                        aux_vals = np.linalg.svd( zvals(gdf.values)['z'] , False )
+                        aux_vals = aux_vals[0]*aux_vals[1]
+                        MF_f = np.concatenate([MF_f.T,aux_vals.T]).T
+    #
     if 'covariation' in distance_type or 'coexpression' in distance_type :
         input_values_f = MF_f
         input_values_s = MF_s
         if 'secondary[' in distance_type :	# THIS IS ACTUALLY A RATHER ODD THING TO DO
 						# BUT SOME POEPLE WILL WANT TO DO IT ANYWAY
             distance_type = distance_type.split('secondary[')[1].split(']')[0]
         else :
```

### Comparing `biocartograph-0.4.2/src/biocartograph/special.py` & `biocartograph-0.5.0/src/biocartograph/special.py`

 * *Files 25% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 """
 import numpy as np
 import pandas as pd
 import umap
 
 from impetuous.quantification import single_fc_compare
 from impetuous.special import unpack
+from impetuous.quantification import spearmanrho , pearsonrho , tjornhammarrho, correlation_core
+
+clean_label = lambda x : x.replace(' ','_').replace('/','Or').replace('\\','').replace('-','')
 
 def calculate_volcano_df( vals_df:pd.DataFrame , levels:list[str] , what:str='Regulation' ,
                                  bLog2:bool=False , bRanked:bool=False ) -> pd.DataFrame :
     if bLog2 :
         for idx in vals_df.index :
             if not idx == what :
                 w = np.min(vals_df.loc[idx].values)
@@ -174,17 +177,27 @@
 						axis:int = 0, order:str = 'descending'  , bRedundant:bool=False ,
 						hierarchy_level_label:str = 'HCLN' , bErrorCheck:bool = False ) -> tuple[list] :
     #
     df = pd.read_csv( header_str+hierarchy_file , sep='\t' , index_col=0 )
     if axis == 1 :
         df = df.T
     df = df.loc[:,[c for c in df.columns if hierarchy_id in c]].apply(pd.to_numeric)
+    nm = np.shape(df)
+    bCreatePC = nm[1]>1
+    if not bCreatePC :
+        print ( 'NOT ENOUGH LABELS FOR CONSTRUCTING A HIERARCHY' )
+        print ( 'SINGLE LABELING SUPPLIED : ' , hierarchy_id )
+        print ( 'FLAT GMT FOR CLUSTERS WILL BE CONSTRUCTED' )
+        gmtdf = df.groupby(hierarchy_id).apply(lambda x:x.index.values.tolist())
+        GMTS = list()
+        for name,entry in zip(gmtdf.index,gmtdf.values) :
+            GMTS.append(  hierarchy_level_label + '-' + 'cluster id ' + str(name) + '\t' + str(name) + '\t' + '\t'.join(entry)  )
+        return ( GMTS , None )
     df.loc[:,hierarchy_id+'0'] = 1 # ROOT
     #
-    # exit(1)
     cvs = sorted([ v[::-1] for v in np.max( df,0 ).items() ] )
     if cvs[0][0] >= cvs[-1][0] :
         print ( 'WARNING: UNUSABLE ORDER' )
     if len(cvs) < 2 :
         print ( 'WARNING: TO FEW LEVELS HIERARCHY LEVELS' )
     cnvs = [ c[1] for c in cvs ]
     df   = df.loc[ : , cnvs ]
@@ -244,37 +257,42 @@
             GMTS.append( '\t'.join([ item[0],'TEXT', *list(item[1]) ]) )
     PCL = []
     for item in  PCD.items() :
         PCL.append([ -1, item[0] , item[1] ])
     return ( GMTS, PCL )
 
 
-
 def reformat_results_and_print_gmtfile_pcfile ( header_str:str          = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' ,
 						hierarchy_file:str      = 'resdf_f.tsv' ,
                                                 hierarchy_id:str        = 'cids.user.' ,
                                                 axis:int = 0, order:str = 'descending' ,
-                                                hierarchy_level_label:str = 'HCLN' ) -> None :
+                                                hierarchy_level_label:str = 'HCLN' ) -> list[str] :
     GMTS,PCL = reformat_results_to_gmtfile_pcfile (	hierarchy_file		=  hierarchy_file ,
                                                 	header_str		=  header_str ,
                                                 	hierarchy_id		=  hierarchy_id ,
                                                 	axis			=  axis ,
 							order			=  order ,
                                                 	hierarchy_level_label	=  hierarchy_level_label )
-
-    gmt_of	= open ( header_str + hierarchy_file.split('.')[0] + '_gmts.gmt' , 'w' )
+    gmtname,pcname = None,None
+    gmtname     = header_str + hierarchy_file.split('.')[0] + '_gmts.gmt'
+    gmt_of	= open ( gmtname , 'w' )
+    print ( 'WRITING TO:' , gmtname )
     for g in GMTS :
         print ( g, file = gmt_of)
     gmt_of.close()
 
-    pc_of	= open ( header_str + hierarchy_file.split('.')[0] + '_pcfile.txt' , 'w' )
-    print ( "parent\tchild" , file = pc_of )
-    for g in PCL :
-        print ( g[1]+'\t'+g[2], file = pc_of)
-    pc_of.close()
+    if not PCL is None :
+        pcname  = header_str + hierarchy_file.split('.')[0] + '_pcfile.txt'
+        print ( 'WRITING TO:' , pcname )
+        pc_of	= open ( pcname , 'w' )
+        print ( "parent\tchild" , file = pc_of )
+        for g in PCL :
+            print ( g[1]+'\t'+g[2], file = pc_of)
+        pc_of.close()
+    return( gmtname , pcname )
 
 def rescreen (  header_str:str          = "../results/DMHMSY_Wed_Apr__5_10_02_33_2023_" ,
                 full_solution:str       = "hierarch_f.tsv" ,
                 o_filename:str          = None ) -> pd.DataFrame :
     #
     filename            = header_str + full_solution
     #
@@ -302,15 +320,15 @@
         return ( 0.0 )
     r   = value / q # wasteful slob ...
     r2  = r*r
     r4  = r2*r2
     r6  = r4*r2
     r12 = r6*r6
     p   = ( 1/r12 - 1/r6 ) * d * (-1)
-    p   = 1. + 1. * (p<0) + p * (p>=0)
+    p   = 1. + 0. * (p<0) + p * (p>=0)
     return ( value / p ) # WARNING ONLY FOR WASTEFUL SAIGAS
 
 def contract ( a:np.array , d:float=None , q:float=None , quantile:float=0.05 ) -> np.array :
     nm = np.shape(a)
     b  = a.reshape(-1)
     d_,q_ = d,q
     if d is None :
@@ -330,12 +348,219 @@
         d_ = 1.0/list(set(sorted( b )))[1]
     if q is None :
         q_ = np.quantile( b , q=quantile )
     # THIS OPERATION IS SLOWER
     return ( a.apply( lambda x : pd.Series([contraction(x_ , q=q_ , d=d_ ) for x_ in x],name=x.name,index=x.index) )  )
 
 
+def generate_hulls ( df:pd.DataFrame , gid:str = 'cids.max' , hid:str='UMAP.' ,
+                     cid:str = None , xid:str = None ,
+                     incremental:bool=False, qhull_options:str = None , bPlottered:bool=False ) -> dict :
+    #
+    # CONSIDERING SWTICH FROM QHULL TO FASTER AND TOPOLOGICALLY
+    # BETTER ALTERNATIVE IN THE FUTURE
+    #
+    if cid is None :
+        cid = hid
+    selection = sorted( list( set([ c for c in df.columns if hid in c or c in gid ]) - set([gid]) ) )
+    selection .append(gid)
+    projection_crds = sorted( list( set([ c for c in df.columns if cid in c ])  ) )
+    if not xid is None :
+        selection = [ s for s in selection if not xid in s ]
+        projection_crds = [ s for s in projection_crds if not xid in s ]
+
+    df_used = df.loc[ :,selection ]
+    nm = np.shape(df_used.values)
+    if nm[-1] < 3 :
+        print ( 'WARNING: MUST HAVE AT LEAST 2D DATA AND A LABEL SPECIFIED' )
+        print ( '         IN A DATAFRAME SO THAT DIM(DF) = N,M WHERE M>=2 ' )
+        print ( '         WILL RETURN EMPTY SOLUTION' )
+    import scipy.spatial as scs
+    if bPlottered :
+        import matplotlib.pyplot as plt
+    hulled = df_used.groupby(gid).apply( lambda x: tuple(( df.loc[x.index,projection_crds].values.tolist() ,
+                         scs.ConvexHull(        [ v[:-1] for v in x.values.tolist() ] ,
+                                                incremental=incremental, qhull_options=qhull_options ) )) )
+    all_convex_hulls = {}
+    for J in range(len( hulled )) :
+        gid_nr		= hulled.index.values[J]
+        ahull		= hulled.iloc[J]
+        points		= np.array( ahull[0] )
+        convex_hull	= ahull[1]
+        if bPlottered :
+            plt .plot ( points[:,0],points[:,1],'o' )
+        hull_border  = [ [ *points[convex_hull.vertices,i], points[convex_hull.vertices[0],i] ] for i in range(len(projection_crds)) ]
+        convex_hull_center  = np.mean(points,0)
+        all_convex_hulls[ gid_nr ] = { 'area':convex_hull.area , 'center':convex_hull_center , 'border':hull_border,
+					'info' : 'scipy spatial ConvexHull : ' + qhull_options if not qhull_options is None else 'default settings' }
+        if bPlottered :
+            plt.plot ( hull_border[0] , hull_border[1] , 'r-')
+            plt.plot ( convex_hull_center[0] , convex_hull_center[1] , '*k' )
+    if bPlottered :
+        plt .show()
+    return ( all_convex_hulls )
+
+def traverse_hierarchical_dictionary ( di:dict ) :
+    item = di
+    if not item is None :
+        for k_ in item.keys() :
+            print ( k_ )
+            traverse_hierarchical_dictionary ( item[k_] )
+
+def generate_neighbor_distance_df ( df:pd.DataFrame , lab:str='PCA' , iex:int=-1 , nNN:int = 20 ) -> pd.DataFrame :
+    from scipy.stats import rankdata
+    df0 = df.loc[ : ,[c for c in df.columns if lab in c ] ]
+    if True :
+        output = []
+        spr = spearmanrho( df0.iloc[:,:iex],df0.iloc[:,:iex] )
+        dsp = 1 - spr
+        for i in range(len( df0 )) :
+            j    = df0.index.values
+            m    = j[i]
+            x    = dsp[i]
+            bSel = rankdata ( x , 'ordinal' ) - 1 < nNN
+            output = [ *output , *sorted( [tuple((d_,r_,m,n_)) for d_,r_,n_ in  zip(  x[bSel], spr[i][bSel] ,j[bSel] )] ) ]
+        return ( pd.DataFrame(output,columns=['cor_distance','cor','gene','neighbor_gene']).loc[:,['gene','neighbor_gene','cor_distance','cor']] )
+
+
+def generate_neighbor_distance_information(  df:pd.DataFrame , lab:str='PCA' , iex:int=-1 , nNN:int = 20 ,sep:str='\t' ) -> str :
+    # results/Clustering_results/brain_HPA23v4/distance/nearest_neighbors.tsv
+    nn_df = generate_neighbor_distance_df ( df=df , lab=lab , iex=iex , nNN=nNN )
+    file_info = sep.join([ str(c) for c in nn_df.columns.values.tolist() ]) + '\n'
+    for v in nn_df.values :
+        file_info += sep.join( [ str(w) for w in v ] ) + '\n'
+    return ( file_info )
+
+
+
+def cluster_center_information ( all_convex_hulls:dict , sep:str = '\t' ) -> str :
+    # results/Clustering_results/brain_HPA23v4/UMAP/cluster_centers.tsv
+    N           = len( list(all_convex_hulls.items())[0][1]['center'] )
+    crdn        = 'xyzuvwabcdefghijklmnopqrst'
+    file_info   = ""
+    if len( crdn ) < N :
+        print ( 'WARNING : THERE IS PROBABLY AN ERROR IN THE HULL CALCULATION ', N , len(crdn) )
+    #
+    file_info += sep.join( [ 'cluster' , *[ crdn[i] for i in range(N) ] ] ) + '\n'
+    for item in all_convex_hulls.items() :
+        file_info += str(item[0]) + sep + sep.join([str(v) for v in item[1]['center']] ) + '\n'
+    return ( file_info )
+
+
+
+def create_cluster_polygon_information ( all_convex_hulls:dict , sep:str = '\t' ) -> str :
+    # results/Clustering_results/brain_HPA23v4/UMAP/UMAP_polygons.tsv
+    DIM         = len( list(all_convex_hulls.items())[0][1]['center'] )
+    crdn        = 'xyzuvwabcdefghijklmnopqrst'.upper()
+    file_info   = ""
+    if len( crdn ) < DIM :
+        print ( 'WARNING : THERE IS PROBABLY AN ERROR IN THE HULL CALCULATION ', DIM , len(crdn) )
+    #
+    file_info += sep.join( [    'cluster' , 'sub_cluster' , 'landmass', 'sub_type' ,
+                                *[ crdn[i] for i in range(DIM) ] ,
+                                'L1' , 'L2' , 'polygon_id'] ) + '\n'
+    #
+    for item in all_convex_hulls.items() :
+        crds = item[1]['border']
+        M    = len(crds[0])
+        crds = np.array(crds).reshape(-1)
+        crds = [ [ crds[k*M+i] for k in range(DIM) ] for i in range(M) ]
+        for crd in crds :
+            file_info += sep.join([ str(item[0]) , '1' , '1' ,'primary' , *[str(c) for c in crd] , '1' , '1' ,   str(item[0])+'_1_1' ]) + '\n'
+    return ( file_info )
+
+def create_directory ( directory_path:str ) :
+    import os
+    drsp = directory_path.split('/')
+    for i in range( len(drsp) ) :
+        if drsp[i] == '.' or drsp[i] == '..' :
+            continue
+        if len(drsp[:i+1])>0 :
+            thisdir = '/'.join(drsp[:i+1])
+            l = set( os.listdir ( '/'.join(thisdir.split('/')[:-1]) ) )
+            if not thisdir.split('/')[-1] in l :
+                os.mkdir( thisdir )
+
+#
+def quick_check_solution(header_str:str = '../results/DMHMSY_Tue_May__2_10_57_05_2023_' ) :
+    file 	= header_str + 'soldf_f.tsv'
+    df		= pd.read_csv(file,sep='\t',index_col=0 )
+    print ( df.iloc[:,np.argmax(df.iloc[1,:].values)]   )
+
+
+def generate_atlas_files ( header_str:str ,
+                fcfile:str = 'clustering/final_consensus.tsv' ,
+		nnfile:str = 'distance/nearest_neighbors.tsv' ,
+                umfile:str = 'UMAP/UMAP.tsv' ,
+                ccfile:str = 'UMAP/cluster_centers.tsv' ,
+		pofile:str = 'UMAP/UMAP_polygons.tsv' , nNN:int=20 ,
+                additional_directories:list[str] = ['data','enrichment','evaluation','graph','PCA','UMAP',
+					'svg','svg/heatmap','svg/bubble','svg/treemap','html','html/clustering_DV']) :
+    #
+    # START ATLAS GEN
+    sep = '\t'
+    df_sol_     = pd.read_csv( header_str + 'resdf_f.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
+    df_pca_     = pd.read_csv( header_str + 'pcas_df.tsv' , sep=sep , index_col=0 ) # SHOULD BE ASSERTED
+    common_idx  = sorted( list( set( df_sol_.index.values ) & set( df_pca_.index.values )))
+    df_sol_     = df_sol_.loc[ common_idx,: ]
+    df_pca_     = df_pca_.loc[ common_idx,: ]
+    #
+    df		= df_sol_
+    minmax      = lambda x: np.array( [ np.min(x,0) , np.max(x,0) ] )
+    scale       = minmax ( df.loc[:,[c for c in df if 'UMAP.' in c ]].values )
+    dfs         = ( df .loc[:,[c for c in df if 'UMAP.' in c ]] - scale[0]) / (scale[1]-scale[0])
+    dfs.columns = [ str(c) + '.scaled' for c in dfs.columns ]
+    df          = pd.concat([df.T,dfs.T]).T
+    all_hulls   = generate_hulls( df , hid = '.scaled' ,
+                        bPlottered=False )
+    #
+    hdir_str = header_str
+    if hdir_str[-1] == '_' :
+        hdir_str =  hdir_str[:-1] + '/'
+    #
+    create_directory ( hdir_str + '/'.join( fcfile.split('/')[:-1]) )
+    final_consensus_df = df_sol_.loc[:,['cids.max']].rename(columns={'cids.max':'cluster'}).copy()
+    final_consensus_df .index.name = 'gene'
+    final_consensus_df .to_csv( hdir_str + fcfile, sep=sep )
+    #
+    create_directory ( hdir_str + '/'.join( umfile.split('/')[:-1]) )
+    udf = df.loc[:,[c for c in df.columns if 'UMAP' in c ] ]
+    udf .columns = [ c.replace('.','_') for c in udf.columns ]
+    udf .to_csv( hdir_str + umfile, sep=sep )
+    #
+    create_directory ( hdir_str + '/'.join( ccfile.split('/')[:-1]) )
+    ccinfo = cluster_center_information( all_hulls )
+    o_f = open( hdir_str + ccfile,'w')
+    print ( ccinfo , file=o_f )
+    o_f .close()
+    #
+    create_directory ( hdir_str + '/'.join( pofile.split('/')[:-1]) )
+    poinfo  = create_cluster_polygon_information( all_hulls )
+    o_f = open( hdir_str + pofile,'w')
+    print ( poinfo , file=o_f )
+    o_f .close()
+    #
+    create_directory ( hdir_str + '/'.join( nnfile.split('/')[:-1]) )
+    nninfo  = generate_neighbor_distance_information(  df_pca_ , lab = 'PCA' ,
+			 iex = -1 , nNN = nNN , sep = '\t' )
+    o_f = open( hdir_str + nnfile,'w')
+    print ( nninfo , file=o_f )
+    o_f .close()
+    for dir in additional_directories :
+        create_directory ( hdir_str + dir )
+
+
 if __name__ == '__main__':
+    #
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
-
-
+    #
+    results_dir = '../results/'
+    header_str  = results_dir + 'DMHMSY_Wed_May__3_11_48_58_2023_'
+    #
+    generate_atlas_files ( header_str = header_str )
+    """ ,
+                nnfile = 'distance/nearest_neighbors.tsv' ,
+                ccfile = 'UMAP/cluster_centers.tsv' ,
+                pofile = 'UMAP/UMAP_polygons.tsv' )
+    """
+    #
```

