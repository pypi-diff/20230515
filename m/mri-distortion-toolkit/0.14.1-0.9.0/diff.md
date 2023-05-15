# Comparing `tmp/mri_distortion_toolkit-0.14.1.tar.gz` & `tmp/mri_distortion_toolkit-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mri_distortion_toolkit-0.14.1.tar", last modified: Mon May 15 04:49:12 2023, max compression
+gzip compressed data, was "mri_distortion_toolkit-0.9.0.tar", last modified: Thu Sep  1 04:26:41 2022, max compression
```

## Comparing `mri_distortion_toolkit-0.14.1.tar` & `mri_distortion_toolkit-0.9.0.tar`

### file list

```diff
@@ -1,35 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)    33359 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/DistortionCorrection.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/FieldCalculation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18369 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/Harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)    64330 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/MarkerAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/PhantomDesigner.py
--rw-r--r--   0 runner    (1001) docker     (123)    29556 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/Reports.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/calculate_harmonics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/MR_report.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/themes/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/themes/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/themes/d42ker-github.css
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/themes/whitey.css
--rw-r--r--   0 runner    (1001) docker     (123)    38542 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3004 2023-05-15 04:49:12.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 04:49:12.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 04:49:12.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-15 04:49:12.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 04:49:12.000000 mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-15 04:49:12.241343 mri_distortion_toolkit-0.14.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 04:49:12.237343 mri_distortion_toolkit-0.14.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_FieldCalculation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_MarkerAnalysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_PhantomDesigner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_distortion_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_harmonics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-15 04:48:58.000000 mri_distortion_toolkit-0.14.1/tests/test_utilities.py
+drwxrwxrwx   0        0        0        0 2022-09-01 04:26:41.909050 mri_distortion_toolkit-0.9.0/
+-rw-rw-rw-   0        0        0     3244 2022-09-01 04:26:41.909547 mri_distortion_toolkit-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2654 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-09-01 04:26:41.843049 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/
+-rw-rw-rw-   0        0        0    21259 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/DistortionCorrection.py
+-rw-rw-rw-   0        0        0     5817 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/FieldCalculation.py
+-rw-rw-rw-   0        0        0    17570 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/Harmonics.py
+-rw-rw-rw-   0        0        0    58798 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/MarkerAnalysis.py
+-rw-rw-rw-   0        0        0    29999 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/Reports.py
+-rw-rw-rw-   0        0        0      290 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/__init__.py
+-rw-rw-rw-   0        0        0     2795 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/calculate_harmonics.py
+drwxrwxrwx   0        0        0        0 2022-09-01 04:26:41.846052 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/
+-rw-rw-rw-   0        0        0     1984 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/MR_report.html
+drwxrwxrwx   0        0        0        0 2022-09-01 04:26:41.853047 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/themes/
+-rw-rw-rw-   0        0        0      221 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/themes/README.md
+-rw-rw-rw-   0        0        0    11866 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/themes/d42ker-github.css
+-rw-rw-rw-   0        0        0     4528 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/themes/whitey.css
+-rw-rw-rw-   0        0        0    30295 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/utilities.py
+drwxrwxrwx   0        0        0        0 2022-09-01 04:26:41.905552 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/
+-rw-rw-rw-   0        0        0     3244 2022-09-01 04:26:41.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2022-09-01 04:26:41.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-09-01 04:26:41.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2022-09-01 04:26:41.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2022-09-01 04:26:41.000000 mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-09-01 04:21:42.000000 mri_distortion_toolkit-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1278 2022-09-01 04:26:41.920547 mri_distortion_toolkit-0.9.0/setup.cfg
```

### Comparing `mri_distortion_toolkit-0.14.1/PKG-INFO` & `mri_distortion_toolkit-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-Metadata-Version: 2.1
-Name: mri_distortion_toolkit
-Version: 0.14.1
-Summary: Quality assurance tools for MRI geometric distortion
-Home-page: https://acrf-image-x-institute.github.io/mri_distortion_toolkit/index.html
-Author: Brendan Whelan, Paul Liu, Shanshan Shan
-Author-email: bwheelz360@gmail.com
-Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/mri_distortion_toolkit
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# mri_distortion_toolkit  
-[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)[![PyPI version](https://badge.fury.io/py/mri_distortion_toolkit.svg)](https://badge.fury.io/py/mri_distortion_toolkit)
-
-This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging.
-
-The workflow steps are below. All steps have well defined input/output so you can use any part of this code independently from the other parts. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
-
-```mermaid
-flowchart LR
-
-AA[Phantom Design]
-
-A[Marker <br>Extraction]--->B[Marker <br>Matching]
-B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
-C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
-D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
-D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
-
-click AA "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/phantom_notes.html"
-click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_extraction.html"
-click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_matching.html"
-click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/field_calculation.html"
-click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/fit_spherical_harmonics.html"
-click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/reporting.html"
-```
-
-
-
-## Setup/Build/Install
-
-```bash
-pip install mri_distortion_toolkit
-```
-
-## Usage
-
-Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
-
-## Directory Structure
-
-- *docsrc* markdown/rst source documentation
-- *tests* test cases
-- *mri_distortion_toolkit* source code 
-- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
+Metadata-Version: 2.1
+Name: mri_distortion_toolkit
+Version: 0.9.0
+Summary: Quality assurance tools for MRI geometric distortion
+Home-page: https://acrf-image-x-institute.github.io/mri_distortion_toolkit/index.html
+Author: Brendan Whelan, Paul Liu, Shanshan Shan
+Author-email: bwheelz360@gmail.com
+Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/mri_distortion_toolkit
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# mri_distortion_toolkit  
+
+[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)
+
+This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging. 
+
+For the measurement of such distortions, see [here](https://github.com/ACRF-Image-X-Institute/MRI_DistortionPhantom). 
+
+The workflow steps are below, but all steps have well defined input/output so you can use any part of this code independently from the other parts. For a tutorial on each step, click on the diagram below. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
+
+```mermaid
+flowchart LR
+    A[Marker <br>Extraction]--->B[Marker <br>Matching]
+    B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
+    C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
+    D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
+    D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
+
+    click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MarkerVolume"
+    click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes"
+    click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldCalculation.ConvertMatchedMarkersToBz"
+    click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldAnalysis.SphericalHarmonicFit"
+    click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.Reports.MRI_QA_Reporter"
+
+```
+
+## Setup/Build/Install
+
+```bash
+pip install mri_distortion_toolkit
+```
+
+
+## Usage
+
+Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
+
+## Directory Structure
+
+- *docsrc* markdown/rst source documentation
+- *tests* test cases
+- *MRI_DistortionQA* source code
+- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
```

### Comparing `mri_distortion_toolkit-0.14.1/README.md` & `mri_distortion_toolkit-0.9.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,43 @@
-# mri_distortion_toolkit  
-[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)[![PyPI version](https://badge.fury.io/py/mri_distortion_toolkit.svg)](https://badge.fury.io/py/mri_distortion_toolkit)
-
-This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging.
-
-The workflow steps are below. All steps have well defined input/output so you can use any part of this code independently from the other parts. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
-
-```mermaid
-flowchart LR
-
-AA[Phantom Design]
-
-A[Marker <br>Extraction]--->B[Marker <br>Matching]
-B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
-C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
-D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
-D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
-
-click AA "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/phantom_notes.html"
-click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_extraction.html"
-click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_matching.html"
-click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/field_calculation.html"
-click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/fit_spherical_harmonics.html"
-click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/reporting.html"
-```
-
-
-
-## Setup/Build/Install
-
-```bash
-pip install mri_distortion_toolkit
-```
-
-## Usage
-
-Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
-
-## Directory Structure
-
-- *docsrc* markdown/rst source documentation
-- *tests* test cases
-- *mri_distortion_toolkit* source code 
-- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
+# mri_distortion_toolkit  
+
+[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)
+
+This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging. 
+
+For the measurement of such distortions, see [here](https://github.com/ACRF-Image-X-Institute/MRI_DistortionPhantom). 
+
+The workflow steps are below, but all steps have well defined input/output so you can use any part of this code independently from the other parts. For a tutorial on each step, click on the diagram below. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
+
+```mermaid
+flowchart LR
+    A[Marker <br>Extraction]--->B[Marker <br>Matching]
+    B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
+    C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
+    D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
+    D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
+
+    click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MarkerVolume"
+    click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes"
+    click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldCalculation.ConvertMatchedMarkersToBz"
+    click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldAnalysis.SphericalHarmonicFit"
+    click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.Reports.MRI_QA_Reporter"
+
+```
+
+## Setup/Build/Install
+
+```bash
+pip install mri_distortion_toolkit
+```
+
+
+## Usage
+
+Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
+
+## Directory Structure
+
+- *docsrc* markdown/rst source documentation
+- *tests* test cases
+- *MRI_DistortionQA* source code
+- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/DistortionCorrection.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/DistortionCorrection.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,720 +1,461 @@
-import math
-import os
-import logging
-import sys
-import warnings
-import pydicom
-import matplotlib.pyplot as plt
-from matplotlib.patches import Circle
-from finufft import Plan
-from finufft import nufft2d1, nufft2d2
-import numpy as np
-from scipy.fft import fft2
-from scipy.fft import fftshift
-from scipy.sparse.linalg import lsqr
-from scipy.sparse.linalg import LinearOperator
-from scipy.interpolate import RectBivariateSpline
-import pandas as pd
-from pathlib import Path
-from .utilities import get_all_files, convert_cartesian_to_spherical, generate_legendre_basis, dicom_to_numpy
-from .utilities import sort_dicom_slices
-from .utilities import get_harmonics
-from .utilities import printProgressBar
-from time import perf_counter
-from abc import abstractmethod
-from .utilities import combine_harmonics
-
-logging.basicConfig(format='[%(filename)s: line %(lineno)d] %(message)s', level=logging.WARNING)
-logger = logging.getLogger(__name__)
-
-
-class DistortionCorrectorBase:
-    """
-    This is the base class which other distortion correction methods can inherit from, and includes the core required
-    behavior.
-
-    :param ImageDirectory: Directory containing images to correct. Note that all images matching ImExtension will be
-        read in; therefore only one series should be inside ImageDirectory (we dont check this!)
-    :type ImageDirectory: pathlib.Path or str
-    :param gradient_harmonics: a list of three harmonics, which should either be csv files exported from an instance of
-        SphericalHarmonicFit, or SphericalHarmonicFit.harmonics
-    :type gradient_harmonics: list
-    :param B0_harmonics: Instance of SphericalHarmonicFit.harmonics describing B0, or else an equivalent csv file
-    :type B0_harmonics: SphericalHarmonicFit.harmonics or csv, optional
-    :param ImExtension: extension of files to read in ImageDirectory, e.g. 'dcm', or 'IMA'
-    :type ImExtension: str, optional
-    :param correct_through_plane: if True, through plane (3D) correction is carried out, which is roughly twice as slow
-        as 2D only
-    :type correct_through_plane: bool. optional
-    :param correct_B0: if True, and if B0_harmonics is supplied, will also correct for B0 effects. Probably only works
-        for standard (non EPI) sequences.
-    :type correct_B0: bool, optional
-    :param B0_direction: 'forward' or 'back'. Determines whether the B0 harmonics should be added (forward) or
-        subtracted (backward) from the gradient harmonics
-    :type B0_direction: str, optional
-    :param pad: pixels to 0 pad image volume. This can be useful in the k-space domain
-    :type pad: int, optional
-    """
-
-    def __init__(self, ImageDirectory, gradient_harmonics, B0_harmonics=None,
-                 dicom_data=None,
-                 ImExtension='.dcm', correct_through_plane=True, correct_B0=False,
-                 B0_direction='forward', pad=0):
-        """
-        init method
-        """
-
-        if 'DistortionCorrectorBase' in str(self.__class__):
-            raise TypeError('DistortionCorrectorBase should not be called directly; it only exists for other correctors'
-                            'to inherit. Quitting')
-
-        self.correct_through_plane = correct_through_plane
-        self.correct_B0 = correct_B0
-        self.B0_direction = B0_direction
-        self._n_zero_pad = pad  # n_pixels to add around each edge of volume. set to 0 for no zero padding
-        self._Gx_Harmonics, self._Gy_Harmonics, self._Gz_Harmonics, self._B0_Harmonics = \
-            get_harmonics(gradient_harmonics[0], gradient_harmonics[1], gradient_harmonics[2], B0_harmonics)
-        self._Gx_Harmonics = self._Gx_Harmonics * 1
-        self._Gy_Harmonics = self._Gy_Harmonics * 1
-        self._Gz_Harmonics = self._Gz_Harmonics * 1
-        self._dicom_data = dicom_data
-
-        if self.correct_B0:
-            if self._B0_Harmonics is None:
-                warnings.warn('cannot correct B0 as no B0 harmonics supplied, continuing')
-            else:
-                self._add_B0_to_gradient()
-
-        self.ImageDirectory = Path(ImageDirectory)
-        self._all_dicom_files = get_all_files(self.ImageDirectory, ImExtension)
-        CompletePathFiles = [self.ImageDirectory / file for file in self._all_dicom_files]
-        dicom_slices = [pydicom.read_file(f) for f in CompletePathFiles]
-        sort_ind = sort_dicom_slices(dicom_slices)[1]
-        self._all_dicom_files = list(np.array(self._all_dicom_files)[sort_ind])
-        self._n_dicom_files = len(self._all_dicom_files)
-
-        self.ImageArray, \
-        self._dicom_affine, \
-        (self._X, self._Y, self._Z) = dicom_to_numpy(self.ImageDirectory,
-                                                     file_extension=ImExtension,
-                                                     return_XYZ=True,
-                                                     zero_pad=self._n_zero_pad,
-                                                     enforce_increasing_coords=False)
-        self._get_rows_and_cols()
-        self._get_iso_offset()
-        self.n_order = int(np.sqrt(self._Gx_Harmonics.size) - 1)
-        self.Images = get_all_files(self.ImageDirectory, ImExtension)
-        self.r_DSV = 150  # only for drawing on the plot
-        self._check_input_data()
-
-    @abstractmethod
-    def _correct_image(self):
-        """
-        This is the method to correct a 2D slice of data; each inheriting corrector must supply its own _correct_image
-        method.
-        """
-        pass
-
-    def _get_rows_and_cols(self):
-        """
-        just extract the number of rows and columns from a dicom header - we need it for zero padding later.
-        I suspect I should be able to derive this from the dicom affine, but this way seems more foolproof
-        """
-        demo_header = pydicom.read_file(self.ImageDirectory / self._all_dicom_files[0])
-        self._Rows, self._Cols, self._Slices = self.ImageArray.shape
-        self._ImageOrientationPatient = demo_header.ImageOrientationPatient
-        self._pixel_spacing = self._dicom_affine[0:3, 0:3].sum(1)
-        self._pixel_spacing = [ps if not ps == 0 else np.nan for ps in self._pixel_spacing]
-
-    def _get_iso_offset(self):
-        """
-        calculate the offset between the center of the volume and scanner isocenter.
-        This offset is used in _calculate_encoding_indices
-        """
-        self._image_position_patient_start = [self._X[0, 0, 0], self._Y[0, 0, 0], self._Z[0, 0, 0]]
-        assert np.allclose(self._image_position_patient_start, self._dicom_affine[0:3, 3])
-        self._image_position_patient_end = [self._X[-1, -1, -1], self._Y[-1, -1, -1], self._Z[-1, -1, -1]]
-        self._iso_offset = -1 * np.add(self._image_position_patient_end, self._image_position_patient_start) / 2
-        pixel_spacing = self._dicom_affine[0:3, 0:3].sum(1)
-        self._iso_offset_pixels = np.divide(self._iso_offset, self._pixel_spacing)
-
-    def _check_input_data(self):
-        """
-        Put any tests of input data here
-        """
-        assert self._Gx_Harmonics.shape == self._Gy_Harmonics.shape == self._Gz_Harmonics.shape
-        assert self._n_zero_pad >= 0
-
-    def _add_B0_to_gradient(self):
-        """
-        combine the B0 harmonics with the gradient harmonics in the frequency encode direciton
-        :return:
-        """
-
-        assert self.B0_direction == 'forward' or self.B0_direction == 'back'
-        if self.B0_direction == 'forward':
-            _operation = 'add'
-        elif self.B0_direction == 'back':
-            _operation = 'subtract'
-        else:
-            raise TypeError('B0_direction must be "forward" or "back"')
-
-        try:
-            freq_encode_direction = self._dicom_data['freq_encode_direction']
-            _test = self._dicom_data['gradient_strength']
-        except (AttributeError, TypeError):
-            raise AttributeError('Cannot combine gradient and B0 harmonics as no dicom_data was supplied. '
-                           'At a minimum, we need the following: '
-                           'dicom_data = {"freq_encode_direction": e.g. "x",'
-                           '              "gradient_strength": e.g. [1,2,3]}'
-                           'continuing with just the supplied gradient harmonics')
-            
-        if freq_encode_direction == 'x':
-            gradient_order = int(np.sqrt(self._Gx_Harmonics.shape[0] - 1))
-            scale = 1/self._dicom_data['gradient_strength'][0]
-            self._Gx_Harmonics = combine_harmonics(self._Gx_Harmonics, self._B0_Harmonics*scale, operation=_operation,
-                                                   n_order_return=gradient_order)
-        elif freq_encode_direction == 'y':
-            gradient_order = int(np.sqrt(self._Gy_Harmonics.shape[0] - 1))
-            scale = 1 / self._dicom_data['gradient_strength'][1]
-            self._Gy_Harmonics = combine_harmonics(self._Gy_Harmonics, self._B0_Harmonics*scale, operation=_operation,
-                                                   n_order_return=gradient_order)
-        elif freq_encode_direction == 'z':
-            gradient_order = int(np.sqrt(self._Gz_Harmonics.shape[0] - 1))
-            scale = 1 / self._dicom_data['gradient_strength'][2]
-            self._Gz_Harmonics = combine_harmonics(self._Gz_Harmonics, self._B0_Harmonics*scale, operation=_operation,
-                                                   n_order_return=gradient_order)
-
-        # from .Harmonics import SphericalHarmonicFit
-        # input_data = pd.DataFrame({'x': [0, 0, 0], 'y': [0, 0, 0], 'z': [0, 0, 0], 'Bz': [0, 1, 2]})
-        # tempH = SphericalHarmonicFit(input_data)
-        # tempH.harmonics = self._Gx_Harmonics
-        # tempH._assess_harmonic_pk_pk()
-        # tempH.plot_harmonics_pk_pk(cut_off=.005)
-
-    def _unpad_image_arrays(self):
-        """
-        remove any zero padding from original and reconstructed image volumes
-        """
-        if self._n_zero_pad > 0:
-            self.ImageArray = self.ImageArray[self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad]
-            self._image_array_corrected = self._image_array_corrected[self._n_zero_pad:-self._n_zero_pad,
-                                          self._n_zero_pad:-self._n_zero_pad,
-                                          self._n_zero_pad:-self._n_zero_pad]
-            self._X = self._X[self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad]
-            self._Y = self._Y[self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad]
-            self._Z = self._Z[self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad,
-                              self._n_zero_pad:-self._n_zero_pad]
-
-    def _calculate_encoding_fields(self):
-        """
-        Based on the spherical harmonics and the coordinates derived from the dicom, estimate the encoding
-        fields that have been applied to each voxel
-        """
-        legendre_basis = generate_legendre_basis(self.coords, self.n_order)
-        self.Gx_encode = (legendre_basis @ self._Gx_Harmonics) * 1e3
-        self.Gy_encode = (legendre_basis @ self._Gy_Harmonics) * 1e3
-        self.Gz_encode = (legendre_basis @ self._Gz_Harmonics) * 1e3
-
-    def _zero_volume(self, volume_to_zero):
-        """
-        takes an input volume and replaces all values <0 with 0.
-        required for the image domain corrector which tends to produce -ve pixels
-        """
-        negative_ind = volume_to_zero < 0
-        logger.warning(
-            f'{np.count_nonzero(negative_ind)} negative pixels detected; setting these to zero and continuing')
-        volume_to_zero[negative_ind] = 0
-        return volume_to_zero
-
-    def _generate_Kspace_data(self):
-        """
-        Get the k space of the current slice data.
-        :return:
-        """
-        self.k_space = fftshift(fft2(fftshift(self._image_to_correct)))
-
-    def _calculate_encoding_indices(self):
-        """
-        generates both the linear (i.e. assumed) indices and the distorted indices.
-        These indices are passed to the NUFFT library.
-        """
-
-        x_lin_size, y_lin_size = self._image_to_correct.shape
-        xn_lin = np.linspace(-x_lin_size / 2, -x_lin_size / 2 + x_lin_size - 1, x_lin_size)
-        yn_lin = np.linspace(-y_lin_size / 2, -y_lin_size / 2 + y_lin_size - 1, y_lin_size)
-        [xn_lin, yn_lin] = np.meshgrid(xn_lin, yn_lin, indexing='ij')
-        xn_lin = xn_lin.flatten()
-        yn_lin = yn_lin.flatten()
-        self.sk = xn_lin / x_lin_size
-        self.tk = yn_lin / y_lin_size
-
-        if (np.round(self._ImageOrientationPatient) == [0, 1, 0, 0, 0, -1]).all():
-            xn_dis = self.Gz_encode / (self._pixel_spacing[2]) + self._iso_offset_pixels[2]
-            self.xj = xn_dis * 2 * np.pi
-            yn_dis = self.Gy_encode / (self._pixel_spacing[1]) + self._iso_offset_pixels[1]
-            self.yj = yn_dis * 2 * np.pi
-        elif (np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 0, -1]).all():
-            xn_dis = (self.Gz_encode / (self._pixel_spacing[2])) + self._iso_offset_pixels[2]
-            self.xj = xn_dis * 2 * np.pi
-            yn_dis = self.Gx_encode / (self._pixel_spacing[0]) + self._iso_offset_pixels[0]
-            self.yj = yn_dis * 2 * np.pi
-        elif (np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 1, 0]).all():
-            xn_dis = self.Gy_encode / (self._pixel_spacing[1]) + self._iso_offset_pixels[1]
-            self.xj = xn_dis * 2 * np.pi
-            yn_dis = self.Gx_encode / (self._pixel_spacing[0]) + self._iso_offset_pixels[0]
-            self.yj = yn_dis * 2 * np.pi
-        elif np.round(self._ImageOrientationPatient == [2, 2, 2, 2, 2, 2]).all():
-            # this is for through plane correction where the real images are [0, 1, 0, 0, 0, -1]
-            self.xj = pd.Series(xn_lin * 2 * np.pi)
-            yn_dis = self.Gx_encode / (self._pixel_spacing[0]) + self._iso_offset_pixels[0]
-            self.yj = pd.Series(yn_dis * 2 * np.pi)
-            xn_dis = pd.Series(np.copy(xn_lin))
-        elif np.round(self._ImageOrientationPatient == [3, 3, 3, 3, 3, 3]).all():
-            # this is for through plane correction where the real images are [1, 0, 0, 0, 0, -1]
-            self.xj = pd.Series(xn_lin * 2 * np.pi)
-            yn_dis = self.Gy_encode / (self._pixel_spacing[1]) + self._iso_offset_pixels[1]
-            self.yj = yn_dis * 2 * np.pi
-            xn_dis = pd.Series(np.copy(xn_lin))
-        elif (np.round(self._ImageOrientationPatient) == [1, 1, 1, 1, 1, 1]).all():
-            # this is for through plane correction where the real images are [1, 0, 0, 0, 1, 0]
-            self.xj = pd.Series(xn_lin * 2 * np.pi)
-            yn_dis = -1 * self.Gz_encode / (self._pixel_spacing[2]) + self._iso_offset_pixels[2]
-            self.yj = yn_dis * 2 * np.pi
-            xn_dis = pd.Series(np.copy(xn_lin))
-        else:
-            raise NotImplementedError('this slice orientation is not handled yet sorry')
-
-        self.xj = self.xj.to_numpy()
-        self.yj = self.yj.to_numpy()
-        self.xn_dis_pixel = np.reshape((xn_dis - xn_lin).values, self._image_to_correct.shape)
-        self.yn_dis_pixel = np.reshape((yn_dis - yn_lin).values, self._image_to_correct.shape)
-
-    def _plot_encoding_fields(self, vmin=None, vmax=None):  # pragma: no cover
-        """
-        debug code; make sure the gradient fields look correct
-        """
-        fig, axs = plt.subplots(nrows=1, ncols=3, figsize=[15, 5])
-        gah = np.squeeze(np.reshape(self.Gx_encode.to_numpy(), self._image_shape)) * 1e6
-
-        Xim = axs[0].imshow(gah, vmin=vmin, vmax=vmax)
-        axs[0].set_title('Gx')
-        # axs[0].set_xlabel(self._row_label)
-        # axs[0].set_ylabel(self._col_label)
-
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs[0].add_artist(draw_circle)
-        axs[0].grid(False)
-
-        gah = np.squeeze(np.reshape(self.Gy_encode.to_numpy(), self._image_shape)) * 1e6
-
-        Yim = axs[1].imshow(gah, vmin=vmin, vmax=vmax)
-        axs[1].set_title('Gy')
-        # axs[1].set_xlabel(self._row_label)
-        # axs[1].set_ylabel(self._col_label)
-
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs[1].add_artist(draw_circle)
-        axs[1].grid(False)
-
-        gah = np.squeeze(np.reshape(self.Gz_encode.to_numpy(), self._image_shape)) * 1e6
-
-        Zim = axs[2].imshow(gah, vmin=vmin, vmax=vmax)
-        axs[2].set_title('Gz')
-        # axs[2].set_xlabel(self._row_label)
-        # axs[2].set_ylabel(self._col_label)
-
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs[2].add_artist(draw_circle)
-        axs[2].grid(False)
-
-        cbar = fig.colorbar(Xim, ax=axs[0], fraction=0.046, pad=0.04)
-        cbar = fig.colorbar(Yim, ax=axs[1], fraction=0.046, pad=0.04)
-        cbar = fig.colorbar(Zim, ax=axs[2], fraction=0.046, pad=0.04)
-        plt.tight_layout()
-        plt.show()
-
-    def _plot_indices(self):  # pragma: no cover
-        """
-        handy debug plot routine to plot linear/distorted indices
-        :return:
-        """
-
-        fig, axs = plt.subplots(nrows=2, ncols=2, figsize=[8, 8])
-        axs[0, 0].plot(self.xj)
-        axs[0, 0].set_title('xj')
-        axs[0, 1].plot(self.yj)
-        axs[0, 1].set_title('yj')
-        axs[1, 0].plot(self.sk)
-        axs[1, 0].set_title('sk')
-        axs[1, 1].plot(self.tk)
-        axs[1, 1].set_title('tk')
-
-    def _plot_coords(self):  # pragma: no cover
-
-        fig, axs = plt.subplots(1, 3)
-        axs[0].plot(self._X_slice.flatten())
-        axs[1].plot(self._Y_slice.flatten())
-        axs[2].plot(self._Z_slice.flatten())
-        plt.show()
-
-    def _plot_images(self):  # pragma: no cover
-        """
-        debugging method to show input, output, and diff images
-        :return:
-        """
-        vmin = 20
-        vmax = 100
-        fig, axs = plt.subplots(nrows=1, ncols=3)
-        axs[0].imshow(self._image_to_correct, vmin=vmin, vmax=vmax)
-        axs[1].imshow(self.outputImage, vmin=vmin, vmax=vmax)
-        axs[2].imshow((abs(np.subtract(self._image_to_correct, self.outputImage))), vmin=vmin, vmax=vmax)
-        axs[2].set_title('abs_difference')
-        plt.tight_layout()
-
-    # public methods
-
-    def correct_all_images(self):
-        """
-        This loops through the image array, and calls _correct_image on each slice.
-        If correct_through_plane is True, this process occurs twice, with the 'slice direction' being changed
-        in the second loop.
-        :return:
-        """
-        start_time = perf_counter()
-
-        update_every_n_slices = 10
-        if self.correct_through_plane:
-            n_images_to_correct = self._n_dicom_files + (self.ImageArray.shape[1] - 2 * self._n_zero_pad)
-        else:
-            n_images_to_correct = self._n_dicom_files
-        loop_axis = 2  # ImageArray always has slice last
-        # nb: the below code allows us to wrap all the data into one 'itterable'; it also changes the view
-        # such that we are looping over the slice direction
-        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
-                          np.rollaxis(self._X, loop_axis),
-                          np.rollaxis(self._Y, loop_axis),
-                          np.rollaxis(self._Z, loop_axis))
-
-        i = 0
-        self._image_array_corrected = np.zeros(self.ImageArray.shape)
-        for array_slice, X, Y, Z in zipped_data:
-            if i < self._n_zero_pad or i > self._n_dicom_files + self._n_zero_pad:
-                # skip these files, they have no meaning anyway and we can't (easily) write them to dicom
-                i += 1
-                continue
-
-            if i % update_every_n_slices == 0:
-                print(printProgressBar(i - self._n_zero_pad, n_images_to_correct))
-            self._image_to_correct = array_slice
-            self._X_slice = X
-            self._Y_slice = Y
-            self._Z_slice = Z
-            self._correct_image()
-            self._image_array_corrected[:, :, i] = self.outputImage
-            i += 1
-
-        if self.correct_through_plane:
-
-            if np.allclose(np.round(self._ImageOrientationPatient), [1, 0, 0, 0, 1, 0]):
-                self._ImageOrientationPatient = [1, 1, 1, 1, 1, 1]
-            elif np.allclose(np.round(self._ImageOrientationPatient), [0, 1, -0, -0, 0, -1]):
-                self._ImageOrientationPatient = [2, 2, 2, 2, 2, 2]
-            elif np.allclose(np.round(self._ImageOrientationPatient), [1, 0, 0, 0, 0, -1]):
-                self._ImageOrientationPatient = [3, 3, 3, 3, 3, 3]
-            else:
-                raise NotImplementedError
-
-            loop_axis = 1
-            zipped_data = zip(np.rollaxis(self._image_array_corrected, loop_axis),
-                              np.rollaxis(self._X, loop_axis),
-                              np.rollaxis(self._Y, loop_axis),
-                              np.rollaxis(self._Z, loop_axis))
-            self._image_array_corrected2 = self._image_array_corrected.copy()
-            j = 0
-            self._Rows = np.rollaxis(self._image_array_corrected, loop_axis).shape[1]
-            self._Cols = np.rollaxis(self._image_array_corrected, loop_axis).shape[2]
-            n_slices = np.rollaxis(self._image_array_corrected, loop_axis).shape[0]
-            for array_slice, X, Y, Z in zipped_data:
-                if j < self._n_zero_pad or j > n_slices + self._n_zero_pad:
-                    # skip these files, they have no meaning anyway and we can't (easily) write them to dicom
-                    j += 1
-                    continue
-
-                if j % update_every_n_slices == 0:
-                    print(printProgressBar(i + j - (self._n_zero_pad * 4), n_images_to_correct))
-                self._image_to_correct = array_slice
-                self._X_slice = X
-                self._Y_slice = Y
-                self._Z_slice = Z
-                self._correct_image()
-                self._image_array_corrected[:, j, :] = self.outputImage
-
-                j += 1
-
-        execution_time = perf_counter() - start_time
-        print(f'\ntotal time: {execution_time: 1.1f}s')
-        print(f'mean time per slice: {execution_time / n_images_to_correct: 1.1}s')
-        self._unpad_image_arrays()
-
-
-    def save_all_images(self, save_loc=None, DSV_radius=None, grid=True):
-        """
-        save corrected data as png
-
-        :param save_loc: path to save data at.
-        :type save_loc: string or path
-        """
-
-        import cProfile, pstats, io
-        from pstats import SortKey
-        pr = cProfile.Profile()
-        pr.enable()
-
-        _start_time = perf_counter()
-        print('saving all data as png...')
-        plt.ioff()
-        if save_loc is None:
-            save_loc = self.ImageDirectory / 'corrected'
-        save_loc = Path(save_loc)
-        if not (self.ImageDirectory / save_loc).is_dir():
-            save_loc.mkdir()
-
-        loop_axis = 2
-        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
-                          np.rollaxis(self._image_array_corrected, loop_axis))
-
-        # generate extent and labels
-        extent = None
-        row_label = None
-        col_label = None
-        FOV = None
-        slice_coords = None
-
-        if ((np.round(self._ImageOrientationPatient) == [0, 1, 0, 0, 0, -1]).all() or
-                np.round(self._ImageOrientationPatient == [2, 2, 2, 2, 2, 2]).all()):
-            extent = (self._X.min(), self._X.max(), self._Z.min(), self._Z.max())
-            slice_coords = np.unique(self._X)
-            row_label = 'X [mm]'
-            col_label = 'Z [mm]'
-
-        elif ((np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 0, -1]).all() or
-              np.round(self._ImageOrientationPatient == [3, 3, 3, 3, 3, 3]).all()):
-
-            extent = (self._Y.min(), self._Y.max(), self._Z.min(), self._Z.max())
-            slice_coords = np.unique(self._Y)
-            row_label = 'Y [mm]'
-            col_label = 'Z [mm]'
-
-        elif ((np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 1, 0]).all() or
-              np.round(self._ImageOrientationPatient == [1, 1, 1, 1, 1, 1]).all()):
-            extent = (self._X.min(), self._X.max(), self._Y.min(), self._Y.max())
-            slice_coords = np.unique(self._Z)
-            row_label = 'X [mm]'
-            col_label = 'Y [mm]'
-
-        if slice_coords is None:
-            slice_coords = np.ones(np.rollaxis(self.ImageArray, loop_axis).shape[0])
-        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
-                          np.rollaxis(self._image_array_corrected, loop_axis),
-                          slice_coords)
-
-        i = 0
-        for original_image, corrected_image, slice_coord in zipped_data:
-            fig, axs = plt.subplots(nrows=1, ncols=2)
-
-            # axs[0].imshow(self.pixel_array, extent=self._extent)
-            im1 = axs[0].imshow(original_image, extent=extent)
-            axs[0].set_title('Original Image')
-            axs[0].set_aspect('equal')
-            axs[0].set_xlabel(row_label)
-            axs[0].set_ylabel(col_label)
-            if grid:
-                axs[0].grid(True)
-            if DSV_radius:
-                h = 150 - slice_coord
-                with warnings.catch_warnings(record=True) as who_cares:
-                    warnings.simplefilter("always")
-                    FOV_radius = np.sqrt((2 * h * DSV_radius) - (h ** 2))
-                circ = Circle((0, 0), FOV_radius, facecolor='none', edgecolor='white')
-                axs[0].add_patch(circ)
-
-            im2 = axs[1].imshow(corrected_image, extent=extent)
-            axs[1].set_title('Corrected Image')
-            axs[1].set_aspect('equal')
-            axs[1].set_xlabel(row_label)
-            axs[1].set_ylabel(col_label)
-            if grid:
-                axs[1].grid(True)
-            if DSV_radius:
-                circ = Circle((0, 0), FOV_radius, facecolor='none', edgecolor='white')
-                axs[1].add_patch(circ)
-            plt.tight_layout()
-            plt.savefig(save_loc / (str(i) + '.png'), format='png')
-            plt.close('all')
-            i += 1
-        print(f'images export to png successful in {perf_counter() - _start_time} s')
-
-        pr.disable()
-        pr.dump_stats('save_images_stats')
-
-
-    def save_all_images_as_dicom(self, save_loc=None):
-        """
-        save corrected data as dicom
-
-        :param save_loc: path to save data at.
-        :type save_loc: string or path
-        """
-        _start_time = perf_counter()
-        print('saving all data as dcm...')
-        if self._image_array_corrected.min() < 0:
-            self._image_array_corrected = self._zero_volume(self._image_array_corrected)
-        if save_loc is None:
-            save_loc = self.ImageDirectory / 'corrected_dcm'
-        save_loc = Path(save_loc)
-        if not save_loc.is_dir():
-            save_loc.mkdir()
-        loop_axis = 2
-        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
-                          np.rollaxis(self._image_array_corrected, loop_axis))
-        i = 0
-        for original_image, corrected_image in zipped_data:
-            current_slice = pydicom.read_file(self.ImageDirectory / self._all_dicom_files[i])
-            temp_dcm = current_slice.copy()
-            temp_dcm.PixelData = np.uint16(corrected_image).tobytes()
-            temp_dcm.save_as(save_loc / (str(i) + '.dcm'))
-            i += 1
-        print(f'images exported to dicom in {perf_counter() - _start_time: 1.1f}s')
-
-
-class KspaceDistortionCorrector(DistortionCorrectorBase):
-    """
-    This performs correction using a least squares based approach in the k-space domain,
-    and is based on `this work <https://onlinelibrary.wiley.com/doi/epdf/10.1002/mrm.25487>`_
-    """
-
-    def __init__(self, pad=10, **kwds):
-
-        super().__init__(pad=pad, **kwds)
-        self.NUFFTlibrary = 'finufft'  # pynufft, finufft, or torchnufft
-        self._check_input_data()
-
-    def _generate_Kspace_data(self):
-        """
-        Get the k space of the current slice data.
-        :return:
-        """
-        self.k_space = fftshift(fft2(fftshift(self._image_to_correct)))
-
-    def _correct_image(self):
-        """
-        List of steps required for each independant input slice.
-        Under some circumstances some steps could be recycled for subsequent slices
-        """
-
-        self._image_shape = np.array(np.squeeze(self._X_slice).shape)
-        coords_cartesian = np.array([self._X_slice.flatten(), self._Y_slice.flatten(), self._Z_slice.flatten()])
-        coords_cartesian = pd.DataFrame(coords_cartesian.T, columns=['x', 'y', 'z'])
-        self.coords = convert_cartesian_to_spherical(coords_cartesian)
-        self._calculate_encoding_fields()
-        self._generate_Kspace_data()
-        self._calculate_encoding_indices()
-        self._perform_least_squares_optimisation()
-
-    def _fiNufft_Ax(self, x):
-        """
-        flatron instiute nufft
-        Returns A*x
-        equivalent to the 'notranpose' option in shanshans code
-        self.xj and yj are non uniform nonuniform source points. they are essentially the encoding signals.
-        self.sk and tk are uniform target points
-        # """
-        if x.dtype is not np.dtype('complex128'):
-            x = x.astype('complex128')
-        # y = nufft2d3(self.xj, self.yj, x, self.sk, self.tk, eps=1e-06, isign=-1)
-        y = self.Nufft_Ax_Plan.execute(x, None)
-        return y.flatten()
-
-    def _fiNufft_Atb(self, x):
-        """
-        flatron instiute nufft
-        This is to define the Nufft as a scipy.sparse.linalg.LinearOperator which can be used by the lsqr algorithm
-        see here for explanation:
-        https://stackoverflow.com/questions/48621407/python-equivalent-of-matlabs-lsqr-with-first-argument-a-function
-        Returns A'*x
-        equivalent to the 'tranpose' option in shanshans code
-        """
-        y = self.Nufft_Atb_Plan.execute(x, None)
-        return y.flatten()
-
-    def _perform_least_squares_optimisation(self):
-        """
-        From
-        `Integrated Image Reconstruction and Gradient Nonlinearity Correction <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4390402/pdf/nihms629785.pdf>`_
-        "A common strategy for reconstructing both fully- and undersampled MRI data is  penalized regression,
-        which seeks to **produce the image** most likely to have produced the set of noisy measurements while potentially
-        also satisfying some other expected properties (e.g., sparsity) (17). Since noise in MRI is Gaussian
-        distributed, penalized least squares regression of the following general form is often employed.
-        So:
-        - the image is what we want to get back.
-        - The noisy measurements are self.k_space
-        - We use the NUFFT to compute the image most likely to have produced k_space, given the encoding fields that we computed.
-        """
-        fk1 = np.reshape(self.k_space, [self._Rows * self._Cols])
-        StartingImage = None  # x0 for lsqr. can be overwritten for each option below.
-
-        if self.NUFFTlibrary == 'finufft':
-            self.Nufft_Ax_Plan = Plan(3, 2, 1, 1e-06, -1)
-            self.Nufft_Ax_Plan.setpts(self.xj, self.yj, None, self.sk, self.tk)
-            self.Nufft_Atb_Plan = Plan(3, 2, 1, 1e-06, 1)
-            self.Nufft_Atb_Plan.setpts(self.sk, self.tk, None, self.xj, self.yj)
-            A = LinearOperator((fk1.shape[0], fk1.shape[0]), matvec=self._fiNufft_Ax, rmatvec=self._fiNufft_Atb)
-            StartingImage = self._image_to_correct.flatten().astype(complex)
-
-        maxit = 20
-        x1 = lsqr(A, fk1, iter_lim=maxit, x0=StartingImage)
-        self.outputImage = abs(np.reshape(x1[0], [self._Rows, self._Cols]))
-
-
-class ImageDomainDistortionCorrector(DistortionCorrectorBase):
-    """
-    This performs image correction in the image domain by constructing a spline between the linear and distorted
-    indices.
-    """
-
-    def _correct_image(self):
-        """
-        List of steps required for each independant input slice.
-        Under some circumstances some steps could be recycled for subsequent slices
-        """
-
-        self._image_shape = np.array(np.squeeze(self._X_slice).shape)
-
-        coords_cartesian = np.array([self._X_slice.flatten(), self._Y_slice.flatten(), self._Z_slice.flatten()])
-        coords_cartesian = pd.DataFrame(coords_cartesian.T, columns=['x', 'y', 'z'])
-        self.coords = convert_cartesian_to_spherical(coords_cartesian)
-        self._calculate_encoding_fields()
-        self._calculate_encoding_indices()
-
-        x_n = np.arange(0, self._image_shape[0], 1)
-        y_n = np.arange(0, self._image_shape[1], 1)
-        pixel_interp = RectBivariateSpline(x_n, y_n, self._image_to_correct)
-
-        yy, xx = np.meshgrid(y_n, x_n)
-        xvector = (self.xn_dis_pixel + xx).flatten()
-        yvector = (self.yn_dis_pixel + yy).flatten()
-
-        _output_image = pixel_interp.ev(xvector, yvector)
-
-        _output_image = np.where((xvector < 0) | (yvector < 0) | (xvector > self._image_shape[0]) |
-                                 (yvector > self._image_shape[1]), 0, _output_image)
-
-        self.outputImage = _output_image.reshape(self._image_shape)
+import os
+import logging
+import warnings
+import pydicom
+import matplotlib.pyplot as plt
+from finufft import Plan
+import numpy as np
+from scipy.fft import fft2
+from scipy.fft import fftshift
+from scipy.sparse.linalg import lsqr
+from scipy.sparse.linalg import LinearOperator
+import pandas as pd
+from pathlib import Path
+from .utilities import get_all_files, convert_cartesian_to_spherical, generate_legendre_basis, dicom_to_numpy
+from .utilities import get_gradient_spherical_harmonics
+from .utilities import printProgressBar
+from time import perf_counter
+
+logging.basicConfig(format='[%(filename)s: line %(lineno)d] %(message)s', level=logging.WARNING)
+logger = logging.getLogger(__name__)
+
+
+class KspaceDistortionCorrector:
+    """
+    This algorithm is based on `this work`_<https://onlinelibrary.wiley.com/doi/epdf/10.1002/mrm.25487>
+    """
+
+    def __init__(self, ImageDirectory, NufftLibrary='finufft', gradient_harmonics=None,
+                 ImExtension='.dcm', dicom_data=None, correct_through_plane=True):
+        """
+        :param ImageDirectory:
+        :param NufftLibrary:
+        :param Gx_Harmonics:
+        :param Gy_Harmonics:
+        :param Gz_Harmonics:
+        :param ImExtension:
+        :param dicom_data:
+        :param correct_through_plane:
+        """
+        self.correct_through_plane = correct_through_plane
+        self._n_zero_pad = 20  # n_pixels to add around each edge of volume. set to 0 for no zero padding
+        self._dicom_data = dicom_data
+        self._Gx_Harmonics, self._Gy_Harmonics, self._Gz_Harmonics = \
+            get_gradient_spherical_harmonics(gradient_harmonics[0], gradient_harmonics[1], gradient_harmonics[2])
+        self._Gx_Harmonics = self._Gx_Harmonics * 1
+        self._Gy_Harmonics = self._Gy_Harmonics * 1
+        self._Gz_Harmonics = self._Gz_Harmonics * -1
+
+        self.ImageDirectory = Path(ImageDirectory)
+        self._all_dicom_files = get_all_files(self.ImageDirectory, ImExtension)
+        self._all_dicom_files = np.sort(self._all_dicom_files)
+        warnings.warn('making assumption that sorting by dicom name is same as series number')
+        # self._all_dicom_files = sort_dicom_slices(self._all_dicom_files)
+        self._n_dicom_files = len(self._all_dicom_files)
+
+
+        self.ImageArray,\
+        self._dicom_affine,\
+        (self._X, self._Y, self._Z) = dicom_to_numpy(self.ImageDirectory,
+                                                     file_extension=ImExtension,
+                                                     return_XYZ=True,
+                                                     zero_pad=self._n_zero_pad,
+                                                     enforce_increasing_coords=False)
+        self._get_rows_and_cols()
+        self.n_order = int(np.sqrt(self._Gx_Harmonics.size) - 1)
+        self.Images = get_all_files(self.ImageDirectory, ImExtension)
+        self.r_DSV = 150  # only for drawing on the plot
+        # Select nufft algorithm to use:
+        if not NufftLibrary in ['pynufft', 'finufft', 'torchnufft']:
+            raise NotImplementedError(f'Unknown NUFFTlibrary entered: {NufftLibrary}.'
+                         f'\nAllowed options are: pynufft, finufft, torchnufft')
+        self.NUFFTlibrary = NufftLibrary  # pynufft, finufft, or torchnufft
+        self._check_input_data()
+
+    def _get_rows_and_cols(self):
+        """
+        just extract the number of rows and columns from a dicom header - we need it for zero padding later.
+        I suspect I should be able to derive this from the dicom affine, but this way seems more foolproof
+        """
+        demo_header = pydicom.read_file(self.ImageDirectory / self._all_dicom_files[0])
+        self._Rows, self._Cols = self.ImageArray.shape[0:2]
+        self._ImageOrientationPatient = demo_header.ImageOrientationPatient
+        self._PixelSpacing = self._dicom_data['pixel_spacing']
+
+    def _check_input_data(self):
+        """
+        Put any tests of input data here
+        """
+        assert self._Gx_Harmonics.shape == self._Gy_Harmonics.shape == self._Gz_Harmonics.shape
+        assert self._n_zero_pad >= 0
+
+    def _correct_image(self):
+        """
+        List of steps required for each independant input slice.
+        Under some circumstances some steps could be recycled for subsequent slices
+        """
+
+        self._image_shape = np.array(np.squeeze(self._X_slice).shape)
+        coords_cartesian = np.array([self._X_slice.flatten(), self._Y_slice.flatten(), self._Z_slice.flatten()])
+        coords_cartesian = pd.DataFrame(coords_cartesian.T, columns=['x', 'y', 'z'])
+        self.coords = convert_cartesian_to_spherical(coords_cartesian)
+        self._calculate_encoding_fields()
+        self._generate_Kspace_data()
+        self._calculate_encoding_indices()
+        self._perform_least_squares_optimisation()
+
+    def _unpad_image_arrays(self):
+        """
+        remove any zero padding from original and reconstructed image volumes
+        """
+        if self._n_zero_pad > 0:
+            self.ImageArray = self.ImageArray[self._n_zero_pad:-self._n_zero_pad,
+                              self._n_zero_pad:-self._n_zero_pad,
+                              self._n_zero_pad:-self._n_zero_pad]
+            self._image_array_corrected = self._image_array_corrected[self._n_zero_pad:-self._n_zero_pad,
+                                          self._n_zero_pad:-self._n_zero_pad,
+                                          self._n_zero_pad:-self._n_zero_pad]
+
+    def _calculate_encoding_fields(self):
+        """
+        Based on the spherical harmonics and the coordinates derived from the dicom, estimate the encoding
+        fields that have been applied to each voxel
+        """
+        legendre_basis = generate_legendre_basis(self.coords, self.n_order)
+        self.Gx_encode = (legendre_basis @ self._Gx_Harmonics)
+        self.Gy_encode = (legendre_basis @ self._Gy_Harmonics)
+        self.Gz_encode = (legendre_basis @ self._Gz_Harmonics)
+
+    def _generate_Kspace_data(self):
+        """
+        Get the k space of the current slice data.
+        :return:
+        """
+        self.k_space = fftshift(fft2(fftshift(self._image_to_correct)))
+
+    def _calculate_encoding_indices(self):
+        """
+        generates both the linear (i.e. assumed) indices and the distorted indices.
+        These indices are passed to the NUFFT library.
+        """
+
+        x_lin_size, y_lin_size = self._image_to_correct.shape
+        xn_lin = np.linspace(-x_lin_size / 2, -x_lin_size / 2 + x_lin_size - 1, x_lin_size)
+        yn_lin = np.linspace(-y_lin_size / 2, -y_lin_size / 2 + y_lin_size - 1, y_lin_size)
+        [xn_lin, yn_lin] = np.meshgrid(xn_lin, yn_lin, indexing='ij')
+        xn_lin = xn_lin.flatten()
+        yn_lin = yn_lin.flatten()
+        self.sk = xn_lin / x_lin_size
+        self.tk = yn_lin / y_lin_size
+
+        if (np.round(self._ImageOrientationPatient) == [0, 1, 0, 0, 0, -1]).all():
+            xn_dis = self.Gz_encode / (self._PixelSpacing[2])
+            self.xj = xn_dis * 2 * np.pi
+            yn_dis = self.Gy_encode / (self._PixelSpacing[1])
+            self.yj = yn_dis * 2 * np.pi
+        elif (np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 0, -1]).all():
+            xn_dis = self.Gz_encode / (self._PixelSpacing[2])
+            self.xj = xn_dis * 2 * np.pi
+            yn_dis = self.Gx_encode / (self._PixelSpacing[0])
+            self.yj = yn_dis * 2 * np.pi
+        elif (np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 1, 0]).all():
+            xn_dis = self.Gy_encode / (self._PixelSpacing[1])
+            self.xj = xn_dis * 2 * np.pi
+            yn_dis = self.Gx_encode / (self._PixelSpacing[0])
+            self.yj = yn_dis * 2 * np.pi
+        elif np.round(self._ImageOrientationPatient == [2, 2, 2, 2, 2, 2]).all():
+            # this is for through plane correction where the real images are [0, 1, 0, 0, 0, -1]
+            self.xj = pd.Series(xn_lin * 2 * np.pi)
+            yn_dis = self.Gx_encode / (self._PixelSpacing[0])
+            self.yj = pd.Series(yn_dis * 2 * np.pi)
+        elif np.round(self._ImageOrientationPatient == [3, 3, 3, 3, 3, 3]).all():
+            # this is for through plane correction where the real images are [1, 0, 0, 0, 0, -1]
+            self.xj = pd.Series(xn_lin * 2 * np.pi)
+            yn_dis = self.Gy_encode / (self._PixelSpacing[1])
+            self.yj = yn_dis * 2 * np.pi
+        elif (np.round(self._ImageOrientationPatient) == [1, 1, 1, 1, 1, 1]).all():
+            # this is for through plane correction where the real images are [1, 0, 0, 0, 1, 0]
+            self.xj = pd.Series(xn_lin * 2 * np.pi)
+            yn_dis = -1*self.Gz_encode / (self._PixelSpacing[2])
+            self.yj = yn_dis * 2 * np.pi
+        else:
+            raise NotImplementedError('this slice orientation is not handled yet sorry')
+
+        self.xj = self.xj.to_numpy()
+        self.yj = self.yj.to_numpy()
+
+    def _fiNufft_Ax(self, x):
+        """
+        flatron instiute nufft
+        Returns A*x
+        equivalent to the 'notranpose' option in shanshans code
+        self.xj and yj are non uniform nonuniform source points. they are essentially the encoding signals.
+        self.sk and tk are uniform target points
+        # """
+
+        if x.dtype is not np.dtype('complex128'):
+            x = x.astype('complex128')
+        # y = nufft2d3(self.xj, self.yj, x, self.sk, self.tk, eps=1e-06, isign=-1)
+        y = self.Nufft_Ax_Plan.execute(x, None)
+        return y.flatten()
+
+    def _fiNufft_Atb(self, x):
+        """
+        flatron instiute nufft
+        This is to define the Nufft as a scipy.sparse.linalg.LinearOperator which can be used by the lsqr algorithm
+        see here for explanation:
+        https://stackoverflow.com/questions/48621407/python-equivalent-of-matlabs-lsqr-with-first-argument-a-function
+        Returns A'*x
+        equivalent to the 'tranpose' option in shanshans code
+        """
+        # y = nufft2d3(self.sk, self.tk, x, self.xj, self.yj, eps=1e-06, isign=1)
+        y = self.Nufft_Atb_Plan.execute(x, None)
+        return y.flatten()
+
+    def _perform_least_squares_optimisation(self):
+        """
+        From
+        `Integrated Image Reconstruction and Gradient Nonlinearity Correction <https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4390402/pdf/nihms629785.pdf>`_
+        "A common strategy for reconstructing both fully- and undersampled MRI data is  penalized regression,
+        which seeks to **produce the image** most likely to have produced the set of noisy measurements while potentially
+        also satisfying some other expected properties (e.g., sparsity) (17). Since noise in MRI is Gaussian
+        distributed, penalized least squares regression of the following general form is often employed.
+        So:
+        - the image is what we want to get back.
+        - The noisy measurements are self.k_space
+        - We use the NUFFT to compute the image most likely to have produced k_space, given the encoding fields that we computed.
+        """
+        fk1 = np.reshape(self.k_space, [self._Rows * self._Cols])
+
+        StartingImage = None  # x0 for lsqr. can be overwritten for each option below.
+
+        if self.NUFFTlibrary == 'finufft':
+            self.Nufft_Ax_Plan = Plan(3, 2, 1, 1e-06, -1)
+            self.Nufft_Ax_Plan.setpts(self.xj, self.yj, None, self.sk, self.tk)
+            self.Nufft_Atb_Plan = Plan(3, 2, 1, 1e-06, 1)
+            self.Nufft_Atb_Plan.setpts(self.sk, self.tk, None, self.xj, self.yj)
+            A = LinearOperator((fk1.shape[0], fk1.shape[0]), matvec=self._fiNufft_Ax, rmatvec=self._fiNufft_Atb)
+            StartingImage = self._image_to_correct.flatten().astype(complex)
+
+
+        maxit = 20
+        x1 = lsqr(A, fk1, iter_lim=maxit, x0=StartingImage)
+        self.outputImage = abs(np.reshape(x1[0], [self._Rows, self._Cols]))
+
+    def _plot_encoding_fields(self, vmin=None, vmax=None):
+        """
+        debug code; make sure the gradient fields look correct
+        """
+        fig, axs = plt.subplots(nrows=1, ncols=3, figsize=[15, 5])
+        gah = np.squeeze(np.reshape(self.Gx_encode.to_numpy(), self._image_shape)) * 1e6
+
+        Xim = axs[0].imshow(gah, vmin=vmin, vmax=vmax)
+        axs[0].set_title('Gx')
+        # axs[0].set_xlabel(self._row_label)
+        # axs[0].set_ylabel(self._col_label)
+
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs[0].add_artist(draw_circle)
+        axs[0].grid(False)
+
+        gah = np.squeeze(np.reshape(self.Gy_encode.to_numpy(), self._image_shape)) * 1e6
+
+        Yim = axs[1].imshow(gah, vmin=vmin, vmax=vmax)
+        axs[1].set_title('Gy')
+        # axs[1].set_xlabel(self._row_label)
+        # axs[1].set_ylabel(self._col_label)
+
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs[1].add_artist(draw_circle)
+        axs[1].grid(False)
+
+        gah = np.squeeze(np.reshape(self.Gz_encode.to_numpy(), self._image_shape)) * 1e6
+
+        Zim = axs[2].imshow(gah, vmin=vmin, vmax=vmax)
+        axs[2].set_title('Gz')
+        # axs[2].set_xlabel(self._row_label)
+        # axs[2].set_ylabel(self._col_label)
+
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs[2].add_artist(draw_circle)
+        axs[2].grid(False)
+
+        cbar = fig.colorbar(Xim, ax=axs[0], fraction=0.046, pad=0.04)
+        cbar = fig.colorbar(Yim, ax=axs[1], fraction=0.046, pad=0.04)
+        cbar = fig.colorbar(Zim, ax=axs[2], fraction=0.046, pad=0.04)
+        plt.tight_layout()
+        plt.show()
+
+    def _plot_indices(self):
+        """
+        handy debug plot routine to plot linear/distorted indices
+        :return:
+        """
+
+        fig, axs = plt.subplots(nrows=2, ncols=2, figsize=[8, 8])
+        axs[0, 0].plot(self.xj)
+        axs[0, 0].set_title('xj')
+        axs[0, 1].plot(self.yj)
+        axs[0, 1].set_title('yj')
+        axs[1, 0].plot(self.sk)
+        axs[1, 0].set_title('sk')
+        axs[1, 1].plot(self.tk)
+        axs[1, 1].set_title('tk')
+
+    def _plot_coords(self):
+
+        fig, axs = plt.subplots(1, 3)
+        axs[0].plot(self._X_slice.flatten())
+        axs[1].plot(self._Y_slice.flatten())
+        axs[2].plot(self._Z_slice.flatten())
+        plt.show()
+
+    def _plot_images(self):
+        """
+        debugging method to show input, output, and diff images
+        :return:
+        """
+        vmin = 20
+        vmax = 100
+        fig, axs = plt.subplots(nrows=1, ncols=3)
+        axs[0].imshow(self._image_to_correct, vmin=vmin, vmax=vmax)
+        axs[1].imshow(self.outputImage, vmin=vmin, vmax=vmax)
+        axs[2].imshow((abs(np.subtract(self._image_to_correct, self.outputImage))), vmin=vmin, vmax=vmax)
+        axs[2].set_title('abs_difference')
+        plt.tight_layout()
+
+    # public methods
+
+    def correct_all_images(self):
+        """
+        This will loop through and correct all IMA files in the input directory
+        :return:
+        """
+        if self.correct_through_plane:
+            n_images_to_correct = self._n_dicom_files + (self.ImageArray.shape[1] - 2 * self._n_zero_pad)
+        else:
+            n_images_to_correct = self._n_dicom_files
+        loop_axis = 2  # ImageArray always has slice last
+        # nb: the below code allows us to wrap all the data into one 'itterable'; it also changes the view
+        # such that we are looping over the slice direction
+        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
+                          np.rollaxis(self._X, loop_axis),
+                          np.rollaxis(self._Y, loop_axis),
+                          np.rollaxis(self._Z, loop_axis))
+
+        i = 0
+        self._image_array_corrected = np.zeros(self.ImageArray.shape)
+        for array_slice, X, Y, Z in zipped_data:
+            if i < self._n_zero_pad or i > self._n_dicom_files + self._n_zero_pad:
+                # skip these files, they have no meaning anyway and we can't (easily) write them to dicom
+                i += 1
+                continue
+
+            t_start = perf_counter()
+            print(f'2D correction: {i-self._n_zero_pad} of {self._n_dicom_files}')
+
+            print(printProgressBar(i-self._n_zero_pad, n_images_to_correct))
+            self._image_to_correct = array_slice
+            self._X_slice = X
+            self._Y_slice = Y
+            self._Z_slice = Z
+            self._correct_image()
+            self._image_array_corrected[:, :, i] = self.outputImage
+            t_stop = perf_counter()
+            print(f"Elapsed time {t_stop - t_start}")
+            i += 1
+
+        if self.correct_through_plane:
+
+            if (np.round(self._ImageOrientationPatient) == [1, 0, 0, 0, 1, 0]).all():
+                self._ImageOrientationPatient = [1, 1, 1, 1, 1, 1]
+            elif np.round(self._ImageOrientationPatient == [0, 1, 0, 0, 0, -1]).all():
+                self._ImageOrientationPatient = [2, 2, 2, 2, 2, 2]
+            elif np.round(self._ImageOrientationPatient == [1, 0, 0, 0, 0, -1]).all():
+                self._ImageOrientationPatient = [3, 3, 3, 3, 3, 3]
+            else:
+                raise NotImplementedError
+
+            loop_axis = 1
+            zipped_data = zip(np.rollaxis(self._image_array_corrected, loop_axis),
+                              np.rollaxis(self._X, loop_axis),
+                              np.rollaxis(self._Y, loop_axis),
+                              np.rollaxis(self._Z, loop_axis))
+            self._image_array_corrected2 = self._image_array_corrected.copy()
+            j = 0
+            self._Rows = np.rollaxis(self._image_array_corrected, loop_axis).shape[1]
+            self._Cols = np.rollaxis(self._image_array_corrected, loop_axis).shape[2]
+            n_slices = np.rollaxis(self._image_array_corrected, loop_axis).shape[0]
+            for array_slice, X, Y, Z in zipped_data:
+                if j < self._n_zero_pad or j > n_slices + self._n_zero_pad:
+                    # skip these files, they have no meaning anyway and we can't (easily) write them to dicom
+                    j += 1
+                    continue
+                t_start = perf_counter()
+                print(f'Through Plane correction: {j - self._n_zero_pad} of {self.ImageArray.shape[loop_axis] - (self._n_zero_pad)}')
+                print(printProgressBar(i+j-(self._n_zero_pad*4), n_images_to_correct))
+                self._image_to_correct = array_slice
+                self._X_slice = X
+                self._Y_slice = Y
+                self._Z_slice = Z
+                self._correct_image()
+                self._image_array_corrected[:, j, :] = self.outputImage
+
+                t_stop = perf_counter()
+                print(f"Elapsed time {t_stop - t_start}")
+
+                j += 1
+
+
+        self._unpad_image_arrays()
+
+    def save_all_images(self):
+        if not os.path.isdir(self.ImageDirectory / 'Corrected'):
+            os.mkdir(self.ImageDirectory / 'Corrected')
+        loop_axis = 2
+
+        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
+                          np.rollaxis(self._image_array_corrected, loop_axis))
+        i = 0
+        for original_image, corrected_image in zipped_data:
+            fig, axs = plt.subplots(nrows=1, ncols=2)
+
+            # axs[0].imshow(self.pixel_array, extent=self._extent)
+            im1 = axs[0].imshow(original_image)
+            axs[0].set_title('Original Image')
+            axs[0].set_aspect('equal')
+            # axs[0].set_xlabel(self._row_label)
+            # axs[0].set_ylabel(self._col_label)
+            axs[0].grid(True)
+            # fig.colorbar(im1, ax=axs[0])
+
+            # axs[1].imshow(self.outputImage, extent=self._extent)
+            im2 = axs[1].imshow(corrected_image)
+            axs[1].set_title('Corrected Image')
+            axs[1].set_aspect('equal')
+            # axs[1].set_xlabel(self._row_label)
+            # axs[1].set_ylabel(self._col_label)
+            axs[1].grid(True)
+            # fig.colorbar(im2, ax=axs[1])
+
+            plt.tight_layout()
+            plt.savefig(self.ImageDirectory / 'Corrected' / (str(i) + '.png'), format='png')
+            plt.close(fig)
+            i += 1
+
+    def save_all_images_as_dicom(self, save_loc=None):
+        if save_loc is None:
+            save_loc = self.ImageDirectory / 'Corrected_dcm'
+        save_loc = Path(save_loc)
+        if not save_loc.is_dir():
+            save_loc.mkdir()
+        loop_axis = 2
+        zipped_data = zip(np.rollaxis(self.ImageArray, loop_axis),
+                          np.rollaxis(self._image_array_corrected, loop_axis))
+        i = 0
+        for original_image, corrected_image in zipped_data:
+            current_slice = pydicom.read_file(self.ImageDirectory / self._all_dicom_files[i])
+            temp_dcm = current_slice.copy()
+            temp_dcm.PixelData = np.uint16(corrected_image).tobytes()
+            temp_dcm.save_as(save_loc / (str(i) + '.dcm'))
+            i += 1
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/FieldCalculation.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/FieldCalculation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,118 +1,113 @@
-import pathlib
-import numpy as np
-import logging
-import json
-from .utilities import get_dicom_data
-
-ch = logging.StreamHandler()
-formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
-ch.setFormatter(formatter)
-logger = logging.getLogger(__name__)
-logger.addHandler(ch)
-logger.setLevel(logging.INFO)
-logger.propagate = False
-
-
-class ConvertMatchedMarkersToBz:
-    """
-    an object to calculate and store magnetic fields.
-    Gradient fields are in T/m
-    B0 fields are in T
-
-    :param MatchedCentroids: a pandas data frame containing columns ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl'].
-        If you want to calculate B0, is should also have ['x_B0', 'y_B0', 'z_B0']. Such a dataframe is normally created
-        within the MatchedMarkerVolumes class. All coordinates in mm.
-    :param dicom_data: either a dictionary or a path to a .json file. The minimume required parameters are below.
-        dicom_data is calculated automatically when MR data is used to create a MarkerVolume, and can be exported
-        to json using::
-
-            marker_volume.save_dicom_data().
-
-        dicom_data example::
-
-            dicom_data = {'FOV': [400, 400, 400],
-            'bandwidth': 203,
-            'gama': 42.6,
-            'image_size': [256, 256, 256]}
-    :type dicom_data: dictionary or path
-
-    """
-
-    def __init__(self, MatchedCentroids, dicom_data):
-        """
-        init
-        """
-
-        self.dicom_data = get_dicom_data(dicom_data)
-        self.MatchedCentroids = MatchedCentroids
-        self.MagneticFields = self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt']].copy()
-        self.MagneticFields = self.MagneticFields .rename(columns={"x_gt": "x", "y_gt": "y", "z_gt": "z"})
-        # ^ aim is to calculate B field at the ground truth marker positions
-        if self.MatchedCentroids.r_gt.mean() < 10 or self.MatchedCentroids.r_gnl.mean() < 10:
-            logger.warning('it appears that your input data is in m, not mm - please use mm!')
-        self._check_dicom_data()
-        self._calculate_Bz()
-
-    def _check_dicom_data(self):
-        """
-        check that the minium data we will be needing is there.
-        """
-        expected_keys = ['FOV', 'bandwidth', 'gama', 'pixel_spacing', 'image_size', 'gradient_strength']
-        for key in expected_keys:
-            if not key in self.dicom_data.keys():
-                raise AttributeError(f'missing required dicom_data field: {key}')
-
-    def _get_B0_calc_direction(self):
-        """
-        if we have information about the frequency encode direction and information about B0 distortion,
-        we should find that the max B0 distortion occurs in the frequency direction.
-        If not, something problably is wrong.
-        in any case, the direction of maximum B0 distortion is returned and used to calcualte B0
-        """
-
-        x_B0_mean = np.mean(np.abs(self.MatchedCentroids.x_B0))
-        y_B0_mean = np.mean(np.abs(self.MatchedCentroids.y_B0))
-        z_B0_mean = np.mean(np.abs(self.MatchedCentroids.z_B0))
-        max = np.max([x_B0_mean, y_B0_mean, z_B0_mean])
-        directions = ['x', 'y', 'z']
-        direction = [int(el == max) for el in [x_B0_mean, y_B0_mean, z_B0_mean]]
-        self._B0_direction_bool = [bool(el) for el in direction]
-        if 'freq_encode_direction' in self.dicom_data.keys():
-            # check that the maximum distortion matches the frequence encode direction
-            if not directions[np.where(direction)[0][0]] == self.dicom_data['freq_encode_direction']:
-                logger.warning(f'\nYou have entered a frequency code direction in '
-                               f'{self.dicom_data["freq_encode_direction"]}, but maximum B0 distortion is detected'
-                               f'in {directions[np.where(direction)[0][0]]}. Proceeding using '
-                               f'{self.dicom_data["freq_encode_direction"]} but you should check this...\n')
-            self._B0_direction_bool = [self.dicom_data["freq_encode_direction"]==el for el in directions]
-        else:
-            logger.warning("\nyou have input data on B0 distortion, but dicom_data['freq_encode_direction'] does not exist."
-                           "Therefore, B0 fields will be calculated based on the direction of maximum B0 distortion, "
-                           "which is \n")
-        self._B0_direction_string = np.array(['x_B0', 'y_B0', 'z_B0'])[self._B0_direction_bool][0]
-
-    def _calculate_Bz(self):
-        """
-        Calculate Gradient Bz at each point. This is based on code from Shanshan.
-        Shanshans notes:
-        - When reversing gradient polarity, the readout (z) and phase encoding (y) directions are reversed,
-         however, the slice selction direction (x) is not.
-        - B0 inhomogeneity distortion appears at readout diretion and is neglectable at phase encoding direction.
-        - This is distorted marker position caused by GNL-only along readout and phase encoding directions
-        """
-        gradient_strength = np.array(self.dicom_data['gradient_strength'])  # unit(T / m)
-        # ^ this is a vector [gx, gy, gz]
-        mm_to_m_factor = 1e-3
-        self.MagneticFields['B_Gx'] = self.MatchedCentroids.x_gnl * gradient_strength[0] * mm_to_m_factor
-        self.MagneticFields['B_Gy'] = self.MatchedCentroids.y_gnl * gradient_strength[1] * mm_to_m_factor
-        self.MagneticFields['B_Gz'] = self.MatchedCentroids.z_gnl * gradient_strength[2] * mm_to_m_factor
-
-        # if possible, add in B0 to data
-        B0_fields = ['x_B0', 'y_B0', 'z_B0']
-        B0_calc_possible = all([el in self.MatchedCentroids.columns for el in B0_fields])
-        if B0_calc_possible:
-            self._get_B0_calc_direction()
-            self.MagneticFields['B0'] = self.MatchedCentroids[[self._B0_direction_string]] * \
-                                        gradient_strength[self._B0_direction_bool][0] * mm_to_m_factor
-
-
+import pathlib
+import numpy as np
+import logging
+import json
+from .utilities import get_dicom_data
+
+ch = logging.StreamHandler()
+formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
+ch.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(ch)
+logger.setLevel(logging.INFO)
+logger.propagate = False
+
+
+class ConvertMatchedMarkersToBz:
+    """
+    :param MatchedCentroids: a pandas data frame containing columns ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl'].
+        If you want to calculate B0, is should also have ['x_B0', 'y_B0', 'z_B0']. Such a dataframe is normally created
+        within the MatchedMarkerVolumes class.
+    :param dicom_data: either a dictionary or a path to a .json file. The minimume required parameters are below.
+        dicom_data is calculated automatically when MR data is used to create a MarkerVolume, and can be exported
+        to json using::
+
+            marker_volume.save_dicom_data().
+
+        dicom_data example::
+
+            dicom_data = {'FOV': [400, 400, 400],
+            'bandwidth': 203,
+            'gama': 42.6,
+            'image_size': [256, 256, 256]}
+    :type dicom_data: dictionary or path
+
+    """
+
+    def __init__(self, MatchedCentroids, dicom_data):
+        """
+        init
+        """
+
+        self.dicom_data = get_dicom_data(dicom_data)
+        self.MatchedCentroids = MatchedCentroids
+        self.MagneticFields = self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt']].copy()
+        self.MagneticFields = self.MagneticFields .rename(columns={"x_gt": "x", "y_gt": "y", "z_gt": "z"})
+        # ^ aim is to calculate B field at the ground truth marker positions
+        if self.MatchedCentroids.r_gt.mean() < 10 or self.MatchedCentroids.r_gnl.mean() < 10:
+            logger.warning('it appears that your input data is in m, not mm - please use mm!')
+        self._check_dicom_data()
+        self._calculate_Bz()
+
+    def _check_dicom_data(self):
+        """
+        check that the minium data we will be needing is there.
+        """
+        expected_keys = ['FOV', 'bandwidth', 'gama', 'pixel_spacing', 'image_size', 'gradient_strength']
+        for key in expected_keys:
+            if not key in self.dicom_data.keys():
+                raise AttributeError(f'missing required dicom_data field: {key}')
+
+    def _get_B0_calc_direction(self):
+        """
+        if we have information about the frequency encode direction and information about B0 distortion,
+        we should find that the max B0 distortion occurs in the frequency direction.
+        If not, something problably is wrong.
+        in any case, the direction of maximum B0 distortion is returned and used to calcualte B0
+        """
+
+        x_B0_mean = np.mean(np.abs(self.MatchedCentroids.x_B0))
+        y_B0_mean = np.mean(np.abs(self.MatchedCentroids.y_B0))
+        z_B0_mean = np.mean(np.abs(self.MatchedCentroids.z_B0))
+        max = np.max([x_B0_mean, y_B0_mean, z_B0_mean])
+        directions = ['x', 'y', 'z']
+        direction = [int(el == max) for el in [x_B0_mean, y_B0_mean, z_B0_mean]]
+        self._B0_direction_bool = [bool(el) for el in direction]
+        if 'freq_encode_direction' in self.dicom_data.keys():
+            # check that the maximum distortion matches the frequence encode direction
+            if not directions[np.where(direction)[0][0]] == self.dicom_data['freq_encode_direction']:
+                logger.warning(f'\nYou have entered a frequency code direction in '
+                               f'{self.dicom_data["freq_encode_direction"]}, but maximum B0 distortion is detected'
+                               f'in {directions[np.where(direction)[0][0]]}. Proceeding using '
+                               f'{self.dicom_data["freq_encode_direction"]} but you should check this...\n')
+            self._B0_direction_bool = [self.dicom_data["freq_encode_direction"]==el for el in directions]
+        else:
+            logger.warning("\nyou have input data on B0 distortion, but dicom_data['freq_encode_direction'] does not exist."
+                           "Therefore, B0 fields will be calculated based on the direction of maximum B0 distortion, "
+                           "which is \n")
+        self._B0_direction_string = np.array(['x_B0', 'y_B0', 'z_B0'])[self._B0_direction_bool][0]
+
+    def _calculate_Bz(self):
+        """
+        Calculate Gradient Bz at each point. This is based on code from Shanshan.
+        Shanshans notes:
+        - When reversing gradient polarity, the readout (z) and phase encoding (y) directions are reversed,
+         however, the slice selction direction (x) is not.
+        - B0 inhomogeneity distortion appears at readout diretion and is neglectable at phase encoding direction.
+        - This is distorted marker position caused by GNL-only along readout and phase encoding directions
+        """
+        gradient_strength = np.array(self.dicom_data['gradient_strength'])  # unit(T / m)
+        # ^ this is a vector [gx, gy, gz]
+        self.MagneticFields['B_Gx'] = self.MatchedCentroids.x_gnl * gradient_strength[0]
+        self.MagneticFields['B_Gy'] = self.MatchedCentroids.y_gnl * gradient_strength[1]
+        self.MagneticFields['B_Gz'] = self.MatchedCentroids.z_gnl * gradient_strength[2]
+
+        # if possible, add in B0 to data
+        B0_fields = ['x_B0', 'y_B0', 'z_B0']
+        B0_calc_possible = all([el in self.MatchedCentroids.columns for el in B0_fields])
+        if B0_calc_possible:
+            self._get_B0_calc_direction()
+            self.MagneticFields['B0'] = self.MatchedCentroids[[self._B0_direction_string]] * \
+                                        gradient_strength[self._B0_direction_bool][0] * 1e-3
+
+
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/Harmonics.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/Harmonics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,367 +1,349 @@
-from pathlib import Path
-import sys, os
-import numpy as np
-import pandas as pd
-import logging
-from matplotlib import pyplot as plt
-from .utilities import bcolors
-from .utilities import convert_cartesian_to_spherical, generate_legendre_basis
-from .utilities import reconstruct_Bz
-from .utilities import generate_harmonic_names
-import seaborn as sns
-
-sns.set_theme(style="whitegrid")
-ch = logging.StreamHandler()
-formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
-ch.setFormatter(formatter)
-logger = logging.getLogger(__name__)
-logger.addHandler(ch)
-logger.setLevel(logging.INFO)  # This toggles all the logging in your app
-logger.propagate = False
-
-
-class SphericalHarmonicFit:
-    """
-    Uses single value decomposition to fit spherical harmonics to InputData.
-
-    Let the legendre basis be called L, the Harmonics be H and the magnetic field B.
-    L will have size [n_coords, n_harmonics], Harmonics has size [n_harmonics, 1] and B has size [n_coords, 1]
-
-    Our proposition is that there exists some set of harmonics such that
-
-    .. math:: L.H = B
-
-    We can find H by inverting L:
-
-    .. math::
-
-        L^{-1}.L.H = L^{-1}.B \\
-        H = L^{-1}.B
-
-    This task is performed using numpys pseudo_inverse functionality to invert L
-
-    :param _input_Bz_data: A pandas dataframe with columns x, y, z, Bz. Data should be in mm and T
-    :type _input_Bz_data: Pandas.DataFrame
-    :param r_outer: radius of sphere of interest. If AssessHarmonicPk_Pk=True, data is reconstucted on r_outer. if
-        TrimDataBy_r_outer=True, data lying outside r_outer will be deleted. Finally, r_outer is used to set the limits
-        on plotting data.
-    :type r_outer: float, optional
-    :param n_order: order of harmonic fit. higher order means more terms to fit, which may result in a better fit
-        but also is slower. If the data you input doesn't satisfy some nyquist criterion (I need to figure this out!)
-        then you will get a spurious result. For most MRI application 8 should be a reasonable number.
-    :type n_order: int, optional
-    :param AssessHarmonicPk_Pk: if True, data is reconstructed on the surface of r_outer, and the pk-pk contribution
-        from each harmonic calculated. This is a very useful way to interpret harmonics which are otherwise quite
-        abstract.
-    :type AssessHarmonicPk_Pk: bool, optional
-    :param QuantifyFit: if True, reconstruct data at all input data points, and compare input data point to
-        reconstructed data point. This is useful to check how well the fit has worked.
-    :type QuantifyFit: bool, optional
-    :param TrimDataBy_r_outer: if True, any input data outside r_outer is deleted
-    :type TrimDataBy_r_outer: bool, optional
-    :param scale: Value to scale the harmonics by. The main intention of this parameter is to normalise gradient
-        field harmonics to gradient strength. harmonics will be multiplied by the value of scale
-    :type scale: float, optional
-    """
-
-    def __init__(self, input_Bz_data, r_outer=150, n_order=5, AssessHarmonicPk_Pk=True, QuantifyFit=True,
-                 TrimDataBy_r_outer=False, scale=1):
-
-        # attributes:
-        self._tol = 1e-3  # tolerance for coordinate filtering in mm
-        self.scale = scale
-        self.TrimDataBy_r_outer = TrimDataBy_r_outer
-        self.r_outer = r_outer
-        self.QuantifyFit = QuantifyFit
-        self._AssessHarmonicPk_Pk = AssessHarmonicPk_Pk
-        self.n_order = n_order
-        self.n_harmonics = (self.n_order + 1) ** 2
-        self._input_Bz_data = input_Bz_data
-        self.__recon_warning_thrown = False
-        self._data_type = None
-        self._determine_Bz_data_type()
-        # basic fitting routine:
-        if self._data_type == 'field_map':
-            self._input_Bz_data = convert_cartesian_to_spherical(self._input_Bz_data)
-            self._check_data_input()
-            if self.TrimDataBy_r_outer:
-                self._filter_data()
-            self._coeff_names = generate_harmonic_names(self.n_order)
-            self.legendre_basis = generate_legendre_basis(self._input_Bz_data, self.n_order)
-            self._svd_fit()
-            self.harmonics = self.harmonics * scale
-        elif self._data_type == 'harmonics':
-            r = self.r_outer
-            azimuth = np.linspace(0, 2 * np.pi, 100)
-            elevation = np.linspace(0, np.pi, 100)
-            [r, azimuth, elevation] = np.meshgrid(r, azimuth, elevation)
-            coords = pd.DataFrame({'r': r.flatten(), 'azimuth': azimuth.flatten(), 'elevation': elevation.flatten()})
-            self.legendre_basis = generate_legendre_basis(coords, self.n_order)
-            self.harmonics = self._input_Bz_data
-        else:
-            raise AttributeError('invalid input data')
-        if self.QuantifyFit and self._data_type == 'field_map':
-            self._quantify_fit()
-        if self._AssessHarmonicPk_Pk:
-            self._assess_harmonic_pk_pk()
-
-    def _determine_Bz_data_type(self):
-        """
-        check whether we have field data, or harmonics
-        """
-        if isinstance(self._input_Bz_data, pd.Series):
-            if not len(self._input_Bz_data) == (self.n_order + 1) ** 2:
-                raise ValueError('length of series does not match input n_order')
-            else:
-                self._data_type = 'harmonics'
-        elif isinstance(self._input_Bz_data, pd.DataFrame):
-            self._data_type = 'field_map'  # not error checks in place downstream
-
-    def _check_data_input(self):
-        """
-        - Make sure the input data actually covers a sphere. If it doesn't, it normally means something has or will go wrong
-            so a warning is triggered.
-        - Make sure that input data is in mm, which is an implicit assumption
-        """
-
-        if not isinstance(self.n_order, int):
-            logger.warning(f'n_order should be integer; round {self.n_order} to {int(self.n_order)}')
-            self.n_order = int(self.n_order)
-
-        if self._data_type == 'field_map':
-            if self._input_Bz_data.r.mean() < 10:
-                logger.warning('it appears that your input data is in m, not mm - please use mm!')
-
-            if (self._input_Bz_data.elevation.max() - self._input_Bz_data.elevation.min()) < 0.75 * np.pi or \
-                    (self._input_Bz_data.azimuth.max() - self._input_Bz_data.azimuth.min()) < 1.8 * np.pi:
-                logger.warning('input sample points do not appear to cover a full sphere')
-            field_map_headings = ['x', 'y', 'z', 'Bz']
-            for col in field_map_headings:
-                if not col in self._input_Bz_data.columns:
-                    raise AttributeError(f'Field map data must contain {field_map_headings}')
-
-    def _filter_data(self):
-        """
-        filter the Bz data by radial coordinate, removing any entries that fall outside self.r_outer
-        """
-
-        data_to_delete_ind = self._input_Bz_data.r > (self.r_outer + self._tol)
-        self._input_Bz_data = self._input_Bz_data.drop(self._input_Bz_data[data_to_delete_ind].index)
-        self._input_Bz_data.reset_index(inplace=True)
-        n_deleted = np.count_nonzero(data_to_delete_ind)
-        if n_deleted > 0:
-            logger.warning(f'deleting {n_deleted} of the original {data_to_delete_ind.size} data points because'
-                           f'they fall outside the r_outer value of {self.r_outer} and TrimDataBy_r_outer=True')
-
-        if self._input_Bz_data.shape[0] == 0:
-            logger.error(f'After filtering for data insdide {self.r_outer} mm, there is no data left!')
-            sys.exit(1)
-
-    def _svd_fit(self):
-        """
-        calculate harmonics using single value decomposition of legendre_basis
-        """
-
-        inverseLegendre = np.linalg.pinv(self.legendre_basis)
-
-        if not np.allclose(inverseLegendre @ self.legendre_basis,
-                           np.eye(inverseLegendre.shape[0], self.legendre_basis.shape[1]),
-                           rtol=5e-3, atol=5e-4):
-            # check that the inverse times itself returns an idendity matrix as it should.
-            logger.error('it appears that single value decomposition has failed. This occurs for a few reasons:'
-                         '\n-  Very small or very large data in the input coordinates'
-                         '\n-  The data does not cover a full sphere: hence the matrix is poorly conditioned and has no inverse'
-                         '\n-  Continuing but you should be careful...')
-
-        harmonics = inverseLegendre @ self._input_Bz_data.Bz
-        self.harmonics = pd.Series(harmonics, index=self._coeff_names)
-
-    def _quantify_fit(self):
-        """
-        Compare the reconstructed field to the original field and calculate some basic goodness of fit metrics
-        """
-        if len(self._input_Bz_data.index) > 1e4:
-            logger.warning('you are reconstructing a lot of points and it might be a bit slow.'
-                           'I should write a down sampling routine here...')
-
-        Bz_recon = self.legendre_basis @ (self.harmonics / self.scale)
-        Residual = np.subtract(self._input_Bz_data.Bz, Bz_recon)
-        self._residual_pk_pk = float(abs(Residual.max() - Residual.min()) * 1e6)
-
-        initial_pk_pk = float(abs(self._input_Bz_data.Bz.max() - self._input_Bz_data.Bz.min()) * 1e6)
-        recon_pk_pk = float(abs(Bz_recon.max() - Bz_recon.min()) * 1e6)
-        residual_percentage = abs(self._residual_pk_pk) * 100 / initial_pk_pk
-
-        try:
-            print(f'Initial pk-pk:       {initial_pk_pk: 1.3e} \u03BCT')
-            print(f'Reconstructed pk-pk: {recon_pk_pk: 1.3e} \u03BCT')
-            print(f'Residual pk-pk:      {self._residual_pk_pk: 1.3e} \u03BCT ({residual_percentage: 1.1f}%)')
-        except UnicodeError:
-            print(f'Initial pk-pk:       {initial_pk_pk: 1.3e} uT')
-            print(f'Reconstructed pk-pk: {recon_pk_pk: 1.3e} uT')
-            print(f'Residual pk-pk:      {self._residual_pk_pk: 1.3e} uT ({residual_percentage: 1.1f}%)')
-
-        if residual_percentage > 2:
-            logger.warning('residual_pk_pk is greater than 2 %. This may indicate that the order is not high enough,'
-                           'or that the data is non physical (but it heavily depends on your use case!')
-
-    def _assess_harmonic_pk_pk(self):
-        """
-        generate the peak-peak perturbation caused over the surface of the sphere due to each harmonic
-        """
-        if len(self.legendre_basis.index) < 1e4:
-            # generate some points to ensure we cover a good portion of the sphere
-            r = self.r_outer
-            azimuth = np.linspace(0, 2 * np.pi, 100)
-            elevation = np.linspace(0, np.pi, 100)
-            [r, azimuth, elevation] = np.meshgrid(r, azimuth, elevation)
-            coords = pd.DataFrame({'r': r.flatten(), 'azimuth': azimuth.flatten(), 'elevation': elevation.flatten()})
-            legendre_basis_to_use = generate_legendre_basis(coords, self.n_order)
-        else:
-            legendre_basis_to_use = self.legendre_basis
-
-        BasisRange = legendre_basis_to_use.apply(lambda x: abs(np.max(x) - np.min(x)))
-        self.HarmonicsPk_Pk = (self.harmonics / self.scale) * BasisRange * 1e6
-
-    # Public Methods
-
-    def plot_harmonics_pk_pk(self, cut_off=.1, title=None, return_axs=False):  # pragma: no cover
-        """
-        produces a barplot of harmonics.
-
-        :param cut_off: cutoff point relative to highest harmonic. e.g. cut_off=.1 means that harmonics which produce
-            less than 10% the pk-pk perturbation of the dominant harmonic are ignored.
-        :type cut_off: float, optional
-        """
-
-        if not hasattr(self, 'HarmonicsPk_Pk'):
-            self._assess_harmonic_pk_pk()
-        plt.figure(figsize=[10, 5])
-        # ax = sns.barplot(self.HarmonicsPk_Pk, y='pk-pk [\u03BCT]', x=)
-        CutOffInd = abs(self.HarmonicsPk_Pk) < cut_off * abs(self.HarmonicsPk_Pk).max()
-        KeyHarmonics = self.HarmonicsPk_Pk.drop(self.HarmonicsPk_Pk[CutOffInd].index)
-        HarmonicsToPlot = KeyHarmonics
-
-        axs = sns.barplot(x=HarmonicsToPlot.index, y=HarmonicsToPlot.values, palette="Blues_d")
-        if title is None:
-            axs.set_title(f'Principle Harmonics pk-pk (>{cut_off * 100: 1.0f}% of max)')
-        else:
-            axs.set_title(title)
-
-        axs.set_ylabel('pk-pk [\u03BCT]')
-        for item in axs.get_xticklabels():
-            item.set_rotation(45)
-        if not return_axs:
-            plt.show()
-        else:
-            return axs
-
-    def plot_cut_planes(self, resolution=2.5, AddColorBar=True, quantity='uT', vmin=None,
-                        vmax=None):  # pragma: no cover
-        """
-        Reconstruct the Bz field at the cardinal planes.
-        Note this is basically the same code copied three times in  a row, one for each plane.
-
-        :param resolution: the resolution of reconstructed data. Default is 2.5 mm
-        :type resolution: float, optional
-        :param AddColorBar: Add a color bar to each plot
-        :type AddColorBar: Boolean, optional
-        :param quantity: quantity to use in reconstruct_Bz; must match the options for that function
-        :type quantity: string, optional
-        :param vmin: same as matplotlib.pyplot.imshow; vmin and vmax control the color map bounds.
-        :type vmin: float, optional
-        :param vmax: same as matplotlib.pyplot.imshow; vmin and vmax control the color map bounds.
-        :type vmax: float, optional
-        """
-
-        fig, (axs1, axs2, axs3) = plt.subplots(nrows=1, ncols=3, figsize=(15, 5))
-        extent = [-self.r_outer - resolution, self.r_outer + resolution, -self.r_outer - resolution,
-                  self.r_outer + resolution]  # same for all plots
-
-        conversion_factor = 1
-        # XY plane
-        x = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        y = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        z = 0
-        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
-        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
-        recon_coords = convert_cartesian_to_spherical(recon_coords)
-        Bz_recon = reconstruct_Bz(harmonics=self.harmonics / self.scale, coords=recon_coords, quantity=quantity)
-        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(x_recon).shape)
-        XYimage = axs1.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
-        axs1.set_xlabel('x [mm]')
-        axs1.set_ylabel('y [mm]')
-        axs1.set_title('a) XY plane')
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs1.grid(False)
-        axs1.add_artist(draw_circle)
-
-        # ZX plane
-        x = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        y = 0
-        z = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
-        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
-        recon_coords = convert_cartesian_to_spherical(recon_coords)
-        Bz_recon = reconstruct_Bz(harmonics=self.harmonics / self.scale, coords=recon_coords, quantity=quantity)
-        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(y_recon).shape)
-        ZXimage = axs2.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
-        axs2.set_xlabel('x [mm]')
-        axs2.set_ylabel('z [mm]')
-        axs2.set_title('b) ZX plane')
-        axs2.grid(False)
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs2.add_artist(draw_circle)
-
-        # ZY plane
-        x = 0
-        y = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        z = np.linspace(-self.r_outer, self.r_outer, int((2 * self.r_outer) / resolution)) * conversion_factor
-        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
-        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
-        recon_coords = convert_cartesian_to_spherical(recon_coords)
-        Bz_recon = reconstruct_Bz(harmonics=self.harmonics / self.scale, coords=recon_coords, quantity=quantity)
-        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(z_recon).shape)
-        ZYimage = axs3.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
-        axs3.set_xlabel('y [mm]')
-        axs3.set_ylabel('z [mm]')
-        axs3.grid(False)
-        axs3.set_title('c) ZY plane')
-        draw_circle = plt.Circle((0, 0), 150, fill=False)
-        axs3.add_artist(draw_circle)
-
-        if AddColorBar:
-            if quantity == 'uT':
-                cb_title = '\u03BCT'
-            elif quantity == 'T':
-                cb_title = 'T'
-            cbar = fig.colorbar(XYimage, ax=axs1, fraction=0.046, pad=0.04)
-            cbar.set_label(cb_title)
-            cbar = fig.colorbar(ZXimage, ax=axs2, fraction=0.046, pad=0.04)
-            cbar.set_label(cb_title)
-            cbar = fig.colorbar(ZYimage, ax=axs3, fraction=0.046, pad=0.04)
-            cbar.set_label(cb_title)
-
-        plt.tight_layout()
-        plt.show()
-
-    def print_key_harmonics(self, cut_off=.01):
-        """
-        print the harmonics with value > cut_off to the terminal in pk-pk.
-
-        :param cut_off: cutoff point relative to highest harmonic. e.g. cut_off=.1 means that harmonics which produce
-            less than 10% the pk-pk perturbation of the dominant harmonic are ignored.
-        :type cut_off: float, optional
-        """
-        if not hasattr(self, 'harmonics_pk_pk'):
-            self._assess_harmonic_pk_pk()
-
-        CutOffInd = abs(self.HarmonicsPk_Pk) < cut_off * abs(self.HarmonicsPk_Pk).max()
-        KeyHarmonics = self.HarmonicsPk_Pk.drop(self.HarmonicsPk_Pk[CutOffInd].index)
-        pd.set_option('display.float_format', lambda x: '%1.4ef' % x)
-        print(f'\nOnly displaying values >= {cut_off * 100: 1.0f}% of the peak harmonic.')
-        try:
-            print('Values are in pk=pk [\u03BCT]')
-        except UnicodeError:
-            print('Values are in pk=pk uT]')
-        print(f'{bcolors.OKBLUE}{KeyHarmonics.to_string()}{bcolors.ENDC}')
+from pathlib import Path
+import sys, os
+import numpy as np
+import pandas as pd
+import logging
+from matplotlib import pyplot as plt
+from .utilities import bcolors
+from .utilities import convert_cartesian_to_spherical, generate_legendre_basis
+from .utilities import reconstruct_Bz
+import seaborn as sns
+
+sns.set_theme(style="whitegrid")
+ch = logging.StreamHandler()
+formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
+ch.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(ch)
+logger.setLevel(logging.INFO)  # This toggles all the logging in your app
+logger.propagate = False
+
+class SphericalHarmonicFit:
+    """
+    Uses single value decomposition to fit spherical harmonics to InputData.
+
+    Let the legendre basis be called L, the Harmonics be H and the magnetic field B.
+    L will have size [n_coords, n_harmonics], Harmonics has size [n_harmonics, 1] and B has size [n_coords, 1]
+
+    Our proposition is that there exists some set of harmonics such that
+
+    .. math:: L.H = B
+
+    We can find H by inverting L:
+
+    .. math::
+
+        L^{-1}.L.H = L^{-1}.B \\
+        H = L^{-1}.B
+
+    This task is performed using numpys pseudo_inverse functionality to invert L
+
+    :param InputData: A pandas dataframe with columns x, y, z, Bz. Data should be in mm and T
+    :type InputData: Pandas.DataFrame
+    :param r_outer: radius of sphere of interest. If AssessHarmonicPk_Pk=True, data is reconstucted on r_outer. if
+        TrimDataBy_r_outer=True, data lying outside r_outer will be deleted. Finally, r_outer is used to set the limits
+        on plotting data.
+    :type r_outer: float, optional
+    :param n_order: order of harmonic fit. higher order means more terms to fit, which may result in a better fit
+        but also is slower. If the data you input doesn't satisfy some nyquist criterion (I need to figure this out!)
+        then you will get a spurious result. For most MRI application 8 should be a reasonable number.
+    :type n_order: int, optional
+    :param AssessHarmonicPk_Pk: if True, data is reconstructed on the surface of r_outer, and the pk-pk contribution
+        from each harmonic calculated. This is a very useful way to interpret harmonics which are otherwise quite
+        abstract.
+    :type AssessHarmonicPk_Pk: bool, optional
+    :param QuantifyFit: if True, reconstruct data at all input data points, and compare input data point to
+        reconstructed data point. This is useful to check how well the fit has worked.
+    :type QuantifyFit: bool, optional
+    :param TrimDataBy_r_outer: if True, any input data outside r_outer is deleted
+    :type TrimDataBy_r_outer: bool, optional
+    :param scale: Value to scale the harmonics by. The main intention of this parameter is to normalise gradient
+        field harmonics to gradient strength. To work with our distortion correction code, you should scale each
+        gradient by 1/gradient_strength in mT/m; e.g. if the gradient strength is 10 mT/m then scale should be 1/10
+    :type scale: float, optional
+    """
+    def __init__(self, input_Bz_data, r_outer=150, n_order=8, AssessHarmonicPk_Pk=True, QuantifyFit=True,
+                 TrimDataBy_r_outer=False, scale=1):
+
+        # attributes:
+        self._tol = 1e-3  # tolerance for coordinate filtering in mm
+        self.scale = scale
+        self.TrimDataBy_r_outer = TrimDataBy_r_outer
+        self.r_outer = r_outer
+        self.QuantifyFit = QuantifyFit
+        self.AssessHarmonicPk_Pk = AssessHarmonicPk_Pk
+        self.n_order = n_order
+        self.n_harmonics = (self.n_order + 1) ** 2
+        self.input_Bz_data = input_Bz_data.copy()
+        self.__recon_warning_thrown = False
+        # basic fitting routine:
+        self.input_Bz_data = convert_cartesian_to_spherical(self.input_Bz_data)
+        self._check_data_input()
+        if self.TrimDataBy_r_outer:
+            self._filter_data()
+        self._generate_harmonic_names()
+        self.legendre_basis = generate_legendre_basis(self.input_Bz_data, self.n_order)
+        self._svd_fit()
+
+        if not self.scale == 1:
+            logger.warning(f'scaling harmonics by {self.scale}')
+            self.harmonics = self.harmonics*scale
+        if self.QuantifyFit:
+            self._quantify_fit()
+        if self.AssessHarmonicPk_Pk:
+            self._assess_harmonic_pk_pk()
+
+    def _check_data_input(self):
+        """
+        - Make sure the input data actually covers a sphere. If it doesn't, it normally means something has or will go wrong
+            so a warning is triggered.
+        - Make sure that input data is in mm, which is an implicit assumption
+        """
+
+        if not isinstance(self.n_order, int):
+            logger.warning(f'n_order should be integer; round {self.n_order} to {int(self.n_order)}')
+            self.n_order = int(self.n_order)
+
+        if self.input_Bz_data.r.mean() < 10:
+            logger.warning('it appears that your input data is in m, not mm - please use mm!')
+
+        if (self.input_Bz_data.elevation.max() - self.input_Bz_data.elevation.min()) < 0.75 * np.pi or \
+                (self.input_Bz_data.azimuth.max() - self.input_Bz_data.azimuth.min()) < 1.8 * np.pi:
+            logger.warning('input sample points do not appear to cover a full sphere')
+
+    def _filter_data(self):
+        """
+        filter the Bz data by radial coordinate, removing any entries that fall outside self.r_outer
+        """
+
+        data_to_delete_ind = self.input_Bz_data.r > (self.r_outer + self._tol)
+        self.input_Bz_data = self.input_Bz_data.drop(self.input_Bz_data[data_to_delete_ind].index)
+        self.input_Bz_data.reset_index(inplace=True)
+        n_deleted = np.count_nonzero(data_to_delete_ind)
+        if n_deleted > 0:
+            logger.warning(f'deleting {n_deleted} of the original {data_to_delete_ind.size} data points because'
+                           f'they fall outside the r_outer value of {self.r_outer} and TrimDataBy_r_outer=True')
+
+        if self.input_Bz_data.shape[0] == 0:
+            logger.error(f'After filtering for data insdide {self.r_outer} mm, there is no data left!')
+            sys.exit(1)
+
+    def _generate_harmonic_names(self):
+        """
+        generate the names of each harmonic. Used to label the columns in the harmonics dataframe
+        """
+        k = 0
+        self._coeff_names = []
+        for n in range(0, self.n_order + 1):  # the plus 1 is because range stops at -1 for some reason
+            self._coeff_names.append(f'A_{n}_0')
+            k = k + 1
+            for m in range(0, n):
+                self._coeff_names.append(f'A_{n}_{m+1}')
+                k = k + 1
+                self._coeff_names.append(f'B_{n}_{m + 1}')
+                k = k + 1
+
+    def _svd_fit(self):
+        """
+        calculate harmonics using single value decomposition of legendre_basis
+        """
+
+        inverseLegendre = np.linalg.pinv(self.legendre_basis)
+
+        if not np.allclose(inverseLegendre @ self.legendre_basis, np.eye(inverseLegendre.shape[0], self.legendre_basis.shape[1]),
+                           rtol=5e-3, atol=5e-4):
+            # check that the inverse times itself returns an idendity matrix as it should.
+            logger.error('it appears that single value decomposition has failed. This occurs for a few reasons:'
+                         '\n-  Very small or very large data in the input coordinates'
+                         '\n-  The data does not cover a full sphere: hence the matrix is poorly conditioned and has no inverse'
+                         '\n-  Continuing but you should be careful...')
+
+        harmonics = inverseLegendre @ self.input_Bz_data.Bz
+        self.harmonics = pd.Series(harmonics, index=self._coeff_names)
+
+    def _quantify_fit(self):
+        """
+        Compare the reconstructed field to the original field and calculate some basic goodness of fit metrics
+        """
+        if len(self.input_Bz_data.index) > 1e4:
+            logger.warning('you are reconstructing a lot of points and it might be a bit slow.'
+                           'I should write a down sampling routine here...')
+
+        Bz_recon = self.legendre_basis @ (self.harmonics/self.scale)
+        Residual = np.subtract(self.input_Bz_data.Bz, Bz_recon)
+        self._residual_pk_pk = float(abs(Residual.max() - Residual.min())*1e6)
+
+        initial_pk_pk = float(abs(self.input_Bz_data.Bz.max() - self.input_Bz_data.Bz.min()) * 1e6)
+        recon_pk_pk = float(abs(Bz_recon.max() - Bz_recon.min()) * 1e6)
+        residual_percentage = abs(self._residual_pk_pk) * 100 / initial_pk_pk
+
+        try:
+            print(f'Initial pk-pk:       {initial_pk_pk: 1.3e} \u03BCT')
+            print(f'Reconstructed pk-pk: {recon_pk_pk: 1.3e} \u03BCT')
+            print(f'Residual pk-pk:      {self._residual_pk_pk: 1.3e} \u03BCT ({residual_percentage: 1.1f}%)')
+        except UnicodeError:
+            print(f'Initial pk-pk:       {initial_pk_pk: 1.3e} uT')
+            print(f'Reconstructed pk-pk: {recon_pk_pk: 1.3e} uT')
+            print(f'Residual pk-pk:      {self._residual_pk_pk: 1.3e} uT ({residual_percentage: 1.1f}%)')
+
+
+        if residual_percentage > 2:
+            logger.warning('residual_pk_pk is greater than 2 %. This may indicate that the order is not high enough,'
+                           'or that the data is non physical (but it heavily depends on your use case!')
+
+    def _assess_harmonic_pk_pk(self):
+        """
+        generate the peak-peak perturbation caused over the surface of the sphere due to each harmonic
+        """
+        if len(self.legendre_basis.index) < 1e4:
+            # generate some points to ensure we cover a good portion of the sphere
+            r = self.r_outer
+            azimuth = np.linspace(0, 2*np.pi, 100)
+            elevation = np.linspace(0, np.pi, 100)
+            [r, azimuth, elevation] = np.meshgrid(r, azimuth, elevation)
+            coords = pd.DataFrame({'r': r.flatten(), 'azimuth': azimuth.flatten(), 'elevation': elevation.flatten()})
+            legendre_basis_to_use = generate_legendre_basis(coords, self.n_order)
+        else:
+            legendre_basis_to_use = self.legendre_basis
+
+        BasisRange = legendre_basis_to_use.apply(lambda x: abs(np.max(x) - np.min(x)))
+        self.HarmonicsPk_Pk = (self.harmonics/self.scale) * BasisRange * 1e6
+
+    # Public Methods
+
+    def plot_harmonics_pk_pk(self, cut_off=.1):  # pragma: no cover
+        """
+        produces a barplot of harmonics.
+
+        :param cut_off: cutoff point relative to highest harmonic. e.g. cut_off=.1 means that harmonics which produce
+            less than 10% the pk-pk perturbation of the dominant harmonic are ignored.
+        :type cut_off: float, optional
+        """
+
+        if not hasattr(self,'HarmonicsPk_Pk'):
+            self._assess_harmonic_pk_pk()
+        plt.figure(figsize=[10, 5])
+        # ax = sns.barplot(self.HarmonicsPk_Pk, y='pk-pk [\u03BCT]', x=)
+        CutOffInd = abs(self.HarmonicsPk_Pk) < cut_off * abs(self.HarmonicsPk_Pk).max()
+        KeyHarmonics = self.HarmonicsPk_Pk.drop(self.HarmonicsPk_Pk[CutOffInd].index)
+        HarmonicsToPlot = KeyHarmonics
+
+        axs = sns.barplot(x=HarmonicsToPlot.index, y=HarmonicsToPlot.values,  palette="Blues_d")
+        axs.set_title(f'Principle Harmonics pk-pk (>{cut_off*100: 1.0f}% of max)')
+
+        axs.set_ylabel('pk-pk [\u03BCT]')
+        for item in axs.get_xticklabels():
+            item.set_rotation(45)
+        plt.show()
+
+    def plot_cut_planes(self, resolution=2.5, AddColorBar=True, quantity='uT', vmin=None, vmax=None):  # pragma: no cover
+        """
+        Reconstruct the Bz field at the cardinal planes.
+        Note this is basically the same code copied three times in  a row, one for each plane.
+
+        :param resolution: the resolution of reconstructed data. Default is 2.5 mm
+        :type resolution: float, optional
+        :param AddColorBar: Add a color bar to each plot
+        :type AddColorBar: Boolean, optional
+        :param quantity: quantity to use in reconstruct_Bz; must match the options for that function
+        :type quantity: string, optional
+        :param vmin: same as matplotlib.pyplot.imshow; vmin and vmax control the color map bounds.
+        :type vmin: float, optional
+        :param vmax: same as matplotlib.pyplot.imshow; vmin and vmax control the color map bounds.
+        :type vmax: float, optional
+        """
+
+        fig, (axs1, axs2, axs3) = plt.subplots(nrows=1, ncols=3, figsize=(15, 5))
+        extent = [-self.r_outer - resolution, self.r_outer + resolution, -self.r_outer - resolution,
+                  self.r_outer + resolution]  # same for all plots
+
+        conversion_factor = 1
+        # XY plane
+        x = np.linspace(-self.r_outer, self.r_outer, int((2*self.r_outer)/resolution)) * conversion_factor
+        y = np.linspace(-self.r_outer, self.r_outer, int((2*self.r_outer)/resolution)) * conversion_factor
+        z = 0
+        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
+        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
+        recon_coords = convert_cartesian_to_spherical(recon_coords)
+        Bz_recon = reconstruct_Bz(harmonics=self.harmonics/self.scale, coords=recon_coords, quantity=quantity)
+        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(x_recon).shape)
+        XYimage = axs1.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
+        axs1.set_xlabel('x [mm]')
+        axs1.set_ylabel('y [mm]')
+        axs1.set_title('a) XY plane')
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs1.grid(False)
+        axs1.add_artist(draw_circle)
+
+        # ZX plane
+        x = np.linspace(-self.r_outer,self.r_outer,int((2*self.r_outer)/resolution)) * conversion_factor
+        y = 0
+        z = np.linspace(-self.r_outer, self.r_outer, int((2*self.r_outer)/resolution)) * conversion_factor
+        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
+        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
+        recon_coords = convert_cartesian_to_spherical(recon_coords)
+        Bz_recon = reconstruct_Bz(harmonics=self.harmonics/self.scale, coords=recon_coords, quantity=quantity)
+        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(y_recon).shape)
+        ZXimage = axs2.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
+        axs2.set_xlabel('x [mm]')
+        axs2.set_ylabel('z [mm]')
+        axs2.set_title('b) ZX plane')
+        axs2.grid(False)
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs2.add_artist(draw_circle)
+
+        # ZY plane
+        x = 0
+        y = np.linspace(-self.r_outer,self.r_outer,int((2*self.r_outer)/resolution)) * conversion_factor
+        z = np.linspace(-self.r_outer,self.r_outer,int((2*self.r_outer)/resolution)) * conversion_factor
+        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
+        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
+        recon_coords = convert_cartesian_to_spherical(recon_coords)
+        Bz_recon = reconstruct_Bz(harmonics=self.harmonics/self.scale, coords=recon_coords, quantity=quantity)
+        Bz_recon = Bz_recon.to_numpy().reshape(np.squeeze(z_recon).shape)
+        ZYimage = axs3.imshow(Bz_recon.T, extent=extent, vmin=vmin, vmax=vmax)
+        axs3.set_xlabel('y [mm]')
+        axs3.set_ylabel('z [mm]')
+        axs3.grid(False)
+        axs3.set_title('c) ZY plane')
+        draw_circle = plt.Circle((0, 0), 150, fill=False)
+        axs3.add_artist(draw_circle)
+
+        if AddColorBar:
+            if quantity == 'uT':
+                cb_title = '\u03BCT'
+            elif quantity == 'T':
+                cb_title = 'T'
+            cbar = fig.colorbar(XYimage, ax=axs1, fraction=0.046, pad=0.04)
+            cbar.set_label(cb_title)
+            cbar = fig.colorbar(ZXimage, ax=axs2, fraction=0.046, pad=0.04)
+            cbar.set_label(cb_title)
+            cbar = fig.colorbar(ZYimage, ax=axs3, fraction=0.046, pad=0.04)
+            cbar.set_label(cb_title)
+
+        plt.tight_layout()
+        plt.show()
+
+    def print_key_harmonics(self, cut_off=.01):
+        """
+        print the harmonics with value > cut_off to the terminal in pk-pk.
+
+        :param cut_off: cutoff point relative to highest harmonic. e.g. cut_off=.1 means that harmonics which produce
+            less than 10% the pk-pk perturbation of the dominant harmonic are ignored.
+        :type cut_off: float, optional
+        """
+        if not hasattr(self, 'harmonics_pk_pk'):
+            self._assess_harmonic_pk_pk()
+
+
+        CutOffInd = abs(self.HarmonicsPk_Pk) < cut_off * abs(self.HarmonicsPk_Pk).max()
+        KeyHarmonics = self.HarmonicsPk_Pk.drop(self.HarmonicsPk_Pk[CutOffInd].index)
+        pd.set_option('display.float_format', lambda x: '%1.4ef' % x)
+        print(f'\nOnly displaying values >= {cut_off*100: 1.0f}% of the peak harmonic.')
+        try:
+            print('Values are in pk=pk [\u03BCT]')
+        except UnicodeError:
+            print('Values are in pk=pk uT]')
+        print(f'{bcolors.OKBLUE}{KeyHarmonics.to_string()}{bcolors.ENDC}')
+
+
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/MarkerAnalysis.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/MarkerAnalysis.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,1221 +1,1076 @@
-import pathlib
-import time
-
-from .utilities import get_all_files, dicom_to_numpy
-import pydicom
-from pathlib import Path
-import numpy as np
-from skimage.filters import gaussian, threshold_otsu
-from skimage.measure import label
-from scipy.interpolate import NearestNDInterpolator
-from matplotlib import pyplot as plt
-import logging
-import os
-import json
-import pandas as pd
-from scipy.spatial.distance import cdist
-from scipy.spatial import transform
-from datetime import datetime
-from warnings import warn
-
-ch = logging.StreamHandler()
-formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
-ch.setFormatter(formatter)
-logger = logging.getLogger(__name__)
-logger.addHandler(ch)
-logger.setLevel(logging.INFO)
-logger.propagate = False
-
-
-class MarkerVolume:
-    """
-    This class excepts either a path to a folder of dicom files or a numpy array of marker positions.
-    In the former case, it will attempt to automatically extract the marker positions. In the latter, it will just
-    use the input marker positions. Once the instance is created, it contains a number of handy plots and functions.
-
-    :param input_data_path: Either a path to a folder of dicoms, or a numpy array with three columns corresponding to the
-        [x,y,z] marker positions
-    :type input_data_path: path, string, np.ndarray
-    :param ImExtension: change to whatever extension your dicom files, most commonly either dcm or IMA
-    :type ImExtension: str, optional
-    :param r_min: any markers at radii less than this will be discounted.
-    :type r_min: float ,optional
-    :param r_max: any markers at radii greater than this will be discounted.
-    :type r_max: float, optional
-    :param iterative_segmentation: If set to true, a slower iterative method will be used to find the threshold value
-        used to segment the markers. Otherwise, otsu's method is used.
-    :type iterative_segmentation: bool, optional
-    :param threshold: Manually set the threshold value. If this is left as None otsu's method is used.
-        This will replace the iterative segmentation method regardless of flag.
-    :type threshold: float, optional
-    :param n_markers_expected: if you know how many markers you expect, you can enter the value here. The code will
-        then warn you if it finds a different number.
-    :type n_markers_expected: int, optional
-    :param gaussian_image_filter_sd: size of filter to blur input data with. Higher values are better at removing
-        noise prior to thresholding, but may also blur out small/low signal markers!
-    :type gaussian_image_filter_sd: float, optional
-    :param correct_fat_water_shift: if True, will attempt to automatically correct marker positions for calculated
-        fat water shift
-    :type correct_fat_water_shift: bool, optional
-    :param marker_size_lower_tol: lower acceptance window for a marker compared to the median size of markers.
-        e.g. markermarker_size_tol=0.5 will result in markers being accepted within when
-        (1-marker_size_lower_tol)*median_marker_size <= marker_size <= (1+markermarker_size_tol)*marker_size_upper_tol
-    :type marker_size_lower_tol: float, optional
-    :param marker_size_upper_tol: upper acceptance window for a marker compared to the median size of markers.
-    :type marker_size_upper_tol: float, optional
-    :param verbose: if True, prints a lot of info about the marker extraction process to the screen. mostly useful
-        during debugging
-    :type verbose: bool, optional
-    :param fat_shift_direction: We aren't sure yet if we can confidently predict the direction that the fat water shift
-        will be in. if you set correct_fat_water_shift=True, you can change the direction it shifts in here. it should
-        take a value of -1, or 1. pull requests making this easier to use very welcome!
-    :type fat_shift_direction: int, optional
-    """
-
-    def __init__(self, input_data, ImExtension='dcm', r_min=None, r_max=None, iterative_segmentation=False,
-                 threshold=None, n_markers_expected=None, fat_shift_direction=None, verbose=False,
-                 gaussian_image_filter_sd=1, correct_fat_water_shift=False, marker_size_lower_tol=0.9,
-                 marker_size_upper_tol=1):
-
-        self.verbose = verbose
-        self._file_extension = ImExtension
-        self._correct_fat_water_shift = correct_fat_water_shift
-        self.dicom_data = None  # overwritten below if possible.
-        self._n_markers_expected = n_markers_expected
-        self._r_min = r_min
-        self._r_max = r_max
-        self._cutoffpoint = threshold
-        self._iterative_segmentation = iterative_segmentation
-        self._chemical_shift_vector = None
-        self._gaussian_image_filter_sd = gaussian_image_filter_sd
-        self._marker_size_lower_tol = marker_size_lower_tol
-        self._marker_size_upper_tol = marker_size_upper_tol
-
-        if isinstance(input_data, (pathlib.Path, str)):
-            self.input_data_path = Path(input_data)
-            if self.input_data_path.is_dir():
-                # dicom input
-                self.InputVolume, self.dicom_affine, (self.X, self.Y, self.Z) = \
-                    dicom_to_numpy(self.input_data_path, file_extension=self._file_extension, return_XYZ=True)
-                self._get_MR_acquisition_data()
-
-                # Segmenting markers
-                self._filter_volume_by_r()
-                start_time = time.perf_counter()
-                self.ThresholdVolume, self.BlurredVolume = self._threshold_volume(self.InputVolume)
-                centroids = self._find_contour_centroids()
-                self.MarkerCentroids = pd.DataFrame(centroids, columns=['x', 'y', 'z'])
-                end_time = time.perf_counter()
-                print(f'total segmentation time: {end_time - start_time: 1.1f} s')
-
-                # Correct for oil water shift
-                if self._correct_fat_water_shift:
-                    self._calculate_chemical_shift_vector(fat_shift_direction=fat_shift_direction)
-                    self.MarkerCentroids = self.MarkerCentroids + self._chemical_shift_vector
-            elif (os.path.isfile(self.input_data_path) and os.path.splitext(self.input_data_path)[1] == '.json'):
-                # slicer input
-                with open(self.input_data_path) as f:
-                    data = json.load(f)
-                arrays = [el for el in data['markups'][0]['controlPoints']]
-                points = [el['position'] for el in arrays]
-                self.MarkerCentroids = pd.DataFrame(points, columns=['x', 'y', 'z'])
-
-                # look for dicom_data json file
-                try:
-                    with open(os.path.join(self.input_data_path.parent, 'dicom_data.json')) as f:
-                        self.dicom_data = json.load(f)
-                except:
-                    logger.warning(
-                        f'MR data file dicom_data.json not found at {self.input_data_path.parent}. Continuing')
-            else:
-                raise FileNotFoundError(f'could not find any data at {self.input_data_path}')
-        elif isinstance(input_data, np.ndarray):
-            # don't need to do anything then.
-            self.MarkerCentroids = pd.DataFrame(input_data, columns=['x', 'y', 'z'])
-            logger.warning("numpy input is deprecated, please use pandas input with ['x', 'y', 'z'] cols instead")
-        elif isinstance(input_data, pd.core.frame.DataFrame):
-            _expected_columns = ['x', 'y', 'z']
-            if not all([col in input_data for col in _expected_columns]):
-                raise AttributeError("input pandas data must have columns called ['x', 'y', 'z']")
-            self.MarkerCentroids = input_data.copy()
-        else:
-            raise TypeError(f'Uknown data input: {type(input_data)}')
-
-        # insert the radial value of each marker:
-        self.MarkerCentroids['r'] = self.MarkerCentroids.apply(
-            lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
-        if self.MarkerCentroids.r.mean() < 10:
-            logger.warning('it appears that your input data is in m, not mm - please use mm!')
-
-        self._filter_markers_by_r()
-        if self._n_markers_expected is not None:
-            if not (self.MarkerCentroids.shape[0] == n_markers_expected):
-                logger.warning(f'For data {self.input_data_path}\n'
-                               f'You entered that you expected to find'
-                               f' {n_markers_expected}, but actually found {self.MarkerCentroids.shape[0]}.')
-
-    def _filter_volume_by_r(self):
-        """
-        Accelerates and improves segmenting by setting all voxels outside of specified radius to the background
-        """
-        if self._r_max or self._r_min:
-            _max = 10000
-            _min = -1
-            if self._r_max:
-                _max = self._r_max
-            if self._r_min:
-                _min = self._r_min
-            background = np.median(self.InputVolume)
-
-            it = np.nditer(self.InputVolume, flags=['multi_index'])
-            for voxel in it:
-                distance = np.sqrt(
-                    self.X[it.multi_index] ** 2 + self.Y[it.multi_index] ** 2 + self.Z[it.multi_index] ** 2)
-                if distance < _min or distance > _max:
-                    self.InputVolume[it.multi_index] = background
-
-    def _filter_markers_by_r(self):
-        """
-        Remove any markers that are less than r_min or more than r_max
-        """
-        if self._r_max:
-            keep_ind = abs(self.MarkerCentroids.r) < self._r_max
-            self.MarkerCentroids = self.MarkerCentroids[keep_ind].reset_index(drop=True)
-        if self._r_min:
-            keep_ind = abs(self.MarkerCentroids.r) > self._r_min
-            self.MarkerCentroids = self.MarkerCentroids[keep_ind].reset_index(drop=True)
-
-    def _get_MR_acquisition_data(self):
-        """
-        If we have MR images, extract the information from thall_dicom_files = get_all_files(self.input_data_path)e
-        dicom header that is needed to convert marker positions to magnetic fields downstream.
-        - This method is dependant on having the full coordinate list which are calculated upstream; this is why it
-            must reside inside this class.
-        - We include many fields that aren't in the dicom header by default
-        - we package this as a simple dict that can be easily saved as json
-        """
-        all_dicom_files = get_all_files(self.input_data_path, file_extension=self._file_extension)
-        # use first one that has pixel data:
-        j = 0
-        while True:
-            example_dicom_file = pydicom.read_file(self.input_data_path / all_dicom_files[j])
-            try:
-                test = example_dicom_file.pixel_array
-                break
-            except AttributeError:
-                j += 1
-
-        if example_dicom_file.Modality == 'MR':
-            if not example_dicom_file.Manufacturer == 'SIEMENS':
-                logger.warning(
-                    'this code has not been tested with non-siemens scanners. If dicom standards work properly'
-                    'this code will too...')
-            x = np.unique(self.X)
-            y = np.unique(self.Y)
-            z = np.unique(self.Z)
-            x_pixel_spacing = np.mean(np.diff(x))
-            y_pixel_spacing = np.mean(np.diff(y))
-            z_pixel_spacing = np.mean(np.diff(z))
-            x_fov = x.max() - x.min() + x_pixel_spacing
-            y_fov = y.max() - y.min() + y_pixel_spacing
-            z_fov = z.max() - z.min() + z_pixel_spacing
-            self._dicom_header = example_dicom_file
-
-            self.dicom_data = {}  # fill up below
-            self.dicom_data['FOV'] = [x_fov, y_fov, z_fov]
-            self.dicom_data['bandwidth'] = float(example_dicom_file.PixelBandwidth)
-
-            self.dicom_data['gama'] = float(example_dicom_file.MagneticFieldStrength * 42.57747851)
-            self.dicom_data['pixel_spacing'] = [x_pixel_spacing, y_pixel_spacing, z_pixel_spacing]
-            self.dicom_data['image_size'] = [x.size, y.size, z.size]
-            self.dicom_data['magnetic_field_strength'] = example_dicom_file.MagneticFieldStrength
-            self.dicom_data['imaging_frequency'] = example_dicom_file.ImagingFrequency
-            try:
-                acquisition_date = datetime.strptime(example_dicom_file.AcquisitionDate, '%Y%m%d')
-                self.dicom_data['acquisition_date'] = acquisition_date.strftime("%d_%B_%Y")
-            except ValueError as e:
-                logger.error(e)
-                logger.error('failed to extract datetime, probably didnt understand date format, continuing...')
-            self.dicom_data['manufacturer'] = example_dicom_file.Manufacturer
-            try:
-                self.dicom_data['sequence_name'] = example_dicom_file.SequenceName
-            except AttributeError:
-                pass
-            try:
-                self.dicom_data['sequence_name'] = example_dicom_file.ScanningSequence
-            except AttributeError:
-                pass
-            # the above works on siemens scanner, not sure if it will prove consistent on others
-            fat_water_delta_f = example_dicom_file.MagneticFieldStrength * 42.57747851 * 3.5
-            self.dicom_data['chem_shift_magnitude'] = (example_dicom_file.PixelBandwidth / fat_water_delta_f) / 2
-            self.dicom_data['InPlanePhaseEncodingDirection'] = example_dicom_file.InPlanePhaseEncodingDirection
-            # extract the frequency, phase, and slice directions (B0 effects occur in freq and slice)
-            directions = ['x', 'y', 'z']
-            phase_encode_direction = None
-            freq_encode_direction = None
-            if self.dicom_data['InPlanePhaseEncodingDirection'] == 'ROW':
-                phase_cosines = example_dicom_file.ImageOrientationPatient[:3]
-                row_cosines = example_dicom_file.ImageOrientationPatient[3:]
-            elif self.dicom_data['InPlanePhaseEncodingDirection'] == 'COL':
-                phase_cosines = example_dicom_file.ImageOrientationPatient[3:]
-                row_cosines = example_dicom_file.ImageOrientationPatient[:3]
-            for i, (phase_cosine, freq_cosine) in enumerate(zip(phase_cosines, row_cosines)):
-                if abs(float(phase_cosine)) == 1:
-                    phase_encode_direction = directions[i]
-                if abs(float(freq_cosine)) == 1:
-                    freq_encode_direction = directions[i]
-            if phase_encode_direction is None:
-                logger.warning('failed to extract phase encoding direction from dicom data, continuing')
-            if freq_encode_direction is None:
-                logger.warning('failed to extract frequency encoding direction from dicom data, continuing')
-            self.dicom_data['phase_encode_direction'] = phase_encode_direction
-            self.dicom_data['freq_encode_direction'] = freq_encode_direction
-            # get slice direction
-            slice_dir_ind = np.equal(example_dicom_file.ImageOrientationPatient[:3],
-                                     example_dicom_file.ImageOrientationPatient[3:])
-            self.dicom_data['slice_direction'] = np.array(directions)[slice_dir_ind][0]
-            bandwidth = np.array(self.dicom_data['bandwidth'])
-            image_size = np.array(self.dicom_data['image_size'])
-            gama = np.array(self.dicom_data['gama'])
-            FOV = np.array(self.dicom_data['FOV'])
-            gradient_strength = bandwidth * image_size / (gama * 1e6 * FOV * 1e-3)  # unit(T / m)
-            self.dicom_data['gradient_strength'] = list(gradient_strength)
-
-        else:
-            self.dicom_data = None
-
-    def _calculate_chemical_shift_vector(self, fat_shift_direction=1):
-        """
-        Calculates a chemical shift vector (x,y,z) to be applied to each marker to account for the fat/water shift.
-
-        :param fat_shift_direction: dictates whether the shift is positive or negative. we aren't sure how consisten
-            this is between scanners so have left as used defined.
-        """
-        if self.dicom_data is None:
-            logger.warning('No dicom data for chemical shift')
-            return
-
-        # TODO check these
-        if fat_shift_direction == 'AP' or fat_shift_direction == 'RL' or fat_shift_direction == 'FH' or fat_shift_direction == -1:
-            fat_shift_direction = -1
-        elif fat_shift_direction == 'PA' or fat_shift_direction == 'LR' or fat_shift_direction == 'HF' or fat_shift_direction == 1:
-            fat_shift_direction = 1
-        else:
-            fat_shift_direction = 0
-            logger.warning('Chemical shift input was invalid')
-
-        # Calculate magnitude (in pixels) of the chemical shift based on the shift frequency of a 1T MRI field (149Hz)
-        directions = ['x', 'y', 'z']
-        direction = np.array(([int(el == self.dicom_data['freq_encode_direction']) for el in directions]))
-        # ^ this just gives a vector with a 1 in the correct direction e.g. [0,1,0]
-        shift = direction * self.dicom_data['chem_shift_magnitude']
-        self._chemical_shift_vector = shift * np.array(self.dicom_data['pixel_spacing'])[
-            direction.astype(bool)] * fat_shift_direction
-
-    def _find_iterative_cutoff(self, blurred_volume):
-        """
-        Replaces the otsu threshold with a slower, iterative method to find the best threshold for segmenting markers.
-        A range of valid thresholds are found and the mean is returned as the best threshold.
-        If no valid thresholds are found, the mean of candidate thresholds that will miss some markers is returned.
-        """
-
-        if self._n_markers_expected is None:
-            logger.warning('Iterative segmentation method requires the expected number of markers to be input.')
-            return None
-
-        # finds a range of thresholds that give a number of segments near to the number of expected markers
-        histogram_division = 100
-
-        candidate_thresholds = []  # Thresholds that have fewer markers than expected, use when no valid thresholds
-        candidate_n_points = []
-        valid_thresholds = []  # Thresholds that should give the corrected number of markers
-
-        # divide the range into segments and calculate how many volumes result from each segment
-        background_value = np.median(np.round(blurred_volume))
-        intensity_range = np.max(blurred_volume) - background_value
-        histogram_segment = intensity_range / histogram_division
-
-        # Testing each histogram segment
-        for i in range(1, histogram_division - 1):
-
-            n_segments = 0
-            cutoff = background_value + i * histogram_segment
-            threshold_volume = blurred_volume > cutoff
-            labels = label(threshold_volume, background=0)
-            unique_labels = np.unique(labels)[1:]  # first label is background so skip
-            # Check number of segments falls within valid range:
-            tol = 0.1
-            if len(unique_labels) < self._n_markers_expected * (1 - tol) or len(
-                    unique_labels) > self._n_markers_expected * (1 + tol):
-                continue  # Too few or too many segments
-            else:
-                # This threshold is possibly valid
-                candidate_thresholds.append(cutoff)
-                # Remove small volumes and check if still valid
-                for label_level in unique_labels:
-                    RegionInd = labels == label_level
-                    if np.count_nonzero(RegionInd) > 2:
-                        n_segments += 1
-                candidate_n_points.append(n_segments)
-                if n_segments >= self._n_markers_expected:
-                    valid_thresholds.append(cutoff)
-                    if self.verbose:
-                        print('Threshold: ' + str(format(cutoff, '.2f')) + ', ' + str(n_segments) + ' segments.')
-                else:
-                    if self.verbose:
-                        print('Threshold: ' + str(format(cutoff, '.2f')) + ' is a candidate.')
-
-            if len(unique_labels) < 10:
-                # threshold is too high and we can stop
-                break
-
-        if valid_thresholds:
-            print(f'Using thresold of {np.mean(valid_thresholds): 1.1f}')
-            return np.mean(valid_thresholds)
-        elif len(candidate_thresholds) > 0:
-            ind = np.argmin(abs(np.subtract(self._n_markers_expected, candidate_n_points)))
-            best_threshold = candidate_thresholds[ind]
-            logger.warning(f'No valid thresholds were found. Using closest possible value of {best_threshold}')
-            return best_threshold
-        else:
-            logger.warning('No valid thresholds were found. Try lowering gaussian blur level.')
-            return None
-
-    def _threshold_volume(self, VolumeToThreshold):
-        """
-        For a 3D numpy array, turn all elements < cutoff to zero, and all other elements to 1.
-        If no cutoff is entered, otsu's method is used to auto-threshold.
-        """
-
-        BlurredVolume = gaussian(VolumeToThreshold, sigma=self._gaussian_image_filter_sd)
-
-        if self._cutoffpoint is not None:
-            # If cutoff point has been manually entered, go straight to thresholding
-            self._iterative_segmentation = False
-        if self._iterative_segmentation is True:
-            self._cutoffpoint = self._find_iterative_cutoff(BlurredVolume)
-        if self._cutoffpoint is None:
-            self._cutoffpoint = threshold_otsu(BlurredVolume)
-
-        ThresholdVolume = BlurredVolume > self._cutoffpoint
-
-        return ThresholdVolume, BlurredVolume
-
-    def _get_marker_max_min_volume(self):
-        """
-        figures out the range of voxels that a marker should have
-        """
-        self._n_voxels = []  # going to keep track of this so we can remove any very small regions if needed
-
-        for label_level in self.unique_labels:  # first label is background so skip
-            # extract x,y,z of each connected region
-            RegionInd = self._labels == label_level
-            self._n_voxels.append(np.count_nonzero(RegionInd))
-        # Set up min and max marker volumes
-        self._n_voxels_median = np.median(np.array(self._n_voxels))
-        self._voxel_min = (1 - self._marker_size_lower_tol) * self._n_voxels_median
-        self._voxel_max = (1 + self._marker_size_upper_tol) * self._n_voxels_median
-
-        # Modify based on number of markers
-        if self._n_markers_expected is not None:
-            self._n_voxels_copy = np.array(self._n_voxels)
-            voxel_difference = np.absolute(np.array(self._n_voxels) - self._n_voxels_median)
-            # Loop that deletes the marker size with the largest difference from median until the expected # of markers
-            while len(self._n_voxels_copy) > self._n_markers_expected:
-                self._n_voxels_copy = np.delete(self._n_voxels_copy, np.argmax(voxel_difference))
-                voxel_difference = np.delete(voxel_difference, np.argmax(voxel_difference))
-            # Set min and max based on the remaining list
-            if np.min(self._n_voxels_copy) > self._voxel_min:
-                self._voxel_min = np.min(self._n_voxels_copy)
-            if np.max(self._n_voxels_copy) < self._voxel_max:
-                self._voxel_max = np.max(self._n_voxels_copy)
-
-        # 3 voxels is the absolute floor
-        if self._voxel_min < 3:
-            self._voxel_min = 3
-
-    def _remove_load(self):
-        '''
-        if it seems very likely that the only thing that has been segmented is the load
-        remove it and try again. We may want to enable this in situations where any large object is detected...
-        '''
-
-        for label_level in self.unique_labels:
-            RegionInd = self._labels == label_level
-            self.InputVolume[RegionInd] = 0
-        self._cutoffpoint = None
-        self.ThresholdVolume, self.BlurredVolume = self._threshold_volume(self.InputVolume)
-        self._labels = label(self.ThresholdVolume, background=0)
-        self.unique_labels = np.unique(self._labels)[1:]  # first label is background so skip
-
-    def _print_thresholding_information(self):
-        print('Threshold value: ' + str(self._cutoffpoint))
-        print('Median marker volume: ' + str(self._n_voxels_median))
-        print('Expected marker volume: ' + str(self._voxel_min) + ' to ' + str(self._voxel_max))
-        print(f'Regions to check: {self.unique_labels.shape}')
-
-    def _print_thresholding_summary(self, n_found_markers, n_skipped_markers):
-        print('----------')
-        print(f'Total regions: {len(self.unique_labels)}')
-        print(f'Total markers found:   {n_found_markers}')
-        print(f'Total skipped:         {n_skipped_markers}')
-
-    def _find_contour_centroids(self):
-        """
-        This code loops through all the found regions, extracts the cartesian coordiantes, and takes the
-        intensity-weighted average as the centroid.
-        It excludes volumes that are bigger/ smaller than the median using the params
-        marker_size_upper_tol and marker_size_lower_tol
-        """
-        self._labels = label(self.ThresholdVolume, background=0)
-        self.unique_labels = np.unique(self._labels)[1:]  # first label is background so skip
-        if self.unique_labels.shape[0] < 3:
-            logger.warning('automatic thresholding didnt work, trying to remove load and try again...')
-            self._remove_load()
-        self._get_marker_max_min_volume()
-
-        if self.verbose:
-            self._print_thresholding_information()
-
-        x_centroids = []
-        y_centroids = []
-        z_centroids = []
-        skipped = 0
-
-        # extract x,y,z of each connected region
-        for i, label_level in enumerate(self.unique_labels):
-            RegionInd = np.equal(self._labels, label_level)
-            voxels = np.count_nonzero(RegionInd)
-            if voxels < self._voxel_min or voxels > self._voxel_max:
-                skipped += 1
-                if self.verbose:
-                    print('\033[93mRegion ' + str(i + 1) + ': Skipped, v = ' + str(voxels) + '\033[0m')
-                continue  # skip outliers
-
-            region_sum = np.sum(self.InputVolume[RegionInd])
-            weighted_x = np.sum(np.multiply(self.X[RegionInd], self.InputVolume[RegionInd]))
-            weighted_y = np.sum(np.multiply(self.Y[RegionInd], self.InputVolume[RegionInd]))
-            weighted_z = np.sum(np.multiply(self.Z[RegionInd], self.InputVolume[RegionInd]))
-            x_centroids.append(weighted_x / region_sum)
-            y_centroids.append(weighted_y / region_sum)
-            z_centroids.append(weighted_z / region_sum)
-            if self.verbose:
-                print('Region ' + str(i + 1) + ': Marker, v = ' + str(voxels))
-
-        if self.verbose:
-            self._print_thresholding_summary(len(x_centroids), skipped)
-
-        return np.array([x_centroids, y_centroids, z_centroids]).T
-
-    # public methods
-
-    def rotate_markers(self, xaxis_angle=0, yaxis_angle=0, zaxis_angle=0):
-        """
-        rotate markers using euler angles
-
-        :param xaxis_angle: rotation around x angle in degrees
-        :param yaxis_angle: rotation around y angle in degrees
-        :param zaxis_angle: rotation around z angle in degrees
-        """
-
-        rotate = np.array([xaxis_angle, yaxis_angle, zaxis_angle], dtype=np.int16)
-        rotation_vector = transform.Rotation.from_euler('xyz', rotate, degrees=True)
-        # Transform centroids
-        rotated = rotation_vector.apply(self.MarkerCentroids[['x', 'y', 'z']])
-        self.MarkerCentroids = pd.DataFrame(rotated, columns=['x', 'y', 'z'])
-        self.MarkerCentroids['r'] = self.MarkerCentroids.apply(
-            lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
-
-    def translate_markers(self, x_shift=0, y_shift=0, z_shift=0):
-        """
-        translate markers
-
-        :param x_shift: x translation in mm
-        :param y_shift: y translation in mm
-        :param z_shift: z translation in mm
-        :return:
-        """
-        translate = np.array([x_shift, y_shift, z_shift], dtype=np.int16)
-        translated = self.MarkerCentroids[['x', 'y', 'z']] + translate
-        self.MarkerCentroids = pd.DataFrame(translated, columns=['x', 'y', 'z'])
-        self.MarkerCentroids['r'] = self.MarkerCentroids.apply(
-            lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
-
-    def plot_3D_markers(self, title='3D marker positions'):  # pragma: no cover
-        """
-        Just a quick plot of the marker positions; very useful sanity check!
-        """
-
-        fig = plt.figure()
-        axs = fig.add_subplot(111, projection='3d')
-        axs.scatter(self.MarkerCentroids.x, self.MarkerCentroids.y, self.MarkerCentroids.z, s=10)
-        axs.set_xlabel('X [mm]')
-        axs.set_ylabel('Y [mm]')
-        axs.set_zlabel('Z [mm]')
-        axs.set_title(title)
-        axs.set_box_aspect(
-            (np.ptp(self.MarkerCentroids.x), np.ptp(self.MarkerCentroids.y), np.ptp(self.MarkerCentroids.z)))
-        plt.show()
-
-    def perturb_marker_positions(self, random_perturbation, systemic_perturbation=0):
-        """
-        add random noise to the marker positions. Useful to perform sensitivity analysis. operates in place.
-
-        :param random_perturbation: upper and lower limits of random_perturbation to each marker coordinates. uniform
-            distribution is used
-        :type random_perturbation: float
-        :param systemic_perturbation: constant offset added to all markers
-        :type systemic_perturbation: float, optional
-        """
-
-        x_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
-                                     size=self.MarkerCentroids.x.shape)
-        y_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
-                                     size=self.MarkerCentroids.x.shape)
-        z_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
-                                     size=self.MarkerCentroids.x.shape)
-        self.MarkerCentroids.x = self.MarkerCentroids.x + x_peturb + systemic_perturbation
-        self.MarkerCentroids.y = self.MarkerCentroids.y + y_peturb + systemic_perturbation
-        self.MarkerCentroids.z = self.MarkerCentroids.z + z_peturb + systemic_perturbation
-
-    def export_to_slicer(self, save_path=None, filename='slicer_centroids'):
-        """
-        export a json file that can be read in by slicer, allowing a good way to visualise marker segmentation
-        performance. This file will be saved at the same spot as input data if dicom was input, otherwise it will be
-        saved to save_path.
-        """
-        # sort out where to save:
-        if save_path is None:
-            try:
-                _save_path = self.input_data_path
-            except AttributeError:  # indicates numpy input
-                logger.error('To save numpy data to slicer format, please enter a value for "save_path" when'
-                             'calling MarkerVolume.export_to_slicer')
-                return
-        else:
-            _save_path = Path(save_path)
-
-        file_content = []  # will fill up one line at a time
-        file_content.append('{"@schema": "https://raw.githubusercontent.com/slicer/slicer/master/Modules/Loadable/'
-                            'Markups/Resources/Schema/markups-schema-v1.0.0.json#",\n')
-        file_content.append('"markups": [{"type": "Fiducial", "coordinateSystem": "LPS", "controlPoints": [\n')
-        for index, row in self.MarkerCentroids.iterrows():
-            if index == self.MarkerCentroids.shape[0] - 1:
-                # for last entry have to delete a comma
-                file_content.append(
-                    f'{{ "label": " ", "position": [{row.x: 1.2f}, {row.y: 1.2f}, {row.z: 1.2f}], "locked": true}}\n')
-            else:
-                file_content.append(
-                    f'{{ "label": " ", "position": [{row.x: 1.2f}, {row.y: 1.2f}, {row.z: 1.2f}], "locked": true}},\n')
-
-        file_content.append(']}]}')
-        # write contents
-        filename = filename + '.mrk.json'
-        file_loc = _save_path / filename
-        with open(file_loc, 'w') as f:
-            f.writelines(file_content)
-
-    def save_dicom_data(self, save_path=None, filename='dicom_data'):
-        """
-        save the dicom data as json.  This file will be saved at the same
-        spot as input data if dicom was input, otherwise it will be saved
-        to save_path.
-        """
-
-        if self.dicom_data is None:
-            logger.warning('cannot save dicom data because there is none...')
-            return
-        if save_path is None:
-            save_path = self.input_data_path
-        save_path = Path(save_path)
-        _file_name, _file_extension = os.path.splitext(filename)
-        if _file_extension == '':
-            _file_extension = '.json'
-        filename = _file_name + _file_extension
-        full_filename = save_path / filename
-
-        with open(full_filename, 'w') as f:
-            json.dump(self.dicom_data, f)
-
-
-class MatchedMarkerVolumes:
-    """
-    :param GroundTruthData:
-    :type GroundTruthData: MarkerVolume object, or path to dicom folder, or numpy array
-    :param DistortedData:
-    :type DistortedData: MarkerVolume object, or path to dicom folder, or numpy array
-    :param reverse_gradient_data:
-    :type reverse_gradient_data: None, or MarkerVolume object, or path to dicom folder, or numpy array
-    :param WarpSearchData: if True, position of found markers is used to update expected positions for ground truth.
-        Recomended is True if there is substantial distortion present.
-    :type WarpSearchData: boolean
-    :param AutomatchMarkers: if True, will automatically match the distorted data to the ground truth using a search
-        algorith. If False, will simply use input data in the order it is entered. This is useful if you have sets
-        of markers that were independently matched through some other process.
-    :type AutomatchMarkers: boolean
-    :param AllowDoubleMatching: when False, each ground truth marker is only allowed to match with one distorted
-        marker. However, sometimes this can result in a chain reaction where one marker gets mismatched then every
-        other marker gets mismatched too. In these cases you can set this parameter to True, and any double matched
-        markers will simply be deleted.
-    :type AllowDoubleMatching: bool, optional
-    :param sorting_method: 'radial' or 'nearest'. This is only important if WarpSearchData is True; in that case,
-        we are building a motion model on-the-fly based on previously seen markers, so the order we see them can be
-        important. For data on a sphere, you may have more success by setting this to 'nearest', but this is a bit
-        of an untested feature
-    :type sorting_method: str, optional
-    :param n_refernce_markers: the n inner_most Reference markers are used to align the ground truth to the MR volume
-        before  matching. this can correct for setup errors. Note that we always move the reference. the best way
-        for this to not matter either way is to not have any set up error!
-    :type n_refernce_markers: int, optional
-    :param skip_unmatchable_markers: if true, distorted markers where the nearest centroid marker is above the maximum
-        distortion threshold are removed
-    :type skip_unmatchable_markers: bool, optional
-    """
-
-    def __init__(self, GroundTruthData, DistortedData, reverse_gradient_data=None, WarpSearchData=True,
-                 AutomatchMarkers=True, AllowDoubleMatching=False, sorting_method='radial', n_refernce_markers=0,
-                 skip_unmatchable_markers=True):
-
-        # warping parameters:
-        self.WarpSearchData = WarpSearchData
-        self.AutomatchMarkers = AutomatchMarkers
-        self._motion_estimate_update_rate = 1  # 1 = every found marker, which is potentially more accurate but slower.
-        self.sorting_method = sorting_method
-        self.AllowDoubleMatching = AllowDoubleMatching
-
-        # match check parameters:
-        self._mean_match_tolerance = 20  # warning raised if mean larger than this
-        self._max_match_tolerance = 30  # warning raised if max larger than this
-
-        self._skip_unmatchable_markers = skip_unmatchable_markers
-        self._n_reference_markers = n_refernce_markers
-
-        # marker data:
-        self.ground_truth_centroids = GroundTruthData.MarkerCentroids
-        self.distorted_centroids = DistortedData.MarkerCentroids
-
-        if reverse_gradient_data is None:
-            self.distorted_centroidsRev = None
-        else:
-            self.distorted_centroidsRev = reverse_gradient_data.MarkerCentroids
-
-
-        # run analysis:
-        if self._n_reference_markers > 0:
-            self._align_reference()
-        if self._skip_unmatchable_markers:
-            self._remove_unmatchable_distorted_centroids()
-        self._check_input_data()
-
-
-
-        if self.AutomatchMarkers:
-            self.distorted_centroids = self._sort_distorted_centroids(self.distorted_centroids)
-            self._CentroidMatch = self._match_distorted_markers_to_ground_truth(self.distorted_centroids)
-            self._check_match()
-            if self.distorted_centroidsRev is not None:
-                self.distorted_centroidsRev = self._sort_distorted_centroids(self.distorted_centroidsRev)
-                self._CentroidMatchRev = self._match_distorted_markers_to_ground_truth(self.distorted_centroidsRev)
-        else:
-            self._create_marker_data_prematched_markers()
-        self._handle_double_matched_markers()
-
-        # analyse marker positions
-        self._generate_marker_position_data()
-
-    def _check_input_data(self):
-        """
-        put any tests on the input data here to make sure the rest of the code can run.
-
-        - tests that there at least as many ground truth centroids than distorted centroids
-        - tests that data appears to be in mm (requirement)
-        """
-        if not self.ground_truth_centroids.shape[0] >= self.distorted_centroids.shape[0]:
-            raise ValueError('There are fewer ground truth centroids than distorted centroids; this means the disorted'
-                             'centroids can never be matched')
-
-        if not self.AutomatchMarkers:
-            if not self.ground_truth_centroids.shape[0] == self.distorted_centroids.shape[0]:
-                raise ValueError(
-                    f'Since you have set AutomatchMarkers=False, there must be equal numbers of ground truth'
-                    f'markers and distorted markers, but ground truth has {self.ground_truth_centroids.shape[0]}'
-                    f'and distorted has {self.distorted_centroids.shape[0]}.')
-
-        if self.distorted_centroidsRev is not None:
-            if not self.ground_truth_centroids.shape[0] >= self.distorted_centroidsRev.shape[0]:
-                raise ValueError('There are fewer ground truth centroids than reversed gradient distorted centroids;'
-                                 ' this means the disorted centroids can never be matched. Quitting')
-
-        if np.max([self.ground_truth_centroids.x.max(), self.ground_truth_centroids.y.max(),
-                   self.ground_truth_centroids.z.max()]) < 50:
-            logger.warning('it appears that the ground truth centroids may not be defined in mm?'
-                           'this will cause the algorithm to fail. Continuing but double check this!')
-
-        if np.max([self.distorted_centroids.x.max(), self.distorted_centroids.y.max(),
-                   self.distorted_centroids.z.max()]) < 50:
-            logger.warning('it appears that the distorted centroids may not be defined in mm?'
-                           'this will cause the algorithm to fail. Continuing but double check this!')
-        if self.distorted_centroidsRev is not None:
-            if np.max([self.distorted_centroidsRev.x.max(), self.distorted_centroidsRev.y.max(),
-                       self.distorted_centroidsRev.z.max()]) < 50:
-                logger.warning('it appears that the reverse gradient distorted centroids may not be defined in mm? '
-                               'this will cause the algorithm to fail. Continuing but double check this!')
-
-    def _get_grid_spacing(self):
-        """
-        Get the spacing between markers using the ground truth data. This is used to build the kernel for RBF
-        interpolation during the marker matching step.
-        """
-        self._x_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.x))))
-        self._y_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.y))))
-        self._z_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.z))))
-
-    def _generate_extrapolant_models(self, CentroidsToSearch, distorted_centroids):
-        """
-        Use the found marker positions to extrapolate the distortion at other positions.
-
-        :param CentroidsToSearch: Current search data. At this point this is based on the
-            ground truth data with matched markers removed.
-
-        returns X_dist, Y_dist, Z_dist, which is the distortion at every marker position in
-        CentroidsToSearch.
-        """
-        points = self.ground_truth_centroids.iloc[self._MatchInd][['x', 'y', 'z']]
-        distortion = self.ground_truth_centroids.iloc[self._MatchInd].to_numpy() - \
-                     distorted_centroids.iloc[0:len(self._MatchInd)].to_numpy()
-
-        # Nearest Neighbore interpolator
-        self._X_interpolator = NearestNDInterpolator(points, distortion[:, 0])
-        self._Y_interpolator = NearestNDInterpolator(points, distortion[:, 1])
-        self._Z_interpolator = NearestNDInterpolator(points, distortion[:, 2])
-
-        points = CentroidsToSearch[['x', 'y', 'z']].to_numpy().squeeze()
-        X_dist = self._X_interpolator(points)
-        Y_dist = self._Y_interpolator(points)
-        Z_dist = self._Z_interpolator(points)
-        return X_dist, Y_dist, Z_dist
-
-    def _align_reference(self, rotation=True):
-        """
-        Moves the ground truth markers to be aligned with the distorted markers based on the central n refernce markers
-        """
-        if self.ground_truth_centroids is None or self.distorted_centroids is None:
-            logger.warning('No centroids loaded')
-            return
-
-        def _calculate_radial_distance(centroids):
-            """
-            insert the radial value of each marker:
-            """
-            centroids['r'] = centroids.apply(
-                lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
-            if centroids.r.mean() < 10:
-                logger.warning('it appears that your input data is in m, not mm - please use mm!')
-            return centroids
-
-        def _match_crosshair(search_centroids, reference_centroids):
-            """
-            match the distorted/ ground truth
-            """
-
-            _matched_reference = pd.DataFrame(columns=['x', 'y', 'z'])
-            search_centroids.reset_index(inplace=True, drop=True)
-            reference_centroids.reset_index(inplace=True, drop=True)
-            for index, row in reference_centroids.iterrows():
-                # Calculate distance from this marker to each item in search list
-                Distances = cdist(search_centroids, np.atleast_2d(row), metric='euclidean')
-                # Match marker with closest and save it
-                ind_nearest = np.argmin(Distances)
-                matched = search_centroids.iloc[ind_nearest]
-                _matched_reference.loc[index] = matched
-
-            return _matched_reference
-
-        # Find the central position in the ground truth data
-        ground_truth = self.ground_truth_centroids.copy()
-        central_x = (ground_truth.x.min() + ground_truth.x.max()) / 2
-        central_y = (ground_truth.y.min() + ground_truth.y.max()) / 2
-        central_z = (ground_truth.z.min() + ground_truth.z.max()) / 2
-
-        # Calculate the distance between each marker and central position
-        ground_truth['r_centre'] = ground_truth.apply(
-            lambda row: np.sqrt((row[0] - central_x) ** 2 + (row[1] - central_y) ** 2 + (row[2] - central_z) ** 2),
-            axis=1)
-
-        # Find the crosshair reference markers
-        self._gt_reference = ground_truth.nsmallest(self._n_reference_markers, 'r_centre')[['x', 'y', 'z']]
-        self._dist_reference = self.distorted_centroids.nsmallest(self._n_reference_markers, 'r')[['x', 'y', 'z']]
-
-        # Calculate translation vector
-        translation_vector = self._dist_reference.mean() - self._gt_reference.mean()
-
-        # Calculate rotation vector
-        if self._n_reference_markers < 3:
-            rotation = False
-        else:
-            matched_reference = _match_crosshair(self._gt_reference + translation_vector, self._dist_reference)
-            rotation_vector, error = transform.Rotation.align_vectors(self._dist_reference, matched_reference)
-
-        # Transform centroids
-        aligned = self.ground_truth_centroids[['x', 'y', 'z']] + translation_vector
-        print(f'aligning ground truth centroids by \n{translation_vector}')
-        if rotation is True:
-            aligned = rotation_vector.apply(aligned)
-            print(f'rotating ground truth centroids by \n{rotation_vector.as_matrix()}')
-
-
-        aligned = pd.DataFrame(aligned, columns=['x', 'y', 'z'])
-        self.ground_truth_centroids = _calculate_radial_distance(aligned)
-
-    def _remove_unmatchable_distorted_centroids(self):
-        """
-            Calculates the distance between each distorted marker and each ground truth markers
-            Distorted markers where the nearest ground truth marker exceeds the distance thresholds are deleted from
-             the search list
-        """
-
-        unmatchable_index = []
-        CentroidsToSearch = self.ground_truth_centroids.copy()
-        DistortedCentroids = self.distorted_centroids.copy()
-
-        for index, row in DistortedCentroids.iterrows():
-            XA = CentroidsToSearch[["x", "y", "z"]].to_numpy()
-            XB = row[0:3].values
-            # Calculate distance from this marker to each item in search list
-            Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
-            # Match marker with closest and save it
-            distance_to_closest = np.min(Distances)
-            if distance_to_closest > self._max_match_tolerance:
-                unmatchable_index.append(index)
-        if unmatchable_index:
-            logger.warning(f'removing {len(unmatchable_index)} markers because no ground truth markers were within'
-                           f'{self._max_match_tolerance} mm')
-
-        self.distorted_centroids = self.distorted_centroids.drop(unmatchable_index, axis=0)
-
-    def _match_distorted_markers_to_ground_truth(self, CentroidsToMatch):
-        """
-        find the closest ground truth marker to a given distortion. The logic of this algorithm is based on Paul
-        Liu's matlab version
-
-        1. Distorted data is sorted by r so that the smallest (least distorted) markers are processed first
-        2. the match is simply based on the minimum distance in cartesian space between the distorted marker and the
-            search markers.
-        3. Once a match has been found, that ground truth is removed from the search space
-        4. if self.WarpSearchData=True, the search markers are warped according to the previously found data. For cases
-            where distortion is small this is probably unnecessary, but for extreme distortions this algorithm will fail
-            without this
-        """
-
-        self._MatchInd = []
-        distances = []
-        CentroidsToSearch = self.ground_truth_centroids.copy()
-        for index, row in CentroidsToMatch.iterrows():
-
-            XA = CentroidsToSearch[["x", "y", "z"]].to_numpy()
-            XB = row[0:3].values
-            # Calculate distance from this marker to each item in search list
-            Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
-            # Match marker with closest and save it
-            ind_closest_point_in_ground_truth = np.argmin(Distances)
-            self._MatchInd.append(ind_closest_point_in_ground_truth)
-            distances.append(np.linalg.norm(
-                self.ground_truth_centroids.iloc[ind_closest_point_in_ground_truth][['x', 'y', 'z']] - row[
-                    ['x', 'y', 'z']]))
-            if not self.AllowDoubleMatching:
-                CentroidsToSearch.iloc[ind_closest_point_in_ground_truth] = pd.Series(
-                    {'x': 1000, 'y': 1000, 'z': 1000, 'r': 1732})
-
-            # warp search data?
-            if self.WarpSearchData and (index % self._motion_estimate_update_rate == 0) and index > 0:
-                # get extrapolated motion at all points:
-                X_dist, Y_dist, Z_dist = self._generate_extrapolant_models(CentroidsToSearch, CentroidsToMatch)
-                # regenerate centroids to search:
-                CentroidsToSearch = self.ground_truth_centroids.copy()
-                # remove found entries:
-                if not self.AllowDoubleMatching:
-                    CentroidsToSearch.iloc[self._MatchInd] = pd.Series({'x': 1000, 'y': 1000, 'z': 1000, 'r': 1732})
-                # update the data with the extrapolated motion
-                CentroidsToSearch[['x']] = CentroidsToSearch[['x']] - X_dist[:, None]
-                CentroidsToSearch[['y']] = CentroidsToSearch[['y']] - Y_dist[:, None]
-                CentroidsToSearch[['z']] = CentroidsToSearch[['z']] - Z_dist[:, None]
-
-        # create a new data frame that has the distorted and ground truth markers
-        MatchedMarkers = self.ground_truth_centroids.iloc[self._MatchInd]
-        MatchedMarkers = MatchedMarkers.rename(columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
-        MatchedMarkers.reset_index(inplace=True, drop=True)
-        MatchedCentroids = pd.concat([CentroidsToMatch, MatchedMarkers], axis=1)
-        MatchedCentroids['match_distance'] = distances
-
-        return MatchedCentroids
-
-    def _check_match(self):
-        """
-        just a simple test to detect where bad matches have been made
-        could add more sophisticated things in here if needed
-        :return:
-        """
-
-        _throw_warning = False
-        if self._CentroidMatch.match_distance.mean() > self._mean_match_tolerance:
-            _throw_warning = True
-        if self._CentroidMatch.match_distance.max() > self._max_match_tolerance:
-            _throw_warning = True
-
-        if _throw_warning:
-            warn(
-                f'\n\nThe marker match may have failed.\n\nThe mean detected distortion is {self._CentroidMatch.match_distance.mean(): 1.1f} mm '
-                f'and the max is {self._CentroidMatch.match_distance.max(): 1.1f}.'
-                f'\nYou can continue by pressing any key, but you should visualize the data using the plot_3D_markers'
-                f' method. If the match has failed, a simple remedy can be to trim the input data at the MarkerVolume'
-                f'\n stage...')
-            input("Press any key to continue...")
-
-    def _handle_double_matched_markers(self):
-        """
-        Checks if any distorted markers have been matched to the same ground truth point
-        """
-        non_unique_ind = self._CentroidMatch.duplicated(subset=['x_gt', 'y_gt', 'z_gt'], keep=False)
-        if any(non_unique_ind):
-            logger.error(f'{np.count_nonzero(non_unique_ind)} distorted centroids were matched to the same ground truth'
-                         f'marker. This may be indicative of a serious issue and you should proceed with caution. For '
-                         f'now, handling this by removing these entries from the analysis pool and continuing...')
-            self._CentroidMatch.drop(self._CentroidMatch.index[non_unique_ind])
-            self._CentroidMatch.reset_index(drop=True)
-
-        if self.distorted_centroidsRev is not None:
-            non_unique_ind = self._CentroidMatchRev.duplicated(subset=['x_gt', 'y_gt', 'z_gt'], keep=False)
-            if any(non_unique_ind):
-                logger.error(
-                    f'{np.count_nonzero(non_unique_ind)} distorted centroids were matched to the same ground truth'
-                    f'marker. This may be indicative of a serious issue and you should proceed with caution. For '
-                    f'now, handling this by removing these entries from the analysis pool and continuing...')
-                self._CentroidMatchRev.drop(self._CentroidMatchRev.index[non_unique_ind])
-                self._CentroidMatchRev.reset_index(drop=True)
-
-    def _create_marker_data_prematched_markers(self):
-        """
-        If no autosorting is requested, this creates the MatchedCentroids DataFrame directly from the input data
-        with no sorting etc.
-        """
-        self._CentroidMatch = self.ground_truth_centroids
-        self._CentroidMatch = self._CentroidMatch.rename(columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
-        self._CentroidMatch = pd.concat([self._CentroidMatch, self.distorted_centroids], axis=1)
-
-        if self.distorted_centroidsRev is not None:
-            self._CentroidMatchRev = self.ground_truth_centroids
-            self._CentroidMatchRev = self._CentroidMatchRev.rename(
-                columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
-            self._CentroidMatchRev = pd.concat([self._CentroidMatchRev, self.distorted_centroidsRev], axis=1)
-
-    def _generate_marker_position_data(self):
-        """
-        Convert the marker position data to the data we want to use for calculating gradient and B0 distortion
-        If only one dataset has been entered, then this is trivial. However, if we have a forward and reverse dataset
-        then we need to use these two seperate the gradient and B0 effects.
-        """
-        if self.distorted_centroidsRev is None:
-            # then our life is easy
-            self.MatchedCentroids = self._CentroidMatch
-            self.MatchedCentroids = self.MatchedCentroids.rename(
-                columns={'x': 'x_gnl', 'y': 'y_gnl', 'z': 'z_gnl', 'r': 'r_gnl'})
-        else:
-            # then we have to do some work to seperate G and B0
-
-            # first we will want to correlate the marker positions by sorting by ground truth r
-            self._CentroidMatch = self._CentroidMatch.sort_values('r_gt').reset_index(drop=True)
-            self._CentroidMatchRev = self._CentroidMatchRev.sort_values('r_gt').reset_index(drop=True)
-            # now find an index where the ground truth markers match; we will discard other markers
-            rev_match_index = []
-            forward_match_index = []
-            tol = 1e-1  # just a small number not a sensitve parameter
-            n_unmatched_markers = 0
-            for index, row in self._CentroidMatch.iterrows():
-                # find the closest ground truth point in the reversed data
-                XA = self._CentroidMatchRev[["x_gt", "y_gt", "z_gt"]].to_numpy()
-                XB = row[['x_gt', 'y_gt', 'z_gt']].values
-                # Calculate distance from this marker to each item in search list
-                Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
-                # calculate location of minimum
-                min_dist_ind = np.argmin(Distances)
-                # if it is less than tolerance, record the position
-                if Distances[min_dist_ind] < tol:
-                    rev_match_index.append(min_dist_ind)
-                    forward_match_index.append(index)
-                else:
-                    n_unmatched_markers += 1  # don't actually need this as can infer from data sizes.
-
-            if n_unmatched_markers > 0:
-                logger.warning(
-                    f'failed to match {n_unmatched_markers} of a total {self.ground_truth_centroids.shape[0]}'
-                    f' input markers. These will be deleted from returned data')
-            # now we have indexes linking our two datasets based on their ground truth match
-            self._CentroidMatchRev = self._CentroidMatchRev.iloc[rev_match_index].reset_index()
-            self._CentroidMatch = self._CentroidMatch.iloc[forward_match_index].reset_index()
-
-            # marker position distortion from gradients is difference between forward and reversed:
-            self.MatchedCentroids = (self._CentroidMatch[['x', 'y', 'z', 'r']] + self._CentroidMatchRev[
-                ['x', 'y', 'z', 'r']]) / 2
-            self.MatchedCentroids = self.MatchedCentroids.rename(
-                columns={'x': 'x_gnl', 'y': 'y_gnl', 'z': 'z_gnl', 'r': 'r_gnl'})
-            # add ground truth to data frame
-            self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt', 'r_gt']] = self._CentroidMatch[
-                ['x_gt', 'y_gt', 'z_gt', 'r_gt']]
-            # marker position distortion from B0 is difference between from total and gradient distortion:
-            '''
-            deta_z_B0=z_dis_AP-z_GNL; %% maximum distortion is 16mm
-            deta_y_B0=y_dis_AP-y_GNL;  %% maximum distortio is 4mm  
-            '''
-            B0_dis = self.MatchedCentroids[['x_gnl', 'y_gnl', 'z_gnl']].to_numpy() - \
-                     self._CentroidMatch[['x', 'y', 'z']].to_numpy()
-            B0_pos = B0_dis + self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt']].to_numpy()
-            self.MatchedCentroids[['x_B0', 'y_B0', 'z_B0']] = B0_dis
-
-    def _sort_distorted_centroids(self, data_to_sort):
-        """
-        sorts the data frame.
-        sorting is important, because the search for a matching ground truth marker is carried out in order
-        """
-
-        if self.sorting_method == 'radial':
-            # sort input data by r
-            data_to_sort = data_to_sort.sort_values('r')
-            data_to_sort.reset_index(inplace=True, drop=True)
-        if self.sorting_method == 'closest':
-            # find the distorted marker that has the closest match to a ground truth marker.
-            min_distance = []
-            XA = self.ground_truth_centroids[["x", "y", "z"]].to_numpy()
-            for index, row in data_to_sort.iterrows():
-                XB = row[0:3].values
-                Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
-                min_distance.append(np.min(Distances))
-            starting_marker_ind = np.argmin(min_distance)
-            # now calculate the distances of every other distorted marker to this marker:
-            XA = data_to_sort[["x", "y", "z"]].to_numpy()
-            XB = np.atleast_2d(data_to_sort.loc[starting_marker_ind][["x", "y", "z"]].to_numpy())
-            Distances = cdist(XA, XB)
-            distance_to_start_ind = np.argsort(Distances, axis=0)
-            assert distance_to_start_ind[0] == starting_marker_ind
-            data_to_sort = data_to_sort.reindex(np.squeeze(distance_to_start_ind))
-            data_to_sort.reset_index(inplace=True, drop=True)
-
-        return data_to_sort
-
-    # public methods
-
-    def plot_3D_markers(self, add_arrows=True, title='3D marker positions'):  # pragma: no cover
-        """
-        Works very similarly to the MarkerVolume version, but plots both sets of markers and adds arrows
-
-        :param add_arrows: if True, arrows drawn between matches
-        :type add_arrows: bool, optional
-        :param title: plot title
-        :type title: str, optional
-        """
-
-        fig = plt.figure()
-        axs = fig.add_subplot(111, projection='3d')
-        axs.scatter(self.MatchedCentroids.x_gt, self.MatchedCentroids.y_gt, self.MatchedCentroids.z_gt)
-        axs.scatter(self.MatchedCentroids.x_gnl, self.MatchedCentroids.y_gnl, self.MatchedCentroids.z_gnl)
-        if add_arrows:
-            mag_color = np.sqrt((self.MatchedCentroids.x_gt - self.MatchedCentroids.x_gnl) ** 2
-                                + (self.MatchedCentroids.y_gt - self.MatchedCentroids.y_gnl) ** 2
-                                + (self.MatchedCentroids.z_gt - self.MatchedCentroids.z_gnl) ** 2)
-            axs.quiver(self.MatchedCentroids.x_gnl, self.MatchedCentroids.y_gnl, self.MatchedCentroids.z_gnl,
-                       self.MatchedCentroids.x_gt - self.MatchedCentroids.x_gnl,
-                       self.MatchedCentroids.y_gt - self.MatchedCentroids.y_gnl,
-                       self.MatchedCentroids.z_gt - self.MatchedCentroids.z_gnl,
-                       edgecolors=("black",))
-
-        axs.set_xlabel('X [mm]')
-        axs.set_ylabel('Y [mm]')
-        axs.set_zlabel('Z [mm]')
-        axs.set_title(title)
-        axs.set_box_aspect((np.ptp(self.MatchedCentroids.x_gt), np.ptp(self.MatchedCentroids.y_gt),
-                            np.ptp(self.MatchedCentroids.z_gt)))
-        plt.legend(['ground truth', 'distorted'])
-        plt.show()
-
-    def plot_compressed_markers(self, z_max=20, z_min=-20, add_arrows=True, title=None):  # pragma: no cover
-        """
-        compresses the 3D markers in the z plane, allowing a 2D visualisation.
-
-        :param z_max: maximum z coordiante of markers to includes
-        :type z_max: float, optional
-        :param z_min: minimum z coordiante of markers to includes
-        :type z_min: float, optional
-        :param add_arrows: if True, arrows drawn between matches
-        :type add_arrows: bool, optional
-        :param title: plot title
-        :type title: str, optional
-
-        """
-
-        def get_markers_as_function_of_z():
-            """
-            finds an index of markers within tolerence of z_pos
-            """
-            data_ind = np.logical_and(self.MatchedCentroids.z_gt > z_min, self.MatchedCentroids.z_gt < z_max)
-            z_loc_data = self.MatchedCentroids[data_ind]
-            return z_loc_data
-
-        def plot_markers_inner(plot_data):
-            """
-            clears exising axes and plots plot_data
-            """
-            axs.clear()
-            z_offset = (plot_data.z_gt - plot_data.z_gnl)
-            axs.scatter(plot_data.x_gnl, plot_data.y_gnl, c='darkturquoise')  # c=z_offset,cmap="magma"
-            axs.scatter(plot_data.x_gt, plot_data.y_gt, c='darkgoldenrod')
-            # axs.legend(['Distorted', 'Ground Truth'])
-            if add_arrows:
-                axs.quiver(plot_data.x_gnl, plot_data.y_gnl,
-                           plot_data.x_gt - plot_data.x_gnl,
-                           plot_data.y_gt - plot_data.y_gnl,
-                           angles="xy", units='xy', scale=1, width=1)
-            axs.set_xlim([-150, 150])
-            axs.set_ylim([-150, 150])
-            axs.set_xlabel('x [mm]', fontsize=15)
-            axs.set_ylabel('y [mm]', fontsize=15)
-            axs.tick_params(axis='both', which='major', labelsize=12)
-            axs.tick_params(axis='both', which='minor', labelsize=12)
-            axs.axis("equal")
-            axs.grid()
-            plt.subplots_adjust(bottom=0.25)
-            plt.legend(['distorted', 'ground truth'])
-            if title:
-                plt.title(title)
-
-        fig, axs = plt.subplots(figsize=[8, 8], ncols=1, nrows=1)
-
-        plot_data = get_markers_as_function_of_z()
-        plot_markers_inner(plot_data)
-        plt.show()
-
-    def plot_reference_markers(self, title='Reference alignment markers'):
-
-        try:
-            fig = plt.figure()
-            axs = fig.add_subplot(111, projection='3d')
-            axs.scatter(self._gt_reference.x, self._gt_reference.y, self._gt_reference.z)
-            axs.scatter(self._dist_reference.x, self._dist_reference.y, self._dist_reference.z)
-
-        except AttributeError:
-            logger.warning('Cannot plt reference  as it does not exist...')
-            return
-
-        axs.set_xlabel('X [mm]')
-        axs.set_ylabel('Y [mm]')
-        axs.set_zlabel('Z [mm]')
-        axs.set_title(title)
-        axs.set_box_aspect((np.ptp(self.MatchedCentroids.x_gt), np.ptp(self.MatchedCentroids.y_gt),
-                            np.ptp(self.MatchedCentroids.z_gt)))
-        plt.legend(['ground truth', 'distorted'])
-        plt.show()
-
-
-
-    def report(self):
-        print(f'mean distortion: {self.MatchedCentroids.match_distance.mean(): 1.1f} mm, '
-              f'std: {np.std(self.MatchedCentroids.match_distance): 1.1f} mm, '
-              f'Max: {self.MatchedCentroids.match_distance.max(): 1.1f} mm')
+import pathlib
+from .utilities import get_all_files, dicom_to_numpy
+import pydicom
+from pathlib import Path
+import numpy as np
+from skimage.filters import gaussian, threshold_otsu
+from skimage.measure import label
+from scipy.interpolate import NearestNDInterpolator
+from matplotlib import pyplot as plt
+import logging
+import os
+import json
+import pandas as pd
+from scipy.spatial.distance import cdist
+from scipy.spatial import transform
+from datetime import datetime
+
+ch = logging.StreamHandler()
+formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
+ch.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(ch)
+logger.setLevel(logging.INFO)
+logger.propagate = False
+
+
+class MarkerVolume:
+    """
+    This class excepts either a path to a folder of dicom files or a numpy array of marker positions.
+    In the former case, it will attempt to automatically extract the marker positions. In the latter, it will just
+    use the input marker positions. Once the instance is created, it contains a number of handy plots and functions.
+
+    :param input_data_path: Either a path to a folder of dicoms, or a numpy array with three columns corresponding to the
+        [x,y,z] marker positions
+    :type input_data_path: path, string, np.ndarray
+    :param ImExtension: change to whatever extension your dicom files, most commonly either dcm or IMA
+    :type ImExtension: str, optional
+    :param r_min: any markers at radii less than this will be discounted.
+    :type r_min: float ,optional
+    :param r_max: any markers at radii greater than this will be discounted.
+    :type r_max: float, optional
+    :param iterative_segmentation: If set to true, a slower iterative method will be used to find the threshold value
+        used to segment the markers. Otherwise, otsu's method is used.
+    :type iterative_segmentation: bool, optional
+    :param threshold: Manually set the threshold value. If this is left as None otsu's method is used.
+        This will replace the iterative segmentation method regardless of flag.
+    :type threshold: float, optional
+    :param n_markers_expected: if you know how many markers you expect, you can enter the value here. The code will
+        then warn you if it finds a different number.
+    :type n_markers_expected: int, optional
+    :param gaussian_image_filter_sd: size of filter to blur input data with. Higher values are better at removing
+        noise prior to thresholding, but may also blur out small/low signal markers!
+    :type gaussian_image_filter_sd: float, optional
+    :param correct_fat_water_shift: if True, will attempt to automatically correct marker positions for calculated
+        fat water shift
+    :type correct_fat_water_shift: bool, optional
+    :param marker_size_lower_tol: lower acceptance window for a marker compared to the median size of markers.
+        e.g. markermarker_size_tol=0.5 will result in markers being accepted within when
+        (1-marker_size_lower_tol)*median_marker_size <= marker_size <= (1+markermarker_size_tol)*marker_size_upper_tol
+    :type marker_size_lower_tol: float, optional
+    :param marker_size_upper_tol: upper acceptance window for a marker compared to the median size of markers.
+    :type marker_size_upper_tol: float, optional
+    :param verbose: if True, prints a lot of info about the marker extraction process to the screen. mostly useful
+        during debugging
+    :type verbose: bool, optional
+    :param fat_shift_direction: We aren't sure yet if we can confidently predict the direction that the fat water shift
+        will be in. if you set correct_fat_water_shift=True, you can change the direction it shifts in here. it should
+        take a value of -1, or 1. pull requests making this easier to use very welcome!
+    :type fat_shift_direction: int, optional
+    """
+
+    def __init__(self, input_data, ImExtension='dcm', r_min=None, r_max=None, iterative_segmentation=False,
+                 threshold=None, n_markers_expected=None, fat_shift_direction=None, verbose=False,
+                 gaussian_image_filter_sd=1, correct_fat_water_shift=False, marker_size_lower_tol=0.9,
+                 marker_size_upper_tol=1):
+
+        self.verbose = verbose
+        self._file_extension = ImExtension
+        self._correct_fat_water_shift = correct_fat_water_shift
+        self.dicom_data = None  # overwritten below if possible.
+        self._n_markers_expected = n_markers_expected
+        self._r_min = r_min
+        self._r_max = r_max
+        self._cutoffpoint = threshold
+        self._iterative_segmentation = iterative_segmentation
+        self._chemical_shift_vector = None
+        self._gaussian_image_filter_sd = gaussian_image_filter_sd
+        self._marker_size_lower_tol = marker_size_lower_tol
+        self._marker_size_upper_tol = marker_size_upper_tol
+
+        if isinstance(input_data, (pathlib.Path, str)):
+            self.input_data_path = Path(input_data)
+            if self.input_data_path.is_dir():
+                # dicom input
+                self.InputVolume, self.dicom_affine, (self.X, self.Y, self.Z) = \
+                    dicom_to_numpy(self.input_data_path, file_extension=self._file_extension, return_XYZ=True)
+                self._calculate_MR_acquisition_data()
+
+                # Segmenting markers
+                self._filter_volume_by_r()
+                self.ThresholdVolume, self.BlurredVolume = self._threshold_volume(self.InputVolume)
+                centroids = self._find_contour_centroids()
+                self.MarkerCentroids = pd.DataFrame(centroids, columns=['x', 'y', 'z'])
+
+                # Correct for oil water shift
+                if self._correct_fat_water_shift:
+                    self._calculate_chemical_shift_vector(fat_shift_direction=fat_shift_direction)
+                    self.MarkerCentroids = self.MarkerCentroids + self._chemical_shift_vector
+            elif (os.path.isfile(self.input_data_path) and os.path.splitext(self.input_data_path)[1] == '.json'):
+                # slicer input
+                with open(self.input_data_path) as f:
+                    data = json.load(f)
+                arrays = [el for el in data['markups'][0]['controlPoints']]
+                points = [el['position'] for el in arrays]
+                self.MarkerCentroids = pd.DataFrame(points, columns=['x', 'y', 'z'])
+
+                # look for dicom_data json file
+                try:
+                    with open(os.path.join(self.input_data_path.parent, 'dicom_data.json')) as f:
+                        self.dicom_data = json.load(f)
+                except:
+                    logger.warning(f'MR data file dicom_data.json not found at {self.input_data_path.parent}. Continuing')
+            else:
+                raise FileNotFoundError(f'could not find any data at {self.input_data_path}')
+        elif isinstance(input_data, np.ndarray):
+            # don't need to do anything then.
+            self.MarkerCentroids = pd.DataFrame(input_data, columns=['x', 'y', 'z'])
+            logger.warning("numpy input is deprecated, please use pandas input with ['x', 'y', 'z'] cols instead")
+        elif isinstance(input_data, pd.core.frame.DataFrame):
+            _expected_columns = ['x', 'y', 'z']
+            if not all([col in input_data for col in _expected_columns]):
+                raise AttributeError("input pandas data must have columns called ['x', 'y', 'z']")
+            self.MarkerCentroids = input_data.copy()
+        else:
+            raise TypeError(f'Uknown data input: {type(input_data)}')
+
+        # insert the radial value of each marker:
+        self.MarkerCentroids['r'] = self.MarkerCentroids.apply(
+            lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
+        if self.MarkerCentroids.r.mean() < 10:
+            logger.warning('it appears that your input data is in m, not mm - please use mm!')
+
+        self._filter_markers_by_r()
+        if self._n_markers_expected is not None:
+            if not (self.MarkerCentroids.shape[0] == n_markers_expected):
+                logger.warning(f'For data {self.input_data_path}\n'
+                               f'You entered that you expected to find'
+                               f' {n_markers_expected}, but actually found {self.MarkerCentroids.shape[0]}.')
+
+    def _filter_volume_by_r(self):
+        """
+        Accelerates and improves segmenting by setting all voxels outside of specified radius to the background
+        """
+        if self._r_max or self._r_min:
+            _max = 10000
+            _min = -1
+            if self._r_max:
+                _max = self._r_max
+            if self._r_min:
+                _min = self._r_min
+            background = np.median(self.InputVolume)
+
+            it = np.nditer(self.InputVolume, flags=['multi_index'])
+            for voxel in it:
+                distance = np.sqrt(
+                    self.X[it.multi_index] ** 2 + self.Y[it.multi_index] ** 2 + self.Z[it.multi_index] ** 2)
+                if distance < _min or distance > _max:
+                    self.InputVolume[it.multi_index] = background
+
+    def _filter_markers_by_r(self):
+        """
+        Remove any markers that are less than r_min or more than r_max
+        """
+        if self._r_max:
+            keep_ind = abs(self.MarkerCentroids.r) < self._r_max
+            self.MarkerCentroids = self.MarkerCentroids[keep_ind].reset_index(drop=True)
+        if self._r_min:
+            keep_ind = abs(self.MarkerCentroids.r) > self._r_min
+            self.MarkerCentroids = self.MarkerCentroids[keep_ind].reset_index(drop=True)
+
+    def _calculate_MR_acquisition_data(self):
+        """
+        If we have MR images, extract the information from thall_dicom_files = get_all_files(self.input_data_path)e
+        dicom header that is needed to convert marker positions to magnetic fields downstream.
+        - This method is dependant on having the full coordinate list which are calculated upstream; this is why it
+            must reside inside this class.
+        - We include many fields that aren't in the dicom header by default
+        - we package this as a simple dict that can be easily saved as json
+        """
+        all_dicom_files = get_all_files(self.input_data_path, file_extension=self._file_extension)
+        # use first one, its as good as any other:
+        example_dicom_file = pydicom.read_file(self.input_data_path / all_dicom_files[0])
+
+        if example_dicom_file.Modality == 'MR':
+            if not example_dicom_file.Manufacturer == 'SIEMENS':
+                logger.warning(
+                    'this code has not been tested with non-siemens scanners. If dicom standards work properly'
+                    'this code will too...')
+            x = np.unique(self.X)
+            y = np.unique(self.Y)
+            z = np.unique(self.Z)
+            x_pixel_spacing = np.mean(np.diff(x))
+            y_pixel_spacing = np.mean(np.diff(y))
+            z_pixel_spacing = np.mean(np.diff(z))
+            x_fov = x.max() - x.min() + x_pixel_spacing
+            y_fov = y.max() - y.min() + y_pixel_spacing
+            z_fov = z.max() - z.min() + z_pixel_spacing
+            self._dicom_header = example_dicom_file
+
+            self.dicom_data = {}  # fill up below
+            self.dicom_data['FOV'] = [x_fov, y_fov, z_fov]
+            self.dicom_data['bandwidth'] = float(example_dicom_file.PixelBandwidth)
+
+            self.dicom_data['gama'] = float(example_dicom_file.MagneticFieldStrength * 42.57747851)
+            self.dicom_data['pixel_spacing'] = [x_pixel_spacing, y_pixel_spacing, z_pixel_spacing]
+            self.dicom_data['image_size'] = [x.size, y.size, z.size]
+            self.dicom_data['magnetic_field_strength'] = example_dicom_file.MagneticFieldStrength
+            self.dicom_data['imaging_frequency'] = example_dicom_file.ImagingFrequency
+            try:
+                acquisition_date = datetime.strptime(example_dicom_file.AcquisitionDate, '%Y%m%d')
+                self.dicom_data['acquisition_date'] = acquisition_date.strftime("%d_%B_%Y")
+            except ValueError as e:
+                logger.error(e)
+                logger.error('failed to extract datetime, probably didnt understand date format, continuing...')
+            self.dicom_data['manufacturer'] = example_dicom_file.Manufacturer
+
+            # the above works on siemens scanner, not sure if it will prove consistent on others
+            fat_water_delta_f = example_dicom_file.MagneticFieldStrength * 42.57747851 * 3.5
+            self.dicom_data['chem_shift_magnitude'] = (example_dicom_file.PixelBandwidth / fat_water_delta_f) / 2
+            self.dicom_data['InPlanePhaseEncodingDirection'] = example_dicom_file.InPlanePhaseEncodingDirection
+            # extract the frequency, phase, and slice directions (B0 effects occur in freq and slice)
+            directions = ['x', 'y', 'z']
+            phase_encode_direction = None
+            freq_encode_direction = None
+            if self.dicom_data['InPlanePhaseEncodingDirection'] == 'ROW':
+                phase_cosines = example_dicom_file.ImageOrientationPatient[:3]
+                row_cosines = example_dicom_file.ImageOrientationPatient[3:]
+            elif self.dicom_data['InPlanePhaseEncodingDirection'] == 'COL':
+                phase_cosines = example_dicom_file.ImageOrientationPatient[3:]
+                row_cosines = example_dicom_file.ImageOrientationPatient[:3]
+            for i, (phase_cosine, freq_cosine) in enumerate(zip(phase_cosines, row_cosines)):
+                if abs(float(phase_cosine)) == 1:
+                    phase_encode_direction = directions[i]
+                if abs(float(freq_cosine)) == 1:
+                    freq_encode_direction = directions[i]
+            if phase_encode_direction is None:
+                logger.warning('failed to extract phase encoding direction from dicom data, continuing')
+            if freq_encode_direction is None:
+                logger.warning('failed to extract frequency encoding direction from dicom data, continuing')
+            self.dicom_data['phase_encode_direction'] = phase_encode_direction
+            self.dicom_data['freq_encode_direction'] = freq_encode_direction
+            # get slice direction
+            slice_dir_ind = np.equal(example_dicom_file.ImageOrientationPatient[:3],
+                                     example_dicom_file.ImageOrientationPatient[3:])
+            self.dicom_data['slice_direction'] = np.array(directions)[slice_dir_ind][0]
+            bandwidth = np.array(self.dicom_data['bandwidth'])
+            image_size = np.array(self.dicom_data['image_size'])
+            gama = np.array(self.dicom_data['gama'])
+            FOV = np.array(self.dicom_data['FOV'])
+            gradient_strength = bandwidth * image_size / (gama * 1e6 * FOV * 1e-3)  # unit(T / m)
+            self.dicom_data['gradient_strength'] = list(gradient_strength)
+
+        else:
+            self.dicom_data = None
+
+    def _calculate_chemical_shift_vector(self, fat_shift_direction=1):
+        """
+        Calculates a chemical shift vector (x,y,z) to be applied to each marker to account for the fat/water shift.
+
+        :param fat_shift_direction: dictates whether the shift is positive or negative. we aren't sure how consisten
+            this is between scanners so have left as used defined.
+        """
+        if self.dicom_data is None:
+            logger.warning('No dicom data for chemical shift')
+            return
+
+        # TODO check these
+        if fat_shift_direction == 'AP' or fat_shift_direction == 'RL' or fat_shift_direction == 'FH' or fat_shift_direction == -1:
+            fat_shift_direction = -1
+        elif fat_shift_direction == 'PA' or fat_shift_direction == 'LR' or fat_shift_direction == 'HF' or fat_shift_direction == 1:
+            fat_shift_direction = 1
+        else:
+            fat_shift_direction = 0
+            logger.warning('Chemical shift input was invalid')
+
+        # Calculate magnitude (in pixels) of the chemical shift based on the shift frequency of a 1T MRI field (149Hz)
+        directions = ['x', 'y', 'z']
+        direction = np.array(([int(el == self.dicom_data['freq_encode_direction']) for el in directions]))
+        # ^ this just gives a vector with a 1 in the correct direction e.g. [0,1,0]
+        shift = direction * self.dicom_data['chem_shift_magnitude']
+        self._chemical_shift_vector = shift * np.array(self.dicom_data['pixel_spacing'])[
+            direction.astype(bool)] * fat_shift_direction
+
+    def _find_iterative_cutoff(self, blurred_volume):
+        """
+        Replaces the otsu threshold with a slower, iterative method to find the best threshold for segmenting markers.
+        A range of valid thresholds are found and the mean is returned as the best threshold.
+        If no valid thresholds are found, the mean of candidate thresholds that will miss some markers is returned.
+        """
+
+        if self._n_markers_expected is None:
+            logger.warning('Iterative segmentation method requires the expected number of markers to be input.')
+            return None
+
+        # finds a range of thresholds that give a number of segments near to the number of expected markers
+        histogram_division = 100
+
+        candidate_thresholds = []       # Thresholds that have fewer markers than expected, use when no valid thresholds
+        candidate_n_points = []
+        valid_thresholds = []           # Thresholds that should give the corrected number of markers
+
+        # divide the range into segments and calculate how many volumes result from each segment
+        background_value = np.median(np.round(blurred_volume))
+        intensity_range = np.max(blurred_volume) - background_value
+        histogram_segment = intensity_range / histogram_division
+
+        # Testing each histogram segment
+        for i in range(1, histogram_division - 1):
+
+            n_segments = 0
+            cutoff = background_value + i * histogram_segment
+            threshold_volume = blurred_volume > cutoff
+            labels = label(threshold_volume, background=0)
+            unique_labels = np.unique(labels)[1:]  # first label is background so skip
+            # Check number of segments falls within valid range:
+            tol = 0.1
+            if len(unique_labels) < self._n_markers_expected*(1-tol) or len(unique_labels) > self._n_markers_expected * (1+tol):
+                continue  # Too few or too many segments
+            else:
+                # This threshold is possibly valid
+                candidate_thresholds.append(cutoff)
+                # Remove small volumes and check if still valid
+                for label_level in unique_labels:
+                    RegionInd = labels == label_level
+                    if np.count_nonzero(RegionInd) > 2:
+                        n_segments += 1
+                candidate_n_points.append(n_segments)
+                if n_segments >= self._n_markers_expected:
+                    valid_thresholds.append(cutoff)
+                    if self.verbose:
+                        print('Threshold: ' + str(format(cutoff, '.2f')) + ', ' + str(n_segments) + ' segments.')
+                else:
+                    if self.verbose:
+                        print('Threshold: ' + str(format(cutoff, '.2f')) + ' is a candidate.')
+
+            if len(unique_labels) < 10:
+                # threshold is too high and we can stop
+                break
+
+        if len(valid_thresholds) > 0:
+            return np.mean(valid_thresholds)
+        elif len(candidate_thresholds) > 0:
+            ind = np.argmin(abs(np.subtract(self._n_markers_expected, candidate_n_points)))
+            best_threshold = candidate_thresholds[ind]
+            logger.warning(f'No valid thresholds were found. Using closest possible value of {best_threshold}')
+            return best_threshold
+        else:
+            logger.warning('No valid thresholds were found. Try lowering gaussian blur level.')
+            return None
+
+    def _threshold_volume(self, VolumeToThreshold):
+        """
+        For a 3D numpy array, turn all elements < cutoff to zero, and all other elements to 1.
+        If no cutoff is entered, otsu's method is used to auto-threshold.
+        """
+
+        BlurredVolume = gaussian(VolumeToThreshold, sigma=self._gaussian_image_filter_sd)
+
+        if self._cutoffpoint is not None:
+            # If cutoff point has been manually entered, go straight to thresholding
+            self._iterative_segmentation = False
+        if self._iterative_segmentation is True:
+            self._cutoffpoint = self._find_iterative_cutoff(BlurredVolume)
+        if self._cutoffpoint is None:
+            self._cutoffpoint = threshold_otsu(BlurredVolume)
+
+        ThresholdVolume = BlurredVolume > self._cutoffpoint
+
+        return ThresholdVolume, BlurredVolume
+
+    def _get_marker_max_min_volume(self):
+        """
+        figures out the range of voxels that a marker should have
+        """
+        self._n_voxels = []  # going to keep track of this so we can remove any very small regions if needed
+
+        for label_level in self.unique_labels:  # first label is background so skip
+            # extract x,y,z of each connected region
+            RegionInd = self._labels == label_level
+            self._n_voxels.append(np.count_nonzero(RegionInd))
+        # Set up min and max marker volumes
+        self._n_voxels_median = np.median(np.array(self._n_voxels))
+        self._voxel_min = (1 - self._marker_size_lower_tol) * self._n_voxels_median
+        self._voxel_max = (1 + self._marker_size_upper_tol) * self._n_voxels_median
+
+        # Modify based on number of markers
+        if self._n_markers_expected is not None:
+            self._n_voxels_copy = np.array(self._n_voxels)
+            voxel_difference = np.absolute(np.array(self._n_voxels) - self._n_voxels_median)
+            # Loop that deletes the marker size with the largest difference from median until the expected # of markers
+            while len(self._n_voxels_copy) > self._n_markers_expected:
+                self._n_voxels_copy = np.delete(self._n_voxels_copy, np.argmax(voxel_difference))
+                voxel_difference = np.delete(voxel_difference, np.argmax(voxel_difference))
+            # Set min and max based on the remaining list
+            if np.min(self._n_voxels_copy) > self._voxel_min:
+                self._voxel_min = np.min(self._n_voxels_copy)
+            if np.max(self._n_voxels_copy) < self._voxel_max:
+                self._voxel_max = np.max(self._n_voxels_copy)
+
+        # 3 voxels is the absolute floor
+        if self._voxel_min < 3:
+            self._voxel_min = 3
+
+    def _remove_load(self):
+        '''
+        if it seems very likely that the only thing that has been segmented is the load
+        remove it and try again. We may want to enable this in situations where any large object is detected...
+        '''
+
+        for label_level in self.unique_labels:
+            RegionInd = self._labels == label_level
+            self.InputVolume[RegionInd] = 0
+        self._cutoffpoint = None
+        self.ThresholdVolume, self.BlurredVolume = self._threshold_volume(self.InputVolume)
+        self._labels = label(self.ThresholdVolume, background=0)
+        self.unique_labels = np.unique(self._labels)[1:]  # first label is background so skip
+
+    def _print_thresholding_information(self):
+        print('Threshold value: ' + str(self._cutoffpoint))
+        print('Median marker volume: ' + str(self._n_voxels_median))
+        print('Expected marker volume: ' + str(self._voxel_min) + ' to ' + str(self._voxel_max))
+        print(f'Regions to check: {self.unique_labels.shape}')
+
+    def _print_thresholding_summary(self, n_found_markers, n_skipped_markers):
+        print('----------')
+        print(f'Total regions: {len(self.unique_labels)}')
+        print(f'Total markers found:   {n_found_markers}')
+        print(f'Total skipped:         {n_skipped_markers}')
+
+    def _find_contour_centroids(self):
+        """
+        This code loops through all the found regions, extracts the cartesian coordiantes, and takes the
+        intensity-weighted average as the centroid.
+        It excludes volumes that are bigger/ smaller than the median using the params
+        marker_size_upper_tol and marker_size_lower_tol
+        """
+        self._labels = label(self.ThresholdVolume, background=0)
+        self.unique_labels = np.unique(self._labels)[1:]  # first label is background so skip
+        if self.unique_labels.shape[0] < 3:
+            logger.warning('automatic thresholding didnt work, trying to remove load and try again...')
+            self._remove_load()
+        self._get_marker_max_min_volume()
+
+        if self.verbose:
+            self._print_thresholding_information()
+
+        x_centroids = []
+        y_centroids = []
+        z_centroids = []
+        skipped = 0
+
+        # extract x,y,z of each connected region
+        for i, label_level in enumerate(self.unique_labels):
+            RegionInd = np.equal(self._labels, label_level)
+            voxels = np.count_nonzero(RegionInd)
+            if voxels < self._voxel_min or voxels > self._voxel_max:
+                skipped += 1
+                if self.verbose:
+                    print('Region ' + str(i + 1) + ': Skipped, v = ' + str(voxels))
+                continue  # skip outliers
+
+            region_sum = np.sum(self.InputVolume[RegionInd])
+            weighted_x = np.sum(np.multiply(self.X[RegionInd], self.InputVolume[RegionInd]))
+            weighted_y = np.sum(np.multiply(self.Y[RegionInd], self.InputVolume[RegionInd]))
+            weighted_z = np.sum(np.multiply(self.Z[RegionInd], self.InputVolume[RegionInd]))
+            x_centroids.append(weighted_x / region_sum)
+            y_centroids.append(weighted_y / region_sum)
+            z_centroids.append(weighted_z / region_sum)
+            if self.verbose:
+                print('Region ' + str(i + 1) + ': Marker, v = ' + str(voxels))
+
+        if self.verbose:
+            self._print_thresholding_summary(len(x_centroids), skipped)
+
+        return np.array([x_centroids, y_centroids, z_centroids]).T
+
+    # public methods
+
+    def plot_3D_markers(self, title='3D marker positions'):  # pragma: no cover
+        """
+        Just a quick plot of the marker positions; very useful sanity check!
+        """
+
+        fig = plt.figure()
+        axs = fig.add_subplot(111, projection='3d')
+        axs.scatter(self.MarkerCentroids.x, self.MarkerCentroids.y, self.MarkerCentroids.z, s=10)
+        axs.set_xlabel('X [mm]')
+        axs.set_ylabel('Y [mm]')
+        axs.set_zlabel('Z [mm]')
+        axs.set_title(title)
+        axs.set_box_aspect(
+            (np.ptp(self.MarkerCentroids.x), np.ptp(self.MarkerCentroids.y), np.ptp(self.MarkerCentroids.z)))
+        plt.show()
+
+    def perturb_marker_positions(self, random_perturbation, systemic_perturbation=0):
+        """
+        add random noise to the marker positions. Useful to perform sensitivity analysis. operates in place.
+
+        :param random_perturbation: upper and lower limits of random_perturbation to each marker coordinates. uniform
+            distribution is used
+        :type random_perturbation: float
+        :param systemic_perturbation: constant offset added to all markers
+        :type systemic_perturbation: float, optional
+        """
+
+        x_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
+                                     size=self.MarkerCentroids.x.shape)
+        y_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
+                                     size=self.MarkerCentroids.x.shape)
+        z_peturb = np.random.uniform(low=-random_perturbation, high=random_perturbation,
+                                     size=self.MarkerCentroids.x.shape)
+        self.MarkerCentroids.x = self.MarkerCentroids.x + x_peturb + systemic_perturbation
+        self.MarkerCentroids.y = self.MarkerCentroids.y + y_peturb + systemic_perturbation
+        self.MarkerCentroids.z = self.MarkerCentroids.z + z_peturb + systemic_perturbation
+
+    def export_to_slicer(self, save_path=None, filename='slicer_centroids'):
+        """
+        export a json file that can be read in by slicer, allowing a good way to visualise marker segmentation
+        performance. This file will be saved at the same spot as input data if dicom was input, otherwise it will be
+        saved to save_path.
+        """
+        # sort out where to save:
+        if save_path is None:
+            try:
+                _save_path = self.input_data_path
+            except AttributeError:  # indicates numpy input
+                logger.error('To save numpy data to slicer format, please enter a value for "save_path" when'
+                             'calling MarkerVolume.export_to_slicer')
+                return
+        else:
+            _save_path = Path(save_path)
+
+        file_content = []  # will fill up one line at a time
+        file_content.append('{"@schema": "https://raw.githubusercontent.com/slicer/slicer/master/Modules/Loadable/'
+                            'Markups/Resources/Schema/markups-schema-v1.0.0.json#",\n')
+        file_content.append('"markups": [{"type": "Fiducial", "coordinateSystem": "LPS", "controlPoints": [\n')
+        for index, row in self.MarkerCentroids.iterrows():
+            if index == self.MarkerCentroids.shape[0] - 1:
+                # for last entry have to delete a comma
+                file_content.append(
+                    f'{{ "label": " ", "position": [{row.x: 1.2f}, {row.y: 1.2f}, {row.z: 1.2f}], "locked": true}}\n')
+            else:
+                file_content.append(
+                    f'{{ "label": " ", "position": [{row.x: 1.2f}, {row.y: 1.2f}, {row.z: 1.2f}], "locked": true}},\n')
+
+        file_content.append(']}]}')
+        # write contents
+        filename = filename + '.mrk.json'
+        file_loc = _save_path / filename
+        with open(file_loc, 'w') as f:
+            f.writelines(file_content)
+
+    def save_dicom_data(self, save_path=None, filename='dicom_data'):
+        """
+        save the dicom data as json.  This file will be saved at the same
+        spot as input data if dicom was input, otherwise it will be saved
+        to save_path.
+        """
+
+        if self.dicom_data is None:
+            logger.warning('cannot save dicom data because there is none...')
+            return
+        if save_path is None:
+            save_path = self.input_data_path
+        save_path = Path(save_path)
+        _file_name, _file_extension = os.path.splitext(filename)
+        if _file_extension == '':
+            _file_extension = '.json'
+        filename = _file_name + _file_extension
+        full_filename = save_path / filename
+
+        with open(full_filename, 'w') as f:
+            json.dump(self.dicom_data, f)
+
+
+class MatchedMarkerVolumes:
+    """
+    :param GroundTruthData:
+    :type GroundTruthData: MarkerVolume object, or path to dicom folder, or numpy array
+    :param DistortedData:
+    :type DistortedData: MarkerVolume object, or path to dicom folder, or numpy array
+    :param reverse_gradient_data:
+    :type reverse_gradient_data: None, or MarkerVolume object, or path to dicom folder, or numpy array
+    :param WarpSearchData: if True, position of found markers is used to update expected positions for ground truth.
+        Recomended is True if there is substantial distortion present.
+    :type WarpSearchData: boolean
+    :param AutomatchMarkers: if True, will automatically match the distorted data to the ground truth using a search
+        algorith. If False, will simply use input data in the order it is entered. This is useful if you have sets
+        of markers that were independently matched through some other process.
+    :type AutomatchMarkers: boolean
+    :param AllowDoubleMatching: when False, each ground truth marker is only allowed to match with one distorted
+        marker. However, sometimes this can result in a chain reaction where one marker gets mismatched then every
+        other marker gets mismatched too. In these cases you can set this parameter to True, and any double matched
+        markers will simply be deleted.
+    :type AllowDoubleMatching: bool, optional
+    :param sorting_method: 'radial' or 'nearest'. This is only important if WarpSearchData is True; in that case,
+        we are building a motion model on-the-fly based on previously seen markers, so the order we see them can be
+        important. For data on a sphere, you may have more success by setting this to 'nearest', but this is a bit
+        of an untested feature
+    :type sorting_method: str, optional
+    :param n_refernce_markers: the n inner_most Reference markers are used to align the ground truth to the MR volume
+        before  matching. this can correct for setup errors. Note that we always move the reference. the best way
+        for this to not matter either way is to not have any set up error!
+    :type n_refernce_markers: int, optional
+    """
+
+    def __init__(self, GroundTruthData, DistortedData, reverse_gradient_data=None, WarpSearchData=True,
+                 AutomatchMarkers=True, AllowDoubleMatching=False, sorting_method='radial', n_refernce_markers=0):
+
+        # warping parameters:
+        self.WarpSearchData = WarpSearchData
+        self.AutomatchMarkers = AutomatchMarkers
+        self._motion_estimate_update_rate = 1  # 1 = every found marker, which is potentially more accurate but slower.
+        self.sorting_method = sorting_method
+        self.AllowDoubleMatching = AllowDoubleMatching
+
+        self._n_reference_markers = n_refernce_markers
+
+        # marker data:
+        self.ground_truth_centroids = GroundTruthData.MarkerCentroids
+        self.distorted_centroids = DistortedData.MarkerCentroids
+
+        if reverse_gradient_data is None:
+            self.distorted_centroidsRev = None
+        else:
+            self.distorted_centroidsRev = reverse_gradient_data.MarkerCentroids
+
+        self._check_input_data()
+        # run analysis:
+
+        # for testing
+        # self._add_setup_error(mm_deg=10)
+
+        if self._n_reference_markers > 0:
+            self._align_reference()
+
+        if self.AutomatchMarkers:
+            self.distorted_centroids = self._sort_distorted_centroids(self.distorted_centroids)
+            self._CentroidMatch = self._match_distorted_markers_to_ground_truth(self.distorted_centroids)
+            if self.distorted_centroidsRev is not None:
+                self.distorted_centroidsRev = self._sort_distorted_centroids(self.distorted_centroidsRev)
+                self._CentroidMatchRev = self._match_distorted_markers_to_ground_truth(self.distorted_centroidsRev)
+        else:
+            self._create_marker_data_prematched_markers()
+        self._handle_double_matched_markers()
+
+        # analyse marker positions
+        self._generate_marker_position_data()
+
+    def _check_input_data(self):
+        """
+        put any tests on the input data here to make sure the rest of the code can run.
+
+        - tests that there at least as many ground truth centroids than distorted centroids
+        - tests that data appears to be in mm (requirement)
+        """
+        if not self.ground_truth_centroids.shape[0] >= self.distorted_centroids.shape[0]:
+            raise ValueError('There are fewer ground truth centroids than distorted centroids; this means the disorted'
+                             'centroids can never be matched')
+
+        if not self.AutomatchMarkers:
+            if not self.ground_truth_centroids.shape[0] == self.distorted_centroids.shape[0]:
+                raise ValueError(
+                    f'Since you have set AutomatchMarkers=False, there must be equal numbers of ground truth'
+                    f'markers and distorted markers, but ground truth has {self.ground_truth_centroids.shape[0]}'
+                    f'and distorted has {self.distorted_centroids.shape[0]}.')
+
+        if self.distorted_centroidsRev is not None:
+            if not self.ground_truth_centroids.shape[0] >= self.distorted_centroidsRev.shape[0]:
+                raise ValueError('There are fewer ground truth centroids than reversed gradient distorted centroids;'
+                                 ' this means the disorted centroids can never be matched. Quitting')
+
+        if np.max([self.ground_truth_centroids.x.max(), self.ground_truth_centroids.y.max(),
+                   self.ground_truth_centroids.z.max()]) < 50:
+            logger.warning('it appears that the ground truth centroids may not be defined in mm?'
+                           'this will cause the algorithm to fail. Continuing but double check this!')
+
+        if np.max([self.distorted_centroids.x.max(), self.distorted_centroids.y.max(),
+                   self.distorted_centroids.z.max()]) < 50:
+            logger.warning('it appears that the distorted centroids may not be defined in mm?'
+                           'this will cause the algorithm to fail. Continuing but double check this!')
+        if self.distorted_centroidsRev is not None:
+            if np.max([self.distorted_centroidsRev.x.max(), self.distorted_centroidsRev.y.max(),
+                       self.distorted_centroidsRev.z.max()]) < 50:
+                logger.warning('it appears that the reverse gradient distorted centroids may not be defined in mm? '
+                               'this will cause the algorithm to fail. Continuing but double check this!')
+
+    def _get_grid_spacing(self):
+        """
+        Get the spacing between markers using the ground truth data. This is used to build the kernel for RBF
+        interpolation during the marker matching step.
+        """
+        self._x_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.x))))
+        self._y_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.y))))
+        self._z_grid_spacing = np.mean(np.diff(np.sort(np.unique(self.ground_truth_centroids.z))))
+
+    def _generate_extrapolant_models(self, CentroidsToSearch, distorted_centroids):
+        """
+        Use the found marker positions to extrapolate the distortion at other positions.
+
+        :param CentroidsToSearch: Current search data. At this point this is based on the
+            ground truth data with matched markers removed.
+
+        returns X_dist, Y_dist, Z_dist, which is the distortion at every marker position in
+        CentroidsToSearch.
+        """
+        points = self.ground_truth_centroids.iloc[self._MatchInd][['x', 'y', 'z']]
+        distortion = self.ground_truth_centroids.iloc[self._MatchInd].to_numpy() - \
+                     distorted_centroids.iloc[0:len(self._MatchInd)].to_numpy()
+
+        # Nearest Neighbore interpolator
+        self._X_interpolator = NearestNDInterpolator(points, distortion[:, 0])
+        self._Y_interpolator = NearestNDInterpolator(points, distortion[:, 1])
+        self._Z_interpolator = NearestNDInterpolator(points, distortion[:, 2])
+
+        points = CentroidsToSearch[['x', 'y', 'z']].to_numpy().squeeze()
+        X_dist = self._X_interpolator(points)
+        Y_dist = self._Y_interpolator(points)
+        Z_dist = self._Z_interpolator(points)
+        return X_dist, Y_dist, Z_dist
+
+    def _align_reference(self, rotation=True):
+        """
+        Moves the ground truth markers to be aligned with the distorted markers based on the central n refernce markers
+        """
+        if self.ground_truth_centroids is None or self.distorted_centroids is None:
+            logger.warning('No centroids loaded')
+            return
+
+        def _calculate_radial_distance(centroids):
+            """
+            insert the radial value of each marker:
+            """
+            centroids['r'] = centroids.apply(
+                lambda row: np.sqrt(row[0] ** 2 + row[1] ** 2 + row[2] ** 2), axis=1)
+            if centroids.r.mean() < 10:
+                logger.warning('it appears that your input data is in m, not mm - please use mm!')
+            return centroids
+
+        def _match_crosshair(search_centroids, reference_centroids):
+            """
+            match the distorted/ ground truth
+            """
+
+            _matched_reference = pd.DataFrame(columns=['x', 'y', 'z'])
+            search_centroids.reset_index(inplace=True, drop=True)
+            reference_centroids.reset_index(inplace=True, drop=True)
+            for index, row in reference_centroids.iterrows():
+                # Calculate distance from this marker to each item in search list
+                Distances = cdist(search_centroids, np.atleast_2d(row), metric='euclidean')
+                # Match marker with closest and save it
+                ind_nearest = np.argmin(Distances)
+                matched = search_centroids.iloc[ind_nearest]
+                _matched_reference.loc[index] = matched
+
+            return _matched_reference
+
+        # Find the central position in the ground truth data
+        ground_truth = self.ground_truth_centroids.copy()
+        central_x = (ground_truth.x.min() + ground_truth.x.max()) / 2
+        central_y = (ground_truth.y.min() + ground_truth.y.max()) / 2
+        central_z = (ground_truth.z.min() + ground_truth.z.max()) / 2
+
+        # Calculate the distance between each marker and central position
+        ground_truth['r_centre'] = ground_truth.apply(
+            lambda row: np.sqrt((row[0] - central_x) ** 2 + (row[1] - central_y) ** 2 + (row[2] - central_z) ** 2),
+            axis=1)
+
+        # Find the crosshair reference markers
+        gt_reference = ground_truth.nsmallest(self._n_reference_markers, 'r_centre')[['x', 'y', 'z']]
+        dist_reference = self.distorted_centroids.nsmallest(self._n_reference_markers, 'r')[['x', 'y', 'z']]
+
+        # Calculate translation vector
+        translation_vector = dist_reference.mean() - gt_reference.mean()
+
+        # Calculate rotation vector
+        if self._n_reference_markers < 3:
+            rotation = False
+        else:
+            matched_reference = _match_crosshair(gt_reference + translation_vector, dist_reference)
+            rotation_vector, error = transform.Rotation.align_vectors(dist_reference, matched_reference)
+
+        # Transform centroids
+        aligned = self.ground_truth_centroids[['x', 'y', 'z']] + translation_vector
+
+        if rotation is True:
+            aligned = rotation_vector.apply(aligned)
+
+        aligned = pd.DataFrame(aligned, columns=['x', 'y', 'z'])
+        self.ground_truth_centroids = _calculate_radial_distance(aligned)
+
+    def _match_distorted_markers_to_ground_truth(self, CentroidsToMatch):
+        """
+        find the closest ground truth marker to a given distortion. The logic of this algorithm is based on Paul
+        Liu's matlab version
+
+        1. Distorted data is sorted by r so that the smallest (least distorted) markers are processed first
+        2. the match is simply based on the minimum distance in cartesian space between the distorted marker and the
+            search markers.
+        3. Once a match has been found, that ground truth is removed from the search space
+        4. if self.WarpSearchData=True, the search markers are warped according to the previously found data. For cases
+            where distortion is small this is probably unnecessary, but for extreme distortions this algorithm will fail
+            without this
+        """
+
+        self._MatchInd = []
+        distances = []
+        CentroidsToSearch = self.ground_truth_centroids.copy()
+        for index, row in CentroidsToMatch.iterrows():
+
+            XA = CentroidsToSearch[["x", "y", "z"]].to_numpy()
+            XB = row[0:3].values
+            # Calculate distance from this marker to each item in search list
+            Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
+            # Match marker with closest and save it
+            ind_closest_point_in_ground_truth = np.argmin(Distances)
+            self._MatchInd.append(ind_closest_point_in_ground_truth)
+            distances.append(np.linalg.norm(
+                self.ground_truth_centroids.iloc[ind_closest_point_in_ground_truth][['x', 'y', 'z']] - row[
+                    ['x', 'y', 'z']]))
+            if not self.AllowDoubleMatching:
+                CentroidsToSearch.iloc[ind_closest_point_in_ground_truth] = pd.Series(
+                    {'x': 1000, 'y': 1000, 'z': 1000, 'r': 1732})
+
+            # warp search data?
+            if self.WarpSearchData and (index % self._motion_estimate_update_rate == 0) and index > 0:
+                # get extrapolated motion at all points:
+                X_dist, Y_dist, Z_dist = self._generate_extrapolant_models(CentroidsToSearch, CentroidsToMatch)
+                # regenerate centroids to search:
+                CentroidsToSearch = self.ground_truth_centroids.copy()
+                # remove found entries:
+                if not self.AllowDoubleMatching:
+                    CentroidsToSearch.iloc[self._MatchInd] = pd.Series({'x': 1000, 'y': 1000, 'z': 1000, 'r': 1732})
+                # update the data with the extrapolated motion
+                CentroidsToSearch[['x']] = CentroidsToSearch[['x']] - X_dist[:, None]
+                CentroidsToSearch[['y']] = CentroidsToSearch[['y']] - Y_dist[:, None]
+                CentroidsToSearch[['z']] = CentroidsToSearch[['z']] - Z_dist[:, None]
+
+        # create a new data frame that has the distorted and ground truth markers
+        MatchedMarkers = self.ground_truth_centroids.iloc[self._MatchInd]
+        MatchedMarkers = MatchedMarkers.rename(columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
+        MatchedMarkers.reset_index(inplace=True, drop=True)
+        MatchedCentroids = pd.concat([CentroidsToMatch, MatchedMarkers], axis=1)
+        MatchedCentroids['match_distance'] = distances
+
+        return MatchedCentroids
+
+    def _handle_double_matched_markers(self):
+        """
+        Checks if any distorted markers have been matched to the same ground truth point
+        """
+        non_unique_ind = self._CentroidMatch.duplicated(subset=['x_gt', 'y_gt', 'z_gt'], keep=False)
+        if any(non_unique_ind):
+            logger.error(f'{np.count_nonzero(non_unique_ind)} distorted centroids were matched to the same ground truth'
+                         f'marker. This may be indicative of a serious issue and you should proceed with caution. For '
+                         f'now, handling this by removing these entries from the analysis pool and continuing...')
+            self._CentroidMatch.drop(self._CentroidMatch.index[non_unique_ind])
+            self._CentroidMatch.reset_index(drop=True)
+
+        if self.distorted_centroidsRev is not None:
+            non_unique_ind = self._CentroidMatchRev.duplicated(subset=['x_gt', 'y_gt', 'z_gt'], keep=False)
+            if any(non_unique_ind):
+                logger.error(
+                    f'{np.count_nonzero(non_unique_ind)} distorted centroids were matched to the same ground truth'
+                    f'marker. This may be indicative of a serious issue and you should proceed with caution. For '
+                    f'now, handling this by removing these entries from the analysis pool and continuing...')
+                self._CentroidMatchRev.drop(self._CentroidMatchRev.index[non_unique_ind])
+                self._CentroidMatchRev.reset_index(drop=True)
+
+    def _create_marker_data_prematched_markers(self):
+        """
+        If no autosorting is requested, this creates the MatchedCentroids DataFrame directly from the input data
+        with no sorting etc.
+        """
+        self._CentroidMatch = self.ground_truth_centroids
+        self._CentroidMatch = self._CentroidMatch.rename(columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
+        self._CentroidMatch = pd.concat([self._CentroidMatch, self.distorted_centroids], axis=1)
+
+        if self.distorted_centroidsRev is not None:
+            self._CentroidMatchRev = self.ground_truth_centroids
+            self._CentroidMatchRev = self._CentroidMatchRev.rename(
+                columns={"x": "x_gt", "y": "y_gt", "z": "z_gt", "r": "r_gt"})
+            self._CentroidMatchRev = pd.concat([self._CentroidMatchRev, self.distorted_centroidsRev], axis=1)
+
+    def _generate_marker_position_data(self):
+        """
+        Convert the marker position data to the data we want to use for calculating gradient and B0 distortion
+        If only one dataset has been entered, then this is trivial. However, if we have a forward and reverse dataset
+        then we need to use these two seperate the gradient and B0 effects.
+        """
+        if self.distorted_centroidsRev is None:
+            # then our life is easy
+            self.MatchedCentroids = self._CentroidMatch
+            self.MatchedCentroids = self.MatchedCentroids.rename(
+                columns={'x': 'x_gnl', 'y': 'y_gnl', 'z': 'z_gnl', 'r': 'r_gnl'})
+        else:
+            # then we have to do some work to seperate G and B0
+
+            # first we will want to correlate the marker positions by sorting by ground truth r
+            self._CentroidMatch = self._CentroidMatch.sort_values('r_gt').reset_index(drop=True)
+            self._CentroidMatchRev = self._CentroidMatchRev.sort_values('r_gt').reset_index(drop=True)
+            # now find an index where the ground truth markers match; we will discard other markers
+            rev_match_index = []
+            forward_match_index = []
+            tol = 1e-1  # just a small number not a sensitve parameter
+            n_unmatched_markers = 0
+            for index, row in self._CentroidMatch.iterrows():
+                # find the closest ground truth point in the reversed data
+                XA = self._CentroidMatchRev[["x_gt", "y_gt", "z_gt"]].to_numpy()
+                XB = row[['x_gt', 'y_gt', 'z_gt']].values
+                # Calculate distance from this marker to each item in search list
+                Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
+                # calculate location of minimum
+                min_dist_ind = np.argmin(Distances)
+                # if it is less than tolerance, record the position
+                if Distances[min_dist_ind] < tol:
+                    rev_match_index.append(min_dist_ind)
+                    forward_match_index.append(index)
+                else:
+                    n_unmatched_markers += 1  # don't actually need this as can infer from data sizes.
+
+            if n_unmatched_markers > 0:
+                logger.warning(
+                    f'failed to match {n_unmatched_markers} of a total {self.ground_truth_centroids.shape[0]}'
+                    f' input markers. These will be deleted from returned data')
+            # now we have indexes linking our two datasets based on their ground truth match
+            self._CentroidMatchRev = self._CentroidMatchRev.iloc[rev_match_index].reset_index()
+            self._CentroidMatch = self._CentroidMatch.iloc[forward_match_index].reset_index()
+
+            # marker position distortion from gradients is difference between forward and reversed:
+            self.MatchedCentroids = (self._CentroidMatch[['x', 'y', 'z', 'r']] + self._CentroidMatchRev[
+                ['x', 'y', 'z', 'r']]) / 2
+            self.MatchedCentroids = self.MatchedCentroids.rename(
+                columns={'x': 'x_gnl', 'y': 'y_gnl', 'z': 'z_gnl', 'r': 'r_gnl'})
+            # add ground truth to data frame
+            self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt', 'r_gt']] = self._CentroidMatch[
+                ['x_gt', 'y_gt', 'z_gt', 'r_gt']]
+            # marker position distortion from B0 is difference between from total and gradient distortion:
+            '''
+            deta_z_B0=z_dis_AP-z_GNL; %% maximum distortion is 16mm
+            deta_y_B0=y_dis_AP-y_GNL;  %% maximum distortio is 4mm  
+            '''
+            B0_dis = self.MatchedCentroids[['x_gnl', 'y_gnl', 'z_gnl']].to_numpy() - \
+                     self._CentroidMatch[['x', 'y', 'z']].to_numpy()
+            B0_pos = B0_dis + self.MatchedCentroids[['x_gt', 'y_gt', 'z_gt']].to_numpy()
+            self.MatchedCentroids[['x_B0', 'y_B0', 'z_B0']] = B0_dis
+
+    def _sort_distorted_centroids(self, data_to_sort):
+        """
+        sorts the data frame.
+        sorting is important, because the search for a matching ground truth marker is carried out in order
+        """
+
+        if self.sorting_method == 'radial':
+            # sort input data by r
+            data_to_sort = data_to_sort.sort_values('r')
+            data_to_sort.reset_index(inplace=True, drop=True)
+        if self.sorting_method == 'closest':
+            # find the distorted marker that has the closest match to a ground truth marker.
+            min_distance = []
+            XA = self.ground_truth_centroids[["x", "y", "z"]].to_numpy()
+            for index, row in data_to_sort.iterrows():
+                XB = row[0:3].values
+                Distances = cdist(XA, np.atleast_2d(XB), metric='euclidean')
+                min_distance.append(np.min(Distances))
+            starting_marker_ind = np.argmin(min_distance)
+            # now calculate the distances of every other distorted marker to this marker:
+            XA = data_to_sort[["x", "y", "z"]].to_numpy()
+            XB = np.atleast_2d(data_to_sort.loc[starting_marker_ind][["x", "y", "z"]].to_numpy())
+            Distances = cdist(XA, XB)
+            distance_to_start_ind = np.argsort(Distances, axis=0)
+            assert distance_to_start_ind[0] == starting_marker_ind
+            data_to_sort = data_to_sort.reindex(np.squeeze(distance_to_start_ind))
+            data_to_sort.reset_index(inplace=True, drop=True)
+
+        return data_to_sort
+
+    # public methods
+
+    def plot_3D_markers(self, add_arrows=True, title='3D marker positions'):  # pragma: no cover
+        """
+        Works very similarly to the MarkerVolume version, but plots both sets of markers and adds arrows
+
+        :param add_arrows: if True, arrows drawn between matches
+        :type add_arrows: bool, optional
+        :param title: plot title
+        :type title: str, optional
+        """
+
+        fig = plt.figure()
+        axs = fig.add_subplot(111, projection='3d')
+        axs.scatter(self.MatchedCentroids.x_gt, self.MatchedCentroids.y_gt, self.MatchedCentroids.z_gt)
+        axs.scatter(self.MatchedCentroids.x_gnl, self.MatchedCentroids.y_gnl, self.MatchedCentroids.z_gnl)
+        if add_arrows:
+            mag_color = np.sqrt((self.MatchedCentroids.x_gt - self.MatchedCentroids.x_gnl) ** 2
+                                + (self.MatchedCentroids.y_gt - self.MatchedCentroids.y_gnl) ** 2
+                                + (self.MatchedCentroids.z_gt - self.MatchedCentroids.z_gnl) ** 2)
+            axs.quiver(self.MatchedCentroids.x_gnl, self.MatchedCentroids.y_gnl, self.MatchedCentroids.z_gnl,
+                       self.MatchedCentroids.x_gt - self.MatchedCentroids.x_gnl,
+                       self.MatchedCentroids.y_gt - self.MatchedCentroids.y_gnl,
+                       self.MatchedCentroids.z_gt - self.MatchedCentroids.z_gnl,
+                       edgecolors=("black",))
+
+        axs.set_xlabel('X [mm]')
+        axs.set_ylabel('Y [mm]')
+        axs.set_zlabel('Z [mm]')
+        axs.set_title(title)
+        axs.set_box_aspect((np.ptp(self.MatchedCentroids.x_gt), np.ptp(self.MatchedCentroids.y_gt),
+                            np.ptp(self.MatchedCentroids.z_gt)))
+        plt.legend(['ground truth', 'distorted'])
+        plt.show()
+
+    def plot_compressed_markers(self, z_max=20, z_min=-20, add_arrows=True, title=None):  # pragma: no cover
+        """
+        compresses the 3D markers in the z plane, allowing a 2D visualisation.
+
+        :param z_max: maximum z coordiante of markers to includes
+        :type z_max: float, optional
+        :param z_min: minimum z coordiante of markers to includes
+        :type z_min: float, optional
+        :param add_arrows: if True, arrows drawn between matches
+        :type add_arrows: bool, optional
+        :param title: plot title
+        :type title: str, optional
+
+        """
+
+        def get_markers_as_function_of_z():
+            """
+            finds an index of markers within tolerence of z_pos
+            """
+            data_ind = np.logical_and(self.MatchedCentroids.z_gt > z_min, self.MatchedCentroids.z_gt < z_max)
+            z_loc_data = self.MatchedCentroids[data_ind]
+            return z_loc_data
+
+        def plot_markers_inner(plot_data):
+            """
+            clears exising axes and plots plot_data
+            """
+            axs.clear()
+            z_offset = (plot_data.z_gt - plot_data.z_gnl)
+            axs.scatter(plot_data.x_gnl, plot_data.y_gnl, c='darkturquoise')  # c=z_offset,cmap="magma"
+            axs.scatter(plot_data.x_gt, plot_data.y_gt, c='darkgoldenrod')
+            # axs.legend(['Distorted', 'Ground Truth'])
+            if add_arrows:
+                axs.quiver(plot_data.x_gnl, plot_data.y_gnl,
+                           plot_data.x_gt - plot_data.x_gnl,
+                           plot_data.y_gt - plot_data.y_gnl,
+                           angles="xy", units='xy', scale=1, width=1)
+            axs.set_xlim([-150, 150])
+            axs.set_ylim([-150, 150])
+            axs.set_xlabel('x [mm]', fontsize=15)
+            axs.set_ylabel('y [mm]', fontsize=15)
+            axs.tick_params(axis='both', which='major', labelsize=12)
+            axs.tick_params(axis='both', which='minor', labelsize=12)
+            axs.axis("equal")
+            axs.grid()
+            plt.subplots_adjust(bottom=0.25)
+            plt.legend(['distorted', 'ground truth'])
+            if title:
+                plt.title(title)
+
+        fig, axs = plt.subplots(figsize=[8, 8], ncols=1, nrows=1)
+
+        plot_data = get_markers_as_function_of_z()
+        plot_markers_inner(plot_data)
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/Reports.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/Reports.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,613 +1,610 @@
-import sys
-import os
-from pathlib import Path
-import numpy as np
-import logging
-import plotly.express as px
-import pandas as pd
-from .utilities import get_harmonics, convert_cartesian_to_spherical, reconstruct_Bz
-from .utilities import convert_spherical_to_cartesian
-import plotly.graph_objects as go
-from distutils.dir_util import copy_tree
-from datetime import datetime
-from jinja2 import Template
-from .utilities import get_dicom_data
-
-ch = logging.StreamHandler()
-formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
-ch.setFormatter(formatter)
-logger = logging.getLogger(__name__)
-logger.addHandler(ch)
-logger.setLevel(logging.INFO)  # This toggles all the logging in your app
-logger.propagate = False
-
-
-class TG284_Tests:  # pragma: no cover
-    """
-    tests defined here
-    https://aapm.onlinelibrary.wiley.com/doi/full/10.1002/mp.14695
-    """
-    def test_distortion_less_than_1mm_within_r_100(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
-        if test_data.abs_dis.max() < 1:
-            return True
-        else:
-            return False
-
-    def test_distortion_less_than_2mm_within_r_200(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=200)
-        if test_data.abs_dis.max() < 1:
-            return True
-        else:
-            return False
-
-
-class DefaultTestSuite:  # pragma: no cover
-    """
-    these are the tests which are run if no others are specified
-    """
-
-    def test_distortion_less_than_2mm_within_r_100(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
-        if test_data.abs_dis.max() < 2:
-            return True
-        else:
-            return False
-
-    def test_distortion_less_than_4mm_within_r_150(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=150)
-        if test_data.abs_dis.max() < 4:
-            return True
-        else:
-            return False
-
-
-class Elekta_Distortion_tests:  # pragma: no cover
-    """
-    Geometric tests for Elekta system as described here:
-    https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.14764
-    """
-
-    def test_distortion_less_than_1_mm_within_r_100_mm(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
-        if test_data.abs_dis.max() < 1:
-            return True
-        else:
-            return False
-
-    def test_distortion_less_than_2_mm_within_r_150_mm(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=150)
-        if test_data.abs_dis.max() < 2:
-            return True
-        else:
-            return False
-
-    def test_distortion_less_than_4_mm_within_r_200_mm(self):
-        """
-        distortion test to be run by MRI_QA_Reporter
-        """
-        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=200)
-        if test_data.abs_dis.max() < 4:
-            return True
-        else:
-            return False
-
-
-class MRI_QA_Reporter:
-    """
-    generate a report based on either some matched data, or harmonics. In the latter case, report data is reconstructed.
-
-    :param MatchedMarkerVolume: pandas dataframe containing  ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl']
-        You must enter one of MatchedMarkerVolume or gradient_harmonics
-    :type MatchedMarkerVolume: pandas.DataFrame, optional
-    :param gradient_harmonics: list of either three pandas series or three paths to csv files
-        from SphericalHarmonicFit.
-        List elements should correspond to [G_x_harmonics, G_y_harmonics, G_z_harmonics].
-        You must enter one of MatchedMarkerVolume or gradient_harmonics
-    :type gradient_harmonics: list, optional
-    :param B0_harmonics: pandas series from SphericalHarmonicFit or path to saved csv file. If entered, is used
-        to report and plot B0 homogeneity
-    :type B0_harmonics: pandas.Series or path, optional
-    :param recon_coords: The coordinates you want to calculate the fields at. a pandas Dataframe which can contain
-        whatever you want, but MUST contain columns called: x, y, z. If left as None a default is generated.
-    :type recon_coords: pandas.DataFrame, optional
-    :param tests_to_run: a class containing any tests to run. The class in this instance serves only as a name
-        space. All methods inside the class starting with 'test' are identified as tests. The test methods will
-        have access to everything inside this class.
-    :type tests_to_run: class, optional
-    :param dicom_data: either a dictionary or path to a saved json file of the dicom_data object generated by
-        MarkerVolume. This data is required for harmonic reconstruction. For MatchedMarkerVolume it is not required,
-        but it does contain useful information about the acquisition so still a good idea to use it.
-    :type dicom_data: dict or path to json, optional
-    :param r_outer: for the harmonic approach, r_outer is used to determine where the data is reconstructed. It is
-        also used to control the limits in which data is plotted
-    :type r_outer: float, optional
-    :param show_plots: if True, all plots will be shown in your browser. Otherwise they are only saved
-    :type show_plots: bool, optional
-    :param style: control the report style. At the moment can only be 'light' or 'dark'
-    :type style: str
-    """
-
-    def __init__(self, MatchedMarkerVolume=None, gradient_harmonics=None, B0_harmonics=None,
-                 recon_coords_cartesian=None, tests_to_run=DefaultTestSuite, dicom_data=None,
-                 r_outer=None, show_plots=False, style='dark'):
-
-        self._html_template_loc = Path(__file__).parent.resolve() / 'jinja_templates' / 'MR_report.html'
-        self._show_plots = show_plots
-        _available_plotly_themes = ["plotly", "plotly_white", "plotly_dark", "ggplot2",
-                                    "seaborn", "simple_white", "none"]
-        self._style = style
-        self._set_styles()
-        self._jinja_dict = {}  # this will hold all the info jinja needs to render
-        self._test_class = tests_to_run
-        self.r_outer = r_outer
-        self.recon_coords_cartesian = recon_coords_cartesian
-        self.dicom_data = get_dicom_data(dicom_data)
-        self._build_acquisition_dict()
-        self._get_analysis_data(MatchedMarkerVolume, gradient_harmonics, B0_harmonics)
-        self._update_MatchedMarkerVolume()
-
-        # put plots here
-        self._plot_distortion_v_r()
-        self._plot_3D_cutplanes()
-        self._plot_B0_surface()
-        self._build_homogeneity_report_table()
-        # self._plot_gradients_surface()
-        self._get_test_results()
-
-    def _build_acquisition_dict(self):
-        """
-        will try and extract acquisition data from dicom_data, and put it in a new dictionary
-        if this new dictionary exists, we will include the acquisition data in the report
-        """
-        if self.dicom_data is None:
-            return
-        self._jinja_dict['acquisition_data'] = {}
-        _fields_of_interest = ['acquisition_date', 'magnetic_field_strength', 'bandwidth', 'pixel_spacing',
-                               'freq_encode_direction', 'manufacturer','sequence_name', 'imaging_frequency']
-        for key in self.dicom_data:
-            if key in _fields_of_interest:
-                new_key = key.replace('_', ' ')
-                self._jinja_dict['acquisition_data'][new_key] = self.dicom_data[key]
-
-    def _set_styles(self):
-        """
-        sets the report style by changing the plotly theme and chanding the html css file
-        """
-        if self._style == 'dark':
-            self._plotly_theme = 'plotly_dark'
-            self._html_theme = "themes/d42ker-github.css"
-        elif self._style == 'light':
-            self._plotly_theme = 'plotly_white'
-            self._html_theme = "themes/whitey.css"
-        else:
-            raise AttributeError(f'unknown style entered: {self._style}. allowed options are "light" or "dark"')
-
-    def _unique_name_generator(self, save_loc, input_name, rel_path=True):
-        """
-        take input name, append the current date to it
-        then check if this new name already exists in save_loc; if it does add integers to it (_1, _2, etc.) until it doesn't
-        """
-        if not save_loc.is_dir():
-            # in this case, the code will likely fail downstream but we don't have to do anything here
-            return input_name
-        input_name, extension = os.path.splitext(input_name)
-        now = datetime.now()  # current date and time
-        date_string = now.strftime("%d_%m_%Y")
-        new_name = input_name + '_' + date_string
-        appended_int = 0
-        while (save_loc / (new_name + extension)).is_file():
-            appended_int = appended_int + 1
-            new_name = new_name + '_' + str(appended_int)
-        new_name = new_name + extension
-        if rel_path:
-            new_name = (save_loc  / new_name).relative_to(save_loc.parent)
-        else:
-            new_name = save_loc / new_name
-        return new_name
-
-    def _get_test_results(self):
-        """
-        runs through all tests found in the _test_class and keeps all the results in _jinja_dict
-        """
-
-        self._jinja_dict['test_collection'] = {}
-        self._jinja_dict['TestSuiteName'] = self._test_class.__name__
-        method_list = [method for method in dir(self._test_class) if method.startswith('__') is False]
-        # this will list all methods except 'dunder' methods e.g. __init__
-        for test in method_list:
-            if test[:4] == 'test':
-                # then we found a true test
-                test_name = test.replace('_', ' ') # under scores to space
-                test_name = test_name.replace('test ','' )  # remove test from the name
-                test_string = getattr(self._test_class, test)(self)
-                if isinstance(test_string, bool):
-                    if test_string:
-                        test_string = "<span style='color:green'>Pass</span>"
-                    else:
-                        test_string = "<span style='color:red'>Fail</span>"
-                elif not isinstance(test_string, str):
-                    raise TypeError('please return test results as either booleans or strings')
-                self._jinja_dict['test_collection'][test_name] = test_string
-
-    def _get_analysis_data(self, MatchedMarkerVolume, gradient_harmonics, B0_harmonics):
-        """
-        check what the user has input, and attach to self
-        if necessary, convert gradient_harmonics to distortion map
-        """
-
-        if MatchedMarkerVolume is not None and gradient_harmonics is not None:
-            raise AttributeError(
-                f'you cannot enter both MatchedMarkerVolume and gradient_harmonics at the same time...')
-
-        if MatchedMarkerVolume is not None:
-            self._check_marker_volume(MatchedMarkerVolume)
-            self._MatchedMarkerVolume = MatchedMarkerVolume.copy()
-
-        if gradient_harmonics is not None:
-            self._check_dicom_data()
-            self._Gx_Harmonics, self._Gy_Harmonics, self._Gz_Harmonics, self._B0_harmonics = \
-                get_harmonics(gradient_harmonics[0], gradient_harmonics[1], gradient_harmonics[2])
-            self._Gx_Harmonics = self._Gx_Harmonics * self.dicom_data['gradient_strength'][0]
-            self._Gy_Harmonics = self._Gy_Harmonics * self.dicom_data['gradient_strength'][1]
-            self._Gz_Harmonics = self._Gz_Harmonics * self.dicom_data['gradient_strength'][2]
-            if self.r_outer is None:
-                logger.warning('no r_outer value entered, using 150 mm')
-                self.r_outer = 150
-            if self.recon_coords_cartesian is None:
-                self.recon_coords_cartesian = self._generate_recon_coords()
-            self.recon_coords = convert_cartesian_to_spherical(self.recon_coords_cartesian)
-            self._reconstruct_gradient_fields()
-            self._convert_magnetic_field_to_distortion()
-
-        if B0_harmonics is not None:
-            if isinstance(B0_harmonics, pd.Series):
-                self.B0_harmonics = B0_harmonics
-            elif isinstance(B0_harmonics, (str, Path)):
-                self.B0_harmonics = pd.read_csv(B0_harmonics, index_col=0).squeeze("columns")
-            else:
-                raise AttributeError('could not read in B0_harmonics...please input either a series or a '
-                                     'path to a saved csv file')
-        else:
-            self.B0_harmonics = None
-
-    def _convert_magnetic_field_to_distortion(self):
-        """
-        converts reconstructed gradient fields into geometric distortion.
-        Essentially this process is doing the opposite of FieldCalculation.ConvertMatchedMarkersToBz
-        """
-        self._MatchedMarkerVolume = pd.DataFrame()
-        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(x_gt=self.recon_coords_cartesian.x)
-        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(y_gt=self.recon_coords_cartesian.y)
-        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(z_gt=self.recon_coords_cartesian.z)
-        bandwidth = np.array(self.dicom_data['bandwidth'])
-        image_size = np.array(self.dicom_data['image_size'])
-        gama = np.array(self.dicom_data['gama'])
-        FOV = np.array(self.dicom_data['FOV'])
-
-        gradient_strength = bandwidth * image_size / (gama * 1e6 * FOV * 1e-3)  # unit(T / m)
-        # ^ this is a vector [gx, gy, gz]
-        # factor of 1e3 is for m to mm
-        self._MatchedMarkerVolume = \
-            self._MatchedMarkerVolume.assign(x_gnl=self.Gx_Bfield * 1e3 / (gradient_strength[0]))
-        self._MatchedMarkerVolume = \
-            self._MatchedMarkerVolume.assign(y_gnl=self.Gy_Bfield * 1e3 / (gradient_strength[1]))
-        self._MatchedMarkerVolume = \
-            self._MatchedMarkerVolume.assign(z_gnl=self.Gz_Bfield * 1e3 / (gradient_strength[2]))
-
-    def _reconstruct_gradient_fields(self):
-        """
-        utilise the utilities.reconstruct_Bz function to reconsutrct each of the gradient fields at recon_coords
-        """
-        self.Gx_Bfield = reconstruct_Bz(self._Gx_Harmonics, self.recon_coords, quantity='T')
-        self.Gy_Bfield = reconstruct_Bz(self._Gy_Harmonics, self.recon_coords, quantity='T')
-        self.Gz_Bfield = reconstruct_Bz(self._Gz_Harmonics, self.recon_coords, quantity='T')
-
-    def _build_homogeneity_report_table(self):
-        """
-        Generate a table of predicted pk-pk homogeneity at different r
-        :return:
-        """
-        if self.B0_harmonics is None:
-            return
-        radii_of_interest = [50, 100, 150, 200]
-        pk_pk = []
-        for DSV_radius in radii_of_interest:
-            azimuth = np.linspace(0, 2 * np.pi, 100)
-            elevation = np.linspace(0, np.pi, 100)
-            [AZ, EL, R] = np.meshgrid(azimuth, elevation, DSV_radius, indexing='ij')
-            surface_coords = pd.DataFrame({'r': R.flatten(), 'azimuth': AZ.flatten(), 'elevation': EL.flatten()})
-            surface_coords = convert_spherical_to_cartesian(surface_coords)
-            B0 = reconstruct_Bz(self.B0_harmonics, surface_coords, quantity='T', r_outer=DSV_radius)
-            pk_pk.append(int((B0.max() - B0.min()) * 1e6))
-        _B0_stats = pd.DataFrame({'r': radii_of_interest, 'pk_pk [\u03BCT]': pk_pk} )
-
-        self._B0_table = go.Figure(data=[go.Table(
-            header=dict(values=list(_B0_stats.columns),
-                        align='left'),
-            cells=dict(values=[_B0_stats.r, _B0_stats['pk_pk [\u03BCT]']],
-                       align='left'))
-        ])
-        self._B0_table.update_layout(template=self._plotly_theme)
-
-    def _check_dicom_data(self):
-        """
-        check that if input dicom data is required, it confirms to minimum standard
-        """
-        _required_fields = ['FOV', 'bandwidth', 'gama', 'image_size', 'gradient_strength']
-
-        if not isinstance(self.dicom_data, dict) or not all(
-                name in self.dicom_data.keys() for name in _required_fields):
-            raise AttributeError(f'dicom_data must be a dict with at least the following keys: {_required_fields}')
-
-    def _check_marker_volume(self, MatchedMarkerVolume):
-        """
-        check that if a MatchedMarkerVolume is entered, is meets expected format
-        """
-        _required_cols = ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl']
-        if not isinstance(MatchedMarkerVolume, pd.DataFrame) or \
-                not all(name in MatchedMarkerVolume.columns for name in _required_cols):
-            raise AttributeError(f'MatchedMarkerVolume must be a dataframe containing columns'
-                                 f'[x_gt, y_gt, z_gt, x_gnl, y_gnl, z_gnl]')
-
-    def _generate_recon_coords(self):
-        """
-        Generate a grid of coordinates to perform reconstruction
-        """
-        x = np.linspace(-self.r_outer, self.r_outer, 50)
-        y = np.linspace(-self.r_outer, self.r_outer, 50)
-        z = np.linspace(-self.r_outer, self.r_outer, 50)
-        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
-        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
-        return recon_coords
-
-    def _plot_distortion_v_r(self):
-        """
-        generate a histogram as a function of r
-        """
-
-        # data over different planes
-        xy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, z_select=0)
-        xy_plot_data['plane'] = 'XY'
-        zx_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, y_select=0)
-        zx_plot_data['plane'] = 'ZX'
-        zy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, x_select=0)
-        zy_plot_data['plane'] = 'ZY'
-        # create a new data frame combined from these for easy plotting
-        all_dsv_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer)
-        all_dsv_plot_data['plane'] = 'Entire DSV'
-
-
-        plot_data = pd.concat([all_dsv_plot_data, xy_plot_data, zx_plot_data, zy_plot_data], ignore_index=True, axis=0)
-        self._fig_distortion_v_r = px.scatter(plot_data, x="r_gt", y="abs_dis",color="plane",
-                                              labels={
-                                                  "r_gt": "Distance from the center (mm)", #rename the x axis
-                                                  "abs_dis": " Absolute Distortion (mm)", #rename the y axis
-                                              },
-                                              title=f"Cardinal plane data, {self.r_outer} DSV")
-
-
-        self._fig_distortion_v_r.update_layout(template=self._plotly_theme)
-        if self._show_plots:
-            self._fig_distortion_v_r.show()
-
-    def _plot_3D_cutplanes(self):
-        """
-        create a 3D cone plot in each of the three cardinal directions
-        """
-        xy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, z_select=0)
-        zx_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, y_select=0)
-        zy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, x_select=0)
-        plot_data = pd.concat([xy_plot_data, zx_plot_data, zy_plot_data], ignore_index=True, axis=0)
-
-        self._fig_3D_planes = go.Figure(data=go.Cone(
-            x=plot_data['x_gt'],
-            y=plot_data['y_gt'],
-            z=plot_data['z_gt'],
-            u=plot_data['x_dis'],
-            v=plot_data['y_dis'],
-            w=plot_data['z_dis'],
-            colorbar=dict(title= 'mm'),
-            sizemode="absolute",
-            sizeref=1))
-
-
-        self._fig_3D_planes.update_layout(scene=dict(aspectratio=dict(x=1, y=1, z=0.8),
-                                                     camera_eye=dict(x=1.2, y=1.2, z=0.6)))
-        self._fig_3D_planes.update_layout(template=self._plotly_theme, scene = dict(
-                    xaxis_title='X Axis (mm)',
-                    yaxis_title='Y Axis (mm)',
-                    zaxis_title='Z Axis (mm)'))
-        if self._show_plots:
-            self._fig_3D_planes.show()
-
-    def _plot_B0_surface(self):
-        """
-        if self.B0_harmonics exists, reconstruct B0 on the surface of r_outer and make a pretty 3D plot
-        """
-
-        if self.B0_harmonics is None:
-            return
-        # generate surface recon coordinates
-        if self.r_outer is not None:
-            r = self.r_outer
-        else:
-            r = 150
-        azimuth = np.linspace(0, 2 * np.pi, 100)
-        elevation = np.linspace(0, np.pi, 100)
-        [AZ, EL, R] = np.meshgrid(azimuth, elevation, r, indexing='ij')
-        surface_coords = pd.DataFrame({'r': R.flatten(), 'azimuth': AZ.flatten(), 'elevation': EL.flatten()})
-        surface_coords = convert_spherical_to_cartesian(surface_coords)
-
-        B0 = reconstruct_Bz(self.B0_harmonics, surface_coords, quantity='uT', r_outer=r)
-        x = surface_coords.x.to_numpy().reshape(100, 100)
-        y = surface_coords.y.to_numpy().reshape(100, 100)
-        z = surface_coords.z.to_numpy().reshape(100, 100)
-        B0 = B0.to_numpy().reshape(100, 100)
-
-        self._fig_DSV_surface = go.Figure(data=[go.Surface(z=z, x=x, y=y,colorbar=dict(title= 'B(uT)'), surfacecolor=B0)])
-
-        self._fig_DSV_surface.update_layout(title='DSV surface [uT]', autosize=True,
-                          template=self._plotly_theme, scene = dict(
-                    xaxis_title='X Axis (mm)',
-                    yaxis_title='Y Axis (mm)',
-                    zaxis_title='Z Axis (mm)') )
-
-        if self._show_plots:
-            self._fig_DSV_surface.show()
-
-    def _update_MatchedMarkerVolume(self):
-        """
-        adds in 'r_gt', 'r_gnl' and 'dis_x,y,z' to _MatchedMarkerVolume input
-        """
-        self._MatchedMarkerVolume['r_gt'] = np.sqrt(self._MatchedMarkerVolume.x_gt ** 2
-                                                    + self._MatchedMarkerVolume.y_gt ** 2
-                                                    + self._MatchedMarkerVolume.z_gt ** 2)
-        self._MatchedMarkerVolume['r_gnl'] = np.sqrt(self._MatchedMarkerVolume.x_gnl ** 2
-                                                     + self._MatchedMarkerVolume.y_gnl ** 2
-                                                     + self._MatchedMarkerVolume.z_gnl ** 2)
-        self._MatchedMarkerVolume['x_dis'] = self._MatchedMarkerVolume.x_gnl - self._MatchedMarkerVolume.x_gt
-        self._MatchedMarkerVolume['y_dis'] = self._MatchedMarkerVolume.y_gnl - self._MatchedMarkerVolume.y_gt
-        self._MatchedMarkerVolume['z_dis'] = self._MatchedMarkerVolume.z_gnl - self._MatchedMarkerVolume.z_gt
-        self._MatchedMarkerVolume['abs_dis'] = np.sqrt(self._MatchedMarkerVolume.x_dis ** 2
-                                                       + self._MatchedMarkerVolume.y_dis ** 2
-                                                       + self._MatchedMarkerVolume.z_dis ** 2)
-        # get resolution in each direction
-        self._x_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.x_gt.unique())))
-        self._y_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.y_gt.unique())))
-        self._z_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.z_gt.unique())))
-
-    def _extract_data_from_MatchedMarkerVolume(self, x_select=None, y_select=None, z_select=None,
-                                               max_num_points=None, r_max=None):
-        """
-        Extract data from the matched volume for use in direct plotting
-
-        uses the values of _x_res etc. to define a tolerance
-        """
-        if (x_select is None) and (y_select is None) and (z_select is None) and (r_max is None):
-            logger.warning('you should set a value for at least one of x_ind, y_ind, and z_ind or r_max')
-        # start with everything selected, overwrite below
-        x_ind = np.ones(self._MatchedMarkerVolume.shape[0])
-        y_ind = np.ones(self._MatchedMarkerVolume.shape[0])
-        z_ind = np.ones(self._MatchedMarkerVolume.shape[0])
-        r_ind = np.ones(self._MatchedMarkerVolume.shape[0])
-
-        if x_select is not None:
-            x_ind = np.logical_and(self._MatchedMarkerVolume.x_gt <= (x_select + self._x_res / 2),
-                                   self._MatchedMarkerVolume.x_gt >= (x_select - self._x_res / 2))
-        if y_select is not None:
-            y_ind = np.logical_and(self._MatchedMarkerVolume.y_gt <= (y_select + self._y_res / 2),
-                                   self._MatchedMarkerVolume.y_gt >= (y_select - self._y_res / 2))
-        if z_select is not None:
-            z_ind = np.logical_and(self._MatchedMarkerVolume.z_gt <= (z_select + self._z_res / 2),
-                                   self._MatchedMarkerVolume.z_gt >= (z_select - self._z_res / 2))
-        if r_max is not None:
-            r_ind = self._MatchedMarkerVolume.r_gt <= r_max
-
-        select_ind = np.logical_and(np.logical_and(x_ind, y_ind), z_ind)
-        select_ind = np.logical_and(select_ind, r_ind)
-        plot_data = self._MatchedMarkerVolume[select_ind]
-        plot_data = plot_data.reset_index(drop=True)
-        if (max_num_points is not None) and plot_data.shape[0] > max_num_points:
-            every_nth_point = int(plot_data.shape[0] / max_num_points)
-            plot_data = plot_data[plot_data.reset_index().index % every_nth_point == 0]
-
-        return plot_data
-
-    def _set_up_directory_structure(self):
-        """
-        ensure we have a place to save the reports.
-        will set up a directory in
-        """
-        if not os.path.isdir(self.output_folder):
-            os.makedirs(self.output_folder)
-        if not os.path.isdir(self.output_folder / 'plots'):
-            os.mkdir(self.output_folder / 'plots')
-
-        # copy themes
-        theme_dir = (Path(__file__).parent / 'jinja_templates' / 'themes').resolve()
-        copy_tree(str(theme_dir), str(self.output_folder / 'themes'))
-
-    def _get_template(self):
-        """
-        loads the jinja template
-        """
-
-        with open(self._html_template_loc) as f:
-            template_text = f.read()
-        j2_template = Template(template_text)
-        return j2_template
-
-    # public methods
-
-    def write_html_report(self, output_folder=None, report_name=None):
-        """
-        Generates a html report encompassing available acquisition information, test results, and intercative
-        plotly figures
-
-        :param output_folder: folder to write report. Defaults to ~/Documents/MR_QA_Reports
-        :type output_folder: Path or string, optional
-        """
-        if output_folder is None:
-            self.output_folder = Path(os.path.expanduser('~')) / 'Documents' / 'MR_QA_Reports'
-        else:
-            self.output_folder = Path(output_folder)
-        self._set_up_directory_structure()
-
-        if report_name is None:
-            report_name = 'MR_QA_report.html'
-        else:
-            report_name = str(Path(report_name).with_suffix('html'))
-
-        # save plots and update jinja_dict
-
-        distortion_v_r_save_name = self._unique_name_generator(self.output_folder / 'plots', 'distortion_v_r.html')
-        self._fig_distortion_v_r.write_html(self.output_folder / distortion_v_r_save_name, full_html=False, include_plotlyjs='cdn')
-        self._jinja_dict['dist_v_r_source'] = distortion_v_r_save_name
-
-        threeD_plane_save_name = self._unique_name_generator(self.output_folder / 'plots', '3D_planes.html')
-        self._fig_3D_planes.write_html(self.output_folder / threeD_plane_save_name, full_html=False, include_plotlyjs='cdn')
-        self._jinja_dict['cutplanes_source'] = threeD_plane_save_name
-
-        if self.B0_harmonics is not None:
-            DSV_surface_save_name = self._unique_name_generator(self.output_folder / 'plots', 'DSV_surface.html',)
-            self._fig_DSV_surface.write_html(self.output_folder / DSV_surface_save_name, full_html=False, include_plotlyjs='cdn')
-            self._jinja_dict['dsv_surf_source'] = DSV_surface_save_name
-
-            B0_table_save_name = self._unique_name_generator(self.output_folder / 'plots', 'B0_table.html')
-            self._B0_table.write_html(self.output_folder / B0_table_save_name, full_html=False, include_plotlyjs='cdn')
-            self._jinja_dict['B0_table_source'] = B0_table_save_name
-        else:
-            self._jinja_dict['dsv_surf_source'] = None
-
-        # set up template
-        self._jinja_dict['html_theme_loc'] = self._html_theme
-        j2_template = self._get_template()
-        report_name = self._unique_name_generator(self.output_folder, report_name, rel_path=False)
-        report_code = os.path.split(report_name)[1]  # for printing
-        report_code = os.path.splitext(report_code)[0]
-        report_code = report_code.replace('MR_QA_report_','')
-        self._jinja_dict['report_name'] = report_code
-        report_string = j2_template.render(self._jinja_dict)
-        with open(report_name, 'w') as f:
-            f.write(report_string)
-
-        print(f'The report has been compiled and can be found at {self.output_folder}')
+import sys
+import os
+from pathlib import Path
+import numpy as np
+import logging
+import plotly.express as px
+import pandas as pd
+from .utilities import get_gradient_spherical_harmonics, convert_cartesian_to_spherical, reconstruct_Bz
+from .utilities import convert_spherical_to_cartesian
+import plotly.graph_objects as go
+from distutils.dir_util import copy_tree
+from datetime import datetime
+from jinja2 import Template
+from .utilities import get_dicom_data
+
+ch = logging.StreamHandler()
+formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
+ch.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(ch)
+logger.setLevel(logging.INFO)  # This toggles all the logging in your app
+logger.propagate = False
+
+
+class TG284_Tests:  # pragma: no cover
+    """
+    tests defined here
+    https://aapm.onlinelibrary.wiley.com/doi/full/10.1002/mp.14695
+    """
+    def test_distortion_less_than_1mm_within_r_100(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
+        if test_data.abs_dis.max() < 1:
+            return True
+        else:
+            return False
+
+    def test_distortion_less_than_2mm_within_r_200(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=200)
+        if test_data.abs_dis.max() < 1:
+            return True
+        else:
+            return False
+
+
+class DefaultTestSuite:  # pragma: no cover
+    """
+    these are the tests which are run if no others are specified
+    """
+
+    def test_distortion_less_than_2mm_within_r_100(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
+        if test_data.abs_dis.max() < 2:
+            return True
+        else:
+            return False
+
+    def test_distortion_less_than_4mm_within_r_150(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=150)
+        if test_data.abs_dis.max() < 4:
+            return True
+        else:
+            return False
+
+
+class Elekta_Distortion_tests:  # pragma: no cover
+    """
+    Geometric tests for Elekta system as described here:
+    https://aapm.onlinelibrary.wiley.com/doi/epdf/10.1002/mp.14764
+    """
+
+    def test_distortion_less_than_1_mm_within_r_100_mm(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=100)
+        if test_data.abs_dis.max() < 1:
+            return True
+        else:
+            return False
+
+    def test_distortion_less_than_2_mm_within_r_150_mm(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=150)
+        if test_data.abs_dis.max() < 2:
+            return True
+        else:
+            return False
+
+    def test_distortion_less_than_4_mm_within_r_200_mm(self):
+        """
+        distortion test to be run by MRI_QA_Reporter
+        """
+        test_data = self._extract_data_from_MatchedMarkerVolume(r_max=200)
+        if test_data.abs_dis.max() < 4:
+            return True
+        else:
+            return False
+
+
+class MRI_QA_Reporter:
+    """
+    generate a report based on either some matched data, or harmonics. In the latter case, report data is reconstructed.
+
+    :param MatchedMarkerVolume: pandas dataframe containing  ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl']
+        You must enter one of MatchedMarkerVolume or gradient_harmonics
+    :type MatchedMarkerVolume: pandas.DataFrame, optional
+    :param gradient_harmonics: list of either three pandas series or three paths to csv files
+        from SphericalHarmonicFit.
+        List elements should correspond to [G_x_harmonics, G_y_harmonics, G_z_harmonics].
+        You must enter one of MatchedMarkerVolume or gradient_harmonics
+    :type gradient_harmonics: list, optional
+    :param B0_harmonics: pandas series from SphericalHarmonicFit or path to saved csv file. If entered, is used
+        to report and plot B0 homogeneity
+    :type B0_harmonics: pandas.Series or path, optional
+    :param recon_coords: The coordinates you want to calculate the fields at. a pandas Dataframe which can contain
+        whatever you want, but MUST contain columns called: x, y, z. If left as None a default is generated.
+    :type recon_coords: pandas.DataFrame, optional
+    :param tests_to_run: a class containing any tests to run. The class in this instance serves only as a name
+        space. All methods inside the class starting with 'test' are identified as tests. The test methods will
+        have access to everything inside this class.
+    :type tests_to_run: class, optional
+    :param dicom_data: either a dictionary or path to a saved json file of the dicom_data object generated by
+        MarkerVolume. This data is required for harmonic reconstruction. For MatchedMarkerVolume it is not required,
+        but it does contain useful information about the acquisition so still a good idea to use it.
+    :type dicom_data: dict or path to json, optional
+    :param r_outer: for the harmonic approach, r_outer is used to determine where the data is reconstructed. It is
+        also used to control the limits in which data is plotted
+    :type r_outer: float, optional
+    :param show_plots: if True, all plots will be shown in your browser. Otherwise they are only saved
+    :type show_plots: bool, optional
+    :param style: control the report style. At the moment can only be 'light' or 'dark'
+    :type style: str
+    """
+
+    def __init__(self, MatchedMarkerVolume=None, gradient_harmonics=None, B0_harmonics=None,
+                 recon_coords_cartesian=None, tests_to_run=DefaultTestSuite, dicom_data=None,
+                 r_outer=None, show_plots=False, style='dark'):
+
+        self._html_template_loc = Path(__file__).parent.resolve() / 'jinja_templates' / 'MR_report.html'
+        self._show_plots = show_plots
+        _available_plotly_themes = ["plotly", "plotly_white", "plotly_dark", "ggplot2",
+                                    "seaborn", "simple_white", "none"]
+        self._style = style
+        self._set_styles()
+        self._jinja_dict = {}  # this will hold all the info jinja needs to render
+        self._test_class = tests_to_run
+        self.r_outer = r_outer
+        self.recon_coords_cartesian = recon_coords_cartesian
+        self.dicom_data = get_dicom_data(dicom_data)
+        self._build_acquisition_dict()
+        self._get_analysis_data(MatchedMarkerVolume, gradient_harmonics, B0_harmonics)
+        self._update_MatchedMarkerVolume()
+
+        # put plots here
+        self._plot_distortion_v_r()
+        self._plot_3D_cutplanes()
+        self._plot_B0_surface()
+        self._build_homogeneity_report_table()
+        # self._plot_gradients_surface()
+        self._get_test_results()
+
+    def _build_acquisition_dict(self):
+        """
+        will try and extract acquisition data from dicom_data, and put it in a new dictionary
+        if this new dictionary exists, we will include the acquisition data in the report
+        """
+        if self.dicom_data is None:
+            return
+        self._jinja_dict['acquisition_data'] = {}
+        _fields_of_interest = ['acquisition_date', 'magnetic_field_strength', 'bandwidth', 'pixel_spacing',
+                               'freq_encode_direction', 'manufacturer', 'imaging_frequency']
+        for key in self.dicom_data:
+            if key in _fields_of_interest:
+                new_key = key.replace('_', ' ')
+                self._jinja_dict['acquisition_data'][new_key] = self.dicom_data[key]
+
+    def _set_styles(self):
+        """
+        sets the report style by changing the plotly theme and chanding the html css file
+        """
+        if self._style == 'dark':
+            self._plotly_theme = 'plotly_dark'
+            self._html_theme = "themes/d42ker-github.css"
+        elif self._style == 'light':
+            self._plotly_theme = 'plotly_white'
+            self._html_theme = "themes/whitey.css"
+        else:
+            raise AttributeError(f'unknown style entered: {self._style}. allowed options are "light" or "dark"')
+
+    def _unique_name_generator(self, save_loc, input_name, rel_path=True):
+        """
+        take input name, append the current date to it
+        then check if this new name already exists in save_loc; if it does add integers to it (_1, _2, etc.) until it doesn't
+        """
+        if not save_loc.is_dir():
+            # in this case, the code will likely fail downstream but we don't have to do anything here
+            return input_name
+        input_name, extension = os.path.splitext(input_name)
+        now = datetime.now()  # current date and time
+        date_string = now.strftime("%d_%m_%Y")
+        new_name = input_name + '_' + date_string
+        appended_int = 0
+        while (save_loc / (new_name + extension)).is_file():
+            appended_int = appended_int + 1
+            new_name = new_name + '_' + str(appended_int)
+        new_name = new_name + extension
+        if rel_path:
+            new_name = (save_loc  / new_name).relative_to(save_loc.parent)
+        else:
+            new_name = save_loc / new_name
+        return new_name
+
+    def _get_test_results(self):
+        """
+        runs through all tests found in the _test_class and keeps all the results in _jinja_dict
+        """
+
+        self._jinja_dict['test_collection'] = {}
+        self._jinja_dict['TestSuiteName'] = self._test_class.__name__
+        method_list = [method for method in dir(self._test_class) if method.startswith('__') is False]
+        # this will list all methods except 'dunder' methods e.g. __init__
+        for test in method_list:
+            if test[:4] == 'test':
+                # then we found a true test
+                test_name = test.replace('_', ' ') # under scores to space
+                test_name = test_name.replace('test ','' )  # remove test from the name
+                test_string = getattr(self._test_class, test)(self)
+                if isinstance(test_string, bool):
+                    if test_string:
+                        test_string = "<span style='color:green'>Pass</span>"
+                    else:
+                        test_string = "<span style='color:red'>Fail</span>"
+                elif not isinstance(test_string, str):
+                    raise TypeError('please return test results as either booleans or strings')
+                self._jinja_dict['test_collection'][test_name] = test_string
+
+    def _get_analysis_data(self, MatchedMarkerVolume, gradient_harmonics, B0_harmonics):
+        """
+        check what the user has input, and attach to self
+        if necessary, convert gradient_harmonics to distortion map
+        """
+
+        if MatchedMarkerVolume is not None and gradient_harmonics is not None:
+            raise AttributeError(
+                f'you cannot enter both MatchedMarkerVolume and gradient_harmonics at the same time...')
+
+        if MatchedMarkerVolume is not None:
+            self._check_marker_volume(MatchedMarkerVolume)
+            self._MatchedMarkerVolume = MatchedMarkerVolume.copy()
+
+        if gradient_harmonics is not None:
+            self._check_dicom_data()
+            self._Gx_Harmonics, self._Gy_Harmonics, self._Gz_Harmonics = \
+                get_gradient_spherical_harmonics(gradient_harmonics[0], gradient_harmonics[1], gradient_harmonics[2])
+            self._Gx_Harmonics = self._Gx_Harmonics * self.dicom_data['gradient_strength'][0]
+            self._Gy_Harmonics = self._Gy_Harmonics * self.dicom_data['gradient_strength'][1]
+            self._Gz_Harmonics = self._Gz_Harmonics * self.dicom_data['gradient_strength'][2]
+            if self.r_outer is None:
+                logger.warning('no r_outer value entered, using 150 mm')
+                self.r_outer = 150
+            if self.recon_coords_cartesian is None:
+                self.recon_coords_cartesian = self._generate_recon_coords()
+            self.recon_coords = convert_cartesian_to_spherical(self.recon_coords_cartesian)
+            self._reconstruct_gradient_fields()
+            self._convert_magnetic_field_to_distortion()
+
+        if B0_harmonics is not None:
+            if isinstance(B0_harmonics, pd.Series):
+                self.B0_harmonics = B0_harmonics
+            elif isinstance(B0_harmonics, (str, Path)):
+                self.B0_harmonics = pd.read_csv(B0_harmonics, index_col=0).squeeze("columns")
+            else:
+                raise AttributeError('could not read in B0_harmonics...please input either a series or a '
+                                     'path to a saved csv file')
+        else:
+            self.B0_harmonics = None
+
+    def _convert_magnetic_field_to_distortion(self):
+        """
+        converts reconstructed gradient fields into geometric distortion.
+        Essentially this process is doing the opposite of FieldCalculation.ConvertMatchedMarkersToBz
+        """
+        self._MatchedMarkerVolume = pd.DataFrame()
+        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(x_gt=self.recon_coords_cartesian.x)
+        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(y_gt=self.recon_coords_cartesian.y)
+        self._MatchedMarkerVolume = self._MatchedMarkerVolume.assign(z_gt=self.recon_coords_cartesian.z)
+        bandwidth = np.array(self.dicom_data['bandwidth'])
+        image_size = np.array(self.dicom_data['image_size'])
+        gama = np.array(self.dicom_data['gama'])
+        FOV = np.array(self.dicom_data['FOV'])
+
+        gradient_strength = bandwidth * image_size / (gama * 1e6 * FOV * 1e-3)  # unit(T / m)
+        # ^ this is a vector [gx, gy, gz]
+        self._MatchedMarkerVolume = \
+            self._MatchedMarkerVolume.assign(x_gnl=self.Gx_Bfield / (gradient_strength[0]))
+        self._MatchedMarkerVolume = \
+            self._MatchedMarkerVolume.assign(y_gnl=self.Gy_Bfield / (gradient_strength[1]))
+        self._MatchedMarkerVolume = \
+            self._MatchedMarkerVolume.assign(z_gnl=self.Gz_Bfield / (gradient_strength[2]))
+
+    def _reconstruct_gradient_fields(self):
+        """
+        utilise the utilities.reconstruct_Bz function to reconsutrct each of the gradient fields at recon_coords
+        """
+        self.Gx_Bfield = reconstruct_Bz(self._Gx_Harmonics, self.recon_coords, quantity='T')
+        self.Gy_Bfield = reconstruct_Bz(self._Gy_Harmonics, self.recon_coords, quantity='T')
+        self.Gz_Bfield = reconstruct_Bz(self._Gz_Harmonics, self.recon_coords, quantity='T')
+
+    def _build_homogeneity_report_table(self):
+        """
+        Generate a table of predicted pk-pk homogeneity at different r
+        :return:
+        """
+        if self.B0_harmonics is None:
+            return
+        radii_of_interest = [50, 100, 150, 200]
+        pk_pk = []
+        for DSV_radius in radii_of_interest:
+            azimuth = np.linspace(0, 2 * np.pi, 100)
+            elevation = np.linspace(0, np.pi, 100)
+            [AZ, EL, R] = np.meshgrid(azimuth, elevation, DSV_radius, indexing='ij')
+            surface_coords = pd.DataFrame({'r': R.flatten(), 'azimuth': AZ.flatten(), 'elevation': EL.flatten()})
+            surface_coords = convert_spherical_to_cartesian(surface_coords)
+            B0 = reconstruct_Bz(self.B0_harmonics, surface_coords, quantity='T', r_outer=DSV_radius)
+            pk_pk.append(int((B0.max() - B0.min()) * 1e6))
+        _B0_stats = pd.DataFrame({'r': radii_of_interest, 'pk_pk [\u03BCT]': pk_pk} )
+
+        self._B0_table = go.Figure(data=[go.Table(
+            header=dict(values=list(_B0_stats.columns),
+                        align='left'),
+            cells=dict(values=[_B0_stats.r, _B0_stats['pk_pk [\u03BCT]']],
+                       align='left'))
+        ])
+        self._B0_table.update_layout(template=self._plotly_theme)
+
+    def _check_dicom_data(self):
+        """
+        check that if input dicom data is required, it confirms to minimum standard
+        """
+        _required_fields = ['FOV', 'bandwidth', 'gama', 'image_size', 'gradient_strength']
+
+        if not isinstance(self.dicom_data, dict) or not all(
+                name in self.dicom_data.keys() for name in _required_fields):
+            raise AttributeError(f'dicom_data must be a dict with at least the following keys: {_required_fields}')
+
+    def _check_marker_volume(self, MatchedMarkerVolume):
+        """
+        check that if a MatchedMarkerVolume is entered, is meets expected format
+        """
+        _required_cols = ['x_gt', 'y_gt', 'z_gt', 'x_gnl', 'y_gnl', 'z_gnl']
+        if not isinstance(MatchedMarkerVolume, pd.DataFrame) or \
+                not all(name in MatchedMarkerVolume.columns for name in _required_cols):
+            raise AttributeError(f'MatchedMarkerVolume must be a dataframe containing columns'
+                                 f'[x_gt, y_gt, z_gt, x_gnl, y_gnl, z_gnl]')
+
+    def _generate_recon_coords(self):
+        """
+        Generate a grid of coordinates to perform reconstruction
+        """
+        x = np.linspace(-self.r_outer, self.r_outer, 50)
+        y = np.linspace(-self.r_outer, self.r_outer, 50)
+        z = np.linspace(-self.r_outer, self.r_outer, 50)
+        [x_recon, y_recon, z_recon] = np.meshgrid(x, y, z, indexing='ij')
+        recon_coords = pd.DataFrame({'x': x_recon.flatten(), 'y': y_recon.flatten(), 'z': z_recon.flatten()})
+        return recon_coords
+
+    def _plot_distortion_v_r(self):
+        """
+        generate a histogram as a function of r
+        """
+
+        # data over different planes
+        xy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, z_select=0)
+        xy_plot_data['plane'] = 'XY'
+        zx_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, y_select=0)
+        zx_plot_data['plane'] = 'ZX'
+        zy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, x_select=0)
+        zy_plot_data['plane'] = 'ZY'
+        # create a new data frame combined from these for easy plotting
+        all_dsv_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer)
+        all_dsv_plot_data['plane'] = 'Entire DSV'
+
+
+        plot_data = pd.concat([all_dsv_plot_data, xy_plot_data, zx_plot_data, zy_plot_data], ignore_index=True, axis=0)
+        self._fig_distortion_v_r = px.scatter(plot_data, x="r_gt", y="abs_dis",color="plane",
+                                              labels={
+                                                  "r_gt": "Distance from the center (mm)", #rename the x axis
+                                                  "abs_dis": " Absolute Distortion (mm)", #rename the y axis
+                                              },
+                                              title=f"Cardinal plane data, {self.r_outer} DSV")
+
+
+        self._fig_distortion_v_r.update_layout(template=self._plotly_theme)
+        if self._show_plots:
+            self._fig_distortion_v_r.show()
+
+    def _plot_3D_cutplanes(self):
+        """
+        create a 3D cone plot in each of the three cardinal directions
+        """
+        xy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, z_select=0)
+        zx_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, y_select=0)
+        zy_plot_data = self._extract_data_from_MatchedMarkerVolume(r_max=self.r_outer, x_select=0)
+        plot_data = pd.concat([xy_plot_data, zx_plot_data, zy_plot_data], ignore_index=True, axis=0)
+
+        self._fig_3D_planes = go.Figure(data=go.Cone(
+            x=plot_data['x_gt'],
+            y=plot_data['y_gt'],
+            z=plot_data['z_gt'],
+            u=plot_data['x_dis'],
+            v=plot_data['y_dis'],
+            w=plot_data['z_dis'],
+
+            colorbar=dict(title= 'mm'),
+
+            sizemode="absolute",
+            sizeref=40))
+
+
+        self._fig_3D_planes.update_layout(scene=dict(aspectratio=dict(x=1, y=1, z=0.8),
+                                                     camera_eye=dict(x=1.2, y=1.2, z=0.6)))
+        self._fig_3D_planes.update_layout(template=self._plotly_theme, scene = dict(
+                    xaxis_title='X Axis (mm)',
+                    yaxis_title='Y Axis (mm)',
+                    zaxis_title='Z Axis (mm)'))
+        if self._show_plots:
+            self._fig_3D_planes.show()
+
+    def _plot_B0_surface(self):
+        """
+        if self.B0_harmonics exists, reconstruct B0 on the surface of r_outer and make a pretty 3D plot
+        """
+
+        if self.B0_harmonics is None:
+            return
+        # generate surface recon coordinates
+        if self.r_outer is not None:
+            r = self.r_outer
+        else:
+            r = 150
+        azimuth = np.linspace(0, 2 * np.pi, 100)
+        elevation = np.linspace(0, np.pi, 100)
+        [AZ, EL, R] = np.meshgrid(azimuth, elevation, r, indexing='ij')
+        surface_coords = pd.DataFrame({'r': R.flatten(), 'azimuth': AZ.flatten(), 'elevation': EL.flatten()})
+        surface_coords = convert_spherical_to_cartesian(surface_coords)
+
+        B0 = reconstruct_Bz(self.B0_harmonics, surface_coords, quantity='uT', r_outer=r)
+        x = surface_coords.x.to_numpy().reshape(100, 100)
+        y = surface_coords.y.to_numpy().reshape(100, 100)
+        z = surface_coords.z.to_numpy().reshape(100, 100)
+        B0 = B0.to_numpy().reshape(100, 100)
+
+        self._fig_DSV_surface = go.Figure(data=[go.Surface(z=z, x=x, y=y,colorbar=dict(title= 'B(uT)'), surfacecolor=B0)])
+
+        self._fig_DSV_surface.update_layout(title='DSV surface [uT]', autosize=True,
+                          template=self._plotly_theme, scene = dict(
+                    xaxis_title='X Axis (mm)',
+                    yaxis_title='Y Axis (mm)',
+                    zaxis_title='Z Axis (mm)') )
+
+        if self._show_plots:
+            self._fig_DSV_surface.show()
+
+    def _update_MatchedMarkerVolume(self):
+        """
+        adds in 'r_gt', 'r_gnl' and 'dis_x,y,z' to _MatchedMarkerVolume input
+        """
+        self._MatchedMarkerVolume['r_gt'] = np.sqrt(self._MatchedMarkerVolume.x_gt ** 2
+                                                    + self._MatchedMarkerVolume.y_gt ** 2
+                                                    + self._MatchedMarkerVolume.z_gt ** 2)
+        self._MatchedMarkerVolume['r_gnl'] = np.sqrt(self._MatchedMarkerVolume.x_gnl ** 2
+                                                     + self._MatchedMarkerVolume.y_gnl ** 2
+                                                     + self._MatchedMarkerVolume.z_gnl ** 2)
+        self._MatchedMarkerVolume['x_dis'] = self._MatchedMarkerVolume.x_gnl - self._MatchedMarkerVolume.x_gt
+        self._MatchedMarkerVolume['y_dis'] = self._MatchedMarkerVolume.y_gnl - self._MatchedMarkerVolume.y_gt
+        self._MatchedMarkerVolume['z_dis'] = self._MatchedMarkerVolume.z_gnl - self._MatchedMarkerVolume.z_gt
+        self._MatchedMarkerVolume['abs_dis'] = np.sqrt(self._MatchedMarkerVolume.x_dis ** 2
+                                                       + self._MatchedMarkerVolume.y_dis ** 2
+                                                       + self._MatchedMarkerVolume.z_dis ** 2)
+        # get resolution in each direction
+        self._x_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.x_gt.unique())))
+        self._y_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.y_gt.unique())))
+        self._z_res = np.mean(np.diff(np.sort(self._MatchedMarkerVolume.z_gt.unique())))
+
+    def _extract_data_from_MatchedMarkerVolume(self, x_select=None, y_select=None, z_select=None,
+                                               max_num_points=None, r_max=None):
+        """
+        Extract data from the matched volume for use in direct plotting
+
+        uses the values of _x_res etc. to define a tolerance
+        """
+        if (x_select is None) and (y_select is None) and (z_select is None) and (r_max is None):
+            logger.warning('you should set a value for at least one of x_ind, y_ind, and z_ind or r_max')
+        # start with everything selected, overwrite below
+        x_ind = np.ones(self._MatchedMarkerVolume.shape[0])
+        y_ind = np.ones(self._MatchedMarkerVolume.shape[0])
+        z_ind = np.ones(self._MatchedMarkerVolume.shape[0])
+        r_ind = np.ones(self._MatchedMarkerVolume.shape[0])
+
+        if x_select is not None:
+            x_ind = np.logical_and(self._MatchedMarkerVolume.x_gt <= (x_select + self._x_res / 2),
+                                   self._MatchedMarkerVolume.x_gt >= (x_select - self._x_res / 2))
+        if y_select is not None:
+            y_ind = np.logical_and(self._MatchedMarkerVolume.y_gt <= (y_select + self._y_res / 2),
+                                   self._MatchedMarkerVolume.y_gt >= (y_select - self._y_res / 2))
+        if z_select is not None:
+            z_ind = np.logical_and(self._MatchedMarkerVolume.z_gt <= (z_select + self._z_res / 2),
+                                   self._MatchedMarkerVolume.z_gt >= (z_select - self._z_res / 2))
+        if r_max is not None:
+            r_ind = self._MatchedMarkerVolume.r_gt <= r_max
+
+        select_ind = np.logical_and(np.logical_and(x_ind, y_ind), z_ind)
+        select_ind = np.logical_and(select_ind, r_ind)
+        plot_data = self._MatchedMarkerVolume[select_ind]
+        plot_data = plot_data.reset_index(drop=True)
+        if (max_num_points is not None) and plot_data.shape[0] > max_num_points:
+            every_nth_point = int(plot_data.shape[0] / max_num_points)
+            plot_data = plot_data[plot_data.reset_index().index % every_nth_point == 0]
+
+        return plot_data
+
+    def _set_up_directory_structure(self):
+        """
+        ensure we have a place to save the reports.
+        will set up a directory in
+        """
+        if not os.path.isdir(self.output_folder):
+            os.makedirs(self.output_folder)
+        if not os.path.isdir(self.output_folder / 'plots'):
+            os.mkdir(self.output_folder / 'plots')
+
+        # copy themes
+        theme_dir = (Path(__file__).parent / 'jinja_templates' / 'themes').resolve()
+        copy_tree(str(theme_dir), str(self.output_folder / 'themes'))
+
+    def _get_template(self):
+        """
+        loads the jinja template
+        """
+
+        with open(self._html_template_loc) as f:
+            template_text = f.read()
+        j2_template = Template(template_text)
+        return j2_template
+
+    # public methods
+
+    def write_html_report(self, output_folder=None):
+        """
+        Generates a html report encompassing available acquisition information, test results, and intercative
+        plotly figures
+
+        :param output_folder: folder to write report. Defaults to ~/Documents/MR_QA_Reports
+        :type output_folder: Path or string, optional
+        """
+        if output_folder is None:
+            self.output_folder = Path(os.path.expanduser('~')) / 'Documents' / 'MR_QA_Reports'
+        else:
+            self.output_folder = Path(output_folder)
+        self._set_up_directory_structure()
+
+        # save plots and update jinja_dict
+
+        distortion_v_r_save_name = self._unique_name_generator(self.output_folder / 'plots', 'distortion_v_r.html')
+        self._fig_distortion_v_r.write_html(self.output_folder / distortion_v_r_save_name, full_html=False, include_plotlyjs='cdn')
+        self._jinja_dict['dist_v_r_source'] = distortion_v_r_save_name
+
+        threeD_plane_save_name = self._unique_name_generator(self.output_folder / 'plots', '3D_planes.html')
+        self._fig_3D_planes.write_html(self.output_folder / threeD_plane_save_name, full_html=False, include_plotlyjs='cdn')
+        self._jinja_dict['cutplanes_source'] = threeD_plane_save_name
+
+        if self.B0_harmonics is not None:
+            DSV_surface_save_name = self._unique_name_generator(self.output_folder / 'plots', 'DSV_surface.html',)
+            self._fig_DSV_surface.write_html(self.output_folder / DSV_surface_save_name, full_html=False, include_plotlyjs='cdn')
+            self._jinja_dict['dsv_surf_source'] = DSV_surface_save_name
+
+            B0_table_save_name = self._unique_name_generator(self.output_folder / 'plots', 'B0_table.html')
+            self._B0_table.write_html(self.output_folder / B0_table_save_name, full_html=False, include_plotlyjs='cdn')
+            self._jinja_dict['B0_table_source'] = B0_table_save_name
+        else:
+            self._jinja_dict['dsv_surf_source'] = None
+
+        # set up template
+        self._jinja_dict['html_theme_loc'] = self._html_theme
+        j2_template = self._get_template()
+        report_name = self._unique_name_generator(self.output_folder, 'MR_QA_report.html', rel_path=False)
+        report_code = os.path.split(report_name)[1]  # for printing
+        report_code = os.path.splitext(report_code)[0]
+        report_code = report_code.replace('MR_QA_report_','')
+        self._jinja_dict['report_name'] = report_code
+        report_string = j2_template.render(self._jinja_dict)
+        with open(report_name, 'w') as f:
+            f.write(report_string)
+
+        print('The report has been compiled and can be found in the MR_QA_Reports folder') #let the user know where to find the finished report
+
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/calculate_harmonics.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/calculate_harmonics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,57 @@
-from .Harmonics import SphericalHarmonicFit
-import numpy as np
-
-def calculate_harmonics(MagneticFields, n_order=5, scale=None):
-    """
-    This function is essentially a wrapper of convenience. Given a set of B fields and dicom_data,
-    it will calculate and return the Gx, Gy, and Gz harmonics.
-
-    :param MagneticFields: a pandas dataframe with columns ['x', 'y', 'z', 'B_Gx', 'B_Gy', 'B_Gz', 'B0']. B0 is optional.
-        x, y, z are in mm and the fields are in any unit - the harmonics will reflect the units
-    :type MagneticFields: pandas dataframe
-    :param n_order: order of harmonic fit
-    :type n_order: int or list, optional
-    :param scale: Can pass a list of four values, the four returned harmonic lists will be scalealised accordingly.
-        e.g. scale = [2,2,2,2] will multiply all harmonics by 2. This is useful to normalise the fields to some
-        value
-    :return: G_x_Harmonics, G_y_Harmonics, G_z_Harmonics, B0_Harmonics
-    """
-
-    if scale is None:
-        scale = [1, 1, 1, 1]
-    if not np.shape(scale)[0] == 4:
-        raise ValueError('scale must be a list such as [2,2,2,2], where the elements correspond to Gx, Gy, Gz, and B0')
-
-    if isinstance(n_order, int):
-        n_order = [n_order, n_order, n_order, n_order]
-    elif not len(n_order) == 4:
-        raise ValueError('n_order must either be a single integer or a list of 4 integers corresponding to'
-                         '[n_order_Gx,n_order_Gy,n_order_Gz,n_order_B0]')
-
-    # calculate harmonics
-    # Gx
-    GradXdata = MagneticFields[['x', 'y', 'z', 'B_Gx']]
-    GradXdata = GradXdata.rename(
-        columns={"B_Gx": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
-    G_x_Harmonics = SphericalHarmonicFit(GradXdata, n_order=n_order[0], r_outer=150, scale=scale[0])
-
-    # Gy
-    GradYdata = MagneticFields[['x', 'y', 'z', 'B_Gy']]
-    GradYdata = GradYdata.rename(
-        columns={"B_Gy": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
-    G_y_Harmonics = SphericalHarmonicFit(GradYdata, n_order=n_order[1], r_outer=150, scale=scale[1])
-
-    # G_z
-    GradZdata = MagneticFields[['x', 'y', 'z', 'B_Gz']]
-    GradZdata = GradZdata.rename(
-        columns={"B_Gz": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
-    G_z_Harmonics = SphericalHarmonicFit(GradZdata, n_order=n_order[2], r_outer=150, scale=scale[2])
-
-    # B0
-    try:
-        B0_data = MagneticFields[['x', 'y', 'z', 'B0']]
-        B0_data = B0_data.rename(
-            columns={"B0": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
-        B0_Harmonics = SphericalHarmonicFit(B0_data, n_order=n_order[3], r_outer=150, scale=scale[3])
-    except KeyError:
-        B0_Harmonics = None
-
-    return G_x_Harmonics, G_y_Harmonics, G_z_Harmonics, B0_Harmonics
+from .Harmonics import SphericalHarmonicFit
+import numpy as np
+
+def calculate_harmonics(MagneticFields, n_order=8, norm=None):
+    """
+    This function is essentially a wrapper of convenience. Given a set of B fields and dicom_data,
+    it will calculate and return the Gx, Gy, and Gz harmonics.
+    Note that the gradient harmonics will be normalised to a gradient strengt of 1 mT/m
+
+    :param MagneticFields: a pandas dataframe with columns ['x', 'y', 'z', 'B_Gx', 'B_Gy', 'B_Gz', 'B0']. B0 is optional.
+        x, y, z are in mm and the fields are in any unit - the harmonics will reflect the units
+    :type MagneticFields: pandas dataframe
+    :param dicom_data: a dict containing required dicom data, such as that generated within the MarkerVolume class
+    :type dicom_data: dict
+    :param n_order: order of harmonic fit
+    :type n_order: int, optional
+    :param norm: Can pass a list of four valuues, the four returned harmonic lists will be normalised accordingly.
+        e.g. norm = [2,2,2,2] will divide all harmonics by 2. This is useful so you can normalise the fields to some
+        value
+    :return: G_x_Harmonics, G_y_Harmonics, G_z_Harmonics, B0_Harmonics
+    """
+
+    if norm is None:
+        norm = [1, 1, 1, 1]
+    if not np.shape(norm)[0] == 4:
+        raise ValueError('norm must be a list such as [2,2,2,2], where the elements correspond to Gx, Gy, Gz, and B0')
+
+    # calculate harmonics
+
+    # Gx
+    GradXdata = MagneticFields[['x', 'y', 'z', 'B_Gx']]
+    GradXdata = GradXdata.rename(
+        columns={"B_Gx": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
+    G_x_Harmonics = SphericalHarmonicFit(GradXdata, n_order=n_order, r_outer=150, scale=norm[0])
+
+    # Gy
+    GradYdata = MagneticFields[['x', 'y', 'z', 'B_Gy']]
+    GradYdata = GradYdata.rename(
+        columns={"B_Gy": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
+    G_y_Harmonics = SphericalHarmonicFit(GradYdata, n_order=n_order, r_outer=150, scale=norm[1])
+
+    # G_z
+    GradZdata = MagneticFields[['x', 'y', 'z', 'B_Gz']]
+    GradZdata = GradZdata.rename(
+        columns={"B_Gz": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
+    G_z_Harmonics = SphericalHarmonicFit(GradZdata, n_order=n_order, r_outer=150, scale=norm[2])
+
+    # B0
+    try:
+        B0_data = MagneticFields[['x', 'y', 'z', 'B0']]
+        B0_data = B0_data.rename(
+            columns={"B0": "Bz"})  # spherical harmonics code expects to receieve one field called Bz
+        B0_Harmonics = SphericalHarmonicFit(B0_data, n_order=n_order, r_outer=150, scale=norm[3])
+    except KeyError:
+        B0_Harmonics = None
+
+    return G_x_Harmonics, G_y_Harmonics, G_z_Harmonics, B0_Harmonics
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/MR_report.html` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/MR_report.html`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-<!doctype html>
-<html>
-<head>
-<meta charset='UTF-8'><meta name='viewport' content='width=device-width initial-scale=1'>
-<title>MR_report:</title>
-</head>
-<link rel="stylesheet" type="text/css" rel="noopener" target="_blank" href={{ html_theme_loc }}>
-<body><h1 id='mr-qa-report'>MR QA report {{ report_name }}</h1>
-
-{% if acquisition_data -%}
-    <h2 id='acquisition_data'>Acquisition Data</h2>
-      <table>
-      {% for key in acquisition_data %}
-         <TR>
-            <TD class="c1">{{key}}</TD>
-            <TD class="c2">{{acquisition_data[key]}}</TD>
-         </TR>
-   {% endfor %}
-      </table>
-{% else -%}
-   <!--None-->
-{%endif %}
-<h2 id='tests'>Tests from: {{ TestSuiteName }}</h2>
-<table>
-<TD class="c1"><strong>Test Name</strong></TD>
-<TD class="c2"><strong>Result</strong></TD>
-{% for item in test_collection %}
-<TR>
-   <TD class="c1">{{item}}</TD>
-   <TD class="c2">{{test_collection[item]}}</TD>
-</TR>
-{% endfor %}
-</table>
-
-   <div></iframe>
-      <h2 id='distortion versus r'><span>Distortion versus r</span></h2><iframe width="85%," height="650,"
-         src={{ dist_v_r_source }}  style="border:none;"></iframe>
-   </div>
-   <div></iframe>
-      <h2 id='3d-cut-planes'><span>3D cut planes</span></h2><iframe width="85%," height="700,"
-         src={{ cutplanes_source }} style="border:none;"></iframe>
-   </div>
-
-{% if dsv_surf_source -%}
-    <div>
-      <div align="left"></iframe>
-         <h2 id='B0 surface'><span>B0 surface</span></h2><iframe width="50%," height="700,"
-            src={{ dsv_surf_source }} l style="border:none;" </iframe>
-      </div>
-      <div align="right"></iframe>
-         <iframe width="400," height="700," src= {{ B0_table_source }}
-            style="border:none;" </iframe>
-      </div>
-   </div>d-cut-planes'><span>3D cut planes</span></h2><iframe width="85%," height="700," src={{ cutplanes_source }} style="border:none;"></iframe></div>
-{% endif %}
-
-</body>
+<!doctype html>
+<html>
+<head>
+<meta charset='UTF-8'><meta name='viewport' content='width=device-width initial-scale=1'>
+<title>MR_report:</title>
+</head>
+<link rel="stylesheet" type="text/css" rel="noopener" target="_blank" href={{ html_theme_loc }}>
+<body><h1 id='mr-qa-report'>MR QA report {{ report_name }}</h1>
+
+{% if acquisition_data -%}
+    <h2 id='acquisition_data'>Acquisition Data</h2>
+      <table>
+      {% for key in acquisition_data %}
+         <TR>
+            <TD class="c1">{{key}}</TD>
+            <TD class="c2">{{acquisition_data[key]}}</TD>
+         </TR>
+   {% endfor %}
+      </table>
+{% else -%}
+   <!--None-->
+{%endif %}
+<h2 id='tests'>Tests from: {{ TestSuiteName }}</h2>
+<table>
+<TD class="c1"><strong>Test Name</strong></TD>
+<TD class="c2"><strong>Result</strong></TD>
+{% for item in test_collection %}
+<TR>
+   <TD class="c1">{{item}}</TD>
+   <TD class="c2">{{test_collection[item]}}</TD>
+</TR>
+{% endfor %}
+</table>
+
+   <div></iframe>
+      <h2 id='distortion versus r'><span>Distortion versus r</span></h2><iframe width="85%," height="650,"
+         src={{ dist_v_r_source }}  style="border:none;"></iframe>
+   </div>
+   <div></iframe>
+      <h2 id='3d-cut-planes'><span>3D cut planes</span></h2><iframe width="85%," height="700,"
+         src={{ cutplanes_source }} style="border:none;"></iframe>
+   </div>
+
+{% if dsv_surf_source -%}
+    <div>
+      <div align="left"></iframe>
+         <h2 id='B0 surface'><span>B0 surface</span></h2><iframe width="50%," height="700,"
+            src={{ dsv_surf_source }} l style="border:none;" </iframe>
+      </div>
+      <div align="right"></iframe>
+         <iframe width="400," height="700," src= {{ B0_table_source }}
+            style="border:none;" </iframe>
+      </div>
+   </div>d-cut-planes'><span>3D cut planes</span></h2><iframe width="85%," height="700," src={{ cutplanes_source }} style="border:none;"></iframe></div>
+{% endif %}
+
+</body>
 </html>
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/jinja_templates/themes/whitey.css` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/jinja_templates/themes/whitey.css`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,267 +1,267 @@
-html {
-	font-size: 19px;
-}
-
-html, body {
-	margin: auto;
-	background: #fefefe;
-}
-body {
-	font-family: "Vollkorn", Palatino, Times;
-	color: #333;
-	line-height: 1.4;
-	text-align: justify;
-}
-#write {
-	max-width: 960px;
-	margin: 0 auto;
-	margin-bottom: 2em;
-	line-height: 1.53;
-}
-
-#write>h2:first-child,
-#write>h3:first-child,
-#write>h4:first-child,
-#write>p:first-child{
-	margin-top: 1.2em;
-}
-
-/* Typography
--------------------------------------------------------- */
-
-#write>h1:first-child,
-h1 {
-	margin-top: 1.6em;
-	font-weight: normal;
-}
-
-h1 {
-	font-size:3em;
-}
-
-h2 {
-	margin-top:2em;
-	font-weight: normal;
-}
-
-h3 {
-	font-weight: normal;
-	font-style: italic;
-	margin-top: 3em;
-}
-
-h1, 
-h2, 
-h3{
-	text-align: center;
-}
-
-h2:after{
-	border-bottom: 1px solid #2f2f2f;
-    content: '';
-    width: 100px;
-    display: block;
-    margin: 0 auto;
-    height: 1px;
-}
-
-h1+h2, h2+h3 {
-	margin-top: 0.83em;
-}
-
-p,
-.mathjax-block {
-	margin-top: 0;
-	-webkit-hypens: auto;
-	-moz-hypens: auto;
-	hyphens: auto;
-}
-ul {
-	list-style: square;
-	padding-left: 1.2em;
-}
-ol {
-	padding-left: 1.2em;
-}
-blockquote {
-	margin-left: 1em;
-	padding-left: 1em;
-	border-left: 1px solid #ddd;
-}
-code,
-pre {
-	font-family: "Consolas", "Menlo", "Monaco", monospace, serif;
-	font-size: .9em;
-	background: white;
-}
-.md-fences{
-	margin-left: 1em;
-	padding-left: 1em;
-	border: 1px solid #ddd;
-	padding-bottom: 8px;
-	padding-top: 6px;
-	margin-bottom: 1.5em;
-}
-
-a {
-	color: #2484c1;
-	text-decoration: none;
-}
-a:hover {
-	text-decoration: underline;
-}
-a img {
-	border: none;
-}
-h1 a,
-h1 a:hover {
-	color: #333;
-	text-decoration: none;
-}
-hr {
-	color: #ddd;
-	height: 1px;
-	margin: 2em 0;
-	border-top: solid 1px #ddd;
-	border-bottom: none;
-	border-left: 0;
-	border-right: 0;
-}
-.md-table-edit {
-	background: #ededed;
-    padding-top: 4px;
-}
-table {
-	margin-bottom: 1.333333rem
-}
-table th,
-table td {
-	padding: 8px;
-	line-height: 1.333333rem;
-	vertical-align: top;
-	border-top: 1px solid #ddd
-}
-table th {
-	font-weight: bold
-}
-table thead th {
-	vertical-align: bottom
-}
-table caption+thead tr:first-child th,
-table caption+thead tr:first-child td,
-table colgroup+thead tr:first-child th,
-table colgroup+thead tr:first-child td,
-table thead:first-child tr:first-child th,
-table thead:first-child tr:first-child td {
-	border-top: 0
-}
-table tbody+tbody {
-	border-top: 2px solid #ddd
-}
-
-.task-list{
-	padding:0;
-}
-
-.task-list-item {
-	padding-left: 1.6rem;
-}
-
-.task-list-item input:before {
-	content: '\221A';
-	display: inline-block;
-	width: 1.33333333rem;
-  	height: 1.6rem;
-	vertical-align: middle;
-	text-align: center;
-	color: #ddd;
-	background-color: #fefefe;
-}
-
-.task-list-item input:checked:before,
-.task-list-item input[checked]:before{
-	color: inherit;
-}
-.md-tag {
-	color: inherit;
-	font: inherit;
-}
-#write pre.md-meta-block {
-	min-height: 35px;
-	padding: 0.5em 1em;
-}
-#write pre.md-meta-block {
-	white-space: pre;
-	background: #f8f8f8;
-	border: 0px;
-	color: #999;
-	
-	width: 100vw;
-	max-width: calc(100% + 60px);
-	margin-left: -30px;
-	border-left: 30px #f8f8f8 solid;
-	border-right: 30px #f8f8f8 solid;
-
-	margin-bottom: 2em;
-	margin-top: -1.3333333333333rem;
-	padding-top: 26px;
-	padding-bottom: 10px;
-	line-height: 1.8em;
-	font-size: 0.9em;
-	font-size: 0.76em;
-	padding-left: 0;
-}
-.md-img-error.md-image>.md-meta{
-	vertical-align: bottom;
-}
-#write>h5.md-focus:before {
-	top: 2px;
-}
-
-.md-toc {
-	margin-top: 40px;
-}
-
-.md-toc-content {
-	padding-bottom: 20px;
-}
-
-.outline-expander:before {
-	color: inherit;
-	font-size: 14px;
-	top: auto;
-	content: "\f0da";
-	font-family: FontAwesome;
-}
-
-.outline-expander:hover:before,
-.outline-item-open>.outline-item>.outline-expander:before {
-  	content: "\f0d7";
-}
-
-/** source code mode */
-#typora-source {
-	font-family: Courier, monospace;
-    color: #6A6A6A;
-}
-
-.html-for-mac #typora-sidebar {
-    -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
-    box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
-}
-
-.cm-s-typora-default .cm-header, 
-.cm-s-typora-default .cm-property,
-.CodeMirror.cm-s-typora-default div.CodeMirror-cursor {
-	color: #428bca;
-}
-
-.cm-s-typora-default .cm-atom, .cm-s-typora-default .cm-number {
-	color: #777777;
-}
-
-.typora-node .file-list-item-parent-loc, 
-.typora-node .file-list-item-time, 
-.typora-node .file-list-item-summary {
-	font-family: arial, sans-serif;
+html {
+	font-size: 19px;
+}
+
+html, body {
+	margin: auto;
+	background: #fefefe;
+}
+body {
+	font-family: "Vollkorn", Palatino, Times;
+	color: #333;
+	line-height: 1.4;
+	text-align: justify;
+}
+#write {
+	max-width: 960px;
+	margin: 0 auto;
+	margin-bottom: 2em;
+	line-height: 1.53;
+}
+
+#write>h2:first-child,
+#write>h3:first-child,
+#write>h4:first-child,
+#write>p:first-child{
+	margin-top: 1.2em;
+}
+
+/* Typography
+-------------------------------------------------------- */
+
+#write>h1:first-child,
+h1 {
+	margin-top: 1.6em;
+	font-weight: normal;
+}
+
+h1 {
+	font-size:3em;
+}
+
+h2 {
+	margin-top:2em;
+	font-weight: normal;
+}
+
+h3 {
+	font-weight: normal;
+	font-style: italic;
+	margin-top: 3em;
+}
+
+h1, 
+h2, 
+h3{
+	text-align: center;
+}
+
+h2:after{
+	border-bottom: 1px solid #2f2f2f;
+    content: '';
+    width: 100px;
+    display: block;
+    margin: 0 auto;
+    height: 1px;
+}
+
+h1+h2, h2+h3 {
+	margin-top: 0.83em;
+}
+
+p,
+.mathjax-block {
+	margin-top: 0;
+	-webkit-hypens: auto;
+	-moz-hypens: auto;
+	hyphens: auto;
+}
+ul {
+	list-style: square;
+	padding-left: 1.2em;
+}
+ol {
+	padding-left: 1.2em;
+}
+blockquote {
+	margin-left: 1em;
+	padding-left: 1em;
+	border-left: 1px solid #ddd;
+}
+code,
+pre {
+	font-family: "Consolas", "Menlo", "Monaco", monospace, serif;
+	font-size: .9em;
+	background: white;
+}
+.md-fences{
+	margin-left: 1em;
+	padding-left: 1em;
+	border: 1px solid #ddd;
+	padding-bottom: 8px;
+	padding-top: 6px;
+	margin-bottom: 1.5em;
+}
+
+a {
+	color: #2484c1;
+	text-decoration: none;
+}
+a:hover {
+	text-decoration: underline;
+}
+a img {
+	border: none;
+}
+h1 a,
+h1 a:hover {
+	color: #333;
+	text-decoration: none;
+}
+hr {
+	color: #ddd;
+	height: 1px;
+	margin: 2em 0;
+	border-top: solid 1px #ddd;
+	border-bottom: none;
+	border-left: 0;
+	border-right: 0;
+}
+.md-table-edit {
+	background: #ededed;
+    padding-top: 4px;
+}
+table {
+	margin-bottom: 1.333333rem
+}
+table th,
+table td {
+	padding: 8px;
+	line-height: 1.333333rem;
+	vertical-align: top;
+	border-top: 1px solid #ddd
+}
+table th {
+	font-weight: bold
+}
+table thead th {
+	vertical-align: bottom
+}
+table caption+thead tr:first-child th,
+table caption+thead tr:first-child td,
+table colgroup+thead tr:first-child th,
+table colgroup+thead tr:first-child td,
+table thead:first-child tr:first-child th,
+table thead:first-child tr:first-child td {
+	border-top: 0
+}
+table tbody+tbody {
+	border-top: 2px solid #ddd
+}
+
+.task-list{
+	padding:0;
+}
+
+.task-list-item {
+	padding-left: 1.6rem;
+}
+
+.task-list-item input:before {
+	content: '\221A';
+	display: inline-block;
+	width: 1.33333333rem;
+  	height: 1.6rem;
+	vertical-align: middle;
+	text-align: center;
+	color: #ddd;
+	background-color: #fefefe;
+}
+
+.task-list-item input:checked:before,
+.task-list-item input[checked]:before{
+	color: inherit;
+}
+.md-tag {
+	color: inherit;
+	font: inherit;
+}
+#write pre.md-meta-block {
+	min-height: 35px;
+	padding: 0.5em 1em;
+}
+#write pre.md-meta-block {
+	white-space: pre;
+	background: #f8f8f8;
+	border: 0px;
+	color: #999;
+	
+	width: 100vw;
+	max-width: calc(100% + 60px);
+	margin-left: -30px;
+	border-left: 30px #f8f8f8 solid;
+	border-right: 30px #f8f8f8 solid;
+
+	margin-bottom: 2em;
+	margin-top: -1.3333333333333rem;
+	padding-top: 26px;
+	padding-bottom: 10px;
+	line-height: 1.8em;
+	font-size: 0.9em;
+	font-size: 0.76em;
+	padding-left: 0;
+}
+.md-img-error.md-image>.md-meta{
+	vertical-align: bottom;
+}
+#write>h5.md-focus:before {
+	top: 2px;
+}
+
+.md-toc {
+	margin-top: 40px;
+}
+
+.md-toc-content {
+	padding-bottom: 20px;
+}
+
+.outline-expander:before {
+	color: inherit;
+	font-size: 14px;
+	top: auto;
+	content: "\f0da";
+	font-family: FontAwesome;
+}
+
+.outline-expander:hover:before,
+.outline-item-open>.outline-item>.outline-expander:before {
+  	content: "\f0d7";
+}
+
+/** source code mode */
+#typora-source {
+	font-family: Courier, monospace;
+    color: #6A6A6A;
+}
+
+.html-for-mac #typora-sidebar {
+    -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
+    box-shadow: 0 6px 12px rgba(0, 0, 0, .175);
+}
+
+.cm-s-typora-default .cm-header, 
+.cm-s-typora-default .cm-property,
+.CodeMirror.cm-s-typora-default div.CodeMirror-cursor {
+	color: #428bca;
+}
+
+.cm-s-typora-default .cm-atom, .cm-s-typora-default .cm-number {
+	color: #777777;
+}
+
+.typora-node .file-list-item-parent-loc, 
+.typora-node .file-list-item-time, 
+.typora-node .file-list-item-summary {
+	font-family: arial, sans-serif;
 }
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit/utilities.py` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit/utilities.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,879 +1,691 @@
-"""
-General purpose reusable functions
-"""
-
-import os
-import pathlib
-import sys
-import glob
-import logging
-from pathlib import Path
-import numpy as np
-from scipy.special import lpmv
-import pandas as pd
-from matplotlib import pyplot as plt
-import pydicom
-import json
-from itertools import compress
-import plotly.graph_objects as go
-import warnings
-
-ch = logging.StreamHandler()
-formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
-ch.setFormatter(formatter)
-logger = logging.getLogger(__name__)
-logger.addHandler(ch)
-logger.setLevel(logging.INFO)  # This toggles all the logging in your app
-logger.propagate = False
-
-
-class bcolors:
-    """
-    This is just here to enable me to print pretty colors to the linux terminal
-    """
-    HEADER = '\033[95m'
-    OKBLUE = '\033[94m'
-    OKCYAN = '\033[96m'
-    OKGREEN = '\033[92m'
-    WARNING = '\033[93m'
-    FAIL = '\033[91m'
-    ENDC = '\033[0m'
-    BOLD = '\033[1m'
-    UNDERLINE = '\033[4m'
-
-
-def build_dicom_affine(Dicomfiles):
-    """
-    Build the dicom affine matrix.
-    The reference I used to create the affine is `NIbabel <https://nipy.org/nibabel/dicom/dicom_orientation.html>`_
-    (we are using the r/c defined under 'DICOM affines again')
-
-    :param Dicomfiles: list of pydicom.dataset.FileDataset instances (created using pydicom.read_file)
-    :type Dicomfiles: list
-    :return: CoordinateMatrix, a 4x4 matrix which transforms the image based coordinates (i,j,k) to world coordinates (x,y,z)
-    """
-
-    assert isinstance(Dicomfiles, list)
-    assert isinstance(Dicomfiles[0], pydicom.dataset.FileDataset)
-
-    ds = Dicomfiles[0]  # just use first one, they all give the same result
-    if not np.logical_or(np.isclose(np.abs(ds.ImageOrientationPatient), 1),
-                         np.isclose(np.abs(ds.ImageOrientationPatient), 0)).all():
-        '''
-        This just checks that the ImageOrientationPatient tag only contains 0 or 1, i.e. that no weird oblique
-        orientation is in use. For now I don't want to support or think about non cardinal encoding directions
-        '''
-        raise NotImplementedError('at the moment we only support cardinal imaging planes')
-
-    CoordinateMatrix = np.zeros([4, 4])
-    F = np.array([ds.ImageOrientationPatient[3:], ds.ImageOrientationPatient[:3]]).T
-    F = np.round(F)
-    first_col = np.multiply(F[:, 0], ds.PixelSpacing[0])
-    sec_col = np.multiply(F[:, 1], ds.PixelSpacing[1])
-    CoordinateMatrix[:, 0][0:3] = first_col
-    CoordinateMatrix[:, 1][0:3] = sec_col
-    CoordinateMatrix[:, 3][0:3] = [float(i) for i in ds.ImagePositionPatient]
-    if Dicomfiles.__len__() > 1:
-        # figure out slice direction
-        SliceLoc = []
-        image_position_patient_list = []
-        for file in Dicomfiles:
-            # need to extract the slice coordinates one at a time (can't think of a better way anyway...)
-            image_position_patient_list.append(file.ImagePositionPatient)
-            SliceLoc.append(file.SliceLocation)
-        SliceLoc = np.array(SliceLoc)
-        image_position_patient_list = np.array(image_position_patient_list)
-        if not np.allclose(np.diff(SliceLoc), np.diff(SliceLoc)[0], atol=.1, rtol=.1):
-            logger.error(f'it appears there are missing or inconsistently spaced slices. Continuing')
-        k = (image_position_patient_list[-1] - image_position_patient_list[0])/(image_position_patient_list.shape[0]-1)
-        CoordinateMatrix[0:3, 2] = k
-
-    return CoordinateMatrix
-
-
-def printProgressBar (iteration, total, prefix = '', suffix = '', decimals = 1, length = 100, fill = '█'):
-    """
-    Call in a loop to create terminal progress bar. `credit here <https://gist.github.com/greenstick/b23e475d2bfdc3a82e34eaa1f6781ee4>`_
-
-    :param iteration: current iteration (Int)
-    :param total: total iterations (Int)
-    :param prefix:  prefix string (Str)
-    :param suffix: suffix string (Str)
-    :param decimals: positive number of decimals in percent complete (Int)
-    :param length: character length of bar (Int)
-    :param fill: bar fill character (Str)
-    :return: progress_string: the string to print
-    """
-    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
-    filledLength = int(length * iteration // total)
-    bar = fill * filledLength + '-' * (length - filledLength)
-    progress_string = f'\r{prefix} |{bar}| {percent}% {suffix}'
-    return progress_string
-
-
-def dicom_to_numpy(path_to_dicoms, FilesToReadIn=None, file_extension='dcm', return_XYZ=False,
-                   zero_pad=0, enforce_increasing_coords=False):
-    """
-    This function does two things:
-
-    1. Loads all the dicom files in path_to_dicoms in a numpy array. data is ordered according to [row, column, slice]
-    2. Builds the matrix that transforms the [r,c,s] indices into [x,y,z] coordinates
-
-    :param path_to_dicoms: folder where all dicoms images are stored
-    :type path_to_dicoms: pathlib.Path or string
-    :param FilesToReadIn: By default, this function will read in all files of file type file_extension. If you only want
-        to read in a subset of files, you can specify them with FilesToReadIn
-    :type FilesToReadIn: list, optional
-    :param file_extension: extension of dicom files, e.g. 'dcm' or 'IMA'
-    :type file_extension: string
-    :param return_XYZ: if True, will build and return three matrics containing the X, Y, and Z coords at each i,j,k
-        pixel.
-    :type return_XYZ: bool, optional
-    :param zero_pad: this many zeros will be placed around the returned volume and the coordinates updated accordingly.
-        main use case was for distortion correction. Note that all returned objects will be  consistently affected
-        by this parameter
-    :type zero_pad: int, optional
-    :returns: ImageArray: a numpy array of voxels
-    :returns: dicom_affine: a matrix that transforms the [r,c,s] indices into [x,y,z] coordinates
-    :returns: (X, Y, Z): Coordinate arrays the same size as ImageArray. Optional
-    """
-    if not FilesToReadIn:
-        FilesToReadIn = get_all_files(path_to_dicoms, file_extension=file_extension)
-    if not FilesToReadIn:
-        raise FileNotFoundError(f'could not find any {file_extension} files in input directory {path_to_dicoms}'
-                                f'\nTry using the ImExtenstion= input option to look for different image types')
-    if isinstance(FilesToReadIn, list):
-        CompletePathFiles = [str(Path(path_to_dicoms) / file) for file in FilesToReadIn]
-    elif isinstance(FilesToReadIn, (str, pathlib.Path)):
-        CompletePathFiles = [str(Path(path_to_dicoms) / FilesToReadIn)]
-
-    dicom_slices = [pydicom.read_file(f) for f in CompletePathFiles]
-
-    dicom_slices = sort_dicom_slices(dicom_slices)[0]
-    dicom_affine = build_dicom_affine(dicom_slices)
-    dicom_affine[0:3, 3] = dicom_affine[0:3, 3] + (-1*zero_pad*dicom_affine[0:3, 0:3].sum(axis=1))  # update start point for zero padding
-    n_rows = dicom_slices[0].Rows + zero_pad*2
-    n_cols = dicom_slices[0].Columns + zero_pad*2
-    n_slices = len(dicom_slices) + zero_pad*2
-
-    ImageArray = np.zeros([n_rows, n_cols, n_slices])
-    if enforce_increasing_coords:
-        # this option exists for the distortion correction code, which increasing indices
-        new_affine = dicom_affine.copy()
-        coordinates_end = dicom_affine @ [n_rows-1, n_cols-1, n_slices-1, 1]
-        for col in [0, 1]:  # check first two cols
-            for i, pixel_increment in enumerate(dicom_affine[:, col]):
-                if pixel_increment < 0:
-                    '''
-                    then we need to force this to positive, and switch the start position to the 
-                    current end position
-                    '''
-                    new_affine[i, col] = -1 * pixel_increment
-                    new_start = coordinates_end[i]
-                    new_affine[i, 3] = new_start
-        dicom_affine = new_affine
-    for i, file in enumerate(dicom_slices):
-        if zero_pad > 0:
-            ImageArray[zero_pad:-zero_pad, zero_pad:-zero_pad, i+zero_pad] = file.pixel_array
-        else:
-            ImageArray[:, :, i] = file.pixel_array
-    if return_XYZ:
-        rcsMatrix = np.zeros([4, n_rows * n_cols * n_slices])
-        r_indices = np.arange(0, n_rows)
-        c_indices = np.arange(0, n_cols)
-        s_indices = np.arange(0, n_slices)
-        [RR, CC, SS] = np.meshgrid(r_indices, c_indices, s_indices, indexing='ij')
-        rcsMatrix[0, :] = RR.flatten()
-        rcsMatrix[1, :] = CC.flatten()
-        rcsMatrix[2, :] = SS.flatten()
-        rcsMatrix[3, :] = 1
-        XYZtemp = np.matmul(dicom_affine, rcsMatrix)
-        X = np.reshape(XYZtemp[0, :], ImageArray.shape)
-        Y = np.reshape(XYZtemp[1, :], ImageArray.shape)
-        Z = np.reshape(XYZtemp[2, :], ImageArray.shape)
-
-        assert ImageArray.shape == X.shape
-
-        return ImageArray, dicom_affine, (X, Y, Z)
-    else:
-        return ImageArray, dicom_affine
-
-
-def sort_dicom_slices(dicom_datasets, filter_non_image_data=True):
-    """
-    sort slices by instance number
-
-    :param dicom_datasets: list of pydicom files
-    :return: sorted list of pydicom files
-    :param filter_non_image_data: if True, any dicom file not containing a pixel_data attribute is removed
-    :type filter_non_image_data: boolean, optional
-    """
-    if filter_non_image_data:
-        contains_pixel_data_ind = [hasattr(dicom, 'pixel_array') for dicom in dicom_datasets]
-        dicom_datasets = list(compress(dicom_datasets, contains_pixel_data_ind))
-    instance_number = [el.InstanceNumber for el in dicom_datasets]
-    sort_ind = np.argsort(instance_number)
-    return list(np.array(dicom_datasets)[sort_ind]), sort_ind
-
-
-def get_all_files(PathToData, file_extension):
-    """
-    quick script to just collect all the files in the Analysis path
-
-    :param PathToData: folder where the files are
-    :type PathToData: pathlib.Path or string
-    :param file_extension: extension of files to return, e.g. 'dcm'
-    :type file_extension: str
-    :returns Files: list of all found files
-    """
-
-    if not file_extension[0] == '.':
-        # handles the case where the user entered 'dcm' instead of '.dcm'
-        file_extension = '.' + file_extension
-    file_extension = '*' + file_extension
-    # check that this is now in the format we require
-    if not file_extension[0:2] == '*.':
-        logger.error('please enter the file_extension parameter like this : file_extension = "jpg"')
-        sys.exit(1)
-
-    if not isinstance(PathToData,Path):
-        PathToData = Path(PathToData)
-
-    if not os.path.isdir(PathToData):
-        raise FileNotFoundError(f'invalid path supplied; {PathToData} does not exist')
-    AllFiles = glob.glob(str(PathToData / file_extension))
-    Files = []
-    for file in AllFiles:
-        head, tail = os.path.split(file)
-        Files.append(tail)
-    if not Files:
-        logging.error(f'no {file_extension} files in {PathToData}')
-
-    return Files
-
-
-def convert_cartesian_to_spherical(InputCoords):
-    """
-    Converts cartesian coordinates [x,y,z] to spherical coordinates [r, azimuth, elevation].
-    If r, azimuth, or elevation already exist as column names they are overwritten.
-    The convention used here matches the convention
-    `matlab uses <https://www.mathworks.com/help/matlab/ref/cart2sph.html>`_, except that we add pi to the azimuth and
-    pi/2 to the elevation such that
-
-    - 0 <= azimuth <= 2*pi
-    - 0 <= elevation <= pi
-
-    There was once a very good reason for doing this; I can't remember what it was anymore but I like to stick
-    to tradition.
-
-    :param InputCoords: a data frame containing (at least) columns x, y, z.
-    :returns InputCoords: same data frame with additional columns [r, azimuth, elevation]
-    """
-    if 'r' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='r')
-    if 'azimuth' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='azimuth')
-    if 'elevation' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='elevation')
-
-    InputCoords.insert(3, "r", np.sqrt(InputCoords.x ** 2 + InputCoords.y ** 2 + InputCoords.z ** 2))
-    InputCoords.insert(4, "azimuth", np.arctan2(InputCoords.y, InputCoords.x) + np.pi)
-    InputCoords.insert(5, "elevation", np.arctan2(InputCoords.z, np.sqrt(InputCoords.x ** 2 + InputCoords.y ** 2)) + np.pi/2)
-
-
-    return InputCoords
-
-
-def generate_harmonic_names(n_order):
-    """
-    generate the names of each harmonic. Used to label the columns in the harmonics dataframe
-
-    :param n_order: order of harmonics
-    :type n_order: int
-
-    :return: coeef_names: a list of names
-    """
-    k = 0
-    coeff_names = []
-    for n in range(0, n_order + 1):  # the plus 1 is because range stops at -1 for some reason
-        coeff_names.append(f'A_{n}_0')
-        k = k + 1
-        for m in range(0, n):
-            coeff_names.append(f'A_{n}_{m + 1}')
-            k = k + 1
-            coeff_names.append(f'B_{n}_{m + 1}')
-            k = k + 1
-    return coeff_names
-
-
-def combine_harmonics(harmonics_1, harmonics_2, operation='add', n_order_return=None):
-    """
-    This is a general purpose function to combine two harmonic series.
-    If the series are of the same order, this is the default order of the returned series.
-    If they are different, by default the returned series will match the higher order.
-    In either case, you can specify the return order to be lower than the default.
-
-    :param harmonics_1: first series to combine
-    :type harmonics_1: array-like
-    :param harmonics_2: second series to combine
-    :type harmonics_2: array-like
-    :param operation: 'add' or 'subtract'
-    :type operation: str, optional
-    :param n_order_return: order of returned series
-    :type n_order_return: int, optional
-
-    :return: combined_harmonics
-    """
-
-    assert isinstance(n_order_return, int) or n_order_return is None
-    assert operation=='add' or operation=='subtract'
-
-    if (len(harmonics_1) == len(harmonics_2)):
-        if operation == 'add':
-            combined_harmonics = np.add(harmonics_1, harmonics_2)
-        elif operation == 'subtract':
-            combined_harmonics = np.subtract(harmonics_1, harmonics_2)
-        harmonics_zeros = harmonics_1.copy()
-        harmonics_zeros[:] = 0
-        new_index = generate_harmonic_names(len(harmonics_2))
-    elif len(harmonics_1) > len(harmonics_2):
-        combined_harmonics = list(np.zeros(len(harmonics_1)))
-        lower_ind = len(harmonics_2)
-        if operation == 'add':
-            combined_harmonics[:lower_ind] = np.add(harmonics_2, harmonics_1[:lower_ind])
-        elif operation == 'subtract':
-            combined_harmonics[:lower_ind] = np.subtract(harmonics_2, harmonics_1[:lower_ind])
-        combined_harmonics[lower_ind:] = harmonics_1[lower_ind:]
-    else:
-        combined_harmonics = list(np.zeros(len(harmonics_1)))
-        lower_ind = len(harmonics_1)
-        if operation == 'add':
-            combined_harmonics[:lower_ind] = np.add(harmonics_2[:lower_ind], harmonics_1)
-        elif operation == 'subtract':
-            combined_harmonics[:lower_ind] = np.subtract(harmonics_2[:lower_ind], harmonics_1)
-        combined_harmonics[lower_ind:] = harmonics_2[lower_ind:]
-
-    n_order_in = int(np.sqrt(len(combined_harmonics)) - 1)
-    new_index = generate_harmonic_names(n_order_in)
-    assert len(combined_harmonics) == np.max([len(harmonics_2), len(harmonics_1)])
-    if n_order_return is not None:
-
-        if n_order_return > n_order_in:
-            logger.warning(f'return order of {n_order_return} specified, but maximum input order is {n_order_in} '
-                          f'so this has no effect')
-            clip_ind = len(combined_harmonics)
-        else:
-            clip_ind = int((n_order_return + 1) ** 2)
-        combined_harmonics = combined_harmonics[:clip_ind]
-        new_index = new_index[:clip_ind]
-
-    combined_harmonics = pd.Series(combined_harmonics, index=new_index)
-
-    return combined_harmonics
-
-
-def convert_spherical_to_cartesian(InputCoords):
-    """
-    Converts spherical coordinates [r, azimuth, elevation] to cartesian coordinates [x,y,z].
-    if the cartesian columns 'x', 'y', 'z' already exist, they will be overwritten
-
-    :param InputCoords: a data frame containing columns r, azimuth, elevation
-    :returns InputCoords:   same data frame with additional columns [x,y,z]
-    """
-    if 'x' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='x')
-    if 'y' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='y')
-    if 'z' in InputCoords.columns:
-        InputCoords = InputCoords.drop(columns='z')
-
-    # InputCoords.insert(3, "x", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
-    # InputCoords.insert(4, "y", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.sin(InputCoords.elevation - np.pi/2))
-    # InputCoords.insert(5, "z", InputCoords.r * np.cos(InputCoords.azimuth))
-
-    InputCoords.insert(3, "x", InputCoords.r * np.cos(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
-    InputCoords.insert(4, "y", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
-    InputCoords.insert(5, "z", InputCoords.r * np.sin(InputCoords.elevation - np.pi/2))
-
-    return InputCoords
-
-
-def generate_legendre_basis(InputCoords, n_order):
-    """
-    Produce spherical base at all coordinate values.
-    This utilises the 'fully normalised' convention described here <https://au.mathworks.com/help/matlab/ref/legendre.html>`_
-    Note that we scale all r values by 1000, which is to help ensure numerical stability. This is based on the assumption
-    that this input data is in mm. The code will throw a warning if this does not appear to the case.
-
-    :param InputCoords: a data frame which can contain whatever you want, but MUST contain columns called
-        elevation, azimuth, and r
-    :type InputCoords: Dataframe
-    :param n_order: order of harmonic fit
-    :type n_order: int
-    :returns legendre_basis: a pandas data frame of size [Ncoords, (n_order +1)**2)]
-    """
-
-    if InputCoords.r.mean() < 10:
-        logger.warning('it appears that your input data is in m, not mm - please use mm!')
-
-    legendre_basis = np.zeros([len(InputCoords.index), (n_order+1)**2])
-    k = 0
-    coeff_names = []
-    for n in range(0, n_order+1):  # the plus 1 is because range stops at -1 for some reason
-        Norm = np.sqrt(n+0.5)
-        P = Norm * lpmv(0, n, np.cos(InputCoords.elevation))
-        legendre_basis[:, k] = np.multiply((InputCoords.r/1000) ** n, P)  # m=0 terms
-        coeff_names.append(f'A_{n}_0')
-        k = k + 1
-        for j in range(0, n):
-            m = j+1  # this looks weird but it works to give values m=1:n
-            Norm = ((-1)**m) * np.sqrt( (n+0.5)*(np.math.factorial(n-m)) / np.math.factorial(n+m))
-            P = Norm * lpmv(m, n, np.cos(InputCoords.elevation))
-            legendre_basis[:,k] = np.multiply(np.multiply((InputCoords.r/1000) ** n, P), np.cos(m * InputCoords.azimuth))
-            coeff_names.append(f'A_{n}_{m}')
-            k = k + 1
-            legendre_basis[:, k] = np.multiply(np.multiply((InputCoords.r/1000) ** n, P), np.sin(m * InputCoords.azimuth))
-            coeff_names.append(f'B_{n}_{m}')
-            k = k + 1
-
-    return pd.DataFrame(legendre_basis, columns=coeff_names)
-
-
-def convert_spherical_harmonics(harmonics, input_format='full', output_format='none'):
-    """
-    function to convert between different harmonic formalisms.
-    At the moment only works between 'fully normalised' and 'unnormalised' but we could add more later if
-    we need to.
-    example::
-
-        g_x_harmonics_no_norm = convert_spherical_harmonics(g_x_harmonics, input_format='full', output_format='none')
-
-    :param harmonics: a pandas series or numpy array of size (n_order+1)^2, where the harmonics are ordered as
-        A00, A10, A11, B11, A20, A21, B21, A22, B22...etc.
-    :param input_format: format of input harmonic normalisation; 'none' or 'full'
-    :param output_format: format of output harmonic normalisation; 'none' or 'full'
-    :return: converted harmonics as a pandas series
-    """
-
-    formats = ['none', 'full']
-    if input_format not in formats:
-        raise NotImplementedError(f'no method exists to convert {input_format} format')
-    if output_format not in formats:
-        raise NotImplementedError(f'no method exists to convert {output_format} format')
-
-    case_string = input_format.lower() + '_' + output_format.lower()
-    if input_format.lower == output_format.lower():
-        case_string = 'same'  # will do nothing, except return the data as a series
-
-    converted_harmonics = harmonics.copy()
-    n_order = np.sqrt(converted_harmonics.shape[0]) - 1
-    assert n_order.is_integer()  # if this is false then an invalid number of harmonics is entered
-    n_order = int(n_order)
-    # generate normalisation factors:
-    k = 0
-    coeff_names = []
-    Norm = []
-    for n in range(0, n_order + 1):  # the plus 1 is because range stops at -1 for some reason
-        Norm.append(np.sqrt(n + 0.5))
-        coeff_names.append(f'A_{n}_0')
-        k = k + 1
-        for j in range(0, n):
-            m = j + 1  # this looks weird but it works to give values m=1:n
-            Norm.append(((-1) ** m) * np.sqrt((n + 0.5) * (np.math.factorial(n - m)) / np.math.factorial(n + m)))
-            coeff_names.append(f'A_{n}_{m}')
-            coeff_names.append(f'B_{n}_{m}')
-            Norm.append(((-1) ** m) * np.sqrt((n + 0.5) * (np.math.factorial(n - m)) / np.math.factorial(n + m)))
-
-    if case_string == 'full_none':
-        converted_harmonics = np.multiply(harmonics, Norm)
-    if case_string == 'none_full':
-        converted_harmonics = np.divide(harmonics, Norm)
-    if isinstance(converted_harmonics, np.ndarray):
-        converted_harmonics = pd.DataFrame(converted_harmonics, index=coeff_names).squeeze()
-
-    return converted_harmonics
-
-
-def get_harmonics(Gx_Harmonics, Gy_Harmonics, Gz_Harmonics, B0_Harmonics=None):
-    """
-    return the gradient spherical harmonics as pandas series. this function is simply a clean way to handle
-    the different ways users can specify harmonics to other componets of this code
-
-    :param Gx_Harmonics: either a pandas series or a path to a csv. If it is already a series we do nothing, but handle
-        this option for cleaner code elsewhere. Gy_Harmonics and Gz_Harmonics are the same.
-    :returns: Gx_Harmonics, Gy_Harmonics, Gz_Harmonics as Pandase series
-    """
-
-    if isinstance(Gx_Harmonics, pd.Series):
-        Gx_Harmonics = Gx_Harmonics
-    elif isinstance(Gx_Harmonics, (str,Path)):
-        if not (Path(Gx_Harmonics).is_file()):
-            raise FileNotFoundError(f'{Gx_Harmonics} does not exist')
-        Gx_Harmonics = pd.read_csv(Gx_Harmonics, index_col=0).squeeze("columns")
-    else:
-        raise AttributeError('could not read in Gx harmonics...please input either a series or a '
-                     'path to a saved csv file')
-
-    if isinstance(Gy_Harmonics, pd.Series):
-        Gy_Harmonics = Gy_Harmonics
-    elif isinstance(Gy_Harmonics, (str,Path)):
-        if not (Path(Gy_Harmonics).is_file()):
-            raise FileNotFoundError(f'{Gy_Harmonics} does not exist')
-        Gy_Harmonics = pd.read_csv(Gy_Harmonics, index_col=0).squeeze("columns")
-    else:
-        raise AttributeError('could not read in Gy harmonics...please input either a series or a '
-                     'path to a saved csv file')
-
-    if isinstance(Gz_Harmonics, pd.Series):
-        Gz_Harmonics = Gz_Harmonics
-    elif isinstance(Gz_Harmonics, (str,Path)):
-        if not (Path(Gz_Harmonics).is_file()):
-            raise FileNotFoundError(f'{Gz_Harmonics} does not exist')
-        Gz_Harmonics = pd.read_csv(Gz_Harmonics, index_col=0).squeeze("columns")
-    else:
-        raise AttributeError('could not read in Gz harmonics...please input either a series or a '
-                     'path to a saved csv file')
-
-    if B0_Harmonics is not None:
-        if isinstance(B0_Harmonics, pd.Series):
-            B0_Harmonics = B0_Harmonics
-        elif isinstance(B0_Harmonics, (str, Path)):
-            if not (Path(B0_Harmonics).is_file()):
-                raise FileNotFoundError(f'{B0_Harmonics} does not exist')
-            B0_Harmonics = pd.read_csv(B0_Harmonics, index_col=0).squeeze("columns")
-        else:
-            raise AttributeError('could not read in B0 harmonics...please input either a series or a '
-                                 'path to a saved csv file')
-
-    return Gx_Harmonics, Gy_Harmonics, Gz_Harmonics, B0_Harmonics
-
-
-def get_dicom_data(dicom_data):
-    """
-    figures out whether dicom data is a dict or a path to a json file
-    if the latter, reads into  a dict and returns
-    """
-
-    if isinstance(dicom_data, dict):
-        return dicom_data
-    elif isinstance(dicom_data,(pathlib.Path, str)):
-        with open(dicom_data, 'r') as f:
-            dicom_data = json.load(f)
-        return dicom_data
-    else:
-        raise AttributeError(f'could not read in dicom_data of type {type(dicom_data)}')
-
-
-def reconstruct_Bz(harmonics, coords, quantity='uT', r_outer=None):
-    """
-    Reconstruct Bz at an arbitrary set of coordinates.
-    n_order of reconstruction is derived from the shape of harmonics
-
-    :param harmonics: a pandas series of size (n_order+1)^2, such as that defined within
-        FieldAnalysis.SphericalHarmonicFit
-    :param coords: a pandas Dataframe which can contain whatever you want, but MUST contain columns called:
-        elevation, azimuth, and r
-    :param quantity:
-        - 'T': return raw field in T
-        - 'uT': return field in uT, with A00 set to 0.
-    :param r_outer: optional parameter; if you try to reconstruct points with r > r_outer a warning is thrown
-    :type r_outer: float or None
-    :returns Bz_recon: Pandas series with the value of Bz at each element in coords
-    """
-
-    if not quantity in ['uT', 'T']:
-        logger.error(f'unsupported quantity "{quantity}" entered for recon.'
-                       f'\n valid options are "field" or "uT". Using uT')
-        quantity = 'uT'
-
-    if any(abs(coords.r) > r_outer):
-        logger.warning(f'you are trying to reconstruct {np.count_nonzero(abs(coords.r) > r_outer)} '
-                       f'data points outside rOuter. You can do it, but the futher away'
-                       'from rOuter you get the less you should trust this.')
-
-    n_order = int(np.sqrt(harmonics.shape[0])-1)
-    legendre_recon = generate_legendre_basis(coords, n_order)
-    if quantity == 'uT':  # field in uT, with A00 set to 0 (e.g. only looking at perturbation)
-        harmonics_temp = harmonics.copy()
-        harmonics_temp.A_0_0 = 0
-        Bz_recon = legendre_recon @ harmonics_temp
-        Bz_recon = Bz_recon * 1e6
-    elif quantity == 'T':  # raw field in T
-        Bz_recon = legendre_recon @ harmonics
-    else:
-        raise NotImplementedError(f'unknown reconstruction option entered: {quantity}')
-
-    return Bz_recon
-
-
-def compare_recon_report_with_ground_truth_report(ground_truth_report, recon_report, tolerance=1):  # pragma: no cover
-    """
-    This is to compare the distortion data contained within two Reports.MRI_QA_recon_reporter
-    objects. The original purpose was to compare a recon_report generated from direct data, and one
-    generated via harmonics, although in principle it can take any two reports.
-
-    :param ground_truth_report: Reports.MRI_QA_recon_reporter instance
-    :param recon_report: Reports.MRI_QA_recon_reporter instance
-    :param tolerance: tolerance in mm
-    """
-    # direct overlay of real versus recon
-    fig, axs = plt.subplots(nrows=2, ncols=2, figsize=[10, 10])
-    if ground_truth_report.r_outer == recon_report.r_outer:
-        # then use r_outer to filter the data
-        gt_data = ground_truth_report._extract_data_from_MatchedMarkerVolume(r_max=ground_truth_report.r_outer)
-        recon_data = recon_report._extract_data_from_MatchedMarkerVolume(r_max=recon_report.r_outer)
-    else:
-        gt_data = ground_truth_report._extract_data_from_MatchedMarkerVolume()
-        recon_data = recon_report._extract_data_from_MatchedMarkerVolume()
-
-    axs[0, 0].scatter(gt_data.r_gt, gt_data.abs_dis)
-    axs[0, 0].scatter(recon_data.r_gt, recon_data.abs_dis)
-    axs[0, 0].legend(['original_data', 'recon_data'])
-    axs[0, 0].set_xlabel('r [mm]')
-    axs[0, 0].set_ylabel('absolute distortion [mm]')
-
-    # scatter of real versus recon
-    axs[0, 1].scatter(gt_data.abs_dis, recon_data.abs_dis)
-    axs[0, 1].set_xlabel('original data')
-    axs[0, 1].set_ylabel('recon data')
-
-    # box plot of errors
-    error = gt_data.abs_dis - recon_data.abs_dis
-    axs[1, 0].boxplot(error)
-    axs[1, 0].set_ylabel('recon error [mm]')
-
-
-    # get index of outliers
-    outliers_ind = error > tolerance
-    print(f'{np.count_nonzero(outliers_ind)} outliers exist, at index {np.where(outliers_ind)}')
-    outliers_ind = np.where(outliers_ind)
-    for ind in outliers_ind[0]:
-        print(f'index {ind} is at {gt_data.x_gt.iloc[ind]: 1.1f},'
-              f' {gt_data.y_gt.iloc[ind]: 1.1f},'
-              f' {gt_data.z_gt.iloc[ind]: 1.1f}  the value in the ground truth is'
-              f' {gt_data.abs_dis.iloc[ind]: 1.1f}'
-              f' and the value in the reconstructed is {recon_data.abs_dis.iloc[ind]: 1.1f}')
-
-
-def enumerate_subfolders(data_loc):
-    """
-    A simple function that prints all the subfolders in data_loc as a dict, e.g::
-
-        {'1': 'folder1',
-         '2': 'folder2'} etc
-
-    I find this is a useful to create a dict object that I copy to the start of my analysis scripts
-    """
-    data_dict = {}
-    subfolders = [ f.path for f in os.scandir(data_loc) if f.is_dir() ]
-    subfolders = np.sort(subfolders)
-    for i, dir in enumerate(subfolders):
-        folder_name = os.path.split(dir)[1]
-        data_dict[str(i)] = folder_name
-    for key in data_dict.keys():
-        print(f"'{key}': '{data_dict[key]}',")
-
-
-def plot_MarkerVolume_overlay(MarkerVolumeList, legend=None):  # pragma: no cover
-    """
-    Plot overlaid 3D scatter plots of the marker positions in each MarkerVolume
-
-    :param MarkerVolumeList: list of MarkerVolume instances
-    :param legend: legend to display on plot
-    :return: None
-    """
-
-    assert isinstance(MarkerVolumeList, list)
-
-    fig = plt.figure()
-    axs = fig.add_subplot(111, projection='3d')
-    for MarkerVolume in MarkerVolumeList:
-        axs.scatter(MarkerVolume.MarkerCentroids.x, MarkerVolume.MarkerCentroids.y, MarkerVolume.MarkerCentroids.z)
-        axs.set_xlabel('X [mm]')
-        axs.set_ylabel('Y [mm]')
-        axs.set_zlabel('Z [mm]')
-        axs.set_title('3D marker positions')
-    axs.set_box_aspect((np.ptp(MarkerVolume.MarkerCentroids.x),
-                        np.ptp(MarkerVolume.MarkerCentroids.y),
-                        np.ptp(MarkerVolume.MarkerCentroids.z)))
-    if legend:
-        plt.legend(legend)
-    plt.show()
-
-
-def plot_compressed_MarkerVolumes(MarkerVolumeList, p_max=20, p_min=-20, title=None, legend=None,
-                                  projection_direction='z'): # pragma: no cover
-    """
-    plot overlay of compressed marker volumes (z coord is ignored)
-
-    :param MarkerVolumeList:  list of MarkerVolume instances
-    :type MarkerVolumeList: list
-    :param p_max: max data to include in projection_direction
-    :type p_max: float, optional
-    :param p_min: min z data to include in projection_direction
-    :type p_min: float, optional
-    :param title: title of plot
-    :type title: str, optional
-    :param legend: legend of plot
-    :type legend: list, optional
-    :return: None
-    """
-
-    fig, axs = plt.subplots(figsize=[8, 8], ncols=1, nrows=1)
-    if not isinstance(MarkerVolumeList, list):
-        MarkerVolumeList = list(MarkerVolumeList)
-
-    if not projection_direction in ['x', 'y', 'z']:
-        warnings.warn(f'projection direction must be "x", "y", or "z", not {projection_direction}.'
-                      f'setting to z and continuing')
-        projection_direction = 'z'
-
-    for MarkerVolume in MarkerVolumeList:
-        if projection_direction == 'z':
-            data_ind = np.logical_and(MarkerVolume.MarkerCentroids.z > p_min, MarkerVolume.MarkerCentroids.z < p_max)
-            plot_data = MarkerVolume.MarkerCentroids[data_ind]
-            axs.scatter(plot_data.x, plot_data.y)
-            axs.set_xlabel('x [mm]', fontsize=15)
-            axs.set_ylabel('y [mm]', fontsize=15)
-        elif projection_direction == 'x':
-            data_ind = np.logical_and(MarkerVolume.MarkerCentroids.x > p_min, MarkerVolume.MarkerCentroids.x < p_max)
-            plot_data = MarkerVolume.MarkerCentroids[data_ind]
-            axs.scatter(plot_data.z, plot_data.y)
-            axs.set_xlabel('z [mm]', fontsize=15)
-            axs.set_ylabel('y [mm]', fontsize=15)
-        elif projection_direction == 'y':
-            data_ind = np.logical_and(MarkerVolume.MarkerCentroids.y > p_min, MarkerVolume.MarkerCentroids.y < p_max)
-            plot_data = MarkerVolume.MarkerCentroids[data_ind]
-            axs.scatter(plot_data.x, plot_data.z)
-            axs.set_xlabel('x [mm]', fontsize=15)
-            axs.set_ylabel('z [mm]', fontsize=15)
-
-        axs.set_xlim([-150, 150])
-        axs.set_ylim([-150, 150])
-        axs.tick_params(axis='both', which='major', labelsize=12)
-        axs.tick_params(axis='both', which='minor', labelsize=12)
-        axs.axis("equal")
-        axs.grid()
-        plt.subplots_adjust(bottom=0.25)
-        if legend:
-            plt.legend(legend)
-        if title:
-            plt.title(title)
-
-
-def plot_matched_volume_hist(VolumeList, legend=None):
-    """
-    create a histogram of total distortion for all input volumes
-
-    :param VolumeList: a list of [matched marker volumes](https://acrf-image-x-institute.github.io/MRI_DistortionQA/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes)
-    :type VolumeList: list
-    :param legend: legend to print
-    :type legend: list, optional
-    :return: None
-    """
-    bins = np.linspace(0, 10, 30)
-    plt.figure()
-    for marker_volume in VolumeList:
-        plt.hist(marker_volume.MatchedCentroids.match_distance, bins=bins, alpha=0.5)
-    if legend:
-        plt.legend(['original', 'corrected'])
-    plt.xlabel('distortion [mm]')
-    plt.tight_layout()
-    plt.show()
-
-
-def plot_distortion_xyz_hist(MatchedMarkerVolume):
-    """
-    plot overlaid x, y, z distortion for an input instance of
-    [MatchedMarkerVolume](https://acrf-image-x-institute.github.io/MRI_DistortionQA/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes)
-
-    :param MatchedMarkerVolume: an instance of MatchedMarkerVolumes
-    """
-
-    x_dis = MatchedMarkerVolume.MatchedCentroids.x_gt - MatchedMarkerVolume.MatchedCentroids.x_gnl
-    y_dis = MatchedMarkerVolume.MatchedCentroids.y_gt - MatchedMarkerVolume.MatchedCentroids.y_gnl
-    z_dis = MatchedMarkerVolume.MatchedCentroids.z_gt - MatchedMarkerVolume.MatchedCentroids.z_gnl
-
-    plt.figure()
-    bins = np.linspace(0, 10, 30)
-    plt.hist(abs(x_dis), bins=bins, alpha=0.5)
-    plt.hist(abs(y_dis), bins=bins, alpha=0.5)
-    plt.hist(abs(z_dis), bins=bins, alpha=0.5)
-    plt.legend(['x', 'y', 'z'])
-    plt.xlabel('distortion [mm]')
-    plt.tight_layout()
-    plt.show()
-
-
-def print_dict(dict):
-    """
-    just provides a nicer display of the input dict than the default print function,
-    got sick of writing the same code over and over...
-    """
-    for key in dict.keys():
-        print(f'{key}: {dict[key]}')
-
-
-def plot_harmonics_over_sphere(harmonics, radius, title=None):  # pragma: no cover
-    """
-    plot the reconstructed harmonics over the surface of a sphere
-    I've used plotly instead of matplotlib for this as I wasnt happy with the matplotlib result.
-
-    :param harmonics: either an instance of SphericalHarmonicFit or the equivalent data frame loaded from csv
-    :param radius: radius of sphere
-    :type radius: float
-    :return: None
-    """
-    if title is None:
-        title = 'DSV surface [uT]'
-    # generate coordinates:
-    _density = 100
-    azimuth = np.linspace(0, 2*np.pi, _density)
-    elevation = np.linspace(0, np.pi, _density)
-    [AZ, EL] = np.meshgrid(azimuth, elevation)
-    R = np.ones(AZ.shape) * radius
-    coords = pd.DataFrame({'elevation': EL.flatten(), 'azimuth': AZ.flatten(), 'r': R.flatten()})
-    coords = convert_spherical_to_cartesian(coords)
-    X = coords.x.to_numpy().reshape(R.shape)
-    Y = coords.y.to_numpy().reshape(R.shape)
-    Z = coords.z.to_numpy().reshape(R.shape)
-
-    Bz = reconstruct_Bz(harmonics, coords)
-    Bz = Bz.to_numpy().reshape(R.shape)
-
-    fig_harmonic_surface = go.Figure(data=[go.Surface(z=Z, x=X, y=Y, colorbar=dict(title='B(uT)',
-                                                                                   titlefont={'size': 20},
-                                                                                   tickfont=dict(size=40)),
-                                                                    surfacecolor=Bz)])
-
-    _available_plotly_themes = ["plotly", "plotly_white", "plotly_dark", "ggplot2",
-                                "seaborn", "simple_white", "none"]
-    _plotly_theme = 'seaborn'
-    assert _plotly_theme in _available_plotly_themes
-    fig_harmonic_surface.update_layout(title=title, autosize=True,
-                                       template=_plotly_theme,
-                                       font={'size': 20},
-                                       scene=dict(xaxis=dict(title='X [mm]', titlefont=dict(size=20)),
-                                                  yaxis=dict(title='Y [mm]', titlefont=dict(size=20)),
-                                                  zaxis=dict(title='Z [mm]', titlefont=dict(size=20))))
-
-    return fig_harmonic_surface
-
-
-def read_opera_table_file(data_loc):
-    """
-    reads a table file from opera Tosca and returns the data as a data frame that can be
-    read into spherical harmonic fit.
-    Expected column order is  X [MM], Y [MM], Z [MM], BZ [T], with 6 header lines.
-    No error handling is included for incorrect input
-
-    :param data_loc: location of table file
-    :type data_loc: str or pathlib.Path
-    :return: Bz_data, a pandas dataframe
-    """
-    with open(data_loc, 'r') as f:
-        data = np.loadtxt(f, skiprows=6)
-    assert data.shape[1] == 4
-
-    input_Bz_data = pd.DataFrame({'x': data[:, 0], 'y': data[:, 1], 'z': data[:, 2], 'Bz': data[:, 3]})
-    return input_Bz_data
+"""
+General purpose reusable functions
+"""
+
+import os
+import pathlib
+import sys
+import glob
+import logging
+from pathlib import Path
+import numpy as np
+from scipy.special import lpmv
+import pandas as pd
+from matplotlib import pyplot as plt
+import pydicom
+import json
+
+
+ch = logging.StreamHandler()
+formatter = logging.Formatter('[%(filename)s: line %(lineno)d %(levelname)8s] %(message)s')
+ch.setFormatter(formatter)
+logger = logging.getLogger(__name__)
+logger.addHandler(ch)
+logger.setLevel(logging.INFO)  # This toggles all the logging in your app
+logger.propagate = False
+
+
+class bcolors:
+    """
+    This is just here to enable me to print pretty colors to the linux terminal
+    """
+    HEADER = '\033[95m'
+    OKBLUE = '\033[94m'
+    OKCYAN = '\033[96m'
+    OKGREEN = '\033[92m'
+    WARNING = '\033[93m'
+    FAIL = '\033[91m'
+    ENDC = '\033[0m'
+    BOLD = '\033[1m'
+    UNDERLINE = '\033[4m'
+
+
+def build_dicom_affine(Dicomfiles):
+    """
+    Build the dicom affine matrix.
+    The reference I used to create the affine is `NIbabel <https://nipy.org/nibabel/dicom/dicom_orientation.html>`_
+    (we are using the r/c defined under 'DICOM affines again')
+
+    :param Dicomfiles: list of pydicom.dataset.FileDataset instances (created using pydicom.read_file)
+    :type Dicomfiles: list
+    :return: CoordinateMatrix, a 4x4 matrix which transforms the image based coordinates (i,j,k) to world coordinates (x,y,z)
+    """
+
+    assert isinstance(Dicomfiles, list)
+    assert isinstance(Dicomfiles[0], pydicom.dataset.FileDataset)
+
+    ds = Dicomfiles[0]  # just use first one, they all give the same result
+    if not np.logical_or(np.isclose(np.abs(ds.ImageOrientationPatient), 1),
+                         np.isclose(np.abs(ds.ImageOrientationPatient), 0)).all():
+        '''
+        This just checks that the ImageOrientationPatient tag only contains 0 or 1, i.e. that no weird oblique
+        orientation is in use. For now I don't want to support or think about non cardinal encoding directions
+        '''
+        raise NotImplementedError('at the moment we only support cardinal imaging planes')
+
+    CoordinateMatrix = np.zeros([4, 4])
+    F = np.array([ds.ImageOrientationPatient[3:], ds.ImageOrientationPatient[:3]]).T
+    F = np.round(F)
+    first_col = np.multiply(F[:, 0], ds.PixelSpacing[0])
+    sec_col = np.multiply(F[:, 1], ds.PixelSpacing[1])
+    CoordinateMatrix[:, 0][0:3] = first_col
+    CoordinateMatrix[:, 1][0:3] = sec_col
+    CoordinateMatrix[:, 3][0:3] = [float(i) for i in ds.ImagePositionPatient]
+    if Dicomfiles.__len__() > 1:
+        # figure out slice direction
+        SliceLoc = []
+        image_position_patient_list = []
+        for file in Dicomfiles:
+            # need to extract the slice coordinates one at a time (can't think of a better way anyway...)
+            image_position_patient_list.append(file.ImagePositionPatient)
+            SliceLoc.append(file.SliceLocation)
+        SliceLoc = np.array(SliceLoc)
+        image_position_patient_list = np.array(image_position_patient_list)
+        if not np.allclose(np.diff(SliceLoc), np.diff(SliceLoc)[0], atol=.1, rtol=.1):
+            logger.error(f'it appears there may be missing or inconsistently spaced slices. Continuing')
+        k = (image_position_patient_list[-1] - image_position_patient_list[0])/(image_position_patient_list.shape[0]-1)
+        CoordinateMatrix[0:3, 2] = k
+
+    return CoordinateMatrix
+
+
+def printProgressBar (iteration, total, prefix = '', suffix = '', decimals = 1, length = 100, fill = '█'):
+    """
+    [credit here](https://gist.github.com/greenstick/b23e475d2bfdc3a82e34eaa1f6781ee4)
+
+    Call in a loop to create terminal progress bar
+
+        iteration   - Required  :
+        total       - Required  :
+        prefix      - Optional  :
+        suffix      - Optional  :
+        decimals    - Optional  :
+        length      - Optional  :
+        fill        - Optional  :
+        printEnd    - Optional  : end character (e.g. "\r", "\r\n") (Str)
+
+    :param iteration: current iteration (Int)
+    :param total: total iterations (Int)
+    :param prefix:  prefix string (Str)
+    :param suffix: suffix string (Str)
+    :param decimals: positive number of decimals in percent complete (Int)
+    :param length: character length of bar (Int)
+    :param fill: bar fill character (Str)
+    :return: progress_string: the string to print
+    """
+    percent = ("{0:." + str(decimals) + "f}").format(100 * (iteration / float(total)))
+    filledLength = int(length * iteration // total)
+    bar = fill * filledLength + '-' * (length - filledLength)
+    progress_string = f'\r{prefix} |{bar}| {percent}% {suffix}'
+    return progress_string
+
+
+def dicom_to_numpy(path_to_dicoms, FilesToReadIn=None, file_extension='dcm', return_XYZ=False,
+                   zero_pad=0, enforce_increasing_coords=False):
+    """
+    This function does two things:
+
+    1. Loads all the dicom files in path_to_dicoms in a numpy array. data is ordered according to [row, column, slice]
+    2. Builds the matrix that transforms the [r,c,s] indices into [x,y,z] coordinates
+
+    :param path_to_dicoms: folder where all dicoms images are stored
+    :type path_to_dicoms: pathlib.Path or string
+    :param FilesToReadIn: By default, this function will read in all files of file type file_extension. If you only want
+        to read in a subset of files, you can specify them with FilesToReadIn
+    :type FilesToReadIn: list, optional
+    :param file_extension: extension of dicom files, e.g. 'dcm' or 'IMA'
+    :type file_extension: string
+    :param return_XYZ: if True, will build and return three matrics containing the X, Y, and Z coords at each i,j,k
+        pixel.
+    :type return_XYZ: bool, optional
+    :param zero_pad: this many zeros will be placed around the returned volume and the coordinates updated accordingly.
+        main use case was for distortion correction. Note that all returned objects will be self consistently affected
+        by this parameter
+    :type zero_pad: int, optional
+    :returns: ImageArray: a numpy array of voxels
+    :returns: dicom_affine: a matrix that transforms the [r,c,s] indices into [x,y,z] coordinates
+    :returns: (X, Y, Z): Coordinate arrays the same size as ImageArray. Optional
+    """
+    if not FilesToReadIn:
+        FilesToReadIn = get_all_files(path_to_dicoms, file_extension=file_extension)
+    if not FilesToReadIn:
+        raise FileNotFoundError(f'could not find any {file_extension} files in input directory {path_to_dicoms}'
+                                f'\nTry using the ImExtenstion= input option to look for different image types')
+    if isinstance(FilesToReadIn, list):
+        CompletePathFiles = [str(Path(path_to_dicoms) / file) for file in FilesToReadIn]
+    elif isinstance(FilesToReadIn, (str, pathlib.Path)):
+        CompletePathFiles = [str(Path(path_to_dicoms) / FilesToReadIn)]
+
+    dicom_slices = [pydicom.read_file(f) for f in CompletePathFiles]
+    dicom_slices = sort_dicom_slices(dicom_slices)
+    dicom_affine = build_dicom_affine(dicom_slices)
+    dicom_affine[0:3, 3] = dicom_affine[0:3, 3] + (-1*zero_pad*dicom_affine[0:3, 0:3].sum(axis=1))  # update start point for zero padding
+    n_rows = dicom_slices[0].Rows + zero_pad*2
+    n_cols = dicom_slices[0].Columns + zero_pad*2
+    n_slices = len(dicom_slices) + zero_pad*2
+
+    ImageArray = np.zeros([n_rows, n_cols, n_slices])
+    if enforce_increasing_coords:
+        # this option exists for the distortion correction code, which increasing indices
+        new_affine = dicom_affine.copy()
+        coordinates_end = dicom_affine @ [n_rows-1, n_cols-1, n_slices-1, 1]
+        for col in [0, 1]:  # check first two cols
+            for i, pixel_increment in enumerate(dicom_affine[:, col]):
+                if pixel_increment < 0:
+                    '''
+                    then we need to force this to positive, and switch the start position to the 
+                    current end position
+                    '''
+                    new_affine[i, col] = -1 * pixel_increment
+                    new_start = coordinates_end[i]
+                    new_affine[i, 3] = new_start
+        dicom_affine = new_affine
+    for i, file in enumerate(dicom_slices):
+        if zero_pad > 0:
+            ImageArray[zero_pad:-zero_pad, zero_pad:-zero_pad, i+zero_pad] = file.pixel_array
+        else:
+            ImageArray[:, :, i] = file.pixel_array
+    if return_XYZ:
+        rcsMatrix = np.zeros([4, n_rows * n_cols * n_slices])
+        r_indices = np.arange(0, n_rows)
+        c_indices = np.arange(0, n_cols)
+        s_indices = np.arange(0, n_slices)
+        [RR, CC, SS] = np.meshgrid(r_indices, c_indices, s_indices, indexing='ij')
+        rcsMatrix[0, :] = RR.flatten()
+        rcsMatrix[1, :] = CC.flatten()
+        rcsMatrix[2, :] = SS.flatten()
+        rcsMatrix[3, :] = 1
+        XYZtemp = np.matmul(dicom_affine, rcsMatrix)
+        X = np.reshape(XYZtemp[0, :], ImageArray.shape)
+        Y = np.reshape(XYZtemp[1, :], ImageArray.shape)
+        Z = np.reshape(XYZtemp[2, :], ImageArray.shape)
+
+        assert ImageArray.shape == X.shape
+
+        return ImageArray, dicom_affine, (X, Y, Z)
+    else:
+        return ImageArray, dicom_affine
+
+
+def sort_dicom_slices(dicom_datasets):
+    """
+    sort slices by instance number
+    :param dicom_datasets: list of pydicom files
+    :return: sorted list of pydicom files
+    """
+    instance_number = [el.InstanceNumber for el in dicom_datasets]
+    sort_ind = np.argsort(instance_number)
+    return list(np.array(dicom_datasets)[sort_ind])
+
+
+def get_all_files(PathToData, file_extension):
+    """
+    quick script to just collect all the files in the Analysis path
+
+    :param PathToData: folder where the files are
+    :type PathToData: pathlib.Path or string
+    :param file_extension: extension of files to return, e.g. 'dcm'
+    :type file_extension: str
+    :returns Files: list of all found files
+    """
+
+    if not file_extension[0] == '.':
+        # handles the case where the user entered 'dcm' instead of '.dcm'
+        file_extension = '.' + file_extension
+    file_extension = '*' + file_extension
+    # check that this is now in the format we require
+    if not file_extension[0:2] == '*.':
+        logger.error('please enter the file_extension parameter like this : file_extension = "jpg"')
+        sys.exit(1)
+
+    if not isinstance(PathToData,Path):
+        PathToData = Path(PathToData)
+
+    if not os.path.isdir(PathToData):
+        raise FileNotFoundError(f'invalid path supplied; {PathToData} does not exist')
+    AllFiles = glob.glob(str(PathToData / file_extension))
+    Files = []
+    for file in AllFiles:
+        head, tail = os.path.split(file)
+        Files.append(tail)
+    if not Files:
+        logging.error(f'no {file_extension} files in {PathToData}')
+
+    return Files
+
+
+def convert_cartesian_to_spherical(InputCoords):
+    """
+    Converts cartesian coordinates [x,y,z] to spherical coordinates [r, azimuth, elevation].
+    If r, azimuth, or elevation already exist as column names they are overwritten.
+    The convention used here matches the convention
+    `matlab uses <https://www.mathworks.com/help/matlab/ref/cart2sph.html>`_, except that we add pi to the azimuth and
+    pi/2 to the elevation such that
+
+    - 0 <= azimuth <= 2*pi
+    - 0 <= elevation <= pi
+
+    There was once a very good reason for doing this; I can't remember what it was anymore but I like to stick
+    to tradition.
+
+    :param InputCoords: a data frame containing (at least) columns x, y, z.
+    :returns InputCoords: same data frame with additional columns [r, azimuth, elevation]
+    """
+    if 'r' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='r')
+    if 'azimuth' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='azimuth')
+    if 'elevation' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='elevation')
+
+    InputCoords.insert(3, "r", np.sqrt(InputCoords.x ** 2 + InputCoords.y ** 2 + InputCoords.z ** 2))
+    InputCoords.insert(4, "azimuth", np.arctan2(InputCoords.y, InputCoords.x) + np.pi)
+    InputCoords.insert(5, "elevation", np.arctan2(InputCoords.z, np.sqrt(InputCoords.x ** 2 + InputCoords.y ** 2)) + np.pi/2)
+
+
+    return InputCoords
+
+
+def convert_spherical_to_cartesian(InputCoords):
+    """
+    Converts spherical coordinates [r, azimuth, elevation] to cartesian coordinates [x,y,z].
+    if the cartesian columns 'x', 'y', 'z' already exist, they will be overwritten
+
+    :param InputCoords: a data frame containing columns r, azimuth, elevation
+    :returns InputCoords:   same data frame with additional columns [x,y,z]
+    """
+    if 'x' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='x')
+    if 'y' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='y')
+    if 'z' in InputCoords.columns:
+        InputCoords = InputCoords.drop(columns='z')
+
+    # InputCoords.insert(3, "x", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
+    # InputCoords.insert(4, "y", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.sin(InputCoords.elevation - np.pi/2))
+    # InputCoords.insert(5, "z", InputCoords.r * np.cos(InputCoords.azimuth))
+
+    InputCoords.insert(3, "x", InputCoords.r * np.cos(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
+    InputCoords.insert(4, "y", InputCoords.r * np.sin(InputCoords.azimuth - np.pi) * np.cos(InputCoords.elevation - np.pi/2))
+    InputCoords.insert(5, "z", InputCoords.r * np.sin(InputCoords.elevation - np.pi/2))
+
+    return InputCoords
+
+
+def generate_legendre_basis(InputCoords, n_order):
+    """
+    Produce spherical base at all coordinate values.
+    This utilises the 'fully normalised' convention described here <https://au.mathworks.com/help/matlab/ref/legendre.html>`_
+    Note that we scale all r values by 1000, which is to help ensure numerical stability. This is based on the assumption
+    that this input data is in mm. The code will throw a warning if this does not appear to the case.
+
+    :param InputCoords: a data frame which can contain whatever you want, but MUST contain columns called
+        elevation, azimuth, and r
+    :type InputCoords: Dataframe
+    :param n_order: order of harmonic fit
+    :type n_order: int
+    :returns legendre_basis: a pandas data frame of size [Ncoords, (n_order +1)**2)]
+    """
+
+    if InputCoords.r.mean() < 10:
+        logger.warning('it appears that your input data is in m, not mm - please use mm!')
+
+    legendre_basis = np.zeros([len(InputCoords.index), (n_order+1)**2])
+    k = 0
+    coeff_names = []
+    for n in range(0, n_order+1):  # the plus 1 is because range stops at -1 for some reason
+        Norm = np.sqrt(n+0.5)
+        P = Norm * lpmv(0, n, np.cos(InputCoords.elevation))
+        legendre_basis[:, k] = np.multiply((InputCoords.r/1000) ** n, P)  # m=0 terms
+        coeff_names.append(f'A_{n}_0')
+        k = k + 1
+        for j in range(0, n):
+            m = j+1  # this looks weird but it works to give values m=1:n
+            Norm = ((-1)**m) * np.sqrt( (n+0.5)*(np.math.factorial(n-m)) / np.math.factorial(n+m))
+            P = Norm * lpmv(m, n, np.cos(InputCoords.elevation))
+            legendre_basis[:,k] = np.multiply(np.multiply((InputCoords.r/1000) ** n, P), np.cos(m * InputCoords.azimuth))
+            coeff_names.append(f'A_{n}_{m}')
+            k = k + 1
+            legendre_basis[:, k] = np.multiply(np.multiply((InputCoords.r/1000) ** n, P), np.sin(m * InputCoords.azimuth))
+            coeff_names.append(f'B_{n}_{m}')
+            k = k + 1
+
+    return pd.DataFrame(legendre_basis, columns=coeff_names)
+
+
+def convert_spherical_harmonics(harmonics, input_format='full', output_format='none'):
+    """
+    function to convert between different harmonic formalisms.
+    At the moment only works between 'fully normalised' and 'unnormalised' but we could add more later if
+    we need to.
+    example::
+
+        g_x_harmonics_no_norm = convert_spherical_harmonics(g_x_harmonics, input_format='full', output_format='none')
+
+    :param harmonics: a pandas series or numpy array of size (n_order+1)^2, where the harmonics are ordered as
+        A00, A10, A11, B11, A20, A21, B21, A22, B22...etc.
+    :param input_format: format of input harmonic normalisation; 'none' or 'full'
+    :param output_format: format of output harmonic normalisation; 'none' or 'full'
+    :return: converted harmonics as a pandas series
+    """
+
+    formats = ['none', 'full']
+    if input_format not in formats:
+        raise NotImplementedError(f'no method exists to convert {input_format} format')
+    if output_format not in formats:
+        raise NotImplementedError(f'no method exists to convert {output_format} format')
+
+    case_string = input_format.lower() + '_' + output_format.lower()
+    if input_format.lower == output_format.lower():
+        case_string = 'same'  # will do nothing, except return the data as a series
+
+    converted_harmonics = harmonics.copy()
+    n_order = np.sqrt(converted_harmonics.shape[0]) - 1
+    assert n_order.is_integer()  # if this is false then an invalid number of harmonics is entered
+    n_order = int(n_order)
+    # generate normalisation factors:
+    k = 0
+    coeff_names = []
+    Norm = []
+    for n in range(0, n_order + 1):  # the plus 1 is because range stops at -1 for some reason
+        Norm.append(np.sqrt(n + 0.5))
+        coeff_names.append(f'A_{n}_0')
+        k = k + 1
+        for j in range(0, n):
+            m = j + 1  # this looks weird but it works to give values m=1:n
+            Norm.append(((-1) ** m) * np.sqrt((n + 0.5) * (np.math.factorial(n - m)) / np.math.factorial(n + m)))
+            coeff_names.append(f'A_{n}_{m}')
+            coeff_names.append(f'B_{n}_{m}')
+            Norm.append(((-1) ** m) * np.sqrt((n + 0.5) * (np.math.factorial(n - m)) / np.math.factorial(n + m)))
+
+    if case_string == 'full_none':
+        converted_harmonics = np.multiply(harmonics, Norm)
+    if case_string == 'none_full':
+        converted_harmonics = np.divide(harmonics, Norm)
+    if isinstance(converted_harmonics, np.ndarray):
+        converted_harmonics = pd.DataFrame(converted_harmonics, index=coeff_names).squeeze()
+
+    return converted_harmonics
+
+
+def get_gradient_spherical_harmonics(Gx_Harmonics, Gy_Harmonics, Gz_Harmonics):
+    """
+    return the gradient spherical harmonics as as pandas series. this function is simply a clean way to handle
+    the different ways users can specify harmonics to other componets of this code
+
+    :param Harmonics:
+
+    :param Gx_Harmonics: either a pandas series or a path to a csv. If it is already a series we do nothing, but handle
+        this option for cleaner code elsewhere. Gy_Harmonics and Gz_Harmonics are the same
+    :returns: Gx_Harmonics, Gy_Harmonics, Gz_Harmonics as Pandase series
+    """
+
+    if isinstance(Gx_Harmonics, pd.Series):
+        Gx_Harmonics = Gx_Harmonics
+    elif isinstance(Gx_Harmonics, (str,Path)):
+        Gx_Harmonics = pd.read_csv(Gx_Harmonics, index_col=0).squeeze("columns")
+    else:
+        raise AttributeError('could not read in Gx harmonics...please input either a series or a '
+                     'path to a saved csv file')
+
+
+    if isinstance(Gy_Harmonics, pd.Series):
+        Gy_Harmonics = Gy_Harmonics
+    elif isinstance(Gy_Harmonics, (str,Path)):
+        Gy_Harmonics = pd.read_csv(Gy_Harmonics, index_col=0).squeeze("columns")
+    else:
+        raise AttributeError('could not read in Gy harmonics...please input either a series or a '
+                     'path to a saved csv file')
+
+
+    if isinstance(Gz_Harmonics, pd.Series):
+        Gz_Harmonics = Gz_Harmonics
+    elif isinstance(Gz_Harmonics, (str,Path)):
+        Gz_Harmonics = pd.read_csv(Gz_Harmonics, index_col=0).squeeze("columns")
+    else:
+        raise AttributeError('could not read in Gz harmonics...please input either a series or a '
+                     'path to a saved csv file')
+
+    return Gx_Harmonics, Gy_Harmonics, Gz_Harmonics
+
+
+def get_dicom_data(dicom_data):
+    """
+    figures out whether dicom data is a dict or a path to a json file
+    if the latter, reads into  a dict and returns
+    """
+
+    if isinstance(dicom_data, dict):
+        return dicom_data
+    elif isinstance(dicom_data,(pathlib.Path, str)):
+        with open(dicom_data, 'r') as f:
+            dicom_data = json.load(f)
+        return dicom_data
+    else:
+        raise AttributeError(f'could not read in dicom_data of type {type(dicom_data)}')
+
+
+def reconstruct_Bz(harmonics, coords, quantity='uT', r_outer=None):
+    """
+    Reconstruct Bz at an arbitrary set of coordinates.
+    n_order of reconstruction is derived from the shape of harmonics
+
+    :param harmonics: a pandas series of size (n_order+1)^2, such as that defined within
+        FieldAnalysis.SphericalHarmonicFit
+    :param coords: a pandas Dataframe which can contain whatever you want, but MUST contain columns called:
+        elevation, azimuth, and r
+    :param quantity:
+        - 'T': return raw field in T
+        - 'uT': return field in uT, with A00 set to 0.
+    :param r_outer: optional parameter; if you try to reconstruct points with r > r_outer a warning is thrown
+    :type r_outer: float or None
+    :returns Bz_recon: Pandase series with the value of Bz at each element in coords
+    """
+
+    if not quantity in ['uT', 'T']:
+        logger.error(f'unsupported quantity "{quantity}" entered for recon.'
+                       f'\n valid options are "field" or "uT". Using uT')
+        quantity = 'uT'
+
+    if any(abs(coords.r) > r_outer):
+        logger.warning(f'you are trying to reconstruct {np.count_nonzero(abs(coords.r) > r_outer)} '
+                       f'data points outside rOuter. You can do it, but the futher away'
+                       'from rOuter you get the less you should trust this.')
+
+    n_order = int(np.sqrt(harmonics.shape[0])-1)
+    legendre_recon = generate_legendre_basis(coords, n_order)
+    if quantity == 'uT':  # field in uT, with A00 set to 0 (e.g. only looking at perturbation)
+        harmonics_temp = harmonics.copy()
+        harmonics_temp.A_0_0 = 0
+        Bz_recon = legendre_recon @ harmonics_temp
+        Bz_recon = Bz_recon * 1e6
+    elif quantity == 'T':  # raw field in T
+        Bz_recon = legendre_recon @ harmonics
+    else:
+        raise NotImplementedError(f'unknown reconstruction option entered: {quantity}')
+
+    return Bz_recon
+
+
+def compare_recon_report_with_ground_truth_report(ground_truth_report, recon_report, tolerance=1):  # pragma: no cover
+    """
+    This is to compare the distortion data contained within two Reports.MRI_QA_recon_reporter
+    objects. The original purpose was to compare a recon_report generated from direct data, and one
+    generated via harmonics, although in principle it can take any two reports.
+
+    :param ground_truth_report: Reports.MRI_QA_recon_reporter instance
+    :param recon_report: Reports.MRI_QA_recon_reporter instance
+    :param tolerance: tolerance in mm
+    """
+    # direct overlay of real versus recon
+    fig, axs = plt.subplots(nrows=2, ncols=2, figsize=[10, 10])
+    if ground_truth_report.r_outer == recon_report.r_outer:
+        # then use r_outer to filter the data
+        gt_data = ground_truth_report._extract_data_from_MatchedMarkerVolume(r_max=ground_truth_report.r_outer)
+        recon_data = recon_report._extract_data_from_MatchedMarkerVolume(r_max=recon_report.r_outer)
+    else:
+        gt_data = ground_truth_report._extract_data_from_MatchedMarkerVolume()
+        recon_data = recon_report._extract_data_from_MatchedMarkerVolume()
+
+    axs[0, 0].scatter(gt_data.r_gt, gt_data.abs_dis)
+    axs[0, 0].scatter(recon_data.r_gt, recon_data.abs_dis)
+    axs[0, 0].legend(['original_data', 'recon_data'])
+    axs[0, 0].set_xlabel('r [mm]')
+    axs[0, 0].set_ylabel('absolute distortion [mm]')
+
+    # scatter of real versus recon
+    axs[0, 1].scatter(gt_data.abs_dis, recon_data.abs_dis)
+    axs[0, 1].set_xlabel('original data')
+    axs[0, 1].set_ylabel('recon data')
+
+    # box plot of errors
+    error = gt_data.abs_dis - recon_data.abs_dis
+    axs[1, 0].boxplot(error)
+    axs[1, 0].set_ylabel('recon error [mm]')
+
+
+    # get index of outliers
+    outliers_ind = error > tolerance
+    print(f'{np.count_nonzero(outliers_ind)} outliers exist, at index {np.where(outliers_ind)}')
+    outliers_ind = np.where(outliers_ind)
+    for ind in outliers_ind[0]:
+        print(f'index {ind} is at {gt_data.x_gt.iloc[ind]: 1.1f},'
+              f' {gt_data.y_gt.iloc[ind]: 1.1f},'
+              f' {gt_data.z_gt.iloc[ind]: 1.1f}  the value in the ground truth is'
+              f' {gt_data.abs_dis.iloc[ind]: 1.1f}'
+              f' and the value in the reconstructed is {recon_data.abs_dis.iloc[ind]: 1.1f}')
+
+
+def enumerate_subfolders(data_loc):
+    """
+    A simple function that prints all the subfolders in data_loc as a dict, e.g.
+
+    {'1': 'folder1',
+     '2': 'folder2'} etc
+
+    I find this is a useful to create a dict object that I copy to the start of my analysis scripts
+    """
+    data_dict = {}
+    subfolders = [ f.path for f in os.scandir(data_loc) if f.is_dir() ]
+    for i, dir in enumerate(subfolders):
+        folder_name = os.path.split(dir)[1]
+        data_dict[str(i)] = folder_name
+    for key in data_dict.keys():
+        print(f"'{key}': '{data_dict[key]}',")
+
+
+def plot_MarkerVolume_overlay(MarkerVolumeList, legend=None):  # pragma: no cover
+    """
+    Plot overlaid 3D scatter plots of the marker positions in each MarkerVolume
+
+    :param MarkerVolumeList: list of MarkerVolume instances
+    :param legend: legend to display on plot
+    :return: None
+    """
+
+    assert isinstance(MarkerVolumeList, list)
+
+    fig = plt.figure()
+    axs = fig.add_subplot(111, projection='3d')
+    for MarkerVolume in MarkerVolumeList:
+        axs.scatter(MarkerVolume.MarkerCentroids.x, MarkerVolume.MarkerCentroids.y, MarkerVolume.MarkerCentroids.z)
+        axs.set_xlabel('X [mm]')
+        axs.set_ylabel('Y [mm]')
+        axs.set_zlabel('Z [mm]')
+        axs.set_title('3D marker positions')
+    axs.set_box_aspect((np.ptp(MarkerVolume.MarkerCentroids.x),
+                        np.ptp(MarkerVolume.MarkerCentroids.y),
+                        np.ptp(MarkerVolume.MarkerCentroids.z)))
+    if legend:
+        plt.legend(legend)
+    plt.show()
+
+
+def plot_compressed_MarkerVolumes(MarkerVolumeList, z_max=20, z_min=-20, title=None, legend=None): # pragma: no cover
+    """
+    plot overlay of compressed marker volumes (z coord is ignored)
+
+    :param MarkerVolumeList:  list of MarkerVolume instances
+    :type MarkerVolumeList: list
+    :param z_max: max z data to include
+    :type z_max: float, optional
+    :param z_min: min z data to include
+    :type z_min: float, optional
+    :param title: title of plot
+    :type title: str, optional
+    :param legend: legend of plot
+    :type legend: list, optional
+    :return: None
+    """
+
+    fig, axs = plt.subplots(figsize=[8, 8], ncols=1, nrows=1)
+    for MarkerVolume in MarkerVolumeList:
+        data_ind = np.logical_and(MarkerVolume.MarkerCentroids.z > z_min, MarkerVolume.MarkerCentroids.z < z_max)
+        plot_data = MarkerVolume.MarkerCentroids[data_ind]
+        axs.scatter(plot_data.x, plot_data.y)
+        axs.set_xlim([-150, 150])
+        axs.set_ylim([-150, 150])
+        axs.set_xlabel('x [mm]', fontsize=15)
+        axs.set_ylabel('y [mm]', fontsize=15)
+        axs.tick_params(axis='both', which='major', labelsize=12)
+        axs.tick_params(axis='both', which='minor', labelsize=12)
+        axs.axis("equal")
+        axs.grid()
+        plt.subplots_adjust(bottom=0.25)
+        if legend:
+            plt.legend(legend)
+        if title:
+            plt.title(title)
+
+
+def plot_matched_volume_hist(VolumeList, legend=None):
+    """
+    create a histogram of total distortion for all input volumes
+
+    :param VolumeList: a list of [matched marker volumes](https://acrf-image-x-institute.github.io/MRI_DistortionQA/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes)
+    :type VolumeList: list
+    :param legend: legend to print
+    :type legend: list, optional
+    :return: None
+    """
+    bins = np.linspace(0, 10, 30)
+    plt.figure()
+    for marker_volume in VolumeList:
+        plt.hist(marker_volume.MatchedCentroids.match_distance, bins=bins, alpha=0.5)
+    if legend:
+        plt.legend(['original', 'corrected'])
+    plt.xlabel('distortion [mm]')
+    plt.tight_layout()
+    plt.show()
+
+
+def plot_distortion_xyz_hist(MatchedMarkerVolume):
+    """
+    plot overlaid x, y, z distortion for an input instance of
+    [MatchedMarkerVolume](https://acrf-image-x-institute.github.io/MRI_DistortionQA/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes)
+
+    :param MatchedMarkerVolume: an instance of MatchedMarkerVolumes
+    """
+
+    x_dis = MatchedMarkerVolume.MatchedCentroids.x_gt - MatchedMarkerVolume.MatchedCentroids.x_gnl
+    y_dis = MatchedMarkerVolume.MatchedCentroids.y_gt - MatchedMarkerVolume.MatchedCentroids.y_gnl
+    z_dis = MatchedMarkerVolume.MatchedCentroids.z_gt - MatchedMarkerVolume.MatchedCentroids.z_gnl
+
+    plt.figure()
+    bins = np.linspace(0, 10, 30)
+    plt.hist(abs(x_dis), bins=bins, alpha=0.5)
+    plt.hist(abs(y_dis), bins=bins, alpha=0.5)
+    plt.hist(abs(z_dis), bins=bins, alpha=0.5)
+    plt.legend(['x', 'y', 'z'])
+    plt.xlabel('distortion [mm]')
+    plt.show()
+
+
+def print_dict(dict):
+    """
+    just provides a nicer display of the input dict than the default print function,
+    got sick of writing the same code over and over...
+    """
+    for key in dict.keys():
+        print(f'{key}: {dict[key]}')
+
```

### Comparing `mri_distortion_toolkit-0.14.1/mri_distortion_toolkit.egg-info/PKG-INFO` & `mri_distortion_toolkit-0.9.0/mri_distortion_toolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-Metadata-Version: 2.1
-Name: mri-distortion-toolkit
-Version: 0.14.1
-Summary: Quality assurance tools for MRI geometric distortion
-Home-page: https://acrf-image-x-institute.github.io/mri_distortion_toolkit/index.html
-Author: Brendan Whelan, Paul Liu, Shanshan Shan
-Author-email: bwheelz360@gmail.com
-Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/mri_distortion_toolkit
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
-# mri_distortion_toolkit  
-[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/mri_distortion_toolkit) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)[![PyPI version](https://badge.fury.io/py/mri_distortion_toolkit.svg)](https://badge.fury.io/py/mri_distortion_toolkit)
-
-This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging.
-
-The workflow steps are below. All steps have well defined input/output so you can use any part of this code independently from the other parts. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
-
-```mermaid
-flowchart LR
-
-AA[Phantom Design]
-
-A[Marker <br>Extraction]--->B[Marker <br>Matching]
-B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
-C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
-D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
-D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
-
-click AA "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/phantom_notes.html"
-click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_extraction.html"
-click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/marker_matching.html"
-click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/field_calculation.html"
-click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/fit_spherical_harmonics.html"
-click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/reporting.html"
-```
-
-
-
-## Setup/Build/Install
-
-```bash
-pip install mri_distortion_toolkit
-```
-
-## Usage
-
-Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
-
-## Directory Structure
-
-- *docsrc* markdown/rst source documentation
-- *tests* test cases
-- *mri_distortion_toolkit* source code 
-- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
+Metadata-Version: 2.1
+Name: mri-distortion-toolkit
+Version: 0.9.0
+Summary: Quality assurance tools for MRI geometric distortion
+Home-page: https://acrf-image-x-institute.github.io/mri_distortion_toolkit/index.html
+Author: Brendan Whelan, Paul Liu, Shanshan Shan
+Author-email: bwheelz360@gmail.com
+Project-URL: Bug Tracker, https://github.com/ACRF-Image-X-Institute/mri_distortion_toolkit
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
+# mri_distortion_toolkit  
+
+[![codecov](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA/branch/main/graph/badge.svg?token=3MCT7S6KVK)](https://codecov.io/gh/ACRF-Image-X-Institute/MRI_DistortionQA) ![](docsrc/__resources/interrogate.svg)  ![tests](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/run_tests.yml/badge.svg) ![docs](https://github.com/ACRF-Image-X-Institute/MRI_DistortionQA/actions/workflows/build_docs.yml/badge.svg)
+
+This code enables characterization, reporting, and correction of geometric distortion in Magnetic Resonance Imaging. 
+
+For the measurement of such distortions, see [here](https://github.com/ACRF-Image-X-Institute/MRI_DistortionPhantom). 
+
+The workflow steps are below, but all steps have well defined input/output so you can use any part of this code independently from the other parts. For a tutorial on each step, click on the diagram below. For an example of our automated reporting template see [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/_static/MR_QA_report_20_05_2022.html)
+
+```mermaid
+flowchart LR
+    A[Marker <br>Extraction]--->B[Marker <br>Matching]
+    B[Marker <br>Matching]--->C[Field <br> Calculation] & E[Automated <br>reporting]
+    C[Field <br> Calculation]-->D[Spherical Harmonic <br>Analysis]
+    D[Spherical Harmonic <br>Analysis]-->E[Automated <br>reporting];
+    D[Spherical Harmonic <br>Analysis]-->F[Distortion Correction]
+
+    click A "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MarkerVolume"
+    click B "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.MarkerAnalysis.MatchedMarkerVolumes"
+    click C "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldCalculation.ConvertMatchedMarkersToBz"
+    click D "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.FieldAnalysis.SphericalHarmonicFit"
+    click E "https://acrf-image-x-institute.github.io/mri_distortion_toolkit/code_docs.html#MRI_DistortionQA.Reports.MRI_QA_Reporter"
+
+```
+
+## Setup/Build/Install
+
+```bash
+pip install mri_distortion_toolkit
+```
+
+
+## Usage
+
+Detailed documentation is [here](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/).
+
+## Directory Structure
+
+- *docsrc* markdown/rst source documentation
+- *tests* test cases
+- *MRI_DistortionQA* source code
+- *examples* source code for the [worked examples](https://acrf-image-x-institute.github.io/mri_distortion_toolkit/examples.html)
```

### Comparing `mri_distortion_toolkit-0.14.1/setup.cfg` & `mri_distortion_toolkit-0.9.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,80 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 6d72 695f 6469 7374 6f72 7469 6f6e  = mri_distortion
-00000020: 5f74 6f6f 6c6b 6974 0a61 7574 686f 7220  _toolkit.author 
-00000030: 3d20 4272 656e 6461 6e20 5768 656c 616e  = Brendan Whelan
-00000040: 2c20 5061 756c 204c 6975 2c20 5368 616e  , Paul Liu, Shan
-00000050: 7368 616e 2053 6861 6e0a 6175 7468 6f72  shan Shan.author
-00000060: 5f65 6d61 696c 203d 2062 7768 6565 6c7a  _email = bwheelz
-00000070: 3336 3040 676d 6169 6c2e 636f 6d0a 6c69  360@gmail.com.li
-00000080: 6365 6e73 655f 6669 6c65 7320 3d20 4c49  cense_files = LI
-00000090: 4345 4e53 452e 6d64 0a76 6572 7369 6f6e  CENSE.md.version
-000000a0: 203d 2061 7474 723a 206d 7269 5f64 6973   = attr: mri_dis
-000000b0: 746f 7274 696f 6e5f 746f 6f6c 6b69 742e  tortion_toolkit.
-000000c0: 5f5f 7665 7273 696f 6e5f 5f0a 6465 7363  __version__.desc
-000000d0: 7269 7074 696f 6e20 3d20 5175 616c 6974  ription = Qualit
-000000e0: 7920 6173 7375 7261 6e63 6520 746f 6f6c  y assurance tool
-000000f0: 7320 666f 7220 4d52 4920 6765 6f6d 6574  s for MRI geomet
-00000100: 7269 6320 6469 7374 6f72 7469 6f6e 0a6c  ric distortion.l
-00000110: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description 
-00000120: 3d20 6669 6c65 3a20 5245 4144 4d45 2e6d  = file: README.m
-00000130: 640a 6c6f 6e67 5f64 6573 6372 6970 7469  d.long_descripti
-00000140: 6f6e 5f63 6f6e 7465 6e74 5f74 7970 6520  on_content_type 
-00000150: 3d20 7465 7874 2f6d 6172 6b64 6f77 6e0a  = text/markdown.
-00000160: 7572 6c20 3d20 6874 7470 733a 2f2f 6163  url = https://ac
-00000170: 7266 2d69 6d61 6765 2d78 2d69 6e73 7469  rf-image-x-insti
-00000180: 7475 7465 2e67 6974 6875 622e 696f 2f6d  tute.github.io/m
-00000190: 7269 5f64 6973 746f 7274 696f 6e5f 746f  ri_distortion_to
-000001a0: 6f6c 6b69 742f 696e 6465 782e 6874 6d6c  olkit/index.html
-000001b0: 0a70 726f 6a65 6374 5f75 726c 7320 3d20  .project_urls = 
-000001c0: 0a09 4275 6720 5472 6163 6b65 7220 3d20  ..Bug Tracker = 
-000001d0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001e0: 6f6d 2f41 4352 462d 496d 6167 652d 582d  om/ACRF-Image-X-
-000001f0: 496e 7374 6974 7574 652f 6d72 695f 6469  Institute/mri_di
-00000200: 7374 6f72 7469 6f6e 5f74 6f6f 6c6b 6974  stortion_toolkit
-00000210: 0a63 6c61 7373 6966 6965 7273 203d 200a  .classifiers = .
-00000220: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000230: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000240: 3a3a 2033 0a09 4c69 6365 6e73 6520 3a3a  :: 3..License ::
-00000250: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
-00000260: 2047 4e55 2047 656e 6572 616c 2050 7562   GNU General Pub
-00000270: 6c69 6320 4c69 6365 6e73 6520 7633 2028  lic License v3 (
-00000280: 4750 4c76 3329 0a0a 5b6f 7074 696f 6e73  GPLv3)..[options
-00000290: 5d0a 7061 636b 6167 655f 6469 7220 3d20  ].package_dir = 
-000002a0: 0a09 3d20 2e0a 7061 636b 6167 6573 203d  ..= ..packages =
-000002b0: 206d 7269 5f64 6973 746f 7274 696f 6e5f   mri_distortion_
-000002c0: 746f 6f6c 6b69 742c 206d 7269 5f64 6973  toolkit, mri_dis
-000002d0: 746f 7274 696f 6e5f 746f 6f6c 6b69 742e  tortion_toolkit.
-000002e0: 6a69 6e6a 615f 7465 6d70 6c61 7465 732c  jinja_templates,
-000002f0: 206d 7269 5f64 6973 746f 7274 696f 6e5f   mri_distortion_
-00000300: 746f 6f6c 6b69 742e 6a69 6e6a 615f 7465  toolkit.jinja_te
-00000310: 6d70 6c61 7465 732e 7468 656d 6573 0a69  mplates.themes.i
-00000320: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000330: 6174 6120 3d20 5472 7565 0a70 7974 686f  ata = True.pytho
-00000340: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000350: 2e38 0a69 6e73 7461 6c6c 5f72 6571 7569  .8.install_requi
-00000360: 7265 7320 3d20 0a09 6e75 6d70 790a 0973  res = ..numpy..s
-00000370: 6369 7079 0a09 7363 696b 6974 2d69 6d61  cipy..scikit-ima
-00000380: 6765 0a09 6d61 7470 6c6f 746c 6962 0a09  ge..matplotlib..
-00000390: 7079 6469 636f 6d0a 0970 616e 6461 730a  pydicom..pandas.
-000003a0: 0973 6561 626f 726e 0a09 706c 6f74 6c79  .seaborn..plotly
-000003b0: 0a09 6a69 6e6a 6132 0a09 6669 6e75 6666  ..jinja2..finuff
-000003c0: 740a 0a5b 6f70 7469 6f6e 732e 7061 636b  t..[options.pack
-000003d0: 6167 655f 6461 7461 5d0a 2a20 3d20 2a2e  age_data].* = *.
-000003e0: 6874 6d6c 2c20 2a2e 6d64 2c20 2a2e 6373  html, *.md, *.cs
-000003f0: 730a 6d72 695f 6469 7374 6f72 7469 6f6e  s.mri_distortion
-00000400: 5f74 6f6f 6c6b 6974 2e6a 696e 6a61 5f74  _toolkit.jinja_t
-00000410: 656d 706c 6174 6573 203d 202a 2e68 746d  emplates = *.htm
-00000420: 6c0a 6d72 695f 6469 7374 6f72 7469 6f6e  l.mri_distortion
-00000430: 5f74 6f6f 6c6b 6974 2e6a 696e 6a61 5f74  _toolkit.jinja_t
-00000440: 656d 706c 6174 6573 2e74 6865 6d65 7320  emplates.themes 
-00000450: 3d20 2a2e 6373 732c 202a 2e6d 640a 0a5b  = *.css, *.md..[
-00000460: 746f 6f6c 3a69 6e74 6572 726f 6761 7465  tool:interrogate
-00000470: 5d0a 6967 6e6f 7265 2d69 6e69 742d 6d65  ].ignore-init-me
-00000480: 7468 6f64 203d 2074 7275 650a 6967 6e6f  thod = true.igno
-00000490: 7265 2d6d 6f64 756c 6520 3d20 7472 7565  re-module = true
-000004a0: 0a66 6169 6c2d 756e 6465 7220 3d20 3935  .fail-under = 95
-000004b0: 0a0a 5b65 6767 5f69 6e66 6f5d 0a74 6167  ..[egg_info].tag
-000004c0: 5f62 7569 6c64 203d 200a 7461 675f 6461  _build = .tag_da
-000004d0: 7465 203d 2030 0a0a                      te = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 206d 7269 5f64 6973 746f 7274 696f   = mri_distortio
+00000020: 6e5f 746f 6f6c 6b69 740d 0a61 7574 686f  n_toolkit..autho
+00000030: 7220 3d20 4272 656e 6461 6e20 5768 656c  r = Brendan Whel
+00000040: 616e 2c20 5061 756c 204c 6975 2c20 5368  an, Paul Liu, Sh
+00000050: 616e 7368 616e 2053 6861 6e0d 0a61 7574  anshan Shan..aut
+00000060: 686f 725f 656d 6169 6c20 3d20 6277 6865  hor_email = bwhe
+00000070: 656c 7a33 3630 4067 6d61 696c 2e63 6f6d  elz360@gmail.com
+00000080: 0d0a 6c69 6365 6e73 655f 6669 6c65 7320  ..license_files 
+00000090: 3d20 4c49 4345 4e53 452e 6d64 0d0a 7665  = LICENSE.md..ve
+000000a0: 7273 696f 6e20 3d20 6174 7472 3a20 6d72  rsion = attr: mr
+000000b0: 695f 6469 7374 6f72 7469 6f6e 5f74 6f6f  i_distortion_too
+000000c0: 6c6b 6974 2e5f 5f76 6572 7369 6f6e 5f5f  lkit.__version__
+000000d0: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
+000000e0: 5175 616c 6974 7920 6173 7375 7261 6e63  Quality assuranc
+000000f0: 6520 746f 6f6c 7320 666f 7220 4d52 4920  e tools for MRI 
+00000100: 6765 6f6d 6574 7269 6320 6469 7374 6f72  geometric distor
+00000110: 7469 6f6e 0d0a 6c6f 6e67 5f64 6573 6372  tion..long_descr
+00000120: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000130: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+00000140: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+00000150: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+00000160: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+00000170: 7474 7073 3a2f 2f61 6372 662d 696d 6167  ttps://acrf-imag
+00000180: 652d 782d 696e 7374 6974 7574 652e 6769  e-x-institute.gi
+00000190: 7468 7562 2e69 6f2f 6d72 695f 6469 7374  thub.io/mri_dist
+000001a0: 6f72 7469 6f6e 5f74 6f6f 6c6b 6974 2f69  ortion_toolkit/i
+000001b0: 6e64 6578 2e68 746d 6c0d 0a70 726f 6a65  ndex.html..proje
+000001c0: 6374 5f75 726c 7320 3d20 0d0a 0942 7567  ct_urls = ...Bug
+000001d0: 2054 7261 636b 6572 203d 2068 7474 7073   Tracker = https
+000001e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4143  ://github.com/AC
+000001f0: 5246 2d49 6d61 6765 2d58 2d49 6e73 7469  RF-Image-X-Insti
+00000200: 7475 7465 2f6d 7269 5f64 6973 746f 7274  tute/mri_distort
+00000210: 696f 6e5f 746f 6f6c 6b69 740d 0a63 6c61  ion_toolkit..cla
+00000220: 7373 6966 6965 7273 203d 200d 0a09 5072  ssifiers = ...Pr
+00000230: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
+00000240: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
+00000250: 330d 0a09 4c69 6365 6e73 6520 3a3a 204f  3...License :: O
+00000260: 5349 2041 7070 726f 7665 6420 3a3a 2047  SI Approved :: G
+00000270: 4e55 2047 656e 6572 616c 2050 7562 6c69  NU General Publi
+00000280: 6320 4c69 6365 6e73 6520 7633 2028 4750  c License v3 (GP
+00000290: 4c76 3329 0d0a 0d0a 5b6f 7074 696f 6e73  Lv3)....[options
+000002a0: 5d0d 0a70 6163 6b61 6765 5f64 6972 203d  ]..package_dir =
+000002b0: 200d 0a09 3d20 2e0d 0a70 6163 6b61 6765   ...= ...package
+000002c0: 7320 3d20 6d72 695f 6469 7374 6f72 7469  s = mri_distorti
+000002d0: 6f6e 5f74 6f6f 6c6b 6974 2c20 6d72 695f  on_toolkit, mri_
+000002e0: 6469 7374 6f72 7469 6f6e 5f74 6f6f 6c6b  distortion_toolk
+000002f0: 6974 2e6a 696e 6a61 5f74 656d 706c 6174  it.jinja_templat
+00000300: 6573 2c20 6d72 695f 6469 7374 6f72 7469  es, mri_distorti
+00000310: 6f6e 5f74 6f6f 6c6b 6974 2e6a 696e 6a61  on_toolkit.jinja
+00000320: 5f74 656d 706c 6174 6573 2e74 6865 6d65  _templates.theme
+00000330: 730d 0a69 6e63 6c75 6465 5f70 6163 6b61  s..include_packa
+00000340: 6765 5f64 6174 6120 3d20 5472 7565 0d0a  ge_data = True..
+00000350: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
+00000360: 3d20 3e3d 332e 380d 0a69 6e73 7461 6c6c  = >=3.8..install
+00000370: 5f72 6571 7569 7265 7320 3d20 0d0a 096e  _requires = ...n
+00000380: 756d 7079 0d0a 0973 6369 7079 0d0a 0973  umpy...scipy...s
+00000390: 6369 6b69 742d 696d 6167 650d 0a09 6d61  cikit-image...ma
+000003a0: 7470 6c6f 746c 6962 0d0a 0970 7964 6963  tplotlib...pydic
+000003b0: 6f6d 0d0a 0970 616e 6461 730d 0a09 7365  om...pandas...se
+000003c0: 6162 6f72 6e0d 0a09 706c 6f74 6c79 0d0a  aborn...plotly..
+000003d0: 096a 696e 6a61 320d 0a0d 0a5b 6f70 7469  .jinja2....[opti
+000003e0: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+000003f0: 5d0d 0a2a 203d 202a 2e68 746d 6c2c 202a  ]..* = *.html, *
+00000400: 2e6d 642c 202a 2e63 7373 0d0a 6d72 695f  .md, *.css..mri_
+00000410: 6469 7374 6f72 7469 6f6e 5f74 6f6f 6c6b  distortion_toolk
+00000420: 6974 2e6a 696e 6a61 5f74 656d 706c 6174  it.jinja_templat
+00000430: 6573 203d 202a 2e68 746d 6c0d 0a6d 7269  es = *.html..mri
+00000440: 5f64 6973 746f 7274 696f 6e5f 746f 6f6c  _distortion_tool
+00000450: 6b69 742e 6a69 6e6a 615f 7465 6d70 6c61  kit.jinja_templa
+00000460: 7465 732e 7468 656d 6573 203d 202a 2e63  tes.themes = *.c
+00000470: 7373 2c20 2a2e 6d64 0d0a 0d0a 5b74 6f6f  ss, *.md....[too
+00000480: 6c3a 696e 7465 7272 6f67 6174 655d 0d0a  l:interrogate]..
+00000490: 6967 6e6f 7265 2d69 6e69 742d 6d65 7468  ignore-init-meth
+000004a0: 6f64 203d 2074 7275 650d 0a69 676e 6f72  od = true..ignor
+000004b0: 652d 6d6f 6475 6c65 203d 2074 7275 650d  e-module = true.
+000004c0: 0a66 6169 6c2d 756e 6465 7220 3d20 3935  .fail-under = 95
+000004d0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000004e0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+000004f0: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

