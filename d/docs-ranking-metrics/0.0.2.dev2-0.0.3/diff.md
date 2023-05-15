# Comparing `tmp/docs-ranking-metrics-0.0.2.dev2.tar.gz` & `tmp/docs-ranking-metrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev2.tar", last modified: Fri May  5 08:41:42 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.3.tar", last modified: Mon May 15 05:22:44 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.2.dev2.tar` & `docs-ranking-metrics-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.357390 docs-ranking-metrics-0.0.2.dev2/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:41:42.356860 docs-ranking-metrics-0.0.2.dev2/PKG-INFO
--rw-rw-rw-   0        0        0     2359 2023-05-05 08:22:52.000000 docs-ranking-metrics-0.0.2.dev2/README.md
--rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:41:42.357390 docs-ranking-metrics-0.0.2.dev2/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.2.dev2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.327684 docs-ranking-metrics-0.0.2.dev2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.337018 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      135 2023-05-05 08:41:36.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9860 2023-05-05 08:41:07.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     7706 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.355277 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       76 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.268306 docs-ranking-metrics-0.0.3/
+-rw-rw-rw-   0        0        0     2368 2023-05-15 05:22:44.267341 docs-ranking-metrics-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2694 2023-05-05 09:18:40.000000 docs-ranking-metrics-0.0.3/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:22:44.268306 docs-ranking-metrics-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.174147 docs-ranking-metrics-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.236935 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      130 2023-05-15 05:21:37.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9860 2023-05-05 08:41:07.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     7720 2023-05-15 05:18:39.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:44.266322 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2368 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-15 05:22:43.000000 docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.2.dev2/PKG-INFO` & `docs-ranking-metrics-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev2
+Version: 0.0.3
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

### Comparing `docs-ranking-metrics-0.0.2.dev2/README.md` & `docs-ranking-metrics-0.0.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,21 @@
 который можно получить в личном кабинете PyPi.
 
 Twine также поддерживает настройку с помощью переменных среды. 
 Поэтому параметры авторизации можно передать через переменные среды:
 * `TWINE_USERNAME` - имя пользователя, которое будет использоваться для аутентификации в репозитории.
 * `TWINE_PASSWORD` - пароль, используемый для аутентификации в репозитории.
 
+# Генерация документации
+Для генерации документации воспользуйтесь командой:
+```commandline
+bash tools/run_docsgen.sh
+```
+Будет запущен docker-контейнер, который сгенерирует документацию в папку `docs`.
+
 # Улучшения
 
 Что можно сделать (идеи приветствуются):
 
 - [X] Исправить подсчет метрик под документы разной релевантности
 - [ ] Внедрить модель https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2
 - [ ] Придумать дополнительные метрики
```

### Comparing `docs-ranking-metrics-0.0.2.dev2/setup.py` & `docs-ranking-metrics-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             Массив меток
 
         Returns
         ------------
         `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
-        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
+        return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
     FAKE_DOC_LABEL: int = -1
 
     def __init__(self, metrics) -> None:
```

### Comparing `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.3/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev2
+Version: 0.0.3
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

