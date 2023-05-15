# Comparing `tmp/gtirb-1.9.0.tar.gz` & `tmp/gtirb-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gtirb-1.9.0.tar", last modified: Mon Nov  2 15:46:28 2020, max compression
+gzip compressed data, was "dist/gtirb-1.9.1.tar", last modified: Thu Nov 12 13:45:17 2020, max compression
```

## Comparing `gtirb-1.9.0.tar` & `gtirb-1.9.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 15:46:28.000000 gtirb-1.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1872 2020-11-02 15:44:05.000000 gtirb-1.9.0/setup.py
--rw-r--r--   0 root         (0) root         (0)    10576 2020-11-02 15:46:28.000000 gtirb-1.9.0/README
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-02 15:46:28.000000 gtirb-1.9.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      776 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)    13097 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb/
--rw-rw-rw-   0 root         (0) root         (0)     9575 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/symbolicexpression.py
--rw-rw-rw-   0 root         (0) root         (0)     8817 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/cfg.py
--rw-rw-rw-   0 root         (0) root         (0)    12410 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/block.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5274 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/symbol.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-02 15:46:28.000000 gtirb-1.9.0/gtirb/proto/
--rw-r--r--   0 root         (0) root         (0)     2457 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/Offset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2472 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/AuxData_pb2.py
--rw-r--r--   0 root         (0) root         (0)    12671 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/SymbolicExpression_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4192 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/Symbol_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2120 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/ProxyBlock_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/proto/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6187 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/IR_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7858 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/CFG_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13448 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/Module_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9970 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/ByteInterval_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5387 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/Section_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2502 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/DataBlock_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2895 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/proto/CodeBlock_pb2.py
--rw-rw-rw-   0 root         (0) root         (0)     1162 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/offset.py
--rw-rw-rw-   0 root         (0) root         (0)     4668 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/util.py
--rw-rw-rw-   0 root         (0) root         (0)      265 2020-11-02 15:44:05.000000 gtirb-1.9.0/gtirb/version.py
--rw-rw-rw-   0 root         (0) root         (0)    18823 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/serialization.py
--rw-rw-rw-   0 root         (0) root         (0)     5609 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/auxdata.py
--rw-rw-rw-   0 root         (0) root         (0)    16570 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/byteinterval.py
--rw-rw-rw-   0 root         (0) root         (0)    20900 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/module.py
--rw-rw-rw-   0 root         (0) root         (0)    12652 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/section.py
--rw-rw-rw-   0 root         (0) root         (0)     2412 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/node.py
--rw-rw-rw-   0 root         (0) root         (0)    14653 2020-11-02 15:44:06.000000 gtirb-1.9.0/gtirb/ir.py
--rw-r--r--   0 root         (0) root         (0)    13097 2020-11-02 15:46:28.000000 gtirb-1.9.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-12 13:45:17.000000 gtirb-1.9.1/
+-rw-r--r--   0 root         (0) root         (0)    13391 2020-11-12 13:45:17.000000 gtirb-1.9.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10806 2020-11-12 13:45:17.000000 gtirb-1.9.1/README
+-rw-r--r--   0 root         (0) root         (0)       38 2020-11-12 13:45:17.000000 gtirb-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1884 2020-11-12 13:42:31.000000 gtirb-1.9.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      776 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)    13391 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       61 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb.egg-info/requires.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb/
+-rw-rw-rw-   0 root         (0) root         (0)     4668 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    14130 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/ir.py
+-rw-rw-rw-   0 root         (0) root         (0)    16570 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/byteinterval.py
+-rw-rw-rw-   0 root         (0) root         (0)     5609 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/auxdata.py
+-rw-rw-rw-   0 root         (0) root         (0)    10094 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-12 13:45:17.000000 gtirb-1.9.1/gtirb/proto/
+-rw-r--r--   0 root         (0) root         (0)     4192 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/Symbol_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9970 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/ByteInterval_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7858 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/CFG_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2502 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/DataBlock_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6187 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/IR_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5387 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/Section_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2457 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/Offset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    12671 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/SymbolicExpression_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13448 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/Module_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/ProxyBlock_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/CodeBlock_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2472 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/proto/AuxData_pb2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/node.py
+-rw-rw-rw-   0 root         (0) root         (0)      265 2020-11-12 13:42:31.000000 gtirb-1.9.1/gtirb/version.py
+-rw-rw-rw-   0 root         (0) root         (0)    12652 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/section.py
+-rw-rw-rw-   0 root         (0) root         (0)    11712 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/block.py
+-rw-rw-rw-   0 root         (0) root         (0)     1162 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/offset.py
+-rw-rw-rw-   0 root         (0) root         (0)     9575 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/symbolicexpression.py
+-rw-rw-rw-   0 root         (0) root         (0)    18823 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/serialization.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20900 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/module.py
+-rw-rw-rw-   0 root         (0) root         (0)     5274 2020-11-12 13:42:32.000000 gtirb-1.9.1/gtirb/symbol.py
```

### Comparing `gtirb-1.9.0/setup.py` & `gtirb-1.9.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,22 +37,22 @@
         )
 
     setuptools.setup(
         name="gtirb",
         version=(
             "1"
             ".9"
-            ".0"
+            ".1"
         ),
         author="GrammaTech",
         author_email="gtirb@grammatech.com",
         description="GrammaTech Intermediate Representation for Binaries",
         packages=setuptools.find_packages(),
         test_suite="setup.gtirb_test_suite",
-        install_requires=["protobuf<3.12.2"] + typing_dep,
+        install_requires=["networkx", "protobuf<3.12.2"] + typing_dep,
         classifiers=[
             "Programming Language :: Python :: 3",
             "License :: OSI Approved :: MIT License",
             "Operating System :: OS Independent",
         ],
         python_requires=">=3",
         long_description=long_description,
```

### Comparing `gtirb-1.9.0/README` & `gtirb-1.9.1/README`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,22 @@
 instructions.  GTIRB is versioned with Major.Minor.Patch versioning
 where Major version increments will require significant source changes
 but should be very rare, Minor version increments may require small
 source changes, and Patch version increments shouldn't break any
 downstream builds.  We do not yet provide ABI compatibility across any
 version changes.
 
+## Python API
+The GTIRB Python API may be installed with the following.  Note
+however, that installation of the `ddisasm` and `gtirb-pprinter`
+packages as described below is recommended for every API.
+```sh
+pip install gtirb
+```
+
 ## Windows
 Pre-built debug and release binaries are available for Windows at:
 [windows-debug/](https://grammatech.github.io/gtirb/pkgs/windows-debug/),
 and
 [windows-release/](https://grammatech.github.io/gtirb/pkgs/windows-release/).
 A symbol server for the debugging symbols for both the release and
 debug binaries is available at
```

### Comparing `gtirb-1.9.0/gtirb.egg-info/SOURCES.txt` & `gtirb-1.9.1/gtirb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb.egg-info/PKG-INFO` & `gtirb-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtirb
-Version: 1.9.0
+Version: 1.9.1
 Summary: GrammaTech Intermediate Representation for Binaries
 Home-page: https://github.com/grammatech/gtirb
 Author: GrammaTech
 Author-email: gtirb@grammatech.com
 License: MIT
 Description: # GTIRB
         
@@ -102,14 +102,22 @@
         instructions.  GTIRB is versioned with Major.Minor.Patch versioning
         where Major version increments will require significant source changes
         but should be very rare, Minor version increments may require small
         source changes, and Patch version increments shouldn't break any
         downstream builds.  We do not yet provide ABI compatibility across any
         version changes.
         
+        ## Python API
+        The GTIRB Python API may be installed with the following.  Note
+        however, that installation of the `ddisasm` and `gtirb-pprinter`
+        packages as described below is recommended for every API.
+        ```sh
+        pip install gtirb
+        ```
+        
         ## Windows
         Pre-built debug and release binaries are available for Windows at:
         [windows-debug/](https://grammatech.github.io/gtirb/pkgs/windows-debug/),
         and
         [windows-release/](https://grammatech.github.io/gtirb/pkgs/windows-release/).
         A symbol server for the debugging symbols for both the release and
         debug binaries is available at
```

### Comparing `gtirb-1.9.0/gtirb/symbolicexpression.py` & `gtirb-1.9.1/gtirb/symbolicexpression.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/block.py` & `gtirb-1.9.1/gtirb/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -286,41 +286,23 @@
             "offset={offset}, "
             "decode_mode={decode_mode}, "
             ")".format(**self.__dict__)
         )
 
     @property
     def incoming_edges(self):
-        if (
-            self.byte_interval is None
-            or self.byte_interval.section is None
-            or self.byte_interval.section.module is None
-            or self.byte_interval.section.module.ir is None
-        ):
+        if self.ir is None:
             return ()
-        return (
-            e
-            for e in self.byte_interval.section.module.ir.cfg
-            if e.target == self
-        )
+        return self.ir.cfg.in_edges(self)
 
     @property
     def outgoing_edges(self):
-        if (
-            self.byte_interval is None
-            or self.byte_interval.section is None
-            or self.byte_interval.section.module is None
-            or self.byte_interval.section.module.ir is None
-        ):
+        if self.ir is None:
             return ()
-        return (
-            e
-            for e in self.byte_interval.section.module.ir.cfg
-            if e.source == self
-        )
+        return self.ir.cfg.out_edges(self)
 
 
 class ProxyBlock(CfgNode):
     """A placeholder that serves as the endpoint (source or target) of a
     :class:`gtirb.Edge`.
 
     ProxyBlock objects allow the construction of CFG edges to or from
@@ -384,23 +366,23 @@
     def references(self):
         if self.module is None:
             return ()
         return (s for s in self.module.symbols if s.referent == self)
 
     @property
     def incoming_edges(self):
-        if self.module is None or self.module.ir is None:
+        if self.ir is None:
             return ()
-        return (e for e in self.module.ir.cfg if e.target == self)
+        return self.ir.cfg.in_edges(self)
 
     @property
     def outgoing_edges(self):
-        if self.module is None or self.module.ir is None:
+        if self.ir is None:
             return ()
-        return (e for e in self.module.ir.cfg if e.source == self)
+        return self.ir.cfg.out_edges(self)
 
     @property
     def ir(self):
         # type: () -> "IR"
         """Get the IR this node ultimately belongs to."""
         if self.module is None:
             return None
```

### Comparing `gtirb-1.9.0/gtirb/__init__.py` & `gtirb-1.9.1/gtirb/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __all__ = [
     "AuxData",
     "AuxDataContainer",
     "Block",
     "ByteBlock",
     "ByteInterval",
+    "CFG",
     "CfgNode",
     "CodeBlock",
     "DataBlock",
     "Edge",
     "IR",
     "Module",
     "Node",
@@ -21,15 +22,15 @@
     "SymAddrConst",
     "SymStackConst",
 ]
 
 from .auxdata import AuxData, AuxDataContainer
 from .block import Block, ByteBlock, CfgNode, CodeBlock, DataBlock, ProxyBlock
 from .byteinterval import ByteInterval
-from .cfg import Edge
+from .cfg import CFG, Edge
 from .ir import IR
 from .module import Module
 from .node import Node
 from .offset import Offset
 from .section import Section
 from .serialization import Serialization
 from .symbol import Symbol
```

### Comparing `gtirb-1.9.0/gtirb/symbol.py` & `gtirb-1.9.1/gtirb/symbol.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/Offset_pb2.py` & `gtirb-1.9.1/gtirb/proto/Offset_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/AuxData_pb2.py` & `gtirb-1.9.1/gtirb/proto/AuxData_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/SymbolicExpression_pb2.py` & `gtirb-1.9.1/gtirb/proto/SymbolicExpression_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/Symbol_pb2.py` & `gtirb-1.9.1/gtirb/proto/Symbol_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/ProxyBlock_pb2.py` & `gtirb-1.9.1/gtirb/proto/ProxyBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/IR_pb2.py` & `gtirb-1.9.1/gtirb/proto/IR_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/CFG_pb2.py` & `gtirb-1.9.1/gtirb/proto/CFG_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/Module_pb2.py` & `gtirb-1.9.1/gtirb/proto/Module_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/ByteInterval_pb2.py` & `gtirb-1.9.1/gtirb/proto/ByteInterval_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/Section_pb2.py` & `gtirb-1.9.1/gtirb/proto/Section_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/DataBlock_pb2.py` & `gtirb-1.9.1/gtirb/proto/DataBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/proto/CodeBlock_pb2.py` & `gtirb-1.9.1/gtirb/proto/CodeBlock_pb2.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/offset.py` & `gtirb-1.9.1/gtirb/offset.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/util.py` & `gtirb-1.9.1/gtirb/util.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/serialization.py` & `gtirb-1.9.1/gtirb/serialization.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/auxdata.py` & `gtirb-1.9.1/gtirb/auxdata.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/byteinterval.py` & `gtirb-1.9.1/gtirb/byteinterval.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/module.py` & `gtirb-1.9.1/gtirb/module.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/section.py` & `gtirb-1.9.1/gtirb/section.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/node.py` & `gtirb-1.9.1/gtirb/node.py`

 * *Files identical despite different names*

### Comparing `gtirb-1.9.0/gtirb/ir.py` & `gtirb-1.9.1/gtirb/ir.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import itertools
 import typing
 from uuid import UUID
 
 from .auxdata import AuxData, AuxDataContainer
 from .block import ByteBlock, CfgNode, CodeBlock, DataBlock, ProxyBlock
 from .byteinterval import ByteInterval, SymbolicExpressionElement
-from .cfg import Edge
+from .cfg import CFG, Edge
 from .module import Module
 from .node import Node
 from .proto import CFG_pb2, IR_pb2
 from .section import Section
 from .symbol import Symbol
 from .util import (
     DictLike,
@@ -32,16 +32,15 @@
 from .version import PROTOBUF_VERSION
 
 
 class IR(AuxDataContainer):
     """A complete internal representation consisting of multiple Modules.
 
     :ivar ~.modules: A list of :class:`Module`\\s contained in the IR.
-    :ivar ~.cfg: A set of :class:`Edge`\\s representing the IR's control
-        flow graph.
+    :ivar ~.cfg: The IR's control flow graph.
     :ivar ~.version: The Protobuf version of this IR.
     """
 
     class _ModuleList(ListWrapper[Module]):
         def __init__(self, node, *args):
             self._node = node  # type: IR
             super().__init__(*args)
@@ -94,15 +93,15 @@
 
         self._local_uuid_cache = dict()  # type: typing.Dict[UUID, Node]
         # Modules are decoded before the aux data, since the UUID decoder
         # checks Node's cache.
         self.modules = IR._ModuleList(
             self, modules
         )  # type: typing.List[Module]
-        self.cfg = set(cfg)  # type: typing.Set[Edge]
+        self.cfg = CFG(cfg)  # type: CFG
         self.version = version  # type: int
         super().__init__(aux_data, uuid)
         self._local_uuid_cache[self.uuid] = self
 
     @classmethod
     def _decode_protobuf(cls, proto_ir, uuid, _):
         # type: (IR_pb2.IR, UUID, typing.Optional["IR"]) -> IR
@@ -112,31 +111,29 @@
                 % (proto_ir.version, PROTOBUF_VERSION)
             )
 
         ir = cls(version=proto_ir.version, uuid=uuid)
         ir.modules.extend(
             Module._from_protobuf(m, ir) for m in proto_ir.modules
         )
-        ir.cfg.update(
-            Edge._from_protobuf(e, ir.get_by_uuid) for e in proto_ir.cfg.edges
-        )
+        ir.cfg = CFG._from_protobuf(proto_ir.cfg.edges, ir)
         ir.aux_data.update(
             AuxDataContainer._read_protobuf_aux_data(proto_ir, ir)
         )
         return ir
 
     def _to_protobuf(self):
         # type: () -> IR_pb2.IR
         proto_ir = IR_pb2.IR()
         proto_ir.uuid = self.uuid.bytes
         proto_ir.version = self.version
         proto_ir.modules.extend(m._to_protobuf() for m in self.modules)
         proto_cfg = CFG_pb2.CFG()
         proto_cfg.vertices.extend(v.uuid.bytes for v in self.cfg_nodes)
-        proto_cfg.edges.extend(e._to_protobuf() for e in self.cfg)
+        proto_cfg.edges.extend(self.cfg._to_protobuf())
         proto_ir.cfg.CopyFrom(proto_cfg)
         self._write_protobuf_aux_data(proto_ir)
         return proto_ir
 
     def deep_eq(self, other):
         # type: (typing.Any) -> bool
         # Do not move __eq__. See docstring for Node.deep_eq for more info.
@@ -145,26 +142,15 @@
         self_modules = sorted(self.modules, key=lambda m: m.uuid)
         other_modules = sorted(other.modules, key=lambda m: m.uuid)
         if not len(self_modules) == len(other_modules):
             return False
         for self_module, other_module in zip(self_modules, other_modules):
             if not self_module.deep_eq(other_module):
                 return False
-        self_edges = sorted(
-            self.cfg, key=lambda e: (e.source.uuid, e.target.uuid)
-        )
-        other_edges = sorted(
-            other.cfg, key=lambda e: (e.source.uuid, e.target.uuid)
-        )
-        if not len(self_edges) == len(other_edges):
-            return False
-        for self_edge, other_edge in zip(self_edges, other_edges):
-            if not self_edge.deep_eq(other_edge):
-                return False
-        return self.version == other.version
+        return self.version == other.version and self.cfg.deep_eq(other.cfg)
 
     @staticmethod
     def load_protobuf_file(protobuf_file):
         # type: (typing.BinaryIO) -> IR
         """Load IR from a Protobuf object.
 
         Use this function when you have a Protobuf object already loaded,
```

### Comparing `gtirb-1.9.0/PKG-INFO` & `gtirb-1.9.1/gtirb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gtirb
-Version: 1.9.0
+Version: 1.9.1
 Summary: GrammaTech Intermediate Representation for Binaries
 Home-page: https://github.com/grammatech/gtirb
 Author: GrammaTech
 Author-email: gtirb@grammatech.com
 License: MIT
 Description: # GTIRB
         
@@ -102,14 +102,22 @@
         instructions.  GTIRB is versioned with Major.Minor.Patch versioning
         where Major version increments will require significant source changes
         but should be very rare, Minor version increments may require small
         source changes, and Patch version increments shouldn't break any
         downstream builds.  We do not yet provide ABI compatibility across any
         version changes.
         
+        ## Python API
+        The GTIRB Python API may be installed with the following.  Note
+        however, that installation of the `ddisasm` and `gtirb-pprinter`
+        packages as described below is recommended for every API.
+        ```sh
+        pip install gtirb
+        ```
+        
         ## Windows
         Pre-built debug and release binaries are available for Windows at:
         [windows-debug/](https://grammatech.github.io/gtirb/pkgs/windows-debug/),
         and
         [windows-release/](https://grammatech.github.io/gtirb/pkgs/windows-release/).
         A symbol server for the debugging symbols for both the release and
         debug binaries is available at
```

