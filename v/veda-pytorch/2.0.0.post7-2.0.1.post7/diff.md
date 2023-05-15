# Comparing `tmp/veda_pytorch-2.0.0.post7-py3-none-manylinux_2_17_x86_64.whl.zip` & `tmp/veda_pytorch-2.0.1.post7-py3-none-manylinux_2_17_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 258554 bytes, number of entries: 8
+Zip file size: 258552 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       18 b- defN 23-Apr-26 08:06 veda/pytorch/__init__.py
--rw-r--r--  2.0 unx     4683 b- defN 23-Apr-26 08:23 veda/pytorch/lib.py
--rwxr-xr-x  2.0 unx  1151592 b- defN 23-Apr-26 08:23 veda/pytorch/lib64/libveda-pytorch.so
--rw-r--r--  2.0 unx     1531 b- defN 23-Apr-26 08:06 veda_pytorch-2.0.0.post7.dist-info/LICENSE
--rw-------  2.0 unx     2723 b- defN 23-Apr-26 08:23 veda_pytorch-2.0.0.post7.dist-info/METADATA
--rw-------  2.0 unx      105 b- defN 23-Apr-26 08:23 veda_pytorch-2.0.0.post7.dist-info/WHEEL
--rw-------  2.0 unx       12 b- defN 23-Apr-26 08:23 veda_pytorch-2.0.0.post7.dist-info/top_list.txt
--rw-------  2.0 unx      709 b- defN 23-Apr-26 08:23 veda_pytorch-2.0.0.post7.dist-info/RECORD
-8 files, 1161373 bytes uncompressed, 257338 bytes compressed:  77.8%
+-rw-r--r--  2.0 unx     4683 b- defN 23-May-15 06:03 veda/pytorch/lib.py
+-rwxr-xr-x  2.0 unx  1151592 b- defN 23-May-15 06:03 veda/pytorch/lib64/libveda-pytorch.so
+-rw-r--r--  2.0 unx     1531 b- defN 23-Apr-26 08:06 veda_pytorch-2.0.1.post7.dist-info/LICENSE
+-rw-------  2.0 unx     2723 b- defN 23-May-15 06:03 veda_pytorch-2.0.1.post7.dist-info/METADATA
+-rw-------  2.0 unx      105 b- defN 23-May-15 06:03 veda_pytorch-2.0.1.post7.dist-info/WHEEL
+-rw-------  2.0 unx       12 b- defN 23-May-15 06:03 veda_pytorch-2.0.1.post7.dist-info/top_list.txt
+-rw-------  2.0 unx      709 b- defN 23-May-15 06:03 veda_pytorch-2.0.1.post7.dist-info/RECORD
+8 files, 1161373 bytes uncompressed, 257336 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: veda/pytorch/lib.py
 Comment: 
 
 Filename: veda/pytorch/lib64/libveda-pytorch.so
 Comment: 
 
-Filename: veda_pytorch-2.0.0.post7.dist-info/LICENSE
+Filename: veda_pytorch-2.0.1.post7.dist-info/LICENSE
 Comment: 
 
-Filename: veda_pytorch-2.0.0.post7.dist-info/METADATA
+Filename: veda_pytorch-2.0.1.post7.dist-info/METADATA
 Comment: 
 
-Filename: veda_pytorch-2.0.0.post7.dist-info/WHEEL
+Filename: veda_pytorch-2.0.1.post7.dist-info/WHEEL
 Comment: 
 
-Filename: veda_pytorch-2.0.0.post7.dist-info/top_list.txt
+Filename: veda_pytorch-2.0.1.post7.dist-info/top_list.txt
 Comment: 
 
-Filename: veda_pytorch-2.0.0.post7.dist-info/RECORD
+Filename: veda_pytorch-2.0.1.post7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## veda/pytorch/lib.py

```diff
@@ -1,16 +1,16 @@
 __all__ = []
 
 import ctypes
 import os
 import collections
 import torch # make sure pytorch was loaded before
 
-if not "2.0.0" in torch.__version__:
-	raise Exception(f"The NEC SX-Aurora TSUBASA can only be used with PyTorch v2.0.0 but you are using {torch.__version__}")
+if not "2.0.1" in torch.__version__:
+	raise Exception(f"The NEC SX-Aurora TSUBASA can only be used with PyTorch v2.0.1 but you are using {torch.__version__}")
 
 cwd				= os.path.dirname(__file__)
 libvedapytorch	= ctypes.cdll.LoadLibrary(os.path.join(cwd, 'lib64/libveda-pytorch.so'))
 libveda			= ctypes.cdll.LoadLibrary(os.path.join(cwd, '../lib64/libveda.so.2'))
 
 libvedapytorch.veda_pytorch_get_current_device.argtypes	= []
 libvedapytorch.veda_pytorch_get_current_device.restype	= ctypes.c_int
```

## Comparing `veda_pytorch-2.0.0.post7.dist-info/LICENSE` & `veda_pytorch-2.0.1.post7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `veda_pytorch-2.0.0.post7.dist-info/METADATA` & `veda_pytorch-2.0.1.post7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: veda-pytorch
-Version: 2.0.0.post7
+Version: 2.0.1.post7
 Requires-Python: >=3.7
 Summary: VEDA PyTorch
 Author: Nicolas Weber
 Author-email: nicolas.weber@neclab.eu
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: C
 Classifier: Programming Language :: C++
 Download-URL: https://github.com/sx-aurora/veda-pytorch/tags
 License: 3 BSD-License
 Platform: linux_x86_x64
 Requires-Dist: veda (>= 2.0.1, < 3)
 Requires-Dist: tungl (>= 0.1.3, < 0.2)
 Requires-Dist: veda-tensors (>= 0.1.4, < 0.2)
-Requires-Dist: torch==2.0.0
+Requires-Dist: torch==2.0.1
 Description-Content-Type: text/markdown
 
 # VEDA PyTorch
 
 VEDA PyTorch is a library to add device support for the NEC SX-Aurora TSUBASA into PyTorch.
 
 [![Github](https://img.shields.io/github/v/tag/sx-aurora/veda-pytorch?display_name=tag&sort=semver)](https://github.com/sx-aurora/veda)
```

### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: veda-pytorch Version: 2.0.0.post7 Requires-Python:
+Metadata-Version: 2.1 Name: veda-pytorch Version: 2.0.1.post7 Requires-Python:
 >=3.7 Summary: VEDA PyTorch Author: Nicolas Weber Author-email:
 nicolas.weber@neclab.eu Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: C Classifier: Programming Language :: C++ Download-URL: https://
 github.com/sx-aurora/veda-pytorch/tags License: 3 BSD-License Platform:
 linux_x86_x64 Requires-Dist: veda (>= 2.0.1, < 3) Requires-Dist: tungl (>=
 0.1.3, < 0.2) Requires-Dist: veda-tensors (>= 0.1.4, < 0.2) Requires-Dist:
-torch==2.0.0 Description-Content-Type: text/markdown # VEDA PyTorch VEDA
+torch==2.0.1 Description-Content-Type: text/markdown # VEDA PyTorch VEDA
 PyTorch is a library to add device support for the NEC SX-Aurora TSUBASA into
 PyTorch. [![Github](https://img.shields.io/github/v/tag/sx-aurora/veda-
 pytorch?display_name=tag&sort=semver)](https://github.com/sx-aurora/veda) [!
 [PyPI](https://img.shields.io/pypi/v/veda-pytorch)](https://pypi.org/project/
 veda-pytorch) [![License](https://img.shields.io/pypi/l/veda-pytorch)](https://
 pypi.org/project/veda-pytorch) ![Python Versions](https://img.shields.io/pypi/
 pyversions/veda-pytorch) ![Linux](https://svgshare.com/i/Zhy.svg) !
```

## Comparing `veda_pytorch-2.0.0.post7.dist-info/RECORD` & `veda_pytorch-2.0.1.post7.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 veda/pytorch/__init__.py, sha256=ZlxwBNSC9gj0M-kDloW5EB13rFzpyIIhGQbXXO1JkCg, 18
-veda/pytorch/lib.py, sha256=8wIJCe-_5uRuVTSk4NSyxemLKuwyMVLPFoVuvh8uY0c, 4683
+veda/pytorch/lib.py, sha256=nEU2HE3pWeYrXYhK9zuHSRNbfFg762UdTox3kcRzZ1k, 4683
 veda/pytorch/lib64/libveda-pytorch.so, sha256=Qj0xWliuBGhaJgtkj18H2mhHDT83sp0rltioHisjAnk, 1151592
-veda_pytorch-2.0.0.post7.dist-info/LICENSE, sha256=YnSGopDGJS9GdQ5iKK7kjgkcB9tcrtgilusqFvMPfNc, 1531
-veda_pytorch-2.0.0.post7.dist-info/METADATA, sha256=FyICpHzobOuWuYf60n8ax6uK6buLcimHSBNWj2Crh10, 2723
-veda_pytorch-2.0.0.post7.dist-info/top_list.txt, sha256=sgW9QjJvB2Gdb2yhdOJEHj-4tk_N4N82wUwPpJvPMnY, 12
-veda_pytorch-2.0.0.post7.dist-info/WHEEL, sha256=1zYEQ6pqba8DUYFxuTE6wbStr1rDJ-OPIGPCUjtGm-c, 105
-veda_pytorch-2.0.0.post7.dist-info/RECORD, , 
+veda_pytorch-2.0.1.post7.dist-info/LICENSE, sha256=YnSGopDGJS9GdQ5iKK7kjgkcB9tcrtgilusqFvMPfNc, 1531
+veda_pytorch-2.0.1.post7.dist-info/METADATA, sha256=B5sfljx_uXWCv2O2ENw7tQfXNcPyq1J3rWSpn46M6nQ, 2723
+veda_pytorch-2.0.1.post7.dist-info/top_list.txt, sha256=sgW9QjJvB2Gdb2yhdOJEHj-4tk_N4N82wUwPpJvPMnY, 12
+veda_pytorch-2.0.1.post7.dist-info/WHEEL, sha256=1zYEQ6pqba8DUYFxuTE6wbStr1rDJ-OPIGPCUjtGm-c, 105
+veda_pytorch-2.0.1.post7.dist-info/RECORD, ,
```

