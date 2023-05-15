# Comparing `tmp/redis_simple_orm-1.2.7.tar.gz` & `tmp/redis_simple_orm-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis_simple_orm-1.2.7.tar", last modified: Fri Apr 28 18:00:35 2023, max compression
+gzip compressed data, was "redis_simple_orm-2.0.0.tar", last modified: Mon May 15 17:11:00 2023, max compression
```

## Comparing `redis_simple_orm-1.2.7.tar` & `redis_simple_orm-2.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/aioredis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     4254 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/aioredis/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5438 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/RSO/txredisapi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/RSO/txredisapi/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.475559 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 18:00:35.000000 redis_simple_orm-1.2.7/redis_simple_orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 18:00:35.479559 redis_simple_orm-1.2.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     7274 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-04-28 18:00:22.000000 redis_simple_orm-1.2.7/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10511 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.763039 redis_simple_orm-2.0.0/RSO/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.763039 redis_simple_orm-2.0.0/RSO/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/asyncio/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/RSO/txredisapi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/RSO/txredisapi/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11370 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 17:11:00.000000 redis_simple_orm-2.0.0/redis_simple_orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 17:11:00.767039 redis_simple_orm-2.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-15 17:10:47.000000 redis_simple_orm-2.0.0/tests/test_model.py
```

### Comparing `redis_simple_orm-1.2.7/LICENSE` & `redis_simple_orm-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.7/PKG-INFO` & `redis_simple_orm-2.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis_simple_orm
-Version: 1.2.7
+Version: 2.0.0
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -31,40 +31,24 @@
 
 As an inspiration and a very good alternative, 
 please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, Your data might be replaced without warning.
 
 
-## Suggestion for this Module Usage
-
- - In case you need to update `index` value,
-   Implement `update` method on `Model` that will remove old `index` value 
-   on index data / redis, then save new `index` value
-
-
 ## Installation
 
-Using [Redis-Py](https://redis-py.readthedocs.io)
+Sync and Async with [Redis-Py](https://redis-py.readthedocs.io)
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io) 
-or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
-
-```bash
-pip install redis_simple_orm[aioredis]
-```
-
-__OR__
-
 Using [`txredisapi`](https://github.com/IlyaSkriblovsky/txredisapi)
 
 ```bash
 pip install redis_simple_orm[txredisapi]
 ```
 
 
@@ -79,274 +63,287 @@
 
 
 ## Usage Example
 
 ### Model
 
 `model.py`
+
 ```python
 from dataclasses import dataclass, field
 
 from redis import Redis
 from RSO.index import HashIndex, SetIndex
 from RSO.model import Model
 
-from .data import USERS
-
-
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+from tests.data import USERS
 
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	SingleIndexUsername,
-    	SingleIndexEmail,
-    	SetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             # email and group_id might be None
-    		if value is None:
+            if value is None:
                 continue
-            result[key] = value
+            else:
+                result[key] = value
         return result
 
     """For easier access, we create some searching method"""
 
     @classmethod
     def search_by_username(cls, redis: Redis, username: str):
-        return SingleIndexUsername.search_model(redis, username, cls)
+        return SingleIndexUsername.search_model(redis, username)
 
     @classmethod
     def search_by_email(cls, redis: Redis, email: str):
-        return SingleIndexEmail.search_model(redis, email, cls)
+        return SingleIndexEmail.search_model(redis, email)
 
     @classmethod
     def search_group_member(cls, redis: Redis, group_id: int):
-        return SetIndexGroupID.search_models(redis, group_id, cls)
+        return SetIndexGroupID.search_models(redis, group_id)
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
 
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
+import os
+
 from redis import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
-redis = Redis(decode_responses=True)
+redis = Redis(
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+    decode_responses=True
+)
 
 
 def create_user(redis: Redis, user_data: dict):
-	user = UserModel(**user_data)
-	user.save(redis)
-	return user
+    user = UserModel(**user_data)
+    user.save(redis)
+    return user
 
 
 def main():
-	# save all user
-	for user_data in USERS:
-		user = create_user(redis, user_data)
-		user.save()
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = UserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = UserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = UserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = UserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = UserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = UserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = UserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = create_user(redis, user_data)
+        user.save(redis)
 
+    """Now see how is the model and index data saved on redis :)"""
 
-main()
-```
+    # search by id
+    user = UserModel.search(redis, 1)
+    assert user is not None
 
+    # search by username
+    user = UserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = UserModel.search_by_username(redis, 'not_exist')
+    assert user is None
 
-## Usage Example (`asyncio` version, also works with `aioredis`)
+    # search by email
+    user = UserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
 
-### Model
+    # search by group id
+    users = UserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = UserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = UserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
-`model.py`
-```python
-from dataclasses import dataclass, field
 
-from aioredis import Redis
-# Alternative
-# from redis.asyncio import Redis
-from RSO.aioredis.index import (
-	HashIndex as AsyncHashIndex, 
-	SetIndex as AsyncSetIndex
-)
-from RSO.aioredis.model import Model as AsyncModel
+main()
 
-from data import USERS
+```
 
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
+## Usage Example (`asyncio` version, also works with `aioredis` `v.2.x`)
 
+### Model
 
-class AsyncSingleIndexUsername(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
+`model.py`
 
+```python
+from dataclasses import dataclass, field
 
-class AsyncSingleIndexEmail(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
+from redis.asyncio import Redis
+from RSO.asyncio.index import (
+    HashIndex as AsyncHashIndex,
+    SetIndex as AsyncSetIndex
+)
+from RSO.asyncio.model import Model as AsyncModel
 
+from tests.data import USERS
 
-class AsyncSetIndexGroupID(AsyncSetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class AsyncUserModel(AsyncModel):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	AsyncSingleIndexUsername,
-    	AsyncSingleIndexEmail,
-    	AsyncSetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             if value is None:
                 continue
             result[key] = value
         return result
 
-
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
-        return await AsyncSingleIndexUsername.search_model(redis, username, cls)
+        return await AsyncSingleIndexUsername.search_model(redis, username)
 
     @classmethod
     async def search_by_email(cls, redis: Redis, email: str):
-        return await AsyncSingleIndexEmail.search_model(redis, email, cls)
+        return await AsyncSingleIndexEmail.search_model(redis, email)
 
     @classmethod
     async def search_group_member(cls, redis: Redis, group_id: int):
-        return await AsyncSetIndexGroupID.search_models(redis, group_id, cls)
+        return await AsyncSetIndexGroupID.search_models(redis, group_id)
+
+
+class AsyncSingleIndexUsername(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'username'
+
+
+class AsyncSingleIndexEmail(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'email'
 
+
+class AsyncSetIndexGroupID(AsyncSetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'group_id'
+
+
+AsyncUserModel.__indexes__ = [
+    AsyncSingleIndexUsername,
+    AsyncSingleIndexEmail,
+    AsyncSetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
 import asyncio
+import os
 
-from aioredis import Redis
+# from aioredis import Redis
+from redis.asyncio import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import AsyncUserModel
 
 
-redis = Redis.from_url('redis://localhost', decode_responses=True)
+redis = Redis.from_url(
+    'redis://localhost', decode_responses=True,
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+)
 
 
 async def main():
-	# save all user
-	for user_data in USERS:
-		user =  AsyncUserModel(**user_data)
-		await user.save(redis)
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = await AsyncUserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = await AsyncUserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = await AsyncUserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = await AsyncUserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = await AsyncUserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = await AsyncUserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = AsyncUserModel(**user_data)
+        await user.save(redis)
+
+    """Now see how is the model and index data saved on redis :)"""
+
+    # search by id
+    user = await AsyncUserModel.search(redis, 1)
+    assert user is not None
+
+    # search by username
+    user = await AsyncUserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = await AsyncUserModel.search_by_username(redis, 'not_exist')
+    assert user is None
+
+    # search by email
+    user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
+
+    # search by group id
+    users = await AsyncUserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = await AsyncUserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = await AsyncUserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
 
 asyncio.run(main())
+
 ```
 
 ## Usage Example (`twisted` version)
 
 ### Model
 
 `model.py`
@@ -356,106 +353,96 @@
 
 from twisted.internet.defer import inlineCallbacks
 from txredisapi import ConnectionHandler
 
 from RSO.txredisapi.index import HashIndex, SetIndex
 from RSO.txredisapi.model import Model
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    
-    __indexes__ = [
-        SingleIndexUsername,
-        SingleIndexEmail,
-        SetIndexGroupID,
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     @classmethod
     @inlineCallbacks
-    def search_by_username(
-        cls, redis: ConnectionHandler, username: str
-    ):
-        result = yield SingleIndexUsername.search_model(
-            redis, username, cls 
-        )
+    def search_by_username(cls, redis: ConnectionHandler, username: str):
+        result = yield SingleIndexUsername.search_model(redis, username)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, email: str
-    ):
-        result = yield SingleIndexEmail.search_model(
-            redis, email, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, email: str):
+        result = yield SingleIndexEmail.search_model(redis, email)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, group_id: int
-    ):
-        result = yield SetIndexGroupID.search_models(
-            redis, group_id, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, group_id: int):
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
-    
+
     @classmethod
     @inlineCallbacks
     def search_group_member(cls, redis: ConnectionHandler, group_id: int):
-        result = yield SetIndexGroupID.search_models(redis, group_id, UserModel)
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
+
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID,
+]
+
 ```
 
 
 ### CRUD
 
 
 `crud.py`
 ```python
 import txredisapi
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
 @inlineCallbacks
 def main():
-    redis = yield txredisapi.Connection()
+    redis = yield txredisapi.Connection(dbid=15, password='RedisPassword')
     for user_data in USERS:
         user = UserModel(**user_data)
         yield user.save(redis)
 
     user = yield UserModel.search(redis, 1)
     assert user is not None
```

### Comparing `redis_simple_orm-1.2.7/README.md` & `redis_simple_orm-2.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -6,40 +6,24 @@
 
 As an inspiration and a very good alternative, 
 please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, Your data might be replaced without warning.
 
 
-## Suggestion for this Module Usage
-
- - In case you need to update `index` value,
-   Implement `update` method on `Model` that will remove old `index` value 
-   on index data / redis, then save new `index` value
-
-
 ## Installation
 
-Using [Redis-Py](https://redis-py.readthedocs.io)
+Sync and Async with [Redis-Py](https://redis-py.readthedocs.io)
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io) 
-or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
-
-```bash
-pip install redis_simple_orm[aioredis]
-```
-
-__OR__
-
 Using [`txredisapi`](https://github.com/IlyaSkriblovsky/txredisapi)
 
 ```bash
 pip install redis_simple_orm[txredisapi]
 ```
 
 
@@ -54,274 +38,287 @@
 
 
 ## Usage Example
 
 ### Model
 
 `model.py`
+
 ```python
 from dataclasses import dataclass, field
 
 from redis import Redis
 from RSO.index import HashIndex, SetIndex
 from RSO.model import Model
 
-from .data import USERS
-
-
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+from tests.data import USERS
 
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	SingleIndexUsername,
-    	SingleIndexEmail,
-    	SetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             # email and group_id might be None
-    		if value is None:
+            if value is None:
                 continue
-            result[key] = value
+            else:
+                result[key] = value
         return result
 
     """For easier access, we create some searching method"""
 
     @classmethod
     def search_by_username(cls, redis: Redis, username: str):
-        return SingleIndexUsername.search_model(redis, username, cls)
+        return SingleIndexUsername.search_model(redis, username)
 
     @classmethod
     def search_by_email(cls, redis: Redis, email: str):
-        return SingleIndexEmail.search_model(redis, email, cls)
+        return SingleIndexEmail.search_model(redis, email)
 
     @classmethod
     def search_group_member(cls, redis: Redis, group_id: int):
-        return SetIndexGroupID.search_models(redis, group_id, cls)
+        return SetIndexGroupID.search_models(redis, group_id)
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
+
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
 
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
+import os
+
 from redis import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
-redis = Redis(decode_responses=True)
+redis = Redis(
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+    decode_responses=True
+)
 
 
 def create_user(redis: Redis, user_data: dict):
-	user = UserModel(**user_data)
-	user.save(redis)
-	return user
+    user = UserModel(**user_data)
+    user.save(redis)
+    return user
 
 
 def main():
-	# save all user
-	for user_data in USERS:
-		user = create_user(redis, user_data)
-		user.save()
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = UserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = UserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = UserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = UserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = UserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = UserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = UserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = create_user(redis, user_data)
+        user.save(redis)
 
+    """Now see how is the model and index data saved on redis :)"""
 
-main()
-```
+    # search by id
+    user = UserModel.search(redis, 1)
+    assert user is not None
 
+    # search by username
+    user = UserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = UserModel.search_by_username(redis, 'not_exist')
+    assert user is None
 
-## Usage Example (`asyncio` version, also works with `aioredis`)
+    # search by email
+    user = UserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
 
-### Model
+    # search by group id
+    users = UserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = UserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = UserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
-`model.py`
-```python
-from dataclasses import dataclass, field
 
-from aioredis import Redis
-# Alternative
-# from redis.asyncio import Redis
-from RSO.aioredis.index import (
-	HashIndex as AsyncHashIndex, 
-	SetIndex as AsyncSetIndex
-)
-from RSO.aioredis.model import Model as AsyncModel
+main()
 
-from data import USERS
+```
 
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
+## Usage Example (`asyncio` version, also works with `aioredis` `v.2.x`)
 
+### Model
 
-class AsyncSingleIndexUsername(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
+`model.py`
 
+```python
+from dataclasses import dataclass, field
 
-class AsyncSingleIndexEmail(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
+from redis.asyncio import Redis
+from RSO.asyncio.index import (
+    HashIndex as AsyncHashIndex,
+    SetIndex as AsyncSetIndex
+)
+from RSO.asyncio.model import Model as AsyncModel
 
+from tests.data import USERS
 
-class AsyncSetIndexGroupID(AsyncSetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class AsyncUserModel(AsyncModel):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	AsyncSingleIndexUsername,
-    	AsyncSingleIndexEmail,
-    	AsyncSetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             if value is None:
                 continue
             result[key] = value
         return result
 
-
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
-        return await AsyncSingleIndexUsername.search_model(redis, username, cls)
+        return await AsyncSingleIndexUsername.search_model(redis, username)
 
     @classmethod
     async def search_by_email(cls, redis: Redis, email: str):
-        return await AsyncSingleIndexEmail.search_model(redis, email, cls)
+        return await AsyncSingleIndexEmail.search_model(redis, email)
 
     @classmethod
     async def search_group_member(cls, redis: Redis, group_id: int):
-        return await AsyncSetIndexGroupID.search_models(redis, group_id, cls)
+        return await AsyncSetIndexGroupID.search_models(redis, group_id)
+
+
+class AsyncSingleIndexUsername(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'username'
+
+
+class AsyncSingleIndexEmail(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'email'
+
+
+class AsyncSetIndexGroupID(AsyncSetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'group_id'
+
 
+AsyncUserModel.__indexes__ = [
+    AsyncSingleIndexUsername,
+    AsyncSingleIndexEmail,
+    AsyncSetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
 import asyncio
+import os
 
-from aioredis import Redis
+# from aioredis import Redis
+from redis.asyncio import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import AsyncUserModel
 
 
-redis = Redis.from_url('redis://localhost', decode_responses=True)
+redis = Redis.from_url(
+    'redis://localhost', decode_responses=True,
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+)
 
 
 async def main():
-	# save all user
-	for user_data in USERS:
-		user =  AsyncUserModel(**user_data)
-		await user.save(redis)
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = await AsyncUserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = await AsyncUserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = await AsyncUserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = await AsyncUserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = await AsyncUserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = await AsyncUserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = AsyncUserModel(**user_data)
+        await user.save(redis)
+
+    """Now see how is the model and index data saved on redis :)"""
+
+    # search by id
+    user = await AsyncUserModel.search(redis, 1)
+    assert user is not None
+
+    # search by username
+    user = await AsyncUserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = await AsyncUserModel.search_by_username(redis, 'not_exist')
+    assert user is None
+
+    # search by email
+    user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
+
+    # search by group id
+    users = await AsyncUserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = await AsyncUserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = await AsyncUserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
 
 asyncio.run(main())
+
 ```
 
 ## Usage Example (`twisted` version)
 
 ### Model
 
 `model.py`
@@ -331,106 +328,96 @@
 
 from twisted.internet.defer import inlineCallbacks
 from txredisapi import ConnectionHandler
 
 from RSO.txredisapi.index import HashIndex, SetIndex
 from RSO.txredisapi.model import Model
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    
-    __indexes__ = [
-        SingleIndexUsername,
-        SingleIndexEmail,
-        SetIndexGroupID,
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     @classmethod
     @inlineCallbacks
-    def search_by_username(
-        cls, redis: ConnectionHandler, username: str
-    ):
-        result = yield SingleIndexUsername.search_model(
-            redis, username, cls 
-        )
+    def search_by_username(cls, redis: ConnectionHandler, username: str):
+        result = yield SingleIndexUsername.search_model(redis, username)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, email: str
-    ):
-        result = yield SingleIndexEmail.search_model(
-            redis, email, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, email: str):
+        result = yield SingleIndexEmail.search_model(redis, email)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, group_id: int
-    ):
-        result = yield SetIndexGroupID.search_models(
-            redis, group_id, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, group_id: int):
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
-    
+
     @classmethod
     @inlineCallbacks
     def search_group_member(cls, redis: ConnectionHandler, group_id: int):
-        result = yield SetIndexGroupID.search_models(redis, group_id, UserModel)
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
+
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID,
+]
+
 ```
 
 
 ### CRUD
 
 
 `crud.py`
 ```python
 import txredisapi
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
 @inlineCallbacks
 def main():
-    redis = yield txredisapi.Connection()
+    redis = yield txredisapi.Connection(dbid=15, password='RedisPassword')
     for user_data in USERS:
         user = UserModel(**user_data)
         yield user.save(redis)
 
     user = yield UserModel.search(redis, 1)
     assert user is not None
 
@@ -456,8 +443,8 @@
 
 
 if __name__ == "__main__":
     main()\
         .addCallback(lambda ign: reactor.stop())\
         .addErrback(lambda ign: reactor.stop())
     reactor.run()
-```
+```
```

### Comparing `redis_simple_orm-1.2.7/RSO/index.py` & `redis_simple_orm-2.0.0/RSO/asyncio/index.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,140 @@
-from typing import Any, List, Optional, Type, TypeVar, Union
+from typing import Any, Optional, TypeVar, Union
 
-from redis.client import Pipeline, Redis
-
-from .base import BaseIndex, BaseModel
+from aioredis.client import Redis, Pipeline
+from redis.asyncio.client import Redis as Redis2, Pipeline as Pipeline2
+from RSO.base import BaseModel, BaseHashIndex, BaseListIndex, BaseSetIndex
 
 T = TypeVar('T')
 
 
-class HashIndex(BaseIndex):
+class HashIndex(BaseHashIndex):
     @classmethod
-    def _to_redis_key(cls) -> str:
-        model_prefix = cls.__model__.__model_name__
-        if cls.__prefix__ is not None:
-            redis_key = f'{cls.__prefix__}::'
-        else:
-            redis_key = ''
-        redis_key = f'{redis_key}{model_prefix}::' \
-                    f'{cls.__index_name__}::{cls.__key__}'
-        return redis_key
-
-    @property
-    def redis_key(self) -> str:
-        return self._to_redis_key()
-
-    def save_index(self, redis: Union[Pipeline, Redis]) -> None:
-        index_value = getattr(self.__model__, self.__key__)
-        redis.hset(self.redis_key, index_value, self._model_key_value)
+    async def save(
+        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
+    ) -> None:
+        index_value = getattr(model_obj, cls.__key__)
+        redis.hset(cls.redis_key(), mapping={
+            index_value: cls.model_key_value(model_obj)
+        })
 
     @classmethod
-    def search_model(
-        cls, redis: Redis, index_value, model_class: Type[BaseModel]
-    ) -> Optional[BaseModel]:
-        setattr(cls, '__model__', model_class)
-        redis_key = cls._to_redis_key()
-        if not redis.exists(redis_key):
+    async def remove(
+        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
+    ) -> None:
+        redis.hdel(cls.redis_key(), cls.index_key_value(model_obj))
+
+    @classmethod
+    async def search_model(cls, redis: Union[Redis, Redis2], index_value):
+        redis_key = cls.redis_key()
+        if not bool(await redis.exists(redis_key)):
             return
 
-        model_primary_value = redis.hmget(redis_key, index_value)
-        if isinstance(model_primary_value, list):
-            model_primary_value = model_primary_value[0]
-        return model_class.search(redis, model_primary_value)
-
-    def remove_from_index(self, redis: Union[Pipeline, Redis]):
-        index_value = getattr(self.__model__, self.__key__)
-        redis.hdel(self.redis_key, index_value)
-
-
-class ListIndex(BaseIndex):
-    @classmethod
-    def _to_redis_key(cls, value) -> str:
-        model_prefix = cls.__model__.__model_name__
-        if cls.__prefix__ is not None:
-            redis_key = f'{cls.__prefix__}::'
-        else:
-            redis_key = ''
-        redis_key = f'{redis_key}{model_prefix}::' \
-                    f'{cls.__index_name__}::{cls.__key__}:{value}'
-        return redis_key
-
-    @property
-    def redis_key(self) -> str:
-        value = getattr(self.__model__, self.__key__)
-        return self._to_redis_key(value)
-
-    def save_index(self, redis: Union[Pipeline, Redis]) -> None:
-        redis.lpush(self.redis_key, self._model_key_value)
-
-    def remove_from_list(
-        self, redis: Union[Pipeline, Redis], model_value: Any,
-        count: int = 1
+        model_key_value = await redis.hmget(redis_key, index_value)
+        if model_key_value and isinstance(model_key_value, list):
+            model_key_value = model_key_value[0]
+        return await cls.__model__.search(redis, model_key_value)
+
+
+class ListIndex(BaseListIndex):
+    @classmethod
+    async def save(
+        cls, redis: Union[Pipeline, Pipeline2], model_obj: T
     ) -> None:
-        """
-        count = 0 to delete all
-        """
-        redis.lrem(self.redis_key, count, model_value)
-
-    @classmethod
-    def get_members(
-        cls, redis: Union[Pipeline, Redis], index_value: Any
-    ) -> List[Any]:
-        return redis.lrange(cls._to_redis_key(index_value), 0, -1)
-
-    @classmethod
-    def search_models(
-        cls, redis: Redis, index_value: Any, model_class: T
-    ) -> List[BaseModel]:
-        setattr(cls, '__model__', model_class)
-        redis_key = cls._to_redis_key(index_value)
-        if not redis.exists(redis_key):
+        redis.lpush(cls.redis_key(model_obj), cls.model_key_value(model_obj))
+
+    @classmethod
+    async def remove(
+        cls, redis: Union[Pipeline, Pipeline2], model_obj: T, count: int = 1
+    ):
+        """count = 0 to remove all"""
+        redis.lrem(
+            cls.redis_key(model_obj),
+            count,
+            cls.model_key_value(model_obj)
+        )
+
+    @classmethod
+    async def get_members(cls, redis: Redis, index_value):
+        redis_key = cls.redis_key_from_value(index_value)
+        return await redis.lrange(redis_key, 0, -1)
+
+    @classmethod
+    async def search_models(cls, redis: Redis, index_value):
+        redis_key = cls.redis_key_from_value(index_value)
+        if not bool(await redis.exists(redis_key)):
             return []
 
-        instance_list = []
-        for value in cls.get_members(redis, index_value):
-            instance = model_class.search(redis, value)
-            instance_list.append(instance)
-        return instance_list
+        model_instances = []
+        for value in (await redis.lrange(redis_key, 0, -1)):
+            model_instance = await cls.__model__.search(redis, value)
+            model_instances.append(model_instance)
+        return model_instances
 
-    def is_exist_on_list(self, redis: Redis, model_value: Any) -> bool:
-        result = redis.execute_command('LPOS', self.redis_key, model_value)
+    @classmethod
+    async def has_member(cls, redis: [Redis, Redis2], model_obj: T) -> bool:
+        return await cls.has_member_value(
+            redis,
+            getattr(model_obj, cls.__key__),
+            getattr(model_obj, model_obj.__key__)
+        )
+
+    @classmethod
+    async def has_member_value(
+        cls, redis: [Redis, Redis2], index_value: Any, model_value: Any
+    ) -> bool:
+        if hasattr(redis, 'lpos'):
+            result = await redis.lpos(
+                cls.redis_key_from_value(index_value),
+                model_value
+            )
+        else:
+            result = await redis.execute(
+                'LPOS',
+                cls.redis_key_from_value(index_value),
+                model_value
+            )
         return result is not None
 
     @classmethod
-    def get_by_rpoplpush(
-        cls, redis: Redis, index_value: Any, model_class: Type[BaseModel]
+    async def get_by_rpoplpush(
+        cls, redis: [Redis, Redis2], index_value: Any,
     ) -> Optional[BaseModel]:
-        cls.__model__ = model_class
-        redis_key = cls._to_redis_key(index_value)
-        if redis.exists(redis_key) == 0:
-            return None
+        redis_key = cls.redis_key_from_value(index_value)
+        if bool(await redis.exists(redis_key)) is False:
+            return
         else:
-            value = redis.rpoplpush(redis_key, redis_key)
-            return model_class.search(redis, value)
+            model_value = await redis.rpoplpush(redis_key, redis_key)
+            return await cls.__model__.search(redis, model_value)
 
-    def remove_from_index(self, redis: Redis, count: int = 1) -> None:
-        """
-        count = 0 to remove all
-        """
-        redis.lrem(self.redis_key, count, self._model_key_value)
 
+class SetIndex(BaseSetIndex):
+    @classmethod
+    async def save(cls, redis: [Pipeline, Pipeline2], model_obj: T) -> None:
+        redis.sadd(
+            cls.redis_key(model_obj),
+            cls.model_key_value(model_obj)
+        )
 
-class SetIndex(BaseIndex):
+    @classmethod
+    async def remove(cls, redis: [Pipeline, Pipeline2], model_obj: T) -> None:
+        redis.srem(
+            cls.redis_key(model_obj),
+            cls.model_key_value(model_obj)
+        )
 
     @classmethod
-    def _to_redis_key(cls, value: Any) -> str:
-        model_prefix = cls.__model__.__model_name__
-        if cls.__prefix__ is not None:
-            redis_key = f'{cls.__prefix__}::'
-        else:
-            redis_key = ''
-        redis_key = f'{redis_key}{model_prefix}::' \
-                    f'{cls.__index_name__}::{cls.__key__}:{value}'
-        return redis_key
-
-    @property
-    def redis_key(self) -> str:
-        value = getattr(self.__model__, self.__key__)
-        return self._to_redis_key(value)
-
-    def save_index(self, redis: Union[Pipeline, Redis]) -> None:
-        redis.sadd(self.redis_key, self._model_key_value)
-
-    @classmethod
-    def get_members(cls, redis: Redis, index_value) -> List[Any]:
-        redis_key = cls._to_redis_key(index_value)
-        return redis.smembers(redis_key)
-
-    @classmethod
-    def search_models(
-        cls, redis: Redis, index_value, model_class: Type[BaseModel]
-    ) -> List[BaseModel]:
-        setattr(cls, '__model__', model_class)
-        redis_key = cls._to_redis_key(index_value)
-        if not redis.exists(redis_key):
+    async def get_members(cls, redis: Redis, index_value):
+        redis_key = cls.redis_key_from_value(index_value)
+        return await redis.smembers(redis_key)
+
+    @classmethod
+    async def search_models(cls, redis: Redis, index_value):
+        redis_key = cls.redis_key_from_value(index_value)
+        if not bool(await redis.exists(redis_key)):
             return []
 
         model_instances = []
-        for value in redis.smembers(redis_key):
-            model_instance = model_class.search(redis, value)
+        for value in (await redis.smembers(redis_key)):
+            model_instance = await cls.__model__.search(redis, value)
             model_instances.append(model_instance)
         return model_instances
-
-    def remove_from_index(self, redis: Union[Pipeline, Redis]):
-        redis.srem(self.redis_key, self._model_key_value)
```

### Comparing `redis_simple_orm-1.2.7/RSO/model.py` & `redis_simple_orm-2.0.0/RSO/model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import asdict
 from typing import Union
 
 from redis.client import Pipeline, Redis
 
 from RSO.base import BaseModel
 
 
@@ -16,23 +15,22 @@
         else:
             pipe = redis.pipeline()
 
         pipe.hset(self.redis_key, mapping=self.to_redis())
         for index_class in self.__indexes__ or []:
             if getattr(self, index_class.__key__) is None:
                 continue
-            index = index_class.create_from_model_class(self)
-            index.save_index(pipe)
+            index_class.save(pipe, self)
 
         if not isinstance(redis, Pipeline):
             pipe.execute()
 
     @classmethod
     def search(cls, redis: Redis, value):
-        redis_key = cls._to_redis_key(value)
+        redis_key = cls.redis_key_from_value(value)
         if bool(redis.exists(redis_key)):
             fields = cls.get_fields()
             redis_data = redis.hmget(redis_key, fields)
             dict_data = cls.from_redis(dict(zip(fields, redis_data)))
             return cls(**dict_data)
         else:
             return None
@@ -40,14 +38,13 @@
     def delete(self, redis: Union[Pipeline, Redis]):
         if isinstance(redis, Pipeline):
             pipe = redis
         else:
             pipe = redis.pipeline()
 
         for index_class in self.__indexes__:
-            index = index_class.create_from_model_class(self)
-            index.remove_from_index(pipe)
+            if getattr(self, index_class.__key__) is not None:
+                index_class.remove(pipe, self)
 
         pipe.delete(self.redis_key)
-        pipe.execute()
-
-        del self
+        if not isinstance(redis, Pipeline):
+            pipe.execute()
```

### Comparing `redis_simple_orm-1.2.7/RSO/txredisapi/model.py` & `redis_simple_orm-2.0.0/RSO/txredisapi/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,79 +23,81 @@
             pipe = redis
             do_commit = False
 
         pipe.hmset(self.redis_key, self.to_redis())
         for index_class in self.__indexes__ or []:
             if getattr(self, index_class.__key__, None) is None:
                 continue
-            index = index_class.create_from_model_class(self)
-            yield index.save_index(pipe)
+            yield index_class.save(pipe, self)
         if do_commit:
             yield pipe.commit()
 
-    @inlineCallbacks
-    def extended_save(
-        self, redis: Union[BaseRedisProtocol, ConnectionHandler]
-    ):
-        """Extended save function to avoid multiple push on list index
-
-        Note: Use this method if you use List Index
-        """
-        list_index_map = {}
-        for index_class in self.__indexes__ or []:
-            if not issubclass(index_class, ListIndex):
-                continue
-            index = index_class.create_from_model_class(self)
-            model_key_value = getattr(self, self.__key__, None)
-            if model_key_value is None:
-                exist_on_index = False
-            else:
-                exist_on_index = yield index.is_exist_on_list(
-                    redis, model_key_value
-                )
-            list_index_map[index] = exist_on_index
-
-        if isinstance(redis, ConnectionHandler):
-            pipe = yield redis.multi()
-        else:
-            raise NotImplementedError
-
-        pipe.hmset(self.redis_key, self.to_redis())
-        for index_class in self.__indexes__ or []:
-            if getattr(self, index_class.__key__, None) is None:
-                continue
-            index = index_class.create_from_model_class(self)
-            yield index.save_index(pipe)
-
-        # remove duplicate on index queue list
-        for index, exist_on_index in list_index_map.items():
-            if exist_on_index is True:
-                model_key_value = getattr(self, self.__key__)
-                yield index.remove_from_list(pipe, model_key_value)
-
-        yield pipe.commit()
-
     @classmethod
     @inlineCallbacks
     def search(cls, redis: ConnectionHandler, value):
-        redis_key = cls._to_redis_key(value)
+        redis_key = cls.redis_key_from_value(value)
         result = yield redis.exists(redis_key)
         if bool(result):
             fields = cls.get_fields()
             redis_data = yield redis.hmget(redis_key, fields)
             dict_data = cls.from_redis(dict(zip(fields, redis_data)))
             return cls(**dict_data)
         return
 
     @inlineCallbacks
     def delete(self, redis: Union[BaseRedisProtocol, ConnectionHandler]):
         if isinstance(redis, ConnectionHandler):
             pipe = yield redis.multi()
+            do_commit = True
         else:
-            raise NotImplementedError
+            pipe = redis
+            do_commit = False
+
         for index_class in self.__indexes__ or []:
             if getattr(self, index_class.__key__) is None:
                 continue
-            index = index_class.create_from_model_class(self)
-            index.remove_from_index(pipe)
+            index_class.remove(pipe, self)
         pipe.delete(self.redis_key)
-        yield pipe.commit()
+        if do_commit:
+            yield pipe.commit()
+
+    # @inlineCallbacks
+    # def extended_save(
+    #     self, redis: Union[BaseRedisProtocol, ConnectionHandler]
+    # ):
+    #     """Extended save function to avoid multiple push on list index
+    #
+    #     Note: Use this method if you use List Index
+    #     """
+    #     list_index_map = {}
+    #     for index_class in self.__indexes__ or []:
+    #         if not issubclass(index_class, ListIndex):
+    #             continue
+    #         index = index_class.create_from_model_class(self)
+    #         model_key_value = getattr(self, self.__key__, None)
+    #         if model_key_value is None:
+    #             exist_on_index = False
+    #         else:
+    #             exist_on_index = yield index.is_exist_on_list(
+    #                 redis, model_key_value
+    #             )
+    #         list_index_map[index] = exist_on_index
+    #
+    #     if isinstance(redis, ConnectionHandler):
+    #         pipe = yield redis.multi()
+    #     else:
+    #         raise NotImplementedError
+    #
+    #     pipe.hmset(self.redis_key, self.to_redis())
+    #     for index_class in self.__indexes__ or []:
+    #         if getattr(self, index_class.__key__, None) is None:
+    #             continue
+    #         index = index_class.create_from_model_class(self)
+    #         yield index.save_index(pipe)
+    #
+    #     # remove duplicate on index queue list
+    #     for index, exist_on_index in list_index_map.items():
+    #         if exist_on_index is True:
+    #             model_key_value = getattr(self, self.__key__)
+    #             yield index.remove_from_list(pipe, model_key_value)
+    #
+    #     yield pipe.commit()
```

### Comparing `redis_simple_orm-1.2.7/redis_simple_orm.egg-info/PKG-INFO` & `redis_simple_orm-2.0.0/redis_simple_orm.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis-simple-orm
-Version: 1.2.7
+Version: 2.0.0
 Summary: Simple Redis ORM (Sync and Async).
 Home-page: https://github.com/jockerz/redis_simple_orm
 Author: Jockerz
 Author-email: jockerz@protonmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -31,40 +31,24 @@
 
 As an inspiration and a very good alternative, 
 please take a look on [walrus](https://walrus.readthedocs.org).
 
 > __NOTE__: Please be aware, Your data might be replaced without warning.
 
 
-## Suggestion for this Module Usage
-
- - In case you need to update `index` value,
-   Implement `update` method on `Model` that will remove old `index` value 
-   on index data / redis, then save new `index` value
-
-
 ## Installation
 
-Using [Redis-Py](https://redis-py.readthedocs.io)
+Sync and Async with [Redis-Py](https://redis-py.readthedocs.io)
 
 ```bash
 pip install redis_simple_orm[redis-py]
 ```
 
 __OR__
 
-Async with [`aioredis`](https://aioredis.readthedocs.io) 
-or [`redis.asyncio.Redis`](`https://redis-py.readthedocs.io/en/stable/examples/asyncio_examples.html`)
-
-```bash
-pip install redis_simple_orm[aioredis]
-```
-
-__OR__
-
 Using [`txredisapi`](https://github.com/IlyaSkriblovsky/txredisapi)
 
 ```bash
 pip install redis_simple_orm[txredisapi]
 ```
 
 
@@ -79,274 +63,287 @@
 
 
 ## Usage Example
 
 ### Model
 
 `model.py`
+
 ```python
 from dataclasses import dataclass, field
 
 from redis import Redis
 from RSO.index import HashIndex, SetIndex
 from RSO.model import Model
 
-from .data import USERS
-
-
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+from tests.data import USERS
 
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	SingleIndexUsername,
-    	SingleIndexEmail,
-    	SetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             # email and group_id might be None
-    		if value is None:
+            if value is None:
                 continue
-            result[key] = value
+            else:
+                result[key] = value
         return result
 
     """For easier access, we create some searching method"""
 
     @classmethod
     def search_by_username(cls, redis: Redis, username: str):
-        return SingleIndexUsername.search_model(redis, username, cls)
+        return SingleIndexUsername.search_model(redis, username)
 
     @classmethod
     def search_by_email(cls, redis: Redis, email: str):
-        return SingleIndexEmail.search_model(redis, email, cls)
+        return SingleIndexEmail.search_model(redis, email)
 
     @classmethod
     def search_group_member(cls, redis: Redis, group_id: int):
-        return SetIndexGroupID.search_models(redis, group_id, cls)
+        return SetIndexGroupID.search_models(redis, group_id)
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
 
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
+import os
+
 from redis import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
-redis = Redis(decode_responses=True)
+redis = Redis(
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+    decode_responses=True
+)
 
 
 def create_user(redis: Redis, user_data: dict):
-	user = UserModel(**user_data)
-	user.save(redis)
-	return user
+    user = UserModel(**user_data)
+    user.save(redis)
+    return user
 
 
 def main():
-	# save all user
-	for user_data in USERS:
-		user = create_user(redis, user_data)
-		user.save()
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = UserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = UserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = UserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = UserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = UserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = UserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = UserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = create_user(redis, user_data)
+        user.save(redis)
 
+    """Now see how is the model and index data saved on redis :)"""
 
-main()
-```
+    # search by id
+    user = UserModel.search(redis, 1)
+    assert user is not None
 
+    # search by username
+    user = UserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = UserModel.search_by_username(redis, 'not_exist')
+    assert user is None
 
-## Usage Example (`asyncio` version, also works with `aioredis`)
+    # search by email
+    user = UserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = UserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
 
-### Model
+    # search by group id
+    users = UserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = UserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = UserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
-`model.py`
-```python
-from dataclasses import dataclass, field
 
-from aioredis import Redis
-# Alternative
-# from redis.asyncio import Redis
-from RSO.aioredis.index import (
-	HashIndex as AsyncHashIndex, 
-	SetIndex as AsyncSetIndex
-)
-from RSO.aioredis.model import Model as AsyncModel
+main()
 
-from data import USERS
+```
 
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
+## Usage Example (`asyncio` version, also works with `aioredis` `v.2.x`)
 
+### Model
 
-class AsyncSingleIndexUsername(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
+`model.py`
 
+```python
+from dataclasses import dataclass, field
 
-class AsyncSingleIndexEmail(AsyncHashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
+from redis.asyncio import Redis
+from RSO.asyncio.index import (
+    HashIndex as AsyncHashIndex,
+    SetIndex as AsyncSetIndex
+)
+from RSO.asyncio.model import Model as AsyncModel
 
+from tests.data import USERS
 
-class AsyncSetIndexGroupID(AsyncSetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class AsyncUserModel(AsyncModel):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-    	AsyncSingleIndexUsername,
-    	AsyncSingleIndexEmail,
-    	AsyncSetIndexGroupID
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     def to_redis(self):
         result = {}
         for key, value in self.dict().items():
             if value is None:
                 continue
             result[key] = value
         return result
 
-
     """For easier access, we create some searching method"""
 
     @classmethod
     async def search_by_username(cls, redis: Redis, username: str):
-        return await AsyncSingleIndexUsername.search_model(redis, username, cls)
+        return await AsyncSingleIndexUsername.search_model(redis, username)
 
     @classmethod
     async def search_by_email(cls, redis: Redis, email: str):
-        return await AsyncSingleIndexEmail.search_model(redis, email, cls)
+        return await AsyncSingleIndexEmail.search_model(redis, email)
 
     @classmethod
     async def search_group_member(cls, redis: Redis, group_id: int):
-        return await AsyncSetIndexGroupID.search_models(redis, group_id, cls)
+        return await AsyncSetIndexGroupID.search_models(redis, group_id)
+
+
+class AsyncSingleIndexUsername(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'username'
+
+
+class AsyncSingleIndexEmail(AsyncHashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'email'
 
+
+class AsyncSetIndexGroupID(AsyncSetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = AsyncUserModel
+    __key__ = 'group_id'
+
+
+AsyncUserModel.__indexes__ = [
+    AsyncSingleIndexUsername,
+    AsyncSingleIndexEmail,
+    AsyncSetIndexGroupID
+]
 ```
 
 ### CRUD
 
 `crud.py`
 ```python
 import asyncio
+import os
 
-from aioredis import Redis
+# from aioredis import Redis
+from redis.asyncio import Redis
 
-from data import USERS
+from tests.data import USERS
 from model import AsyncUserModel
 
 
-redis = Redis.from_url('redis://localhost', decode_responses=True)
+redis = Redis.from_url(
+    'redis://localhost', decode_responses=True,
+    db=int(os.getenv('REDIS_DB', 15)),
+    password=os.getenv('REDIS_PASS', 'RedisPassword'),
+)
 
 
 async def main():
-	# save all user
-	for user_data in USERS:
-		user =  AsyncUserModel(**user_data)
-		await user.save(redis)
-
-	"""Now see how is the model and index data saved on redis :)"""
-
-	# search by id
-	user = await AsyncUserModel.search(redis, 1)
-	assert user is not None
-
-	# search by username
-	user = await AsyncUserModel.search_by_username(redis, 'first_user')
-	assert user is not None
-	user = await AsyncUserModel.search_by_username(redis, 'not_exist')
-	assert user is None
-
-	# search by email
-	user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
-	assert user is not None
-	user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
-	assert user is None
-
-	# search by group id
-	users = await AsyncUserModel.search_group_member(redis, 1)
-	assert len(users) == 3
-	users = await AsyncUserModel.search_group_member(redis, 2)
-	assert len(users) == 2
-	users = await AsyncUserModel.search_group_member(redis, 1_000_000)
-	assert len(users) == 0
+    # save all user
+    for user_data in USERS:
+        user = AsyncUserModel(**user_data)
+        await user.save(redis)
+
+    """Now see how is the model and index data saved on redis :)"""
+
+    # search by id
+    user = await AsyncUserModel.search(redis, 1)
+    assert user is not None
+
+    # search by username
+    user = await AsyncUserModel.search_by_username(redis, 'first_user')
+    assert user is not None
+    user = await AsyncUserModel.search_by_username(redis, 'not_exist')
+    assert user is None
+
+    # search by email
+    user = await AsyncUserModel.search_by_email(redis, 'first_user@contoh.com')
+    assert user is not None
+    user = await AsyncUserModel.search_by_email(redis, 'not_exist@contoh.com')
+    assert user is None
+
+    # search by group id
+    users = await AsyncUserModel.search_group_member(redis, 1)
+    assert len(users) == 3
+    users = await AsyncUserModel.search_group_member(redis, 2)
+    assert len(users) == 2
+    users = await AsyncUserModel.search_group_member(redis, 1_000_000)
+    assert len(users) == 0
 
 
 asyncio.run(main())
+
 ```
 
 ## Usage Example (`twisted` version)
 
 ### Model
 
 `model.py`
@@ -356,106 +353,96 @@
 
 from twisted.internet.defer import inlineCallbacks
 from txredisapi import ConnectionHandler
 
 from RSO.txredisapi.index import HashIndex, SetIndex
 from RSO.txredisapi.model import Model
 
-REDIS_MODEL_PREFIX = 'MY_REDIS_MODEL'
-
-
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
+REDIS_MODEL_PREFIX = None
 
 
 @dataclass
 class UserModel(Model):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    
-    __indexes__ = [
-        SingleIndexUsername,
-        SingleIndexEmail,
-        SetIndexGroupID,
-    ]
 
     user_id: int
     username: str
     email: str = field(default=None)
     group_id: int = field(default=None)
 
     @classmethod
     @inlineCallbacks
-    def search_by_username(
-        cls, redis: ConnectionHandler, username: str
-    ):
-        result = yield SingleIndexUsername.search_model(
-            redis, username, cls 
-        )
+    def search_by_username(cls, redis: ConnectionHandler, username: str):
+        result = yield SingleIndexUsername.search_model(redis, username)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, email: str
-    ):
-        result = yield SingleIndexEmail.search_model(
-            redis, email, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, email: str):
+        result = yield SingleIndexEmail.search_model(redis, email)
         return result
 
     @classmethod
     @inlineCallbacks
-    def search_by_email(
-        cls, redis: ConnectionHandler, group_id: int
-    ):
-        result = yield SetIndexGroupID.search_models(
-            redis, group_id, cls 
-        )
+    def search_by_email(cls, redis: ConnectionHandler, group_id: int):
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
-    
+
     @classmethod
     @inlineCallbacks
     def search_group_member(cls, redis: ConnectionHandler, group_id: int):
-        result = yield SetIndexGroupID.search_models(redis, group_id, UserModel)
+        result = yield SetIndexGroupID.search_models(redis, group_id)
         return result
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
+
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID,
+]
+
 ```
 
 
 ### CRUD
 
 
 `crud.py`
 ```python
 import txredisapi
 from twisted.internet import reactor
 from twisted.internet.defer import inlineCallbacks
 
-from data import USERS
+from tests.data import USERS
 from model import UserModel
 
 
 @inlineCallbacks
 def main():
-    redis = yield txredisapi.Connection()
+    redis = yield txredisapi.Connection(dbid=15, password='RedisPassword')
     for user_data in USERS:
         user = UserModel(**user_data)
         yield user.save(redis)
 
     user = yield UserModel.search(redis, 1)
     assert user is not None
```

### Comparing `redis_simple_orm-1.2.7/setup.py` & `redis_simple_orm-2.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `redis_simple_orm-1.2.7/tests/test_example.py` & `redis_simple_orm-2.0.0/tests/test_example.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,80 +1,69 @@
 from dataclasses import dataclass, field
 
 import pytest
 from fakeredis import FakeRedis as Redis, aioredis
 
 from RSO.index import HashIndex, SetIndex
 from RSO.model import Model
-from RSO.aioredis.index import (
+from RSO.asyncio.index import (
     HashIndex as AsyncHashIndex,
     SetIndex as AsyncSetIndex
 )
-from RSO.aioredis.model import Model as AsyncModel
+from RSO.asyncio.model import Model as AsyncModel
 
+from tests.models.base import BaseUserModel
 from tests.models.const import REDIS_MODEL_PREFIX
 from .data import USERS
 
 
-class SingleIndexUsername(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
-    __key__ = 'username'
-
-
-class SingleIndexEmail(HashIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
-    __key__ = 'email'
-
-
-class SetIndexGroupID(SetIndex):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
-    __key__ = 'group_id'
-
-
 @dataclass
-class UserModel(Model):
+class UserModel(Model, BaseUserModel):
     __prefix__ = REDIS_MODEL_PREFIX
     __model_name__ = 'user'
     __key__ = 'user_id'
-    __indexes__ = [
-        SingleIndexUsername,
-        SingleIndexEmail,
-        SetIndexGroupID
-    ]
-
-    user_id: int
-    username: str
-    email: str = field(default=None)
-    group_id: int = field(default=None)
-
-    def to_redis(self):
-        result = {}
-        for key, value in self.dict().items():
-            # email and group_id might be None
-            if value is None:
-                continue
-            result[key] = value
-        return result
 
     """For easier access, we create some searching method"""
 
     @classmethod
     def search_by_username(cls, redis: Redis, username: str):
-        return SingleIndexUsername.search_model(redis, username, cls)
+        return SingleIndexUsername.search_model(redis, username)
 
     @classmethod
     def search_by_email(cls, redis: Redis, email: str):
-        return SingleIndexEmail.search_model(redis, email, cls)
+        return SingleIndexEmail.search_model(redis, email)
 
     @classmethod
     def search_group_member(cls, redis: Redis, group_id: int):
-        return SetIndexGroupID.search_models(redis, group_id, cls)
+        return SetIndexGroupID.search_models(redis, group_id)
+
+
+class SingleIndexUsername(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'username'
+
+
+class SingleIndexEmail(HashIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'email'
+
+
+class SetIndexGroupID(SetIndex):
+    __prefix__ = REDIS_MODEL_PREFIX
+    __model__ = UserModel
+    __key__ = 'group_id'
+
+
+UserModel.__indexes__ = [
+    SingleIndexUsername,
+    SingleIndexEmail,
+    SetIndexGroupID
+]
 
 
 def test_main_sync(sync_redis):
     redis = sync_redis
 
     # save all user
     for user_data in USERS:
@@ -107,70 +96,56 @@
     assert len(users) == 2
     users = UserModel.search_group_member(redis, 1_000_000)
     assert len(users) == 0
 
 
 # Async
 
+@dataclass
+class AsyncUserModel(AsyncModel, BaseUserModel):
+    __prefix__ = REDIS_MODEL_PREFIX
+
+    """For easier access, we create some searching method"""
+
+    @classmethod
+    async def search_by_username(cls, redis: Redis, username: str):
+        return await AsyncSingleIndexUsername.search_model(redis, username)
+
+    @classmethod
+    async def search_by_email(cls, redis: Redis, email: str):
+        return await AsyncSingleIndexEmail.search_model(redis, email)
+
+    @classmethod
+    async def search_group_member(cls, redis: Redis, group_id: int):
+        return await AsyncSetIndexGroupID.search_models(redis, group_id)
+
 
 class AsyncSingleIndexUsername(AsyncHashIndex):
     __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexUsername'
+    __model__ = AsyncUserModel
     __key__ = 'username'
 
 
 class AsyncSingleIndexEmail(AsyncHashIndex):
     __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexEmail'
+    __model__ = AsyncUserModel
     __key__ = 'email'
 
 
 class AsyncSetIndexGroupID(AsyncSetIndex):
     __prefix__ = REDIS_MODEL_PREFIX
-    __model__ = 'IndexGroupID'
+    __model__ = AsyncUserModel
     __key__ = 'group_id'
 
 
-@dataclass
-class AsyncUserModel(AsyncModel):
-    __prefix__ = REDIS_MODEL_PREFIX
-    __model_name__ = 'user'
-    __key__ = 'user_id'
-    __indexes__ = [
-        AsyncSingleIndexUsername,
-        AsyncSingleIndexEmail,
-        AsyncSetIndexGroupID
-    ]
-
-    user_id: int
-    username: str
-    email: str = field(default=None)
-    group_id: int = field(default=None)
-
-    def to_redis(self):
-        result = {}
-        for key, value in self.dict().items():
-            if value is None:
-                continue
-            result[key] = value
-        return result
-
-    """For easier access, we create some searching method"""
-
-    @classmethod
-    async def search_by_username(cls, redis: Redis, username: str):
-        return await AsyncSingleIndexUsername.search_model(redis, username, cls)
-
-    @classmethod
-    async def search_by_email(cls, redis: Redis, email: str):
-        return await AsyncSingleIndexEmail.search_model(redis, email, cls)
-
-    @classmethod
-    async def search_group_member(cls, redis: Redis, group_id: int):
-        return await AsyncSetIndexGroupID.search_models(redis, group_id, cls)
+AsyncUserModel.__indexes__ = [
+    AsyncSingleIndexUsername,
+    AsyncSingleIndexEmail,
+    AsyncSetIndexGroupID
+]
 
 
 @pytest.mark.asyncio
 async def test_async_main(async_redis):
     redis = async_redis
 
     # save all user
```

### Comparing `redis_simple_orm-1.2.7/tests/test_index.py` & `redis_simple_orm-2.0.0/tests/test_index.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,112 +9,97 @@
     ListIndexQueue,
     NoPrefixUserModel,
     NoPrefixSingleIndexUsername,
     NoPrefixSetIndexGroupID,
     NoPrefixListIndexQueue,
 )
 
-
 BIRTH_DATE = date.fromisoformat('1999-09-09')
 
 
 class TestHashIndex:
     def test_redis_key(self):
         # With prefix
-        user = UserModel(
-            user_id=1, username='username', email='test@email'
-        )
-        index = SingleIndexUsername.create_from_model_class(user)
-        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert SingleIndexUsername.redis_key().startswith(REDIS_MODEL_PREFIX), \
+            f'redis_key: {SingleIndexUsername.redis_key()}'
 
         # Without prefix
-        user = NoPrefixUserModel(
-            user_id=1, username='username', email='test@email'
-        )
-        index = NoPrefixSingleIndexUsername.create_from_model_class(user)
-        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert not NoPrefixSingleIndexUsername.redis_key().startswith(
+            REDIS_MODEL_PREFIX
+        ), f'redis_key: {NoPrefixSingleIndexUsername.redis_key()}'
 
 
     def test_search_model(self, sync_redis):
-        user = UserModel(
-            user_id=1, username='username', email='test@email'
-        )
+        user = UserModel(user_id=1, username='username', email='test@email')
         user.save(sync_redis)
 
-        assert SingleIndexUsername.search_model(
-            sync_redis, user.username, UserModel
-        ) is not None
-        assert SingleIndexEmail.search_model(
-            sync_redis, user.email, UserModel
-        ) is not None
+        assert SingleIndexUsername.search_model(sync_redis, user.username) \
+               is not None
+        assert SingleIndexEmail.search_model(sync_redis, user.email) \
+               is not None
 
     def test_search_not_found(self, sync_redis):
-        assert SingleIndexUsername.search_model(
-            sync_redis, 'not_exist', UserModel
-        ) is None
-
-        assert SingleIndexEmail.search_model(
-            sync_redis, 'not_exist@email', UserModel
-        ) is None
+        assert SingleIndexUsername.search_model(sync_redis, 'not_exist') \
+               is None
+
+        assert SingleIndexEmail.search_model(sync_redis, 'not_exist@email') \
+               is None
 
     def test_after_delete(self, sync_redis):
         user = UserModel(
             user_id=1, username='username', email='test@email'
         )
         user.save(sync_redis)
 
-        assert SingleIndexUsername.search_model(
-            sync_redis, user.username, UserModel
-        ) is not None
-        assert SingleIndexEmail.search_model(
-            sync_redis, user.email, UserModel
-        ) is not None
+        assert SingleIndexUsername.search_model(sync_redis, user.username) \
+               is not None
+        assert SingleIndexEmail.search_model(sync_redis, user.email) \
+               is not None
 
         user.delete(sync_redis)
 
-        assert SingleIndexUsername.search_model(
-            sync_redis, user.username, UserModel
-        ) is None
-        assert SingleIndexEmail.search_model(
-            sync_redis, user.email, UserModel
-        ) is None
+        assert SingleIndexUsername.search_model(sync_redis, user.username) \
+               is None
+        assert SingleIndexEmail.search_model(sync_redis, user.email) \
+               is None
 
 
 class TestListIndex:
     def test_redis_key(self):
         # With prefix
         user = UserModel(
             user_id=1, username='username', email='test@email'
         )
-        index = ListIndexQueue.create_from_model_class(user)
-        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert ListIndexQueue.redis_key(user).startswith(REDIS_MODEL_PREFIX)
 
         # Without prefix
         user = NoPrefixUserModel(
             user_id=1, username='username', email='test@email'
         )
-        index = NoPrefixListIndexQueue.create_from_model_class(user)
-        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert not NoPrefixListIndexQueue.redis_key(user).startswith(
+            REDIS_MODEL_PREFIX
+        )
 
 
     def test_success(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
             group_id=2,
             queue_id=3,
             birth_date=BIRTH_DATE
         )
         user.save(sync_redis)
 
-        index = ListIndexQueue.create_from_model_class(user)
-
-        assert index.is_exist_on_list(sync_redis, user.user_id) is True
-        assert sync_redis.exists(index.redis_key)
+        assert ListIndexQueue.has_member_value(
+            sync_redis, user.queue_id, user.user_id
+        ) is True
+        assert ListIndexQueue.has_member(sync_redis, user) is True
+        assert sync_redis.exists(ListIndexQueue.redis_key(user))
         assert len(
             ListIndexQueue.get_members(sync_redis, user.queue_id)
         ) == 1
 
     def test_multiple_times_saved(self, sync_redis):
         user = UserModel(
             user_id=1,
@@ -122,48 +107,45 @@
             email='test@create.success',
             group_id=2,
             queue_id=3,
             birth_date=date.fromisoformat('1999-09-09')
         )
         user.save(sync_redis)
 
-        index = ListIndexQueue.create_from_model_class(user)
-        assert index.is_exist_on_list(sync_redis, user.user_id) is True
+        assert ListIndexQueue.has_member(sync_redis, user) is True
 
         user.save(sync_redis)
-        assert len(sync_redis.lrange(index.redis_key, 0, -1)) == 2
+        assert len(sync_redis.lrange(
+            ListIndexQueue.redis_key(user), 0, -1
+        )) == 2
 
     def test_not_using_list_index(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
             group_id=2,
             birth_date=date.fromisoformat('1999-09-09')
         )
         user.save(sync_redis)
-        index = ListIndexQueue.create_from_model_class(user)
 
-        assert len(sync_redis.lrange(index.redis_key, 0, -1)) == 0
-        assert index.is_exist_on_list(sync_redis, user.user_id) is False
+        assert ListIndexQueue.has_member(sync_redis, user) is False
 
     def test_rpushlpop(self, sync_redis):
         for data in (
             dict(user_id=1, username='uname1', queue_id=3, email='test1@email'),
             dict(user_id=2, username='uname2', queue_id=3, email='test2@email'),
         ):
             user = UserModel(**data)
             user.save(sync_redis)
 
-        index = ListIndexQueue.create_from_model_class(user)
-
-        old_list_data = sync_redis.lrange(index.redis_key, 0, -1)
+        redis_key = ListIndexQueue.redis_key_from_value(user.queue_id)
+        old_list_data = sync_redis.lrange(redis_key, 0, -1)
 
-        redis_key = index.redis_key
-        user = ListIndexQueue.get_by_rpoplpush(sync_redis, 3, UserModel)
+        user = ListIndexQueue.get_by_rpoplpush(sync_redis, 3)
         assert user is not None
 
         new_list_data = sync_redis.lrange(redis_key, 0, -1)
         assert len(new_list_data) == 2
         assert new_list_data[0] == old_list_data[1]
         assert new_list_data[1] == old_list_data[0]
 
@@ -173,59 +155,55 @@
             username='test_create_success',
             email='test@email',
             group_id=2,
             queue_id=3,
             birth_date=date.fromisoformat('1999-09-09')
         )
         user.save(sync_redis)
-        index = ListIndexQueue.create_from_model_class(user)
         user.delete(sync_redis)
 
-        assert index.is_exist_on_list(sync_redis, user.user_id) is False
-        assert len(ListIndexQueue.search_models(
-            sync_redis, user.queue_id, UserModel
-        )) == 0
+        assert ListIndexQueue.has_member_value(
+            sync_redis, user.queue_id, user.user_id
+        ) is False
+        assert len(ListIndexQueue.search_models(sync_redis, user.queue_id)) \
+               == 0
 
 
 class TestSetIndex:
 
     def test_redis_key(self):
         # With prefix
         user = UserModel(
             user_id=1, username='username', email='test@email'
         )
-        index = SetIndexGroupID.create_from_model_class(user)
-        assert index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert SetIndexGroupID.redis_key(user).startswith(REDIS_MODEL_PREFIX)
 
         # Without prefix
         user = NoPrefixUserModel(
             user_id=1, username='username', email='test@email'
         )
-        index = NoPrefixSetIndexGroupID.create_from_model_class(user)
-        assert not index.redis_key.startswith(REDIS_MODEL_PREFIX)
+        assert not NoPrefixSetIndexGroupID.redis_key(user).startswith(
+            REDIS_MODEL_PREFIX
+        )
 
     def test_search_model(self, sync_redis):
         user = UserModel(
             user_id=1, username='username', group_id=10,
             email='test@email',
         )
         user.save(sync_redis)
 
-        result = SetIndexGroupID.search_models(sync_redis, 10, UserModel)
+        result = SetIndexGroupID.search_models(sync_redis, 10)
         assert len(result) == 1
 
     def test_after_delete(self, sync_redis):
         user = UserModel(
             user_id=1, username='username', group_id=10,
             email='test@email',
         )
         user.save(sync_redis)
         user.delete(sync_redis)
 
-        assert len(SetIndexGroupID.search_models(
-            sync_redis, 10, UserModel
-        )) == 0
+        assert len(SetIndexGroupID.search_models(sync_redis, 10,)) == 0
 
     def test_not_found(self, sync_redis):
-        assert len(SetIndexGroupID.search_models(
-            sync_redis, 10, UserModel
-        )) == 0
+        assert len(SetIndexGroupID.search_models(sync_redis, 10)) == 0
```

### Comparing `redis_simple_orm-1.2.7/tests/test_model.py` & `redis_simple_orm-2.0.0/tests/test_model.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,25 +39,36 @@
             birth_date=date.fromisoformat('1999-09-09')
         )
         assert user.is_exists(sync_redis) is False
 
         user.save(sync_redis)
         assert user.is_exists(sync_redis) is True
 
-        index_username = SingleIndexUsername.create_from_model_class(user)
-        assert bool(sync_redis.exists(index_username.redis_key)) \
+        assert bool(sync_redis.exists(SingleIndexUsername.redis_key())) \
                is True
+        assert bool(sync_redis.exists(SingleIndexUsername.redis_key())) is True
 
-        index_email = SingleIndexEmail.create_from_model_class(user)
-        assert bool(sync_redis.exists(index_email.redis_key)) is True
-
-        index_group_id = SetIndexGroupID.create_from_model_class(user)
-        redis_key = index_group_id._to_redis_key(user.group_id)
-        assert bool(sync_redis.exists(redis_key)) is True
+    def test_double_save(self, sync_redis):
+        user = UserModel(
+            user_id=1,
+            username='test_create_success',
+            email='test@create.success',
+            group_id=10,
+            birth_date=date.fromisoformat('1999-09-09')
+        )
+        user.save(sync_redis)
+        user.save(sync_redis)
 
+        assert user.is_exists(sync_redis) is True
+        assert SingleIndexUsername.search_model(sync_redis, user.username) \
+               is not None
+        assert SingleIndexEmail.search_model(sync_redis, user.email) \
+               is not None
+        assert len(SetIndexGroupID.search_models(sync_redis, user.group_id)) \
+               == 1
 
 class TestModelGet:
     def test_success(self, sync_redis):
         user = UserModel(
             user_id=1,
             username='test_create_success',
             email='test@create.success',
```

