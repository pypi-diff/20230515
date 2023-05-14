# Comparing `tmp/ragas-0.0.1a6.tar.gz` & `tmp/ragas-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragas-0.0.1a6.tar", last modified: Sun May 14 19:24:19 2023, max compression
+gzip compressed data, was "ragas-0.0.1a7.tar", last modified: Sun May 14 22:03:46 2023, max compression
```

## Comparing `ragas-0.0.1a6.tar` & `ragas-0.0.1a7.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.849377 ragas-0.0.1a6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-14 19:24:02.000000 ragas-0.0.1a6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 19:24:02.000000 ragas-0.0.1a6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-14 19:24:02.000000 ragas-0.0.1a6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 19:24:19.857377 ragas-0.0.1a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-14 19:24:02.000000 ragas-0.0.1a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-14 19:24:02.000000 ragas-0.0.1a6/docs/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 19:24:02.000000 ragas-0.0.1a6/examples/data_prep.py
--rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-05-14 19:24:02.000000 ragas-0.0.1a6/examples/quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-14 19:24:02.000000 ragas-0.0.1a6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/ragas/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/ragas/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/factual.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/metrics/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 19:24:02.000000 ragas-0.0.1a6/ragas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/ragas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 19:24:19.000000 ragas-0.0.1a6/ragas.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 19:24:02.000000 ragas-0.0.1a6/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 19:24:02.000000 ragas-0.0.1a6/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 19:24:19.857377 ragas-0.0.1a6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.853377 ragas-0.0.1a6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/benchmarks/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/benchmarks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 19:24:19.857377 ragas-0.0.1a6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 19:24:02.000000 ragas-0.0.1a6/tests/unit/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.796328 ragas-0.0.1a7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-14 22:03:31.000000 ragas-0.0.1a7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 22:03:31.000000 ragas-0.0.1a7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-14 22:03:31.000000 ragas-0.0.1a7/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-14 22:03:46.792328 ragas-0.0.1a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-05-14 22:03:31.000000 ragas-0.0.1a7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-14 22:03:31.000000 ragas-0.0.1a7/citations.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)    33956 2023-05-14 22:03:31.000000 ragas-0.0.1a7/docs/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-14 22:03:31.000000 ragas-0.0.1a7/examples/data_prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25111 2023-05-14 22:03:31.000000 ragas-0.0.1a7/examples/quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 22:03:31.000000 ragas-0.0.1a7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/factual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/metrics/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-14 22:03:31.000000 ragas-0.0.1a7/ragas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/ragas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-14 22:03:46.000000 ragas-0.0.1a7/ragas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-14 22:03:31.000000 ragas-0.0.1a7/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-14 22:03:31.000000 ragas-0.0.1a7/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 22:03:46.796328 ragas-0.0.1a7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.788328 ragas-0.0.1a7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/benchmarks/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/benchmarks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:03:46.792328 ragas-0.0.1a7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 22:03:31.000000 ragas-0.0.1a7/tests/unit/test_simple.py
```

### Comparing `ragas-0.0.1a6/.github/workflows/ci.yaml` & `ragas-0.0.1a7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/.github/workflows/python-publish.yml` & `ragas-0.0.1a7/.github/workflows/python-publish.yml`

 * *Files 8% similar despite different names*

```diff
@@ -26,16 +26,17 @@
     - name: Set up Python
       uses: actions/setup-python@v3
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install --upgrade setuptools
-        pip install --upgrade build
+        pip install --upgrade setuptools setuptools_scm[toml] build 
+    - name: get setuptools-scm version 
+      run: python -m setuptools_scm
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@27b31702a0e7fc50959f5ad993c78deac1bdfc29
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `ragas-0.0.1a6/.gitignore` & `ragas-0.0.1a7/.gitignore`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/LICENSE` & `ragas-0.0.1a7/LICENSE`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/Makefile` & `ragas-0.0.1a7/Makefile`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/docs/assets/logo.png` & `ragas-0.0.1a7/docs/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/examples/data_prep.py` & `ragas-0.0.1a7/examples/data_prep.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/examples/quickstart.ipynb` & `ragas-0.0.1a7/examples/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/ragas/metrics/base.py` & `ragas-0.0.1a7/ragas/metrics/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,15 +73,15 @@
                 assert isinstance(
                     generated_text, str
                 ), f"generated_text should be str but got {type(generated_text)}"
                 generated_texts = [generated_text] * split_indices
                 scores = metric.score(ground_truths, generated_texts)
                 score = np.max(scores)
 
-            row[f"{metric.name}_score"] = score
+            row[f"{metric.name}"] = score
 
         return row
 
 
 @dataclass
 class Result(dict):
     scores: Dataset
```

### Comparing `ragas-0.0.1a6/ragas/metrics/factual.py` & `ragas-0.0.1a7/ragas/metrics/factual.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from transformers import (
     AutoConfig,
     AutoModelForSequenceClassification,
     AutoTokenizer,
     PreTrainedModel,
 )
 
+from ragas.exceptions import RagasException
 from ragas.metrics import Metric
 from ragas.utils import device_check
 
 if t.TYPE_CHECKING:
     from torch import device as Device
 
 from transformers.models.auto.modeling_auto import (
@@ -205,20 +206,24 @@
     max_answers: int = 10
     crosscheck_candidates: bool = True
     load_single = False
     batch_size: int = 4
     include_nouns: bool = True
     save_results: bool = False
 
-    def __post_init__(
-        self,
-    ):
-        self.nlp = spacy.load(SPACY_MODEL)
+    def __post_init__(self):
         self.qa = QAGQ.from_pretrained(self.qa_model_name)
         self.qg = QAGQ.from_pretrained(self.qg_model_name)
+        try:
+            self.nlp = spacy.load(SPACY_MODEL)
+        except OSError:
+            raise RagasException(
+                f"Spacy model [{SPACY_MODEL}] not found. Please run "
+                "`python -m spacy download {SPACY_MODEL}` to install it."
+            )
 
     @property
     def name(self):
         return "Qsquare"
 
     @property
     def is_batchable(self):
```

### Comparing `ragas-0.0.1a6/ragas/metrics/similarity.py` & `ragas-0.0.1a7/ragas/metrics/similarity.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 import numpy as np
 from numpy.linalg import norm
 from sentence_transformers import SentenceTransformer
 
 from ragas.metrics.base import Metric
 
-if t.TYPE_CHECKING:
-    from torch import Tensor
-
 BERT_METRIC = t.Literal["cosine", "euclidean"]
 
 
 @dataclass
 class BERTScore(Metric):
     similarity_metric: t.Literal[BERT_METRIC] = "cosine"
     model_path: str = "all-MiniLM-L6-v2"
@@ -41,17 +38,19 @@
     ):
         gndtruth_emb = self.model.encode(
             ground_truth, batch_size=self.batch_size, convert_to_numpy=True
         )
         gentext_emb = self.model.encode(
             generated_text, batch_size=self.batch_size, convert_to_numpy=True
         )
-        assert isinstance(gentext_emb, Tensor) and isinstance(gndtruth_emb, Tensor), (
+        assert isinstance(gentext_emb, np.ndarray) and isinstance(
+            gndtruth_emb, np.ndarray
+        ), (
             f"Both gndtruth_emb[{type(gentext_emb)}], gentext_emb[{type(gentext_emb)}]"
-            " should be Tensor."
+            " should be numpy ndarray."
         )
 
         if self.similarity_metric == "cosine":
             score = np.dot(gndtruth_emb, gentext_emb.T) / (
                 norm(gndtruth_emb) * norm(gentext_emb)
             )
```

### Comparing `ragas-0.0.1a6/ragas/metrics/simple.py` & `ragas-0.0.1a7/ragas/metrics/simple.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/ragas/utils.py` & `ragas-0.0.1a7/ragas/utils.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/ragas.egg-info/SOURCES.txt` & `ragas-0.0.1a7/ragas.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 .gitignore
 LICENSE
 Makefile
 README.md
+citations.md
 pyproject.toml
 .github/workflows/ci.yaml
 .github/workflows/python-publish.yml
 docs/assets/logo.png
 examples/data_prep.py
 examples/quickstart.ipynb
 ragas/__init__.py
 ragas/_version.py
+ragas/exceptions.py
 ragas/utils.py
 ragas.egg-info/PKG-INFO
 ragas.egg-info/SOURCES.txt
 ragas.egg-info/dependency_links.txt
 ragas.egg-info/requires.txt
 ragas.egg-info/top_level.txt
 ragas/metrics/__init__.py
```

### Comparing `ragas-0.0.1a6/tests/benchmarks/benchmark.py` & `ragas-0.0.1a7/tests/benchmarks/benchmark.py`

 * *Files identical despite different names*

### Comparing `ragas-0.0.1a6/tests/benchmarks/utils.py` & `ragas-0.0.1a7/tests/benchmarks/utils.py`

 * *Files identical despite different names*

