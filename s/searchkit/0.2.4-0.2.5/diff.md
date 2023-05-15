# Comparing `tmp/searchkit-0.2.4.tar.gz` & `tmp/searchkit-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.4.tar", last modified: Wed May 10 09:52:05 2023, max compression
+gzip compressed data, was "searchkit-0.2.5.tar", last modified: Mon May 15 14:27:28 2023, max compression
```

## Comparing `searchkit-0.2.4.tar` & `searchkit-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.4/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-10 09:52:05.554224 searchkit-0.2.4/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.4/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.4/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.4/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-05-10 08:57:33.000000 searchkit-0.2.4/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.4/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-10 09:51:27.000000 searchkit-0.2.4/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     3981 2023-05-10 09:51:27.000000 searchkit-0.2.4/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-10 09:52:05.554224 searchkit-0.2.4/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-10 09:52:05.000000 searchkit-0.2.4/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-10 09:52:05.554224 searchkit-0.2.4/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.4/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.5/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-15 14:27:28.015197 searchkit-0.2.5/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.5/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-05-11 09:19:48.000000 searchkit-0.2.5/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-05-11 09:19:48.000000 searchkit-0.2.5/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    26546 2023-05-15 14:26:31.000000 searchkit-0.2.5/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.5/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    49277 2023-05-11 09:19:48.000000 searchkit-0.2.5/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     5726 2023-05-15 14:26:31.000000 searchkit-0.2.5/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-05-15 14:27:28.015197 searchkit-0.2.5/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3105 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-05-15 14:27:28.000000 searchkit-0.2.5/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-05-15 14:27:28.015197 searchkit-0.2.5/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.5/setup.py
```

### Comparing `searchkit-0.2.4/LICENSE` & `searchkit-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.4/PKG-INFO` & `searchkit-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.4/README.md` & `searchkit-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.4/pyproject.toml` & `searchkit-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.4/searchkit/constraints.py` & `searchkit-0.2.5/searchkit/constraints.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 import tempfile
 import uuid
 
 from datetime import datetime, timedelta
 from functools import cached_property
 
-from searchkit.utils import MPCache
+from searchkit.utils import MPCacheSharded
 from searchkit.log import log
 
 
 class ConstraintBase(abc.ABC):
 
     @cached_property
     def id(self):
@@ -197,93 +197,178 @@
                 self.invalid_range,
                 self.search_range_end,
                 self.cur_pos,
                 self.cur_ln,
                 self.rc))
 
 
-class SeekInfo(object):
+class FileMarkers(object):
+    INDEX_FSIZE_LIMIT = (1024 ** 3) * 10
+    SYNC_LIMIT = 100000
+    # NOTE: chunk much contain a newline
+    BLOCK_SIZE_BASE = 4096
+    CHUNK_SIZE = BLOCK_SIZE_BASE * 64
 
-    def __init__(self, fd, cache_path=None):
+    def __init__(self, fd, eof_pos, cache_path=None):
         """
-        @param cache_path: provide a path to save cache info if you want it to
-                          persist.
+        Index start position for every line in file. Starts at current
+        position and is non-destructive i.e. original position is
+        restored.
+
+        This is an expensive operation and we only want to do it once per
+        file/path so the results are cached on disk and loaded when needed.
+
+        NOTE: this is only safe to use if the file does not change between
+              calls.
         """
-        self.fd = fd
-        self.iterations = 0
-        self._orig_pos = self.fd.tell()
         if cache_path is None:
-            cache_path = tempfile.mkdtemp()
+            self.cache_path = tempfile.mkdtemp()
+            log.debug("cache path not provided to filemarkers so using a "
+                      "custom one (%s)", self.cache_path)
+        else:
+            self.cache_path = cache_path
 
-        self.cache = MPCache('file_markers_{}'.format(self.fname_hash),
-                             'search_constraints', cache_path)
+        self.fd = fd
+        self.file_path = self.fd.name
+        hash = self._fname_hash(self.file_path)
+        mtimesize = self._fmtime_size(self.file_path)
+        self.cache_id = 'file_markers_{}_{}'.format(hash, mtimesize)
+        self.cache_type = 'search_constraints'
+        self.orig_pos = self.fd.tell()
+        self.eof_pos = eof_pos
+        self._primed = False
+        self._num_lines = None
+        self.chunk_size = self.CHUNK_SIZE
+
+    def _do_chunk(self, cache, chunk, current_position, marker):
+        if (self.fd.tell() < self.eof_pos) and '\n' not in chunk:
+            log.warning("no newline found in chunk len=%s starting at "
+                        "%s - increasing chunksize by %s bytes and "
+                        "trying again", self.chunk_size, current_position,
+                        self.BLOCK_SIZE_BASE)
+            self.chunk_size += self.BLOCK_SIZE_BASE
+            self.fd.seek(current_position)
+            return -1, marker
+
+        markers = {}
+        chunkpos = 0
+        while True:
+            n = chunk[chunkpos:].find('\n')
+            if n == -1:
+                break
 
-    @cached_property
-    def fname_hash(self):
+            chunkpos += n + 1
+            if current_position + chunkpos == self.eof_pos:
+                # don't save eof
+                break
+
+            marker += 1
+            markers[marker] = current_position + chunkpos
+            if marker % self.SYNC_LIMIT == 0:
+                log.debug("indexed {0:.2f}% of file".format(
+                          (100 / self._num_lines) * marker))
+
+        cache.bulk_set(markers)
+        return chunkpos, marker
+
+    def _prime(self):
+        self.fd.seek(self.orig_pos)
+        self._num_lines = sum(1 for i in self.fd)
+        self.fd.seek(self.orig_pos)
+        log.debug("priming index cache for file %s in %s (numlines=%s)",
+                  self.file_path,
+                  self.cache_path, self._num_lines)
+        with MPCacheSharded(self.cache_id, self.cache_type,
+                            self.cache_path) as cache:
+            if cache.get(self._num_lines - 1) is not None:
+                log.debug("using existing file index from cache.")
+                self._primed = True
+                return
+
+            main_marker = 0
+            main_pos = self.orig_pos
+            cache.set(main_marker, self.orig_pos)
+            remainder = ''
+            for chunk in self._readchunk(self.fd):
+                if remainder != '':
+                    chunk = remainder + chunk
+
+                chunk_pos, main_marker = self._do_chunk(cache, chunk, main_pos,
+                                                        main_marker)
+                if chunk_pos >= 0:
+                    remainder = chunk[chunk_pos:]
+                    main_pos += chunk_pos
+                else:
+                    # this implies we are going around again
+                    remainder = ''
+
+        self.fd.seek(self.orig_pos)
+        log.debug("finished creating index. (lines=%s)", self._num_lines)
+        self._primed = True
+
+    def _fname_hash(self, path):
         hash = hashlib.sha256()
-        hash.update(self.fd.name.encode('utf-8'))
+        hash.update(path.encode('utf-8'))
         return hash.hexdigest()
 
-    @property
-    def fmtime_size(self):
+    def _fmtime_size(self, path):
         """
         Criteria used to determine if file contents changed since markers were
         last generated.
         """
-        if not os.path.exists(self.fd.name):
+        if not os.path.exists(path):
             return 0
 
-        mtime = os.path.getmtime(self.fd.name)
-        size = os.path.getsize(self.fd.name)
+        mtime = os.path.getmtime(path)
+        size = os.path.getsize(path)
         return "{}+{}".format(mtime, size)
 
-    @cached_property
-    def markers(self):
-        """
-        Creates a list of positions of each start of line. Starts at current
-        position in the file and is non-destructive i.e. original position is
-        restored.
+    def _readchunk(self, fd):
+        while True:
+            data = fd.read(self.chunk_size).decode()
+            if data == '':
+                break
 
-        Since this is an expensive operation we only want to do it once per
-        file/path so the results are cached on disk and loaded when needed.
+            yield data
 
-        NOTE: this is only safe to use if the file does not change between
-              calls.
-        """
-        log.debug("loading markers for '%s'", self.fd.name)
-        fname = self.fd.name
-        fmtime_size = self.fmtime_size
-        if fmtime_size:
-            cached = self.cache.get(fmtime_size)
-            if cached:
-                log.debug("finished loading markers for '%s' with mtime %s",
-                          fname, fmtime_size)
-                return cached
+    def __getitem__(self, key):
+        if not self._primed:
+            self._prime()
+
+        with MPCacheSharded(self.cache_id, self.cache_type,
+                            self.cache_path) as cache:
+            return cache.get(key)
+
+    def __iter__(self):
+        if not self._primed:
+            self._prime()
+
+        with MPCacheSharded(self.cache_id, self.cache_type,
+                            self.cache_path) as cache:
+            for value in sorted(cache):
+                yield value
 
-        log.debug("no cached markers for '%s' - generating new set",
-                  self.fd.name)
+    def __len__(self):
+        if not self._primed:
+            self._prime()
 
-        self.fd.seek(self.orig_pos)
-        _markers = [self.fd.tell()]
-        for _ in self.fd:
-            _markers.append(self.fd.tell())
+        return self._num_lines
 
-        # pop EOF
-        _markers.pop()
 
-        # restore
-        self.fd.seek(self.orig_pos)
-        if fmtime_size:
-            self.cache.set(fmtime_size, _markers)
-        else:
-            log.warning("not caching markers for file '%s' since mtime not "
-                        "valid", self.fd.name)
+class SeekInfo(object):
 
-        log.debug("finished loading markers for '%s'", fname)
-        return _markers
+    def __init__(self, fd, cache_path=None):
+        """
+        @param cache_path: provide a path to save cache info if you want it to
+                          persist.
+        """
+        self.fd = fd
+        self.iterations = 0
+        self._orig_pos = self.fd.tell()
+        self.markers = FileMarkers(fd, self.eof_pos, cache_path)
 
     @cached_property
     def eof_pos(self):
         """
         Returns file EOF position.
         """
         orig = self.fd.tell()
@@ -455,29 +540,35 @@
                             If that is not desired this can be set to False.
         """
         search_state = BinarySearchState(self.fd_info, self.fd_info.fd.tell())
         offset = 0
 
         # check first line before going ahead with full search which requires
         # generating file markers that is expensive for large files.
-        search_state.next_pos = search_state.cur_pos + 1
         if self._check_line(search_state) == search_state.next_pos:
             self.fd_info.reset()
             log.debug("first line is valid so assuming same for rest of "
                       "file")
             log.debug("seek %s finished (skipped %d lines) current_pos=%s, "
                       "offset=%s iterations=%s",
                       self.fd_info.fd.name, offset,
                       self.fd_info.fd.tell(), offset, self.fd_info.iterations)
 
             return offset
 
+        log.debug("first line is not valid - checking rest of file")
+        self.fd_info.reset()
         search_state.start()
-        if len(self.fd_info.markers) > 0:
+        num_lines = len(self.fd_info.markers)
+        if num_lines > 0:
             while True:
+                if search_state.cur_ln >= num_lines:
+                    log.debug("reached eof - no more lines to check")
+                    break
+
                 self.fd_info.iterations += 1
                 search_state = self._seek_next(search_state)
                 if search_state.rc == search_state.RC_ERROR:
                     offset = 0
                     self.fd_info.reset()
                     break
 
@@ -591,14 +682,16 @@
         for g in ret.groups():
             str_date += "{} ".format(g)
 
         str_date = str_date.strip()
         try:
             return datetime.strptime(str_date, self.date_format)
         except ValueError:
+            # this can happen if the line is incomplete or does not contain a
+            # timestamp.
             log.exception("")
 
     @property
     def _is_valid(self):
         return self._since_date is not None
 
     @cached_property
@@ -634,21 +727,28 @@
     def apply_to_file(self, fd, destructive=True):
         self.fd_info = SeekInfo(fd, cache_path=self.cache_path)
         if not self._is_valid:
             log.warning("c:%s unable to apply constraint to %s", self.id,
                         fd.name)
             return
 
+        # indexing files larger than this takes too long and is too resource
+        # intensive so best to fall back to per-line check.
+        if os.path.getsize(fd.name) >= FileMarkers.INDEX_FSIZE_LIMIT:
+            log.debug("s:%s: file %s too big to perform binary search - "
+                      "skipping", self.id, fd.name)
+            return
+
         if fd.name in self._results:
             return self._results[fd.name]
 
-        log.debug("s:%s: starting binary seek search to %s in file %s "
+        log.debug("c:%s: starting binary seek search to %s in file %s "
                   "(destructive=True)", self.id, self._since_date, fd.name)
         self._results[fd.name] = self._seek_to_first_valid(destructive)
-        log.debug("s:%s: finished binary seek search in file %s", self.id,
+        log.debug("c:%s: finished binary seek search in file %s", self.id,
                   fd.name)
         return self._results[fd.name]
 
     def stats(self):
         _stats = {'line': {'pass': self._line_pass,
                            'fail': self._line_fail}}
         if self.fd_info:
```

### Comparing `searchkit-0.2.4/searchkit/search.py` & `searchkit-0.2.5/searchkit/search.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.4/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.5/searchkit.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.4
+Version: 0.2.5
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

