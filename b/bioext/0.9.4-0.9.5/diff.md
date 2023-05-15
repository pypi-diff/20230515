# Comparing `tmp/bioext-0.9.4.tar.gz` & `tmp/bioext-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bioext-0.9.4.tar", last modified: Sat Jun 23 02:01:35 2012, max compression
+gzip compressed data, was "dist/bioext-0.9.5.tar", last modified: Mon Jul  2 23:27:44 2012, max compression
```

## Comparing `bioext-0.9.4.tar` & `bioext-0.9.5.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/bioext.egg-info/
--rw-r--r--   0 Lance      (502) staff       (20)        1 2012-06-23 02:01:35.000000 bioext-0.9.4/bioext.egg-info/dependency_links.txt
--rw-r--r--   0 Lance      (502) staff       (20)      367 2012-06-23 02:01:35.000000 bioext-0.9.4/bioext.egg-info/PKG-INFO
--rw-r--r--   0 Lance      (502) staff       (20)      328 2012-06-23 02:01:35.000000 bioext-0.9.4/bioext.egg-info/SOURCES.txt
--rw-r--r--   0 Lance      (502) staff       (20)        7 2012-06-23 02:01:35.000000 bioext-0.9.4/bioext.egg-info/top_level.txt
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/lib/
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/lib/BioExt/
--rw-r--r--   0 Lance      (502) staff       (20)      195 2012-06-23 02:01:06.000000 bioext-0.9.4/lib/BioExt/__init__.py
--rw-r--r--   0 Lance      (502) staff       (20)     4219 2012-04-18 21:42:21.000000 bioext-0.9.4/lib/BioExt/_orflist.py
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/lib/BioExt/_references/
--rw-r--r--   0 Lance      (502) staff       (20)      323 2012-06-22 23:49:41.000000 bioext-0.9.4/lib/BioExt/_references/__init__.py
--rw-r--r--   0 Lance      (502) staff       (20)     1488 2012-06-22 23:51:27.000000 bioext-0.9.4/lib/BioExt/_references/_factory.py
--rw-r--r--   0 Lance      (502) staff       (20)      877 2012-06-22 23:51:46.000000 bioext-0.9.4/lib/BioExt/_references/_lazyseq.py
--rw-r--r--   0 Lance      (502) staff       (20)     6324 2012-06-23 01:41:10.000000 bioext-0.9.4/lib/BioExt/_util.py
-drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-06-23 02:01:35.000000 bioext-0.9.4/lib/BioExt/stats/
--rw-r--r--   0 Lance      (502) staff       (20)     2666 2012-02-23 06:20:10.000000 bioext-0.9.4/lib/BioExt/stats/__init__.py
--rw-r--r--   0 Lance      (502) staff       (20)      367 2012-06-23 02:01:35.000000 bioext-0.9.4/PKG-INFO
--rw-r--r--   0 Lance      (502) staff       (20)       59 2012-06-23 02:01:35.000000 bioext-0.9.4/setup.cfg
--rw-r--r--   0 Lance      (502) staff       (20)      933 2012-06-23 02:00:48.000000 bioext-0.9.4/setup.py
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/bioext.egg-info/
+-rw-r--r--   0 Lance      (502) staff       (20)        1 2012-07-02 23:27:44.000000 bioext-0.9.5/bioext.egg-info/dependency_links.txt
+-rw-r--r--   0 Lance      (502) staff       (20)      367 2012-07-02 23:27:44.000000 bioext-0.9.5/bioext.egg-info/PKG-INFO
+-rw-r--r--   0 Lance      (502) staff       (20)      484 2012-07-02 23:27:44.000000 bioext-0.9.5/bioext.egg-info/SOURCES.txt
+-rw-r--r--   0 Lance      (502) staff       (20)        7 2012-07-02 23:27:44.000000 bioext-0.9.5/bioext.egg-info/top_level.txt
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/lib/
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/lib/BioExt/
+-rw-r--r--   0 Lance      (502) staff       (20)      255 2012-07-02 21:01:22.000000 bioext-0.9.5/lib/BioExt/__init__.py
+-rw-r--r--   0 Lance      (502) staff       (20)     4219 2012-04-18 21:42:21.000000 bioext-0.9.5/lib/BioExt/_orflist.py
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/lib/BioExt/_references/
+-rw-r--r--   0 Lance      (502) staff       (20)      323 2012-06-22 23:49:41.000000 bioext-0.9.5/lib/BioExt/_references/__init__.py
+-rw-r--r--   0 Lance      (502) staff       (20)     1488 2012-07-02 21:21:18.000000 bioext-0.9.5/lib/BioExt/_references/_factory.py
+-rw-r--r--   0 Lance      (502) staff       (20)     1022 2012-07-02 21:00:48.000000 bioext-0.9.5/lib/BioExt/_references/_lazyseq.py
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/lib/BioExt/_scorematrix/
+-rw-r--r--   0 Lance      (502) staff       (20)      294 2012-07-02 23:26:16.000000 bioext-0.9.5/lib/BioExt/_scorematrix/__init__.py
+-rw-r--r--   0 Lance      (502) staff       (20)      702 2012-07-02 21:25:52.000000 bioext-0.9.5/lib/BioExt/_scorematrix/_factory.py
+-rw-r--r--   0 Lance      (502) staff       (20)      756 2012-07-02 23:26:43.000000 bioext-0.9.5/lib/BioExt/_scorematrix/_lazyscorematrix.py
+-rw-r--r--   0 Lance      (502) staff       (20)     3474 2012-07-02 23:26:48.000000 bioext-0.9.5/lib/BioExt/_scorematrix/_scorematrix.py
+-rw-r--r--   0 Lance      (502) staff       (20)     6324 2012-06-23 01:41:10.000000 bioext-0.9.5/lib/BioExt/_util.py
+drwxr-xr-x   0 Lance      (502) staff       (20)        0 2012-07-02 23:27:44.000000 bioext-0.9.5/lib/BioExt/stats/
+-rw-r--r--   0 Lance      (502) staff       (20)     2666 2012-02-23 06:20:10.000000 bioext-0.9.5/lib/BioExt/stats/__init__.py
+-rw-r--r--   0 Lance      (502) staff       (20)      367 2012-07-02 23:27:44.000000 bioext-0.9.5/PKG-INFO
+-rw-r--r--   0 Lance      (502) staff       (20)       59 2012-07-02 23:27:44.000000 bioext-0.9.5/setup.cfg
+-rw-r--r--   0 Lance      (502) staff       (20)     1107 2012-07-02 21:24:25.000000 bioext-0.9.5/setup.py
```

### Comparing `bioext-0.9.4/lib/BioExt/_orflist.py` & `bioext-0.9.5/lib/BioExt/_orflist.py`

 * *Files identical despite different names*

### Comparing `bioext-0.9.4/lib/BioExt/_references/_factory.py` & `bioext-0.9.5/lib/BioExt/_references/_factory.py`

 * *Files identical despite different names*

### Comparing `bioext-0.9.4/lib/BioExt/_references/_lazyseq.py` & `bioext-0.9.5/lib/BioExt/_references/_lazyseq.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,10 +28,13 @@
         if ext in ('.gb',):
             filetype = 'genbank'
         elif ext in ('.fa', '.faa', '.fna'):
             filetype = 'fasta'
         else:
             msg = "reference has an unknown file type extension '%s'" % ext
             raise ValueError(msg)
-        with open(self._seqpath) as fh:
-            record = SeqIO.read(fh, filetype)
-        return record
+        if exists(self._seqpath):
+            with open(self._seqpath) as fh:
+                return SeqIO.read(fh, filetype)
+        else:
+            msg = "cannot load sequence '%s', file missing!" % self._seqpath
+            raise RuntimeError(msg)
```

### Comparing `bioext-0.9.4/lib/BioExt/_util.py` & `bioext-0.9.5/lib/BioExt/_util.py`

 * *Files identical despite different names*

### Comparing `bioext-0.9.4/lib/BioExt/stats/__init__.py` & `bioext-0.9.5/lib/BioExt/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `bioext-0.9.4/setup.py` & `bioext-0.9.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,18 +12,26 @@
 setup(name='bioext',
       version=_bioext_version,
       description='Misc utilities and definitions not included or hidden in biopython',
       author='N Lance Hepler',
       author_email='nlhepler@gmail.com',
       url='http://github.com/nlhepler/bioext',
       license='GNU GPL version 3',
-      packages=['BioExt', 'BioExt.stats', 'BioExt._references'],
+      packages=[
+        'BioExt',
+        'BioExt._references',
+        'BioExt._scorematrix',
+        'BioExt.stats'
+      ],
       package_dir={
         'BioExt': 'lib/BioExt',
         'BioExt._references': 'lib/BioExt/_references',
+        'BioExt._scorematrix': 'lib/BioExt/_scorematrix',
         'BioExt.stats': 'lib/BioExt/stats'
       },
       package_data={
-        'BioExt': _installrefdirs
+        'BioExt': [
+            'data/scorematrices/*.txt'
+        ] + _installrefdirs
       },
       requires=['Bio (>=1.58)', 'numpy (>=1.6)', 'scipy (>=0.10.1)']
      )
```

