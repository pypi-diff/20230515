# Comparing `tmp/sparclclient-1.2.0b3.dev9-py3-none-any.whl.zip` & `tmp/sparclclient-1.2.0b4.dev0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,22 @@
-Zip file size: 30950 bytes, number of entries: 19
--rw-rw-r--  2.0 unx     8000 b- defN 23-Apr-20 21:46 sparcl/Results.py
--rw-rw-r--  2.0 unx     1035 b- defN 23-Apr-20 22:56 sparcl/__init__.py
+Zip file size: 31659 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx     8039 b- defN 23-Apr-30 18:22 sparcl/Results.py
+-rw-rw-r--  2.0 unx     1035 b- defN 23-May-15 13:20 sparcl/__init__.py
 -rw-rw-r--  2.0 unx      798 b- defN 23-Mar-15 14:12 sparcl/big_retrieve.py
--rw-rw-r--  2.0 unx    29684 b- defN 23-Apr-20 21:46 sparcl/client.py
+-rw-rw-r--  2.0 unx    29776 b- defN 23-May-15 13:11 sparcl/client.py
 -rw-rw-r--  2.0 unx      953 b- defN 23-Feb-08 18:38 sparcl/conf.py
 -rw-rw-r--  2.0 unx      887 b- defN 23-Mar-15 15:44 sparcl/dls_376.py
 -rw-rw-r--  2.0 unx     3813 b- defN 23-Apr-20 21:46 sparcl/exceptions.py
 -rw-rw-r--  2.0 unx     5002 b- defN 23-Mar-26 21:24 sparcl/fields.py
--rw-rw-r--  2.0 unx     9799 b- defN 23-Apr-20 22:52 sparcl/gather_2d.py
+-rw-rw-r--  2.0 unx     9254 b- defN 23-May-12 19:28 sparcl/gather_2d.py
+-rw-rw-r--  2.0 unx     1329 b- defN 23-Apr-30 15:12 sparcl/resample_spectra.py
 -rw-rw-r--  2.0 unx    13112 b- defN 23-Feb-08 18:38 sparcl/type_conversion.py
 -rw-rw-r--  2.0 unx     1867 b- defN 23-Feb-28 20:09 sparcl/unsupported.py
 -rw-rw-r--  2.0 unx     4682 b- defN 23-Mar-26 21:03 sparcl/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Feb-08 18:38 sparcl/benchmarks/__init__.py
 -rw-rw-r--  2.0 unx     9667 b- defN 23-Feb-08 18:38 sparcl/benchmarks/benchmarks.py
--rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/LICENSE
--rw-rw-r--  2.0 unx      872 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1518 b- defN 23-Apr-20 23:00 sparclclient-1.2.0b3.dev9.dist-info/RECORD
-19 files, 93364 bytes uncompressed, 28486 bytes compressed:  69.5%
+-rw-rw-r--  2.0 unx     1576 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      872 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1601 b- defN 23-May-15 13:22 sparclclient-1.2.0b4.dev0.dist-info/RECORD
+20 files, 94362 bytes uncompressed, 29067 bytes compressed:  69.2%
```

## zipnote {}

```diff
@@ -21,14 +21,17 @@
 
 Filename: sparcl/fields.py
 Comment: 
 
 Filename: sparcl/gather_2d.py
 Comment: 
 
+Filename: sparcl/resample_spectra.py
+Comment: 
+
 Filename: sparcl/type_conversion.py
 Comment: 
 
 Filename: sparcl/unsupported.py
 Comment: 
 
 Filename: sparcl/utils.py
@@ -36,23 +39,23 @@
 
 Filename: sparcl/benchmarks/__init__.py
 Comment: 
 
 Filename: sparcl/benchmarks/benchmarks.py
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev9.dist-info/LICENSE
+Filename: sparclclient-1.2.0b4.dev0.dist-info/LICENSE
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev9.dist-info/METADATA
+Filename: sparclclient-1.2.0b4.dev0.dist-info/METADATA
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev9.dist-info/WHEEL
+Filename: sparclclient-1.2.0b4.dev0.dist-info/WHEEL
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev9.dist-info/top_level.txt
+Filename: sparclclient-1.2.0b4.dev0.dist-info/top_level.txt
 Comment: 
 
-Filename: sparclclient-1.2.0b3.dev9.dist-info/RECORD
+Filename: sparclclient-1.2.0b4.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparcl/Results.py

```diff
@@ -58,15 +58,15 @@
                 if orig == '_dr':
                     # keep DR around unchanged. We need it to rename back
                     # to Internal Field Names later.
                     newrec[orig] = rec[orig]
                 else:
                     new = self.fields._science_name(orig, dr)
                     if new is None:
-                        keep = False
+                        keep = False # We don't have name mapping, toss rec
                     newrec[new] = rec[orig]
             if keep:
                 newrecs.append(_AttrDict(newrec))
         self.recs = newrecs
 
     # Convert Science field names to Internal field names.
     def to_internal_fields(self):
```

## sparcl/__init__.py

```diff
@@ -27,8 +27,8 @@
 #__version__ = '1.0.0b1.dev7'
 #__version__ = '1.0.0b1.dev8'
 #__version__ = '1.0.0b1.dev9'
 #__version__ = '1.0.1b2.dev1'
 #__version__ = '1.1rc1'
 #__version__ = '1.1rc2'
 #__version__ = '1.1'
-__version__ = '1.2.0b3.dev9'
+__version__ = '1.2.0b4.dev0'
```

## sparcl/client.py

```diff
@@ -663,14 +663,15 @@
     def retrieve_by_specid(self,
                            specid_list,
                            *,
                            svc='spectras',  # 'retrieve',
                            format='pkl',    # 'json',
                            include='DEFAULT',
                            dataset_list=None,
+                           limit=500,
                            verbose=False):
         """Retrieve spectra records from the SPARC database by list of specids.
 
         Args:
             specid_list (:obj:`list`): List of specids.
 
             include (:obj:`list`, optional): List of field names to include
@@ -712,22 +713,23 @@
             constraints = {'specid': specid_list,
                            'data_release': dataset_list}
 
         # Science Field Name for uuid.
         dr = list(self.fields.all_drs)[0]
         idfld = self.fields._science_name('id', dr)
 
-        found = self.find([idfld], constraints=constraints)
+        found = self.find([idfld], constraints=constraints, limit=limit)
         if verbose:
             print(f'Found {found.count} matches.')
         res = self.retrieve(found.ids,
                             svc=svc,
                             format=format,
                             include=include,
                             dataset_list=dataset_list,
+                            limit=limit,
                             verbose=verbose)
         if verbose:
             print(f'Got {res.count} records.')
         return res
 
 
 if __name__ == "__main__":
```

## sparcl/gather_2d.py

```diff
@@ -1,54 +1,22 @@
 """Align or resample spectra related fields across multiple records."""
 # See client.py for Doctest example
 #
-# See:
-#   https://spectres.readthedocs.io/en/latest/
 # For info about problems with floating point,
 #   See:  https://docs.python.org/3/tutorial/floatingpoint.html
 #   Also: https://docs.python.org/3/library/decimal.html#floating-point-notes
 #
 import math
 from decimal import Decimal
 #
-import spectres
 import numpy as np
 #
 import sparcl.client
 
 
-# Per paper, should be able to pass all flux in one call to spectres
-# https://arxiv.org/pdf/1705.05165.pdf
-# Perhaps users would rather the bins uniform (1,5,20 Angstroms?)
-def _resample_flux(records, wavstep=1):
-    smallest = math.floor(min([min(r.wavelength) for r in records]))
-    largest = math.ceil(max([max(r.wavelength) for r in records]))
-
-    #!wrange = largest - smallest
-    #new_wavs = np.fromfunction(lambda i: i + smallest, (wrange,), dtype=int)
-    #flux_2d = np.ones([len(records), wrange])
-
-    new_wavs = np.array(range(smallest, largest + 1, wavstep))
-    flux_2d = np.full([len(records), len(new_wavs)], None, dtype=float)
-
-    for idx, rec in enumerate(records):
-        flux_2d[idx] = spectres.spectres(new_wavs,
-                                         rec.wavelength,
-                                         rec.flux,
-                                         verbose=False)
-    return flux_2d, new_wavs
-
-
-def _tt0(numrecs=20):
-    client = sparcl.client.SparclClient()
-    found = client.find(constraints=dict(data_release=['BOSS-DR16']),
-                        limit=numrecs)
-    got = client.retrieve(found.ids)
-    flux_2d, new_wavs = _resample_flux(got.records)
-    return flux_2d, new_wavs
 
 
 # Map every wavelength of every record to index (ri,wi)
 # where
 #   ri: Record Index
 #   wi: Window Index (offset of wavelength in WINDOW)
 #   window: ordered list of wavelengths that include ALL unique
@@ -84,22 +52,25 @@
     for ri, rec in enumerate(records):
         for wi, rwl in enumerate(rec.wavelength):  # wi=recwavelengthIndex
             if precision is None:
                 recwl = Decimal(rwl)
             else:
                 recwl = Decimal(rwl).quantize(PLACES)
             wwl = window[offsets[ri] + wi]
-            msg = (f'Wavelength in '
-                   f'Record[{ri}][{wi}] ({recwl}) does not match '
-                   f'Window[{offsets[ri]+wi} = offset[{ri}]={offsets[ri]} '
-                   f'+ {wi}]  ({wwl})'
-                   )
-            assert recwl == wwl, msg
-            # f'RecWL[{wi}] {rwl} != WindowWL[{offsets[ri+wi]}] {wwl} '
-            # f'offset={offsets[ri]}')
+            #! msg = (f'Wavelength in '
+            #!        f'Record[{ri}][{wi}] ({recwl}) does not match '
+            #!        f'Window[{offsets[ri]+wi} = offset[{ri}]={offsets[ri]} '
+            #!        f'+ {wi}]  ({wwl})'
+            #!        )
+            #! assert recwl == wwl, msg
+            if recwl != wwl:
+                msg = (f'The spectra cannot be aligned with the given'
+                       f' "precision" parameter ({precision}).'
+                       f' Try lowering the precision value.')
+                raise Exception(msg)
 
 
 # We want to align a bunch of records by wavelength into a single
 # 2d numpy array (record vs wavelength).  In general, we
 # are not guaranteed that this is possible -- even if using only
 # records from a single DataSet. So validate it first.
 # (If not valid, allowing wavelength slop might help.)
@@ -123,14 +94,15 @@
     print(f'Built window len={len(window)}; offsets={offsets}')
     #return records, window, offsets
     ar = _align_wavelengths(records)
     return ar
 
 
 # precision:: number of decimal places
+# "records" must contain "wavelength" field.
 def _wavelength_grid_offsets(records, precision=11):
     PLACES = Decimal(10) ** -precision
 
     # set of wavelengths from ALL records. Quantized to precision
     gset = set()  # Grid SET
     for r in records:
         gset.update([Decimal(w).quantize(PLACES) for w in r.wavelength])
@@ -171,55 +143,67 @@
 
 # Align flux from records into one array using quantization
 #! def flux_records(records, precision=None):
 #!     grid, offsets = wavelength_grid_offsets(records, precision=precision)
 #!     ar = _flux_grid(records, grid, offsets, precision=precision)
 #!     return ar, np.array([float(x) for x in grid])
 
+def _validate_spectra_fields(records, fields):
+    spectra_fields = [client.fields.n2o['BOSS-DR16'][k] for k,v in client.fields.attrs['BOSS-DR16'].items() if v['storage']=='S']
+    [k for k in records[0].keys() if not k.startswith('_')]
+
+
 # TOP level: Intended for access from Jupyter NOTEBOOK.
 # Align spectra related field from records into one array using quantization.
-def align_records(records, fields=None, precision=7):
+def align_records(records, fields=['flux','wavelength'], precision=7):
     """Align given spectra-type fields to a common wavelength grid.
 
     Args:
         records (list): List of dictionaries. The keys for all these dictionaries
             are Science Field Names.
 
         fields (:obj:`list`, optional): List of Science Field Names of
             spectra related fields to align and include in the results.
+            DEFAULT=['flux', 'wavelength']
 
         precision (:obj:`int`, optional): Number of decimal points to use for
-            quantizing wavelengths into a grid. Default=7
+            quantizing wavelengths into a grid.
+            DEFAULT=7
 
     Returns:
         tuple containing:
         - ar_dict(dict): Dictionary of 2D numpy arrays keyed by Field Name.
               Each array is shape: (numRecs, numzGridWavelengths)
         - grid(ndarray): 1D numpy array containing wavelength values.
 
     Example:
         >>> client = sparcl.client.SparclClient()
-        >>> specflds = ['wavelength', 'flux', 'ivar', 'mask', 'model']
+        >>> specflds = ['wavelength', 'model']
         >>> cons = {"data_release": ['BOSS-DR16']}
         >>> found = client.find(constraints=cons, limit=21)
         >>> got = client.retrieve(found.ids, include=specflds)
         >>> ar_dict, grid = align_records(got.records, fields=specflds)
         >>> ar_dict['model'].shape
         (21, 4670)
 
     """
+    # Report Garbage In
+    if 'wavelength' not in fields:
+        msg = (f'You must provide "wavelength" in the list provided'
+               f' in the "fields" paramter.  Got: {fields}')
+        raise Exception(msg)
+    if 'wavelength' not in records[0]:
+        msg = (f'Records must contain the "wavelength" field.'
+               f' The first record contains fields: {sorted(records[0].keys())}')
+        raise Exception(msg)
+
+    #! _validate_spectra_fields(records, fields)
     grid, offsets = _wavelength_grid_offsets(records, precision=precision)
     _validate_wavelength_alignment(records, grid, offsets, precision=precision)
 
-    # One slice for each record; each slice a 2darray(wavelength, fieldName)=fldVal
-    #! slices = list()
-    #! for rec in records:
-    #!     ar = rec_grid(rec, fields, grid, offsets, precision=None):
-    #!     slices.append(ar)
-
     # One slice for each field; each slice a 2darray(wavelength, record)=fldVal
     adict = dict()
     for fld in fields:
         ar = _field_grid(records, fld, grid, offsets, precision=None)
         adict[fld] = ar
 
     return adict, np.array([float(x) for x in grid])
```

## Comparing `sparclclient-1.2.0b3.dev9.dist-info/LICENSE` & `sparclclient-1.2.0b4.dev0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparclclient-1.2.0b3.dev9.dist-info/METADATA` & `sparclclient-1.2.0b4.dev0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparclclient
-Version: 1.2.0b3.dev9
+Version: 1.2.0b4.dev0
 Summary: A client for getting spectra data from NOIRLab.
 Home-page: https://github.com/astro-datalab/sparclclient
 Author: NOIRLab DataLab
 Author-email: datalab-spectro@noirlab.edu
 Project-URL: Documentation, https://sparclclient.readthedocs.io/en/latest/
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3.6
```

## Comparing `sparclclient-1.2.0b3.dev9.dist-info/RECORD` & `sparclclient-1.2.0b4.dev0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-sparcl/Results.py,sha256=yHetKpwujeqW2RXloo-_9d3JgTu11VLrwSZzVwqZcJU,8000
-sparcl/__init__.py,sha256=OxAYp-Ca2BNX2OhG2VesOv1QdBPa5TPbkdiaG2xp4gY,1035
+sparcl/Results.py,sha256=S4jQcXnw6qfdIEL-NEsCqMK6LolFaERGxjNWIvNhACM,8039
+sparcl/__init__.py,sha256=zTDqx1DZGxvXQ9ixlF3fwnBoK112erhc-7tJLpBwjdY,1035
 sparcl/big_retrieve.py,sha256=q0ScH87QqPL4bz4g0hB0AO3k4c_TiuQrWjBJHqHhE60,798
-sparcl/client.py,sha256=EbLkZmEnTMUh2AnijIrqIbUalAcm3LQnGM6RkBbTWUM,29684
+sparcl/client.py,sha256=IEbXDqMsnMGcuhuSgvQNhVhwOdJgWFQDLcH68qp4dzE,29776
 sparcl/conf.py,sha256=O9l4-vpWBZK0QjhHxjskGO8kHPxBj7mkWlchd2rot1c,953
 sparcl/dls_376.py,sha256=WvZjuZFRU0jgH3ELRrMQdslkMWiF2wFQrSag0cYii-I,887
 sparcl/exceptions.py,sha256=q7ONsLsop9OQJJCD4SEzfdsojv0yo3WQT0SluaxGOQ0,3813
 sparcl/fields.py,sha256=7MpaJQr2d1GktS7aeM4010jyLqDdKQ7BZIF9hM0IjII,5002
-sparcl/gather_2d.py,sha256=0AOBbjt8orrMg-IgOgIjTruHMFxlUqwgN5WTopab7Ao,9799
+sparcl/gather_2d.py,sha256=ZRr41vNHV4tnf63-QuTu04SlWv6TOzK-CeHpbt9YwOY,9254
+sparcl/resample_spectra.py,sha256=2MO-sDCCFg2eNiK6jQs2EJRu4bNnXycGV8WaOydssG4,1329
 sparcl/type_conversion.py,sha256=RX7OD1iGuuUrf-yAd0ISdiqBq4CP7QlCw0vvkAdHdsQ,13112
 sparcl/unsupported.py,sha256=vkSaK3Ppcxx6mMsqBktUjI0uS7RwBJYH2BkBABsnyIM,1867
 sparcl/utils.py,sha256=YlLUP0j4thUyEwTJAaqJ7zzsvbCxPe5EYTn9kvWGfBY,4682
 sparcl/benchmarks/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 sparcl/benchmarks/benchmarks.py,sha256=FPZ2KExfVWHhGt3B4VyfgOhxxsemj7OeBWJO0dyDDC4,9667
-sparclclient-1.2.0b3.dev9.dist-info/LICENSE,sha256=y10EluGMCzGs9X4oYCYyix3l6u-lawB_vlGR8qe442Q,1576
-sparclclient-1.2.0b3.dev9.dist-info/METADATA,sha256=6vglH_6at8TrSgsV8eoWxycL0E-zjUfyCqomQ-R3nhA,872
-sparclclient-1.2.0b3.dev9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-sparclclient-1.2.0b3.dev9.dist-info/top_level.txt,sha256=d5CZ3Duxq3MyQTB2ZqOrdtSBv4GdVceF-pOZFmsuHZY,7
-sparclclient-1.2.0b3.dev9.dist-info/RECORD,,
+sparclclient-1.2.0b4.dev0.dist-info/LICENSE,sha256=y10EluGMCzGs9X4oYCYyix3l6u-lawB_vlGR8qe442Q,1576
+sparclclient-1.2.0b4.dev0.dist-info/METADATA,sha256=E9oVUvxzIgf8GLHD_0ET14UWRzmCcG2lR9u7p5iPvIg,872
+sparclclient-1.2.0b4.dev0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+sparclclient-1.2.0b4.dev0.dist-info/top_level.txt,sha256=d5CZ3Duxq3MyQTB2ZqOrdtSBv4GdVceF-pOZFmsuHZY,7
+sparclclient-1.2.0b4.dev0.dist-info/RECORD,,
```

