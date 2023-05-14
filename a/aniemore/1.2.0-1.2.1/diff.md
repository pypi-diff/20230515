# Comparing `tmp/aniemore-1.2.0.tar.gz` & `tmp/aniemore-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aniemore-1.2.0.tar", max compression
+gzip compressed data, was "aniemore-1.2.1.tar", max compression
```

## Comparing `aniemore-1.2.0.tar` & `aniemore-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,20 @@
--rw-r--r--   0        0        0        0 2023-02-19 15:39:16.440064 aniemore-1.2.0/aniemore/__init__.py
--rw-r--r--   0        0        0        0 2023-03-09 00:36:38.168893 aniemore-1.2.0/aniemore/custom/__init__.py
--rw-r--r--   0        0        0    28010 2023-05-11 01:32:48.849285 aniemore-1.2.0/aniemore/custom/models.py
--rw-r--r--   0        0        0      587 2023-04-13 19:34:20.236375 aniemore-1.2.0/aniemore/datasets.py
--rw-r--r--   0        0        0     4729 2023-05-11 01:32:48.849285 aniemore-1.2.0/aniemore/models.py
--rw-r--r--   0        0        0        0 2023-03-09 00:36:38.169894 aniemore-1.2.0/aniemore/recognizers/__init__.py
--rw-r--r--   0        0        0     9924 2023-04-15 01:26:46.065774 aniemore-1.2.0/aniemore/recognizers/multimodal.py
--rw-r--r--   0        0        0     5641 2023-04-13 23:41:12.889330 aniemore-1.2.0/aniemore/recognizers/text.py
--rw-r--r--   0        0        0     3981 2023-04-13 23:56:25.137542 aniemore-1.2.0/aniemore/recognizers/voice.py
--rw-r--r--   0        0        0        0 2023-02-19 15:39:16.444744 aniemore-1.2.0/aniemore/utils/__init__.py
--rw-r--r--   0        0        0    15860 2023-04-13 21:22:28.319429 aniemore-1.2.0/aniemore/utils/classes.py
--rw-r--r--   0        0        0     3104 2023-04-12 13:02:56.273113 aniemore-1.2.0/aniemore/utils/speech2text.py
--rw-r--r--   0        0        0     1125 2023-02-19 15:39:16.439561 aniemore-1.2.0/LICENSE
--rw-r--r--   0        0        0     2303 2023-05-11 01:32:48.850285 aniemore-1.2.0/pyproject.toml
--rw-r--r--   0        0        0    11671 2023-05-11 01:32:48.848285 aniemore-1.2.0/README.md
--rw-r--r--   0        0        0    13775 1970-01-01 00:00:00.000000 aniemore-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.440064 aniemore-1.2.1/aniemore/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.168893 aniemore-1.2.1/aniemore/custom/__init__.py
+-rw-r--r--   0        0        0    12719 2023-05-14 22:39:20.716425 aniemore-1.2.1/aniemore/custom/modeling_classificators.py
+-rw-r--r--   0        0        0      847 2023-05-14 22:39:20.716425 aniemore-1.2.1/aniemore/custom/modeling_hubert.py
+-rw-r--r--   0        0        0      910 2023-05-14 22:39:20.717423 aniemore-1.2.1/aniemore/custom/modeling_unispeech_sat.py
+-rw-r--r--   0        0        0     3040 2023-05-14 22:39:20.717423 aniemore-1.2.1/aniemore/custom/modeling_wav2vec2.py
+-rw-r--r--   0        0        0    12293 2023-05-14 22:39:20.718425 aniemore-1.2.1/aniemore/custom/modeling_wavlm.py
+-rw-r--r--   0        0        0      587 2023-04-13 19:34:20.236375 aniemore-1.2.1/aniemore/datasets.py
+-rw-r--r--   0        0        0     4783 2023-05-14 22:39:20.719425 aniemore-1.2.1/aniemore/models.py
+-rw-r--r--   0        0        0        0 2023-03-09 00:36:38.169894 aniemore-1.2.1/aniemore/recognizers/__init__.py
+-rw-r--r--   0        0        0     9924 2023-04-15 01:26:46.065774 aniemore-1.2.1/aniemore/recognizers/multimodal.py
+-rw-r--r--   0        0        0     5641 2023-04-13 23:41:12.889330 aniemore-1.2.1/aniemore/recognizers/text.py
+-rw-r--r--   0        0        0     3981 2023-04-13 23:56:25.137542 aniemore-1.2.1/aniemore/recognizers/voice.py
+-rw-r--r--   0        0        0        0 2023-02-19 15:39:16.444744 aniemore-1.2.1/aniemore/utils/__init__.py
+-rw-r--r--   0        0        0    15851 2023-05-14 22:39:20.719425 aniemore-1.2.1/aniemore/utils/classes.py
+-rw-r--r--   0        0        0     3104 2023-04-12 13:02:56.273113 aniemore-1.2.1/aniemore/utils/speech2text.py
+-rw-r--r--   0        0        0     1125 2023-02-19 15:39:16.439561 aniemore-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2303 2023-05-14 22:39:20.721425 aniemore-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0    11694 2023-05-11 01:35:43.058318 aniemore-1.2.1/README.md
+-rw-r--r--   0        0        0    13798 1970-01-01 00:00:00.000000 aniemore-1.2.1/PKG-INFO
```

### Comparing `aniemore-1.2.0/aniemore/datasets.py` & `aniemore-1.2.1/aniemore/datasets.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/aniemore/models.py` & `aniemore-1.2.1/aniemore/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
     UniSpeechSatForSequenceClassification,
     HubertForSequenceClassification,
     AutoModelForSequenceClassification,
     BertForSequenceClassification,
     PreTrainedModel
 )
 
-from aniemore.custom.models import (
-    Wav2Vec2BertForSequenceClassification,
-    WavLMBertForSequenceClassification, WavLMBertFusionForSequenceClassification
+from aniemore.custom.modeling_wav2vec2 import Wav2Vec2BertForSequenceClassification
+from aniemore.custom.modeling_wavlm import (
+    WavLMBertForSequenceClassification,
+    WavLMBertFusionForSequenceClassification
 )
 
 
 class Model(NamedTuple):
     """
     NamedTuple класс, используемый для более удобного доступа к информации о модели
```

### Comparing `aniemore-1.2.0/aniemore/recognizers/multimodal.py` & `aniemore-1.2.1/aniemore/recognizers/multimodal.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/aniemore/recognizers/text.py` & `aniemore-1.2.1/aniemore/recognizers/text.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/aniemore/recognizers/voice.py` & `aniemore-1.2.1/aniemore/recognizers/voice.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/aniemore/utils/classes.py` & `aniemore-1.2.1/aniemore/utils/classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     AutoConfig,
     AutoTokenizer,
     AutoFeatureExtractor,
     BertForSequenceClassification,
     PreTrainedModel
 )
 
-from aniemore.custom.models import BaseMultiModalForSequenceBaseClassification
+from aniemore.custom.modeling_classificators import BaseMultiModalForSequenceBaseClassification
 from aniemore.models import Model
 
 RecognizerOutputOne: Type[Dict[str, float]] = dict
 
 
 class RecognizerOutputTuple(NamedTuple):
     """Структура для хранения результатов распознавания"""
@@ -74,15 +74,15 @@
             self.tokenizer = AutoTokenizer.from_pretrained(self.model_url)
         else:
             self.feature_extractor = AutoFeatureExtractor.from_pretrained(self.model_url)
 
         try:
             self.config = AutoConfig.from_pretrained(self.model_url)
             self._model = self.model_cls.from_pretrained(self.model_url, config=self.config)
-        except Exception as exc:  # TODO: needs more precise exception work
+        except (RuntimeError, ValueError) as exc:
             self.config = AutoConfig.from_pretrained(self.model_url, trust_remote_code=True)
             self._model = self.model_cls.from_pretrained(
                 self.model_url, trust_remote_code=True, config=self.config
             )
         finally:
             self._model = self._model.to(self.device)
```

### Comparing `aniemore-1.2.0/aniemore/utils/speech2text.py` & `aniemore-1.2.1/aniemore/utils/speech2text.py`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/LICENSE` & `aniemore-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aniemore-1.2.0/pyproject.toml` & `aniemore-1.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "aniemore"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
     "Ilya Lubenets <lii291001@gmail.com>",
     "Nikita Davidchuk <ar4ikov228@gmail.com>",
     "Artem Amentes <artem@socialcode.ru>",
 ]
 maintainers = [
     "Ilya Lubenets <lii291001@gmail.com>",
```

### Comparing `aniemore-1.2.0/README.md` & `aniemore-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 |----------------------------------------------------------------------------------------------------------------------------------|----------|
 | Голосовые модели                                                                                                                 |          |
 | [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
 | [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                               | 75%      |
 | [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                     | 82%      |
 | [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                   | 75%      |
 | [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)              | 72%      |
-| [**wavlm-bert-base**](Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
+| [**wavlm-bert-base**](https://huggingface.co/Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
 | [**wavlm-bert-fusion**](https://huggingface.co/Aniemore/wavlm-bert-fusion-s-emotion-russian-resd)                                | 83%      |
 | Текстовые модели                                                                                                                 |          |
 | [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                   | 74%      |
 | [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)             | 85%      |
 | [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                 | 76%      |
 | [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                   | 72%      |
```

### Comparing `aniemore-1.2.0/PKG-INFO` & `aniemore-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aniemore
-Version: 1.2.0
+Version: 1.2.1
 Summary: Aniemore (Artem Nikita Ilya EMOtion REcognition) is a library for emotion recognition in voice and text for russian language.
 License: MIT
 Author: Ilya Lubenets
 Author-email: lii291001@gmail.com
 Maintainer: Ilya Lubenets
 Maintainer-email: lii291001@gmail.com
 Requires-Python: >=3.8,<3.12
@@ -93,15 +93,15 @@
 |----------------------------------------------------------------------------------------------------------------------------------|----------|
 | Голосовые модели                                                                                                                 |          |
 | [**wav2vec2-xlsr-53-russian-emotion-recognition**](https://huggingface.co/Aniemore/wav2vec2-xlsr-53-russian-emotion-recognition) | 73%      |
 | [**wav2vec2-emotion-russian-resd**](https://huggingface.co/Aniemore/wav2vec2-emotion-russian-resd)                               | 75%      |
 | [**wavlm-emotion-russian-resd**](https://huggingface.co/Aniemore/wavlm-emotion-russian-resd)                                     | 82%      |
 | [**hubert-emotion-russian-resd**](https://huggingface.co/Aniemore/hubert-emotion-russian-resd)                                   | 75%      |
 | [**unispeech-sat-emotion-russian-resd Copied**](https://huggingface.co/Aniemore/unispeech-sat-emotion-russian-resd)              | 72%      |
-| [**wavlm-bert-base**](Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
+| [**wavlm-bert-base**](https://huggingface.co/Aniemore/wavlm-bert-base-s-emotion-russian-resd)                                                           | 81%      |
 | [**wavlm-bert-fusion**](https://huggingface.co/Aniemore/wavlm-bert-fusion-s-emotion-russian-resd)                                | 83%      |
 | Текстовые модели                                                                                                                 |          |
 | [**rubert-base-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-base-emotion-russian-cedr-m7)                   | 74%      |
 | [**rubert-tiny2-russian-emotion-detection**](https://huggingface.co/Aniemore/rubert-tiny2-russian-emotion-detection)             | 85%      |
 | [**rubert-large-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-large-emotion-russian-cedr-m7)                 | 76%      |
 | [**rubert-tiny-emotion-russian-cedr-m7**](https://huggingface.co/Aniemore/rubert-tiny-emotion-russian-cedr-m7)                   | 72%      |
```

