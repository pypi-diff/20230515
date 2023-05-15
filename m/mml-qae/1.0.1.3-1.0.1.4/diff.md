# Comparing `tmp/mml_qae-1.0.1.3.tar.gz` & `tmp/mml_qae-1.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mml_qae-1.0.1.3.tar", last modified: Sun May 14 08:20:01 2023, max compression
+gzip compressed data, was "dist\mml_qae-1.0.1.4.tar", last modified: Mon May 15 13:33:01 2023, max compression
```

## Comparing `mml_qae-1.0.1.3.tar` & `mml_qae-1.0.1.4.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/
--rw-rw-rw-   0        0        0     3651 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2829 2023-05-14 08:19:44.000000 mml_qae-1.0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae/
--rw-rw-rw-   0        0        0     1664 2023-05-14 08:17:49.000000 mml_qae-1.0.1.3/mml_qae/MoreErrors.py
--rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.3/mml_qae/__init__.py
--rw-rw-rw-   0        0        0     2897 2023-05-14 08:16:28.000000 mml_qae-1.0.1.3/mml_qae/lists_of_number.py
--rw-rw-rw-   0        0        0     1399 2023-05-14 08:18:15.000000 mml_qae-1.0.1.3/mml_qae/one_list_of_number.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/
--rw-rw-rw-   0        0        0     3651 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/mml_qae.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 08:20:01.000000 mml_qae-1.0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      668 2023-05-14 08:19:54.000000 mml_qae-1.0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:15:44.000000 mml_qae-1.0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     4193 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3431 2023-05-15 13:32:28.000000 mml_qae-1.0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae/
+-rw-rw-rw-   0        0        0     1664 2023-05-14 08:17:49.000000 mml_qae-1.0.1.4/mml_qae/MoreErrors.py
+-rw-rw-rw-   0        0        0        0 2023-05-13 07:17:18.000000 mml_qae-1.0.1.4/mml_qae/__init__.py
+-rw-rw-rw-   0        0        0     2905 2023-05-15 13:22:26.000000 mml_qae-1.0.1.4/mml_qae/lists_of_number.py
+-rw-rw-rw-   0        0        0     1407 2023-05-15 13:23:01.000000 mml_qae-1.0.1.4/mml_qae/one_list_of_number.py
+drwxrwxrwx   0        0        0        0 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae.egg-info/
+-rw-rw-rw-   0        0        0     4193 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/mml_qae.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-15 13:33:00.000000 mml_qae-1.0.1.4/mml_qae.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      689 2023-05-15 13:32:45.000000 mml_qae-1.0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 13:33:01.000000 mml_qae-1.0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      668 2023-05-15 13:32:55.000000 mml_qae-1.0.1.4/setup.py
```

### Comparing `mml_qae-1.0.1.3/PKG-INFO` & `mml_qae-1.0.1.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,54 @@
-Metadata-Version: 2.1
-Name: mml_qae
-Version: 1.0.1.3
-Summary: The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.
-Home-page: https://www.python.org
-Author: ETRO_secondleader
-Author-email: ETRO_gfyx@163.com
-License: UNKNOWN
-Description: # Python:mml-qae库帮助文档
-        ## 使用环境
-        + Python环境:最好使用3.7.2。如果不在3.7.2环境下出现报错，请区分ImportError(由mml内部引入包的版本错误)和其他错误。
-        + 编译格式：没什么好说的，Python默认使用的Unicode和UTF-8解码格式。
-        + 请尽可能保持mml-qae包的最新版本。1.2及以前的版本并不全面！
-        ---
-        ## 开发者发言
-        + We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with nature language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more porperly way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I can't promise how long the interval between two updataions. Another thing need to be attentioned, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will tell all of those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name to the built-in functions! And that's all. Have a nice day with MachineLearning and DataDealing!
-        + Packages needed
-        > + statsmodels
-        > + sklearn
-        > + jieba
-        > + spaCy
-        > + pandas
-        > + numpy
-        > + matplotlib
-        > + wordcloud
-        ---
-        ## 历史版本(包括部分未公布的版本)
-        + 1 简易大数据处理与网络构建
-        > +  1.0 预发布版本
-        > > + 1.0.0 
-        >      初代版本，无项目描述。
-        > > + 1.0.1
-        >      修复1.0.0中的明显问题。
-        > > > + 1.0.1.1  加入项目描述.
-        > > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
-        > > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
-        > >  + 1.0.2
-        >      加入封装好的自然语言处理快捷方法。
-        > > > + 1.0.2.1  加入中文处理模型.
-        > > > + 1.0.2.2  加入英语处理模型.
-        > >  + 1.0.3     修复1.0版本的bug和问题。
-        > +  1.1 完善版本
-        > >  + 1.1.1 加入数据库处理方法。
-        > > > + 1.1.1.1 MySQL
-        > > > + 1.1.1.2 NoSQL
-        > > > + 1.1.1.3 更多数据库
-        > >  + 1.1.2 Spark多线程方法封装
-        > > > + 1.1.2.1 多线程封装
-        > > > + 1.1.2.2 集群管理方法封装
-        > >  + 1.1.3 简易网络构建方法封装
-        > > > + 1.1.3.1 本地index.html的构建方法封装
-        > > > + 1.1.3.2 爬虫的封装
-        > + 1.2 修复版本
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+# Python:mml-qae库帮助文档
+## 使用环境
++ Python环境:最好使用3.7.2。如果不在3.7.2环境下出现报错，请区分ImportError(由mml内部引入包的版本错误)和其他错误。
++ 编译格式：没什么好说的，Python默认使用的Unicode和UTF-8解码格式。
++ 请尽可能保持mml-qae包的最新版本。1.2及以前的版本并不全面！
+---
+## 开发公告
+    此处将放置每一个的更新日志.与历史版本一栏不同的是,这里是实时更新且更加详细的.
++ 1.0.0 2023.5.14 初代版本.框架构建.
++ 1.0.1 ----------- 略微扩充了方法.
++ 1.0.1.1 --------- 向pypi.org中扩充了项目描述.
++ 1.0.1.2 --------- 向pypi.org中扩充了说明文档.(由于作者脑抽忘记再1.0.1.1时上传了不得不新增一个版本)
++ 1.0.1.3 --------- 加入了子模块MoreErrors以提供更多错误支持.
++ 1.0.1.4 2023.5.15 突然引起的恶性错误,此为紧急修复版本.
+---
+## 开发者发言
++ We now have packages to deal with big data like statsmodels, sklearn, Spark, or packages to deal with natural language, such as jieba or spaCy. I admit that those packages are really useful while facing whith tons of csv data. BUT! I think we need a nicer package to deal with data, don't we? So, the mml-qae package(the whole name is My Machine Learning-Quicker and Easier) is here to help you. Alright, so, I have to say that I didn't do anything new, but I put those complex codes together into grand-new methods, so that you will be able to deal with MachineLearning and DataDealing. I started this project on 14th, May 2023 with version 1.0.1. In a more proper way, I worked on this project with my team ETRO(to see the Author's Email). I promise to update it regularly, but I cannot say how long the interval between two updataions will be for certain. Another thing needed to be paid attentioned is, this package only works at Python3.7.2, and you MUST pip install the packages needed in mml, like statsmodels. I will speak of all those packages you need to preinstall in README.md. Last but not least, never use 'from mml-qae import *'. Many methods in mml are the same name with the built-in functions! That'll be all, and have fun with MachineLearning and DataDealing!
++ Packages needed
+> + statsmodels
+> + sklearn
+> + jieba
+> + spaCy
+> + pandas
+> + numpy
+> + matplotlib
+> + wordcloud
+---
+## 历史版本(包括部分未公布的版本)
++ 1 简易大数据处理与网络构建
+> +  1.0 预发布版本
+> > + 1.0.0 
+>      初代版本，无项目描述。
+> > + 1.0.1
+>      修复1.0.0中的明显问题。
+> > > + 1.0.1.1  加入项目描述.
+> > > + 1.0.1.2  加入帮助文档README.md并修复一些小问题
+> > > + 1.0.1.3  加入一些自定义错误和修复一些小问题
+> >  + 1.0.2
+>      加入封装好的自然语言处理快捷方法。
+> > > + 1.0.2.1  加入中文处理模型.
+> > > + 1.0.2.2  加入英语处理模型.
+> >  + 1.0.3     修复1.0版本的bug和问题。
+> +  1.1 完善版本
+> >  + 1.1.1 加入数据库处理方法。
+> > > + 1.1.1.1 MySQL
+> > > + 1.1.1.2 NoSQL
+> > > + 1.1.1.3 更多数据库
+> >  + 1.1.2 Spark多线程方法封装
+> > > + 1.1.2.1 多线程封装
+> > > + 1.1.2.2 集群管理方法封装
+> >  + 1.1.3 简易网络构建方法封装
+> > > + 1.1.3.1 本地index.html的构建方法封装
+> > > + 1.1.3.2 爬虫的封装
+> + 1.2 修复版本
```

### Comparing `mml_qae-1.0.1.3/mml_qae/MoreErrors.py` & `mml_qae-1.0.1.4/mml_qae/MoreErrors.py`

 * *Files identical despite different names*

### Comparing `mml_qae-1.0.1.3/mml_qae/lists_of_number.py` & `mml_qae-1.0.1.4/mml_qae/lists_of_number.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #对多组数字参数的分析: 通过多组数据判断某一特征的目标
 import pandas as pd 
 import numpy as np
 from sklearn.model_selection import train_test_split as tts
 from sklearn.neighbors import KNeighborsClassifier as knc 
 from sklearn.metrics import accuracy_score as acc
-import MoreErrors as me
+import mml_qae.MoreErrors as me
 def max_of_list(l:list):
     
     maxium=l[0]
     for i in l:
         try:
             i=float(i)
         except:
```

### Comparing `mml_qae-1.0.1.3/mml_qae/one_list_of_number.py` & `mml_qae-1.0.1.4/mml_qae/one_list_of_number.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import matplotlib.pyplot as plt 
 import statsmodels.api as sm
 import numpy as np 
-import MoreErrors as me
+import mml_qae.MoreErrors as me
 def make_results(lista,listb,i=False):#给定两列表返回预测组 
     """给定两个列表(顺序:特征组,目标组)\n i值默认为假,不打印模型准确度;为真则打印准确度""" 
     X=lista
     Y=listb
     dX=np.column_stack((X,np.power(X,2),np.power(X,3),np.power(X,4),np.sin(X),np.tan(X),np.cos(X)  ))
     X_added=sm.add_constant(dX)
     model=sm.OLS(Y,X_added)
```

### Comparing `mml_qae-1.0.1.3/setup.py` & `mml_qae-1.0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools 
 
 with open("README.md", "r",encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
       name='mml_qae',
-      version='1.0.1.3',
+      version='1.0.1.4',
       description='The packages for the machine learning(just easily learn!) are always hard to study, and difficult to use. Now you have the MyMachineLearning_Quicker_and_Easier! It can maybe help you to use machine learning.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='ETRO_secondleader',
       author_email='ETRO_gfyx@163.com',
       url='https://www.python.org', 
       packages=setuptools.find_packages(),
```

