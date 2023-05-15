# Comparing `tmp/protloc_mex1-0.0.4.tar.gz` & `tmp/protloc_mex1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protloc_mex1-0.0.4.tar", last modified: Wed May 10 07:39:21 2023, max compression
+gzip compressed data, was "protloc_mex1-0.0.5.tar", last modified: Mon May 15 11:12:08 2023, max compression
```

## Comparing `protloc_mex1-0.0.4.tar` & `protloc_mex1-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1143 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      536 2023-04-26 08:22:56.000000 protloc_mex1-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.622341 protloc_mex1-0.0.4/protloc_mex1/
--rw-rw-rw-   0        0        0    14385 2023-05-08 13:54:14.000000 protloc_mex1-0.0.4/protloc_mex1/AA_count.py
--rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.4/protloc_mex1/GO_count.py
--rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.4/protloc_mex1/SHAP_conduct.py
--rw-rw-rw-   0        0        0    28926 2023-04-29 13:10:06.000000 protloc_mex1-0.0.4/protloc_mex1/SHAP_plus.py
--rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.4/protloc_mex1/__init__.py
--rw-rw-rw-   0        0        0    10886 2023-05-09 03:16:02.000000 protloc_mex1-0.0.4/protloc_mex1/classifier_evalute.py
-drwxrwxrwx   0        0        0        0 2023-05-10 07:39:21.662513 protloc_mex1-0.0.4/protloc_mex1.egg-info/
--rw-rw-rw-   0        0        0     1143 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      380 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       91 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-10 07:39:21.000000 protloc_mex1-0.0.4/protloc_mex1.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      859 2023-05-10 07:30:07.000000 protloc_mex1-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-10 07:39:21.666519 protloc_mex1-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.679195 protloc_mex1-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-04-25 08:38:35.000000 protloc_mex1-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     7733 2023-05-15 11:12:08.678632 protloc_mex1-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     6953 2023-05-15 09:50:59.000000 protloc_mex1-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.610279 protloc_mex1-0.0.5/protloc_mex1/
+-rw-rw-rw-   0        0        0    14498 2023-05-15 08:52:22.000000 protloc_mex1-0.0.5/protloc_mex1/AA_count.py
+-rw-rw-rw-   0        0        0     8014 2023-04-29 12:40:52.000000 protloc_mex1-0.0.5/protloc_mex1/GO_count.py
+-rw-rw-rw-   0        0        0    10510 2023-04-28 13:10:04.000000 protloc_mex1-0.0.5/protloc_mex1/SHAP_conduct.py
+-rw-rw-rw-   0        0        0    31630 2023-05-11 12:52:32.000000 protloc_mex1-0.0.5/protloc_mex1/SHAP_plus.py
+-rw-rw-rw-   0        0        0       39 2023-04-29 12:25:34.000000 protloc_mex1-0.0.5/protloc_mex1/__init__.py
+-rw-rw-rw-   0        0        0    10886 2023-05-09 03:16:02.000000 protloc_mex1-0.0.5/protloc_mex1/classifier_evalute.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:12:08.675013 protloc_mex1-0.0.5/protloc_mex1.egg-info/
+-rw-rw-rw-   0        0        0     7733 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       91 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-15 11:12:08.000000 protloc_mex1-0.0.5/protloc_mex1.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      859 2023-05-15 11:01:00.000000 protloc_mex1-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:12:08.679195 protloc_mex1-0.0.5/setup.cfg
```

### Comparing `protloc_mex1-0.0.4/LICENSE.txt` & `protloc_mex1-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.4/protloc_mex1/AA_count.py` & `protloc_mex1-0.0.5/protloc_mex1/AA_count.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,56 +7,56 @@
 
 from Bio.SeqUtils.ProtParam import ProteinAnalysis
 
 import numpy as np
 
 import re
 
-def dna_sequence_conduct(df):
+def dna_sequence_conduct(df,sequence_name= 'gene_seq'):
     
     elements = {'C': {'A': 5, 'T': 5, 'C': 4, 'G': 5},
                 'H': {'A': 5, 'T': 6, 'C': 5, 'G': 5},
                 'N': {'A': 5, 'T': 2, 'C': 3, 'G': 5},
                 'O': {'A': 0, 'T': 2, 'C': 1, 'G': 1}}
 
     # 过滤所有非法碱基
-    df['gene_seq'] = df['gene_seq'].apply(lambda x: ''.join([base for base in x if base in {'A', 'T', 'C', 'G'}]))
+    df[sequence_name] = df[sequence_name].apply(lambda x: ''.join([base for base in x if base in {'A', 'T', 'C', 'G'}]))
     # 计算元素的频率
-    df['Carbon']   = df['gene_seq'].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
-    df['Hydrogen'] = df['gene_seq'].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
-    df['Nitrogen'] = df['gene_seq'].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
-    df['Oxygen']   = df['gene_seq'].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
+    df['Carbon']   = df[sequence_name].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
+    df['Hydrogen'] = df[sequence_name].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
+    df['Nitrogen'] = df[sequence_name].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
+    df['Oxygen']   = df[sequence_name].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
     # 计算碱基频率
-    df['A'] = df['gene_seq'].apply(lambda x: x.count('A') / len(x))
-    df['T'] = df['gene_seq'].apply(lambda x: x.count('T') / len(x))
-    df['G'] = df['gene_seq'].apply(lambda x: x.count('G') / len(x))
-    df['C'] = df['gene_seq'].apply(lambda x: x.count('C') / len(x))
+    df['A'] = df[sequence_name].apply(lambda x: x.count('A') / len(x))
+    df['T'] = df[sequence_name].apply(lambda x: x.count('T') / len(x))
+    df['G'] = df[sequence_name].apply(lambda x: x.count('G') / len(x))
+    df['C'] = df[sequence_name].apply(lambda x: x.count('C') / len(x))
     
     
     return df
 
-def rna_sequence_conduct(df):
+def rna_sequence_conduct(df, sequence_name= 'gene_seq'):
     
     elements = {'C': {'A': 5, 'U': 4, 'C': 4, 'G': 5},
                 'H': {'A': 5, 'U': 4, 'C': 5, 'G': 5},
                 'N': {'A': 5, 'U': 2, 'C': 3, 'G': 5},
                 'O': {'A': 0, 'U': 2, 'C': 1, 'G': 1}}
 
     # 过滤所有非法碱基
-    df['gene_seq'] = df['gene_seq'].apply(lambda x: ''.join([base for base in x if base in {'A', 'U', 'C', 'G'}]))
+    df[sequence_name] = df[sequence_name].apply(lambda x: ''.join([base for base in x if base in {'A', 'U', 'C', 'G'}]))
     # 计算元素的频率
-    df['Carbon']   = df['gene_seq'].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
-    df['Hydrogen'] = df['gene_seq'].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
-    df['Nitrogen'] = df['gene_seq'].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
-    df['Oxygen']   = df['gene_seq'].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
+    df['Carbon']   = df[sequence_name].apply(lambda x: sum([elements['C'][base] for base in x]) / len(x))
+    df['Hydrogen'] = df[sequence_name].apply(lambda x: sum([elements['H'][base] for base in x]) / len(x))
+    df['Nitrogen'] = df[sequence_name].apply(lambda x: sum([elements['N'][base] for base in x]) / len(x))
+    df['Oxygen']   = df[sequence_name].apply(lambda x: sum([elements['O'][base] for base in x]) / len(x))
     # 计算碱基频率
-    df['A'] = df['gene_seq'].apply(lambda x: x.count('A') / len(x))
-    df['U'] = df['gene_seq'].apply(lambda x: x.count('U') / len(x))
-    df['G'] = df['gene_seq'].apply(lambda x: x.count('G') / len(x))
-    df['C'] = df['gene_seq'].apply(lambda x: x.count('C') / len(x))
+    df['A'] = df[sequence_name].apply(lambda x: x.count('A') / len(x))
+    df['U'] = df[sequence_name].apply(lambda x: x.count('U') / len(x))
+    df['G'] = df[sequence_name].apply(lambda x: x.count('G') / len(x))
+    df['C'] = df[sequence_name].apply(lambda x: x.count('C') / len(x))
     
     
     return df
 
 def protein_sequence_conduct(file_data, sequence_name="Sequence"):
     """
     Conduct protein sequence analysis and add relevant protein properties to an input pandas dataframe.
```

### Comparing `protloc_mex1-0.0.4/protloc_mex1/GO_count.py` & `protloc_mex1-0.0.5/protloc_mex1/GO_count.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.4/protloc_mex1/SHAP_conduct.py` & `protloc_mex1-0.0.5/protloc_mex1/SHAP_conduct.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.4/protloc_mex1/SHAP_plus.py` & `protloc_mex1-0.0.5/protloc_mex1/SHAP_plus.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,45 +63,86 @@
         for i in list(feature_inner_name):
             type_data_all_feature_shap_outcome[i]=list(map(lambda x: type_data_all_feature_shap[x][i],type_data_all_feature_shap.keys()))   
               
             type_data_all_feature_shap_outcome[i]=reduce(lambda x,y: pd.concat([x,y],axis=1),type_data_all_feature_shap_outcome[i])       
             
         return(type_data_all_feature_shap_outcome)
     
-    def SHAP_importance_sum_claulate_process(self,depleted_ID_len=0,file_name='human_'):
-        scale=MinMaxScaler()
-        self.type_data_shap_sum_all=dict()
-        self.type_data_shap_sum_all_outcome=dict()
-        self.shap_feature_importance=dict()
-        self.shap_feature_importance_T=None
-        for value in self.shapley_data_all.keys():
-            ##shap求和，并且归一化
+    # def SHAP_importance_sum_claulate_process(self,depleted_ID_len=0,file_name='human_'):
+    #     scale=MinMaxScaler()
+    #     self.type_data_shap_sum_all=dict()
+    #     self.type_data_shap_sum_all_outcome=dict()
+    #     self.shap_feature_importance=dict()
+    #     self.shap_feature_importance_T=None
+    #     for value in self.shapley_data_all.keys():
+    #         ##shap求和，并且归一化
             
-            self.type_data_shap_sum_all[value]=np.array(self.shapley_data_all[value].iloc[:,:len(self.shapley_data_all[value].columns)-depleted_ID_len]).sum(axis=1)
-            self.type_data_shap_sum_all[value]=pd.DataFrame({'sum_shap':self.type_data_shap_sum_all[value].reshape(-1,),
-                                                        'scale':scale.fit_transform(self.type_data_shap_sum_all[value].reshape(-1,1)).reshape(-1,)},
-                                                       index=self.shapley_data_all[value].index)
-            self.type_data_shap_sum_all_outcome[value]=pd.merge(self.shapley_data_all[value],self.type_data_shap_sum_all[value],how="inner",left_index=True,right_index=True)
+    #         self.type_data_shap_sum_all[value]=np.array(self.shapley_data_all[value].iloc[:,:len(self.shapley_data_all[value].columns)-depleted_ID_len]).sum(axis=1)
+    #         self.type_data_shap_sum_all[value]=pd.DataFrame({'sum_shap':self.type_data_shap_sum_all[value].reshape(-1,),
+    #                                                     'scale':scale.fit_transform(self.type_data_shap_sum_all[value].reshape(-1,1)).reshape(-1,)},
+    #                                                    index=self.shapley_data_all[value].index)
+    #         self.type_data_shap_sum_all_outcome[value]=pd.merge(self.shapley_data_all[value],self.type_data_shap_sum_all[value],how="inner",left_index=True,right_index=True)
             
             
-            ##特征的shap绝对值相加作为特征的重要性
-            self.shap_feature_importance[value]=np.abs(self.shapley_data_all[value].iloc[:,:len(self.shapley_data_all[value].columns)-depleted_ID_len])
-            self.shap_feature_importance[value]=self.shap_feature_importance[value].mean(axis=0)
-            self.shap_feature_importance[value]=pd.DataFrame(self.shap_feature_importance[value],columns=[value])
-
-        self.shap_feature_importance=reduce(lambda x,y: pd.merge(x,y,how="inner",left_index=True,right_index=True),self.shap_feature_importance.values())
-
-        self.shap_feature_importance.columns=[re.compile('('+file_name+')|(_shap_value)').sub('',name) for name in self.shap_feature_importance.columns]
-        ##shap_feature_importance转置
-        self.shap_feature_importance_T=self.shap_feature_importance.T
-        return{'type_data_shap_sum_all_outcome':self.type_data_shap_sum_all_outcome,
-               'shap_feature_importance':self.shap_feature_importance,
-               'shap_feature_importance_T':self.shap_feature_importance_T}
+    #         ##特征的shap绝对值相加作为特征的重要性
+    #         self.shap_feature_importance[value]=np.abs(self.shapley_data_all[value].iloc[:,:len(self.shapley_data_all[value].columns)-depleted_ID_len])
+    #         self.shap_feature_importance[value]=self.shap_feature_importance[value].mean(axis=0)
+    #         self.shap_feature_importance[value]=pd.DataFrame(self.shap_feature_importance[value],columns=[value])
+
+    #     self.shap_feature_importance=reduce(lambda x,y: pd.merge(x,y,how="inner",left_index=True,right_index=True),self.shap_feature_importance.values())
+
+    #     self.shap_feature_importance.columns=[re.compile('('+file_name+')|(_shap_value)').sub('',name) for name in self.shap_feature_importance.columns]
+    #     ##shap_feature_importance转置
+    #     self.shap_feature_importance_T=self.shap_feature_importance.T
+    #     return{'type_data_shap_sum_all_outcome':self.type_data_shap_sum_all_outcome,
+    #            'shap_feature_importance':self.shap_feature_importance,
+    #            'shap_feature_importance_T':self.shap_feature_importance_T}
+    
+    
+    def SHAP_importance_sum_claulate_process(self, base_probablity_dict, depleted_ID_len=0, file_name='human_'):
+        scale = MinMaxScaler()
+        self.type_data_shap_sum_all = dict()
+        self.type_data_shap_sum_all_outcome = dict()
+        self.shap_feature_importance = dict()
+        self.shap_feature_importance_T = None
+        for value in self.shapley_data_all.keys():
+            # shap求和，并且归一化
+            sum_shap = np.array(self.shapley_data_all[value].iloc[:, :len(self.shapley_data_all[value].columns)-depleted_ID_len]).sum(axis=1)
+
+            # 获取对应的基准概率
+            base_value = base_probablity_dict[value]
+
+            # 创建 sum_shap 的副本，用于计算 probablity
+            probablity = sum_shap.copy()
+
+            # 将基准概率加到 probablity 值上
+            probablity += base_value
+
+            self.type_data_shap_sum_all[value] = pd.DataFrame({'sum_shap': sum_shap.reshape(-1,),
+                                                               'scale': scale.fit_transform(sum_shap.reshape(-1,1)).reshape(-1,),
+                                                               'probablity': probablity},  # 新增probablity列
+                                                              index=self.shapley_data_all[value].index)
+            self.type_data_shap_sum_all_outcome[value] = pd.merge(self.shapley_data_all[value], self.type_data_shap_sum_all[value], how="inner", left_index=True, right_index=True)
+
+            # 特征的shap绝对值相加作为特征的重要性
+            self.shap_feature_importance[value] = np.abs(self.shapley_data_all[value].iloc[:, :len(self.shapley_data_all[value].columns)-depleted_ID_len])
+            self.shap_feature_importance[value] = self.shap_feature_importance[value].mean(axis=0)
+            self.shap_feature_importance[value] = pd.DataFrame(self.shap_feature_importance[value], columns=[value])
+
+        self.shap_feature_importance = reduce(lambda x, y: pd.merge(x, y, how="inner", left_index=True, right_index=True), self.shap_feature_importance.values())
+
+        self.shap_feature_importance.columns = [re.compile('('+file_name+')|(_shap_value)').sub('', name) for name in self.shap_feature_importance.columns]
+        # shap_feature_importance转置
+        self.shap_feature_importance_T = self.shap_feature_importance.T
+        return {'type_data_shap_sum_all_outcome': self.type_data_shap_sum_all_outcome,
+                'shap_feature_importance': self.shap_feature_importance,
+                'shap_feature_importance_T': self.shap_feature_importance_T}
     
 
+    
 
 class FeaturePlotSource:
     def __init__(self, X_data, shapley_data_all):
         self.X_data = X_data
         self.shapley_data_all = shapley_data_all
     
     def plot(self):
```

### Comparing `protloc_mex1-0.0.4/protloc_mex1/classifier_evalute.py` & `protloc_mex1-0.0.5/protloc_mex1/classifier_evalute.py`

 * *Files identical despite different names*

### Comparing `protloc_mex1-0.0.4/pyproject.toml` & `protloc_mex1-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "protloc_mex1"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Ze Yu Luo", email="1024226968@qq.com" },
 ]
 description = "..."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

