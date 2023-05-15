# Comparing `tmp/ScandEval-7.0.0.tar.gz` & `tmp/ScandEval-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ScandEval-7.0.0.tar", max compression
+gzip compressed data, was "ScandEval-7.1.0.tar", max compression
```

## Comparing `ScandEval-7.0.0.tar` & `ScandEval-7.1.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 ScandEval-7.0.0/LICENSE
--rw-r--r--   0        0        0     6755 2023-05-13 14:10:06.419933 ScandEval-7.0.0/README.md
--rw-r--r--   0        0        0     1845 2023-05-13 14:10:46.963356 ScandEval-7.0.0/pyproject.toml
--rw-r--r--   0        0        0      839 2023-05-13 13:56:49.238045 ScandEval-7.0.0/src/scandeval/__init__.py
--rw-r--r--   0        0        0     8919 2023-04-12 09:02:17.736254 ScandEval-7.0.0/src/scandeval/benchmark_config_factory.py
--rw-r--r--   0        0        0    28601 2023-05-13 13:50:06.250309 ScandEval-7.0.0/src/scandeval/benchmark_dataset.py
--rw-r--r--   0        0        0    17639 2023-04-12 09:02:17.736765 ScandEval-7.0.0/src/scandeval/benchmarker.py
--rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 ScandEval-7.0.0/src/scandeval/callbacks.py
--rw-r--r--   0        0        0     6661 2023-04-12 09:02:17.736945 ScandEval-7.0.0/src/scandeval/cli.py
--rw-r--r--   0        0        0     6035 2023-04-12 09:02:17.737107 ScandEval-7.0.0/src/scandeval/config.py
--rw-r--r--   0        0        0     4962 2022-12-29 15:49:44.942921 ScandEval-7.0.0/src/scandeval/dataset_configs.py
--rw-r--r--   0        0        0     1920 2022-11-03 09:23:55.849427 ScandEval-7.0.0/src/scandeval/dataset_factory.py
--rw-r--r--   0        0        0     3352 2022-12-29 15:49:44.943265 ScandEval-7.0.0/src/scandeval/dataset_tasks.py
--rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 ScandEval-7.0.0/src/scandeval/exceptions.py
--rw-r--r--   0        0        0    12351 2023-02-22 12:37:31.608038 ScandEval-7.0.0/src/scandeval/hf_hub.py
--rw-r--r--   0        0        0     7946 2022-07-14 15:19:22.963227 ScandEval-7.0.0/src/scandeval/languages.py
--rw-r--r--   0        0        0    16518 2023-05-13 13:57:46.801269 ScandEval-7.0.0/src/scandeval/model_loading.py
--rw-r--r--   0        0        0    15045 2023-03-10 17:33:33.955970 ScandEval-7.0.0/src/scandeval/named_entity_recognition.py
--rw-r--r--   0        0        0    14150 2023-04-12 09:02:17.737732 ScandEval-7.0.0/src/scandeval/question_answering.py
--rw-r--r--   0        0        0    11733 2022-12-24 12:57:14.794624 ScandEval-7.0.0/src/scandeval/question_answering_trainer.py
--rw-r--r--   0        0        0     4692 2022-12-29 15:49:44.943541 ScandEval-7.0.0/src/scandeval/scores.py
--rw-r--r--   0        0        0     3899 2022-12-24 12:57:14.794885 ScandEval-7.0.0/src/scandeval/sequence_classification.py
--rw-r--r--   0        0        0     5812 2023-04-12 09:02:17.737892 ScandEval-7.0.0/src/scandeval/speed_benchmark.py
--rw-r--r--   0        0        0      163 2022-11-03 09:23:55.851896 ScandEval-7.0.0/src/scandeval/types.py
--rw-r--r--   0        0        0     9001 2023-05-13 13:57:24.239401 ScandEval-7.0.0/src/scandeval/utils.py
--rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 ScandEval-7.0.0/setup.py
--rw-r--r--   0        0        0     8243 1970-01-01 00:00:00.000000 ScandEval-7.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-01-26 21:11:58.574218 ScandEval-7.1.0/LICENSE
+-rw-r--r--   0        0        0     6755 2023-05-13 14:13:06.300002 ScandEval-7.1.0/README.md
+-rw-r--r--   0        0        0     1845 2023-05-15 13:06:56.154168 ScandEval-7.1.0/pyproject.toml
+-rw-r--r--   0        0        0      839 2023-05-13 13:56:49.238045 ScandEval-7.1.0/src/scandeval/__init__.py
+-rw-r--r--   0        0        0     8919 2023-04-12 09:02:17.736254 ScandEval-7.1.0/src/scandeval/benchmark_config_factory.py
+-rw-r--r--   0        0        0    28601 2023-05-13 13:50:06.250309 ScandEval-7.1.0/src/scandeval/benchmark_dataset.py
+-rw-r--r--   0        0        0    17639 2023-04-12 09:02:17.736765 ScandEval-7.1.0/src/scandeval/benchmarker.py
+-rw-r--r--   0        0        0     1382 2022-11-03 09:23:55.848473 ScandEval-7.1.0/src/scandeval/callbacks.py
+-rw-r--r--   0        0        0     6661 2023-04-12 09:02:17.736945 ScandEval-7.1.0/src/scandeval/cli.py
+-rw-r--r--   0        0        0     6035 2023-04-12 09:02:17.737107 ScandEval-7.1.0/src/scandeval/config.py
+-rw-r--r--   0        0        0     4962 2022-12-29 15:49:44.942921 ScandEval-7.1.0/src/scandeval/dataset_configs.py
+-rw-r--r--   0        0        0     1920 2022-11-03 09:23:55.849427 ScandEval-7.1.0/src/scandeval/dataset_factory.py
+-rw-r--r--   0        0        0     3352 2022-12-29 15:49:44.943265 ScandEval-7.1.0/src/scandeval/dataset_tasks.py
+-rw-r--r--   0        0        0      650 2022-07-22 11:05:37.491231 ScandEval-7.1.0/src/scandeval/exceptions.py
+-rw-r--r--   0        0        0    12351 2023-02-22 12:37:31.608038 ScandEval-7.1.0/src/scandeval/hf_hub.py
+-rw-r--r--   0        0        0     7946 2022-07-14 15:19:22.963227 ScandEval-7.1.0/src/scandeval/languages.py
+-rw-r--r--   0        0        0    17159 2023-05-15 13:06:18.166268 ScandEval-7.1.0/src/scandeval/model_loading.py
+-rw-r--r--   0        0        0    15045 2023-03-10 17:33:33.955970 ScandEval-7.1.0/src/scandeval/named_entity_recognition.py
+-rw-r--r--   0        0        0    29225 2023-05-15 13:06:18.166623 ScandEval-7.1.0/src/scandeval/norbert.py
+-rw-r--r--   0        0        0    14150 2023-04-12 09:02:17.737732 ScandEval-7.1.0/src/scandeval/question_answering.py
+-rw-r--r--   0        0        0    11733 2022-12-24 12:57:14.794624 ScandEval-7.1.0/src/scandeval/question_answering_trainer.py
+-rw-r--r--   0        0        0     4692 2022-12-29 15:49:44.943541 ScandEval-7.1.0/src/scandeval/scores.py
+-rw-r--r--   0        0        0     3899 2022-12-24 12:57:14.794885 ScandEval-7.1.0/src/scandeval/sequence_classification.py
+-rw-r--r--   0        0        0     5812 2023-04-12 09:02:17.737892 ScandEval-7.1.0/src/scandeval/speed_benchmark.py
+-rw-r--r--   0        0        0      163 2022-11-03 09:23:55.851896 ScandEval-7.1.0/src/scandeval/types.py
+-rw-r--r--   0        0        0     9001 2023-05-13 13:57:24.239401 ScandEval-7.1.0/src/scandeval/utils.py
+-rw-r--r--   0        0        0     8623 1970-01-01 00:00:00.000000 ScandEval-7.1.0/setup.py
+-rw-r--r--   0        0        0     8243 1970-01-01 00:00:00.000000 ScandEval-7.1.0/PKG-INFO
```

### Comparing `ScandEval-7.0.0/LICENSE` & `ScandEval-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/README.md` & `ScandEval-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/pyproject.toml` & `ScandEval-7.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ScandEval"
-version = "7.0.0"
+version = "7.1.0"
 description = "Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks."
 authors = ["Dan Saattrup Nielsen <saattrupdan@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://scandeval.github.io"
 repository = "https://github.com/saattrupdan/ScandEval"
```

### Comparing `ScandEval-7.0.0/src/scandeval/__init__.py` & `ScandEval-7.1.0/src/scandeval/__init__.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/benchmark_config_factory.py` & `ScandEval-7.1.0/src/scandeval/benchmark_config_factory.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/benchmark_dataset.py` & `ScandEval-7.1.0/src/scandeval/benchmark_dataset.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/benchmarker.py` & `ScandEval-7.1.0/src/scandeval/benchmarker.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/callbacks.py` & `ScandEval-7.1.0/src/scandeval/callbacks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/cli.py` & `ScandEval-7.1.0/src/scandeval/cli.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/config.py` & `ScandEval-7.1.0/src/scandeval/config.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/dataset_configs.py` & `ScandEval-7.1.0/src/scandeval/dataset_configs.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/dataset_factory.py` & `ScandEval-7.1.0/src/scandeval/dataset_factory.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/dataset_tasks.py` & `ScandEval-7.1.0/src/scandeval/dataset_tasks.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/exceptions.py` & `ScandEval-7.1.0/src/scandeval/exceptions.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/hf_hub.py` & `ScandEval-7.1.0/src/scandeval/hf_hub.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/languages.py` & `ScandEval-7.1.0/src/scandeval/languages.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/model_loading.py` & `ScandEval-7.1.0/src/scandeval/model_loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     XLMRobertaForQuestionAnswering,
     XLMRobertaForSequenceClassification,
     XLMRobertaForTokenClassification,
 )
 from transformers.tokenization_utils import PreTrainedTokenizer
 
 from .exceptions import InvalidBenchmark
+from .norbert import load_norbert_model
 from .utils import block_terminal_output, get_class_by_name
 
 
 def load_model(
     model_id: str,
     revision: str,
     supertask: str,
@@ -93,14 +94,29 @@
                     num_labels=num_labels,
                     id2label=id2label,
                     label2id=label2id,
                     cache_dir=cache_dir,
                 )
                 model = model_cls(config)
 
+            # Special handling of NorBERT3 models, as they are not included in the
+            # `transformers` library yet
+            elif "norbert3" in model_id:
+                model = load_norbert_model(
+                    model_id=model_id,
+                    revision=revision,
+                    supertask=supertask,
+                    num_labels=num_labels,
+                    id2label=id2label,
+                    label2id=label2id,
+                    from_flax=from_flax,
+                    use_auth_token=use_auth_token,
+                    cache_dir=cache_dir,
+                )
+
             # Otherwise load the pretrained model
             else:
                 try:
                     config = AutoConfig.from_pretrained(
                         model_id,
                         revision=revision,
                         use_auth_token=use_auth_token,
```

### Comparing `ScandEval-7.0.0/src/scandeval/named_entity_recognition.py` & `ScandEval-7.1.0/src/scandeval/named_entity_recognition.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/question_answering.py` & `ScandEval-7.1.0/src/scandeval/question_answering.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/question_answering_trainer.py` & `ScandEval-7.1.0/src/scandeval/question_answering_trainer.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/scores.py` & `ScandEval-7.1.0/src/scandeval/scores.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/sequence_classification.py` & `ScandEval-7.1.0/src/scandeval/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/speed_benchmark.py` & `ScandEval-7.1.0/src/scandeval/speed_benchmark.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/src/scandeval/utils.py` & `ScandEval-7.1.0/src/scandeval/utils.py`

 * *Files identical despite different names*

### Comparing `ScandEval-7.0.0/setup.py` & `ScandEval-7.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'transformers>=4.20.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['scandeval = scandeval.cli:benchmark']}
 
 setup_kwargs = {
     'name': 'scandeval',
-    'version': '7.0.0',
+    'version': '7.1.0',
     'description': 'Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.',
     'long_description': '<div align=\'center\'>\n<img src="https://raw.githubusercontent.com/saattrupdan/ScandEval/main/gfx/scandeval.png" width="517" height="217">\n</div>\n\n### Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.\n\n______________________________________________________________________\n[![PyPI Status](https://badge.fury.io/py/scandeval.svg)](https://pypi.org/project/scandeval/)\n[![Paper](https://img.shields.io/badge/arXiv-2304.00906-b31b1b.svg)](https://arxiv.org/abs/2304.00906)\n[![License](https://img.shields.io/github/license/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/blob/main/LICENSE)\n[![LastCommit](https://img.shields.io/github/last-commit/saattrupdan/ScandEval)](https://github.com/saattrupdan/ScandEval/commits/main)\n[![Code Coverage](https://img.shields.io/badge/Coverage-76%25-yellowgreen.svg)](https://github.com/saattrupdan/ScandEval/tree/main/tests)\n[![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.0-4baaaa.svg)](https://github.com/saattrupdan/ScandEval/blob/main/CODE_OF_CONDUCT.md)\n\n\n## Installation\nTo install the package simply write the following command in your favorite terminal:\n```\n$ pip install scandeval\n```\n\n## Quickstart\n### Benchmarking from the Command Line\nThe easiest way to benchmark pretrained models is via the command line interface. After\nhaving installed the package, you can benchmark your favorite model like so:\n```\n$ scandeval --model-id <model-id>\n```\n\nHere `model_id` is the HuggingFace model ID, which can be found on the [HuggingFace\nHub](https://huggingface.co/models). By default this will benchmark the model on all\nthe datasets eligible. If you want to benchmark on a specific dataset, this can be done\nvia the `--dataset` flag. This will for instance evaluate the model on the\n`AngryTweets` dataset:\n```\n$ scandeval --model-id <model-id> --dataset angry-tweets\n```\n\nWe can also separate by language. To benchmark all Danish models on all Danish\ndatasets, say, this can be done using the `language` tag, like so:\n```\n$ scandeval --language da\n```\n\nMultiple models, datasets and/or languages can be specified by just attaching multiple\narguments. Here is an example with two models:\n```\n$ scandeval --model-id <model-id1> --model-id <model-id2> --dataset angry-tweets\n```\n\nThe specific model version to use can also be added after the suffix \'@\':\n```\n$ scandeval --model-id <model-id>@<commit>\n```\n\nIt can be a branch name, a tag name, or a commit id. It defaults to \'main\' for latest.\n\nSee all the arguments and options available for the `scandeval` command by typing\n```\n$ scandeval --help\n```\n\n### Benchmarking from a Script\nIn a script, the syntax is similar to the command line interface. You simply initialise\nan object of the `Benchmarker` class, and call this benchmark object with your favorite\nmodels and/or datasets:\n```\n>>> from scandeval import Benchmarker\n>>> benchmark = Benchmarker()\n>>> benchmark(\'<model-id>\')\n```\n\nTo benchmark on a specific dataset, you simply specify the second argument, shown here\nwith the `AngryTweets` dataset again:\n```\n>>> benchmark(\'<model_id>\', \'angry-tweets\')\n```\n\nIf you want to benchmark a subset of all the models on the Hugging Face Hub, you can\nspecify several parameters in the `Benchmarker` initializer to narrow down the list of\nmodels to the ones you care about. As a simple example, the following would benchmark\nall the Nynorsk models on Nynorsk datasets:\n```\n>>> benchmark = Benchmarker(language=\'nn\')\n>>> benchmark()\n```\n\n\n## Citing ScandEval\nIf you want to cite the framework then feel free to use this:\n\n```\n@inproceedings{nielsen2023scandeval,\n  title={ScandEval: A Benchmark for Scandinavian Natural Language Processing},\n  author={Nielsen, Dan Saattrup},\n  booktitle={The 24rd Nordic Conference on Computational Linguistics},\n  year={2023}\n}\n```\n\n\n## Remarks\nThe image used in the logo has been created by the amazing [Scandinavia and the\nWorld](https://satwcomic.com/) team. Go check them out!\n\n\n## Project structure\n```\n.\n├── .flake8\n├── .github\n│\xa0\xa0 └── workflows\n│\xa0\xa0     └── ci.yaml\n├── .gitignore\n├── .pre-commit-config.yaml\n├── CHANGELOG.md\n├── LICENSE\n├── README.md\n├── gfx\n│\xa0\xa0 └── scandeval.png\n├── makefile\n├── poetry.toml\n├── pyproject.toml\n├── src\n│\xa0\xa0 ├── scandeval\n│\xa0\xa0 │\xa0\xa0 ├── __init__.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_config_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmark_dataset.py\n│\xa0\xa0 │\xa0\xa0 ├── benchmarker.py\n│\xa0\xa0 │\xa0\xa0 ├── callbacks.py\n│\xa0\xa0 │\xa0\xa0 ├── cli.py\n│\xa0\xa0 │\xa0\xa0 ├── config.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_configs.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_factory.py\n│\xa0\xa0 │\xa0\xa0 ├── dataset_tasks.py\n│\xa0\xa0 │\xa0\xa0 ├── exceptions.py\n│\xa0\xa0 │\xa0\xa0 ├── hf_hub.py\n│\xa0\xa0 │\xa0\xa0 ├── languages.py\n│\xa0\xa0 │\xa0\xa0 ├── model_loading.py\n│\xa0\xa0 │\xa0\xa0 ├── named_entity_recognition.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering.py\n│\xa0\xa0 │\xa0\xa0 ├── question_answering_trainer.py\n│\xa0\xa0 │\xa0\xa0 ├── scores.py\n│\xa0\xa0 │\xa0\xa0 ├── sequence_classification.py\n│\xa0\xa0 │\xa0\xa0 ├── speed_benchmark.py\n│\xa0\xa0 │\xa0\xa0 ├── types.py\n│\xa0\xa0 │\xa0\xa0 └── utils.py\n│\xa0\xa0 └── scripts\n│\xa0\xa0     ├── create_angry_tweets.py\n│\xa0\xa0     ├── create_dane.py\n│\xa0\xa0     ├── create_mim_gold_ner.py\n│\xa0\xa0     ├── create_norec.py\n│\xa0\xa0     ├── create_norne.py\n│\xa0\xa0     ├── create_scala.py\n│\xa0\xa0     ├── create_scandiqa.py\n│\xa0\xa0     ├── create_suc3.py\n│\xa0\xa0     ├── create_swerec.py\n│\xa0\xa0     ├── create_wikiann_fo.py\n│\xa0\xa0     ├── fill_in_missing_model_metadata.py\n│\xa0\xa0     ├── fix_dot_env_file.py\n│\xa0\xa0     ├── load_ud_pos.py\n│\xa0\xa0     └── versioning.py\n└── tests\n    ├── __init__.py\n    ├── conftest.py\n    ├── test_benchmark_config_factory.py\n    ├── test_benchmark_dataset.py\n    ├── test_benchmarker.py\n    ├── test_callbacks.py\n    ├── test_cli.py\n    ├── test_config.py\n    ├── test_dataset_configs.py\n    ├── test_dataset_factory.py\n    ├── test_dataset_tasks.py\n    ├── test_exceptions.py\n    ├── test_hf_hub.py\n    ├── test_languages.py\n    ├── test_model_loading.py\n    ├── test_named_entity_recognition.py\n    ├── test_question_answering.py\n    ├── test_question_answering_trainer.py\n    ├── test_scores.py\n    ├── test_sequence_classification.py\n    ├── test_speed_benchmark.py\n    ├── test_types.py\n    └── test_utils.py\n```\n',
     'author': 'Dan Saattrup Nielsen',
     'author_email': 'saattrupdan@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://scandeval.github.io',
```

### Comparing `ScandEval-7.0.0/PKG-INFO` & `ScandEval-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scandeval
-Version: 7.0.0
+Version: 7.1.0
 Summary: Evaluation of pretrained language models on mono- or multilingual Scandinavian language tasks.
 Home-page: https://scandeval.github.io
 License: MIT
 Author: Dan Saattrup Nielsen
 Author-email: saattrupdan@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

