# Comparing `tmp/taskiq_redis-0.3.0.tar.gz` & `tmp/taskiq_redis-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_redis-0.3.0.tar", max compression
+gzip compressed data, was "taskiq_redis-0.3.1.tar", max compression
```

## Comparing `taskiq_redis-0.3.0.tar` & `taskiq_redis-0.3.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2576 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/README.md
--rw-r--r--   0        0        0     1587 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      257 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/__init__.py
--rw-r--r--   0        0        0      314 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/exceptions.py
--rw-r--r--   0        0        0     4154 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/redis_backend.py
--rw-r--r--   0        0        0     4006 2023-04-09 23:26:16.010239 taskiq_redis-0.3.0/taskiq_redis/redis_broker.py
--rw-r--r--   0        0        0     3699 1970-01-01 00:00:00.000000 taskiq_redis-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2715 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/README.md
+-rw-r--r--   0        0        0     1587 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      257 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/exceptions.py
+-rw-r--r--   0        0        0     4338 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/redis_backend.py
+-rw-r--r--   0        0        0     4006 2023-05-15 09:14:59.394144 taskiq_redis-0.3.1/taskiq_redis/redis_broker.py
+-rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 taskiq_redis-0.3.1/PKG-INFO
```

### Comparing `taskiq_redis-0.3.0/README.md` & `taskiq_redis-0.3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 ```
 
 # Usage
 
 Let's see the example with the redis broker and redis async result:
 
 ```python
+# broker.py
 import asyncio
 
 from taskiq_redis import ListQueueBroker, RedisAsyncResultBackend
 
 redis_async_result = RedisAsyncResultBackend(
     redis_url="redis://localhost:6379",
 )
@@ -38,20 +39,26 @@
     """Solve all problems in the world."""
     await asyncio.sleep(5.5)
     print("All problems are solved!")
 
 
 async def main():
     task = await best_task_ever.kiq()
-    print(await task.get_result())
+    print(await task.wait_result())
 
 
-asyncio.run(main())
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
+Launch the workers:
+`taskiq worker broker:broker`
+Then run the main code:
+`python3 broker.py`
+
 ## PubSubBroker and ListQueueBroker configuration
 
 We have two brokers with similar interfaces, but with different logic.
 The PubSubBroker uses redis' pubsub mechanism and is very powerful,
 but it executes every task on all workers, because PUBSUB broadcasts message
 to all subscribers.
```

### Comparing `taskiq_redis-0.3.0/pyproject.toml` & `taskiq_redis-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq-redis"
-version = "0.3.0"
+version = "0.3.1"
 description = "Redis integration for taskiq"
 authors = ["taskiq-team <taskiq@norely.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_redis-0.3.0/taskiq_redis/redis_backend.py` & `taskiq_redis-0.3.1/taskiq_redis/redis_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from redis.asyncio import ConnectionPool, Redis
 from taskiq import AsyncResultBackend
 from taskiq.abc.result_backend import TaskiqResult
 
 from taskiq_redis.exceptions import (
     DuplicateExpireTimeSelectedError,
     ExpireTimeMustBeMoreThanZeroError,
+    ResultIsMissingError,
 )
 
 _ReturnType = TypeVar("_ReturnType")
 
 
 class RedisAsyncResultBackend(AsyncResultBackend[_ReturnType]):
     """Async result based on redis."""
@@ -105,25 +106,29 @@
         with_logs: bool = False,
     ) -> TaskiqResult[_ReturnType]:
         """
         Gets result from the task.
 
         :param task_id: task's id.
         :param with_logs: if True it will download task's logs.
+        :raises ResultIsMissingError: if there is no result when trying to get it.
         :return: task's return value.
         """
         async with Redis(connection_pool=self.redis_pool) as redis:
             if self.keep_results:
                 result_value = await redis.get(
                     name=task_id,
                 )
             else:
                 result_value = await redis.getdel(
                     name=task_id,
                 )
 
+        if result_value is None:
+            raise ResultIsMissingError()
+
         taskiq_result: TaskiqResult[_ReturnType] = pickle.loads(result_value)
 
         if not with_logs:
             taskiq_result.log = None
 
         return taskiq_result
```

### Comparing `taskiq_redis-0.3.0/taskiq_redis/redis_broker.py` & `taskiq_redis-0.3.1/taskiq_redis/redis_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq_redis-0.3.0/PKG-INFO` & `taskiq_redis-0.3.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-redis
-Version: 0.3.0
+Version: 0.3.1
 Summary: Redis integration for taskiq
 Home-page: https://github.com/taskiq-python/taskiq-redis
 Keywords: taskiq,tasks,distributed,async,redis,result_backend
 Author: taskiq-team
 Author-email: taskiq@norely.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python
@@ -41,14 +41,15 @@
 ```
 
 # Usage
 
 Let's see the example with the redis broker and redis async result:
 
 ```python
+# broker.py
 import asyncio
 
 from taskiq_redis import ListQueueBroker, RedisAsyncResultBackend
 
 redis_async_result = RedisAsyncResultBackend(
     redis_url="redis://localhost:6379",
 )
@@ -65,20 +66,26 @@
     """Solve all problems in the world."""
     await asyncio.sleep(5.5)
     print("All problems are solved!")
 
 
 async def main():
     task = await best_task_ever.kiq()
-    print(await task.get_result())
+    print(await task.wait_result())
 
 
-asyncio.run(main())
+if __name__ == "__main__":
+    asyncio.run(main())
 ```
 
+Launch the workers:
+`taskiq worker broker:broker`
+Then run the main code:
+`python3 broker.py`
+
 ## PubSubBroker and ListQueueBroker configuration
 
 We have two brokers with similar interfaces, but with different logic.
 The PubSubBroker uses redis' pubsub mechanism and is very powerful,
 but it executes every task on all workers, because PUBSUB broadcasts message
 to all subscribers.
```

