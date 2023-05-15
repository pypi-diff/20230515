# Comparing `tmp/postgres-tq-0.0.1.tar.gz` & `tmp/postgres-tq-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgres-tq-0.0.1.tar", last modified: Thu May 11 16:00:24 2023, max compression
+gzip compressed data, was "postgres-tq-0.0.2.tar", last modified: Mon May 15 13:34:25 2023, max compression
```

## Comparing `postgres-tq-0.0.1.tar` & `postgres-tq-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/postgres_tq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-11 16:00:24.000000 postgres-tq-0.0.1/postgres_tq.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/postgrestq/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/postgrestq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16061 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/postgrestq/task_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:00:24.033214 postgres-tq-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-11 16:00:06.000000 postgres-tq-0.0.1/tests/test_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/postgres_tq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-15 13:34:25.000000 postgres-tq-0.0.2/postgres_tq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 13:34:25.000000 postgres-tq-0.0.2/postgres_tq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 13:34:25.000000 postgres-tq-0.0.2/postgres_tq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-15 13:34:25.000000 postgres-tq-0.0.2/postgres_tq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-15 13:34:25.000000 postgres-tq-0.0.2/postgres_tq.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/postgrestq/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/postgrestq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16358 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/postgrestq/task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 13:34:25.037379 postgres-tq-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-05-15 13:34:12.000000 postgres-tq-0.0.2/tests/test_task_queue.py
```

### Comparing `postgres-tq-0.0.1/PKG-INFO` & `postgres-tq-0.0.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,12 @@
-Metadata-Version: 2.1
-Name: postgres-tq
-Version: 0.0.1
-Summary: Postgres Based Task Queue
-Author-email: FlixTech <open-source@flixbus.com>
-License: MIT
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+[![postgres-tq Actions Status](https://github.com/flix-tech/postgres-tq/workflows/CI/CD%20Pipeline/badge.svg?branch=main)](https://github.com/flix-tech/postgres-tq/actions)
+[![License](https://img.shields.io/github/license/flix-tech/postgres-tq)](https://pypi.org/project/postgres-tq/)
+[![PyPI - Python Version](https://img.shields.io/pypi/v/postgres-tq)](https://pypi.org/project/postgres-tq/)
 
-# Postgres Task queue
+# Postgres Task Queue
 
 This repo will contain the [Postgres](https://www.postgresql.org/) based task queue logic, similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on postgres instead.
 
 Similar to redis-tq, this package allows for sharing data between multiple processes or hosts.
 
 Tasks support a "lease time". After that time other workers may consider this client to have crashed or stalled and pick up the item instead. The number of retries can also be configured.
 
@@ -29,14 +24,24 @@
     processing BOOLEAN NOT NULL DEFAULT false,
     lease_timeout FLOAT,
     deadline TIMESTAMP,
     completed_at TIMESTAMP
 )
 ```
 
+## Installation
+
+postgres-tq is available on [PyPI][] so you can simply install via:
+
+```bash
+$ pip install postgres-tq
+```
+
+[PyPI]: https://pypi.org/project/postgres-tq/
+
 ## How it works
 
 It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
 
 ```sql
 UPDATE task_queue
 SET processing = true,
@@ -109,34 +114,34 @@
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 
 for task, id_ in taskqueue:
-    # do something with task and it automatically
+    # do something with task and it's automatically
     # marked as completed by the iterator at the end
     # of the iteration
 
 ```
 
 If the consumer crashes (i.e. the task is not marked as completed after lease_timeout seconds), the task will be put back into the task queue. This rescheduling will happen at most ttl times and then the task will be dropped. A callback can be provided if you want to monitor such cases.
 
 ## Running the tests
 
 The tests will check a presence of an Postgres DB in the port 15432. To initiate one using docker you can run:
 
-```
-make run-postgres
+```bash
+$ make run-postgres
 ```
 
 Then run
 
-```
-make test
+```bash
+$ pdm run make test
 ```
 
-Make sure you have `pdm` and `Docker` installed for this to work.
+`pdm run` will ensure that the `make test` command is executed within the context of the virtual environment managed by `pdm`. Make sure you have `pdm` and `Docker` installed for this to work.
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `postgres-tq-0.0.1/postgres_tq.egg-info/PKG-INFO` & `postgres-tq-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 Metadata-Version: 2.1
 Name: postgres-tq
-Version: 0.0.1
+Version: 0.0.2
 Summary: Postgres Based Task Queue
 Author-email: FlixTech <open-source@flixbus.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# Postgres Task queue
+[![postgres-tq Actions Status](https://github.com/flix-tech/postgres-tq/workflows/CI/CD%20Pipeline/badge.svg?branch=main)](https://github.com/flix-tech/postgres-tq/actions)
+[![License](https://img.shields.io/github/license/flix-tech/postgres-tq)](https://pypi.org/project/postgres-tq/)
+[![PyPI - Python Version](https://img.shields.io/pypi/v/postgres-tq)](https://pypi.org/project/postgres-tq/)
+
+# Postgres Task Queue
 
 This repo will contain the [Postgres](https://www.postgresql.org/) based task queue logic, similar to [our redis-tq](https://github.com/flix-tech/redis-tq) but based on postgres instead.
 
 Similar to redis-tq, this package allows for sharing data between multiple processes or hosts.
 
 Tasks support a "lease time". After that time other workers may consider this client to have crashed or stalled and pick up the item instead. The number of retries can also be configured.
 
@@ -29,14 +34,24 @@
     processing BOOLEAN NOT NULL DEFAULT false,
     lease_timeout FLOAT,
     deadline TIMESTAMP,
     completed_at TIMESTAMP
 )
 ```
 
+## Installation
+
+postgres-tq is available on [PyPI][] so you can simply install via:
+
+```bash
+$ pip install postgres-tq
+```
+
+[PyPI]: https://pypi.org/project/postgres-tq/
+
 ## How it works
 
 It uses row level locks of postgres to mimic the atomic pop and atomic push of redis-tq when getting a new task from the queue:
 
 ```sql
 UPDATE task_queue
 SET processing = true,
@@ -109,34 +124,34 @@
 
 ```py
 from postgrestq import TaskQueue
 
 task_queue = TaskQueue(POSTGRES_CONN_STR, queue_name, reset=True)
 
 for task, id_ in taskqueue:
-    # do something with task and it automatically
+    # do something with task and it's automatically
     # marked as completed by the iterator at the end
     # of the iteration
 
 ```
 
 If the consumer crashes (i.e. the task is not marked as completed after lease_timeout seconds), the task will be put back into the task queue. This rescheduling will happen at most ttl times and then the task will be dropped. A callback can be provided if you want to monitor such cases.
 
 ## Running the tests
 
 The tests will check a presence of an Postgres DB in the port 15432. To initiate one using docker you can run:
 
-```
-make run-postgres
+```bash
+$ make run-postgres
 ```
 
 Then run
 
-```
-make test
+```bash
+$ pdm run make test
 ```
 
-Make sure you have `pdm` and `Docker` installed for this to work.
+`pdm run` will ensure that the `make test` command is executed within the context of the virtual environment managed by `pdm`. Make sure you have `pdm` and `Docker` installed for this to work.
 
 ## License
 
 This project is licensed under the [MIT License](LICENSE).
```

### Comparing `postgres-tq-0.0.1/postgrestq/task_queue.py` & `postgres-tq-0.0.2/postgrestq/task_queue.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 
 
 class TaskQueue:
     def __init__(
         self,
         dsn: str,
         queue_name: str,
-        table_name: str = 'task_queue',
+        table_name: str = "task_queue",
         reset: bool = False,
         create_table: bool = False,
         ttl_zero_callback: Optional[
-            Callable[[UUID, Optional[str]], None]] = None
+            Callable[[UUID, Optional[str]], None]
+        ] = None,
     ):
         """Initialize the task queue.
 
         Note: a task has to be at any given time either in the task
         queue or in the processing queue. If a task is moved from one
         queue to the other it has to be in an atomic fashion!
 
@@ -70,50 +71,53 @@
     def _create_queue_table(self) -> None:
         """
         Creates a task_queue table
         """
         # TODO: check if the table already exist
         # whether it has the same schema
         with self.conn.cursor() as cur:
-            cur.execute(sql.SQL(
-                """CREATE TABLE IF NOT EXISTS  {} (
+            cur.execute(
+                sql.SQL(
+                    """CREATE TABLE IF NOT EXISTS  {} (
                             id UUID PRIMARY KEY,
                             queue_name TEXT NOT NULL,
                             task JSONB NOT NULL,
                             ttl INT NOT NULL,
                             created_at TIMESTAMP NOT NULL DEFAULT NOW(),
                             processing BOOLEAN NOT NULL DEFAULT false,
                             lease_timeout FLOAT,
                             deadline TIMESTAMP,
                             completed_at TIMESTAMP
                         )"""
-                    ).format(sql.Identifier(self._table_name)))
+                ).format(sql.Identifier(self._table_name))
+            )
 
     def __len__(self) -> int:
         """
         Returns the length of processing or to be processed tasks
         """
         with self.conn.cursor() as cursor:
-            cursor.execute(sql.SQL("""
+            cursor.execute(
+                sql.SQL(
+                    """
                 SELECT count(1) as count
                 FROM {}
                 WHERE queue_name = %s
                     AND completed_at IS NULL
-            """).format(sql.Identifier(self._table_name)),
-                (self._queue_name,))
+            """
+                ).format(sql.Identifier(self._table_name)),
+                (self._queue_name,),
+            )
             row = cursor.fetchone()
             count: int = row[0] if row else 0
             self.conn.commit()
             return count
 
     def add(
-        self,
-        task: Dict[Any, Any],
-        lease_timeout: float,
-        ttl: int = 3
+        self, task: Dict[str, Any], lease_timeout: float, ttl: int = 3
     ) -> None:
         """Add a task to the task queue.
 
         Parameters
         ----------
         task : something that can be JSON-serialized
         lease_timeout : float
@@ -124,37 +128,38 @@
             job dies.
 
         """
         # make sure the timeout is an actual number, otherwise we'll run
         # into problems later when we calculate the actual deadline
         lease_timeout = float(lease_timeout)
 
-        # we wrap the task itself with some meta data
         id_ = str(uuid4())
-        wrapped_task = {
-            'task': task,
-        }
-        serialized_task = self._serialize(wrapped_task)
+
+        serialized_task = self._serialize(task)
 
         with self.conn.cursor() as cursor:
             # store the task + metadata and put task-id into the task queue
-            cursor.execute(sql.SQL("""
+            cursor.execute(
+                sql.SQL(
+                    """
                 INSERT INTO {} (
                     id,
                     queue_name,
                     task,
                     ttl,
                     lease_timeout
                 )
                 VALUES (%s, %s, %s, %s, %s)
-            """).format(sql.Identifier(self._table_name)),
-                (id_, self._queue_name, serialized_task, ttl, lease_timeout))
+            """
+                ).format(sql.Identifier(self._table_name)),
+                (id_, self._queue_name, serialized_task, ttl, lease_timeout),
+            )
             self.conn.commit()
 
-    def get(self) -> Tuple[Optional[Dict[Any, Any]], Optional[UUID]]:
+    def get(self) -> Tuple[Optional[Dict[str, Any]], Optional[UUID]]:
         """Get a task from the task queue (non-blocking).
 
         This statement marks the next available task in the queue as
         "processing" and returns its ID and task details. The query
         uses a FOR UPDATE SKIP LOCKED clause to lock the selected
         task so that other workers can't select the same task simultaneously.
 
@@ -185,16 +190,17 @@
             The next item from the task list or (None, None) if it's
             empty
 
         """
         conn = self.conn
 
         with conn.cursor() as cur:
-
-            cur.execute(sql.SQL("""
+            cur.execute(
+                sql.SQL(
+                    """
                 UPDATE {}
                 SET processing = true,
                     deadline =
                         NOW() + CAST(lease_timeout || ' seconds' AS INTERVAL)
                 WHERE id = (
                     SELECT id
                     FROM {}
@@ -202,57 +208,59 @@
                         AND processing = false
                         AND queue_name = %s
                         AND ttl > 0
                     ORDER BY created_at
                     FOR UPDATE SKIP LOCKED
                     LIMIT 1
                 )
-                RETURNING id, task;""")
-                        .format(
-                            sql.Identifier(self._table_name),
-                            sql.Identifier(self._table_name)
-                        ),
-                        (self._queue_name,),)
+                RETURNING id, task;"""
+                ).format(
+                    sql.Identifier(self._table_name),
+                    sql.Identifier(self._table_name),
+                ),
+                (self._queue_name,),
+            )
 
             row = cur.fetchone()
             if row is None:
                 return None, None
-            task_id, wrapped_task = row
-            task = wrapped_task['task']
-            logger.info(f'Got task with id {task_id}')
+            task_id, task = row
+            logger.info(f"Got task with id {task_id}")
             conn.commit()
             return task, task_id
 
-    def complete(self, task_id: UUID) -> None:
+    def complete(self, task_id: Optional[UUID]) -> None:
         """Mark a task as completed.
 
         Marks a task as completed by setting completed_at column by
         the current timestamp.
 
         If the job is in the queue, which happens if it took too long
         and it expired, is removed from that too.
 
 
         Parameters
         ----------
-        task_id : str
+        task_id : UUID | None
             the task ID
 
         """
-        logger.info(f'Marking task {task_id} as completed')
+        logger.info(f"Marking task {task_id} as completed")
         conn = self.conn
         with conn.cursor() as cur:
-
-            cur.execute(sql.SQL("""
+            cur.execute(
+                sql.SQL(
+                    """
                 UPDATE {}
                 SET completed_at = NOW(),
                     processing = false
-                WHERE id = %s""")
-                        .format(sql.Identifier(self._table_name)),
-                        (task_id,),)
+                WHERE id = %s"""
+                ).format(sql.Identifier(self._table_name)),
+                (task_id,),
+            )
             conn.commit()
 
     def is_empty(self) -> bool:
         """Check if the task queue is empty.
 
         Internally, this function also checks the currently processed
         tasks for expiration and teals with TTL and re-scheduling them
@@ -279,56 +287,63 @@
         Note: lease check is only performed against the tasks in
         that are processing.
 
         """
         # goes through all the tasks that are marked as processing
         # and check the ones with expired timeout
         with self.conn.cursor() as cur:
-            cur.execute(sql.SQL("""
+            cur.execute(
+                sql.SQL(
+                    """
                 SELECT id
                 FROM {}
                 WHERE completed_at IS NULL
                     AND processing = true
                     AND queue_name = %s
                     AND deadline < NOW()
                 ORDER BY created_at;
-            """).format(sql.Identifier(self._table_name)),
-                        (self._queue_name,))
+            """
+                ).format(sql.Identifier(self._table_name)),
+                (self._queue_name,),
+            )
             expired_tasks = cur.fetchall()
             self.conn.commit()
             logger.debug(f"Expired tasks {expired_tasks}")
         for row in expired_tasks:
             task_id: UUID = row[0]
             logger.debug(f"Got expired task with id {task_id}")
             task, ttl = self.get_updated_expired_task(task_id)
 
             if ttl is None:
                 # race condition! between the time we got `key` from the
                 # set of tasks (this outer loop) and the time we tried
                 # to get that task from the queue, it has been completed
                 # and therefore deleted from the queue. In this case
                 # tasks is None and we can continue
-                logger.info(f"Task {task_id} was marked completed while we "
-                            "checked for expired leases, nothing to do.")
+                logger.info(
+                    f"Task {task_id} was marked completed while we "
+                    "checked for expired leases, nothing to do."
+                )
                 continue
 
             if ttl <= 0:
-                logger.error(f'Job {task} with id {task_id} '
-                             'failed too many times, marking it as completed.')
+                logger.error(
+                    f"Job {task} with id {task_id} "
+                    "failed too many times, marking it as completed."
+                )
                 # # here committing to release the previous update lock
                 self.conn.commit()
                 self.complete(task_id)
 
                 if self.ttl_zero_callback:
                     self.ttl_zero_callback(task_id, task)
             self.conn.commit()
 
     def get_updated_expired_task(
-        self,
-        task_id: UUID
+        self, task_id: UUID
     ) -> Tuple[Optional[str], Optional[int]]:
         """
         Given the id of an expired task, it tries to reschedule the
         task by marking it as not processing, resetting the deadline
         and decreaasing TTL by one. It returns None if the task is
         already updated or (being updated) by another worker.
 
@@ -336,15 +351,17 @@
         -------
         (task, ttl) :
             The updated task and ttl values for the expired task with
             task_id after it's rescheduled
 
         """
         with self.conn.cursor() as cur:
-            cur.execute(sql.SQL("""
+            cur.execute(
+                sql.SQL(
+                    """
                 UPDATE {}
                 SET ttl = ttl - 1,
                     processing = false,
                     deadline = NULL
                 WHERE id = (
                     SELECT id
                     FROM {}
@@ -352,35 +369,40 @@
                         AND processing = true
                         AND queue_name = %s
                         AND id = %s
                     FOR UPDATE SKIP LOCKED
                     LIMIT 1
                 )
                 RETURNING task, ttl;
-            """).format(
-                            sql.Identifier(self._table_name),
-                            sql.Identifier(self._table_name)
-                        ),
-                        (self._queue_name, task_id,))
+            """
+                ).format(
+                    sql.Identifier(self._table_name),
+                    sql.Identifier(self._table_name),
+                ),
+                (
+                    self._queue_name,
+                    task_id,
+                ),
+            )
             updated_row = cur.fetchone()
 
             if updated_row is None:
                 return None, None
 
-            wrapped_task, ttl = updated_row
-            task = self._serialize(wrapped_task['task'])
+            task, ttl = updated_row
+            task = self._serialize(task)
             return task, ttl
 
     def _serialize(self, task: Any) -> str:
         return json.dumps(task, sort_keys=True)
 
     def _deserialize(self, blob: str) -> Any:
         return json.loads(blob)
 
-    def reschedule(self, task_id: UUID) -> None:
+    def reschedule(self, task_id: Optional[UUID]) -> None:
         """Move a task back from the processing- to the task queue.
 
         Workers can use this method to "drop" a work unit in case of
         eviction.
 
         This function does not modify the TTL.
 
@@ -394,55 +416,58 @@
         ValueError :
             Task is not being processed, and cannot be re-scheduled
 
         """
 
         if not isinstance(task_id, UUID):
             raise ValueError("task_id must be a UUID")
-        logger.info(f'Rescheduling task {task_id}..')
+        logger.info(f"Rescheduling task {task_id}..")
         conn = self.conn
         with conn.cursor() as cur:
-
-            cur.execute(sql.SQL("""
+            cur.execute(
+                sql.SQL(
+                    """
                 UPDATE {}
                 SET processing = false,
                     deadline = NULL
                 WHERE id = (
                     SELECT id
                     FROM {}
                     WHERE processing = true
                         AND id = %s
                     FOR UPDATE SKIP LOCKED
                 )
-                RETURNING id;""").format(
-                            sql.Identifier(self._table_name),
-                            sql.Identifier(self._table_name)
-                        ), (task_id,),)
+                RETURNING id;"""
+                ).format(
+                    sql.Identifier(self._table_name),
+                    sql.Identifier(self._table_name),
+                ),
+                (task_id,),
+            )
 
             found = cur.fetchone()
             conn.commit()
             if found is None:
-                raise ValueError(f'Task {task_id} does not exist.')
+                raise ValueError(f"Task {task_id} does not exist.")
 
     def _reset(self) -> None:
-        """Delete all tasks in the DB with our queue name.
-
-        """
+        """Delete all tasks in the DB with our queue name."""
         with self.conn.cursor() as cursor:
             cursor.execute(
-                sql.SQL(
-                    "DELETE FROM {} WHERE queue_name = %s "
-                ).format(sql.Identifier(self._table_name)),
-                (self._queue_name,),)
+                sql.SQL("DELETE FROM {} WHERE queue_name = %s ").format(
+                    sql.Identifier(self._table_name)
+                ),
+                (self._queue_name,),
+            )
 
             self.conn.commit()
 
-    def __iter__(self) -> Iterator[
-        Tuple[Optional[Dict[Any, Any]], Optional[UUID]]
-            ]:
+    def __iter__(
+        self,
+    ) -> Iterator[Tuple[Optional[Dict[str, Any]], Optional[UUID]]]:
         """Iterate over tasks and mark them as complete.
 
         This allows to easily iterate over the tasks to process them:
 
             >>> for task in task_queue:
                     execute_task(task)
 
@@ -461,11 +486,11 @@
         while True:
             task, id_ = self.get()
             if id_ is not None:
                 yield task, id_
                 self.complete(id_)
             if self.is_empty():
                 logger.debug(
-                    f'{self._queue_name} is empty. '
-                    'Nothing to process anymore...'
+                    f"{self._queue_name} is empty. "
+                    "Nothing to process anymore..."
                 )
                 break
```

### Comparing `postgres-tq-0.0.1/pyproject.toml` & `postgres-tq-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 log_cli = true
 log_cli_level = "INFO"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 
 [project]
 name = "postgres-tq"
-version = "0.0.1"
+version = "0.0.2"
 description = "Postgres Based Task Queue"
 authors = [
     {name = "FlixTech", email = "open-source@flixbus.com"},
 ]
 dependencies = [
     "psycopg[binary]>=3.1.8",
 ]
```

