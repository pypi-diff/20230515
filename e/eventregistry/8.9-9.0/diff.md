# Comparing `tmp/eventregistry-8.9.tar.gz` & `tmp/eventregistry-9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\eventregistry-8.9.tar", last modified: Wed Oct 21 16:38:28 2020, max compression
+gzip compressed data, was "eventregistry-9.0.tar", last modified: Mon May 15 10:33:01 2023, max compression
```

## Comparing `eventregistry-8.9.tar` & `eventregistry-9.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxrwxrwx   0        0        0        0 2020-10-21 16:38:28.000000 eventregistry-8.9/
-drwxrwxrwx   0        0        0        0 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry/
--rw-rw-rw-   0        0        0    10324 2020-05-26 09:45:11.000000 eventregistry-8.9/eventregistry/Analytics.py
--rw-rw-rw-   0        0        0     9791 2018-08-23 06:52:29.000000 eventregistry-8.9/eventregistry/Base.py
--rw-rw-rw-   0        0        0     5356 2019-04-11 08:45:27.000000 eventregistry-8.9/eventregistry/Counts.py
--rw-rw-rw-   0        0        0     2485 2019-04-11 08:41:35.000000 eventregistry-8.9/eventregistry/DailyShares.py
--rw-rw-rw-   0        0        0     1966 2020-05-26 09:45:13.000000 eventregistry-8.9/eventregistry/EventForText.py
--rw-rw-rw-   0        0        0    37279 2020-10-21 16:11:20.000000 eventregistry-8.9/eventregistry/EventRegistry.py
--rw-rw-rw-   0        0        0     3724 2019-04-11 08:42:12.000000 eventregistry-8.9/eventregistry/Info.py
--rw-rw-rw-   0        0        0    13132 2019-03-20 07:53:59.000000 eventregistry-8.9/eventregistry/Query.py
--rw-rw-rw-   0        0        0     5262 2019-04-11 08:42:14.000000 eventregistry-8.9/eventregistry/QueryArticle.py
--rw-rw-rw-   0        0        0    35918 2020-08-18 08:34:15.000000 eventregistry-8.9/eventregistry/QueryArticles.py
--rw-rw-rw-   0        0        0    28830 2020-05-26 09:45:12.000000 eventregistry-8.9/eventregistry/QueryEvent.py
--rw-rw-rw-   0        0        0    32884 2020-02-10 17:14:56.000000 eventregistry-8.9/eventregistry/QueryEvents.py
--rw-rw-rw-   0        0        0     6856 2019-05-12 19:25:42.000000 eventregistry-8.9/eventregistry/QueryStory.py
--rw-rw-rw-   0        0        0     4221 2020-08-18 07:56:40.000000 eventregistry-8.9/eventregistry/Recent.py
--rw-rw-rw-   0        0        0    23866 2019-10-30 08:07:43.000000 eventregistry-8.9/eventregistry/ReturnInfo.py
--rw-rw-rw-   0        0        0    18052 2020-10-21 10:34:11.000000 eventregistry-8.9/eventregistry/TopicPage.py
--rw-rw-rw-   0        0        0     4309 2019-04-11 08:45:27.000000 eventregistry-8.9/eventregistry/Trends.py
--rw-rw-rw-   0        0        0       21 2020-10-21 16:37:50.000000 eventregistry-8.9/eventregistry/_version.py
--rw-rw-rw-   0        0        0      712 2019-03-26 17:02:27.000000 eventregistry-8.9/eventregistry/__init__.py
-drwxrwxrwx   0        0        0        0 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/
--rw-rw-rw-   0        0        0        1 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2017-04-12 20:31:39.000000 eventregistry-8.9/eventregistry.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      730 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       18 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/requires.txt
--rw-rw-rw-   0        0        0      747 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       14 2020-10-21 16:38:28.000000 eventregistry-8.9/eventregistry.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      730 2020-10-21 16:38:28.000000 eventregistry-8.9/PKG-INFO
--rw-rw-rw-   0        0        0     5683 2018-08-12 11:33:39.000000 eventregistry-8.9/README.md
--rw-rw-rw-   0        0        0       42 2020-10-21 16:38:28.000000 eventregistry-8.9/setup.cfg
--rw-rw-rw-   0        0        0     1313 2017-10-14 11:29:58.000000 eventregistry-8.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.441188 eventregistry-9.0/
+-rw-rw-rw-   0        0        0     1099 2016-03-26 08:55:17.000000 eventregistry-9.0/LICENSE
+-rw-rw-rw-   0        0        0      712 2023-05-15 10:33:01.440187 eventregistry-9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8181 2023-05-15 10:10:31.000000 eventregistry-9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.425172 eventregistry-9.0/eventregistry/
+-rw-rw-rw-   0        0        0    10851 2023-04-03 08:02:00.000000 eventregistry-9.0/eventregistry/Analytics.py
+-rw-rw-rw-   0        0        0    10060 2023-01-19 14:20:19.000000 eventregistry-9.0/eventregistry/Base.py
+-rw-rw-rw-   0        0        0     4052 2023-03-23 11:29:32.000000 eventregistry-9.0/eventregistry/Counts.py
+-rw-rw-rw-   0        0        0     2529 2023-01-19 08:55:17.000000 eventregistry-9.0/eventregistry/DailyShares.py
+-rw-rw-rw-   0        0        0     2046 2023-01-19 08:56:51.000000 eventregistry-9.0/eventregistry/EventForText.py
+-rw-rw-rw-   0        0        0    39635 2023-05-10 09:36:42.000000 eventregistry-9.0/eventregistry/EventRegistry.py
+-rw-rw-rw-   0        0        0     3976 2023-01-19 08:59:06.000000 eventregistry-9.0/eventregistry/Info.py
+-rw-rw-rw-   0        0        0      255 2022-03-11 10:55:55.000000 eventregistry-9.0/eventregistry/Logger.py
+-rw-rw-rw-   0        0        0    16179 2023-05-10 09:57:48.000000 eventregistry-9.0/eventregistry/Query.py
+-rw-rw-rw-   0        0        0     5481 2023-01-19 09:19:52.000000 eventregistry-9.0/eventregistry/QueryArticle.py
+-rw-rw-rw-   0        0        0    40411 2023-04-04 09:59:02.000000 eventregistry-9.0/eventregistry/QueryArticles.py
+-rw-rw-rw-   0        0        0    30185 2023-01-19 10:23:22.000000 eventregistry-9.0/eventregistry/QueryEvent.py
+-rw-rw-rw-   0        0        0    35667 2023-03-30 14:36:40.000000 eventregistry-9.0/eventregistry/QueryEvents.py
+-rw-rw-rw-   0        0        0    34065 2023-05-09 12:22:22.000000 eventregistry-9.0/eventregistry/QueryMentions.py
+-rw-rw-rw-   0        0        0     7235 2023-01-19 13:28:14.000000 eventregistry-9.0/eventregistry/QueryStory.py
+-rw-rw-rw-   0        0        0     4420 2023-01-19 13:29:26.000000 eventregistry-9.0/eventregistry/Recent.py
+-rw-rw-rw-   0        0        0    24919 2023-05-15 09:21:43.000000 eventregistry-9.0/eventregistry/ReturnInfo.py
+-rw-rw-rw-   0        0        0    19605 2023-01-19 13:38:39.000000 eventregistry-9.0/eventregistry/TopicPage.py
+-rw-rw-rw-   0        0        0     4461 2023-01-19 13:40:32.000000 eventregistry-9.0/eventregistry/Trends.py
+-rw-rw-rw-   0        0        0      755 2021-06-29 08:01:31.000000 eventregistry-9.0/eventregistry/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-15 10:32:18.000000 eventregistry-9.0/eventregistry/_version.py
+drwxrwxrwx   0        0        0        0 2023-05-15 10:33:01.439194 eventregistry-9.0/eventregistry.egg-info/
+-rw-rw-rw-   0        0        0      712 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      810 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2017-04-12 20:31:39.000000 eventregistry-9.0/eventregistry.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       18 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-15 10:33:00.000000 eventregistry-9.0/eventregistry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 10:33:01.441188 eventregistry-9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2017-10-14 11:29:58.000000 eventregistry-9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `eventregistry-8.9/eventregistry/Analytics.py` & `eventregistry-9.0/eventregistry/Analytics.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,85 +7,90 @@
 - sentiment detection: what is the sentiment expressed in the given text
 - language detection: detect in which language is the given text written
 
 NOTE: the functionality is currently in BETA. The API calls or the provided outputs may change in the future.
 """
 
 import json
+from typing import Union, List
+from eventregistry.EventRegistry import EventRegistry
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 
 class Analytics:
-    def __init__(self, eventRegistry):
+    def __init__(self, eventRegistry: EventRegistry):
         """
         @param eventRegistry: instance of EventRegistry class
         """
         self._er = eventRegistry
 
 
-    def annotate(self, text, lang = None, customParams = None):
+    def annotate(self, text: str, lang: str = None, customParams: dict = None):
         """
         identify the list of entities and nonentities mentioned in the text
         @param text: input text to annotate
         @param lang: language of the provided document (can be an ISO2 or ISO3 code). If None is provided, the language will be automatically detected
         @param customParams: None or a dict with custom parameters to send to the annotation service
         @returns: dict
         """
         params = {"lang": lang, "text": text}
         if customParams:
             params.update(customParams)
         return self._er.jsonRequestAnalytics("/api/v1/annotate", params)
 
 
-    def categorize(self, text, taxonomy = "dmoz"):
+    def categorize(self, text: str, taxonomy: str = "dmoz", concepts: List[str] = None):
         """
         determine the set of up to 5 categories the text is about. Currently, only English text can be categorized!
         @param text: input text to categorize
         @param taxonomy: which taxonomy use for categorization. Options "dmoz" (over 5000 categories in 3 levels, English language only)
             or "news" (general news categorization, 9 categories, any langauge)
         @returns: dict
         """
-        return self._er.jsonRequestAnalytics("/api/v1/categorize", { "text": text, "taxonomy": taxonomy })
+        params = { "text": text, "taxonomy": taxonomy }
+        if isinstance(concepts, list) and len(concepts) > 0:
+            params["concepts"] = concepts
+        return self._er.jsonRequestAnalytics("/api/v1/categorize", params)
 
 
-    def sentiment(self, text, method = "vocabulary", sentencesToAnalyze = 10, returnSentences = True):
+    def sentiment(self, text: str, method: str = "vocabulary", sentencesToAnalyze: int = 10, returnSentences: bool = True):
         """
         determine the sentiment of the provided text in English language
         @param text: input text to categorize
         @param method: method to use to compute the sentiment. possible values are "vocabulary" (vocabulary based sentiment analysis)
             and "rnn" (neural network based sentiment classification)
         @param sentencesToAnalyze: number of sentences in the provided text on which to compute the sentiment.
         @param returnSentences: should the output also contain the list of sentences on which we computed sentiment?
         @returns: dict
         """
         assert method == "vocabulary" or method == "rnn"
         return self._er.jsonRequestAnalytics("/api/v1/sentiment", { "text": text, "method": method, "sentences": sentencesToAnalyze, "returnSentences": returnSentences })
 
 
-    def semanticSimilarity(self, text1, text2, distanceMeasure = "cosine"):
+    def semanticSimilarity(self, text1: str, text2: str, distanceMeasure: str = "cosine"):
         """
         determine the semantic similarity of the two provided documents
         @param text1: first document to analyze
         @param text2: second document to analyze
         @param distanceMeasure: distance measure to use for comparing two documents. Possible values are "cosine" (default) or "jaccard"
         @returns: dict
         """
         return self._er.jsonRequestAnalytics("/api/v1/semanticSimilarity", { "text1": text1, "text2": text2, "distanceMeasure": distanceMeasure })
 
 
-    def detectLanguage(self, text):
+    def detectLanguage(self, text: str):
         """
         determine the language of the given text
         @param text: input text to analyze
         @returns: dict
         """
         return self._er.jsonRequestAnalytics("/api/v1/detectLanguage", { "text": text })
 
 
-    def extractArticleInfo(self, url, proxyUrl = None, headers = None, cookies = None):
+    def extractArticleInfo(self, url: str, proxyUrl: str = None, headers: Union[str, dict] = None, cookies: Union[dict, str] = None):
         """
         extract all available information about an article available at url `url`. Returned information will include
         article title, body, authors, links in the articles, ...
         @param url: article url to extract article information from
         @param proxyUrl: proxy that should be used for downloading article information. format: {schema}://{username}:{pass}@{proxy url/ip}
         @param headers: dict with headers to set in the request (optional)
         @param cookies: dict with cookies to set in the request (optional)
@@ -101,26 +106,26 @@
         if cookies:
             if isinstance(cookies, dict):
                 cookies = json.dumps(cookies)
             params["cookies"] = cookies
         return self._er.jsonRequestAnalytics("/api/v1/extractArticleInfo", params)
 
 
-    def ner(self, text):
+    def ner(self, text: str):
         """
         extract named entities from the provided text. Supported languages are English, German, Spanish and Chinese.
         @param text: text on wich to extract named entities
         @returns: dict
         """
         return self._er.jsonRequestAnalytics("/api/v1/ner", {"text": text})
 
 
-    def trainTopicOnTweets(self, twitterQuery, useTweetText=True, useIdfNormalization=True,
-            normalization="linear", maxTweets=2000, maxUsedLinks=500, ignoreConceptTypes=[],
-            maxConcepts = 20, maxCategories = 10, notifyEmailAddress = None):
+    def trainTopicOnTweets(self, twitterQuery: str, useTweetText: bool = True, useIdfNormalization: bool = True,
+            normalization: bool = "linear", maxTweets: int = 2000, maxUsedLinks: int = 500, ignoreConceptTypes: Union[str, List[str]] = [],
+            maxConcepts: int = 20, maxCategories: int = 10, notifyEmailAddress: str = None):
         """
         create a new topic and train it using the tweets that match the twitterQuery
         @param twitterQuery: string containing the content to search for. It can be a Twitter user account (using "@" prefix or user's Twitter url),
                 a hash tag (using "#" prefix) or a regular keyword.
         @param useTweetText: do you want to analyze the content of the tweets and extract the concepts mentioned in them? If False, only content shared
             in the articles in the user's tweets will be analyzed
         @param useIdfNormalization: normalize identified concepts by their IDF in the news (punish very common concepts)
@@ -141,41 +146,41 @@
         if notifyEmailAddress:
             params["notifyEmailAddress"] = notifyEmailAddress
         if len(ignoreConceptTypes) > 0:
             params["ignoreConceptTypes"] = ignoreConceptTypes
         return self._er.jsonRequestAnalytics("/api/v1/trainTopicOnTwitter", params)
 
 
-    def trainTopicCreateTopic(self, name):
+    def trainTopicCreateTopic(self, name: str):
         """
         create a new topic to train. The user should remember the "uri" parameter returned in the result
         @returns object containing the "uri" property that should be used in the follow-up call to trainTopic* methods
         """
         return self._er.jsonRequestAnalytics("/api/v1/trainTopic", { "action": "createTopic", "name": name})
 
 
-    def trainTopicClearTopic(self, uri):
+    def trainTopicClearTopic(self, uri: str):
         """
         if the topic is already existing, clear the definition of the topic. Use this if you want to retrain an existing topic
         @param uri: uri of the topic (obtained by calling trainTopicCreateTopic method) to clear
         """
         return self._er.jsonRequestAnalytics("/api/v1/trainTopic", { "action": "clearTopic", "uri": uri })
 
 
-    def trainTopicAddDocument(self, uri, text):
+    def trainTopicAddDocument(self, uri: str, text: str):
         """
         add the information extracted from the provided "text" to the topic with uri "uri"
         @param uri: uri of the topic (obtained by calling trainTopicCreateTopic method)
         @param text: text to analyze and extract information from
         """
         return self._er.jsonRequestAnalytics("/api/v1/trainTopic", { "action": "addDocument", "uri": uri, "text": text})
 
 
-    def trainTopicGetTrainedTopic(self, uri, maxConcepts = 20, maxCategories = 10,
-            ignoreConceptTypes=[], idfNormalization = True):
+    def trainTopicGetTrainedTopic(self, uri: str, maxConcepts: int = 20, maxCategories: int = 10,
+            ignoreConceptTypes: Union[str, List[str]] = [], idfNormalization: bool = True):
         """
         retrieve topic for the topic for which you have already finished training
         @param uri: uri of the topic (obtained by calling trainTopicCreateTopic method)
         @param maxConcepts: number of top concepts to retrieve in the topic
         @param maxCategories: number of top categories to retrieve in the topic
         @param ignoreConceptTypes: what types of concepts you would like to ignore in the profile. options: person, org, loc, wiki or an array with those
         @param idfNormalization: should the concepts be normalized by punishing the commonly mentioned concepts
```

### Comparing `eventregistry-8.9/eventregistry/Base.py` & `eventregistry-9.0/eventregistry/Base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ﻿"""
 utility classes for Event Registry
 """
 
 import six, warnings, os, sys, re, datetime, time
-
+from eventregistry.Logger import logger
+from typing import Union, List
 
 mainLangs = ["eng", "deu", "zho", "slv", "spa"]
 allLangs = [ "eng", "deu", "spa", "cat", "por", "ita", "fra", "rus", "ara", "tur", "zho", "slv", "hrv", "srp" ]
 conceptTypes = ["loc", "person", "org", "keyword", "wiki", "conceptClass", "conceptFolder"]
 
 
 def deprecated(func):
@@ -41,15 +42,15 @@
 
 
 class Struct(object):
     """
     helper class for converting dict to a native python object
     instead of a["b"]["c"] we can write a.b.c
     """
-    def __init__(self, data):
+    def __init__(self, data: dict):
         for name, value in data.items():
             setattr(self, name, self._wrap(value))
 
 
     def _wrap(self, value):
         if isinstance(value, (tuple, list, set, frozenset)):
             return type(value)([self._wrap(v) for v in value])
@@ -99,108 +100,108 @@
     """
     Base class for Query and AdminQuery
     used for storing parameters for a query. Parameter values can either be
     simple values (set by _setVal()) or an array of values (set by multiple
     calls to _addArrayVal() method)
     """
     def __init__(self):
-        self.queryParams = {}
+        self.queryParams: dict = {}
 
 
     @staticmethod
-    def copy(obj):
+    def copy(obj: "QueryParamsBase"):
         assert isinstance(obj, QueryParamsBase)
         ret = QueryParamsBase()
         ret.queryParams = dict(obj.queryParams)
         return ret
 
 
     @staticmethod
-    def encodeDate(val):
+    def encodeDate(val: Union[datetime.datetime, datetime.date, str]):
         """encode val that can be a date in different forms as a date that can be sent to Er"""
         if isinstance(val, datetime.datetime):
             return val.date().isoformat()
         elif isinstance(val, datetime.date):
             return val.isoformat()
         elif isinstance(val, six.string_types):
             assert re.match("^\d{4}-\d{2}-\d{2}$", val), "date value '%s' was not provided in the 'YYYY-MM-DD' format" % (val)
             return val
         raise AssertionError("date was not in the expected format")
 
 
     @staticmethod
-    def encodeDateTime(val):
+    def encodeDateTime(val: Union[datetime.datetime, str]):
         """encode datetime into UTC ISO format which can be sent to ER"""
         if isinstance(val, datetime.datetime):
             # if we have a datetime in some tz, we convert it first to UTC
             if val.utcoffset() != None:
                 import pytz
                 val = val.astimezone(pytz.utc)
             return val.isoformat()
         elif isinstance(val, six.string_types):
             assert re.match("^\d{4}-\d{2}-\d{2}T\d{2}:\d{2}:\d{2}(\.\d+)?$", val), "datetime value '%s' was not provided in the 'YYYY-MM-DDTHH:MM:SS.SSSS' format" % (val)
             return val
         raise AssertionError("datetime was not in the recognizable data type. Use datetime or string in ISO format")
 
 
-    def _clearVal(self, propName):
+    def _clearVal(self, propName: str):
         """remove the value of a property propName (if existing)"""
         if propName in self.queryParams:
             del self.queryParams[propName]
 
 
-    def _hasVal(self, propName):
+    def _hasVal(self, propName: str):
         """do we have in the query property named propName"""
         return propName in self.queryParams
 
 
-    def _setVal(self, propName, val):
+    def _setVal(self, propName: str, val):
         """set a value of a property in the query"""
         if isinstance(val, six.string_types):
             # in python 2 we need to first encode, before removing the invalid characters
             if six.PY2:
                 val = val.encode("utf8")
             val = removeInvalidChars(val)
         self.queryParams[propName] = val
 
 
-    def _setValIfNotDefault(self, propName, val, defVal):
+    def _setValIfNotDefault(self, propName: str, val, defVal):
         """set to queryParams property propName to val if val != defVal"""
         if val != defVal:
             self._setVal(propName, val)
 
 
-    def _setDateVal(self, propName, val):
+    def _setDateVal(self, propName: str, val):
         """set a property value that represents date. Value can be string in YYYY-MM-DD format, datetime.date or datetime.datetime"""
         encodedVal = self.encodeDate(val)
         self._setVal(propName, encodedVal)
 
 
-    def _addArrayVal(self, propName, val):
+    def _addArrayVal(self, propName: str, val):
         """add a value to an array of values for a property"""
         if isinstance(val, six.string_types):
             # in python 2 we need to first encode, before removing the invalid characters
             if six.PY2:
                 val = val.encode("utf8")
             val = removeInvalidChars(val)
         if propName not in self.queryParams:
             self.queryParams[propName] = []
         self.queryParams[propName].append(val)
 
 
-    def _update(self, object):
+    def _update(self, object: dict):
         self.queryParams.update(object)
 
 
     def _getQueryParams(self):
         """return the parameters."""
         return dict(self.queryParams)
 
 
-    def _setQueryArrVal(self, value, propName, propOperName, defaultOperName):
+    def _setQueryArrVal(self, value: Union[str, QueryItems, list], propName: str, propOperName: str, defaultOperName: str):
         """
         parse the value "value" and use it to set the property propName and the operator with name propOperName
         @param value: None, string, QueryItems or list. Values to be set using property name propName
         @param propOperName: property to set containing the "and" or "or". Relevant only if multiple items are provided in "value". Can be None if only one value is possible
         @param defaultOperName: which operator should be used in case "value" is a list. If a list, we will print also a warning to suggest use of QueryItems
         """
         # by default we have None - so don't do anything
@@ -222,15 +223,15 @@
         # if we have a list, set it, but also weport
         elif isinstance(value, list):
             self.queryParams[propName] = value
             # if we need to specify the operator for the property
             if propOperName != None:
                 self.queryParams[propOperName] = defaultOperName
                 if len(value) > 1:
-                    print("Warning: The value of parameter '%s' was provided as a list and '%s' operator was used implicitly between the items. We suggest specifying the list using the QueryItems.AND() or QueryItems.OR() to ensure the appropriate operator is used." % (propName, defaultOperName))
+                    logger.warning("Warning: The value of parameter '%s' was provided as a list and '%s' operator was used implicitly between the items. We suggest specifying the list using the QueryItems.AND() or QueryItems.OR() to ensure the appropriate operator is used." % (propName, defaultOperName))
 
         # there should be no other valid types
         else:
             assert False, "Parameter '%s' was of unsupported type. It should either be None, a string or an instance of QueryItems" % (propName)
```

### Comparing `eventregistry-8.9/eventregistry/Counts.py` & `eventregistry-9.0/eventregistry/Counts.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 ﻿"""
 provides classes for obtaining information about how frequently individual concepts or categories
 have been mentioned in news articles (if source == "news") of in social media (if source == "social")
 """
 
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from typing import Union, List
 
 
 class CountsBase(QueryParamsBase):
     def _getPath(self):
         return "/api/v1/counters"
 
 
 
 class GetCounts(CountsBase):
     def __init__(self,
-                 uriOrUriList,
-                 source = "news",
-                 type = "concept",
-                 dateStart = None,
-                 dateEnd = None,
-                 returnInfo = ReturnInfo()):
+                 uriOrUriList: Union[str, List[str]],
+                 type: Union[str, List[str]] = "concept",
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         obtain information about how frequently a concept or category is mentioned in the articles on particular dates
-        by specifying source="custom" one can obtain counts for custom concepts, such as stocks, macroeconomic indicators, etc. The uri
-        for these can be found using EventRegistry.getCustomConceptUri() method.
+        The uri for these can be found using EventRegistry.getCustomConceptUri() method.
         Usage example:
             q = GetCounts([er.getConceptUri("Obama"), er.getConceptUri("ebola")])
             ret = er.execQuery(q)
         Return object:
             {
                 "http://en.wikipedia.org/wiki/Barack_Obama": [
                     {
@@ -47,47 +44,35 @@
                         "date": "2015-05-07"
                     },
                     ...
                 ]
             }
 
         @param uriOrUriList: concept/category uri or a list of uris
-        @param source: input source information from which to compute top trends. Options: "news", "social", "custom", "geo" or "sentiment"
         @param type: what do the uris represent? "concept" or "category"
-        @param dateStart: starting date from which to provide counts onwards (either None, datetime.date or "YYYY-MM-DD")
-        @param dateEnd: ending date until which to provide counts (either None, datetime.date or "YYYY-MM-DD")
         @param returnInfo: what details should be included in the returned information
         """
         CountsBase.__init__(self)
         self._setVal("action", "getCounts")
-        self._setVal("source", source)
         self._setVal("type", type)
         self._update(returnInfo.getParams())
         self._setVal("uri", uriOrUriList)
-        if dateStart != None:
-            self._setDateVal("dateStart", dateStart)
-        if dateEnd != None:
-            self._setDateVal("dateEnd", dateEnd)
 
 
 
 class GetCountsEx(CountsBase):
     def __init__(self,
-                 uriOrUriList,
-                 source = "news",
-                 type = "concept",
-                 dateStart = None,
-                 dateEnd = None,
-                 returnInfo = ReturnInfo()):
+                 uriOrUriList: Union[str, List[str]],
+                 type: str = "concept",
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         obtain information about how frequently a concept or category is mentioned in the articles on particular dates
         Similar to GetCounts, but the output is more friendly for a larger set of provided uris/ids at once
         Usage example:
             q = GetCountsEx(type = "category")
-            q.queryById(range(10))  # return trends of first 10 categories
             ret = er.execQuery(q)
         Return object:
             {
                 "categoryInfo": [
                     {
                         "id": 0,
                         "label": "Root",
@@ -108,21 +93,14 @@
                     ...
                 ]
             }
 
         @param uriOrUriList: concept/category uri or a list of uris
         @param source: input source information from which to compute top trends. Options: "news", "social"
         @param type: what do the uris represent? "concept" or "category"
-        @param dateStart: starting date from which to provide counts onwards (either None, datetime.date or "YYYY-MM-DD")
-        @param dateEnd: ending date until which to provide counts (either None, datetime.date or "YYYY-MM-DD")
         @param returnInfo: what details should be included in the returned information
         """
         CountsBase.__init__(self)
         self._setVal("action", "getCountsEx")
-        self._setVal("source", source)
         self._setVal("type", type)
         self._update(returnInfo.getParams())
         self._setVal("uri", uriOrUriList)
-        if dateStart != None:
-            self._setDateVal("dateStart", dateStart)
-        if dateEnd != None:
-            self._setDateVal("dateEnd", dateEnd)
```

### Comparing `eventregistry-8.9/eventregistry/DailyShares.py` & `eventregistry-9.0/eventregistry/DailyShares.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 
 
 # get top shared articles for today or any other day
 class GetTopSharedArticles(QueryParamsBase):
     def __init__(self,
-                 date = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
-                 count = 20,      # number of top shared articles to return
-                 returnInfo = ReturnInfo()):
+                 date: str = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
+                 count: int = 20,      # number of top shared articles to return
+                 returnInfo: ReturnInfo = ReturnInfo()):
         QueryParamsBase.__init__(self)
         self._setVal("action", "getArticles")
         self._setVal("resultType", "articles")
         self._setVal("articlesCount", count)
         self._setVal("articlesSortBy", "socialScore")
         self._update(returnInfo.getParams("articles"))
 
@@ -32,17 +32,17 @@
     def _getPath(self):
         return "/api/v1/article"
 
 
 # get top shared events for today or any other day
 class GetTopSharedEvents(QueryParamsBase):
     def __init__(self,
-                 date = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
-                 count = 20,      # number of top shared articles to return
-                 returnInfo = ReturnInfo()):
+                 date: str = None,     # specify the date (either in YYYY-MM-DD or datetime.date format) for which to return top shared articles. If None then today is used
+                 count: int = 20,      # number of top shared articles to return
+                 returnInfo: ReturnInfo = ReturnInfo()):
         QueryParamsBase.__init__(self)
         self._setVal("action", "getEvents")
         self._setVal("resultType", "events")
         self._setVal("eventsCount", count)
         self._setVal("eventsSortBy", "socialScore")
         self._update(returnInfo.getParams("events"))
```

### Comparing `eventregistry-8.9/eventregistry/EventForText.py` & `eventregistry-9.0/eventregistry/EventForText.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,29 +25,30 @@
 * eventUri is the uri of the corresponding event in the Event Registry
 * storyUri is the uri of the story in the Event Registry
 You can use QueryEvent or QueryStory to obtain more information about these events/stories
 """
 
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from eventregistry.EventRegistry import EventRegistry
 
 class GetEventForText(QueryParamsBase):
     def __init__(self,
-                 eventRegistry,             # instance of EventRegistry class
-                 nrOfEventsToReturn = 5):   # number of events to return for the given text
+                 eventRegistry: EventRegistry,             # instance of EventRegistry class
+                 nrOfEventsToReturn: int = 5):   # number of events to return for the given text
         QueryParamsBase.__init__(self)
         self._er = eventRegistry
         self._nrOfEventsToReturn = nrOfEventsToReturn
 
 
-    def compute(self,
-                text,           # text for which to find the most similar event
-                lang = "eng"):  # language in which the text is written
+    def compute(self, text: str, lang: str = "eng"):
         """
         compute the list of most similar events for the given text
+        @param text: text for which to find the most similar event
+        @param lang: language in which the text is written
         """
         params = { "lang": lang, "text": text, "topClustersCount": self._nrOfEventsToReturn }
         res = self._er.jsonRequest("/api/v1/getEventForText/getEventForText", params)
         if "topStories" in res:
             return res.get("topStories", [])
         return res
```

### Comparing `eventregistry-8.9/eventregistry/EventRegistry.py` & `eventregistry-9.0/eventregistry/EventRegistry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 ﻿"""
 main class responsible for obtaining results from the Event Registry
 """
-import six, os, sys, traceback, json, re, requests, time
-import threading
+import six, os, sys, traceback, json, re, requests, time, logging, threading
 
+from typing import Union, List
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from eventregistry.Logger import logger
 
 
 class EventRegistry(object):
     """
     the core object that is used to access any data in Event Registry
     it is used to send all the requests and queries
     """
     def __init__(self,
-                 apiKey = None,
-                 host = None,
-                 hostAnalytics = None,
-                 logging = False,
-                 minDelayBetweenRequests = 0.5,
-                 repeatFailedRequestCount = -1,
-                 allowUseOfArchive = True,
-                 verboseOutput = False,
-                 printHostInfo = True,
-                 settingsFName = None):
+                 apiKey: str = None,
+                 host: str = None,
+                 hostAnalytics: str = None,
+                 minDelayBetweenRequests: float = 0.5,
+                 repeatFailedRequestCount: int = -1,
+                 allowUseOfArchive: bool = True,
+                 verboseOutput: bool = False,
+                 settingsFName: str = None):
         """
-        @param apiKey: API key that should be used to make the requests to the Event Registry. API key is assigned to each user account and can be obtained on this page: http://eventregistry.org/me?tab=settings
+        @param apiKey: API key that should be used to make the requests to the Event Registry. API key is assigned to each user account and can be obtained on
+            this page: https://newsapi.ai/dashboard
         @param host: host to use to access the Event Registry backend. Use None to use the default host.
         @param hostAnalytics: the host address to use to perform the analytics api calls
-        @param logging: log all requests made to a 'requests_log.txt' file
         @param minDelayBetweenRequests: the minimum number of seconds between individual api calls
-        @param repeatFailedRequestCount: if a request fails (for example, because ER is down), what is the max number of times the request should be repeated (-1 for indefinitely)
-        @param allowUseOfArchive: default is True. Determines if the queries made should potentially be executed on the archive data. If False, all queries (regardless how the date conditions are set) will be
-                executed on data from the last 31 days. Queries executed on the archive are more expensive so set it to False if you are just interested in recent data
-        @param verboseOutput: if True, additional info about query times etc will be printed to console
-        @param printHostInfo: print which urls are used as the hosts
-        @param settingsFName: If provided it should be a full path to 'settings.json' file where apiKey an/or host can be loaded from. If None, we will look for the settings file in the eventregistry module folder
+        @param repeatFailedRequestCount: if a request fails (for example, because ER is down), what is the max number of times the request
+            should be repeated (-1 for indefinitely)
+        @param allowUseOfArchive: default is True. Determines if the queries made should potentially be executed on the archive data.
+            If False, all queries (regardless how the date conditions are set) will be executed on data from the last 31 days.
+            Queries executed on the archive are more expensive so set it to False if you are just interested in recent data
+        @param verboseOutput: if True, additional info about errors etc will be printed to console
+        @param settingsFName: If provided it should be a full path to 'settings.json' file where apiKey an/or host can be loaded from.
+            If None, we will look for the settings file in the eventregistry module folder
         """
         self._host = host
         self._hostAnalytics = hostAnalytics
         self._lastException = None
-        self._logRequests = logging
+        self._logRequests = False
         self._minDelayBetweenRequests = minDelayBetweenRequests
         self._repeatFailedRequestCount = repeatFailedRequestCount
         self._allowUseOfArchive = allowUseOfArchive
         self._verboseOutput = verboseOutput
         self._lastQueryTime = time.time()
         self._headers = {}
         self._dailyAvailableRequests = -1
@@ -56,80 +57,75 @@
         self._apiKey = apiKey
         self._extraParams = None
 
         # if there is a settings.json file in the directory then try using it to load the API key from it
         # and to read the host name from it (if custom host is not specified)
         currPath = os.path.split(os.path.realpath(__file__))[0]
         settFName = settingsFName or os.path.join(currPath, "settings.json")
-        if apiKey and printHostInfo:
-            print("using user provided API key for making requests")
+        if apiKey:
+            logger.debug("using user provided API key for making requests")
 
         if os.path.exists(settFName):
             settings = json.load(open(settFName))
             self._host = host or settings.get("host", "http://eventregistry.org")
             self._hostAnalytics = hostAnalytics or settings.get("hostAnalytics", "http://analytics.eventregistry.org")
             # if api key is set, then use it when making the requests
             if "apiKey" in settings and not apiKey:
-                if printHostInfo:
-                    print("found apiKey in settings file which will be used for making requests")
+                logger.debug("found apiKey in settings file which will be used for making requests")
                 self._apiKey = settings["apiKey"]
         else:
             self._host = host or "http://eventregistry.org"
             self._hostAnalytics = hostAnalytics or "http://analytics.eventregistry.org"
 
         if self._apiKey == None:
             print("No API key was provided. You will be allowed to perform only a very limited number of requests per day.")
         self._requestLogFName = os.path.join(currPath, "requests_log.txt")
 
-        if printHostInfo:
-            print("Event Registry host: %s" % (self._host))
-            print("Text analytics host: %s" % (self._hostAnalytics))
+        logger.debug("Event Registry host: %s" % (self._host))
+        logger.debug("Text analytics host: %s" % (self._hostAnalytics))
 
         # list of status codes - when we get them as a response from the call, we don't want to repeat the query as the response will likely always be the same
         self._stopStatusCodes = set([
             204,        # Information not available. Request succeeded, but the requested information is not available.
             400,        # Bad request. The request was unacceptable, most likely due to invalid or missing parameter.
             401,        # User's limit reached. The user reached the limit of the tokens in his account. The requests are rejected.
             403,        # Invalid account. The user's IP or account is disabled, potentially due to misuse.
         ])
 
-        # check what is the version of your module compared to the latest one
-        self.checkVersion()
-
 
     def checkVersion(self):
         """
         check what is the latest version of the python sdk and report in case there is a newer version
         """
         try:
             respInfo = self._reqSession.get(self._host + "/static/pythonSDKVersion.txt")
             if respInfo.status_code != 200 or len(respInfo.text) > 20:
                 return
             latestVersion = respInfo.text.strip()
             import eventregistry._version as _version
             currentVersion = _version.__version__
             for (latest, current) in zip(latestVersion.split("."), currentVersion.split(".")):
                 if int(latest) > int(current):
-                    print("==============\nYour version of the module is outdated, please update to the latest version")
-                    print("Your version is %s while the latest is %s" % (currentVersion, latestVersion))
-                    print("Update by calling: pip install --upgrade eventregistry\n==============")
+                    logger.info("==============\nYour version of the module is outdated, please update to the latest version")
+                    logger.info("Your version is %s while the latest is %s" % (currentVersion, latestVersion))
+                    logger.info("Update by calling: pip install --upgrade eventregistry\n==============")
                     return
                 # in case the server mistakenly has a lower version that the user has, don't report an error
                 elif int(latest) < int(current):
                     return
         except:
             pass
 
 
-    def setLogging(self, val):
+    def setLogging(self, val: bool):
         """should all requests be logged to a file or not?"""
         self._logRequests = val
 
 
-    def setExtraParams(self, params):
+    def setExtraParams(self, params: dict):
         if params != None:
             assert(isinstance(params, dict))
         self._extraParams = params
 
 
     def getHost(self):
         return self._host
@@ -137,27 +133,22 @@
 
     def getLastException(self):
         """return the last exception"""
         return self._lastException
 
 
     def printLastException(self):
-        print(str(self._lastException))
+        logger.error(str(self._lastException))
 
 
     def format(self, obj):
         """return a string containing the object in a pretty formated version"""
         return json.dumps(obj, sort_keys=True, indent=4, separators=(',', ': '))
 
 
-    def printConsole(self, text):
-        """print time prefix + text to console"""
-        print(time.strftime("%H:%M:%S") + " " + str(text))
-
-
     def getRemainingAvailableRequests(self):
         """get the number of requests that are still available for the user today. Information is only accessible after you make some query."""
         return self._remainingAvailableRequests
 
 
     def getDailyAvailableRequests(self):
         """get the total number of requests that the user can make in a day. Information is only accessible after you make some query."""
@@ -170,15 +161,15 @@
 
 
     def getServiceStatus(self):
         """return the status of various services used in Event Registry pipeline"""
         return self.jsonRequest("/api/v1/getServiceStatus", {"apiKey": self._apiKey})
 
 
-    def getUrl(self, query):
+    def getUrl(self, query: QueryParamsBase):
         """
         return the url that can be used to get the content that matches the query
         @param query: instance of Query class
         """
         assert isinstance(query, QueryParamsBase), "query parameter should be an instance of a class that has Query as a base class, such as QueryArticles or QueryEvents"
         import urllib
         # don't modify original query params
@@ -194,15 +185,15 @@
     def getLastHeaders(self):
         """
         return the headers returned in the response object of the last executed request
         """
         return self._headers
 
 
-    def getLastHeader(self, headerName, default = None):
+    def getLastHeader(self, headerName: str, default = None):
         """
         get a value of the header headerName that was set in the headers in the last response object
         """
         return self._headers.get(headerName, default)
 
 
     def printLastReqStats(self):
@@ -217,15 +208,15 @@
     def getLastReqArchiveUse(self):
         """
         return True or False depending on whether the last request used the archive or not
         """
         return self.getLastHeader("req-archive", "0") == "1"
 
 
-    def execQuery(self, query, allowUseOfArchive = None):
+    def execQuery(self, query:QueryParamsBase, allowUseOfArchive: bool = None):
         """
         main method for executing the search queries.
         @param query: instance of Query class
         @param allowUseOfArchive: potentially override the value set when constructing EventRegistry class.
             If not None set it to boolean to determine if the request can be executed on the archive data or not
             If left to None then the value set in the EventRegistry constructor will be used
         """
@@ -233,15 +224,15 @@
         # don't modify original query params
         allParams = query._getQueryParams()
         # make the request
         respInfo = self.jsonRequest(query._getPath(), allParams, allowUseOfArchive = allowUseOfArchive)
         return respInfo
 
 
-    def jsonRequest(self, methodUrl, paramDict, customLogFName = None, allowUseOfArchive = None):
+    def jsonRequest(self, methodUrl: str, paramDict: dict, customLogFName: str = None, allowUseOfArchive: bool = None):
         """
         make a request for json data. repeat it _repeatFailedRequestCount times, if they fail (indefinitely if _repeatFailedRequestCount = -1)
         @param methodUrl: url on er (e.g. "/api/v1/article")
         @param paramDict: optional object containing the parameters to include in the request (e.g. { "articleUri": "123412342" }).
         @param customLogFName: potentially a file name where the request information can be logged into
         @param allowUseOfArchive: potentially override the value set when constructing EventRegistry class.
             If not None set it to boolean to determine if the request can be executed on the archive data or not
@@ -276,164 +267,161 @@
         if self._extraParams:
             paramDict.update(self._extraParams)
 
         tryCount = 0
         self._headers = {}  # reset any past data
         returnData = None
         respInfo = None
-        while self._repeatFailedRequestCount < 0 or tryCount < self._repeatFailedRequestCount:
+        url = self._host + methodUrl
+        while self._repeatFailedRequestCount < 0 or tryCount <= self._repeatFailedRequestCount:
             tryCount += 1
             try:
-                url = self._host + methodUrl
-
                 # make the request
-                respInfo = self._reqSession.post(url, json = paramDict)
+                respInfo = self._reqSession.post(url, json = paramDict, timeout=60)
                 # remember the returned headers
                 self._headers = respInfo.headers
                 # if we got some error codes print the error and repeat the request after a short time period
                 if respInfo.status_code != 200:
                     raise Exception(respInfo.text)
                 # did we get a warning. if yes, print it
                 if self.getLastHeader("warning"):
-                    print("=========== WARNING ===========\n%s\n===============================" % (self.getLastHeader("warning")))
+                    logger.warning("=========== WARNING ===========\n%s\n===============================" % (self.getLastHeader("warning")))
                 # remember the available requests
                 self._dailyAvailableRequests = tryParseInt(self.getLastHeader("x-ratelimit-limit", ""), val = -1)
                 self._remainingAvailableRequests = tryParseInt(self.getLastHeader("x-ratelimit-remaining", ""), val = -1)
-                try:
-                    returnData = respInfo.json()
-                    break
-                except Exception as ex:
-                    print("EventRegistry.jsonRequest(): Exception while parsing the returned json object. Repeating the query...")
-                    open("invalidJsonResponse.json", "w").write(respInfo.text)
+
+                returnData = respInfo.json()
+                break
             except Exception as ex:
                 self._lastException = ex
-                print("Event Registry exception while executing the request:")
                 if self._verboseOutput:
-                    print("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
-                self.printLastException()
+                    logger.error("Event Registry exception while executing the request:")
+                    logger.error("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
+                    self.printLastException()
                 # in case of invalid input parameters, don't try to repeat the search but we simply raise the same exception again
                 if respInfo != None and respInfo.status_code in self._stopStatusCodes:
-                    raise ex
+                    break
                 # in case of the other exceptions (maybe the service is temporarily unavailable) we try to repeat the query
-                print("The request will be automatically repeated in 3 seconds...")
-                time.sleep(3)   # sleep for X seconds on error
+                logger.info("The request will be automatically repeated in 3 seconds...")
+                time.sleep(5)   # sleep for X seconds on error
         self._lock.release()
         if returnData == None:
             raise self._lastException or Exception("No valid return data provided")
         return returnData
 
 
-    def jsonRequestAnalytics(self, methodUrl, paramDict):
+    def jsonRequestAnalytics(self, methodUrl: str, paramDict: dict):
         """
         call the analytics service to execute a method like annotation, categorization, etc.
         @param methodUrl: api endpoint url to call
         @param paramDict: a dictionary with values to send to the api endpoint
         """
         if self._apiKey:
             paramDict["apiKey"] = self._apiKey
         self._lock.acquire()
         returnData = None
         respInfo = None
         self._lastException = None
         self._headers = {}  # reset any past data
         tryCount = 0
-        while self._repeatFailedRequestCount < 0 or tryCount < self._repeatFailedRequestCount:
+        while self._repeatFailedRequestCount < 0 or tryCount <= self._repeatFailedRequestCount:
             tryCount += 1
             try:
                 url = self._hostAnalytics + methodUrl
                 # make the request
-                respInfo = self._reqSession.post(url, json = paramDict)
+                respInfo = self._reqSession.post(url, json = paramDict, timeout=60)
                 # remember the returned headers
                 self._headers = respInfo.headers
                 # if we got some error codes print the error and repeat the request after a short time period
                 if respInfo.status_code != 200:
                     raise Exception(respInfo.text)
+
                 returnData = respInfo.json()
                 break
             except Exception as ex:
                 self._lastException = ex
-                print("Event Registry Analytics exception while executing the request:")
                 if self._verboseOutput:
-                    print("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
-                self.printLastException()
-                # in case of invalid input parameters, don't try to repeat the action
-                if respInfo != None and respInfo.status_code == 530:
-                    print("The request will not be repeated since we received a response code 530")
+                    logger.error("Event Registry Analytics exception while executing the request:")
+                    logger.error("endpoint: %s\nParams: %s" % (url, json.dumps(paramDict, indent=4)))
+                    self.printLastException()
+                # in case of invalid input parameters, don't try to repeat the search but we simply raise the same exception again
+                if respInfo != None and respInfo.status_code in self._stopStatusCodes:
                     break
-                print("The request will be automatically repeated in 3 seconds...")
-                time.sleep(3)   # sleep for X seconds on error
+                logger.info("The request will be automatically repeated in 3 seconds...")
+                time.sleep(5)   # sleep for X seconds on error
         self._lock.release()
         if returnData == None:
             raise self._lastException or Exception("No valid return data provided")
         return returnData
 
     #
     # suggestion methods - return type is a list of matching items
 
-    def suggestConcepts(self, prefix, sources = ["concepts"], lang = "eng", conceptLang = "eng", page = 1, count = 20, returnInfo = ReturnInfo(), **kwargs):
+    def suggestConcepts(self, prefix: str, sources: Union[str, list] = ["concepts"], lang: str = "eng", conceptLang: str = "eng", page: int = 1, count: int = 20, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
-        return a list of concepts that contain the given prefix. returned matching concepts are sorted based on their frequency of occurence in news (from most to least frequent)
+        return a list of concepts that contain the given prefix. returned matching concepts are sorted based on their
+            frequency of occurence in news (from most to least frequent)
         @param prefix: input text that should be contained in the concept
-        @param sources: what types of concepts should be returned. valid values are person, loc, org, wiki, entities (== person + loc + org), concepts (== entities + wiki), conceptClass, conceptFolder
+        @param sources: what types of concepts should be returned. valid values are person, loc, org, wiki, entities (== person + loc + org), concepts (== entities + wiki)
         @param lang: language in which the prefix is specified
         @param conceptLang: languages in which the label(s) for the concepts are to be returned
         @param page:  page of the results (1, 2, ...)
         @param count: number of returned suggestions per page
         @param returnInfo: what details about concepts should be included in the returned information
         """
         assert page > 0, "page parameter should be above 0"
         params = { "prefix": prefix, "source": sources, "lang": lang, "conceptLang": conceptLang, "page": page, "count": count}
         params.update(returnInfo.getParams())
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestConceptsFast", params)
 
 
-    def suggestCategories(self, prefix, page = 1, count = 20, returnInfo = ReturnInfo(), **kwargs):
+    def suggestCategories(self, prefix: str, page: int = 1, count: int = 20, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of dmoz categories that contain the prefix
         @param prefix: input text that should be contained in the category name
         @param page:  page of the results (1, 2, ...)
         @param count: number of returned suggestions
         @param returnInfo: what details about categories should be included in the returned information
         """
         assert page > 0, "page parameter should be above 0"
         params = { "prefix": prefix, "page": page, "count": count }
         params.update(returnInfo.getParams())
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestCategoriesFast", params)
 
 
-    def suggestNewsSources(self, prefix, dataType = ["news", "pr", "blog"], page = 1, count = 20, **kwargs):
+    def suggestNewsSources(self, prefix: str, dataType: Union[str, list] = ["news", "pr", "blog"], page: int = 1, count: int = 20, **kwargs):
         """
         return a list of news sources that match the prefix
         @param prefix: input text that should be contained in the source name or uri
         @param dataType: suggest sources that provide content in these data types ("news", "pr", "blog" or a list of any of those)
         @param page: page of results
         @param count: number of returned suggestions
         """
         assert page > 0, "page parameter should be above 0"
         params = {"prefix": prefix, "dataType": dataType, "page": page, "count": count}
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestSourcesFast", params)
 
 
-    def suggestSourceGroups(self, prefix, page = 1, count = 20, **kwargs):
+    def suggestSourceGroups(self, prefix: str, page: int = 1, count: int = 20, **kwargs):
         """
         return a list of news source groups that match the prefix
         @param prefix: input text that should be contained in the source group name or uri
         @param page:  page of the results (1, 2, ...)
         @param count: number of returned suggestions
         """
         assert page > 0, "page parameter should be above 0"
         params = { "prefix": prefix, "page": page, "count": count }
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestSourceGroups", params)
 
 
-    def suggestLocations(self, prefix, sources = ["place", "country"], lang = "eng", count = 20, countryUri = None, sortByDistanceTo = None, returnInfo = ReturnInfo(), **kwargs):
+    def suggestLocations(self, prefix: str, sources: Union[str, list] = ["place", "country"], lang: str = "eng", count: int = 20, countryUri: str = None, sortByDistanceTo: bool = None, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of geo locations (cities or countries) that contain the prefix
         @param prefix: input text that should be contained in the location name
         @param source: what types of locations are we interested in. Possible options are "place" and "country"
         @param lang: language in which the prefix is specified
         @param count: number of returned suggestions
         @param countryUri: if provided, then return only those locations that are inside the specified country
@@ -447,15 +435,15 @@
             assert isinstance(sortByDistanceTo, (tuple, list)), "sortByDistanceTo has to contain a tuple with latitude and longitude of the location"
             assert len(sortByDistanceTo) == 2, "The sortByDistanceTo should contain two float numbers"
             params["closeToLat"] = sortByDistanceTo[0]
             params["closeToLon"] = sortByDistanceTo[1]
         return self.jsonRequest("/api/v1/suggestLocationsFast", params)
 
 
-    def suggestLocationsAtCoordinate(self, latitude, longitude, radiusKm, limitToCities = False, lang = "eng", count = 20, ignoreNonWiki = True, returnInfo = ReturnInfo(), **kwargs):
+    def suggestLocationsAtCoordinate(self, latitude: Union[int, float], longitude: Union[int, float], radiusKm: Union[int, float], limitToCities: bool = False, lang: str = "eng", count: int = 20, ignoreNonWiki: bool = True, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of geo locations (cities or places) that are close to the provided (lat, long) values
         @param latitude: latitude part of the coordinate
         @param longitude: longitude part of the coordinate
         @param radiusKm: radius in kilometres around the coordinates inside which the locations should be returned
         @param limitToCities: limit the set of results only to cities (True) or also to general places (False)
         @param lang: language in which the location label should be returned
@@ -467,57 +455,96 @@
         assert isinstance(longitude, (int, float)), "The 'longitude' should be a number"
         params = { "action": "getLocationsAtCoordinate", "lat": latitude, "lon": longitude, "radius": radiusKm, "limitToCities": limitToCities, "count": count, "lang": lang }
         params.update(returnInfo.getParams())
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestLocationsFast", params)
 
 
-    def suggestSourcesAtCoordinate(self, latitude, longitude, radiusKm, count = 20, **kwargs):
+    def suggestSourcesAtCoordinate(self, latitude: Union[int, float], longitude: Union[int, float], radiusKm: Union[int, float], count: int = 20, **kwargs):
         """
         return a list of news sources that are close to the provided (lat, long) values
         @param latitude: latitude part of the coordinate
         @param longitude: longitude part of the coordinate
         @param radiusKm: radius in kilometres around the coordinates inside which the news sources should be located
         @param count: number of returned suggestions
         """
         assert isinstance(latitude, (int, float)), "The 'latitude' should be a number"
         assert isinstance(longitude, (int, float)), "The 'longitude' should be a number"
         params = {"action": "getSourcesAtCoordinate", "lat": latitude, "lon": longitude, "radius": radiusKm, "count": count}
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestSourcesFast", params)
 
 
-    def suggestSourcesAtPlace(self, conceptUri, dataType = "news", page = 1, count = 20, **kwargs):
+    def suggestSourcesAtPlace(self, conceptUri: str, dataType: Union[str, List[str]] = "news", page = 1, count = 20, **kwargs):
         """
         return a list of news sources that are close to the provided (lat, long) values
         @param conceptUri: concept that represents a geographic location for which we would like to obtain a list of sources located at the place
         @param dataType: type of the news source ("news", "pr", "blog" or a list of any of those)
         @param page: page of the results (1, 2, ...)
         @param count: number of returned sources
         """
         params = {"action": "getSourcesAtPlace", "conceptUri": conceptUri, "page": page, "count": count, "dataType": dataType}
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestSourcesFast", params)
 
 
-    def suggestAuthors(self, prefix, page = 1, count = 20, **kwargs):
+    def suggestAuthors(self, prefix: str, page: int = 1, count: int = 20, **kwargs):
         """
         return a list of news sources that match the prefix
         @param prefix: input text that should be contained in the author name and source url
         @param page: page of results
         @param count: number of returned suggestions
         """
         assert page > 0, "page parameter should be above 0"
         params = {"prefix": prefix, "page": page, "count": count}
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestAuthorsFast", params)
 
 
+    def suggestEventTypes(self, prefix: str, page: int = 1, count: int = 20, **kwargs):
+        """
+        return a list of event types that match the prefix
+        @param prefix: input text that should be contained in the industry name
+        @param page: page of results
+        @param count: number of returned suggestions
+        """
+        assert page > 0, "page parameter should be above 0"
+        params = {"prefix": prefix, "page": page, "count": count}
+        params.update(kwargs)
+        return self.jsonRequest("/api/v1/eventType/suggestEventTypes", params)
+
+
+    def suggestIndustries(self, prefix: str, page: int = 1, count: int = 20, **kwargs):
+        """
+        return a list of industries that match the prefix. Note: Industries can only be used when querying mentions (QueryMentions, QueryMentionsIter)
+        @param prefix: input text that should be contained in the industry name
+        @param page: page of results
+        @param count: number of returned suggestions
+        """
+        assert page > 0, "page parameter should be above 0"
+        params = {"prefix": prefix, "page": page, "count": count}
+        params.update(kwargs)
+        return self.jsonRequest("/api/v1/eventType/suggestIndustries", params)
+
+
+    def getSdgUris(self):
+        """
+        return a list of SDG uris. Note: Industries can only be used when querying mentions (QueryMentions, QueryMentionsIter)
+        """
+        return self.jsonRequest("/api/v1/eventType/sdg/getItems", {})
+
 
-    def suggestConceptClasses(self, prefix, lang = "eng", conceptLang = "eng", source = ["dbpedia", "custom"], page = 1, count = 20, returnInfo = ReturnInfo(), **kwargs):
+    def getSasbUris(self):
+        """
+        return a list of SASB uris. Note: SASB uris can only be used when querying mentions (QueryMentions, QueryMentionsIter)
+        """
+        return self.jsonRequest("/api/v1/eventType/sasb/getItems", {})
+
+
+    def suggestConceptClasses(self, prefix: str, lang: str = "eng", conceptLang: str = "eng", source: Union[str, List[str]] = ["dbpedia", "custom"], page: int = 1, count: int = 20, returnInfo: ReturnInfo = ReturnInfo(), **kwargs):
         """
         return a list of concept classes that match the given prefix
         @param prefix: input text that should be contained in the category name
         @param lang: language in which the prefix is specified
         @param conceptLang: languages in which the label(s) for the concepts are to be returned
         @param source: what types of concepts classes should be returned. valid values are 'dbpedia' or 'custom'
         @param page:  page of the results (1, 2, ...)
@@ -530,132 +557,142 @@
         params.update(kwargs)
         return self.jsonRequest("/api/v1/suggestConceptClasses", params)
 
 
     #
     # get info methods - return type is a single item that is the best match to the given input
 
-    def getConceptUri(self, conceptLabel, lang = "eng", sources = ["concepts"]):
+    def getConceptUri(self, conceptLabel: str, lang: str = "eng", sources: Union[str, List[str]] = ["concepts"]):
         """
         return a concept uri that is the best match for the given concept label
         if there are multiple matches for the given conceptLabel, they are sorted based on their frequency of occurence in news (most to least frequent)
         @param conceptLabel: partial or full name of the concept for which to return the concept uri
-        @param sources: what types of concepts should be returned. valid values are person, loc, org, wiki, entities (== person + loc + org), concepts (== entities + wiki), conceptClass, conceptFolder
+        @param sources: what types of concepts should be returned. valid values are person, loc, org, wiki, entities (== person + loc + org), concepts (== entities + wiki)
         """
         matches = self.suggestConcepts(conceptLabel, lang = lang, sources = sources)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getLocationUri(self, locationLabel, lang = "eng", sources = ["place", "country"], countryUri = None, sortByDistanceTo = None):
+    def getLocationUri(self, locationLabel: str, lang: str = "eng", sources: Union[str, List[str]] = ["place", "country"], countryUri: str = None, sortByDistanceTo: str = None):
         """
         return a location uri that is the best match for the given location label
         @param locationLabel: partial or full location name for which to return the location uri
         @param sources: what types of locations are we interested in. Possible options are "place" and "country"
         @param countryUri: if set, then filter the possible locatiosn to the locations from that country
         @param sortByDistanceTo: sort candidates by distance to the given (lat, long) pair
         """
         matches = self.suggestLocations(locationLabel, sources = sources, lang = lang, countryUri = countryUri, sortByDistanceTo = sortByDistanceTo)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "wikiUri" in matches[0]:
             return matches[0]["wikiUri"]
         return None
 
 
-    def getCategoryUri(self, categoryLabel):
+    def getCategoryUri(self, categoryLabel: str):
         """
         return a category uri that is the best match for the given label
         @param categoryLabel: partial or full name of the category for which to return category uri
         """
         matches = self.suggestCategories(categoryLabel)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getNewsSourceUri(self, sourceName, dataType = ["news", "pr", "blog"]):
+    def getNewsSourceUri(self, sourceName: str, dataType: Union[str, List[str]] = ["news", "pr", "blog"]):
         """
         return the news source that best matches the source name
         @param sourceName: partial or full name of the source or source uri for which to return source uri
         @param dataType: return the source uri that provides content of these data types ("news", "pr", "blog" or a list of any of those)
         """
         matches = self.suggestNewsSources(sourceName, dataType = dataType)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getSourceUri(self, sourceName, dataType=["news", "pr", "blog"]):
+    def getSourceUri(self, sourceName: str, dataType: Union[str, List[str]] = ["news", "pr", "blog"]):
         """
         alternative (shorter) name for the method getNewsSourceUri()
         """
         return self.getNewsSourceUri(sourceName, dataType)
 
 
-    def getSourceGroupUri(self, sourceGroupName):
+    def getSourceGroupUri(self, sourceGroupName: str):
         """
         return the URI of the source group that best matches the name
         @param sourceGroupName: partial or full name of the source group
         """
         matches = self.suggestSourceGroups(sourceGroupName)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getConceptClassUri(self, classLabel, lang = "eng"):
+    def getConceptClassUri(self, classLabel: str, lang: str = "eng"):
         """
         return a uri of the concept class that is the best match for the given label
         @param classLabel: partial or full name of the concept class for which to return class uri
         """
         matches = self.suggestConceptClasses(classLabel, lang = lang)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
-    def getConceptInfo(self, conceptUri,
-                       returnInfo = ReturnInfo(conceptInfo = ConceptInfoFlags(
-                           synonyms = True, image = True, description = True))):
+    def getConceptInfo(self, conceptUri: str,
+                       returnInfo: ReturnInfo = ReturnInfo(conceptInfo = ConceptInfoFlags(synonyms = True, image = True, description = True))):
         """
         return detailed information about a particular concept
         @param conceptUri: uri of the concept
         @param returnInfo: what details about the concept should be included in the returned information
         """
         params = returnInfo.getParams()
         params.update({"uri": conceptUri })
         return self.jsonRequest("/api/v1/concept/getInfo", params)
 
 
-    def getAuthorUri(self, authorName):
+    def getAuthorUri(self, authorName: str):
         """
         return author uri that is the best match for the given author name (and potentially source url)
         if there are multiple matches for the given author name, they are sorted based on the number of articles they have written (from most to least frequent)
         @param authorName: partial or full name of the author, potentially also containing the source url (e.g. "george brown nytimes")
         """
         matches = self.suggestAuthors(authorName)
         if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
             return matches[0]["uri"]
         return None
 
 
+    def getEventTypeUri(self, eventTypeLabel: str):
+        """
+        return event type uri that is the best match for the given label
+        @param eventTypeLabel: partial or full name of the event type for which we want to retrieve uri
+        """
+        matches = self.suggestEventTypes(eventTypeLabel)
+        if matches != None and isinstance(matches, list) and len(matches) > 0 and "uri" in matches[0]:
+            return matches[0]["uri"]
+        return None
+
+
     @staticmethod
-    def getUriFromUriWgt(uriWgtList):
+    def getUriFromUriWgt(uriWgtList: List[str]):
         """
         convert an array of items that contain uri:wgt to a list of items with uri only. Used for QueryArticle and QueryEvent classes
         """
         assert isinstance(uriWgtList, list), "uriWgtList has to be a list of strings that represent article uris"
         uriList = [uriWgt.split(":")[0] for uriWgt in uriWgtList]
         return uriList
 
 
     #
     # additional utility methods
 
-    def getArticleUris(self, articleUrls):
+    def getArticleUris(self, articleUrls: Union[str, List[str]]):
         """
         if you have article urls and you want to query them in ER you first have to obtain their uris in the ER.
         @param articleUrls a single article url or a list of article urls
         @returns returns dict where key is article url and value is either None if no match found or a string with article URI.
         """
         assert isinstance(articleUrls, (six.string_types, list)), "Expected a single article url or a list of urls"
         return self.jsonRequest("/api/v1/articleMapper", { "articleUrl": articleUrls })
@@ -663,15 +700,15 @@
 
     def getSourceGroups(self):
         """return the list of URIs of all known source groups"""
         ret = self.jsonRequest("/api/v1/sourceGroup/getSourceGroups", {})
         return ret
 
 
-    def getSourceGroup(self, sourceGroupUri):
+    def getSourceGroup(self, sourceGroupUri: str):
         """return info about the source group"""
         ret = self.jsonRequest("/api/v1/sourceGroup/getSourceGroupInfo", { "uri": sourceGroupUri })
         return ret
 
 
     #
     # internal methods
@@ -682,26 +719,26 @@
         if t - self._lastQueryTime < self._minDelayBetweenRequests:
             time.sleep(self._minDelayBetweenRequests - (t - self._lastQueryTime))
         self._lastQueryTime = t
 
 
 
 class ArticleMapper:
-    def __init__(self, er, rememberMappings = True):
+    def __init__(self, er: EventRegistry, rememberMappings: bool = True):
         """
         create instance of article mapper
         it will map from article urls to article uris
         the mappings can be remembered so it will not repeat requests for the same article urls
         """
         self._er = er
         self._articleUrlToUri = {}
         self._rememberMappings = rememberMappings
 
 
-    def getArticleUri(self, articleUrl):
+    def getArticleUri(self, articleUrl: str):
         """
         given the article url, return an array with 0, 1 or more article uris. Not all returned article uris are necessarily valid anymore. For news sources
         of lower importance we remove the duplicated articles and just keep the latest content
         @param articleUrl: string containing the article url
         @returns string: list of strings representing article uris.
         """
         if articleUrl in self._articleUrlToUri:
```

### Comparing `eventregistry-8.9/eventregistry/Info.py` & `eventregistry-9.0/eventregistry/Info.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 ﻿from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from typing import Union, List
 
 
 class GetSourceInfo(QueryParamsBase):
     def __init__(self,
-                 uriOrUriList = None,
-                 returnInfo = ReturnInfo()):
+                 uriOrUriList: Union[str, List[str]] = None,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         obtain desired information about one or more news sources
         @param uriOrUriList: single source uri or a list of source uris for which to return information
         @param returnInfo: what details about the source should be included in the returned information
         """
         QueryParamsBase.__init__(self)
         self._setVal("action", "getInfo")
         if uriOrUriList != None:
             self.queryByUri(uriOrUriList)
         self._update(returnInfo.getParams())
 
 
-    def queryByUri(self, uriOrUriList):
+    def queryByUri(self, uriOrUriList: Union[str, List[str]]):
         """search sources by uri(s)"""
         self._setVal("uri", uriOrUriList)
 
 
-    def queryById(self, idOrIdList):
+    def queryById(self, idOrIdList: Union[str, List[str]]):
         """search concepts by id(s)"""
         self._setVal("id", idOrIdList)
 
 
     def _getPath(self):
         return "/api/v1/source"
 
 
 
 class GetConceptInfo(QueryParamsBase):
     def __init__(self,
-                 uriOrUriList = None,
-                 returnInfo = ReturnInfo()):
+                 uriOrUriList: Union[str, List[str]] = None,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         obtain information about concepts
         @param uriOrUriList: single concept uri or a list of concept uris for which to return information
         @param returnInfo: what details about the source should be included in the returned information
         """
         QueryParamsBase.__init__(self)
         self._setVal("action", "getInfo")
@@ -52,40 +53,40 @@
     def _getPath(self):
         return "/api/v1/concept"
 
 
 
 class GetCategoryInfo(QueryParamsBase):
     def __init__(self,
-                 uriOrUriList = None,
-                 returnInfo = ReturnInfo()):
+                 uriOrUriList: Union[str, List[str]] = None,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         obtain information about categories
         @param uriOrUriList: single category uri or a list of category uris for which to return information
         @param returnInfo: what details about the source should be included in the returned information
         """
         QueryParamsBase.__init__(self)
         self._setVal("action", "getInfo")
         if uriOrUriList != None:
             self.queryByUri(uriOrUriList)
         self._update(returnInfo.getParams())
 
 
-    def queryByUri(self, uriOrUriList):
+    def queryByUri(self, uriOrUriList: Union[str, List[str]]):
         """search categories by their uri(s)"""
         self._setVal("uri", uriOrUriList)
 
 
     def _getPath(self):
         return "/api/v1/category"
 
 
 
 class GetSourceStats(QueryParamsBase):
-    def __init__(self, sourceUri = None):
+    def __init__(self, sourceUri: Union[str, List[str]] = None):
         """
         get stats about one or more sources - return json object will include:
          "uri"
          "id"
          "totalArticles" - total number of articles from this source
          "withStory" - number of articles assigned to a story (cluster)
          "duplicates" - number of articles that are duplicates of another article
@@ -99,10 +100,10 @@
             self._setVal("uri", sourceUri)
 
 
     def _getPath(self):
         return "/api/v1/source"
 
 
-    def queryByUri(self, uriOrUriList):
+    def queryByUri(self, uriOrUriList: Union[str, List[str]]):
         """ get stats about one or more sources specified by their uris """
         self.queryParams["uri"] = uriOrUriList
```

### Comparing `eventregistry-8.9/eventregistry/Query.py` & `eventregistry-9.0/eventregistry/Query.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from .Base import QueryParamsBase, QueryItems
-import six
+import six, datetime
+from typing import Union, List
 
 
 class _QueryCore(object):
     def __init__(self):
         self._queryObj = {}
 
 
@@ -19,29 +20,37 @@
         if value != defVal:
             self._queryObj[propName] = value
 
 
 
 class BaseQuery(_QueryCore):
     def __init__(self,
-                 keyword = None,
-                 conceptUri = None,
-                 categoryUri = None,
-                 sourceUri = None,
-                 locationUri = None,
-                 lang = None,
-                 dateStart = None,
-                 dateEnd = None,
-                 dateMention = None,
-                 sourceLocationUri = None,
-                 sourceGroupUri=None,
-                 authorUri = None,
-                 keywordLoc = "body",
+                 keyword: Union[str, QueryItems] = None,
+                 conceptUri: Union[str, QueryItems] = None,
+                 categoryUri: Union[str, QueryItems] = None,
+                 sourceUri: Union[str, QueryItems] = None,
+                 locationUri: Union[str, QueryItems] = None,
+                 lang: Union[str, QueryItems] = None,
+                 dateStart: Union[datetime.datetime, datetime.date, str] = None,
+                 dateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                 sourceLocationUri: Union[str, List[str]] = None,
+                 sourceGroupUri: Union[str, List[str]] = None,
+                 # article or event search only:
+                 dateMention: Union[datetime.datetime, datetime.date, str] = None,
+                 authorUri: Union[str, List[str]] = None,
+                 keywordLoc: str = "body",
+                 # event search only:
                  minMaxArticlesInEvent = None,
-                 exclude = None):
+                 # mention search only:
+                 industryUri: Union[str, QueryItems] = None,
+                 sdgUri: Union[str, QueryItems] = None,
+                 sasbUri: Union[str, QueryItems] = None,
+                 esgUri: Union[str, QueryItems] = None,
+                 # universal:
+                 exclude: Union["BaseQuery", "CombinedQuery"] = None):
         """
         @param keyword: keyword(s) to query. Either None, string or QueryItems instance
         @param conceptUri: concept(s) to query. Either None, string or QueryItems instance
         @param sourceUri: source(s) to query. Either None, string or QueryItems instance
         @param locationUri: location(s) to query. Either None, string or QueryItems instance
         @param categoryUri: categories to query. Either None, string or QueryItems instance
         @param lang: language(s) to query. Either None, string or QueryItems instance
@@ -78,28 +87,33 @@
             else:
                 self._queryObj["dateMention"] = QueryParamsBase.encodeDate(dateMention)
 
         self._setQueryArrVal("sourceLocationUri", sourceLocationUri)
         self._setQueryArrVal("sourceGroupUri", sourceGroupUri)
         self._setQueryArrVal("authorUri", authorUri)
 
+        self._setQueryArrVal("industryUri", industryUri)
+        self._setQueryArrVal("sdgUri", sdgUri)
+        self._setQueryArrVal("sasbUri", sasbUri)
+        self._setQueryArrVal("esgUri", esgUri)
+
         if keywordLoc != "body":
             self._queryObj["keywordLoc"] = keywordLoc
 
         if minMaxArticlesInEvent != None:
             assert isinstance(minMaxArticlesInEvent, tuple), "minMaxArticlesInEvent parameter should either be None or a tuple with two integer values"
             self._queryObj["minArticlesInEvent"] = minMaxArticlesInEvent[0]
             self._queryObj["maxArticlesInEvent"] = minMaxArticlesInEvent[1]
 
         if exclude != None:
             assert isinstance(exclude, (CombinedQuery, BaseQuery)), "exclude parameter was not a CombinedQuery or BaseQuery instance"
             self._queryObj["$not"] = exclude.getQuery()
 
 
-    def _setQueryArrVal(self, propName, value):
+    def _setQueryArrVal(self, propName: str, value):
         # by default we have None - so don't do anything
         if value is None:
             return
         # if we have an instance of QueryItems then apply it
         if isinstance(value, QueryItems):
             self._queryObj[propName] = { value.getOper(): value.getItems() }
 
@@ -114,16 +128,16 @@
 
 class CombinedQuery(_QueryCore):
     def __init__(self):
         super(CombinedQuery, self).__init__()
 
 
     @staticmethod
-    def AND(queryArr,
-            exclude = None):
+    def AND(queryArr: List[Union["BaseQuery", "CombinedQuery"]],
+            exclude: Union["BaseQuery", "CombinedQuery"] = None):
         """
         create a combined query with multiple items on which to perform an AND operation
         @param queryArr: a list of items on which to perform an AND operation. Items can be either a CombinedQuery or BaseQuery instances.
         @param exclude: a instance of BaseQuery, CombinedQuery or None. Used to filter out results matching the other criteria specified in this query
         """
         assert isinstance(queryArr, list), "provided argument as not a list"
         assert len(queryArr) > 0, "queryArr had an empty list"
@@ -135,16 +149,16 @@
         if exclude != None:
             assert isinstance(exclude, (CombinedQuery, BaseQuery)), "exclude parameter was not a CombinedQuery or BaseQuery instance"
             q.setQueryParam("$not", exclude.getQuery())
         return q
 
 
     @staticmethod
-    def OR(queryArr,
-           exclude = None):
+    def OR(queryArr: List[Union["BaseQuery", "CombinedQuery"]],
+           exclude: Union["BaseQuery", "CombinedQuery"] = None):
         """
         create a combined query with multiple items on which to perform an OR operation
         @param queryArr: a list of items on which to perform an OR operation. Items can be either a CombinedQuery or BaseQuery instances.
         @param exclude: a instance of BaseQuery, CombinedQuery or None. Used to filter out results matching the other criteria specified in this query
         """
         assert isinstance(queryArr, list), "provided argument as not a list"
         assert len(queryArr) > 0, "queryArr had an empty list"
@@ -158,25 +172,25 @@
             q.setQueryParam("$not", exclude.getQuery())
         return q
 
 
 
 class ComplexArticleQuery(_QueryCore):
     def __init__(self,
-                 query,
-                 dataType="news",
-                 minSentiment=None,
-                 maxSentiment=None,
-                 minSocialScore=0,
-                 minFacebookShares=0,
-                 startSourceRankPercentile=0,
-                 endSourceRankPercentile = 100,
-                 isDuplicateFilter = "keepAll",
-                 hasDuplicateFilter = "keepAll",
-                 eventFilter = "keepAll"):
+                 query: Union["BaseQuery", "CombinedQuery"],
+                 dataType: Union[str, List[str]] = "news",
+                 minSentiment: float = None,
+                 maxSentiment: float = None,
+                 minSocialScore: int = 0,
+                 minFacebookShares: int = 0,
+                 startSourceRankPercentile: int = 0,
+                 endSourceRankPercentile: int = 100,
+                 isDuplicateFilter: str = "keepAll",
+                 hasDuplicateFilter: str = "keepAll",
+                 eventFilter: str = "keepAll"):
         """
         create an article query using a complex query
         @param query: an instance of CombinedQuery or BaseQuery to use to find articles that match the conditions
         @param dataType: data type to search for. Possible values are "news" (news content), "pr" (PR content) or "blogs".
                 If you want to use multiple data types, put them in an array (e.g. ["news", "pr"])
         @param minSentiment: what should be the minimum sentiment on the articles in order to return them (None means that we don't filter by sentiment)
         @param maxSentiment: what should be the maximum sentiment on the articles in order to return them (None means that we don't filter by sentiment)
@@ -230,17 +244,17 @@
         if len(filter) > 0:
             self._queryObj["$filter"] = filter
 
 
 
 class ComplexEventQuery(_QueryCore):
     def __init__(self,
-                query,
-                minSentiment=None,
-                maxSentiment=None):
+                query: Union["BaseQuery", "CombinedQuery"],
+                minSentiment: float = None,
+                maxSentiment: float = None):
         """
         create an event query using a complex query
         @param query: an instance of CombinedQuery or BaseQuery to use to find events that match the conditions
         """
         super(ComplexEventQuery, self).__init__()
 
         assert isinstance(query, (CombinedQuery, BaseQuery)), "query parameter was not a CombinedQuery or BaseQuery instance"
@@ -249,7 +263,45 @@
             filter["minSentiment"] = minSentiment
         if maxSentiment != None:
             filter["maxSentiment"] = maxSentiment
 
         if len(filter) > 0:
             self._queryObj["$filter"] = filter
         self._queryObj["$query"] = query.getQuery()
+
+
+
+class ComplexMentionQuery(_QueryCore):
+    def __init__(self,
+                query: Union["BaseQuery", "CombinedQuery"],
+                minSentiment: float = None,
+                maxSentiment: float = None,
+                minSentenceIndex: int = None,
+                maxSentenceIndex: int = None,
+                showDuplicates: bool = False):
+        """
+        create a mention query using a complex query
+        @param query: an instance of CombinedQuery or BaseQuery to use to find events that match the conditions
+        @param minSentiment: the minimum sentiment of the mentions to return
+        @param maxSentiment: the maximum sentiment of the mentions to return
+        @param minSentenceIndex: the minimum sentence index of the mentions to return
+        @param maxSentenceIndex: the maximum sentence index of the mentions to return
+        """
+        super(ComplexMentionQuery, self).__init__()
+
+        assert isinstance(query, (CombinedQuery, BaseQuery)), "query parameter was not a CombinedQuery or BaseQuery instance"
+        filter = {}
+        if minSentiment != None:
+            filter["minSentiment"] = minSentiment
+        if maxSentiment != None:
+            filter["maxSentiment"] = maxSentiment
+
+        if minSentenceIndex != None:
+            filter["minSentenceIndex"] = minSentenceIndex
+        if maxSentenceIndex != None:
+            filter["maxSentenceIndex"] = maxSentenceIndex
+        if showDuplicates:
+            filter["showDuplicates"] = showDuplicates
+
+        if len(filter) > 0:
+            self._queryObj["$filter"] = filter
+        self._queryObj["$query"] = query.getQuery()
```

### Comparing `eventregistry-8.9/eventregistry/QueryArticle.py` & `eventregistry-9.0/eventregistry/QueryArticle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ﻿from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
-
+from typing import List, Union
 
 class QueryArticle(Query):
     def __init__(self,
-                 articleUriOrUriList,
-                 requestedResult = None):
+                 articleUriOrUriList: Union[str, List[str]],
+                 requestedResult: "RequestArticle" = None):
         """
         Class for obtaining available info for one or more articles in the Event Registry
         @param articleUriOrUriList: a single article uri or a list of article uris
         @param requestedResult: the information to return as the result of the query. By default return the information about the article
         """
         super(QueryArticle, self).__init__()
         self._setVal("articleUri", articleUriOrUriList)
@@ -18,25 +18,25 @@
 
 
     def _getPath(self):
         return "/api/v1/article"
 
 
     @staticmethod
-    def queryByUri(articleUriOrUriList):
+    def queryByUri(articleUriOrUriList: Union[str, List[str]]):
         """
         obtain information about one or more articles by providing their article uris (newsfeed ids, such as "284017606")
         @param articleUriOrUriList: single article uri or a list of article uris to query
         """
         q = QueryArticle([])
         q.queryParams["articleUri"] = articleUriOrUriList
         return q
 
 
-    def setRequestedResult(self, requestArticle):
+    def setRequestedResult(self, requestArticle: "RequestArticle"):
         """
         Set the single result type that you would like to be returned. If some other request type was previously set, it will be overwritten.
         Result types can be the classes that extend RequestArticle base class (see classes below).
         """
         assert isinstance(requestArticle, RequestArticle), "QueryArticle class can only accept result requests that are of type RequestArticle"
         self.resultTypeList = [requestArticle]
 
@@ -49,31 +49,31 @@
 
     def getResultType(self):
         return self.resultType
 
 
 
 class RequestArticleInfo(RequestArticle):
-    def __init__(self, returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
+    def __init__(self, returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return details about the article
         @param returnInfo: what details should be included in the returned information
         """
         self.resultType = "info"
         self.__dict__.update(returnInfo.getParams("info"))
 
 
 
 class RequestArticleSimilarArticles(RequestArticle):
     def __init__(self,
-                 page = 1,
-                 count = 20,
-                 lang = ["eng"],
-                 limitPerLang = -1,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
+                 page: int = 1,
+                 count: int = 20,
+                 lang: Union[str, List[str]] = ["eng"],
+                 limitPerLang: int = -1,
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return a list of similar articles based on the CCA
         @param page: page of the articles
         @param count: number of articles to return (at most 200)
         @param lang: in which language(s) should be the similar articles
         @param limitPerLang: max number of articles per language to return (-1 for no limit)
         @param returnInfo: what details should be included in the returned information
@@ -87,18 +87,18 @@
         self.similarArticlesLimitPerLang = limitPerLang
         self.__dict__.update(returnInfo.getParams("similarArticles"))
 
 
 
 class RequestArticleDuplicatedArticles(RequestArticle):
     def __init__(self,
-                 page = 1,
-                 count = 20,
-                 sortBy = "cosSim", sortByAsc = False,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
+                 page: int = 1,
+                 count: int = 20,
+                 sortBy: str = "cosSim", sortByAsc: bool = False,
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return a list of duplicated articles of the current article
         @param page: page of the articles
         @param count: number of articles to return (at most 200)
         @param sortBy: how are the articles sorted. Options: id, date, cosSim, fq, socialScore, facebookShares, twitterShares
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -112,14 +112,14 @@
         self.duplicatedArticlesSortByAsc = sortByAsc
         self.__dict__.update(returnInfo.getParams("duplicatedArticles"))
 
 
 
 class RequestArticleOriginalArticle(RequestArticle):
     def __init__(self,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = -1))):
         """
         return the article that is the original of the given article (the current article is a duplicate)
         @param returnInfo: what details should be included in the returned information
         """
         self.resultType = "originalArticle"
         self.__dict__.update(returnInfo.getParams("originalArticle"))
```

### Comparing `eventregistry-8.9/eventregistry/QueryArticles.py` & `eventregistry-9.0/eventregistry/QueryArticles.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,56 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Query import *
+from eventregistry.Logger import logger
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
 
 
 class QueryArticles(Query):
     def __init__(self,
-                keywords = None,
-                conceptUri = None,
-                categoryUri = None,
-                sourceUri = None,
-                sourceLocationUri = None,
-                sourceGroupUri = None,
-                authorUri = None,
-                locationUri = None,
-                lang = None,
-                dateStart = None,
-                dateEnd = None,
-                dateMentionStart = None,
-                dateMentionEnd=None,
-                keywordsLoc="body",
-
-                ignoreKeywords = None,
-                ignoreConceptUri = None,
-                ignoreCategoryUri = None,
-                ignoreSourceUri = None,
-                ignoreSourceLocationUri = None,
-                ignoreSourceGroupUri = None,
-                ignoreAuthorUri = None,
-                ignoreLocationUri = None,
-                ignoreLang = None,
-                ignoreKeywordsLoc = "body",
-
-                isDuplicateFilter = "keepAll",
-                hasDuplicateFilter = "keepAll",
-                eventFilter = "keepAll",
-                startSourceRankPercentile = 0,
-                endSourceRankPercentile = 100,
-                minSentiment = -1,
-                maxSentiment = 1,
-                dataType = "news",
-                requestedResult = None):
+                keywords: Union[str, QueryItems] = None,
+                conceptUri: Union[str, QueryItems] = None,
+                categoryUri: Union[str, QueryItems] = None,
+                sourceUri: Union[str, QueryItems] = None,
+                sourceLocationUri: Union[str, QueryItems] = None,
+                sourceGroupUri: Union[str, QueryItems] = None,
+                authorUri: Union[str, QueryItems] = None,
+                locationUri: Union[str, QueryItems] = None,
+                lang: Union[str, QueryItems] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                keywordsLoc: str = "body",
+
+                ignoreKeywords: Union[str, QueryItems] = None,
+                ignoreConceptUri: Union[str, QueryItems] = None,
+                ignoreCategoryUri: Union[str, QueryItems] = None,
+                ignoreSourceUri: Union[str, QueryItems] = None,
+                ignoreSourceLocationUri: Union[str, QueryItems] = None,
+                ignoreSourceGroupUri: Union[str, QueryItems] = None,
+                ignoreAuthorUri: Union[str, QueryItems] = None,
+                ignoreLocationUri: Union[str, QueryItems] = None,
+                ignoreLang: Union[str, QueryItems] = None,
+                ignoreKeywordsLoc: str = "body",
+
+                isDuplicateFilter: str = "keepAll",
+                hasDuplicateFilter: str = "keepAll",
+                eventFilter: str = "keepAll",
+                authorsFilter: str = "keepAll",
+                videosFilter: str = "keepAll",
+                linksFilter: str = "keepAll",
+                startSourceRankPercentile: int = 0,
+                endSourceRankPercentile: int = 100,
+                minSentiment: float = -1,
+                maxSentiment: float = 1,
+                dataType: Union[str, List[str]] = "news",
+                requestedResult: "RequestArticles" = None):
         """
         Query class for searching for individual articles in the Event Registry.
         The resulting articles have to match all specified conditions. If a parameter value equals "" or [], then it is ignored.
         In order for query to be valid, it has to have at least one positive condition (condition that does not start with ignore*).
 
         @param keywords: find articles that mention the specified keywords.
             A single keyword/phrase can be provided as a string, multiple keywords/phrases can be provided as a list of strings.
@@ -99,14 +105,29 @@
                 "keepOnlyHasDuplicates" (return only the articles that have been later copied by others)
                 "keepAll" (no filtering, default)
         @param eventFilter: some articles describe a known event and some don't. This filter allows you to filter the resulting articles based on this criteria.
                 Possible values are:
                 "skipArticlesWithoutEvent" (skip articles that are not describing any known event in ER)
                 "keepOnlyArticlesWithoutEvent" (return only the articles that are not describing any known event in ER)
                 "keepAll" (no filtering, default)
+        @param authorsFilter: for some articles we are able to extract who their author is and for some we cannot. This filter allows you to filter the resulting articles based on this criteria.
+                Possible values are:
+                "skipIfHasAuthors" (skip articles for which we have identified who their author is)
+                "keepOnlyIfHasAuthors" (return only the articles for which we have extracted their author)
+                "keepAll" (no filtering, default)
+        @param videosFilter: some articles contain a link to a video and some don't. This filter allows you to filter the resulting articles based on this criteria.
+                Possible values are:
+                "skipIfHasVideos" (skip articles that don't contain any link to a video)
+                "keepOnlyIfHasVideos" (return only the articles that contain a link to a video)
+                "keepAll" (no filtering, default)
+        @param linksFilter: some articles contain some links to other urls (potentially other articles) and some don't. This filter allows you to filter the resulting articles based on this criteria.
+                Possible values are:
+                "skipIfHasLinks" (skip articles that contain one or more links to other urls)
+                "keepOnlyIfHasLinks" (return only the articles that contain a link to other urls)
+                "keepAll" (no filtering, default)
         @param startSourceRankPercentile: starting percentile of the sources to consider in the results (default: 0). Value should be in range 0-90 and divisible by 10.
         @param endSourceRankPercentile: ending percentile of the sources to consider in the results (default: 100). Value should be in range 10-100 and divisible by 10.
         @param minSentiment: minimum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all non-English articles)
         @param maxSentiment: maximum value of the sentiment, that the returned articles should have. Range [-1, 1]. Note: setting the value will remove all articles that don't have
                 a computed value for the sentiment (all non-English articles)
         @param dataType: what data types should we search? "news" (news content, default), "pr" (press releases), or "blog".
@@ -155,14 +176,17 @@
 
         self._setValIfNotDefault("keywordLoc", keywordsLoc, "body")
         self._setValIfNotDefault("ignoreKeywordLoc", ignoreKeywordsLoc, "body")
 
         self._setValIfNotDefault("isDuplicateFilter", isDuplicateFilter, "keepAll")
         self._setValIfNotDefault("hasDuplicateFilter", hasDuplicateFilter, "keepAll")
         self._setValIfNotDefault("eventFilter", eventFilter, "keepAll")
+        self._setValIfNotDefault("hasAuthorsFilter", authorsFilter, "keepAll")
+        self._setValIfNotDefault("hasLinksFilter", linksFilter, "keepAll")
+        self._setValIfNotDefault("hasVideosFilter", videosFilter, "keepAll")
         assert startSourceRankPercentile >= 0 and startSourceRankPercentile % 10 == 0 and startSourceRankPercentile <= 100
         assert endSourceRankPercentile >= 0 and endSourceRankPercentile % 10 == 0 and endSourceRankPercentile <= 100
         assert startSourceRankPercentile < endSourceRankPercentile
         if startSourceRankPercentile != 0:
             self._setVal("startSourceRankPercentile", startSourceRankPercentile)
         if endSourceRankPercentile != 100:
             self._setVal("endSourceRankPercentile", endSourceRankPercentile)
@@ -179,57 +203,66 @@
         self.setRequestedResult(requestedResult or RequestArticlesInfo())
 
 
     def _getPath(self):
         return "/api/v1/article"
 
 
-    def setRequestedResult(self, requestArticles):
+    def setRequestedResult(self, requestArticles: "RequestArticles"):
         """
         Set the single result type that you would like to be returned. Any previously set result types will be overwritten.
         Result types can be the classes that extend RequestArticles base class (see classes below).
         """
         assert isinstance(requestArticles, RequestArticles), "QueryArticles class can only accept result requests that are of type RequestArticles"
         self.resultTypeList = [requestArticles]
 
 
     @staticmethod
-    def initWithArticleUriList(uriList):
+    def initWithArticleUriList(uriList: Union[str, List[str]], returnInfo: ReturnInfo = None):
         """
         instead of making a query, provide a list of article URIs manually, and then produce the desired results on top of them
         """
-        q = QueryArticles()
-        assert isinstance(uriList, list), "uriList has to be a list of strings that represent article uris"
-        q.queryParams = { "action": "getArticles", "articleUri": uriList }
+        # we need to set the dataType parameter here, otherwise users cannot ask for blog or pr articles using this way
+        q = QueryArticles(requestedResult=RequestArticlesInfo(returnInfo=returnInfo))
+        assert isinstance(uriList, str) or isinstance(uriList, list), "uriList has to be a list of strings or a string that represent article uris"
+        q.queryParams = { "action": "getArticles", "articleUri": uriList, "dataType": ["news", "blog", "pr"] }
         return q
 
 
     @staticmethod
-    def initWithArticleUriWgtList(uriWgtList):
+    def initWithArticleUriWgtList(uriWgtList: Union[str, List[str]], returnInfo: ReturnInfo = None):
         """
         instead of making a query, provide a list of article URIs manually, and then produce the desired results on top of them
         """
-        q = QueryArticles()
-        assert isinstance(uriWgtList, list), "uriList has to be a list of strings that represent article uris"
-        q.queryParams = { "action": "getArticles", "articleUriWgtList": ",".join(uriWgtList) }
+        # we need to set the dataType parameter here, otherwise users cannot ask for blog or pr articles using this way
+        q = QueryArticles(requestedResult=RequestArticlesInfo(returnInfo=returnInfo))
+        if isinstance(uriWgtList, list):
+            q.queryParams = { "action": "getArticles", "articleUriWgtList": ",".join(uriWgtList) }
+        elif isinstance(uriWgtList, str):
+            q.queryParams = { "action": "getArticles", "articleUriWgtList": uriWgtList, "dataType": ["news", "blog", "pr"] }
+        else:
+            assert False, "uriWgtList parameter did not contain a list or a string"
         return q
 
 
     @staticmethod
-    def initWithComplexQuery(query):
+    def initWithComplexQuery(query: Union[ComplexArticleQuery, str, dict]):
         """
         create a query using a complex article query
         """
         q = QueryArticles()
         # provided an instance of ComplexArticleQuery
         if isinstance(query, ComplexArticleQuery):
             q._setVal("query", json.dumps(query.getQuery()))
         # provided query as a string containing the json object
         elif isinstance(query, six.string_types):
-            foo = json.loads(query)
+            try:
+                foo = json.loads(query)
+            except:
+                raise Exception("Failed to parse the provided string content as a JSON object. Please check the content provided as a parameter to the initWithComplexQuery() method")
             q._setVal("query", query)
         # provided query as a python dict
         elif isinstance(query, dict):
             q._setVal("query", json.dumps(query))
         else:
             assert False, "The instance of query parameter was not a ComplexArticleQuery, a string or a python dict"
         return q
@@ -237,31 +270,31 @@
 
 
 class QueryArticlesIter(QueryArticles, six.Iterator):
     """
     class that simplifies and combines functionality from QueryArticles and RequestArticlesInfo. It provides an iterator
     over the list of articles that match the specified conditions
     """
-    def count(self, eventRegistry):
+    def count(self, eventRegistry: EventRegistry):
         """
         return the number of articles that match the criteria
         """
         self.setRequestedResult(RequestArticlesInfo())
         res = eventRegistry.execQuery(self)
         if "error" in res:
-            print(res["error"])
+            logger.error(res["error"])
         count = res.get("articles", {}).get("totalResults", 0)
         return count
 
 
-    def execQuery(self, eventRegistry,
-                  sortBy = "rel",
-                  sortByAsc = False,
-                  returnInfo = None,
-                  maxItems = -1,
+    def execQuery(self, eventRegistry: EventRegistry,
+                  sortBy: str = "rel",
+                  sortByAsc: bool = False,
+                  returnInfo: ReturnInfo = None,
+                  maxItems: int = -1,
                   **kwargs):
         """
         @param eventRegistry: instance of EventRegistry class. used to query new article list and uris
         @param sortBy: how are articles sorted. Options: date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         @param maxItems: maximum number of items to be returned. Used to stop iteration sooner than results run out
@@ -278,15 +311,15 @@
         self._currItem = 0
         # list of cached articles that are yet to be returned by the iterator
         self._articleList = []
         return self
 
 
     @staticmethod
-    def initWithComplexQuery(query):
+    def initWithComplexQuery(query: Union[ComplexArticleQuery, str, dict]):
         """
         @param query: complex query as ComplexArticleQuery instance, string or a python dict
         """
         q = QueryArticlesIter()
 
         # provided an instance of ComplexArticleQuery
         if isinstance(query, ComplexArticleQuery):
@@ -300,39 +333,42 @@
             q._setVal("query", json.dumps(query))
         else:
             assert False, "The instance of query parameter was not a ComplexArticleQuery, a string or a python dict"
         return q
 
 
     @staticmethod
-    def initWithArticleUriList(uriList):
+    def initWithArticleUriList(uriList: Union[str, List[str]]):
         """
         instead of making a query, provide a list of article URIs manually, and then produce the desired results on top of them
         """
+        # we need to set the dataType parameter here, otherwise users cannot ask for blog or pr articles using this way
         q = QueryArticlesIter()
-        assert isinstance(uriList, list), "uriList has to be a list of strings that represent article uris"
-        q.queryParams = { "action": "getArticles", "articleUri": uriList }
+        if isinstance(uriList, list) or isinstance(uriList, str):
+            q.queryParams = { "action": "getArticles", "articleUri": uriList, "dataType": ["news", "blog", "pr"] }
+        else:
+            assert False, "uriList parameter did not contain a list or a string"
         return q
 
 
     def _getNextArticleBatch(self):
         """download next batch of articles based on the article uris in the uri list"""
         # try to get more uris, if none
         self._articlePage += 1
         # if we have already obtained all pages, then exit
         if self._totalPages != None and self._articlePage > self._totalPages:
             return
         self.setRequestedResult(RequestArticlesInfo(page=self._articlePage,
             sortBy=self._sortBy, sortByAsc=self._sortByAsc,
             returnInfo = self._returnInfo))
         if self._er._verboseOutput:
-            print("Downloading article page %d..." % (self._articlePage))
+            logger.debug("Downloading article page %d..." % (self._articlePage))
         res = self._er.execQuery(self)
         if "error" in res:
-            print("Error while obtaining a list of articles: " + res["error"])
+            logger.error("Error while obtaining a list of articles: " + res["error"])
         else:
             self._totalPages = res.get("articles", {}).get("pages", 0)
         results = res.get("articles", {}).get("results", [])
         self._articleList.extend(results)
 
 
     def __iter__(self):
@@ -361,18 +397,18 @@
     def getResultType(self):
         return self.resultType
 
 
 
 class RequestArticlesInfo(RequestArticles):
     def __init__(self,
-                 page = 1,
-                 count = 100,
-                 sortBy = "date", sortByAsc = False,
-                 returnInfo = None):
+                 page: int = 1,
+                 count: int = 100,
+                 sortBy: str = "date", sortByAsc: bool = False,
+                 returnInfo : ReturnInfo = None):
         """
         return article details for resulting articles
         @param page: page of the articles to return
         @param count: number of articles to return for the given page (at most 100)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -384,28 +420,28 @@
         self.articlesCount = count
         self.articlesSortBy = sortBy
         self.articlesSortByAsc = sortByAsc
         if returnInfo != None:
             self.__dict__.update(returnInfo.getParams("articles"))
 
 
-    def setPage(self, page):
+    def setPage(self, page: int):
         """
         set the page of results to obtain
         """
         assert page >= 1, "page has to be >= 1"
         self.articlesPage = page
 
 
 
 class RequestArticlesUriWgtList(RequestArticles):
     def __init__(self,
-                 page = 1,
-                 count = 10000,
-                 sortBy = "fq", sortByAsc = False):
+                 page: int = 1,
+                 count: int = 10000,
+                 sortBy: str = "fq", sortByAsc: bool = False):
         """
         return a list of article uris together with the scores
         @param page: page of the results (1, 2, ...)
         @param count: number of items to return in a single query (at most 50000)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False) according to the sortBy criteria
         """
@@ -414,15 +450,15 @@
         self.resultType = "uriWgtList"
         self.uriWgtListPage = page
         self.uriWgtListCount = count
         self.uriWgtListSortBy = sortBy
         self.uriWgtListSortByAsc = sortByAsc
 
 
-    def setPage(self, page):
+    def setPage(self, page: int):
         assert page >= 1, "page has to be >= 1"
         self.uriWgtListPage = page
 
 
 
 class RequestArticlesTimeAggr(RequestArticles):
     def __init__(self):
@@ -431,19 +467,19 @@
         """
         self.resultType = "timeAggr"
 
 
 
 class RequestArticlesConceptAggr(RequestArticles):
     def __init__(self,
-                 conceptCount=25,
-                 conceptCountPerType = None,
-                 conceptScoring = "importance",
-                 articlesSampleSize = 10000,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 25,
+                 conceptCountPerType: int = None,
+                 conceptScoring: str = "importance",
+                 articlesSampleSize: str = 10000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of concepts of resulting articles
         @param conceptCount: number of top concepts to return (at most 500)
         @param conceptCountPerType: if you wish to limit the number of top concepts per type (person, org, loc, wiki) then set this to some number.
             If you want to get equal number of concepts for each type then set conceptCountPerType to conceptCount/4 (since there are 4 concept types)
         @param conceptScoring: how should the top concepts be computed. Possible values are
             "importance" (takes into account how frequently a concept is mentioned and how relevant it is in an article),
@@ -462,67 +498,68 @@
             self.conceptAggrConceptCountPerType = conceptCountPerType
         self.__dict__.update(returnInfo.getParams("conceptAggr"))
 
 
 
 class RequestArticlesCategoryAggr(RequestArticles):
     def __init__(self,
-                 articlesSampleSize = 20000,
-                 returnInfo = ReturnInfo()):
+                 articlesSampleSize: int = 20000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of categories of resulting articles
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the categories should be included in the returned information
         """
         assert articlesSampleSize <= 50000
         self.resultType = "categoryAggr"
         self.categoryAggrSampleSize = articlesSampleSize
         self.__dict__.update(returnInfo.getParams("categoryAggr"))
 
 
 
 class RequestArticlesSourceAggr(RequestArticles):
     def __init__(self,
-                 sourceCount = 50,
-                 normalizeBySourceArts = False,
-                 returnInfo = ReturnInfo()):
+                 sourceCount: int = 50,
+                 normalizeBySourceArts: bool = False,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of news sources of resulting articles
         @param sourceCount: the number of top sources to return
         @param normalizeBySourceArts: some sources generate significantly more content than others which is why
             they can appear as top souce for a given query. If you want to normalize and sort the sources by the total number of
             articles that they have published set this to True. This will return as top sources those that potentially publish less
             content overall, but their published content is more about the searched query.
         @param returnInfo: what details about the sources should be included in the returned information
         """
         self.resultType = "sourceAggr"
         self.sourceAggrSourceCount = sourceCount
+        self.sourceAggrNormalizeBySourceArts = normalizeBySourceArts
         self.__dict__.update(returnInfo.getParams("sourceAggr"))
 
 
 class RequestArticlesKeywordAggr(RequestArticles):
     def __init__(self,
-                 articlesSampleSize = 2000):
+                 articlesSampleSize: int = 2000):
         """
         get top keywords in the resulting articles
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 20000)
         """
         assert articlesSampleSize <= 20000
         self.resultType = "keywordAggr"
         self.keywordAggrSampleSize = articlesSampleSize
 
 
 
 class RequestArticlesConceptGraph(RequestArticles):
     def __init__(self,
-                 conceptCount = 25,
-                 linkCount = 50,
-                 articlesSampleSize = 10000,
-                 skipQueryConcepts = True,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 25,
+                 linkCount: int = 50,
+                 articlesSampleSize: int = 10000,
+                 skipQueryConcepts: bool = True,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get concept graph of resulting articles. Identify concepts that frequently co-occur with other concepts
         @param conceptCount: how many concepts should be returned (at most 1000)
         @param linkCount: how many top links between the concepts should be returned (at most 2000)
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
@@ -536,18 +573,18 @@
         self.conceptGraphSkipQueryConcepts = skipQueryConcepts
         self.__dict__.update(returnInfo.getParams("conceptGraph"))
 
 
 
 class RequestArticlesConceptMatrix(RequestArticles):
     def __init__(self,
-                 conceptCount = 25,
-                 measure = "pmi",
-                 articlesSampleSize = 10000,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 25,
+                 measure: str = "pmi",
+                 articlesSampleSize: int = 10000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get aggreate of concept co-occurences of resulting articles
         @param conceptCount: how many concepts should be returned (at most 200)
         @param measure: how should the interestingness between the selected pairs of concepts be computed. Options: pmi (pointwise mutual information), pairTfIdf (pair frequence * IDF of individual concepts), chiSquare
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details should be included in the returned information
         """
@@ -559,18 +596,18 @@
         self.conceptMatrixSampleSize = articlesSampleSize
         self.__dict__.update(returnInfo.getParams("conceptMatrix"))
 
 
 
 class RequestArticlesConceptTrends(RequestArticles):
     def __init__(self,
-                 conceptUris = None,
-                 conceptCount = 25,
-                 articlesSampleSize=10000,
-                 returnInfo = ReturnInfo()):
+                 conceptUris: Union[str, List[str]] = None,
+                 conceptCount: int = 25,
+                 articlesSampleSize: int = 10000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get trending of concepts in the resulting articles
         @param conceptUris: list of concept URIs for which to return trending information. If None, then top concepts will be automatically computed
         @param conceptCount: if the concepts are not provided, what should be the number of automatically determined concepts to return (at most 50)
         @param articlesSampleSize: on what sample of results should the aggregate be computed (at most 50000)
         @param returnInfo: what details should be included in the returned information
         """
@@ -592,24 +629,24 @@
     def __init__(self):
         self.resultType = "dateMentionAggr"
 
 
 
 class RequestArticlesRecentActivity(RequestArticles):
     def __init__(self,
-                 maxArticleCount=100,
-                 updatesAfterNewsUri=None,
-                 updatesafterBlogUri=None,
-                 updatesAfterPrUri=None,
-                 updatesAfterTm = None,
-                 updatesAfterMinsAgo = None,
-                 updatesUntilTm = None,
-                 updatesUntilMinsAgo = None,
-                 mandatorySourceLocation = False,
-                 returnInfo = None):
+                 maxArticleCount: int = 100,
+                 updatesAfterNewsUri: str = None,
+                 updatesafterBlogUri: str = None,
+                 updatesAfterPrUri: str = None,
+                 updatesAfterTm: Union[datetime.datetime, datetime.date, str] = None,
+                 updatesAfterMinsAgo: int = None,
+                 updatesUntilTm: Union[datetime.datetime, datetime.date, str] = None,
+                 updatesUntilMinsAgo: int = None,
+                 mandatorySourceLocation: bool = False,
+                 returnInfo: ReturnInfo = None):
         """
         get the list of articles that were recently added to the Event Registry and match the selected criteria
         @param maxArticleCount: the maximum number of articles to return in the call (the number can be even higher than 100 but in case more articles
             are returned, the call will also use more tokens)
         @param updatesAfterTm: the time after which the articles were added (returned by previous call to the same method)
         @param updatesAfterMinsAgo: how many minutes into the past should we check (set either this or updatesAfterTm property, but not both)
         @param updatesUntilTm: what is the latest time when the articles were added (in case you don't want the most recent articles)
```

### Comparing `eventregistry-8.9/eventregistry/QueryEvent.py` & `eventregistry-9.0/eventregistry/QueryEvent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,69 +1,72 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.QueryArticles import QueryArticles, RequestArticlesInfo
 from eventregistry.Query import *
+from eventregistry.Logger import logger
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
 
 
 class QueryEvent(Query):
     """
     Class for obtaining available info for one or more events in the Event Registry
     """
     def __init__(self,
-                 eventUriOrList,
-                 requestedResult = None):
+                 eventUriOrList: Union[str, List[str]],
+                 requestedResult: "RequestEvent" = None):
         """
         @param eventUriOrUriList: a single event uri or a list of event uris (max 50)
         @param requestedResult: the information to return as the result of the query. By default return the details of the event
         """
         super(QueryEvent, self).__init__()
         self._setVal("action", "getEvent")
         self._setVal("eventUri", eventUriOrList)
         self.setRequestedResult(requestedResult or RequestEventInfo())
 
 
     def _getPath(self):
         return "/api/v1/event"
 
 
-    def setRequestedResult(self, requestEvent):
+    def setRequestedResult(self, requestEvent: "RequestEvent"):
         """
         Set the single result type that you would like to be returned. Any previously set result types will be overwritten.
         Result types can be the classes that extend RequestEvent base class (see classes below).
         """
         assert isinstance(requestEvent, RequestEvent), "QueryEvent class can only accept result requests that are of type RequestEvent"
         self.resultTypeList = [requestEvent]
 
 
 
 class QueryEventArticlesIter(QueryEvent, six.Iterator):
     """
     Class for obtaining an iterator over all articles in the event
     """
-    def __init__(self, eventUri,
-                lang = None,
-                keywords = None,
-                conceptUri = None,
-                categoryUri = None,
-                sourceUri = None,
-                sourceLocationUri = None,
-                sourceGroupUri = None,
-                authorUri = None,
-                locationUri = None,
-                dateStart = None,
-                dateEnd = None,
-                dateMentionStart = None,
-                dateMentionEnd=None,
-                keywordsLoc="body",
-
-                startSourceRankPercentile = 0,
-                endSourceRankPercentile=100,
-                minSentiment = -1,
-                maxSentiment = 1):
+    def __init__(self, eventUri: str,
+                lang: Union[str, QueryItems] = None,
+                keywords: Union[str, QueryItems] = None,
+                conceptUri: Union[str, QueryItems] = None,
+                categoryUri: Union[str, QueryItems] = None,
+                sourceUri: Union[str, QueryItems] = None,
+                sourceLocationUri: Union[str, QueryItems] = None,
+                sourceGroupUri: Union[str, QueryItems] = None,
+                authorUri: Union[str, QueryItems] = None,
+                locationUri: Union[str, QueryItems] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                keywordsLoc: str = "body",
+
+                startSourceRankPercentile: int = 0,
+                endSourceRankPercentile: int = 100,
+                minSentiment: float = -1,
+                maxSentiment: float = 1):
         """
         @param eventUri: a single event for which we want to obtain the list of articles in it
         @param lang: find articles that are written in the specified language.
             If more than one language is specified, resulting articles has to be written in *any* of the languages.
         @param keywords: limit the event articles to those that mention the specified keywords.
             A single keyword/phrase can be provided as a string, multiple keywords/phrases can be provided as a list of strings.
             Use QueryItems.AND() if *all* provided keywords/phrases should be mentioned, or QueryItems.OR() if *any* of the keywords/phrases should be mentioned.
@@ -110,15 +113,15 @@
         self._setQueryArrVal(categoryUri, "categoryUri", "categoryOper", "or")
         self._setQueryArrVal(sourceUri, "sourceUri", "sourceOper", "or")
         self._setQueryArrVal(sourceLocationUri, "sourceLocationUri", None, "or")
         self._setQueryArrVal(sourceGroupUri, "sourceGroupUri", "sourceGroupOper", "or")
         self._setQueryArrVal(authorUri, "authorUri", "authorOper", "or")
         self._setQueryArrVal(locationUri, "locationUri", None, "or")        # location such as "http://en.wikipedia.org/wiki/Ljubljana"
 
-        self._setQueryArrVal(lang, "lang", None, "or")                      # a single lang or list (possible: eng, deu, spa, zho, slv)
+        self._setQueryArrVal(lang, "articlesLang", None, "or")                      # a single lang or list
 
         # starting date of the published articles (e.g. 2014-05-02)
         if dateStart != None:
             self._setDateVal("dateStart", dateStart)
         # ending date of the published articles (e.g. 2014-05-02)
         if dateEnd != None:
             self._setDateVal("dateEnd", dateEnd)
@@ -143,31 +146,31 @@
             assert minSentiment >= -1 and minSentiment <= 1
             self._setVal("minSentiment", minSentiment)      # e.g. -0.5
         if maxSentiment != 1:
             assert maxSentiment >= -1 and maxSentiment <= 1
             self._setVal("maxSentiment", maxSentiment)      # e.g. 0.5
 
 
-    def count(self, eventRegistry):
+    def count(self, eventRegistry: EventRegistry):
         """
         return the number of articles that match the criteria
         @param eventRegistry: instance of EventRegistry class. used to obtain the necessary data
         """
         self.setRequestedResult(RequestEventArticles(**self.queryParams))
         res = eventRegistry.execQuery(self)
         if "error" in res:
-            print(res["error"])
+            logger.error(res["error"])
         count = res.get(self.queryParams["eventUri"], {}).get("articles", {}).get("totalResults", 0)
         return count
 
 
-    def execQuery(self, eventRegistry,
-            sortBy = "cosSim", sortByAsc = False,
-            returnInfo = None,
-            maxItems = -1):
+    def execQuery(self, eventRegistry: EventRegistry,
+            sortBy: str = "cosSim", sortByAsc: bool = False,
+            returnInfo: ReturnInfo = None,
+            maxItems: int = -1):
         """
         @param eventRegistry: instance of EventRegistry class. used to obtain the necessary data
 
         @param sortBy: order in which event articles are sorted. Options: none (no specific sorting), id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
         @param maxItems: maximum number of items to be returned. Used to stop iteration sooner than results run out
@@ -193,24 +196,24 @@
         eventUri = self.queryParams["eventUri"]
         # move to the next page to download
         self._articlePage += 1
         # if we have already obtained all pages, then exit
         if self._totalPages != None and self._articlePage > self._totalPages:
             return
         if self._er._verboseOutput:
-            print("Downloading article page %d from event %s" % (self._articlePage, eventUri))
+            logger.debug("Downloading article page %d from event %s" % (self._articlePage, eventUri))
 
         self.setRequestedResult(RequestEventArticles(
             page = self._articlePage,
             sortBy = self._articlesSortBy, sortByAsc = self._articlesSortByAsc,
             returnInfo = self._returnInfo,
             **self.queryParams))
         res = self._er.execQuery(self)
         if "error" in res:
-            print(res["error"])
+            logger.error(res["error"])
         else:
             self._totalPages = res.get(eventUri, {}).get("articles", {}).get("pages", 0)
         arts = res.get(eventUri, {}).get("articles", {}).get("results", [])
         self._articleList.extend(arts)
 
 
     def __iter__(self):
@@ -239,48 +242,48 @@
 
     def getResultType(self):
         return self.resultType
 
 
 
 class RequestEventInfo(RequestEvent):
-    def __init__(self, returnInfo = ReturnInfo()):
+    def __init__(self, returnInfo: ReturnInfo = ReturnInfo()):
         """
         return details about an event
         """
         self.resultType = "info"
         self.__dict__.update(returnInfo.getParams("info"))
 
 
 
 class RequestEventArticles(RequestEvent, QueryParamsBase):
     def __init__(self,
                 page = 1,
                 count = 100,
 
-                lang = None,
-                keywords = None,
-                conceptUri = None,
-                categoryUri = None,
-                sourceUri = None,
-                sourceLocationUri = None,
-                sourceGroupUri = None,
-                authorUri = None,
-                locationUri = None,
-                dateStart = None,
-                dateEnd = None,
-                dateMentionStart = None,
-                dateMentionEnd=None,
-                keywordsLoc="body",
+                lang: Union[str, QueryItems] = None,
+                keywords: Union[str, QueryItems] = None,
+                conceptUri: Union[str, QueryItems] = None,
+                categoryUri: Union[str, QueryItems] = None,
+                sourceUri: Union[str, QueryItems] = None,
+                sourceLocationUri: Union[str, QueryItems] = None,
+                sourceGroupUri: Union[str, QueryItems] = None,
+                authorUri: Union[str, QueryItems] = None,
+                locationUri: Union[str, QueryItems] = None,
+                dateStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
+                dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                keywordsLoc: str = "body",
 
-                startSourceRankPercentile = 0,
-                endSourceRankPercentile = 100,
+                startSourceRankPercentile: int = 0,
+                endSourceRankPercentile: int = 100,
 
-                sortBy = "cosSim", sortByAsc = False,
-                returnInfo = None,
+                sortBy: str = "cosSim", sortByAsc: bool = False,
+                returnInfo: ReturnInfo = None,
                 **kwds):
         """
         return articles about the event
         @param page: page of the articles to return (1, 2, ...)
         @param count: number of articles to return per page (at most 100)
 
         @param keywords: limit the event articles to those that mention the specified keywords.
@@ -376,16 +379,16 @@
             self.__dict__.update(returnInfo.getParams("articles"))
         del self.queryParams
 
 
 
 class RequestEventArticleUriWgts(RequestEvent):
     def __init__(self,
-                 lang = None,
-                 sortBy="cosSim", sortByAsc=False,
+                 lang: Union[str, List[str]] = None,
+                 sortBy: str = "cosSim", sortByAsc: bool = False,
                  **kwds):
         """
         return just a list of article uris and their associated weights
         @param lang: a single language or a list of languages in which to return the articles. Set None to return all articles
         @param sortBy: order in which event articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         @param kwds: any other potential query parameters - can be any of the parameters used in RequestEventArticles() constructor
@@ -396,15 +399,15 @@
         self.uriWgtListSortByAsc = sortByAsc
         self.resultType = "uriWgtList"
         self.__dict__.update(**kwds)
 
 
 
 class RequestEventKeywordAggr(RequestEvent):
-    def __init__(self, lang=None,
+    def __init__(self, lang: Union[str, List[str]] = None,
                 **kwds):
         """
         return keyword aggregate (tag-cloud) from articles in the event
         @param lang: if not `None` then the top keywords will only be computed from the articles in the specified language.
             The value should match one of the languages for which we have articles in the event.
         @param kwds: any other potential query parameters - can be any of the parameters used in RequestEventArticles() constructor
         """
@@ -430,18 +433,18 @@
         """
         self.resultType = "dateMentionAggr"
 
 
 
 class RequestEventArticleTrend(RequestEvent):
     def __init__(self,
-                 lang = None,
-                 page = 1, count = 100,
-                 minArticleCosSim = -1,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
+                 lang: str = None,
+                 page: int = 1, count: int = 100,
+                 minArticleCosSim: int = -1,
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
         """
         return trending information for the articles about the event
         @param lang: languages for which to compute the trends. If None, then compute trends for all articles
         @param page: page of the articles for which to return information (1, 2, ...)
         @param count: number of articles returned per page (at most 100)
         @param minArticleCosSim: ignore articles that have cos similarity to centroid lower than the specified value (-1 for no limit)
         @param returnInfo: what details should be included in the returned information
@@ -455,21 +458,21 @@
         self.articleTrendMinArticleCosSim = minArticleCosSim
         self.__dict__.update(returnInfo.getParams("articleTrend"))
 
 
 
 class RequestEventSimilarEvents(RequestEvent):
     def __init__(self,
-                conceptInfoList,
-                count = 50,                    # number of similar events to return
-                dateStart = None,              # what can be the oldest date of the similar events
-                dateEnd = None,                # what can be the newest date of the similar events
-                addArticleTrendInfo = False,   # add info how the articles in the similar events are distributed over time
-                aggrHours = 6,                 # if similarEventsAddArticleTrendInfo == True then this is the aggregating window
-                returnInfo = ReturnInfo()):
+                conceptInfoList: List[dict],
+                count: int = 50,                    # number of similar events to return
+                dateStart: Union[datetime.datetime, datetime.date, str] = None,              # what can be the oldest date of the similar events
+                dateEnd: Union[datetime.datetime, datetime.date, str] = None,                # what can be the newest date of the similar events
+                addArticleTrendInfo: bool = False,   # add info how the articles in the similar events are distributed over time
+                aggrHours: int = 6,                 # if similarEventsAddArticleTrendInfo == True then this is the aggregating window
+                returnInfo: ReturnInfo = ReturnInfo()):
         """
         compute and return a list of similar events
         @param conceptInfoList: array of concepts and their importance, e.g. [{ "uri": "http://en.wikipedia.org/wiki/Barack_Obama", "wgt": 100 }, ...]
         @param count: number of similar events to return (at most 50)
         @param dateStart: what can be the oldest date of the similar events
         @param dateEnd: what can be the newest date of the similar events
         @param addArticleTrendInfo: for the returned events compute how they were trending (intensity of reporting) in different time periods
```

### Comparing `eventregistry-8.9/eventregistry/QueryEvents.py` & `eventregistry-9.0/eventregistry/QueryEvents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,48 @@
 ﻿import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Query import *
-
+from eventregistry.Logger import logger
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
 
 class QueryEvents(Query):
     def __init__(self,
-                 keywords = None,
-                 conceptUri = None,
-                 categoryUri = None,
-                 sourceUri = None,
-                 sourceLocationUri = None,
-                 sourceGroupUri = None,
-                 authorUri = None,
-                 locationUri = None,
-                 lang = None,
-                 dateStart = None,
-                 dateEnd = None,
-                 reportingDateStart = None,
-                 reportingDateEnd = None,
-                 minSentiment = -1,
-                 maxSentiment = 1,
-                 minArticlesInEvent = None,
-                 maxArticlesInEvent = None,
-                 dateMentionStart = None,
-                 dateMentionEnd = None,
-                 ignoreKeywords = None,
-                 ignoreConceptUri = None,
-                 ignoreCategoryUri = None,
-                 ignoreSourceUri = None,
-                 ignoreSourceLocationUri = None,
-                 ignoreSourceGroupUri = None,
-                 ignoreAuthorUri = None,
-                 ignoreLocationUri = None,
-                 ignoreLang = None,
-                 keywordsLoc = "body",
-                 ignoreKeywordsLoc = "body",
-                 requestedResult = None):
+                 keywords: Union[str, QueryItems] = None,
+                 conceptUri: Union[str, QueryItems] = None,
+                 categoryUri: Union[str, QueryItems] = None,
+                 sourceUri: Union[str, QueryItems] = None,
+                 sourceLocationUri: Union[str, QueryItems] = None,
+                 sourceGroupUri: Union[str, QueryItems] = None,
+                 authorUri: Union[str, QueryItems] = None,
+                 locationUri: Union[str, QueryItems] = None,
+                 lang: Union[str, QueryItems] = None,
+                 dateStart: Union[datetime.datetime, datetime.date, str] = None,
+                 dateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                 reportingDateStart: Union[datetime.datetime, datetime.date, str] = None,
+                 reportingDateEnd: Union[datetime.datetime, datetime.date, str] = None,
+                 minSentiment: float = -1,
+                 maxSentiment: float = 1,
+                 minArticlesInEvent: int = None,
+                 maxArticlesInEvent: int = None,
+                 dateMentionStart: Union[datetime.datetime, datetime.date, str] = None,
+                 dateMentionEnd: Union[datetime.datetime, datetime.date, str] = None,
+                 ignoreKeywords: Union[str, QueryItems] = None,
+                 ignoreConceptUri: Union[str, QueryItems] = None,
+                 ignoreCategoryUri: Union[str, QueryItems] = None,
+                 ignoreSourceUri: Union[str, QueryItems] = None,
+                 ignoreSourceLocationUri: Union[str, QueryItems] = None,
+                 ignoreSourceGroupUri: Union[str, QueryItems] = None,
+                 ignoreAuthorUri: Union[str, QueryItems] = None,
+                 ignoreLocationUri: Union[str, QueryItems] = None,
+                 ignoreLang: Union[str, QueryItems] = None,
+                 keywordsLoc: str = "body",
+                 ignoreKeywordsLoc: str = "body",
+                 requestedResult: "RequestEvents" = None):
         """
         Query class for searching for events in the Event Registry.
         The resulting events have to match all specified conditions. If a parameter value equals "" or [], then it is ignored.
         In order for query to be valid, it has to have at least one positive condition (condition that does not start with ignore*).
 
         @param keywords: find events where articles mention all the specified keywords.
             A single keyword/phrase can be provided as a string, multiple keywords/phrases can be provided as a list of strings.
@@ -152,57 +154,64 @@
         self.setRequestedResult(requestedResult or RequestEventsInfo())
 
 
     def _getPath(self):
         return "/api/v1/event"
 
 
-    def setRequestedResult(self, requestEvents):
+    def setRequestedResult(self, requestEvents: "RequestEvents"):
         """
         Set the single result type that you would like to be returned. Any previously set result types will be overwritten.
         Result types can be the classes that extend RequestEvents base class (see classes below).
         """
         assert isinstance(requestEvents, RequestEvents), "QueryEvents class can only accept result requests that are of type RequestEvents"
         self.resultTypeList = [requestEvents]
 
 
     @staticmethod
     def initWithEventUriList(uriList):
         """
         Set a custom list of event uris. The results will be then computed on this list - no query will be done (all conditions will be ignored).
         """
         q = QueryEvents()
-        assert isinstance(uriList, list), "uriList has to be a list of strings that represent event uris"
+        assert isinstance(uriList, str) or isinstance(uriList, list), "uriList has to be a list of strings or a string that represent event uris"
         q.queryParams = { "action": "getEvents", "eventUriList": ",".join(uriList) }
         return q
 
 
     @staticmethod
     def initWithEventUriWgtList(uriWgtList):
         """
         Set a custom list of event uris. The results will be then computed on this list - no query will be done (all conditions will be ignored).
         """
         q = QueryEvents()
-        assert isinstance(uriWgtList, list), "uriWgtList has to be a list of strings that represent event uris with their weights"
-        q.queryParams = { "action": "getEvents", "eventUriWgtList": ",".join(uriWgtList) }
+        if isinstance(uriWgtList, list):
+            q.queryParams = { "action": "getEvents", "eventUriWgtList": ",".join(uriWgtList) }
+        elif isinstance(uriWgtList, str):
+            q.queryParams = { "action": "getEvents", "eventUriWgtList": uriWgtList }
+        else:
+            assert False, "uriWgtList parameter did not contain a list or a string"
         return q
 
 
     @staticmethod
-    def initWithComplexQuery(query):
+    def initWithComplexQuery(query: Union[ComplexEventQuery, str, dict]):
         """
         create a query using a complex event query
         """
         q = QueryEvents()
         # provided an instance of ComplexEventQuery
         if isinstance(query, ComplexEventQuery):
             q._setVal("query", json.dumps(query.getQuery()))
         # provided query as a string containing the json object
         elif isinstance(query, six.string_types):
-            foo = json.loads(query)
+            try:
+                foo = json.loads(query)
+            except:
+                raise Exception("Failed to parse the provided string content as a JSON object. Please check the content provided as a parameter to the initWithComplexQuery() method")
             q._setVal("query", query)
         # provided query as a python dict
         elif isinstance(query, dict):
             q._setVal("query", json.dumps(query))
         # unrecognized value provided
         else:
             assert False, "The instance of query parameter was not a ComplexEventQuery, a string or a python dict"
@@ -212,31 +221,31 @@
 
 class QueryEventsIter(QueryEvents, six.Iterator):
     """
     class that simplifies and combines functionality from QueryEvents and RequestEventsInfo. It provides an iterator
     over the list of events that match the specified conditions
     """
 
-    def count(self, eventRegistry):
+    def count(self, eventRegistry: EventRegistry):
         """
         return the number of events that match the criteria
         """
         self.setRequestedResult(RequestEventsInfo())
         res = eventRegistry.execQuery(self)
         if "error" in res:
-            print(res["error"])
+            logger.error(res["error"])
         count = res.get("events", {}).get("totalResults", 0)
         return count
 
 
-    def execQuery(self, eventRegistry,
-                  sortBy = "rel",
-                  sortByAsc = False,
-                  returnInfo = None,
-                  maxItems = -1,
+    def execQuery(self, eventRegistry: EventRegistry,
+                  sortBy: str = "rel",
+                  sortByAsc: bool = False,
+                  returnInfo: ReturnInfo = None,
+                  maxItems: int = -1,
                   **kwargs):
         """
         @param eventRegistry: instance of EventRegistry class. used to query new event list and uris
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
         @param returnInfo: what details should be included in the returned information
@@ -282,18 +291,18 @@
         if self._totalPages != None and self._eventPage > self._totalPages:
             return
         self.setRequestedResult(RequestEventsInfo(page=self._eventPage, count=self._eventBatchSize,
             sortBy= self._sortBy, sortByAsc=self._sortByAsc,
             returnInfo = self._returnInfo))
         # download articles and make sure that we set the same archive flag as it was returned when we were processing the uriList request
         if self._er._verboseOutput:
-            print("Downloading event page %d..." % (self._eventPage))
+            logger.debug("Downloading event page %d..." % (self._eventPage))
         res = self._er.execQuery(self)
         if "error" in res:
-            print("Error while obtaining a list of events: " + res["error"])
+            logger.error("Error while obtaining a list of events: " + res["error"])
         else:
             self._totalPages = res.get("events", {}).get("pages", 0)
         results = res.get("events", {}).get("results", [])
         self._eventList.extend(results)
 
 
     def __iter__(self):
@@ -321,18 +330,18 @@
 
     def getResultType(self):
         return self.resultType
 
 
 
 class RequestEventsInfo(RequestEvents):
-    def __init__(self, page = 1,
-                 count = 50,
-                 sortBy = "rel", sortByAsc = False,
-                 returnInfo = None):
+    def __init__(self, page: int = 1,
+                 count: int = 50,
+                 sortBy: str = "rel", sortByAsc: bool = False,
+                 returnInfo: ReturnInfo = None):
         """
         return event details for resulting events
         @param page: page of the results to return (1, 2, ...)
         @param count: number of events to return per page (at most 50)
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
@@ -345,29 +354,29 @@
         self.eventsCount = count
         self.eventsSortBy = sortBy
         self.eventsSortByAsc = sortByAsc
         if returnInfo != None:
             self.__dict__.update(returnInfo.getParams("events"))
 
 
-    def setPage(self, page):
+    def setPage(self, page: int):
         assert page >= 1, "page has to be >= 1"
         self.eventsPage = page
 
 
-    def setCount(self, count):
+    def setCount(self, count: int):
         self.eventsCount = count
 
 
 
 class RequestEventsUriWgtList(RequestEvents):
     def __init__(self,
-                 page = 1,
-                 count = 50000,
-                 sortBy = "rel", sortByAsc = False):
+                 page: int = 1,
+                 count: int = 50000,
+                 sortBy: str = "rel", sortByAsc: bool = False):
         """
         return a simple list of event uris together with the scores for resulting events
         @param page: page of the results (1, 2, ...)
         @param count: number of results to include per page (at most 100000)
         @param sortBy: how should the resulting events be sorted. Options: date (by event date), rel (relevance to the query), size (number of articles),
             socialScore (amount of shares in social media), none (no specific sorting)
         @param sortByAsc: should the events be sorted in ascending order (True) or descending (False)
@@ -392,29 +401,29 @@
         return time distribution of resulting events
         """
         self.resultType = "timeAggr"
 
 
 
 class RequestEventsKeywordAggr(RequestEvents):
-    def __init__(self, lang = None):
+    def __init__(self, lang: str = None):
         """
         return keyword aggregate (tag cloud) on words in articles in resulting events
         @param lang: in which language to produce the list of top keywords. If None, then compute on all articles
         """
         self.resultType = "keywordAggr"
         if lang != None:
             self.keywordAggrLang = lang
 
 
 
 class RequestEventsLocAggr(RequestEvents):
     def __init__(self,
-                 eventsSampleSize = 100000,
-                 returnInfo = ReturnInfo()):
+                 eventsSampleSize: int = 100000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of locations of resulting events
         @param eventsSampleSize: sample of events to use to compute the location aggregate (at most 100000)
         @param returnInfo: what details (about locations) should be included in the returned information
         """
         assert eventsSampleSize <= 100000
         self.resultType = "locAggr"
@@ -422,33 +431,33 @@
         self.__dict__.update(returnInfo.getParams("locAggr"))
 
 
 
 class RequestEventsLocTimeAggr(RequestEvents):
 
     def __init__(self,
-                 eventsSampleSize = 100000,
-                 returnInfo = ReturnInfo()):
+                 eventsSampleSize: int = 100000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return aggreate of locations and times of resulting events
         @param eventsSampleSize: sample of events to use to compute the location aggregate (at most 100000)
         @param returnInfo: what details (about locations) should be included in the returned information
         """
         assert eventsSampleSize <= 100000
         self.resultType = "locTimeAggr"
         self.locTimeAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("locTimeAggr"))
 
 
 
 class RequestEventsConceptAggr(RequestEvents):
     def __init__(self,
-                 conceptCount = 20,
-                 eventsSampleSize = 100000,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 20,
+                 eventsSampleSize: int = 100000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         compute which concept are the most frequently occuring in the list of resulting events
         @param conceptCount: number of top concepts to return (at most 200)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 1000000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
         assert conceptCount <= 200
@@ -458,18 +467,18 @@
         self.conceptAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("conceptAggr"))
 
 
 
 class RequestEventsConceptGraph(RequestEvents):
     def __init__(self,
-                 conceptCount = 50,
-                 linkCount = 150,
-                 eventsSampleSize = 50000,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 50,
+                 linkCount: int = 150,
+                 eventsSampleSize: int = 50000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         compute which concept pairs frequently co-occur together in the resulting events
         @param conceptCount: number of top concepts to return (at most 1,000)
         @param linkCount: number of links between the concepts to return (at most 2,000)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 100000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
@@ -482,18 +491,18 @@
         self.conceptGraphSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("conceptGraph"))
 
 
 
 class RequestEventsConceptMatrix(RequestEvents):
     def __init__(self,
-                 conceptCount = 25,
-                 measure = "pmi",
-                 eventsSampleSize = 100000,
-                 returnInfo = ReturnInfo()):
+                 conceptCount: int = 25,
+                 measure: str = "pmi",
+                 eventsSampleSize: int = 100000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get a matrix of concepts and their dependencies. For individual concept pairs
         return how frequently they co-occur in the resulting events and
         how "surprising" this is, based on the frequency of individual concepts
         @param conceptCount: number of top concepts to return (at most 200)
         @param measure: how should the interestingness between the selected pairs of concepts be computed. Options: pmi (pointwise mutual information), pairTfIdf (pair frequence * IDF of individual concepts), chiSquare
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
@@ -507,17 +516,17 @@
         self.conceptMatrixSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("conceptMatrix"))
 
 
 
 class RequestEventsConceptTrends(RequestEvents):
     def __init__(self,
-                 conceptUris = None,
-                 conceptCount = 10,
-                 returnInfo = ReturnInfo()):
+                 conceptUris: Union[str, List[str]] = None,
+                 conceptCount: int = 10,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return a list of top trending concepts and their daily trending info over time
         @param conceptUris: list of concept URIs for which to return trending information. If None, then top concepts will be automatically computed
         @param count: if the concepts are not provided, what should be the number of automatically determined concepts to return (at most 50)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
         assert conceptCount <= 50
@@ -527,17 +536,17 @@
         self.conceptTrendsConceptCount = conceptCount
         self.__dict__.update(returnInfo.getParams("conceptTrends"))
 
 
 
 class RequestEventsSourceAggr(RequestEvents):
     def __init__(self,
-                 sourceCount = 30,
-                 eventsSampleSize = 50000,
-                 returnInfo = ReturnInfo()):
+                 sourceCount: int = 30,
+                 eventsSampleSize: int = 50000,
+                 returnInfo : ReturnInfo = ReturnInfo()):
         """
         return top news sources that report about the events that match the search conditions
         @param sourceCount: number of top sources to return (at most 200)
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
         @param returnInfo: what details about the sources should be included in the returned information
         """
         assert sourceCount <= 200
@@ -547,17 +556,17 @@
         self.sourceAggrSampleSize = eventsSampleSize
         self.__dict__.update(returnInfo.getParams("sourceAggr"))
 
 
 
 class RequestEventsDateMentionAggr(RequestEvents):
     def __init__(self,
-                 minDaysApart = 0,
-                 minDateMentionCount = 5,
-                 eventsSampleSize = 100000):
+                 minDaysApart: int = 0,
+                 minDateMentionCount: int = 5,
+                 eventsSampleSize: int = 100000):
         """
         return events and the dates that are mentioned in articles about these events
         @param minDaysApart: ignore events that don't have a date that is more than this number of days apart from the tested event
         @param minDateMentionCount: report only dates that are mentioned at least this number of times
         @param eventsSampleSize: on what sample of results should the aggregate be computed (at most 300000)
         """
         assert eventsSampleSize <= 300000
@@ -566,17 +575,17 @@
         self.dateMentionAggrMinDateMentionCount = minDateMentionCount
         self.dateMentionAggrSampleSize = eventsSampleSize
 
 
 
 class RequestEventsEventClusters(RequestEvents):
     def __init__(self,
-                 keywordCount = 30,
-                 maxEventsToCluster = 10000,
-                 returnInfo = ReturnInfo()):
+                 keywordCount: int = 30,
+                 maxEventsToCluster: int = 10000,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return hierarchical clustering of events into smaller clusters. 2-means clustering is applied on each node in the tree
         @param keywordCount: number of keywords to report in each of the clusters (at most 100)
         @param maxEventsToCluster: try to cluster at most this number of events (at most 10000)
         @param returnInfo: what details about the concepts should be included in the returned information
         """
         assert keywordCount <= 100
@@ -586,32 +595,32 @@
         self.eventClustersMaxEventsToCluster = maxEventsToCluster
         self.__dict__.update(returnInfo.getParams("eventClusters"))
 
 
 
 class RequestEventsCategoryAggr(RequestEvents):
     def __init__(self,
-                 returnInfo = ReturnInfo()):
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         return distribution of events into dmoz categories
         @param returnInfo: what details about the categories should be included in the returned information
         """
         self.resultType = "categoryAggr"
         self.__dict__.update(returnInfo.getParams("categoryAggr"))
 
 
 
 class RequestEventsRecentActivity(RequestEvents):
     def __init__(self,
-                 maxEventCount = 50,
-                 updatesAfterTm = None,
-                 updatesAfterMinsAgo = None,
-                 mandatoryLocation = True,
-                 minAvgCosSim = 0,
-                 returnInfo = None):
+                 maxEventCount: int = 50,
+                 updatesAfterTm: Union[datetime.datetime, datetime.date, str] = None,
+                 updatesAfterMinsAgo: int = None,
+                 mandatoryLocation: bool = True,
+                 minAvgCosSim: float = 0,
+                 returnInfo: ReturnInfo = None):
         """
         return a list of recently changed events that match search conditions
         @param maxEventCount: max events to return (at most 200)
         @param updatesAfterTm: the time after which the events were added/updated (returned by previous call to the same method)
         @param updatesAfterMinsAgo: how many minutes into the past should we check (set either this or updatesAfterTm property, but not both)
         @param mandatoryLocation: return only events that have a geographic location assigned to them
         @param minAvgCosSim: the minimum avg cos sim of the events to be returned (events with lower quality should not be included)
@@ -627,7 +636,30 @@
         if updatesAfterMinsAgo != None:
             self.recentActivityEventsUpdatesAfterMinsAgo = updatesAfterMinsAgo
         self.recentActivityEventsMinAvgCosSim = minAvgCosSim
         if returnInfo != None:
             self.__dict__.update(returnInfo.getParams("recentActivityEvents"))
 
 
+class RequestEventsBreakingEvents(RequestEvents):
+    def __init__(self,
+                 page: int = 1,
+                 count: int = 50,
+                 minBreakingScore: float = 0.2,
+                 returnInfo: ReturnInfo = None):
+        """
+        return a list of events that are currently breaking
+        @param page: max events to return (at most 50)
+        @param count: max events to return (at most 50)
+        @param minBreakingScore: the minimum score of "breakingness" of the events to be returned
+        @param returnInfo: what details should be included in the returned information
+        """
+        assert page >= 1
+        assert count <= 50
+        self.resultType = "breakingEvents"
+        self.breakingEventsPage = page
+        self.breakingEventsCount = count
+        self.breakingEventsMinBreakingScore = minBreakingScore
+        if returnInfo != None:
+            self.__dict__.update(returnInfo.getParams("breakingEvents"))
+
+
```

### Comparing `eventregistry-8.9/eventregistry/QueryStory.py` & `eventregistry-9.0/eventregistry/QueryStory.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 ﻿from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
+
 
 class QueryStory(Query):
     """
     Class for obtaining available info for one or more stories (clusters) in the Event Registry
     NOTE: Story in our terminology is a cluster of articles (and not a single article). An event is
     then something that consists of one or more stories (typically in different languages).
 
     @param storyUriOrList: a single story uri or a list of story uris
     """
-    def __init__(self, storyUriOrList = None):
+    def __init__(self, storyUriOrList: Union[str, List[str]] = None):
         super(QueryStory, self).__init__()
         self._setVal("action", "getStory")
         if storyUriOrList != None:
             self.queryByUri(storyUriOrList)
 
 
     def _getPath(self):
         return "/api/v1/story"
 
 
-    def queryByUri(self, uriOrUriList):
+    def queryByUri(self, uriOrUriList: Union[str, List[str]]):
         """search stories by their uri(s)"""
         self._setVal("storyUri", uriOrUriList)
 
 
-    def setRequestedResult(self, requestStory):
+    def setRequestedResult(self, requestStory: "RequestStory"):
         """
         Set the single result type that you would like to be returned. If some other request type was previously set, it will be overwritten.
         Result types can be the classes that extend RequestStory base class (see classes below).
         """
         assert isinstance(requestStory, RequestStory), "QueryStory class can only accept result requests that are of type RequestStory"
         self.resultTypeList = [requestStory]
 
@@ -45,29 +48,29 @@
 
 
 
 class RequestStoryInfo(RequestStory):
     """
     return details about a story
     """
-    def __init__(self, returnInfo = ReturnInfo()):
+    def __init__(self, returnInfo: ReturnInfo = ReturnInfo()):
         self.resultType = "info"
         self.__dict__.update(returnInfo.getParams("info"))
 
 
 
 class RequestStoryArticles(RequestStory):
     """
     return articles about the story
     """
     def __init__(self,
-                 page = 1,
-                 count = 100,
-                 sortBy = "cosSim", sortByAsc = False,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 200))):
+                 page: int = 1,
+                 count: int = 100,
+                 sortBy: str = "cosSim", sortByAsc: bool = False,
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 200))):
         """
         return articles in the story (cluster)
         @param page: page of the articles to return (1, 2, ...)
         @param count: number of articles to return per page (at most 100)
         @param sortBy: order in which articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         @param returnInfo: what details should be included in the returned information
@@ -84,15 +87,15 @@
 
 
 class RequestStoryArticleUris(RequestStory):
     """
     return a list of article uris
     """
     def __init__(self,
-                 sortBy = "cosSim", sortByAsc = False  # order in which story articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to story centroid), socialScore (total shares in social media), facebookShares (shares on fb), twitterShares (shares on twitter)
+                 sortBy: str = "cosSim", sortByAsc: bool = False  # order in which story articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to story centroid), socialScore (total shares in social media), facebookShares (shares on fb), twitterShares (shares on twitter)
                  ):
         """
         return articles in the story (cluster)
         @param sortBy: order in which articles are sorted. Options: id (internal id), date (published date), cosSim (closeness to event centroid), sourceImportanceRank (importance of the news source, custom set), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares in social media)
         @param sortByAsc: should the articles be sorted in ascending order (True) or descending (False) based on sortBy value
         """
         self.articleUrisSortBy = sortBy
@@ -102,17 +105,17 @@
 
 
 class RequestStoryArticleTrend(RequestStory):
     """
     return trending information for the articles about the story
     """
     def __init__(self,
-                 lang = mainLangs,
-                 minArticleCosSim = -1,
-                 returnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
+                 lang: Union[str, List[str]] = mainLangs,
+                 minArticleCosSim: float = -1,
+                 returnInfo: ReturnInfo = ReturnInfo(articleInfo = ArticleInfoFlags(bodyLen = 0))):
         self.resultType = "articleTrend"
         self.articleTrendLang = lang
         self.articleTrendMinArticleCosSim = minArticleCosSim
         self.__dict__.update(returnInfo.getParams("articleTrend"))
 
 
 
@@ -124,20 +127,20 @@
         @param dateStart: what can be the oldest date of the similar stories
         @param dateEnd: what can be the newest date of the similar stories
         @param addArticleTrendInfo: for the returned stories compute how they were trending (intensity of reporting) in different time periods
         @param aggrHours: time span that is used as a unit when computing the trending info
         @param returnInfo: what details should be included in the returned information
         """
     def __init__(self,
-                conceptInfoList,
-                count=50,                   # number of similar stories to return
-                dateStart = None,           # what can be the oldest date of the similar stories
-                dateEnd = None,             # what can be the newest date of the similar stories
-                lang = [],
-                returnInfo = ReturnInfo()):
+                conceptInfoList: Union[str, List[str]],
+                count: int = 50,                                    # number of similar stories to return
+                dateStart: Union[datetime.date, str] = None,        # what can be the oldest date of the similar stories
+                dateEnd: Union[datetime.date, str] = None,          # what can be the newest date of the similar stories
+                lang: Union[str, List[str]] = [],
+                returnInfo: ReturnInfo = ReturnInfo()):
         assert count <= 50
         assert isinstance(conceptInfoList, list)
         self.action = "getSimilarStories"
         self.concepts = json.dumps(conceptInfoList)
         self.storiesCount = count
         if dateStart != None:
             self.dateStart = QueryParamsBase.encodeDate(dateStart)
```

### Comparing `eventregistry-8.9/eventregistry/Recent.py` & `eventregistry-9.0/eventregistry/Recent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
 provides classes for getting new/updated events and articles
 """
 
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
 
 class GetRecentEvents(QueryParamsBase):
     def __init__(self,
-                 eventRegistry,
-                 mandatoryLang = None,
-                 mandatoryLocation = True,
-                 returnInfo = ReturnInfo(),
+                 eventRegistry: EventRegistry,
+                 mandatoryLang: Union[str, List[str]] = None,
+                 mandatoryLocation: bool = True,
+                 returnInfo: ReturnInfo = ReturnInfo(),
                  **kwargs):
         """
         Return info about recently added/modified events
         @param eventRegistry: instance of class EventRegistry
         @param mandatoryLang: set a lang or array of langs if you wish to only get events covered at least by the specified language
         @param mandatoryLocation: if set to True then return only events that have a known geographic location
         @param returnInfo: what details should be included in the returned information
@@ -49,18 +51,18 @@
         # or empty
         return {}
 
 
 
 class GetRecentArticles(QueryParamsBase):
     def __init__(self,
-                 eventRegistry,
-                 mandatorySourceLocation = False,
-                 articleLang = None,
-                 returnInfo = ReturnInfo(),
+                 eventRegistry: EventRegistry,
+                 mandatorySourceLocation: bool = False,
+                 articleLang: Union[str, List[str]] = None,
+                 returnInfo: ReturnInfo = ReturnInfo(),
                  **kwargs):
         """
         Return info about recently added articles
         @param eventRegistry: instance of class EventRegistry
         @param mandatorySourceLocation: if True then return only articles from sources for which we know geographic location
         @param articleLang: None, string or a list of strings, depending if we should return all articles, or articles in one or more languages
         @param returnInfo: what details should be included in the returned information
```

### Comparing `eventregistry-8.9/eventregistry/ReturnInfo.py` & `eventregistry-9.0/eventregistry/ReturnInfo.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,24 @@
     def _getFlags(self):
         """return the dict of stored flags"""
         if not hasattr(self, "flags"):
             self.flags = {}
         return self.flags
 
 
-    def _setVal(self, name, val, defVal = None):
+    def _setVal(self, name: str, val, defVal = None):
         """set value of name to val in case the val != defVal"""
         if val == defVal:
             return
         if not hasattr(self, "vals"):
             self.vals = {}
         self.vals[name] = val
 
 
-    def _getVals(self, prefix = ""):
+    def _getVals(self, prefix: str = ""):
         """
         return the values in the vals dict
         in case prefix is "", change the first letter of the name to lowercase, otherwise use prefix+name as the new name
         """
         if not hasattr(self, "vals"):
             self.vals = {}
         dict = {}
@@ -84,32 +84,32 @@
     @param location: the geographic location that the event mentioned in the article is about
     @param dates: the dates when the articles was crawled and the date when it was published (based on the rss feed date)
     @param extractedDates: the list of dates found mentioned in the article
     @param originalArticle: if the article is a duplicate, this will provide information about the original article
     @param storyUri: uri of the story (cluster) to which the article belongs
     """
     def __init__(self,
-                 bodyLen = -1,
-                 basicInfo = True,
-                 title = True,
-                 body = True,
-                 url = True,
-                 eventUri = True,
-                 authors = True,
-                 concepts = False,
-                 categories = False,
-                 links = False,
-                 videos = False,
-                 image = True,
-                 socialScore = False,
-                 sentiment = True,
-                 location = False,
-                 extractedDates = False,
-                 originalArticle = False,
-                 storyUri=False,
+                 bodyLen: int = -1,
+                 basicInfo: bool = True,
+                 title: bool = True,
+                 body: bool = True,
+                 url: bool = True,
+                 eventUri: bool = True,
+                 authors: bool = True,
+                 concepts: bool = False,
+                 categories: bool = False,
+                 links: bool = False,
+                 videos: bool = False,
+                 image: bool = True,
+                 socialScore: bool = False,
+                 sentiment: bool = True,
+                 location: bool = False,
+                 extractedDates: bool = False,
+                 originalArticle: bool = False,
+                 storyUri: bool = False,
                  **kwdArgs):
         self._setVal("articleBodyLen", bodyLen, -1)
         self._setFlag("includeArticleBasicInfo", basicInfo, True)
         self._setFlag("includeArticleTitle", title, True)
         self._setFlag("includeArticleBody", body, True)
         self._setFlag("includeArticleUrl", url, True)
         self._setFlag("includeArticleEventUri", eventUri, True)
@@ -143,26 +143,26 @@
     @param medoidArticle: the article that is closest to the center of the cluster of articles assigned to the story
     @param infoArticle: the article from which we have extracted the title and summary for the story
     @param commonDates: dates that were frequently identified in the articles belonging to the story
     @param socialScore: score computed based on how frequently the articles in the story were shared on social media
     @param imageCount: number of images to be returned for a story
     """
     def __init__(self,
-                basicStats = True,
-                location = True,
-                date = False,
-                title = False,
-                summary = False,
-                concepts = False,
-                categories = False,
-                medoidArticle = False,
-                infoArticle = False,
-                commonDates = False,
-                socialScore = False,
-                imageCount = 0,
+                basicStats: bool = True,
+                location: bool = True,
+                date: bool = False,
+                title: bool = False,
+                summary: bool = False,
+                concepts: bool = False,
+                categories: bool = False,
+                medoidArticle: bool = False,
+                infoArticle: bool = False,
+                commonDates: bool = False,
+                socialScore: bool = False,
+                imageCount: int = 0,
                 **kwdArgs):
         self._setFlag("includeStoryBasicStats", basicStats, True)
         self._setFlag("includeStoryLocation", location, True)
         self._setFlag("includeStoryDate", date, False)
         self._setFlag("includeStoryTitle", title, False)
         self._setFlag("includeStorySummary", summary, False)
         self._setFlag("includeStoryConcepts", concepts, False)
@@ -190,26 +190,26 @@
     @param commonDates: return the dates that were commonly found in the articles about the event
     @param infoArticle: return for each language the article from which we have extracted the summary and title for event for that language
     @param stories: return the list of stories (clusters) that are about the event
     @param socialScore: score computed based on how frequently the articles in the event were shared on social media
     @param imageCount: number of images to be returned for an event
     """
     def __init__(self,
-                title = True,
-                summary = True,
-                articleCounts = True,
-                concepts = True,
-                categories = True,
-                location = True,
-                date = True,
-                commonDates = False,
-                infoArticle = False,
-                stories = False,
-                socialScore = False,
-                imageCount = 0,
+                title: bool = True,
+                summary: bool = True,
+                articleCounts: bool = True,
+                concepts: bool = True,
+                categories: bool = True,
+                location: bool = True,
+                date: bool = True,
+                commonDates: bool = False,
+                infoArticle: bool = False,
+                stories: bool = False,
+                socialScore: bool = False,
+                imageCount: int = 0,
                 **kwdArgs):
         self._setFlag("includeEventTitle", title, True)
         self._setFlag("includeEventSummary", summary, True)
         self._setFlag("includeEventArticleCounts", articleCounts, True)
         self._setFlag("includeEventConcepts", concepts, True)
         self._setFlag("includeEventCategories", categories, True)
         self._setFlag("includeEventLocation", location, True)
@@ -220,32 +220,55 @@
         self._setFlag("includeEventStories", stories, False)
         self._setFlag("includeEventSocialScore", socialScore, False)
         self._setVal("eventImageCount", imageCount, 0)
         self._addKwdArgs(kwdArgs)
 
 
 
+class MentionInfoFlags(ReturnInfoFlagsBase):
+    """
+    What information about a mention should be returned by the API call
+
+    @param basicInfo: return basic information about the mention
+    @param slots: return the list of slots (concepts) related to the mention
+    @param categories: return the list of categories associated with the article that contains the sentence from the mention
+    @param frameworks: return list of frameworks to which the event type of the mention belongs
+    """
+    def __init__(self,
+                basicInfo: bool = True,
+                slots: bool = True,
+                categories: bool = False,
+                frameworks: bool = True,
+                **kwdArgs):
+        self._setFlag("includeMentionBasicInfo", basicInfo, True)
+        self._setFlag("includeMentionSlots", slots, True)
+        self._setFlag("includeMentionCategories", categories, False)
+        self._setFlag("includeMentionFrameworks", frameworks, True)
+        self._addKwdArgs(kwdArgs)
+
+
+
 class SourceInfoFlags(ReturnInfoFlagsBase):
     """
     What information about a news source should be returned by the API call
 
     @param title: title of the news source
     @param description: description of the news source
     @param location: geographic location of the news source
     @param ranking: a set of rankings for the news source
     @param image: different images associated with the news source
     @param socialMedia: different social media accounts used by the news source
     """
     def __init__(self,
-                title = True,
-                description = False,
-                location = False,
-                ranking = False,
-                image = False,
-                socialMedia = False,
+                title: bool = True,
+                description: bool = False,
+                location: bool = False,
+                ranking: bool = False,
+                image: bool = False,
+                socialMedia: bool = False,
                 **kwdArgs):
         self._setFlag("includeSourceTitle", title, True)
         self._setFlag("includeSourceDescription", description, False)
         self._setFlag("includeSourceLocation", location, False)
         self._setFlag("includeSourceRanking", ranking, False)
         self._setFlag("includeSourceImage", image, False)
         self._setFlag("includeSourceSocialMedia", socialMedia, False)
@@ -256,15 +279,15 @@
 class CategoryInfoFlags(ReturnInfoFlagsBase):
     """
     What information about a category should be returned by the API call
 
     @param trendingScore: information about how the category is currently trending. The score is computed as Pearson residual by comparing the trending of the category in last 2 days compared to last 14 days
     """
     def __init__(self,
-                trendingScore = False,
+                trendingScore: bool = False,
                 **kwdArgs):
         self._setFlag("includeCategoryTrendingScore", trendingScore, False)
         self._addKwdArgs(kwdArgs)
 
 
 
 class ConceptInfoFlags(ReturnInfoFlagsBase):
@@ -278,22 +301,22 @@
     @param image: provide an image associated with the concept
     @param description: description of the concept
     @param trendingScore: information about how the concept is currently trending. The score is computed as Pearson residual by comparing the trending of the concept in last 2 days compared to last 14 days
     @type type: str | list
     @type lang: str | list
     """
     def __init__(self,
-                type = "concepts",
-                lang = "eng",
-                label = True,
-                synonyms = False,
-                image = False,
-                description = False,
-                trendingScore = False,
-                maxConceptsPerType = 20,
+                type: str = "concepts",
+                lang: str = "eng",
+                label: bool = True,
+                synonyms: bool = False,
+                image: bool = False,
+                description: bool = False,
+                trendingScore: bool = False,
+                maxConceptsPerType: int = 20,
                 **kwdArgs):
         self._setVal("conceptType", type, "concepts")
         self._setVal("conceptLang", lang, "eng")
         self._setFlag("includeConceptLabel", label, True)
         self._setFlag("includeConceptSynonyms", synonyms, False)
         self._setFlag("includeConceptImage", image, False)
         self._setFlag("includeConceptDescription", description, False)
@@ -318,26 +341,26 @@
     @param countryDetails: return additional details about the country
     @param countryContinent: return continent where the country is located
 
     @param placeFeatureCode: return the geonames feature code of the place
     @param placeCountry: return information about the country where the place is located
     """
     def __init__(self,
-                label = True,
-                wikiUri = False,
-                geoNamesId = False,
-                population = False,
-                geoLocation = False,
-
-                countryArea = False,
-                countryDetails = False,
-                countryContinent = False,
+                label: bool = True,
+                wikiUri: bool = False,
+                geoNamesId: bool = False,
+                population: bool = False,
+                geoLocation: bool = False,
+
+                countryArea: bool = False,
+                countryDetails: bool = False,
+                countryContinent: bool = False,
 
-                placeFeatureCode = False,
-                placeCountry = True,
+                placeFeatureCode: bool = False,
+                placeCountry: bool = True,
                 **kwdArgs):
         self._setFlag("includeLocationLabel", label, True)
         self._setFlag("includeLocationWikiUri", wikiUri, False)
         self._setFlag("includeLocationGeoNamesId", geoNamesId, False)
         self._setFlag("includeLocationPopulation", population, False)
         self._setFlag("includeLocationGeoLocation", geoLocation, False)
 
@@ -355,16 +378,16 @@
     """
     What information about a concept class should be returned by the API call
 
     @param parentLabels: return the list of labels of the parent concept classes
     @param concepts: return the list of concepts assigned to the concept class
     """
     def __init__(self,
-                parentLabels = True,
-                concepts = False,
+                parentLabels: bool = True,
+                concepts: bool = False,
                 **kwdArgs):
         self._setFlag("includeConceptClassParentLabels", parentLabels, True)
         self._setFlag("includeConceptClassConcepts", concepts, False)
         self._addKwdArgs(kwdArgs)
 
 
 
@@ -372,16 +395,16 @@
     """
     What information about a concept folder should be returned by the API call
 
     @param definition: return the complete definition of the concept folder
     @param owner: return information about the owner of the concept folder
     """
     def __init__(self,
-                definition = False,
-                owner = False,
+                definition: bool = False,
+                owner: bool = False,
                 **kwdArgs):
         self._setFlag("includeConceptFolderDefinition", definition, False)
         self._setFlag("includeConceptFolderOwner", owner, False)
         self._addKwdArgs(kwdArgs)
 
 
 
@@ -392,74 +415,64 @@
     @param articleInfo: what details about the articles should be returned
     @param eventInfo: what details about the event should be returned
     @param sourceInfo: what details about the article's news source should be returned
     @param storyInfo: what details about the stories (clusters) should be returned
     @param categoryInfo: what details about the categories should be returned
     @param conceptInfo: what details about the concepts should be returned
     @param locationInfo: what details about the locations should be returned (locations are sub-types of concepts so their information will be a property inside the concept information)
-    @param conceptClassInfo: what details about the concept classes should be returned (concept classes are sub-types of concepts so their information will be a property inside the concept information)
+    @param mentionInfo: what details about the mention should be returned
     @param conceptFolderInfo: what details about the concept folders should be returned (concept folders are sub-types of concepts so their information will be a property inside the concept information)
-
-    @type articleInfo: ArticleInfoFlags
-    @type eventInfo: EventInfoFlags
-    @type sourceInfo: SourceInfoFlags
-    @type storyInfo: StoryInfoFlags
-    @type categoryInfo: CategoryInfoFlags
-    @type conceptInfo: ConceptInfoFlags
-    @type locationInfo: LocationInfoFlags
-    @type conceptClassInfo: ConceptClassInfoFlags
-    @type conceptFolderInfo: ConceptFolderInfoFlags
-    """
-    def __init__(self,
-                 articleInfo = ArticleInfoFlags(),
-                 eventInfo = EventInfoFlags(),
-                 sourceInfo = SourceInfoFlags(),
-                 categoryInfo = CategoryInfoFlags(),
-                 conceptInfo = ConceptInfoFlags(),
-                 locationInfo = LocationInfoFlags(),
-                 storyInfo = StoryInfoFlags(),
-                 conceptClassInfo = ConceptClassInfoFlags(),
-                 conceptFolderInfo = ConceptFolderInfoFlags()):
+    """
+    def __init__(self,
+                 articleInfo : ArticleInfoFlags = ArticleInfoFlags(),
+                 eventInfo : EventInfoFlags = EventInfoFlags(),
+                 sourceInfo : SourceInfoFlags = SourceInfoFlags(),
+                 categoryInfo : CategoryInfoFlags = CategoryInfoFlags(),
+                 conceptInfo : ConceptInfoFlags = ConceptInfoFlags(),
+                 locationInfo : LocationInfoFlags = LocationInfoFlags(),
+                 storyInfo : StoryInfoFlags = StoryInfoFlags(),
+                 mentionInfo : MentionInfoFlags = MentionInfoFlags(),
+                 conceptFolderInfo : ConceptFolderInfoFlags= ConceptFolderInfoFlags()):
         assert isinstance(articleInfo, ArticleInfoFlags)
         assert isinstance(eventInfo, EventInfoFlags)
         assert isinstance(sourceInfo, SourceInfoFlags)
         assert isinstance(categoryInfo, CategoryInfoFlags)
         assert isinstance(conceptInfo, ConceptInfoFlags)
         assert isinstance(locationInfo, LocationInfoFlags)
         assert isinstance(storyInfo, StoryInfoFlags)
-        assert isinstance(conceptClassInfo, ConceptClassInfoFlags)
+        assert isinstance(mentionInfo, MentionInfoFlags)
         assert isinstance(conceptFolderInfo, ConceptFolderInfoFlags)
         self.articleInfo = articleInfo
         self.eventInfo = eventInfo
         self.sourceInfo = sourceInfo
         self.categoryInfo = categoryInfo
         self.conceptInfo = conceptInfo
         self.locationInfo = locationInfo
         self.storyInfo = storyInfo
-        self.conceptClassInfo = conceptClassInfo
+        self.mentionInfo = mentionInfo
         self.conceptFolderInfo = conceptFolderInfo
 
 
     @staticmethod
-    def loadFromFile(fileName):
+    def loadFromFile(fileName: str):
         """
         load the configuration for the ReturnInfo from a fileName
         @param fileName: filename that contains the json configuration to use in the ReturnInfo
         """
         assert os.path.exists(fileName), "File " + fileName + " does not exist"
         conf = json.load(open(fileName))
         return ReturnInfo(
             articleInfo=ArticleInfoFlags(**conf.get("articleInfo", {})),
             eventInfo=EventInfoFlags(**conf.get("eventInfo", {})),
             sourceInfo=SourceInfoFlags(**conf.get("sourceInfo", {})),
             categoryInfo=CategoryInfoFlags(**conf.get("categoryInfo", {})),
             conceptInfo=ConceptInfoFlags(**conf.get("conceptInfo", {})),
             locationInfo=LocationInfoFlags(**conf.get("locationInfo", {})),
             storyInfo=StoryInfoFlags(**conf.get("storyInfo", {})),
-            conceptClassInfo=ConceptClassInfoFlags(**conf.get("conceptClassInfo", {})),
+            mentionInfo=MentionInfoFlags(**conf.get("mentionInfo", {})),
             conceptFolderInfo=ConceptFolderInfoFlags(**conf.get("conceptFolderInfo", {}))
         )
 
 
     def getConf(self):
         """
         return configuration in a json object that stores properties set by each *InfoFlags class
@@ -468,45 +481,45 @@
             "articleInfo": self.articleInfo._getFlags().copy(),
             "eventInfo": self.eventInfo._getFlags().copy(),
             "sourceInfo": self.sourceInfo._getFlags().copy(),
             "categoryInfo":  self.categoryInfo._getFlags().copy(),
             "conceptInfo": self.conceptInfo._getFlags().copy(),
             "locationInfo": self.locationInfo._getFlags().copy(),
             "storyInfo": self.storyInfo._getFlags().copy(),
-            "conceptClassInfo": self.articleInfo._getFlags().copy(),
+            "mentionInfo": self.mentionInfo._getFlags().copy(),
             "conceptFolderInfo": self.articleInfo._getFlags().copy()
         }
         conf["articleInfo"].update(self.articleInfo._getVals())
         conf["eventInfo"].update(self.eventInfo._getVals())
         conf["sourceInfo"].update(self.sourceInfo._getVals())
         conf["categoryInfo"].update(self.categoryInfo._getVals())
         conf["conceptInfo"].update(self.conceptInfo._getVals())
         conf["locationInfo"].update(self.locationInfo._getVals())
         conf["storyInfo"].update(self.storyInfo._getVals())
-        conf["conceptClassInfo"].update(self.conceptClassInfo._getVals())
+        conf["mentionInfo"].update(self.mentionInfo._getVals())
         conf["conceptFolderInfo"].update(self.conceptFolderInfo._getVals())
         return conf
 
 
     def getParams(self, prefix = ""):
         dict = {}
         dict.update(self.articleInfo._getFlags())
         dict.update(self.eventInfo._getFlags())
         dict.update(self.sourceInfo._getFlags())
         dict.update(self.conceptInfo._getFlags())
         dict.update(self.categoryInfo._getFlags())
         dict.update(self.locationInfo._getFlags())
         dict.update(self.storyInfo._getFlags())
-        dict.update(self.conceptClassInfo._getFlags())
+        dict.update(self.mentionInfo._getFlags())
         dict.update(self.conceptFolderInfo._getFlags())
 
         dict.update(self.articleInfo._getVals())
         dict.update(self.eventInfo._getVals())
         dict.update(self.sourceInfo._getVals())
         dict.update(self.conceptInfo._getVals())
         dict.update(self.categoryInfo._getVals())
         dict.update(self.locationInfo._getVals())
         dict.update(self.storyInfo._getVals())
-        dict.update(self.conceptClassInfo._getVals())
+        dict.update(self.mentionInfo._getVals())
         dict.update(self.conceptFolderInfo._getVals())
         return dict
```

### Comparing `eventregistry-8.9/eventregistry/TopicPage.py` & `eventregistry-9.0/eventregistry/TopicPage.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,41 @@
 class that provides the ability to use topic pages (monitoring functionality)
 through the API
 """
 
 import six, json
 from eventregistry.Base import *
 from eventregistry.ReturnInfo import *
+from eventregistry.EventRegistry import EventRegistry
+from typing import Union, List
+
+
+class TopicPages(QueryParamsBase):
+    """
+    get the list of user owned topic pages
+    """
+    def __init__(self, eventRegistry: EventRegistry):
+        """
+        create an instance of a topic page
+
+        @param eventRegistry: instance of class EventRegistry
+        """
+        self.eventRegistry = eventRegistry
+
+    def getMyTopicPages(self):
+        """
+        get the list of topic pages owned by me
+        """
+        userProfile = self.eventRegistry.jsonRequest("/api/v1/user/getUserProfile", {})
+        return userProfile.get("ownedTopicPages", [])
+
+
 
 class TopicPage(QueryParamsBase):
-    def __init__(self, eventRegistry):
+    def __init__(self, eventRegistry: EventRegistry):
         """
         create an instance of a topic page
 
         @param eventRegistry: instance of class EventRegistry
         """
         self.eventRegistry = eventRegistry
         # topic page definition
@@ -44,15 +68,15 @@
             "restrictToSetSources": False,
             "restrictToSetLocations": False,
 
             "dataType": [ "news" ]
         }
 
 
-    def loadTopicPageFromER(self, uri):
+    def loadTopicPageFromER(self, uri: str):
         """
         load an existing topic page from Event Registry based on the topic page URI
         @param uri: uri of the topic page saved in your Event Registry account
         """
         params = {
             "action": "getTopicPageJson",
             "includeConceptDescription": True,
@@ -62,23 +86,23 @@
             "uri": uri
         }
         self.topicPage = self._createEmptyTopicPage()
         self.concept = self.eventRegistry.jsonRequest("/api/v1/topicPage", params)
         self.topicPage.update(self.concept.get("topicPage", {}))
 
 
-    def loadTopicPageFromDefinition(self, definitionDict):
+    def loadTopicPageFromDefinition(self, definitionDict: dict):
         """
         load the topic page definition from a python dictionary
         """
         assert isinstance(definitionDict, dict)
         self.topicPage = definitionDict
 
 
-    def loadTopicPageFromFile(self, fname):
+    def loadTopicPageFromFile(self, fname: str):
         """
         load topic page from an existing file
         """
         assert os.path.exists(fname)
         f = open(fname, "r", encoding="utf-8")
         self.topicPage = json.load(f)
 
@@ -86,105 +110,115 @@
     def saveTopicPageDefinition(self):
         """
         return a python dict containing the topic page definition. you can use it to load a topic page later
         """
         return self.topicPage
 
 
-    def saveTopicPageDefinitionToFile(self, fname):
+    def saveTopicPageDefinitionToFile(self, fname: str):
         """
         save the topic page definition to a file
         """
         open(fname, "w", encoding="utf-8").write(json.dumps(self.topicPage, indent = 4, sort_keys = True))
 
     #
     # methods for adding filters to the topic
     #
 
-    def setArticleThreshold(self, value):
+    def setArticleThreshold(self, value: int):
         """
         what is the minimum total weight that an article has to have in order to get it among the results?
         @param value: threshold to use
         """
         assert isinstance(value, int)
         assert value >= 0
         self.topicPage["articleTreshWgt"] = value
 
 
-    def setEventThreshold(self, value):
+    def setEventThreshold(self, value: int):
         """
         what is the minimum total weight that an event has to have in order to get it among the results?
         @param value: threshold to use
         """
         assert isinstance(value, int)
         assert value >= 0
         self.topicPage["eventTreshWgt"] = value
 
 
-    def setArticleIsDuplicateFilter(self, value):
+    def setArticleIsDuplicateFilter(self, value: str):
         """
         @param value: some articles can be duplicates of other articles. What should be done with them. Possible values are:
             "skipDuplicates" (skip the resulting articles that are duplicates of other articles)
             "keepOnlyDuplicates" (return only the duplicate articles)
             "keepAll" (no filtering, default)
         """
         assert value == "skipDuplicates" or value == "keepOnlyDuplicates" or value == "keepAll"
         self.topicPage["isDuplicateFilter"] = value
 
 
-    def setArticleHasEventFilter(self, value):
+    def setArticleHasEventFilter(self, value: str):
         """
         @param value: some articles describe a known event and some don't. This filter allows you to filter the resulting articles based on this criteria.
             Possible values are:
             "skipArticlesWithoutEvent" (skip articles that are not describing any known event in ER)
             "keepOnlyArticlesWithoutEvent" (return only the articles that are not describing any known event in ER)
             "keepAll" (no filtering, default)
         """
         assert value == "skipArticlesWithoutEvent" or value == "keepOnlyArticlesWithoutEvent" or value == "keepAll"
         self.topicPage["articleHasEvent"] = value
 
 
-    def setArticleHasDuplicateFilter(self, value):
+    def setArticleHasDuplicateFilter(self, value: str):
         """
         @param value: some articles are later copied by others. What should be done with such articles. Possible values are:
             "skipHasDuplicates" (skip the articles that have been later copied by others)
             "keepOnlyHasDuplicates" (return only the articles that have been later copied by others)
             "keepAll" (no filtering, default)
         """
         assert value == "skipHasDuplicates" or value == "keepOnlyHasDuplicates" or value == "keepAll"
         self.topicPage["articleHasDuplicate"] = value
 
 
-    def setDataTypes(self, dataTypes):
+    def setDataTypes(self, dataTypes: Union[str, List[str]]):
         """
         what data types should we search? "news" (news content, default), "pr" (press releases), or "blog".
             If you want to use multiple data types, put them in an array (e.g. ["news", "pr"])
         """
         self.topicPage["dataType"] = dataTypes
 
 
-    def setMaxDaysBack(self, maxDaysBack):
+    def setMaxDaysBack(self, maxDaysBack: int):
         """
         what is the maximum allowed age of the results?
         """
         assert isinstance(maxDaysBack, int), "maxDaysBack value has to be a positive integer"
         assert maxDaysBack >= 1
         self.topicPage["maxDaysBack"] = maxDaysBack
 
 
-    def setSourceRankPercentile(self, startPercentile=0, endPercentile=100):
+    def setSourceRankPercentile(self, startPercentile: int = 0, endPercentile: int = 100):
         assert startPercentile >= 0 and startPercentile <= 90, "startPercentile is out of valid values (0 - 90)"
         assert endPercentile >= 10 and endPercentile <= 100, "endPercentile is out of valid values (10 - 100)"
         assert startPercentile < endPercentile, "startPercentile has to be smaller than endPercentile"
         assert startPercentile % 10 == 0, "startPecentile has to be a multiple of 10"
         assert endPercentile % 10 == 0, "endPercentile has to be a multiple of 10"
         self.topicPage["startSourceRankPercentile"] = startPercentile
         self.topicPage["endSourceRankPercentile"] = endPercentile
 
 
+    def setSentiment(self, minSentiment: float = -1, maxSentiment: float = 1):
+        """
+        what should be the sentiment of the returned articles and events?
+        """
+        assert minSentiment >= -1, "minSentiment has to be >= -1"
+        assert maxSentiment <= 1, "maxSentiment has to be <= 1"
+        self.topicPage["minSentiment"] = minSentiment
+        self.topicPage["maxSentiment"] = maxSentiment
+
+
     def clearConcepts(self):
         self.topicPage["concepts"] = []
 
 
     def clearKeywords(self):
         self.topicPage["keywords"] = []
 
@@ -205,155 +239,156 @@
         self.topicPage["sourceGroups"] = []
 
 
     def clearLocations(self):
         self.topicPage["locations"] = []
 
 
-    def addConcept(self, conceptUri, weight, label = None, conceptType = None, required = False, excluded = False):
+    def addConcept(self, conceptUri: str, weight: float, label: str = None, conceptType: str = None, required: bool = False, excluded: bool = False):
         """
         add a relevant concept to the topic page
         @param conceptUri: uri of the concept to be added
         @param weight: importance of the provided concept (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO be annotated with this concept
         @param excluded: if true, then all results annotated with this concept will be ignored
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
         concept = {"uri": conceptUri, "wgt": weight, "required": required, "excluded": excluded }
-        if label != None: concept["label"] = label
-        if conceptType != None: concept["type"] = conceptType
+        if label != None:
+            concept["label"] = label
+        if conceptType != None:
+            concept["type"] = conceptType
         self.topicPage["concepts"].append(concept)
 
 
-    def addKeyword(self, keyword, weight, required = False, excluded = False):
+    def addKeyword(self, keyword: str, weight: float, required: bool = False, excluded: bool = False):
         """
         add a relevant keyword to the topic page
         @param keyword: keyword or phrase to be added
         @param weight: importance of the provided keyword (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO mention this keyword to appear in the results
         @param excluded: if true, then no results that mention this keyword will be returned
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
         self.topicPage["keywords"].append({"keyword": keyword, "wgt": weight, "required": required, "excluded": excluded })
 
 
-    def addCategory(self, categoryUri, weight, required = False, excluded = False):
+    def addCategory(self, categoryUri: str, weight: float, required: bool = False, excluded: bool = False):
         """
         add a relevant category to the topic page
         @param categoryUri: uri of the category to be added
         @param weight: importance of the provided category (typically in range 1 - 50)
         @param required: if true, then all results will HAVE TO be annotated with this category to appear in the results
         @param excluded: if true, then no results with this category will be returned
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         assert not (required == True and excluded == True), "Parameters required and excluded can not be True at the same time"
         self.topicPage["categories"].append({"uri": categoryUri, "wgt": weight, "required": required, "excluded": excluded })
 
 
-    def addSource(self, sourceUri, weight, excluded = False):
+    def addSource(self, sourceUri: str, weight: float, excluded: bool = False):
         """
         add a news source to the topic page
         @param sourceUri: uri of the news source to add to the topic page
         @param weight: importance of the news source (typically in range 1 - 50)
         @param excluded: if true, then the results from these sources will be ignored
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         self.topicPage["sources"].append({"uri": sourceUri, "wgt": weight, "excluded": excluded })
 
 
-    def addSourceLocation(self, sourceLocationUri, weight, excluded = False):
+    def addSourceLocation(self, sourceLocationUri: str, weight: float, excluded: bool = False):
         """
         add a list of relevant sources by identifying them by their geographic location
         @param sourceLocationUri: uri of the location where the sources should be geographically located
         @param weight: importance of the provided list of sources (typically in range 1 - 50)
         @param excluded: if true, then the results from the sources from this location will be ignored
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         self.topicPage["sourceLocations"].append({"uri": sourceLocationUri, "wgt": weight, "excluded": excluded })
 
 
-    def addSourceGroup(self, sourceGroupUri, weight, excluded = False):
+    def addSourceGroup(self, sourceGroupUri: str, weight: float, excluded: bool = False):
         """
         add a list of relevant sources by specifying a whole source group to the topic page
         @param sourceGroupUri: uri of the source group to add
         @param weight: importance of the provided list of sources (typically in range 1 - 50)
         @param excluded: if true, then the results from sources from this group will be ignored
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         self.topicPage["sourceGroups"].append({"uri": sourceGroupUri, "wgt": weight, "excluded": excluded })
 
 
-    def addLocation(self, locationUri, weight):
+    def addLocation(self, locationUri: str, weight: float):
         """
         add relevant location to the topic page
         @param locationUri: uri of the location to add
         @param weight: importance of the provided location (typically in range 1 - 50)
         """
         assert isinstance(weight, (float, int)), "weight value has to be a positive or negative integer"
         self.topicPage["locations"].append({"uri": locationUri, "wgt": weight})
 
 
-    def setLanguages(self, languages):
+    def setLanguages(self, languages: Union[str, List[str]]):
         """
         restrict the results to the list of specified languages
         """
         if isinstance(languages, six.string_types):
             languages = [languages]
         for lang in languages:
             assert len(lang) == 3, "Expected to get language in ISO3 code"
         self.topicPage["langs"] = languages
 
 
-    def restrictToSetConceptsAndKeywords(self, restrict):
+    def restrictToSetConceptsAndKeywords(self, restrict: bool):
         """
         if true then the results have to mention at least one of the specified concepts or keywords
         """
         assert isinstance(restrict, bool), "restrict value has to be a boolean value"
         self.topicPage["restrictToSetConcepts"] = restrict
 
 
-    def restrictToSetCategories(self, restrict):
+    def restrictToSetCategories(self, restrict: bool):
         """
         if set to true then return only results that are assigned to one of the specified categories
         """
         assert isinstance(restrict, bool), "restrict value has to be a boolean value"
         self.topicPage["restrictToSetCategories"] = restrict
 
 
-    def restrictToSetSources(self, restrict):
+    def restrictToSetSources(self, restrict: bool):
         """
         if set to true then return only results from one of the specified news sources
         this includes also sources set by source groups or by source locations
         """
         assert isinstance(restrict, bool), "restrict value has to be a boolean value"
         self.topicPage["restrictToSetSources"] = restrict
 
 
-    def restrictToSetLocations(self, restrict):
+    def restrictToSetLocations(self, restrict: bool):
         """
         if set to true, then return only results that are located at one of the specified locations
         """
         assert isinstance(restrict, bool), "restrict value has to be a boolean value"
         self.topicPage["restrictToSetLocations"] = restrict
 
 
     #
     # getting content
     #
 
 
     def getArticles(self,
-                page=1,
-                count=100,
-                sortBy = "rel",
-                sortByAsc = False,
-                dataType = "news",
-                returnInfo=ReturnInfo(),
+                page: int = 1,
+                count: int = 100,
+                sortBy: str = "rel",
+                sortByAsc: bool = False,
+                returnInfo: ReturnInfo = ReturnInfo(),
                 **kwargs):
         """
         return a list of articles that match the topic page
         @param page: which page of the results to return (default: 1)
         @param count: number of articles to return (default: 100)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
@@ -373,19 +408,19 @@
         }
         params.update(returnInfo.getParams("articles"))
         params.update(kwargs)
         return self.eventRegistry.jsonRequest("/api/v1/article", params)
 
 
     def getEvents(self,
-                page=1,
-                count=50,
-                sortBy = "rel",
-                sortByAsc = False,
-                returnInfo=ReturnInfo(),
+                page: int = 1,
+                count: int = 50,
+                sortBy: str = "rel",
+                sortByAsc: bool = False,
+                returnInfo: ReturnInfo = ReturnInfo(),
                 **kwargs):
         """
         return a list of events that match the topic page
         @param page: which page of the results to return (default: 1)
         @param count: number of articles to return (default: 50)
         @param sortBy: how are articles sorted. Options: id (internal id), date (publishing date), cosSim (closeness to the event centroid), rel (relevance to the query), sourceImportance (manually curated score of source importance - high value, high importance), sourceImportanceRank (reverse of sourceImportance), sourceAlexaGlobalRank (global rank of the news source), sourceAlexaCountryRank (country rank of the news source), socialScore (total shares on social media), facebookShares (shares on Facebook only)
         @param sortByAsc: should the results be sorted in ascending order (True) or descending (False)
@@ -395,12 +430,14 @@
         assert count <= 50
         params = {
             "action": "getEventsForTopicPage",
             "resultType": "events",
             "dataType": self.topicPage["dataType"],
             "eventsCount": count,
             "eventsPage": page,
+            "eventsSortBy": sortBy,
+            "eventsSortByAsc": sortByAsc,
             "topicPage": json.dumps(self.topicPage)
         }
         params.update(returnInfo.getParams("events"))
         params.update(kwargs)
         return self.eventRegistry.jsonRequest("/api/v1/event", params)
```

### Comparing `eventregistry-8.9/eventregistry/Trends.py` & `eventregistry-9.0/eventregistry/Trends.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 class TrendsBase(QueryParamsBase):
     def _getPath(self):
         return "/api/v1/trends"
 
 
 class GetTrendingConcepts(TrendsBase):
     def __init__(self,
-                 source = "news",
-                 count = 20,
-                 conceptType = ["person", "org", "loc"],
-                 returnInfo = ReturnInfo()):
+                 source: str = "news",
+                 count: int = 20,
+                 conceptType: Union[str, List[str]] = ["person", "org", "loc"],
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending concepts
         @param source: source information from which to compute top trends. Options: "news", "social", "pr", "blogs"
         @param count: number of top trends to return
         @param conceptType: which types of concepts are we interested in
         @param returnInfo: what details should be included in the returned information
         """
@@ -35,17 +35,17 @@
         self._setVal("conceptType", conceptType)
         self._update(returnInfo.getParams())
 
 
 
 class GetTrendingCategories(TrendsBase):
     def __init__(self,
-                 source = "news",
-                 count = 20,
-                 returnInfo = ReturnInfo()):
+                 source: str = "news",
+                 count: int = 20,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending categories
         @param source: source information from which to compute top trends. Options: "news", "social", "pr", "blogs"
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
         QueryParamsBase.__init__(self)
@@ -56,16 +56,16 @@
         self._setVal("categoryCount", count)
         self._update(returnInfo.getParams())
 
 
 
 class GetTrendingCustomItems(TrendsBase):
     def __init__(self,
-                 count = 20,
-                 returnInfo = ReturnInfo()):
+                 count: int = 20,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending items for which the users provided the data
         this data can be stock prices, energy prices, etc...
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
         QueryParamsBase.__init__(self)
@@ -73,33 +73,33 @@
         self._setVal("conceptCount", count)
         self._update(returnInfo.getParams())
 
 
 
 class GetTrendingConceptGroups(TrendsBase):
     def __init__(self,
-                 source = "news",
-                 count = 20,
-                 returnInfo = ReturnInfo()):
+                 source: str = "news",
+                 count: int = 20,
+                 returnInfo: ReturnInfo = ReturnInfo()):
         """
         get currently top trending groups of concepts
         a group can be identified by the concept type or by a concept class uri
         @param source: source information from which to compute top trends. Options: "news", "social"
         @param count: number of top trends to return
         @param returnInfo: what details should be included in the returned information
         """
         QueryParamsBase.__init__(self)
         self._setVal("action", "getConceptTrendGroups")
         self._setVal("source", source)
         self._setVal("conceptCount", count)
         self._update(returnInfo.getParams())
 
 
-    def getConceptTypeGroups(self, types = ["person", "org", "loc"]):
+    def getConceptTypeGroups(self, types: Union[str, List[str]] = ["person", "org", "loc"]):
         """request trending of concepts of specified types"""
         self._setVal("conceptType", types)
 
 
-    def getConceptClassUris(self, conceptClassUris):
+    def getConceptClassUris(self, conceptClassUris: Union[str, List[str]]):
         """request trending of concepts assigned to the specified concept classes"""
         self._setVal("conceptClassUri", conceptClassUris)
```

### Comparing `eventregistry-8.9/eventregistry/__init__.py` & `eventregistry-9.0/eventregistry/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from eventregistry.EventForText import *
 from eventregistry.ReturnInfo import *
 from eventregistry.Query import *
 from eventregistry.QueryEvents import *
 from eventregistry.QueryEvent import *
 from eventregistry.QueryArticles import *
 from eventregistry.QueryArticle import *
+from eventregistry.QueryMentions import *
 from eventregistry.QueryStory import *
 from eventregistry.Counts import *
 from eventregistry.DailyShares import *
 from eventregistry.Info import *
 from eventregistry.Recent import *
 from eventregistry.Trends import *
 from eventregistry.Analytics import *
```

### Comparing `eventregistry-8.9/eventregistry.egg-info/PKG-INFO` & `eventregistry-9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eventregistry
-Version: 8.9
+Version: 9.0
 Summary: A package that can be used to query information in Event Registry (http://eventregistry.org/)
 Home-page: https://github.com/EventRegistry/event-registry-python
 Author: Gregor Leban
 Author-email: gregor@eventregistry.org
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Intended Audience :: Information Technology
+License-File: LICENSE
```

### Comparing `eventregistry-8.9/eventregistry.egg-info/SOURCES.txt` & `eventregistry-9.0/eventregistry.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,24 @@
+LICENSE
 README.md
 setup.py
 eventregistry/Analytics.py
 eventregistry/Base.py
 eventregistry/Counts.py
 eventregistry/DailyShares.py
 eventregistry/EventForText.py
 eventregistry/EventRegistry.py
 eventregistry/Info.py
+eventregistry/Logger.py
 eventregistry/Query.py
 eventregistry/QueryArticle.py
 eventregistry/QueryArticles.py
 eventregistry/QueryEvent.py
 eventregistry/QueryEvents.py
+eventregistry/QueryMentions.py
 eventregistry/QueryStory.py
 eventregistry/Recent.py
 eventregistry/ReturnInfo.py
 eventregistry/TopicPage.py
 eventregistry/Trends.py
 eventregistry/__init__.py
 eventregistry/_version.py
```

### Comparing `eventregistry-8.9/PKG-INFO` & `eventregistry-9.0/eventregistry.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: eventregistry
-Version: 8.9
+Version: 9.0
 Summary: A package that can be used to query information in Event Registry (http://eventregistry.org/)
 Home-page: https://github.com/EventRegistry/event-registry-python
 Author: Gregor Leban
 Author-email: gregor@eventregistry.org
 License: MIT
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Topic :: Text Processing :: General
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
 Classifier: Intended Audience :: Information Technology
+License-File: LICENSE
```

### Comparing `eventregistry-8.9/README.md` & `eventregistry-9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,80 +1,143 @@
-## Accessing Event Registry data through Python
-
-This library contains classes that allow one to obtain from Event Registry (http://eventregistry.org) all available data, such as news articles, events, trends, etc.
-
-The detailed documentation on how to use the library is available at the [project's wiki page](https://github.com/EventRegistry/event-registry-python/wiki). Examples of use are in the [Examples folder in the repository](https://github.com/EventRegistry/event-registry-python/tree/master/eventregistry/examples).
-
-Changes introduced in the different versions of the module are described in the [CHANGELOG.md](https://github.com/EventRegistry/event-registry-python/blob/master/CHANGELOG.md) as well as on the [Releases](https://github.com/EventRegistry/event-registry-python/releases) page.
+Event Registry is a Python package that can be used to easily access the news data available in [Event Registry](http://eventregistry.org/) through the API. The package can be used to query for articles or events by filtering using a large set of filters, like keywords, concepts, topics, sources, sentiment, date, etc. Details about the News API are available on the [landing page of the product](https://newsapi.ai/).
 
 ## Installation
 
 Event Registry package can be installed using Python's pip installer. In the command line, simply type:
 
     pip install eventregistry
 
-and the package should be installed. Alternatively, you can also clone the package from the GitHub repository at https://github.com/EventRegistry/event-registry-python. After cloning it, open the command line and run:
+and the package should be installed. Alternatively, you can also clone the package from the [GitHub repository](https://github.com/EventRegistry/event-registry-python). After cloning it, open the command line and run:
 
     python setup.py install
 
 ### Validating installation
 
 To ensure the package has been properly installed run python and type:
 
 ```python
 import eventregistry
 ```
 
-If you don't get any error messages then your installation has been successful.
+If you don't get any error messages, then your installation has been successful.
 
 ### Updating the package
 
 As features are added to the package you will need at some point to update it. In case you have downloaded the package from GitHub simply do a `git pull`. If you have installed it using the `pip` command, then simply run
 
 	pip install eventregistry --upgrade
 
 ### Authentication and API key
 
-When making queries to Event Registry you will have to use an API key that you can obtain for free. The details how to obtain and use the key are described in the [Authorization](../../wiki/EventRegistry-class#authorization) section.
+When making queries to Event Registry you will have to use an API key that you can obtain for free. The details on how to obtain and use the key are described in the [Authorization](../../wiki/EventRegistry-class#authorization) section.
 
-## Three simple examples to make you interested
+## Four simple examples to get you interested
 
-**Print a list of recently added articles mentioning George Clooney**
+**Print a list of recently articles or blog posts from *US based sources* *with positive sentiment* mentioning phrases *"George Clooney"* or *"Sandra Bullock"***
 
 ```python
 from eventregistry import *
 er = EventRegistry(apiKey = YOUR_API_KEY)
-q = QueryArticlesIter(conceptUri = er.getConceptUri("George Clooney"))
-for art in q.execQuery(er, sortBy = "date"):
-    print art
+
+# get the USA URI
+usUri = er.getLocationUri("USA")    # = http://en.wikipedia.org/wiki/United_States
+
+q = QueryArticlesIter(
+    keywords = QueryItems.OR(["George Clooney", "Sandra Bullock"]),
+    minSentiment = 0.4,
+    sourceLocationUri = usUri,
+    dataType = ["news", "blog"])
+
+# obtain at most 500 newest articles or blog posts, remove maxItems to get all
+for art in q.execQuery(er, sortBy = "date", maxItems = 500):
+    print(art)
 ```
 
+**Print a list of most relevant *business* articles from the last month related to *Microsoft* or *Google*. The articles should be in any language (including Chinese, Arabic, ...)**
+
+```python
+from eventregistry import *
+# allowUseOfArchive=False will allow us to search only over the last month of data
+er = EventRegistry(apiKey = YOUR_API_KEY, allowUseOfArchive=False)
+
+# get the URIs for the companies and the category
+microsoftUri = er.getConceptUri("Microsoft")    # = http://en.wikipedia.org/wiki/Microsoft
+googleUri = er.getConceptUri("Google")          # = http://en.wikipedia.org/wiki/Google
+businessUri = er.getCategoryUri("news business")    # = news/Business
+
+q = QueryArticlesIter(
+    conceptUri = QueryItems.OR([microsoftUri, googleUri]),
+    categoryUri = businessUri)
+
+# obtain at most 500 newest articles, remove maxItems to get all
+for art in q.execQuery(er, sortBy = "date", maxItems = 500):
+    print(art)
+```
+
+
 **Search for latest events related to Star Wars**
 
 ```python
 from eventregistry import *
 er = EventRegistry(apiKey = YOUR_API_KEY)
-q = QueryEvents(conceptUri = er.getConceptUri("Star Wars"))
-q.setRequestedResult(RequestEventsInfo(sortBy = "date", count=10))   # return event details for last 10 events
-print er.execQuery(q)
+
+q = QueryEvents(keywords = "Star Wars")
+q.setRequestedResult(RequestEventsInfo(sortBy = "date", count = 50))   # request event details for latest 50 events
+
+# get the full list of 50 events at once
+print(er.execQuery(q))
+```
+
+**Search for articles that (a) mention immigration, (b) are related to business, and (c) were published by news sources located in New York City**
+
+```python
+from eventregistry import *
+er = EventRegistry(apiKey = YOUR_API_KEY)
+
+q = QueryArticlesIter(
+    # here we don't use keywords so we will also get articles that mention immigration using various synonyms
+    conceptUri = er.getConceptUri("immigration"),
+    categoryUri = er.getCategoryUri("business"),
+    sourceLocationUri = er.getLocationUri("New York City"))
+
+# obtain 500 articles that have were shared the most on social media
+for art in q.execQuery(er, sortBy = "socialScore", maxItems = 500):
+    print(art)
 ```
 
 **What are the currently trending topics**
 
 ```python
 from eventregistry import *
 er = EventRegistry(apiKey = YOUR_API_KEY)
+
 # top 10 trending concepts in the news
 q = GetTrendingConcepts(source = "news", count = 10)
-print er.execQuery(q)
+print(er.execQuery(q))
 ```
 
-## Where to next?
+## Learning from examples
+
+We believe that it's easiest to learn how to use our service by looking at examples. For this reason, we have prepared examples of various most used features. View the examples grouped by main search actions:
+
+[View examples of searching for articles](https://github.com/EventRegistry/event-registry-python/blob/master/eventregistry/examples/QueryArticlesExamples.py)
+
+[View examples of searching for events](https://github.com/EventRegistry/event-registry-python/blob/master/eventregistry/examples/QueryEventsExamples.py)
 
-Depending on your interest and existing knowledge of the `eventregistry` package you can check different things:
+[View examples of obtaining information about an individual event](https://github.com/EventRegistry/event-registry-python/blob/master/eventregistry/examples/QueryEventExamples.py)
+
+[Examples of how to obtain the full feed of articles](https://github.com/EventRegistry/event-registry-python/blob/master/eventregistry/examples/FeedOfNewArticlesExamples.py)
+
+[Examples of how to obtain the full feed of events](https://github.com/EventRegistry/event-registry-python/blob/master/eventregistry/examples/FeedOfNewEventsExamples.py)
+
+## Play with interactive Jupyter notebook
+
+To interactively learn about how to use the SDK, see examples of use, see how to get extra meta-data properties, and more, please open [this Binder](https://mybinder.org/v2/gh/EventRegistry/event-registry-python-intro/master). You'll be able to view and modify the examples.
+
+## Where to next?
 
 **[Terminology](../../wiki/Terminology)**. There are numerous terms in the Event Registry that you will constantly see. If you don't know what we mean by an *event*, *story*, *concept* or *category*, you should definitely check this page first.
 
 **[Learn about `EventRegistry` class](../../wiki/Eventregistry-class)**. You will need to use the `EventRegistry` class whenever you will want to interact with Event Registry so you should learn about it.
 
 **[Details about articles/events/concepts/categories/... that we can provide](../../wiki/ReturnInfo-class)**. When you will be requesting information about events, articles, concepts, and other things, what details can you ask for each of these?
 
@@ -82,14 +145,10 @@
 
 **[Querying articles](../../wiki/Searching-for-articles)**. Read if you want to search for articles based on the publisher's URL, article date, mentioned concepts or others.
 
 **[Trends](../../wiki/Trends)**. Are you interested in finding which concepts are currently trending the most in the news? Maybe which movie actor is most popular in social media? How about trending of various news categories?
 
 **[Articles and events shared the most on social media](../../wiki/Social-shares)**. Do you want to get the list of articles that have been shared the most on Facebook and Twitter on a particular date? What about the most relevant event based on shares on social media?
 
-**[Daily mentions and sentiment of concepts and categories](../../wiki/Number-of-mentions-in-news-or-social-media)**. Are you interested in knowing how often was a particular concept or category mentioned in the news in the previous two years? How about the sentiment expressed on social media about your favorite politician?
-
-**[Correlations of concepts](../../wiki/Correlations)**. Do you have some time series of daily measurements? Why not find the concepts that correlate the most with it based on the number of mentions in the news.
-
 ## Data access and usage restrictions
 
-Event Registry is a commercial service but it allows also unsubscribed users to perform a certain number of operations. Free users are not allowed to use the obtained data for any commercial purposes (see the details on our [Terms of Service page](http://eventregistry.org/terms)). In order to avoid these restrictions please contact us about the [available plans](http://eventregistry.org/pricing).
+Event Registry is a commercial service but it allows also unsubscribed users to perform a certain number of operations. Non-paying users are not allowed to use the obtained data for any commercial purposes (see the details on our [Terms of Service page](http://newsapi.ai/terms)) and have access to only last 30 days of content. In order to avoid these restrictions please contact us about the [available plans](http://newsapi.ai/plans).
```

### Comparing `eventregistry-8.9/setup.py` & `eventregistry-9.0/setup.py`

 * *Files identical despite different names*

