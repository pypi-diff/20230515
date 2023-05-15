# Comparing `tmp/openlimit-0.2.6.tar.gz` & `tmp/openlimit-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlimit-0.2.6.tar", last modified: Thu May  4 13:03:38 2023, max compression
+gzip compressed data, was "openlimit-0.2.7.tar", last modified: Mon May 15 08:24:26 2023, max compression
```

## Comparing `openlimit-0.2.6.tar` & `openlimit-0.2.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.562792 openlimit-0.2.6/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-04 13:03:38.562679 openlimit-0.2.6/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.6/README.md
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.560601 openlimit-0.2.6/openlimit/
--rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.6/openlimit/__init__.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.561807 openlimit-0.2.6/openlimit/buckets/
--rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.6/openlimit/buckets/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.6/openlimit/buckets/bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.6/openlimit/buckets/redis_bucket.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1792 2023-05-01 20:23:40.000000 openlimit-0.2.6/openlimit/rate_limiters.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     2928 2023-04-25 12:09:39.000000 openlimit-0.2.6/openlimit/redis_rate_limiters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.562427 openlimit-0.2.6/openlimit/utilities/
--rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.6/openlimit/utilities/__init__.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1576 2023-04-23 11:03:35.000000 openlimit-0.2.6/openlimit/utilities/context_decorators.py
--rw-r--r--   0 jshobrook   (501) staff       (20)     1641 2023-05-04 13:02:49.000000 openlimit-0.2.6/openlimit/utilities/token_counters.py
-drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-04 13:03:38.561195 openlimit-0.2.6/openlimit.egg-info/
--rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/PKG-INFO
--rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/SOURCES.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/dependency_links.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/requires.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-05-04 13:03:38.000000 openlimit-0.2.6/openlimit.egg-info/top_level.txt
--rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-05-04 13:03:38.562831 openlimit-0.2.6/setup.cfg
--rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-05-04 13:03:33.000000 openlimit-0.2.6/setup.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-15 08:24:26.629731 openlimit-0.2.7/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-15 08:24:26.629614 openlimit-0.2.7/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3216 2023-04-23 12:13:25.000000 openlimit-0.2.7/README.md
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-15 08:24:26.627572 openlimit-0.2.7/openlimit/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      226 2023-04-23 11:35:43.000000 openlimit-0.2.7/openlimit/__init__.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-15 08:24:26.628706 openlimit-0.2.7/openlimit/buckets/
+-rw-r--r--   0 jshobrook   (501) staff       (20)       98 2023-04-23 11:38:27.000000 openlimit-0.2.7/openlimit/buckets/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)      988 2023-04-23 11:03:59.000000 openlimit-0.2.7/openlimit/buckets/bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1869 2023-04-23 11:01:20.000000 openlimit-0.2.7/openlimit/buckets/redis_bucket.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1870 2023-05-15 08:23:51.000000 openlimit-0.2.7/openlimit/rate_limiters.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     3006 2023-05-15 08:23:11.000000 openlimit-0.2.7/openlimit/redis_rate_limiters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-15 08:24:26.629319 openlimit-0.2.7/openlimit/utilities/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      252 2023-04-23 11:41:16.000000 openlimit-0.2.7/openlimit/utilities/__init__.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1575 2023-05-15 08:22:07.000000 openlimit-0.2.7/openlimit/utilities/context_decorators.py
+-rw-r--r--   0 jshobrook   (501) staff       (20)     1641 2023-05-04 13:02:49.000000 openlimit-0.2.7/openlimit/utilities/token_counters.py
+drwxr-xr-x   0 jshobrook   (501) staff       (20)        0 2023-05-15 08:24:26.628217 openlimit-0.2.7/openlimit.egg-info/
+-rw-r--r--   0 jshobrook   (501) staff       (20)      351 2023-05-15 08:24:26.000000 openlimit-0.2.7/openlimit.egg-info/PKG-INFO
+-rw-r--r--   0 jshobrook   (501) staff       (20)      468 2023-05-15 08:24:26.000000 openlimit-0.2.7/openlimit.egg-info/SOURCES.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)        1 2023-05-15 08:24:26.000000 openlimit-0.2.7/openlimit.egg-info/dependency_links.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       15 2023-05-15 08:24:26.000000 openlimit-0.2.7/openlimit.egg-info/requires.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       10 2023-05-15 08:24:26.000000 openlimit-0.2.7/openlimit.egg-info/top_level.txt
+-rw-r--r--   0 jshobrook   (501) staff       (20)       38 2023-05-15 08:24:26.629771 openlimit-0.2.7/setup.cfg
+-rw-r--r--   0 jshobrook   (501) staff       (20)      559 2023-05-15 08:22:41.000000 openlimit-0.2.7/setup.py
```

### Comparing `openlimit-0.2.6/README.md` & `openlimit-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.6/openlimit/buckets/bucket.py` & `openlimit-0.2.7/openlimit/buckets/bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.6/openlimit/buckets/redis_bucket.py` & `openlimit-0.2.7/openlimit/buckets/redis_bucket.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.6/openlimit/rate_limiters.py` & `openlimit-0.2.7/openlimit/rate_limiters.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,31 +40,31 @@
 
 ######
 # MAIN
 ######
 
 
 class ChatRateLimiter(RateLimiter):
-    def __init__(self, request_limit, token_limit):
+    def __init__(self, request_limit=3500, token_limit=90000):
         super().__init__(
-            request_limit=3500,
-            token_limit=90000,
+            request_limit=request_limit,
+            token_limit=token_limit,
             token_counter=utils.num_tokens_consumed_by_chat_request
         )
 
 
 class CompletionRateLimiter(RateLimiter):
-    def __init__(self, request_limit, token_limit):
+    def __init__(self, request_limit=3500, token_limit=350000):
         super().__init__(
-            request_limit=3500,
-            token_limit=350000,
+            request_limit=request_limit,
+            token_limit=token_limit,
             token_counter=utils.num_tokens_consumed_by_completion_request
         )
 
 
 class EmbeddingRateLimiter(RateLimiter):
-    def __init__(self, request_limit, token_limit):
+    def __init__(self, request_limit=3500, token_limit=70000000):
         super().__init__(
-            request_limit=3500, 
-            token_limit=70000000, 
+            request_limit=request_limit, 
+            token_limit=token_limit, 
             token_counter=utils.num_tokens_consumed_by_embedding_request
         )
```

### Comparing `openlimit-0.2.6/openlimit/redis_rate_limiters.py` & `openlimit-0.2.7/openlimit/redis_rate_limiters.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,37 +67,37 @@
 
 ######
 # MAIN
 ######
 
 
 class ChatRateLimiterWithRedis(RateLimiterWithRedis):
-    def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
+    def __init__(self, request_limit=3500, token_limit=90000, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit=3500, 
-            token_limit=90000, 
+            request_limit=request_limit, 
+            token_limit=token_limit, 
             token_counter=utils.num_tokens_consumed_by_chat_request,
             bucket_key="chat", 
             redis_url=redis_url
         )
 
 
 class CompletionRateLimiterWithRedis(RateLimiterWithRedis):
-    def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
+    def __init__(self, request_limit=3500, token_limit=350000, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit=3500, 
-            token_limit=350000, 
+            request_limit=request_limit, 
+            token_limit=token_limit, 
             token_counter=utils.num_tokens_consumed_by_completion_request,
             bucket_key="completion", 
             redis_url=redis_url
         )
 
 
 class EmbeddingRateLimiterWithRedis(RateLimiterWithRedis):
-    def __init__(self, request_limit, token_limit, redis_url="redis://localhost:5050"):
+    def __init__(self, request_limit=3500, token_limit=70000000, redis_url="redis://localhost:5050"):
         super().__init__(
-            request_limit=3500, 
-            token_limit=70000000, 
+            request_limit=request_limit, 
+            token_limit=token_limit, 
             token_counter=utils.num_tokens_consumed_by_embedding_request,
             bucket_key="embedding", 
             redis_url=redis_url
         )
```

### Comparing `openlimit-0.2.6/openlimit/utilities/context_decorators.py` & `openlimit-0.2.7/openlimit/utilities/context_decorators.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     def __init__(self, rate_limiter):
         self.rate_limiter = rate_limiter
 
     def __call__(self, func):
         @wraps(func)
         def wrapper(*args, **kwargs):
-            num_tokens = self.rater_limiter.token_counter(**kwargs)
+            num_tokens = self.rate_limiter.token_counter(**kwargs)
             asyncio.run(self.rate_limiter.wait_for_capacity(num_tokens))
             return func(*args, **kwargs)
 
         @wraps(func)
         async def async_wrapper(*args, **kwargs):
             num_tokens = self.rate_limiter.token_counter(**kwargs)
             await self.rate_limiter.wait_for_capacity(num_tokens)
```

### Comparing `openlimit-0.2.6/openlimit/utilities/token_counters.py` & `openlimit-0.2.7/openlimit/utilities/token_counters.py`

 * *Files identical despite different names*

### Comparing `openlimit-0.2.6/setup.py` & `openlimit-0.2.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from setuptools import setup
 
 setup(
     name="openlimit",
     description="Rate limiter for the OpenAI API",
-    version="v0.2.6",
+    version="v0.2.7",
     packages=["openlimit", "openlimit.utilities", "openlimit.buckets"],
     python_requires=">=3",
     url="https://github.com/shobrook/openlimit",
     author="shobrook",
     author_email="shobrookj@gmail.com",
     # classifiers=[],
     install_requires=["redis", "tiktoken"],
```

