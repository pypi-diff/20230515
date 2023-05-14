# Comparing `tmp/gmm_mi-0.4.3.tar.gz` & `tmp/gmm_mi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmm_mi-0.4.3.tar", last modified: Tue Jan 10 21:36:30 2023, max compression
+gzip compressed data, was "gmm_mi-0.5.0.tar", last modified: Mon Apr 24 10:26:43 2023, max compression
```

## Comparing `gmm_mi-0.4.3.tar` & `gmm_mi-0.5.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.939179 gmm_mi-0.4.3/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.4.3/LICENSE.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.4.3/LICENSE_EXT.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10538 2023-01-10 21:36:30.937179 gmm_mi-0.4.3/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     9963 2023-01-04 21:01:21.000000 gmm_mi-0.4.3/README.md
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.842179 gmm_mi-0.4.3/gmm_mi/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.4.3/gmm_mi/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.4.3/gmm_mi/cross_validation.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.872179 gmm_mi-0.4.3/gmm_mi/data/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.4.3/gmm_mi/data/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.4.3/gmm_mi/data/synthetic_data.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    22614 2023-01-04 21:00:55.000000 gmm_mi-0.4.3/gmm_mi/gmm.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.4.3/gmm_mi/initializations.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    44094 2023-01-10 21:34:56.000000 gmm_mi-0.4.3/gmm_mi/mi.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.4.3/gmm_mi/param_holders.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.4.3/gmm_mi/single_fit.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.928179 gmm_mi-0.4.3/gmm_mi/utils/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.4.3/gmm_mi/utils/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.4.3/gmm_mi/utils/analytic_MI.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.4.3/gmm_mi/utils/plotting.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.4.3/gmm_mi/utils/transformations.py
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.866179 gmm_mi-0.4.3/gmm_mi.egg-info/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10538 2023-01-10 21:36:30.000000 gmm_mi-0.4.3/gmm_mi.egg-info/PKG-INFO
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-01-10 21:36:30.000000 gmm_mi-0.4.3/gmm_mi.egg-info/SOURCES.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-01-10 21:36:30.000000 gmm_mi-0.4.3/gmm_mi.egg-info/dependency_links.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-01-10 21:36:30.000000 gmm_mi-0.4.3/gmm_mi.egg-info/requires.txt
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-01-10 21:36:30.000000 gmm_mi-0.4.3/gmm_mi.egg-info/top_level.txt
-drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-01-10 21:36:30.934179 gmm_mi-0.4.3/notebooks/
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.4.3/notebooks/__init__.py
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-01-10 21:36:30.940179 gmm_mi-0.4.3/setup.cfg
--rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-01-10 21:35:03.000000 gmm_mi-0.4.3/setup.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.936193 gmm_mi-0.5.0/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    35149 2022-08-06 22:31:49.000000 gmm_mi-0.5.0/LICENSE.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      625 2022-08-06 22:32:40.000000 gmm_mi-0.5.0/LICENSE_EXT.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10810 2023-04-24 10:26:43.924193 gmm_mi-0.5.0/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10235 2023-04-13 10:08:57.000000 gmm_mi-0.5.0/README.md
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.828193 gmm_mi-0.5.0/gmm_mi/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:00:35.000000 gmm_mi-0.5.0/gmm_mi/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     7226 2022-10-10 13:21:45.000000 gmm_mi-0.5.0/gmm_mi/cross_validation.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.863193 gmm_mi-0.5.0/gmm_mi/data/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-10 10:03:30.000000 gmm_mi-0.5.0/gmm_mi/data/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2823 2022-09-08 16:08:51.000000 gmm_mi-0.5.0/gmm_mi/data/synthetic_data.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    22614 2023-01-04 21:00:55.000000 gmm_mi-0.5.0/gmm_mi/gmm.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    12706 2022-10-10 13:23:09.000000 gmm_mi-0.5.0/gmm_mi/initializations.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    44094 2023-01-10 21:34:56.000000 gmm_mi-0.5.0/gmm_mi/mi.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2202 2023-01-04 21:01:21.000000 gmm_mi-0.5.0/gmm_mi/param_holders.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     2234 2022-10-10 13:21:54.000000 gmm_mi-0.5.0/gmm_mi/single_fit.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.909193 gmm_mi-0.5.0/gmm_mi/utils/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:25.000000 gmm_mi-0.5.0/gmm_mi/utils/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1852 2022-10-10 13:17:18.000000 gmm_mi-0.5.0/gmm_mi/utils/analytic_MI.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    29790 2023-01-04 21:01:21.000000 gmm_mi-0.5.0/gmm_mi/utils/plotting.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      929 2022-09-30 20:11:49.000000 gmm_mi-0.5.0/gmm_mi/utils/transformations.py
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.847193 gmm_mi-0.5.0/gmm_mi.egg-info/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)    10810 2023-04-24 10:26:43.000000 gmm_mi-0.5.0/gmm_mi.egg-info/PKG-INFO
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)      525 2023-04-24 10:26:43.000000 gmm_mi-0.5.0/gmm_mi.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        1 2023-04-24 10:26:43.000000 gmm_mi-0.5.0/gmm_mi.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       77 2023-04-24 10:26:43.000000 gmm_mi-0.5.0/gmm_mi.egg-info/requires.txt
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       17 2023-04-24 10:26:43.000000 gmm_mi-0.5.0/gmm_mi.egg-info/top_level.txt
+drwxrwxr-x   0 dpiras   (20025) dpiras   (20025)        0 2023-04-24 10:26:43.921193 gmm_mi-0.5.0/notebooks/
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)        0 2022-08-02 10:30:55.000000 gmm_mi-0.5.0/notebooks/__init__.py
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)       38 2023-04-24 10:26:43.937193 gmm_mi-0.5.0/setup.cfg
+-rw-rw-r--   0 dpiras   (20025) dpiras   (20025)     1153 2023-04-24 10:25:34.000000 gmm_mi-0.5.0/setup.py
```

### Comparing `gmm_mi-0.4.3/LICENSE.txt` & `gmm_mi-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/LICENSE_EXT.txt` & `gmm_mi-0.5.0/LICENSE_EXT.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/PKG-INFO` & `gmm_mi-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm_mi
-Version: 0.4.3
+Version: 0.5.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 
 # GMM-MI 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/25639122/195098930-93a9865b-a0c7-4792-9474-dc0d1056e358.png?raw=true" alt="GMM-MI_logo"/>
 </p>
 
-Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://arxiv.org/abs/2211.00024). Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
+Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://iopscience.iop.org/article/10.1088/2632-2153/acc444), published in Machine Learning: Science and Technology. Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
 
 ## Installation
 
 To install GMM-MI, follow these steps:
 1. (optional) `conda create -n gmm_mi python=3.9 jupyter` (create a custom `conda` environment with python 3.9) 
 2. (optional) `conda activate gmm_mi` (activate it)
 3. Install GMM-MI:
@@ -150,22 +150,28 @@
 ## Contributing and contacts
 
 Feel free to [fork](https://github.com/dpiras/GMM-MI/fork) this repository to work on it; otherwise, please [raise an issue](https://github.com/dpiras/GMM-MI/issues) or contact [Davide Piras](mailto:dr.davide.piras@gmail.com).
 
 ## Citation
 If you use GMM-MI, please cite the corresponding paper:
 
-     @article{Piras22, 
-          author = {Piras, Davide and Peiris, Hiranya V. and Pontzen, Andrew and Lucie-Smith, Luisa and Guo, Ningyuan and Nord, Brian},
+     @article{Piras23, 
+          author = {Davide Piras and Hiranya V Peiris and Andrew Pontzen and 
+                    Luisa Lucie-Smith and Ningyuan Guo and Brian Nord},
           title = {A robust estimator of mutual information for deep learning interpretability},
-          journal = {arXiv e-prints},
-          url = {https://arxiv.org/abs/2211.00024},
-          doi = {10.48550/ARXIV.2211.00024},
-          year = {2022}
-     }
+          journal = {Machine Learning: Science and Technology},
+          doi = {10.1088/2632-2153/acc444},
+          url = {https://dx.doi.org/10.1088/2632-2153/acc444},
+          year = {2023},
+          month = {apr},
+          publisher = {IOP Publishing},
+          volume = {4},
+          number = {2},
+          pages = {025006}
+    }
 
 ## License
 
 GMM-MI is released under the GPL-3 license - see [LICENSE](https://github.com/dpiras/GMM-MI/blob/main/LICENSE.txt)-, subject to 
 the non-commercial use condition - see [LICENSE_EXT](https://github.com/dpiras/GMM-MI/blob/main/LICENSE_EXT.txt).
 
      GMM-MI
```

### Comparing `gmm_mi-0.4.3/README.md` & `gmm_mi-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # GMM-MI 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/25639122/195098930-93a9865b-a0c7-4792-9474-dc0d1056e358.png?raw=true" alt="GMM-MI_logo"/>
 </p>
 
-Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://arxiv.org/abs/2211.00024). Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
+Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://iopscience.iop.org/article/10.1088/2632-2153/acc444), published in Machine Learning: Science and Technology. Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
 
 ## Installation
 
 To install GMM-MI, follow these steps:
 1. (optional) `conda create -n gmm_mi python=3.9 jupyter` (create a custom `conda` environment with python 3.9) 
 2. (optional) `conda activate gmm_mi` (activate it)
 3. Install GMM-MI:
@@ -134,22 +134,28 @@
 ## Contributing and contacts
 
 Feel free to [fork](https://github.com/dpiras/GMM-MI/fork) this repository to work on it; otherwise, please [raise an issue](https://github.com/dpiras/GMM-MI/issues) or contact [Davide Piras](mailto:dr.davide.piras@gmail.com).
 
 ## Citation
 If you use GMM-MI, please cite the corresponding paper:
 
-     @article{Piras22, 
-          author = {Piras, Davide and Peiris, Hiranya V. and Pontzen, Andrew and Lucie-Smith, Luisa and Guo, Ningyuan and Nord, Brian},
+     @article{Piras23, 
+          author = {Davide Piras and Hiranya V Peiris and Andrew Pontzen and 
+                    Luisa Lucie-Smith and Ningyuan Guo and Brian Nord},
           title = {A robust estimator of mutual information for deep learning interpretability},
-          journal = {arXiv e-prints},
-          url = {https://arxiv.org/abs/2211.00024},
-          doi = {10.48550/ARXIV.2211.00024},
-          year = {2022}
-     }
+          journal = {Machine Learning: Science and Technology},
+          doi = {10.1088/2632-2153/acc444},
+          url = {https://dx.doi.org/10.1088/2632-2153/acc444},
+          year = {2023},
+          month = {apr},
+          publisher = {IOP Publishing},
+          volume = {4},
+          number = {2},
+          pages = {025006}
+    }
 
 ## License
 
 GMM-MI is released under the GPL-3 license - see [LICENSE](https://github.com/dpiras/GMM-MI/blob/main/LICENSE.txt)-, subject to 
 the non-commercial use condition - see [LICENSE_EXT](https://github.com/dpiras/GMM-MI/blob/main/LICENSE_EXT.txt).
 
      GMM-MI
```

### Comparing `gmm_mi-0.4.3/gmm_mi/cross_validation.py` & `gmm_mi-0.5.0/gmm_mi/cross_validation.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/data/synthetic_data.py` & `gmm_mi-0.5.0/gmm_mi/data/synthetic_data.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/gmm.py` & `gmm_mi-0.5.0/gmm_mi/gmm.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/initializations.py` & `gmm_mi-0.5.0/gmm_mi/initializations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/mi.py` & `gmm_mi-0.5.0/gmm_mi/mi.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/param_holders.py` & `gmm_mi-0.5.0/gmm_mi/param_holders.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/single_fit.py` & `gmm_mi-0.5.0/gmm_mi/single_fit.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/utils/analytic_MI.py` & `gmm_mi-0.5.0/gmm_mi/utils/analytic_MI.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/utils/plotting.py` & `gmm_mi-0.5.0/gmm_mi/utils/plotting.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi/utils/transformations.py` & `gmm_mi-0.5.0/gmm_mi/utils/transformations.py`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/gmm_mi.egg-info/PKG-INFO` & `gmm_mi-0.5.0/gmm_mi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmm-mi
-Version: 0.4.3
+Version: 0.5.0
 Summary: Estimate mutual information distribution with Gaussian mixture models
 Home-page: https://github.com/dpiras/GMM-MI
 Author: Davide Piras
 Author-email: dr.davide.piras@gmail.com
 License: GNU General Public License v3.0 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -16,15 +16,15 @@
 
 # GMM-MI 
 
 <p align="center">
   <img src="https://user-images.githubusercontent.com/25639122/195098930-93a9865b-a0c7-4792-9474-dc0d1056e358.png?raw=true" alt="GMM-MI_logo"/>
 </p>
 
-Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://arxiv.org/abs/2211.00024). Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
+Welcome to GMM-MI (pronounced ``Jimmie``)! This package allows you to calculate mutual information (MI) with its associated uncertainty, combining Gaussian mixture models (GMMs) and bootstrap. GMM-MI is accurate, computationally efficient and fully in python; you can read more about GMM-MI [in our paper](https://iopscience.iop.org/article/10.1088/2632-2153/acc444), published in Machine Learning: Science and Technology. Please [cite it](#citation) if you use it in your work! Check out also the [poster accepted at the Machine Learning and the Physical Sciences workshop at NeurIPS 2022](https://neurips.cc/media/PosterPDFs/NeurIPS%202022/56922.png), and the accompanying [video](https://user-images.githubusercontent.com/25639122/201700436-3c3f6216-1925-4a09-9b04-419a64bfda15.mp4).
 
 ## Installation
 
 To install GMM-MI, follow these steps:
 1. (optional) `conda create -n gmm_mi python=3.9 jupyter` (create a custom `conda` environment with python 3.9) 
 2. (optional) `conda activate gmm_mi` (activate it)
 3. Install GMM-MI:
@@ -150,22 +150,28 @@
 ## Contributing and contacts
 
 Feel free to [fork](https://github.com/dpiras/GMM-MI/fork) this repository to work on it; otherwise, please [raise an issue](https://github.com/dpiras/GMM-MI/issues) or contact [Davide Piras](mailto:dr.davide.piras@gmail.com).
 
 ## Citation
 If you use GMM-MI, please cite the corresponding paper:
 
-     @article{Piras22, 
-          author = {Piras, Davide and Peiris, Hiranya V. and Pontzen, Andrew and Lucie-Smith, Luisa and Guo, Ningyuan and Nord, Brian},
+     @article{Piras23, 
+          author = {Davide Piras and Hiranya V Peiris and Andrew Pontzen and 
+                    Luisa Lucie-Smith and Ningyuan Guo and Brian Nord},
           title = {A robust estimator of mutual information for deep learning interpretability},
-          journal = {arXiv e-prints},
-          url = {https://arxiv.org/abs/2211.00024},
-          doi = {10.48550/ARXIV.2211.00024},
-          year = {2022}
-     }
+          journal = {Machine Learning: Science and Technology},
+          doi = {10.1088/2632-2153/acc444},
+          url = {https://dx.doi.org/10.1088/2632-2153/acc444},
+          year = {2023},
+          month = {apr},
+          publisher = {IOP Publishing},
+          volume = {4},
+          number = {2},
+          pages = {025006}
+    }
 
 ## License
 
 GMM-MI is released under the GPL-3 license - see [LICENSE](https://github.com/dpiras/GMM-MI/blob/main/LICENSE.txt)-, subject to 
 the non-commercial use condition - see [LICENSE_EXT](https://github.com/dpiras/GMM-MI/blob/main/LICENSE_EXT.txt).
 
      GMM-MI
```

### Comparing `gmm_mi-0.4.3/gmm_mi.egg-info/SOURCES.txt` & `gmm_mi-0.5.0/gmm_mi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmm_mi-0.4.3/setup.py` & `gmm_mi-0.5.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 PACKAGENAME = 'gmm_mi'
 
 setup(
     name='gmm_mi',
-    version="0.4.3",
+    version="0.5.0",
     author='Davide Piras',
     author_email='dr.davide.piras@gmail.com',
     description='Estimate mutual information distribution with Gaussian mixture models',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/dpiras/GMM-MI',
     license='GNU General Public License v3.0 (GPLv3)',
```

