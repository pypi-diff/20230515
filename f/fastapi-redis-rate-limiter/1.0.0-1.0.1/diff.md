# Comparing `tmp/fastapi_redis_rate_limiter-1.0.0.tar.gz` & `tmp/fastapi_redis_rate_limiter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_redis_rate_limiter-1.0.0.tar", last modified: Sun May 14 19:08:25 2023, max compression
+gzip compressed data, was "fastapi_redis_rate_limiter-1.0.1.tar", last modified: Sun May 14 22:16:42 2023, max compression
```

## Comparing `fastapi_redis_rate_limiter-1.0.0.tar` & `fastapi_redis_rate_limiter-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 19:08:25.535497 fastapi_redis_rate_limiter-1.0.0/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-05-13 23:43:44.000000 fastapi_redis_rate_limiter-1.0.0/LICENSE
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     3119 2023-05-14 19:08:25.535497 fastapi_redis_rate_limiter-1.0.0/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2637 2023-05-14 18:53:17.000000 fastapi_redis_rate_limiter-1.0.0/README.md
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 19:08:25.535497 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      165 2023-05-14 00:11:20.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/__init__.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2594 2023-05-13 23:25:14.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/redis_client.py
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2534 2023-05-14 18:28:14.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/redis_rate_limiter_middleware.py
-drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 19:08:25.535497 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     3119 2023-05-14 19:08:25.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/PKG-INFO
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      417 2023-05-14 19:08:25.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/SOURCES.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-05-14 19:08:25.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/dependency_links.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       30 2023-05-14 19:08:25.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/requires.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       27 2023-05-14 19:08:25.000000 fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/top_level.txt
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-05-14 19:08:25.539497 fastapi_redis_rate_limiter-1.0.0/setup.cfg
--rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      812 2023-05-14 18:52:43.000000 fastapi_redis_rate_limiter-1.0.0/setup.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 22:16:42.221811 fastapi_redis_rate_limiter-1.0.1/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     1064 2023-05-13 23:43:44.000000 fastapi_redis_rate_limiter-1.0.1/LICENSE
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     3119 2023-05-14 22:16:42.221811 fastapi_redis_rate_limiter-1.0.1/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2637 2023-05-14 18:53:17.000000 fastapi_redis_rate_limiter-1.0.1/README.md
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 22:16:42.221811 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      165 2023-05-14 00:11:20.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/__init__.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2761 2023-05-14 22:15:11.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/redis_client.py
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     2534 2023-05-14 18:28:14.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/redis_rate_limiter_middleware.py
+drwxrwxr-x   0 yusuf     (1000) yusuf     (1000)        0 2023-05-14 22:16:42.221811 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)     3119 2023-05-14 22:16:42.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/PKG-INFO
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      417 2023-05-14 22:16:42.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)        1 2023-05-14 22:16:42.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       30 2023-05-14 22:16:42.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/requires.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       27 2023-05-14 22:16:42.000000 fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/top_level.txt
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)       38 2023-05-14 22:16:42.221811 fastapi_redis_rate_limiter-1.0.1/setup.cfg
+-rw-rw-r--   0 yusuf     (1000) yusuf     (1000)      812 2023-05-14 22:16:37.000000 fastapi_redis_rate_limiter-1.0.1/setup.py
```

### Comparing `fastapi_redis_rate_limiter-1.0.0/LICENSE` & `fastapi_redis_rate_limiter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_redis_rate_limiter-1.0.0/PKG-INFO` & `fastapi_redis_rate_limiter-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_redis_rate_limiter
-Version: 1.0.0
+Version: 1.0.1
 Summary: fastapi rate limiter middleware
 Home-page: https://github.com/iunary/fastapi-redis-rate-limiter
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: fastapi rate limiter,redis,middleware
 Platform: UNKNOWN
```

### Comparing `fastapi_redis_rate_limiter-1.0.0/README.md` & `fastapi_redis_rate_limiter-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/redis_client.py` & `fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/redis_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import redis
+from redis import Redis
 
 
 class RedisError(Exception):
     """Custom exception for Redis errors."""
 
 
 class RedisClient:
     """
     A Redis client wrapper class for simplified interaction with Redis.
     """
 
-    def __init__(self, host: str = "localhost", port: int = 6379, db: int = 0):
+    def __init__(self, client: Redis = None, host: str = "localhost", port: int = 6379, db: int = 0):
         """
         Initializes the Redis client.
 
         Args:
             host (str): Redis server host. Defaults to "localhost".
             port (int): Redis server port. Defaults to 6379.
             db (int): Redis database index. Defaults to 0.
         """
-        self.client = redis.Redis(host=host, port=port, db=db)
+        if client is not None and isinstance(client, Redis):
+            self.client = client
+        else:
+            self.client = redis.Redis(host=host, port=port, db=db)
+        
 
     def get(self, key: str):
         """
         Retrieves the value associated with the given key from Redis.
 
         Args:
             key (str): The key to retrieve the value for.
```

### Comparing `fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter/redis_rate_limiter_middleware.py` & `fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter/redis_rate_limiter_middleware.py`

 * *Files identical despite different names*

### Comparing `fastapi_redis_rate_limiter-1.0.0/fastapi_redis_rate_limiter.egg-info/PKG-INFO` & `fastapi_redis_rate_limiter-1.0.1/fastapi_redis_rate_limiter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-redis-rate-limiter
-Version: 1.0.0
+Version: 1.0.1
 Summary: fastapi rate limiter middleware
 Home-page: https://github.com/iunary/fastapi-redis-rate-limiter
 Author: Yusuf
 Author-email: contact@yusuf.im
 License: MIT
 Keywords: fastapi rate limiter,redis,middleware
 Platform: UNKNOWN
```

### Comparing `fastapi_redis_rate_limiter-1.0.0/setup.py` & `fastapi_redis_rate_limiter-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "1.0.0"
+VERSION = "1.0.1"
 
 with open("README.md", "r") as readme:
     long_description = readme.read()
 
 setup(
     name="fastapi_redis_rate_limiter",
     version=VERSION,
```

