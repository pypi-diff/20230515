# Comparing `tmp/lpdensity-2.3.1.tar.gz` & `tmp/lpdensity-2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lpdensity-2.3.1.tar", last modified: Fri May 27 13:35:53 2022, max compression
+gzip compressed data, was "lpdensity-2.4.tar", last modified: Mon Jan 23 19:02:10 2023, max compression
```

## Comparing `lpdensity-2.3.1.tar` & `lpdensity-2.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-27 13:35:53.355866 lpdensity-2.3.1/
--rw-r--r--   0 rajitachandak   (501) staff       (20)     2455 2022-05-27 13:35:53.355928 lpdensity-2.3.1/PKG-INFO
--rw-r--r--   0 rajitachandak   (501) staff       (20)     1897 2022-05-26 17:54:00.000000 lpdensity-2.3.1/README.md
--rw-r--r--   0 rajitachandak   (501) staff       (20)      104 2022-05-26 17:54:00.000000 lpdensity-2.3.1/pyproject.toml
--rw-r--r--   0 rajitachandak   (501) staff       (20)      764 2022-05-27 13:35:53.356209 lpdensity-2.3.1/setup.cfg
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-27 13:35:53.353805 lpdensity-2.3.1/src/
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-27 13:35:53.355111 lpdensity-2.3.1/src/lpdensity/
--rw-r--r--   0 rajitachandak   (501) staff       (20)       70 2022-05-26 17:54:00.000000 lpdensity-2.3.1/src/lpdensity/__init__.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    10783 2022-05-26 17:54:00.000000 lpdensity-2.3.1/src/lpdensity/lpbwdensity.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    28112 2022-05-26 17:54:00.000000 lpdensity-2.3.1/src/lpdensity/lpbwdensity_fn.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)    21665 2022-05-26 17:54:00.000000 lpdensity-2.3.1/src/lpdensity/lpdensity.py
--rw-r--r--   0 rajitachandak   (501) staff       (20)     8987 2022-05-26 17:54:00.000000 lpdensity-2.3.1/src/lpdensity/lpdensity_fn.py
-drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2022-05-27 13:35:53.355757 lpdensity-2.3.1/src/lpdensity.egg-info/
--rw-r--r--   0 rajitachandak   (501) staff       (20)     2455 2022-05-27 13:35:53.000000 lpdensity-2.3.1/src/lpdensity.egg-info/PKG-INFO
--rw-r--r--   0 rajitachandak   (501) staff       (20)      362 2022-05-27 13:35:53.000000 lpdensity-2.3.1/src/lpdensity.egg-info/SOURCES.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)        1 2022-05-27 13:35:53.000000 lpdensity-2.3.1/src/lpdensity.egg-info/dependency_links.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)       34 2022-05-27 13:35:53.000000 lpdensity-2.3.1/src/lpdensity.egg-info/requires.txt
--rw-r--r--   0 rajitachandak   (501) staff       (20)       10 2022-05-27 13:35:53.000000 lpdensity-2.3.1/src/lpdensity.egg-info/top_level.txt
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-23 19:02:10.048410 lpdensity-2.4/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3773 2023-01-23 19:02:10.048478 lpdensity-2.4/PKG-INFO
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3217 2023-01-23 18:49:09.000000 lpdensity-2.4/README.md
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      104 2022-12-31 06:54:46.000000 lpdensity-2.4/pyproject.toml
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      762 2023-01-23 19:02:10.048771 lpdensity-2.4/setup.cfg
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-23 19:02:10.045736 lpdensity-2.4/src/
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-23 19:02:10.047581 lpdensity-2.4/src/lpdensity/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)       70 2022-12-31 06:54:46.000000 lpdensity-2.4/src/lpdensity/__init__.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    10783 2022-12-31 06:54:46.000000 lpdensity-2.4/src/lpdensity/lpbwdensity.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    28112 2022-12-31 06:54:46.000000 lpdensity-2.4/src/lpdensity/lpbwdensity_fn.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)    21665 2022-12-31 06:54:46.000000 lpdensity-2.4/src/lpdensity/lpdensity.py
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     8987 2022-12-31 06:54:46.000000 lpdensity-2.4/src/lpdensity/lpdensity_fn.py
+drwxr-xr-x   0 rajitachandak   (501) staff       (20)        0 2023-01-23 19:02:10.048295 lpdensity-2.4/src/lpdensity.egg-info/
+-rw-r--r--   0 rajitachandak   (501) staff       (20)     3773 2023-01-23 19:02:10.000000 lpdensity-2.4/src/lpdensity.egg-info/PKG-INFO
+-rw-r--r--   0 rajitachandak   (501) staff       (20)      362 2023-01-23 19:02:10.000000 lpdensity-2.4/src/lpdensity.egg-info/SOURCES.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)        1 2023-01-23 19:02:10.000000 lpdensity-2.4/src/lpdensity.egg-info/dependency_links.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)       34 2023-01-23 19:02:10.000000 lpdensity-2.4/src/lpdensity.egg-info/requires.txt
+-rw-r--r--   0 rajitachandak   (501) staff       (20)       10 2023-01-23 19:02:10.000000 lpdensity-2.4/src/lpdensity.egg-info/top_level.txt
```

### Comparing `lpdensity-2.3.1/PKG-INFO` & `lpdensity-2.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: lpdensity
-Version: 2.3.1
-Summary: Implements local polynomial point estimation with robust bias-corrected uniform confidence intervals.
-Home-page: https://github.com/nppackages/lpdensity
-Author: Rajita Chandak
-Author-email: rchandak@princeton.edu
-Project-URL: Bug Tracker, https://github.com/nppackages/lpdensity/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 # LPDENSITY
 
 The `lpdensity` package provides Stata and R implementations of bandwidth selection, point estimation and inference procedures for local polynomial distribution and density methods.
 
 This work was supported by the National Science Foundation through grant SES-1459931, SES-1459967, SES-1947805 and SES-1947662.
 
 ## Authors
@@ -28,16 +14,16 @@
 
 Rajita Chandak (maintainer) (<rchandak@princeton.edu>)
 
 ## Website
 
 https://nppackages.github.io/lpdensity/
 
-## ReadTheDocs Manual
-https://lpdensity.readthedocs.io/en/latest/
+## Manual
+https://github.com/nppackages/lpdensity/tree/master/Python/lpdensity/docs/build/latex/lpdensity.pdf
 
 ## Installation
 To install/update use pip
 ```
 pip install lpdensity
 ```
 
@@ -46,29 +32,45 @@
 from lpdensity import lpdensity, lpbwdensity
 ```
 ## Dependencies
 - numpy
 - pandas
 - math
 - scipy
+- sympy
 - plotnine
 
 ## References
 
 For overviews and introductions, see [lpdensity website](https://nppackages.github.io/lpdensity/)
 
-### Software Implementation
+### Software and Implementation
 
--Cattaneo, Jansson and Ma (2021): [lpdensity: Local Polynomial Density Estimation and Inference.](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JSS.pdf). <br>
-Journal of Statistical Software, forthcoming.
+- Cattaneo, Jansson and Ma (2022): [lpdensity: Local Polynomial Density Estimation and Inference](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JSS.pdf).<br>
+_Journal of Statistical Software_ 101(2): 1-25.
 
 ### Technical and Methodological
 
-- Cattaneo, Jansson and Ma (2020): [Simple Local Polynomial Density Estimators.](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
-Journal of the American Statistical Association 115(531): 1449-1455.
-[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA--Supplement.pdf).
-
-- Cattaneo, Jansson and Ma (2021): [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JoE.pdf).<br>
-Journal of Econometrics, forthcoming.<br>
-[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JoE--Supplement.pdf).
+- Cattaneo, Jansson and Ma (2020): [Simple Local Polynomial Density Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
+_Journal of the American Statistical Association_ 115(531): 1449-1455.<br>
+[Supplemental appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA--Supplement.pdf).
+
+- Cattaneo, Jansson and Ma (2022): [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JoE.pdf).<br>
+_Journal of Econometrics_, forthcoming.<br>
+[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JoE--Supplement.pdf).
+
+- Calonico, S., M. D. Cattaneo, and M. H. Farrell (2018): [On the Effect of Bias Estimation on Coverage Accuracy in Nonparametric Inference](https://nppackages.github.io/references/Calonico-Cattaneo-Farrell_2018_JASA.pdf).<br>
+_Journal of the American Statistical Association_ 113(522): 767-779.
+
+- Calonico, S., M. D. Cattaneo, and M. H. Farrell (2022): [Coverage Error Optimal Confidence Intervals for Local Polynomial Regression](https://cattaneo.princeton.edu/papers/Calonico-Cattaneo-Farrell_2022_Bernoulli.pdf).<br>
+_Bernoulli_ 28(4): 2998-3022.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2020). [Simple Local Polynomial Density Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
+_Journal of the American Statistical Association_, 115(531): 1449-1455.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2022). [lpdensity: Local Polynomial Density Estimation and Inference](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JSS.pdf). <br>
+_Journal of Statistical Software_, 101(2), 1–25.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2023). [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2023_JoE.pdf). <br>
+_Journal of Econometrics_, forthcoming.
 
-<br><br> 
+<br><br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `lpdensity-2.3.1/setup.cfg` & `lpdensity-2.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = lpdensity
-version = 2.3.1
+version = 2.4
 author = Rajita Chandak
 author_email = rchandak@princeton.edu
 description = Implements local polynomial point estimation with robust bias-corrected uniform confidence intervals.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nppackages/lpdensity
 project_urls =
```

### Comparing `lpdensity-2.3.1/src/lpdensity/lpbwdensity.py` & `lpdensity-2.4/src/lpdensity/lpbwdensity.py`

 * *Files identical despite different names*

### Comparing `lpdensity-2.3.1/src/lpdensity/lpbwdensity_fn.py` & `lpdensity-2.4/src/lpdensity/lpbwdensity_fn.py`

 * *Files identical despite different names*

### Comparing `lpdensity-2.3.1/src/lpdensity/lpdensity.py` & `lpdensity-2.4/src/lpdensity/lpdensity.py`

 * *Files identical despite different names*

### Comparing `lpdensity-2.3.1/src/lpdensity/lpdensity_fn.py` & `lpdensity-2.4/src/lpdensity/lpdensity_fn.py`

 * *Files identical despite different names*

### Comparing `lpdensity-2.3.1/src/lpdensity.egg-info/PKG-INFO` & `lpdensity-2.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lpdensity
-Version: 2.3.1
+Version: 2.4
 Summary: Implements local polynomial point estimation with robust bias-corrected uniform confidence intervals.
 Home-page: https://github.com/nppackages/lpdensity
 Author: Rajita Chandak
 Author-email: rchandak@princeton.edu
 Project-URL: Bug Tracker, https://github.com/nppackages/lpdensity/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -28,16 +28,16 @@
 
 Rajita Chandak (maintainer) (<rchandak@princeton.edu>)
 
 ## Website
 
 https://nppackages.github.io/lpdensity/
 
-## ReadTheDocs Manual
-https://lpdensity.readthedocs.io/en/latest/
+## Manual
+https://github.com/nppackages/lpdensity/tree/master/Python/lpdensity/docs/build/latex/lpdensity.pdf
 
 ## Installation
 To install/update use pip
 ```
 pip install lpdensity
 ```
 
@@ -46,29 +46,45 @@
 from lpdensity import lpdensity, lpbwdensity
 ```
 ## Dependencies
 - numpy
 - pandas
 - math
 - scipy
+- sympy
 - plotnine
 
 ## References
 
 For overviews and introductions, see [lpdensity website](https://nppackages.github.io/lpdensity/)
 
-### Software Implementation
+### Software and Implementation
 
--Cattaneo, Jansson and Ma (2021): [lpdensity: Local Polynomial Density Estimation and Inference.](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JSS.pdf). <br>
-Journal of Statistical Software, forthcoming.
+- Cattaneo, Jansson and Ma (2022): [lpdensity: Local Polynomial Density Estimation and Inference](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JSS.pdf).<br>
+_Journal of Statistical Software_ 101(2): 1-25.
 
 ### Technical and Methodological
 
-- Cattaneo, Jansson and Ma (2020): [Simple Local Polynomial Density Estimators.](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
-Journal of the American Statistical Association 115(531): 1449-1455.
-[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA--Supplement.pdf).
-
-- Cattaneo, Jansson and Ma (2021): [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JoE.pdf).<br>
-Journal of Econometrics, forthcoming.<br>
-[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2021_JoE--Supplement.pdf).
+- Cattaneo, Jansson and Ma (2020): [Simple Local Polynomial Density Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
+_Journal of the American Statistical Association_ 115(531): 1449-1455.<br>
+[Supplemental appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA--Supplement.pdf).
 
-<br><br> 
+- Cattaneo, Jansson and Ma (2022): [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JoE.pdf).<br>
+_Journal of Econometrics_, forthcoming.<br>
+[Supplemental Appendix](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JoE--Supplement.pdf).
+
+- Calonico, S., M. D. Cattaneo, and M. H. Farrell (2018): [On the Effect of Bias Estimation on Coverage Accuracy in Nonparametric Inference](https://nppackages.github.io/references/Calonico-Cattaneo-Farrell_2018_JASA.pdf).<br>
+_Journal of the American Statistical Association_ 113(522): 767-779.
+
+- Calonico, S., M. D. Cattaneo, and M. H. Farrell (2022): [Coverage Error Optimal Confidence Intervals for Local Polynomial Regression](https://cattaneo.princeton.edu/papers/Calonico-Cattaneo-Farrell_2022_Bernoulli.pdf).<br>
+_Bernoulli_ 28(4): 2998-3022.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2020). [Simple Local Polynomial Density Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2020_JASA.pdf).<br>
+_Journal of the American Statistical Association_, 115(531): 1449-1455.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2022). [lpdensity: Local Polynomial Density Estimation and Inference](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2022_JSS.pdf). <br>
+_Journal of Statistical Software_, 101(2), 1–25.
+
+- Cattaneo, M. D., M. Jansson, and X. Ma (2023). [Local Regression Distribution Estimators](https://nppackages.github.io/references/Cattaneo-Jansson-Ma_2023_JoE.pdf). <br>
+_Journal of Econometrics_, forthcoming.
+
+<br><br>
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

