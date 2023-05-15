# Comparing `tmp/ket-lang-0.6.0.dev1.tar.gz` & `tmp/ket-lang-0.6rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ket-lang-0.6.0.dev1.tar", last modified: Fri May 12 19:47:45 2023, max compression
+gzip compressed data, was "ket-lang-0.6rc2.tar", last modified: Mon May 15 18:50:19 2023, max compression
```

## Comparing `ket-lang-0.6.0.dev1.tar` & `ket-lang-0.6rc2.tar`

### file list

```diff
@@ -1,90 +1,92 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/
--rw-rw-rw-   0 root         (0) root         (0)    11455 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7173 2023-05-12 19:47:45.417518 ket-lang-0.6.0.dev1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6412 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/README.md
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-12 19:47:45.417518 ket-lang-0.6.0.dev1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.388515 ket-lang-0.6.0.dev1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.394515 ket-lang-0.6.0.dev1/src/ket/
--rw-rw-rw-   0 root         (0) root         (0)     1313 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1642 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    29132 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.395516 ket-lang-0.6.0.dev1/src/ket/clib/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3937 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     9012 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/libket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.396516 ket-lang-0.6.0.dev1/src/ket/clib/libs/
--rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.398516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/
--rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      565 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      761 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/README.md
--rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/kbw.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.401516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/
--rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/bitwise.rs
--rw-rw-rw-   0 root         (0) root         (0)     4404 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/c_wrapper.rs
--rw-rw-rw-   0 root         (0) root         (0)     1942 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/convert.rs
--rw-rw-rw-   0 root         (0) root         (0)    20501 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/dense.rs
--rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)      311 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     9825 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs
--rw-rw-rw-   0 root         (0) root         (0)    20230 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/sparse.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.402516 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/shor.rs
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.405516 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/.git
--rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      420 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/CHANGELOG.md
--rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/Cargo.toml
--rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/README.md
--rw-rw-rw-   0 root         (0) root         (0)     8457 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.h
--rw-rw-rw-   0 root         (0) root         (0)    10442 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.hpp
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.409517 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.410517 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/error.rs
--rw-rw-rw-   0 root         (0) root         (0)       49 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/mod.rs
--rw-rw-rw-   0 root         (0) root         (0)     6838 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/objects.rs
--rw-rw-rw-   0 root         (0) root         (0)    11058 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/c_wrapper/process.rs
--rw-rw-rw-   0 root         (0) root         (0)     6119 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/code_block.rs
--rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/decompose.rs
--rw-rw-rw-   0 root         (0) root         (0)     4605 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/error.rs
--rw-rw-rw-   0 root         (0) root         (0)     6275 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/gates.rs
--rw-rw-rw-   0 root         (0) root         (0)     4853 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/instruction.rs
--rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/ir.rs
--rw-rw-rw-   0 root         (0) root         (0)      255 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/lib.rs
--rw-rw-rw-   0 root         (0) root         (0)     4147 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/object.rs
--rw-rw-rw-   0 root         (0) root         (0)    21092 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/process.rs
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-12 19:47:33.000000 ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/serialize.rs
--rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/clib/wrapper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.411517 ket-lang-0.6.0.dev1/src/ket/gates/
--rw-rw-rw-   0 root         (0) root         (0)     8530 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/base_gates.py
--rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/gates/quantum_gate.py
--rw-rw-rw-   0 root         (0) root         (0)     3913 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/import_ket.py
--rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/kbw.py
--rw-rw-rw-   0 root         (0) root         (0)     5795 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/lib.py
--rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.413517 ket-lang-0.6.0.dev1/src/ket/preprocessor/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/statements.py
--rw-rw-rw-   0 root         (0) root         (0)     8995 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/preprocessor/transformer.py
--rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/process.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.414517 ket-lang-0.6.0.dev1/src/ket/standard/
--rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4593 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/adj.py
--rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/src/ket/standard/ctrl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7173 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2257 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-12 19:47:45.000000 ket-lang-0.6.0.dev1/src/ket_lang.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 19:47:45.416518 ket-lang-0.6.0.dev1/tests/
--rw-rw-rw-   0 root         (0) root         (0)     4698 2023-05-12 19:47:32.000000 ket-lang-0.6.0.dev1/tests/test_gates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/
+-rw-rw-rw-   0 root         (0) root         (0)    11455 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       53 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6527 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-05-15 18:50:19.770542 ket-lang-0.6rc2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.741540 ket-lang-0.6rc2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.747541 ket-lang-0.6rc2/src/ket/
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1642 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    29132 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.748541 ket-lang-0.6rc2/src/ket/clib/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3937 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     9012 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/libket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.748541 ket-lang-0.6rc2/src/ket/clib/libs/
+-rw-rw-rw-   0 root         (0) root         (0)     1707 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.751541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/
+-rw-rw-rw-   0 root         (0) root         (0)       58 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      638 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      716 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      901 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      929 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/kbw.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.754541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/
+-rw-rw-rw-   0 root         (0) root         (0)     1255 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/bitwise.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4404 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/c_api.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/convert.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20501 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/dense.rs
+-rw-rw-rw-   0 root         (0) root         (0)     2247 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)      307 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     9825 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/quantum_execution.rs
+-rw-rw-rw-   0 root         (0) root         (0)    20230 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/sparse.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.754541 ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1075 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/shor.rs
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.757541 ket-lang-0.6rc2/src/ket/clib/libs/libket/
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.git
+-rw-rw-rw-   0 root         (0) root         (0)       20 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.758541 ket-lang-0.6rc2/src/ket/clib/libs/libket/.vscode/
+-rw-rw-rw-   0 root         (0) root         (0)       70 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/.vscode/settings.json
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/CHANGELOG.md
+-rw-rw-rw-   0 root         (0) root         (0)      685 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/Cargo.toml
+-rw-rw-rw-   0 root         (0) root         (0)    11460 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      746 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     8457 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.h
+-rw-rw-rw-   0 root         (0) root         (0)    10442 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.hpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.762542 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.763542 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/
+-rw-rw-rw-   0 root         (0) root         (0)     1569 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     1061 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/mod.rs
+-rw-rw-rw-   0 root         (0) root         (0)    14867 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/objects.rs
+-rw-rw-rw-   0 root         (0) root         (0)    27318 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/c_api/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6119 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/code_block.rs
+-rw-rw-rw-   0 root         (0) root         (0)     8846 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/decompose.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4605 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/error.rs
+-rw-rw-rw-   0 root         (0) root         (0)     6275 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/gates.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4853 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/instruction.rs
+-rw-rw-rw-   0 root         (0) root         (0)      867 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/ir.rs
+-rw-rw-rw-   0 root         (0) root         (0)      251 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/lib.rs
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/object.rs
+-rw-rw-rw-   0 root         (0) root         (0)    21092 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/process.rs
+-rw-rw-rw-   0 root         (0) root         (0)      540 2023-05-15 18:50:08.000000 ket-lang-0.6rc2/src/ket/clib/libs/libket/src/serialize.rs
+-rw-rw-rw-   0 root         (0) root         (0)     3101 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/clib/wrapper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.764542 ket-lang-0.6rc2/src/ket/gates/
+-rw-rw-rw-   0 root         (0) root         (0)     8530 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1955 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/base_gates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4245 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/gates/quantum_gate.py
+-rw-rw-rw-   0 root         (0) root         (0)     3913 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/import_ket.py
+-rw-rw-rw-   0 root         (0) root         (0)     1359 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/kbw.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1446 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.765542 ket-lang-0.6rc2/src/ket/preprocessor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2222 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/statements.py
+-rw-rw-rw-   0 root         (0) root         (0)     8995 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/preprocessor/transformer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3751 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/process.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.766542 ket-lang-0.6rc2/src/ket/standard/
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4593 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/adj.py
+-rw-rw-rw-   0 root         (0) root         (0)     7792 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/src/ket/standard/ctrl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/src/ket_lang.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7284 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2284 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        4 2023-05-15 18:50:19.000000 ket-lang-0.6rc2/src/ket_lang.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 18:50:19.769542 ket-lang-0.6rc2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     4698 2023-05-15 18:50:07.000000 ket-lang-0.6rc2/tests/test_gates.py
```

### Comparing `ket-lang-0.6.0.dev1/LICENSE` & `ket-lang-0.6rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/PKG-INFO` & `ket-lang-0.6rc2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,57 +1,35 @@
-Metadata-Version: 2.1
-Name: ket-lang
-Version: 0.6.0.dev1
-Summary: Ket quantum programming language interpreter and library
-Home-page: https://quantumket.org
-Author: Evandro Chagas Ribeiro da Rosa
-Author-email: evandro@quantuloop.com
-License: Apache-2.0
-Project-URL: Source, https://gitlab.com/quantum-ket/ket
-Keywords: quantum computer,quantum programming,quantum simulator
-Platform: linux
-Platform: win32
-Platform: osx
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Rust
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-
 [![PyPI](https://img.shields.io/pypi/v/ket-lang.svg)](https://pypi.org/project/ket-lang/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 
 # Ket Quantum Programming
 
 [[_TOC_]]
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
 Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-## Installation :arrow_down
+## Installation :arrow_down:
 
-Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
+Ket requires Python 3.8 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll
+## Documentation :scroll:
 
 Documentation available at <https://quantumket.org>.
 
-## Examples :bulb
+## Examples :bulb:
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -72,20 +50,32 @@
 # 13
 ```
 
 ### Shor's Algorithm
 
 ```py
 from ket import *
-from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
 from math import log2, gcd
 
+def qft(qubits: quant, invert: bool = True):
+    if len(qubits) == 1:
+        H(qubits)
+    else:
+        head, *tail = qubits
+        H(head)
+        for i, c in enumerate(reversed(tail)):
+            ctrl(c, phase(pi / 2**(i + 1)), head)
+        qft(tail, invert=False)
+
+    if invert:
+        for i in range(len(qubits) // 2):
+            swap(qubits[i], qubits[- i - 1])
 
 def quantum_subroutine(N, x):
     n = N.bit_length()
 
     def subroutine():
         reg1 = H(quant(n))
         reg2 = pown(x, reg1, N)
@@ -198,37 +188,34 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer
+## Ket Development :hammer:
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
-If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
-
-## Roadmap :notebook_with_decorative_cover
+## Roadmap :notebook_with_decorative_cover:
 
-* [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
-* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
+* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks.
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book
+## Cite Ket :book:
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -247,10 +234,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family
+## Community :family:
 
 Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.6.0.dev1/README.md` & `ket-lang-0.6rc2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,57 @@
+Metadata-Version: 2.1
+Name: ket-lang
+Version: 0.6rc2
+Summary: Ket quantum programming language interpreter and library
+Home-page: https://quantumket.org
+Author: Evandro Chagas Ribeiro da Rosa
+Author-email: evandro@quantuloop.com
+License: Apache-2.0
+Project-URL: Source, https://gitlab.com/quantum-ket/ket
+Keywords: quantum computer,quantum programming,quantum simulator
+Platform: linux
+Platform: win32
+Platform: osx
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Rust
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+
 [![PyPI](https://img.shields.io/pypi/v/ket-lang.svg)](https://pypi.org/project/ket-lang/)
 [![Contributor Covenant](https://img.shields.io/badge/Contributor%20Covenant-2.1-4baaaa.svg)](CODE_OF_CONDUCT.md)
 
 # Ket Quantum Programming
 
 [[_TOC_]]
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
 Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-## Installation :arrow_down
+## Installation :arrow_down:
 
-Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
+Ket requires Python 3.8 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll
+## Documentation :scroll:
 
 Documentation available at <https://quantumket.org>.
 
-## Examples :bulb
+## Examples :bulb:
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -50,20 +72,32 @@
 # 13
 ```
 
 ### Shor's Algorithm
 
 ```py
 from ket import *
-from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
 from math import log2, gcd
 
+def qft(qubits: quant, invert: bool = True):
+    if len(qubits) == 1:
+        H(qubits)
+    else:
+        head, *tail = qubits
+        H(head)
+        for i, c in enumerate(reversed(tail)):
+            ctrl(c, phase(pi / 2**(i + 1)), head)
+        qft(tail, invert=False)
+
+    if invert:
+        for i in range(len(qubits) // 2):
+            swap(qubits[i], qubits[- i - 1])
 
 def quantum_subroutine(N, x):
     n = N.bit_length()
 
     def subroutine():
         reg1 = H(quant(n))
         reg2 = pown(x, reg1, N)
@@ -176,37 +210,34 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer
+## Ket Development :hammer:
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
-If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
-
-## Roadmap :notebook_with_decorative_cover
+## Roadmap :notebook_with_decorative_cover:
 
-* [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
-* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
+* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks.
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book
+## Cite Ket :book:
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -225,10 +256,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family
+## Community :family:
 
 Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.6.0.dev1/setup.cfg` & `ket-lang-0.6rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/__init__.py` & `ket-lang-0.6rc2/src/ket/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .process import *
 from .gates import __all__ as all_gate
 from .import_ket import __all__ as all_import
 from .base import __all__ as all_base
 from .standard import __all__ as all_standard
 from .process import __all__ as all_process
 
-__version__ = '0.6.0dev1'
+__version__ = '0.6rc2'
 __all__ = all_gate + all_import + all_base + all_standard + all_process
 
 from .import_ket import code_ket
 
 from .base import QUANTUM_EXECUTION_TARGET
 if QUANTUM_EXECUTION_TARGET is None:
     from .kbw import use_sparse
```

### Comparing `ket-lang-0.6.0.dev1/src/ket/__main__.py` & `ket-lang-0.6rc2/src/ket/__main__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/base.py` & `ket-lang-0.6rc2/src/ket/base.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/kbw.py` & `ket-lang-0.6rc2/src/ket/clib/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libket.py` & `ket-lang-0.6rc2/src/ket/clib/libket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/__init__.py` & `ket-lang-0.6rc2/src/ket/clib/libs/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/Cargo.toml` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/Cargo.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 readme = "README.md"
 edition = "2021"
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-libket = { git = "https://gitlab.com/quantum-ket/libket.git"}
+libket = "0.3.0"
 serde = { version = "1.0", features = ["derive"] }
 serde_json = "1.0"
 bincode = "1.3"
 num = "0.4"
 rand = "0.8.5"
 rayon = "1.5.3"
 twox-hash = "1.6.3"
```

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/LICENSE` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/README.md` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/kbw.h` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/kbw.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/bitwise.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/bitwise.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/c_wrapper.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/c_api.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/convert.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/convert.rs`

 * *Files 8% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         ket::DumpData::Probability {
             basis_states,
             probabilities,
         } => {
             let mut count_map = HashMap::new();
             let dist = WeightedIndex::new(probabilities).unwrap();
 
-            (0..shots).into_iter().for_each(|_| {
+            (0..shots).for_each(|_| {
                 count_map
                     .entry(&basis_states[dist.sample(rng)])
                     .and_modify(|c| *c += 1)
                     .or_insert(1u32);
             });
 
             let mut basis_states = Vec::new();
```

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/dense.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/dense.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/error.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/quantum_execution.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/quantum_execution.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/src/sparse.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/src/sparse.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/kbw/tests/shor.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/kbw/tests/shor.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/Cargo.toml` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/Cargo.toml`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/LICENSE` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/LICENSE`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/README.md` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/README.md`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.h` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.h`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/libket.hpp` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/libket.hpp`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/code_block.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/code_block.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/decompose.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/decompose.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/error.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/error.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/gates.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/gates.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/instruction.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/instruction.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/ir.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/ir.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/object.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/object.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/process.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/process.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/libs/libket/src/serialize.rs` & `ket-lang-0.6rc2/src/ket/clib/libs/libket/src/serialize.rs`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/clib/wrapper.py` & `ket-lang-0.6rc2/src/ket/clib/wrapper.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/gates/__init__.py` & `ket-lang-0.6rc2/src/ket/gates/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/gates/base_gates.py` & `ket-lang-0.6rc2/src/ket/gates/base_gates.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/gates/quantum_gate.py` & `ket-lang-0.6rc2/src/ket/gates/quantum_gate.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/import_ket.py` & `ket-lang-0.6rc2/src/ket/import_ket.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/kbw.py` & `ket-lang-0.6rc2/src/ket/kbw.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/lib.py` & `ket-lang-0.6rc2/src/ket/lib.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,58 +10,24 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from math import pi, sqrt, asin
+from math import sqrt, asin
 from typing import Callable
 
 from .base import quant, dump, future
-from .gates import H, phase, swap, cnot, X, Y, Z, S, RY
+from .gates import H, cnot, X, Y, Z, S, RY
 from .standard import control, ctrl
 from .process import run, exec_quantum
 from .preprocessor.statements import _ket_if, _ket_next
 
 
-def qft(qubits: quant, invert: bool = True) -> quant:
-    """Quantum Fourier Transformation
-
-    Apply a QFT_ on the qubits of q.
-
-    .. _QFT: https://en.wikipedia.org/wiki/Quantum_Fourier_transform
-
-    Args:
-        q: input qubits
-        invert: if ``True``, invert qubits with swap gates
-
-    return:
-        Qubits in the reserved order
-    """
-
-    if len(qubits) == 1:
-        H(qubits)
-    else:
-        *head, tail = qubits
-        H(tail)
-        for i, ctrl_qubit in enumerate(reversed(head)):
-            with control(ctrl_qubit):
-                phase(pi / 2**(i + 1), tail)
-        qft(head, invert=False)
-
-    if invert:
-        size = len(qubits)
-        for i in range(size // 2):
-            swap(qubits[i], qubits[size - i - 1])
-        return qubits
-
-    return reversed(qubits)
-
-
 def dump_matrix(gate: Callable | list[Callable], size: int = 1) -> list[list[complex]]:
     """Get the matrix of a quantum operation
 
     Args:
         u: Quantum operation.
         size: Number of qubits.
     """
```

### Comparing `ket-lang-0.6.0.dev1/src/ket/plugins.py` & `ket-lang-0.6rc2/src/ket/plugins.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/preprocessor/statements.py` & `ket-lang-0.6rc2/src/ket/preprocessor/statements.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/preprocessor/transformer.py` & `ket-lang-0.6rc2/src/ket/preprocessor/transformer.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/process.py` & `ket-lang-0.6rc2/src/ket/process.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/standard/__init__.py` & `ket-lang-0.6rc2/src/ket/standard/__init__.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/standard/adj.py` & `ket-lang-0.6rc2/src/ket/standard/adj.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket/standard/ctrl.py` & `ket-lang-0.6rc2/src/ket/standard/ctrl.py`

 * *Files identical despite different names*

### Comparing `ket-lang-0.6.0.dev1/src/ket_lang.egg-info/PKG-INFO` & `ket-lang-0.6rc2/src/ket_lang.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ket-lang
-Version: 0.6.0.dev1
+Version: 0.6rc2
 Summary: Ket quantum programming language interpreter and library
 Home-page: https://quantumket.org
 Author: Evandro Chagas Ribeiro da Rosa
 Author-email: evandro@quantuloop.com
 License: Apache-2.0
 Project-URL: Source, https://gitlab.com/quantum-ket/ket
 Keywords: quantum computer,quantum programming,quantum simulator
@@ -29,29 +29,29 @@
 
 Ket is an embedded programming language that introduces the ease of Python to quantum programming, letting anyone quickly prototype and test a quantum application.
 
 Python is the most widely used programming language for machine learning and data science and has been the language of choice for quantum programming. Ket is a Python-embedded language, but many can use it as a Python library in most cases. So you can use Ket together with NumPy, ScyPy, Pandas, and other popular Python libraries.
 
 Ket's goal is to streamline the development of hardware-independent classical quantum applications by providing transparent interaction of classical and quantum data. See <https://quantumket.org> to learn more about Ket.
 
-## Installation :arrow_down
+## Installation :arrow_down:
 
-Ket requires Python 3.7 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
+Ket requires Python 3.8 or newer and is available for Linux, Windows, and macOS. If you are not using x86_64 (example ARM), you must install [Rust](https://www.rust-lang.org/tools/install) before installing Ket.
 
 You can install Ket using [`pip`](https://pip.pypa.io/en/stable/user_guide/). To do so, copy and paste the following command into your terminal:
 
 ```shell
 pip install ket-lang
 ```
 
-## Documentation :scroll
+## Documentation :scroll:
 
 Documentation available at <https://quantumket.org>.
 
-## Examples :bulb
+## Examples :bulb:
 
 ### Grover's Algorithm
 
 ```py
 from ket import *
 from math import sqrt, pi
 
@@ -72,20 +72,32 @@
 # 13
 ```
 
 ### Shor's Algorithm
 
 ```py
 from ket import *
-from ket.lib import qft
 from ket.plugins import pown
 from random import randint
 from functools import reduce
 from math import log2, gcd
 
+def qft(qubits: quant, invert: bool = True):
+    if len(qubits) == 1:
+        H(qubits)
+    else:
+        head, *tail = qubits
+        H(head)
+        for i, c in enumerate(reversed(tail)):
+            ctrl(c, phase(pi / 2**(i + 1)), head)
+        qft(tail, invert=False)
+
+    if invert:
+        for i in range(len(qubits) // 2):
+            swap(qubits[i], qubits[- i - 1])
 
 def quantum_subroutine(N, x):
     n = N.bit_length()
 
     def subroutine():
         reg1 = H(quant(n))
         reg2 = pown(x, reg1, N)
@@ -198,37 +210,34 @@
 # Bob Qubit:
 # |0⟩     (50.00%)
 #  0.707107               ≅      1/√2
 # |1⟩     (50.00%)
 #  0.500000+0.500000i     ≅  (1+i)/√4
 ```
 
-## Ket Development :hammer
+## Ket Development :hammer:
 
 Setup for Ket development:
 
 ```shell
 git clone https://gitlab.com/quantum-ket/ket.git
 cd ket
 pip install -e . --user
 ```
 
-If you are using [VS Code](https://code.visualstudio.com/), Ket has a [Dev Container](https://code.visualstudio.com/docs/remote/containers) :whale:.
-
-## Roadmap :notebook_with_decorative_cover
+## Roadmap :notebook_with_decorative_cover:
 
-* [ ] Quantum gate decomposition.
 * [ ] Quantum code optimization.
 * [ ] Quantum circuit visualization.
   
-* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks like the [`qft`](https://quantumket.org/ket#ket.lib.qft).  
+* :zap: We plan to expand the [quantum library](https://quantumket.org/ket#quantum-library) with quantum algorithm building blocks.
 * :package: Full quantum algorithm implementations must be packaged with  Ket as a dependency.
 * :x: Low-level quantum control, like pulse programming, is out of Ket's scope.
 
-## Cite Ket :book
+## Cite Ket :book:
 
 When using Ket for research projects, please cite:
 
 > Evandro Chagas Ribeiro da Rosa and Rafael de Santiago. 2021. Ket Quantum Programming. J. Emerg. Technol. Comput. Syst. 18, 1, Article 12 (January 2022), 25 pages. DOI: [10.1145/3474224](https://doi.org/10.1145/3474224)
 
 ```bibtex
 @article{ket,
@@ -247,10 +256,10 @@
    month = oct,
    articleno = {12},
    numpages = {25},
    keywords = {Quantum programming, cloud quantum computation, qubit simulation}
 }
 ```
 
-## Community :family
+## Community :family:
 
 Join the conversation on our [Discord](https://discord.gg/XkXvwRQ9aa).
```

### Comparing `ket-lang-0.6.0.dev1/src/ket_lang.egg-info/SOURCES.txt` & `ket-lang-0.6rc2/src/ket_lang.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 src/ket/clib/libs/kbw/.gitignore
 src/ket/clib/libs/kbw/CHANGELOG.md
 src/ket/clib/libs/kbw/Cargo.toml
 src/ket/clib/libs/kbw/LICENSE
 src/ket/clib/libs/kbw/README.md
 src/ket/clib/libs/kbw/kbw.h
 src/ket/clib/libs/kbw/src/bitwise.rs
-src/ket/clib/libs/kbw/src/c_wrapper.rs
+src/ket/clib/libs/kbw/src/c_api.rs
 src/ket/clib/libs/kbw/src/convert.rs
 src/ket/clib/libs/kbw/src/dense.rs
 src/ket/clib/libs/kbw/src/error.rs
 src/ket/clib/libs/kbw/src/lib.rs
 src/ket/clib/libs/kbw/src/quantum_execution.rs
 src/ket/clib/libs/kbw/src/sparse.rs
 src/ket/clib/libs/kbw/tests/shor.rs
@@ -37,28 +37,29 @@
 src/ket/clib/libs/libket/.gitignore
 src/ket/clib/libs/libket/CHANGELOG.md
 src/ket/clib/libs/libket/Cargo.toml
 src/ket/clib/libs/libket/LICENSE
 src/ket/clib/libs/libket/README.md
 src/ket/clib/libs/libket/libket.h
 src/ket/clib/libs/libket/libket.hpp
+src/ket/clib/libs/libket/.vscode/settings.json
 src/ket/clib/libs/libket/src/code_block.rs
 src/ket/clib/libs/libket/src/decompose.rs
 src/ket/clib/libs/libket/src/error.rs
 src/ket/clib/libs/libket/src/gates.rs
 src/ket/clib/libs/libket/src/instruction.rs
 src/ket/clib/libs/libket/src/ir.rs
 src/ket/clib/libs/libket/src/lib.rs
 src/ket/clib/libs/libket/src/object.rs
 src/ket/clib/libs/libket/src/process.rs
 src/ket/clib/libs/libket/src/serialize.rs
-src/ket/clib/libs/libket/src/c_wrapper/error.rs
-src/ket/clib/libs/libket/src/c_wrapper/mod.rs
-src/ket/clib/libs/libket/src/c_wrapper/objects.rs
-src/ket/clib/libs/libket/src/c_wrapper/process.rs
+src/ket/clib/libs/libket/src/c_api/error.rs
+src/ket/clib/libs/libket/src/c_api/mod.rs
+src/ket/clib/libs/libket/src/c_api/objects.rs
+src/ket/clib/libs/libket/src/c_api/process.rs
 src/ket/gates/__init__.py
 src/ket/gates/base_gates.py
 src/ket/gates/quantum_gate.py
 src/ket/preprocessor/__init__.py
 src/ket/preprocessor/statements.py
 src/ket/preprocessor/transformer.py
 src/ket/standard/__init__.py
```

### Comparing `ket-lang-0.6.0.dev1/tests/test_gates.py` & `ket-lang-0.6rc2/tests/test_gates.py`

 * *Files identical despite different names*

