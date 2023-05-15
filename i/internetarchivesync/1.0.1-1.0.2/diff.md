# Comparing `tmp/internetarchivesync-1.0.1.tar.gz` & `tmp/internetarchivesync-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internetarchivesync-1.0.1.tar", max compression
+gzip compressed data, was "internetarchivesync-1.0.2.tar", max compression
```

## Comparing `internetarchivesync-1.0.1.tar` & `internetarchivesync-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       22 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/__init__.py
--rw-r--r--   0        0        0     3395 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/archive_download.py
--rw-r--r--   0        0        0     8127 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/archive_sync.py
--rw-r--r--   0        0        0     4097 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/download.py
--rw-r--r--   0        0        0     1665 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/io.py
--rw-r--r--   0        0        0     6943 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/observer.py
--rw-r--r--   0        0        0     3910 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/internetarchivesync/sync.py
--rw-r--r--   0        0        0      664 2023-05-13 14:49:48.824474 internetarchivesync-1.0.1/logging_config.ini
--rw-r--r--   0        0        0      879 2023-05-13 15:14:16.456885 internetarchivesync-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 internetarchivesync-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-13 14:49:48.824474 internetarchivesync-1.0.2/internetarchivesync/__init__.py
+-rw-r--r--   0        0        0     3564 2023-05-14 20:17:15.977586 internetarchivesync-1.0.2/internetarchivesync/archive_download.py
+-rw-r--r--   0        0        0     8155 2023-05-14 20:17:07.973408 internetarchivesync-1.0.2/internetarchivesync/archive_sync.py
+-rw-r--r--   0        0        0     4097 2023-05-14 20:15:52.623727 internetarchivesync-1.0.2/internetarchivesync/download.py
+-rw-r--r--   0        0        0     1665 2023-05-14 20:15:38.535413 internetarchivesync-1.0.2/internetarchivesync/io.py
+-rw-r--r--   0        0        0      664 2023-05-13 14:49:48.824474 internetarchivesync-1.0.2/internetarchivesync/logging_config.ini
+-rw-r--r--   0        0        0     7291 2023-05-14 20:18:42.903525 internetarchivesync-1.0.2/internetarchivesync/observer.py
+-rw-r--r--   0        0        0     3996 2023-05-15 20:03:25.782059 internetarchivesync-1.0.2/internetarchivesync/sync.py
+-rw-r--r--   0        0        0      846 2023-05-15 20:05:51.705336 internetarchivesync-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      558 1970-01-01 00:00:00.000000 internetarchivesync-1.0.2/PKG-INFO
```

### Comparing `internetarchivesync-1.0.1/internetarchivesync/archive_download.py` & `internetarchivesync-1.0.2/internetarchivesync/archive_download.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module to download archive from archive.org."""
 
 import logging
 import os
-from typing import Tuple
+from typing import Optional, Tuple
 
 import requests
 
 import internetarchivesync.download
 
 log = logging.getLogger(__name__)
 
@@ -14,31 +14,35 @@
 class AuthenticationError(Exception):
     """Authentication Failed."""
 
 
 class S3Auth(requests.auth.AuthBase):
     """Attaches S3 Basic Authentication to the given Request object."""
 
-    def __init__(self, access_key=None, secret_key=None):
-        self.access_key = access_key
-        self.secret_key = secret_key
-
-    def __call__(self, r):
+    def __init__(self, access_key: str, secret_key: str):
+        self.access_key: str = access_key
+        self.secret_key: str = secret_key
+
+    def __call__(
+        self, prepared_request: requests.models.PreparedRequest
+    ) -> requests.models.PreparedRequest:
         if not self.access_key:
             if self.secret_key:
                 raise AuthenticationError("No access_key set!")
         if not self.secret_key:
             if self.access_key:
                 raise AuthenticationError("No secret_key set!")
             else:
                 raise AuthenticationError("No access_key or secret_key set!")
 
-        r.headers["Authorization"] = f"LOW {self.access_key}:{self.secret_key}"
+        prepared_request.headers[
+            "Authorization"
+        ] = f"LOW {self.access_key}:{self.secret_key}"
 
-        return r
+        return prepared_request
 
 
 def get_access_secret_s3_tuple(host: str, email: str, password: str) -> Tuple[str, str]:
     """Returns the tuple (access, secret) required for S3 Basic Authentication.
 
     Args:
         host (str): archive.org host.
```

### Comparing `internetarchivesync-1.0.1/internetarchivesync/archive_sync.py` & `internetarchivesync-1.0.2/internetarchivesync/archive_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
         return src
 
     def move_file_to_cave(
         self,
         observer: internetarchivesync.observer.ProgressObserver,
         file_path: str,
-    ):
+    ) -> None:
         """Move file to cave.
 
         Args:
             observer (Observer): Observer.
             file_path (str): desired archive file.
         """
 
@@ -127,15 +127,15 @@
         """Move files to cave."""
 
         only_localy = (
             set(self.local_archive_content.keys())
             - set(self.remote_archive_content.keys())
             - set(self.metadatas)  # Don't move metadatas
         )
-        move_job = []  # type: List[Tuple[Callable[..., Any], Tuple]]
+        move_job = []  # type: List[Tuple[Callable[..., Any], Tuple[Any, ...]]]
         for file_to_move in only_localy:
             move_job.append((self.move_file_to_cave, (file_to_move,)))
         _ = internetarchivesync.observer.manage_jobs(
             move_job, "Moving files to *cave*".ljust(32), 1
         )
 
     def compare(
@@ -175,15 +175,15 @@
         good = []
 
         if recheck is None:
             files_to_check = on_both_side  # type: Iterable[str]
         else:
             files_to_check = recheck
 
-        hash_job = []  # type:List[Tuple[Callable[..., Any], Tuple]]
+        hash_job = []  # type:List[Tuple[Callable[..., Any], Tuple[Any, ...]]]
         for file_to_check in files_to_check:
             file_path = os.path.join(self.base_dir, self.archive_name, file_to_check)
             hash_job.append(
                 (internetarchivesync.io.get_file_info, (file_path, skip_md5))
             )
 
         if not skip_md5:
```

### Comparing `internetarchivesync-1.0.1/internetarchivesync/download.py` & `internetarchivesync-1.0.2/internetarchivesync/download.py`

 * *Files identical despite different names*

### Comparing `internetarchivesync-1.0.1/internetarchivesync/io.py` & `internetarchivesync-1.0.2/internetarchivesync/io.py`

 * *Files identical despite different names*

### Comparing `internetarchivesync-1.0.1/internetarchivesync/observer.py` & `internetarchivesync-1.0.2/internetarchivesync/observer.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """"Module to manage the progress of several tasks via the observer pattern."""
 
 import logging
 from concurrent.futures import ALL_COMPLETED, ThreadPoolExecutor, wait
 from time import sleep
-from typing import Any, Callable, List, Tuple
+from typing import Any, Callable, List, Optional, Tuple
 
 from rich.console import Group
 from rich.live import Live
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     FileSizeColumn,
     MofNCompleteColumn,
     Progress,
     SpinnerColumn,
+    TaskID,
     TextColumn,
     TotalFileSizeColumn,
     TransferSpeedColumn,
 )
 
 log = logging.getLogger(__name__)
 
@@ -31,33 +32,33 @@
     def __init__(self, task_id: int):
         """ProgressObserver constructor.
 
         Args:
             task_id (int): Task ID to manage.
         """
 
-    def started(self, total: int, description: str):
+    def started(self, total: int, description: str = "") -> None:
         """Method to call when task start.
 
         Args:
             total (int): total number of steps.
             description (str): description of the task.
         """
 
-    def update(self, advance: int):
+    def update(self, advance: int) -> None:
         """Method to call when task progress.
 
         Args:
             advance (int): number of steps to advance.
         """
 
-    def completed(self):
+    def completed(self) -> None:
         """Method to call when task is completed."""
 
-    def wraps_task(self, fun, *args):
+    def wraps_task(self, fun: Callable[..., Any], *args: Any) -> Any:
         """Wraps the task to force it to always be completed.
 
         Args:
             fun : Task to launch.
             args: Arguments to use.
 
         Returns:
@@ -79,48 +80,48 @@
     def __init__(self, rich_progress: Progress, task_id: int):
         """RichProgressObserver constructor.
 
         Args:
             rich_progress (Progress): Rich Progress object that manages the progression.
             task_id (int): Task ID to handle.
         """
-        super().__init__(task_id)
+        super().__init__(TaskID(task_id))
         self.rich_progress = rich_progress
-        self.task_id = task_id
-        self.total = None
+        self.task_id: TaskID = TaskID(task_id)
+        self.total: Optional[int] = None
 
-    def started(self, total, description=None):
+    def started(self, total: Optional[int], description: str = "") -> None:
         if description:
             self.rich_progress.update(self.task_id, description=f"[cyan] {description}")
         self.rich_progress.tasks[self.task_id].visible = True
         self.rich_progress.update(self.task_id, total=total)
         self.total = total
         self.rich_progress.start_task(self.task_id)
 
-    def update(self, advance):
+    def update(self, advance: float) -> None:
         self.rich_progress.update(self.task_id, advance=advance)
 
-    def completed(self):
+    def completed(self) -> None:
         if self.total:
             self.rich_progress.update(self.task_id, completed=self.total)
         else:
             self.rich_progress.update(self.task_id, total=1)
             self.rich_progress.update(self.task_id, completed=1)
         self.rich_progress.tasks[self.task_id].visible = False
 
 
 def manage_jobs(
-    jobs: List[Tuple[Callable[..., Any], Tuple]],
+    jobs: List[Tuple[Callable[..., Any], Tuple[Any, ...]]],
     description_of_jobs_group: str = "All Jobs",
     progression_type: int = 0,
 ) -> Any:
     """Manage the to-do list.
 
     Args:
-        jobs (List[Tuple[Callable[..., Any], Tuple]]): to-do list.
+        jobs (List[Tuple[Callable[..., Any], Tuple[Any, ...]]]): to-do list.
         overall_progress (Progress): Progress.
         description_of_jobs_group (str): Description of the to-do list group.
 
     Returns:
         The list of the returns of tasks.
     """
 
@@ -156,17 +157,16 @@
         job_progress,
         overall_progress,
     )
 
     futures = []
 
     with Live(progress_group, refresh_per_second=10):
-
         pool = ThreadPoolExecutor(max_workers=4)
-        for (fun, arg) in jobs:
+        for fun, arg in jobs:
             task_id = job_progress.add_task("[cyan] truc", visible=False)
             rich_progress_observer = RichProgressObserver(job_progress, task_id)
             futures.append(pool.submit(rich_progress_observer.wraps_task, fun, *arg))
         while not overall_progress.finished:
             completed = 0
             for task in job_progress.tasks:
                 if task.finished:
@@ -182,46 +182,51 @@
         results.append(result)
 
     return results
 
 
 if __name__ == "__main__":
 
-    def task1(observer, param1: str, param2: str, param3: str):
+    def task1(observer: ProgressObserver, param1: str, param2: str, param3: str) -> str:
         """Task of test."""
         observer.started(3)
         sleep(0.2)
         observer.update(1)
         sleep(0.2)
         observer.update(1)
         sleep(0.2)
         observer.update(1)
         observer.completed()
         return f"T1 {param1},{param2},{param3}"
 
-    def task2(observer, array):
+    def task2(observer: ProgressObserver, array: List[str]) -> str:
         """Task of test."""
         observer.started(len(array))
         for _ in array:
             sleep(0.1)
             observer.update(1)
         observer.completed()
         return f"T2 {''.join(array)}"
 
-    def task3(observer, array):
+    def task3(observer: ProgressObserver, array: List[str]) -> str:
         """Task of test."""
         observer.started(len(array))
         for _ in array:
             observer.update(1)
             raise Exception("test")
         observer.completed()
         return f"T3 {''.join(array)}"
 
-    test_jobs = []  # type: List[Tuple[Callable[..., Any], Tuple]]
-    test_jobs.append((task1, ("a", "b", "c")))
+    test_jobs = []  # type: List[ Tuple[Callable[..., Any], Tuple[Any, ...]] ]
+    test_jobs.append(
+        (
+            task1,
+            ("a", "b", "c"),
+        )
+    )
     test_jobs.append((task2, (["a", "b", "c"],)))
     test_jobs.append((task1, ("d", "e", "f")))
     test_jobs.append((task2, (["d", "e", "f"],)))
     test_jobs.append((task1, ("g", "h", "i")))
     test_jobs.append((task2, (["g", "h", "i"],)))
     test_jobs.append((task1, ("j", "k", "l")))
     test_jobs.append((task2, (["j", "k", "l"],)))
```

### Comparing `internetarchivesync-1.0.1/internetarchivesync/sync.py` & `internetarchivesync-1.0.2/internetarchivesync/sync.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """ Tool to donwload and update an archive.org's archive. """
 
 import argparse
+import importlib.resources
 import logging
 import logging.config
 from typing import Any, Callable, List, Tuple
 
 from rich.console import Console
 
 import internetarchivesync.archive_download as archive_download
 import internetarchivesync.archive_sync as archive_sync
 import internetarchivesync.observer as observer
 
 log = logging.getLogger(__name__)
 
-logging.config.fileConfig("logging_config.ini")
+logging.config.fileConfig(
+    importlib.resources.open_text(__package__, "logging_config.ini")
+)
 
 parser = argparse.ArgumentParser(
     prog="async",
     description="Synchronise une archive local à partir de la version sur archive.org",
 )
 parser.add_argument("name", help="Nom de l'archive archive.org.", action="store")
 parser.add_argument("-l", "--login", help="Login archive.org.", action="store")
@@ -104,15 +107,15 @@
     console.print(f":sad_but_relieved_face: File to redownload ({len(bad)}):")
     for f in bad:
         console.print(f"  ❌ [red]{f}[/red]")
     console.print(f":sad_but_relieved_face: File to download ({len(only_remotely)}):")
     for f in only_remotely:
         console.print(f"  ❌ [red]{f}[/red]")
 else:
-    dl_job = []  # type: List[Tuple[Callable[..., Any], Tuple]]
+    dl_job = []  # type:List[Tuple[Callable[..., Any], Tuple[Any, ...]]]
     to_redownload = set(only_remotely) | set(bad)
 
     for f in to_redownload:
         dl_job.append(
             (
                 archive_download.download_archive_files,
                 (LOGIN, PASSWORD, CONTENT_DIRECTORY, ARCHIVE_NAME, f),
```

### Comparing `internetarchivesync-1.0.1/logging_config.ini` & `internetarchivesync-1.0.2/internetarchivesync/logging_config.ini`

 * *Files identical despite different names*

### Comparing `internetarchivesync-1.0.1/pyproject.toml` & `internetarchivesync-1.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 [tool.poetry]
 name = "InternetArchiveSync"
-version = "1.0.1"
+version = "1.0.2"
 description = "A python tool to donwload an internet archive."
 authors = ["Mathieu <git@bigbisous.org>"]
-include = ["logging_config.ini"]
 
 [tool.poetry.dependencies]
 python = "^3.9"
 requests = "^2.26.0"
 defusedxml = "^0.7.1"
 rich = "^13.3.5"
 pytest = "^7.3.1"
```

### Comparing `internetarchivesync-1.0.1/PKG-INFO` & `internetarchivesync-1.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internetarchivesync
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python tool to donwload an internet archive.
 Author: Mathieu
 Author-email: git@bigbisous.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

