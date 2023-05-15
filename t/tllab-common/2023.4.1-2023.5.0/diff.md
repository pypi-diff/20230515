# Comparing `tmp/tllab_common-2023.4.1.tar.gz` & `tmp/tllab_common-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tllab_common-2023.4.1.tar", max compression
+gzip compressed data, was "tllab_common-2023.5.0.tar", max compression
```

## Comparing `tllab_common-2023.4.1.tar` & `tllab_common-2023.5.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.4.1/LICENSE
--rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.4.1/README.md
--rw-r--r--   0        0        0      890 2023-05-09 13:39:29.933328 tllab_common-2023.4.1/pyproject.toml
--rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.4.1/tllab_common/__init__.py
--rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.4.1/tllab_common/findcells.py
--rw-r--r--   0        0        0     5262 2023-05-09 13:37:30.393996 tllab_common-2023.4.1/tllab_common/fit.py
--rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.4.1/tllab_common/misc.py
--rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.4.1/tllab_common/transform.txt
--rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.4.1/tllab_common/transforms.py
--rwxr-xr-x   0        0        0    68716 2023-04-06 14:47:24.519652 tllab_common-2023.4.1/tllab_common/wimread.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-26 07:43:57.060764 tllab_common-2023.5.0/LICENSE
+-rw-r--r--   0        0        0      770 2021-11-19 15:34:09.296030 tllab_common-2023.5.0/README.md
+-rw-r--r--   0        0        0      890 2023-05-15 13:29:04.713409 tllab_common-2023.5.0/pyproject.toml
+-rw-r--r--   0        0        0      461 2023-04-26 07:34:18.368614 tllab_common-2023.5.0/tllab_common/__init__.py
+-rwxr-xr-x   0        0        0    10047 2022-09-20 13:24:57.600406 tllab_common-2023.5.0/tllab_common/findcells.py
+-rw-r--r--   0        0        0     5262 2023-05-10 16:28:47.573261 tllab_common-2023.5.0/tllab_common/fit.py
+-rw-r--r--   0        0        0    10422 2023-04-26 14:30:00.605612 tllab_common-2023.5.0/tllab_common/misc.py
+-rw-r--r--   0        0        0      187 2021-10-14 16:27:02.346127 tllab_common-2023.5.0/tllab_common/transform.txt
+-rw-r--r--   0        0        0     9202 2022-08-08 15:25:51.713820 tllab_common-2023.5.0/tllab_common/transforms.py
+-rwxr-xr-x   0        0        0    69946 2023-05-15 13:07:41.540425 tllab_common-2023.5.0/tllab_common/wimread.py
+-rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 tllab_common-2023.5.0/PKG-INFO
```

### Comparing `tllab_common-2023.4.1/LICENSE` & `tllab_common-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/README.md` & `tllab_common-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/pyproject.toml` & `tllab_common-2023.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tllab_common"
-version = "2023.4.1"
+version = "2023.5.0"
 description = "Common code for the Lenstra lab."
 authors = ["Lenstra lab NKI <t.lenstra@nki.nl>"]
 license = "GPLv3"
 readme = "README.md"
 keywords = ["burst", "transcription"]
 include = ["transform.txt"]
 repository = "https://github.com/Lenstralab/tllab_common"
```

### Comparing `tllab_common-2023.4.1/tllab_common/findcells.py` & `tllab_common-2023.5.0/tllab_common/findcells.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/tllab_common/fit.py` & `tllab_common-2023.5.0/tllab_common/fit.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/tllab_common/misc.py` & `tllab_common-2023.5.0/tllab_common/misc.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/tllab_common/transforms.py` & `tllab_common-2023.5.0/tllab_common/transforms.py`

 * *Files identical despite different names*

### Comparing `tllab_common-2023.4.1/tllab_common/wimread.py` & `tllab_common-2023.5.0/tllab_common/wimread.py`

 * *Files 3% similar despite different names*

```diff
@@ -582,43 +582,50 @@
     @abstractmethod
     def __frame__(self, c, z, t):  # Override this, return the frame at c, z, t
         return np.random.randint(0, 255, self.shape[:2])
 
     def close(self):
         return
 
+    @staticmethod
+    def split_path_series(path):
+        if isinstance(path, str):
+            path = Path(path)
+        if isinstance(path, Path) and path.name.startswith('Pos'):
+            return path.parent, int(path.name.lstrip('Pos'))
+        return path, 0
+
     def __new__(cls, path, *args, **kwargs):
         if cls is not imread:
             return super().__new__(cls)
         if len(cls.__subclasses__()) == 0:
             raise Exception('Restart python kernel please!')
         if isinstance(path, imread):
             path = path.path
+        path, _ = imread.split_path_series(path)
         for subclass in sorted(cls.__subclasses__(), key=lambda subclass: subclass.priority):
             if subclass._can_open(Path(path)):
                 return super().__new__(subclass)
 
-    def __init__(self, path, series=0, transform=False, drift=False, beadfile=None, sigma=None, dtype=None, meta=None):
-        if isinstance(path, str):
-            path = Path(path)
+    def __init__(self, path, transform=False, drift=False, beadfile=None, sigma=None, dtype=None, meta=None):
+        path, self.series = self.split_path_series(path)
         if isinstance(path, Path):
             self.path = path.absolute()
             self.title = self.path.stem
             try:
                 self.acquisitiondate = datetime.fromtimestamp(os.path.getmtime(self.path)).strftime('%y-%m-%dT%H:%M:%S')
             except Exception:
                 self.acquisitiondate = ''
         else:
             self.path = path  # ndarray
         self.transform = transform
         self.drift = drift
         self.beadfile = beadfile
         self.dtype = dtype
         self.shape = (0, 0, 0, 0, 0)
-        self.series = series
         self.meta = meta
         self.pxsize = 1e-1
         self.settimeinterval = 0
         self.pxsizecam = 0
         self.magnification = 0
         self.exposuretime = (0,)
         self.deltaz = 1
@@ -638,16 +645,19 @@
         self.duolink = 'None'
         self.detector = [0, 1]
         self.track = [0]
         self.metadata = {}
         self.cache = deque_dict(16)
         self._frame_decorator = None
         self.frameoffset = (self.shape[0] / 2, self.shape[1] / 2)  # how far apart the centers of frame and sensor are
+        self.len_series = 1
 
         self.__metadata__()
+        if self.series >= self.len_series:
+            raise IndexError(f'Series {self.series} does not exist.')
 
         if not hasattr(self, 'cnamelist'):
             self.cnamelist = 'abcdefghijklmnopqrstuvwxyz'[:self.shape[2]]
 
         if self.meta is not None:
             for key, item in self.meta.items():
                 self.__dict__[key] = item
@@ -889,15 +899,15 @@
         return self
 
     def __exit__(self, *args, **kwargs):
         if hasattr(self, 'close'):
             self.close()
 
     def __reduce__(self):
-        return self.__class__, (self.path, self.series, self.transform, self.drift, self.beadfile, self.sigma,
+        return self.__class__, (self.path / f"Pos{self.series}", self.transform, self.drift, self.beadfile, self.sigma,
                                 self.dtype)
 
     def czt(self, n):
         """ returns indices c, z, t used when calling im(n)
         """
         if not isinstance(n, tuple):
             c = n % self.shape[2]
@@ -1205,25 +1215,32 @@
     def _can_open(path):
         return isinstance(path, Path) and path.suffix == '.czi'
 
     def __metadata__(self):
         # TODO: make sure frame function still works when a subblock has data from more than one frame
         self.reader = czifile.CziFile(self.path)
         self.shape = tuple([self.reader.shape[self.reader.axes.index(directory_entry)] for directory_entry in 'XYCZT'])
-
+        self.len_series = self.reader.shape[self.reader.axes.index('S')] if 'S' in self.reader.axes else 1
         filedict = {}
         for directory_entry in self.reader.filtered_subblock_directory:
             idx = self.get_index(directory_entry, self.reader.start)
-            for c in range(*idx[self.reader.axes.index('C')]):
-                for z in range(*idx[self.reader.axes.index('Z')]):
-                    for t in range(*idx[self.reader.axes.index('T')]):
-                        if (c, z, t) in filedict:
-                            filedict[(c, z, t)].append(directory_entry)
-                        else:
-                            filedict[(c, z, t)] = [directory_entry]
+            if 'S' in self.reader.axes and self.series in range(*idx[self.reader.axes.index('S')]):
+                for c in range(*idx[self.reader.axes.index('C')]):
+                    for z in range(*idx[self.reader.axes.index('Z')]):
+                        for t in range(*idx[self.reader.axes.index('T')]):
+                            if (c, z, t) in filedict:
+                                filedict[(c, z, t)].append(directory_entry)
+                            else:
+                                filedict[(c, z, t)] = [directory_entry]
+        x_min = min([f.start[f.axes.index('X')] for f in filedict[0, 0, 0]])
+        y_min = min([f.start[f.axes.index('Y')] for f in filedict[0, 0, 0]])
+        x_max = max([f.start[f.axes.index('X')] + f.shape[f.axes.index('X')] for f in filedict[0, 0, 0]])
+        y_max = max([f.start[f.axes.index('Y')] + f.shape[f.axes.index('Y')] for f in filedict[0, 0, 0]])
+        self.shape = (x_max - x_min, y_max - y_min) + \
+                     tuple([self.reader.shape[self.reader.axes.index(directory_entry)] for directory_entry in 'CZT'])
         self.filedict = filedict
         self.metadata = xmldata(untangle.parse(self.reader.metadata()))
 
         unit = {'nm': 1e9, 'µm': 1e6, 'um': 1e6, 'mm': 1e3, 'm': 1}
         for item in self.metadata['ImageDocument']['Metadata']['Scaling']['Items']['Distance']:
             if item['Id'] == 'X':
                 self.pxsize = float(item['Value']) * unit[item.get('DefaultUnitFormat', 'um')]
@@ -1283,20 +1300,25 @@
             self.track, self.detector = zip(*[[int(i) for i in re.findall(r'\d', c)] for c in self.cnamelist])
         except ValueError:
             self.track = tuple(range(len(self.cnamelist)))
             self.detector = (0,) * len(self.cnamelist)
 
     def __frame__(self, c=0, z=0, t=0):
         f = np.zeros(self.shape[:2], self.dtype)
-        for directory_entry in self.filedict[(c, z, t)]:
+        directory_entries = self.filedict[c, z, t]
+        x_min = min([f.start[f.axes.index('X')] for f in directory_entries])
+        y_min = min([f.start[f.axes.index('Y')] for f in directory_entries])
+        xy_min = {'X': x_min, 'Y': y_min}
+        for directory_entry in directory_entries:
             subblock = directory_entry.data_segment()
             tile = subblock.data(resize=True, order=0)
-            index = [slice(i - j, i - j + k) for i, j, k in
-                     zip(directory_entry.start, self.reader.start, tile.shape)]
-            index = tuple([index[self.reader.axes.index(i)] for i in 'XY'])
+            axes_min = [xy_min.get(ax, 0) for ax in directory_entry.axes]
+            index = [slice(i - j - m, i - j + k)
+                     for i, j, k, m in zip(directory_entry.start, self.reader.start, tile.shape, axes_min)]
+            index = tuple(index[self.reader.axes.index(i)] for i in 'XY')
             f[index] = tile.squeeze()
         return f
 
     def close(self):
         self.reader.close()
 
     @staticmethod
@@ -1309,25 +1331,17 @@
                                      self.reader.attachments()))[0].data())
         return sorted(tval[tval > 0])[:self.shape[4]]
 
 
 class metaread(imread):
     priority = 10
 
-    def __init__(self, path, series=None, *args, **kwargs):
-        path = Path(path)
-        self.acquisitiondate = datetime.fromtimestamp(os.path.getmtime(path.parent)).strftime('%y-%m-%dT%H:%M:%S')
-        if series is None:
-            super().__init__(path, int(re.findall(r'\d+', path.name)[0]), *args, **kwargs)
-        else:
-            super().__init__(path / str(series), series, *args, **kwargs)
-
     @staticmethod
     def _can_open(path):
-        return isinstance(path, Path) and path.parent.suffix.lower() == '.nd' or path.suffix.lower() == '.nd'
+        return isinstance(path, Path) and path.suffix.lower() == '.nd'
 
     def __metadata__(self):
         filelist = sorted([file for file in os.listdir(self.path.parent.parent)
                            if re.search(f'_s{self.series}(_|\\.tif$)', file, re.IGNORECASE)])
         with tifffile.TiffFile(self.path.parent.parent / filelist[0]) as tif:
             self.metadata = xmldata(tif.metaseries_metadata)
         self.nd_metadata = xmldata({line[0]: line[1] for line in metaread.parse_nd(
@@ -1418,22 +1432,26 @@
     priority = 20
 
     @staticmethod
     def _can_open(path):
         return isinstance(path, Path) and path.suffix == ''
 
     def __metadata__(self):
-        filelist = sorted([file for file in os.listdir(self.path) if re.search(r'^img_\d{3,}.*\d{3,}.*\.tif$', file,
-                                                                               re.IGNORECASE)])
+        pattern = re.compile(r'^img_\d{3,}.*\d{3,}.*\.tif$', re.IGNORECASE)
+        filelist = sorted([str(file.name)
+                           for file in (self.path / f"Pos{self.series}").iterdir() if pattern.search(str(file.name))])
+        pattern = re.compile('^Pos\d+$')
+        self.len_series = len([file for file in self.path.iterdir() if pattern.search(str(file.name))])
+
         try:
-            with tifffile.TiffFile(self.path / filelist[0]) as tif:
+            with tifffile.TiffFile(self.path / f"Pos{self.series}" / filelist[0]) as tif:
                 self.metadata = xmldata({key: yaml.safe_load(value)
                                          for key, value in tif.pages[0].tags[50839].value.items()})
         except Exception:  # fallback
-            self.metadata = xmldata(json.loads((self.path / 'metadata.txt').read_text()))
+            self.metadata = xmldata(json.loads((self.path / f"Pos{self.series}" / 'metadata.txt').read_text()))
 
         # compare channel names from metadata with filenames
         cnamelist = self.metadata.search('ChNames', [])
         cnamelist = [c for c in cnamelist if any([c in f for f in filelist])]
 
         self.filedict = {}
         maxc = 0
@@ -1487,15 +1505,15 @@
             self.magnification = self.pxsizecam / self.pxsize
         self.pcf = self.shape[2] * self.metadata.re_search(r'(?i)conversion\sfactor\scoeff', 1)
         self.filter = self.metadata.search('ZeissReflectorTurret-Label', self.filter)[0]
         self.track = [0] * self.shape[2]
         self.detector = list(range(self.shape[2]))
 
     def __frame__(self, c=0, z=0, t=0):
-        return tifffile.imread(self.path / self.filedict[(c, z, t)])
+        return tifffile.imread(self.path / f"Pos{self.series}" / self.filedict[(c, z, t)])
 
 
 class bfread(imread):
     """ This class is used as a last resort, when we don't have another way to open the file. We don't like it because
         it requires the java vm.
     """
     priority = 99  # panic and open with BioFormats
@@ -1507,17 +1525,15 @@
     def __metadata__(self):
         jvm().start_vm()  # We need java for this :(
         self.key = np.random.randint(1e9)
         self.reader = bioformats.get_image_reader(self.key, str(self.path))
         omexml = bioformats.get_omexml_metadata(str(self.path))
         self.metadata = xmldata(untangle.parse(omexml))
 
-        s = self.reader.rdr.getSeriesCount()
-        if self.series >= s:
-            print('Series {} does not exist.'.format(self.series))
+        self.len_series = self.reader.rdr.getSeriesCount()
         self.reader.rdr.setSeries(self.series)
 
         Y = self.reader.rdr.getSizeY()
         X = self.reader.rdr.getSizeX()
         C = self.reader.rdr.getSizeC()
         Z = self.reader.rdr.getSizeZ()
         T = self.reader.rdr.getSizeT()
```

### Comparing `tllab_common-2023.4.1/PKG-INFO` & `tllab_common-2023.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tllab-common
-Version: 2023.4.1
+Version: 2023.5.0
 Summary: Common code for the Lenstra lab.
 Home-page: https://github.com/Lenstralab/tllab_common
 License: GPLv3
 Keywords: burst,transcription
 Author: Lenstra lab NKI
 Author-email: t.lenstra@nki.nl
 Requires-Python: >=3.8,<4.0
```

