# Comparing `tmp/hyphy-python-0.1.8.tar.gz` & `tmp/hyphy-python-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hyphy-python-0.1.8.tar", last modified: Mon Dec 11 15:19:19 2017, max compression
+gzip compressed data, was "dist/hyphy-python-0.1.9.tar", last modified: Fri Feb 16 16:27:39 2018, max compression
```

## Comparing `hyphy-python-0.1.8.tar` & `hyphy-python-0.1.9.tar`

### file list

```diff
@@ -1,1721 +1,1721 @@
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/HyPhy/
--rw-r--r--   0 sweaver    (501) staff       (20)     2170 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/HyPhy/__init__.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/
--rw-r--r--   0 sweaver    (501) staff       (20)      415 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/.gitignore
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/cmake/
--rw-r--r--   0 sweaver    (501) staff       (20)     1070 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/cmake/cmake_uninstall.cmake.in
--rw-r--r--   0 sweaver    (501) staff       (20)     2829 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/cmake/FindOpenCL.cmake
--rw-r--r--   0 sweaver    (501) staff       (20)    23928 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/CMakeLists.txt
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/CMakeWin32/
--rw-r--r--   0 sweaver    (501) staff       (20)     3499 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/CMakeWin32/CMakeLists.txt
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/
--rw-r--r--   0 sweaver    (501) staff       (20)     3851 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/cl2hdr.c
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/
--rw-r--r--   0 sweaver    (501) staff       (20)    43769 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/aclocal.m4
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/
--rwxr-xr-x   0 sweaver    (501) staff       (20)    44826 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.guess
--rw-r--r--   0 sweaver    (501) staff       (20)     1841 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.h.in
--rwxr-xr-x   0 sweaver    (501) staff       (20)    35454 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.sub
--rwxr-xr-x   0 sweaver    (501) staff       (20)    20334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/depcomp
--rwxr-xr-x   0 sweaver    (501) staff       (20)    13998 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/install-sh
--rw-r--r--   0 sweaver    (501) staff       (20)   283680 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/ltmain.sh
--rwxr-xr-x   0 sweaver    (501) staff       (20)    10346 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/missing
--rw-r--r--   0 sweaver    (501) staff       (20)     6645 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CHANGES
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/cmake/
--rw-r--r--   0 sweaver    (501) staff       (20)     9548 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/cmake/internal_utils.cmake
--rw-r--r--   0 sweaver    (501) staff       (20)     9120 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CMakeLists.txt
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/
--rw-r--r--   0 sweaver    (501) staff       (20)    10486 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.cbproj
--rw-r--r--   0 sweaver    (501) staff       (20)     2008 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.groupproj
--rw-r--r--   0 sweaver    (501) staff       (20)     1865 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_all.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     1993 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_link.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     8580 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_main.cbproj
--rw-r--r--   0 sweaver    (501) staff       (20)     8691 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_unittest.cbproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)   564464 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/configure
--rw-r--r--   0 sweaver    (501) staff       (20)     2574 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/configure.ac
--rw-r--r--   0 sweaver    (501) staff       (20)     1358 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CONTRIBUTORS
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/
--rw-r--r--   0 sweaver    (501) staff       (20)   354360 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest-all.cc
--rw-r--r--   0 sweaver    (501) staff       (20)   830563 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1765 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest_main.cc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/
--rw-r--r--   0 sweaver    (501) staff       (20)    11523 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-death-test.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-message.h
--rw-r--r--   0 sweaver    (501) staff       (20)    75864 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h
--rw-r--r--   0 sweaver    (501) staff       (20)    18796 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h.pump
--rw-r--r--   0 sweaver    (501) staff       (20)    31609 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-printers.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9952 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-spi.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6509 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-test-part.h
--rw-r--r--   0 sweaver    (501) staff       (20)    10242 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-typed-test.h
--rw-r--r--   0 sweaver    (501) staff       (20)    88434 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest.h
--rw-r--r--   0 sweaver    (501) staff       (20)    15145 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_pred_impl.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2324 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_prod.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/
--rw-r--r--   0 sweaver    (501) staff       (20)    13429 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-death-test-internal.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9603 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-filepath.h
--rw-r--r--   0 sweaver    (501) staff       (20)    44145 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-internal.h
--rw-r--r--   0 sweaver    (501) staff       (20)     8101 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-linked_ptr.h
--rw-r--r--   0 sweaver    (501) staff       (20)   192176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9416 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h.pump
--rw-r--r--   0 sweaver    (501) staff       (20)    24191 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util.h
--rw-r--r--   0 sweaver    (501) staff       (20)    68796 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-port.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6968 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-string.h
--rw-r--r--   0 sweaver    (501) staff       (20)    28223 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9226 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h.pump
--rw-r--r--   0 sweaver    (501) staff       (20)   185666 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9317 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h.pump
--rw-r--r--   0 sweaver    (501) staff       (20)     1475 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/LICENSE
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/
--rw-r--r--   0 sweaver    (501) staff       (20)    13302 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/acx_pthread.m4
--rw-r--r--   0 sweaver    (501) staff       (20)     3217 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/gtest.m4
--rw-r--r--   0 sweaver    (501) staff       (20)   287004 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/libtool.m4
--rw-r--r--   0 sweaver    (501) staff       (20)    12347 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltoptions.m4
--rw-r--r--   0 sweaver    (501) staff       (20)     4372 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltsugar.m4
--rw-r--r--   0 sweaver    (501) staff       (20)      690 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltversion.m4
--rw-r--r--   0 sweaver    (501) staff       (20)     6126 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/lt~obsolete.m4
--rw-r--r--   0 sweaver    (501) staff       (20)     9739 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/Makefile.am
--rw-r--r--   0 sweaver    (501) staff       (20)    59044 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/Makefile.in
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/
--rwxr-xr-x   0 sweaver    (501) staff       (20)     2456 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.sln
--rwxr-xr-x   0 sweaver    (501) staff       (20)     3374 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     2432 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.sln
--rwxr-xr-x   0 sweaver    (501) staff       (20)     3371 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     3514 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main-md.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     3508 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4515 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test-md.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4509 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest-md.vcproj
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4003 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest.vcproj
--rw-r--r--   0 sweaver    (501) staff       (20)    16090 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/README
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/
--rw-r--r--   0 sweaver    (501) staff       (20)     4072 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/prime_tables.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2502 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     1937 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5053 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample10_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     5129 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2298 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     3006 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3926 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     5365 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample3-inl.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5351 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample3_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     1927 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2083 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1909 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     6590 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample5_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     8989 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample6_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     5099 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample7_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     6944 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample8_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     5951 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample9_unittest.cc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/
--rwxr-xr-x   0 sweaver    (501) staff       (20)     8813 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/fuse_gtest_files.py
--rwxr-xr-x   0 sweaver    (501) staff       (20)    21986 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/gen_gtest_pred_impl.py
--rwxr-xr-x   0 sweaver    (501) staff       (20)    10087 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/gtest-config.in
--rwxr-xr-x   0 sweaver    (501) staff       (20)    23673 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/pump.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/
--rw-r--r--   0 sweaver    (501) staff       (20)     2161 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-all.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    50949 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-death-test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    14238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-filepath.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    46465 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-internal-inl.h
--rw-r--r--   0 sweaver    (501) staff       (20)    27466 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-port.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    12275 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-printers.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     4159 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-test-part.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     3762 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-typed-test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)   184142 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     1765 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest_main.cc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/
--rw-r--r--   0 sweaver    (501) staff       (20)     3679 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_ex_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    43236 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    23653 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-filepath_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     4125 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-linked_ptr_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     9783 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-listener_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     5302 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-message_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     7938 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-options_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2884 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test2_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    33346 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2343 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.h
--rw-r--r--   0 sweaver    (501) staff       (20)    39094 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-port_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    49588 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-printers_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     7282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-test-part_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     9250 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-tuple_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2059 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test2_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    11369 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2485 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.h
--rw-r--r--   0 sweaver    (501) staff       (20)    13207 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-unittest-api_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2251 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_all_test.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     7339 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3263 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     9901 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     8919 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4911 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     2888 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     3487 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3576 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     6606 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_environment_test.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)    21261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3564 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     5856 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     2131 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     6515 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest.py
--rw-r--r--   0 sweaver    (501) staff       (20)     4710 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     1888 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_main_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_no_test_unittest.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)    12005 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)    32438 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)    28164 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_golden_lin.txt
--rw-r--r--   0 sweaver    (501) staff       (20)    77378 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_pred_impl_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     4772 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_premature_exit_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2209 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_prod_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     8193 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_repeat_test.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)    12549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3306 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2221 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_sole_header_test.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     9641 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_stress_test.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)    10812 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_test_utils.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3444 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_ex_test.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     5766 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     3104 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     2480 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test.py
--rw-r--r--   0 sweaver    (501) staff       (20)     1921 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)   239177 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_unittest.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile1_test_.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile2_test_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     5340 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfiles_test.py
--rwxr-xr-x   0 sweaver    (501) staff       (20)    14580 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest.py
--rw-r--r--   0 sweaver    (501) staff       (20)     6143 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest_.cc
--rwxr-xr-x   0 sweaver    (501) staff       (20)     8876 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_test_utils.py
--rw-r--r--   0 sweaver    (501) staff       (20)     1732 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/production.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2172 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/production.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/
--rw-r--r--   0 sweaver    (501) staff       (20)      983 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/DebugProject.xcconfig
--rw-r--r--   0 sweaver    (501) staff       (20)      551 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/FrameworkTarget.xcconfig
--rw-r--r--   0 sweaver    (501) staff       (20)     1199 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/General.xcconfig
--rw-r--r--   0 sweaver    (501) staff       (20)      993 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/ReleaseProject.xcconfig
--rw-r--r--   0 sweaver    (501) staff       (20)      587 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/StaticLibraryTarget.xcconfig
--rw-r--r--   0 sweaver    (501) staff       (20)      238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/TestTarget.xcconfig
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/
--rw-r--r--   0 sweaver    (501) staff       (20)    50972 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/project.pbxproj
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/
--rw-r--r--   0 sweaver    (501) staff       (20)     1010 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/Info.plist
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/
--rw-r--r--   0 sweaver    (501) staff       (20)      846 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/Info.plist
--rw-r--r--   0 sweaver    (501) staff       (20)     2354 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/runtests.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     2307 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.cc
--rw-r--r--   0 sweaver    (501) staff       (20)     2270 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2669 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget_test.cc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/
--rw-r--r--   0 sweaver    (501) staff       (20)    16060 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/
--rw-r--r--   0 sweaver    (501) staff       (20)     2587 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/runtests.sh
--rwxr-xr-x   0 sweaver    (501) staff       (20)     4536 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/versiongenerate.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/
--rw-r--r--   0 sweaver    (501) staff       (20)   111311 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/shell.c
--rw-r--r--   0 sweaver    (501) staff       (20)  5143688 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c
--rw-r--r--   0 sweaver    (501) staff       (20)   353468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3.h
--rw-r--r--   0 sweaver    (501) staff       (20)    26110 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3ext.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/BatchLanguage/
--rw-r--r--   0 sweaver    (501) staff       (20)     1490 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/BatchLanguage/MatrixIndexing.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      860 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/BatchLanguage/profile_test.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     1634 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/data/aspectrin.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)     9290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions+MLE.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5649 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10367 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1617 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions3.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      614 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Categories/displayFunction.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     3773 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/data/hiv.seq
--rw-r--r--   0 sweaver    (501) staff       (20)     2911 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint1.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3411 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2274 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint3.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1491 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/shared.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/data/
--rw-r--r--   0 sweaver    (501) staff       (20)    13602 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/data/actin2.flt
--rw-r--r--   0 sweaver    (501) staff       (20)     2610 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/HKY852blocks.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2739 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/HKY852blocks2models.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/
--rw-r--r--   0 sweaver    (501) staff       (20)     1925 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/aa.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     1147 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/3.seq
--rw-r--r--   0 sweaver    (501) staff       (20)      968 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/stewart.aa
--rw-r--r--   0 sweaver    (501) staff       (20)     2982 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/ubiq.flt
--rw-r--r--   0 sweaver    (501) staff       (20)     3527 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/ExonIntron.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/Models/
--rw-r--r--   0 sweaver    (501) staff       (20)      189 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/Models/EI.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3246 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/Models/MG94x2.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     3761 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/data/hiv.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)     2055 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/F81.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2162 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/HKY85.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2317 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/HKY85shared.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/JC69.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2066 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/K2P.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2115 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/K2Pshared.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2942 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/Non-Rev.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2182 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/REV.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2406 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/REVshared.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     1436 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/3.seq
--rw-r--r--   0 sweaver    (501) staff       (20)     1607 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/aspectrin1.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)     2067 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/aspectrin2.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)    22349 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/molclock.seq
--rw-r--r--   0 sweaver    (501) staff       (20)     4824 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81K81uf_relratio.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3660 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81relrate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3800 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81relratio.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5741 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/HKY85relrate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4797 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/HKY85relratio.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3872 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/MolecularClockF81.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3534 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/MolecularClockHKY85.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     1436 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/data/3.seq
--rw-r--r--   0 sweaver    (501) staff       (20)     3762 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/data/hiv.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)     3819 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/ParametricBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4028 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/PBootstrapHetRates.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5061 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/Examples/Simulation/RelativeRatePBS.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/help/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/help/Commands/
--rw-r--r--   0 sweaver    (501) staff       (20)     4309 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/help/Commands/query.bf
--rw-r--r--   0 sweaver    (501) staff       (20)   139264 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/help/Commands/reference.sql
--rw-r--r--   0 sweaver    (501) staff       (20)  1058637 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/help/Getting Started With HyPhy.pdf
--rw-r--r--   0 sweaver    (501) staff       (20)   966666 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/help/SelectionAnalyses.pdf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/installers/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/
--rw-r--r--   0 sweaver    (501) staff       (20)   183895 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/DMG.key
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/
--rw-r--r--   0 sweaver    (501) staff       (20)  2146965 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/Disk Image
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/
--rw-r--r--   0 sweaver    (501) staff       (20)    59967 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/Preview.jpg
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/installers/Win/
--rw-r--r--   0 sweaver    (501) staff       (20)     4544 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/installers/Win/hyphy.nsi
--rw-r--r--   0 sweaver    (501) staff       (20)     1432 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/installers/Win/license.rtf
--rw-r--r--   0 sweaver    (501) staff       (20)     1419 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/LICENSE
--rw-r--r--   0 sweaver    (501) staff       (20)      243 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/package.json
--rw-r--r--   0 sweaver    (501) staff       (20)     2204 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/README.md
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/
--rw-r--r--   0 sweaver    (501) staff       (20)      565 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Approximate_CDF
--rw-r--r--   0 sweaver    (501) staff       (20)     2173 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Column Operations
--rw-r--r--   0 sweaver    (501) staff       (20)     3746 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Complex Select Cells By Value
--rw-r--r--   0 sweaver    (501) staff       (20)     3177 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Contigency Table
--rw-r--r--   0 sweaver    (501) staff       (20)     1344 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Covariance
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/
--rw-r--r--   0 sweaver    (501) staff       (20)     1370 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/DescriptiveStats.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      364 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/FromSQLFlatFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      984 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/HY_DBW_TemplateList
--rw-r--r--   0 sweaver    (501) staff       (20)     1119 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToChartWindow.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      806 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToConsole.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      779 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2219 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFileFromPandit.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1478 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFrontierFastaFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2292 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToSQLFlatFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1093 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToTabFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2075 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Descriptive Statistics
--rw-r--r--   0 sweaver    (501) staff       (20)     3809 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Distribution Moments
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/
--rw-r--r--   0 sweaver    (501) staff       (20)     2226 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Event Posteriors
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/
--rw-r--r--   0 sweaver    (501) staff       (20)      696 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/posteriors.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1571 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Most Likely Class Assignment
--rw-r--r--   0 sweaver    (501) staff       (20)      753 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Distribution
--rw-r--r--   0 sweaver    (501) staff       (20)     1754 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Moments
--rw-r--r--   0 sweaver    (501) staff       (20)     1982 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Prior Moments
--rw-r--r--   0 sweaver    (501) staff       (20)     5473 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Gaussian Penalty Clustering
--rw-r--r--   0 sweaver    (501) staff       (20)     2078 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Goodness of Fit
--rw-r--r--   0 sweaver    (501) staff       (20)     2277 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Histogram
--rw-r--r--   0 sweaver    (501) staff       (20)     2548 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/K-Mean Clustering
--rw-r--r--   0 sweaver    (501) staff       (20)     2343 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/KH Resampler
--rw-r--r--   0 sweaver    (501) staff       (20)     1738 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Linear Fit
--rw-r--r--   0 sweaver    (501) staff       (20)     4135 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Linear Fit.orig
--rw-r--r--   0 sweaver    (501) staff       (20)     2232 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Mean Profile Plot
--rw-r--r--   0 sweaver    (501) staff       (20)     3813 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Median Profile Plot
--rw-r--r--   0 sweaver    (501) staff       (20)     7009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Poisson Mixture Fit
--rw-r--r--   0 sweaver    (501) staff       (20)      617 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Populate Cells
--rw-r--r--   0 sweaver    (501) staff       (20)     7062 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Profile Mean Clustering
--rw-r--r--   0 sweaver    (501) staff       (20)      560 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Running Sum
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/
--rw-r--r--   0 sweaver    (501) staff       (20)     1589 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/lhc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3267 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/sir.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2522 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/srs.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1095 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Select Cells By Index
--rw-r--r--   0 sweaver    (501) staff       (20)     2354 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Select Cells By Value
--rw-r--r--   0 sweaver    (501) staff       (20)      455 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/SingleColumn
--rw-r--r--   0 sweaver    (501) staff       (20)      480 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Sort
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     4680 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/data/brown.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)    10605 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/data/integrase_BDA.nex
--rw-r--r--   0 sweaver    (501) staff       (20)     4222 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/data/p51.aa
--rw-r--r--   0 sweaver    (501) staff       (20)    11176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/data/p51.nex
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/
--rw-r--r--   0 sweaver    (501) staff       (20)     5091 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Character Plot
--rw-r--r--   0 sweaver    (501) staff       (20)    11533 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Character Plot Two
--rw-r--r--   0 sweaver    (501) staff       (20)     3863 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Compare Subsets
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/ibfs/
--rw-r--r--   0 sweaver    (501) staff       (20)     1154 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/ibfs/char_colors.def
--rw-r--r--   0 sweaver    (501) staff       (20)     5719 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Sequence Plot
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/TBD/
--rw-r--r--   0 sweaver    (501) staff       (20)    11228 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/TBD/Character Plot By Sequence
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/
--rw-r--r--   0 sweaver    (501) staff       (20)      808 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Alt_Yeast_Nuclear.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      802 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Ascidian_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      782 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Blepharisma_Nuclear.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      816 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Ciliate.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      804 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Echinoderm_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      799 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Euplotid_Nuclear.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      800 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Flatworm_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      807 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Invertebrate_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      786 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Mold_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      818 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Thraustochytrium_mtDNA.cod
--rw-r--r--   0 sweaver    (501) staff       (20)     1343 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Vertebratemtdna.cod
--rw-r--r--   0 sweaver    (501) staff       (20)      762 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Yeast_mtDNA.cod
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/
--rw-r--r--   0 sweaver    (501) staff       (20)     2138 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/aa.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/
--rw-r--r--   0 sweaver    (501) staff       (20)      129 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/Equal
--rw-r--r--   0 sweaver    (501) staff       (20)    10410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/Estimated
--rw-r--r--   0 sweaver    (501) staff       (20)      158 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/Observed In Data Set
--rw-r--r--   0 sweaver    (501) staff       (20)      164 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/Observed In Partition
--rw-r--r--   0 sweaver    (501) staff       (20)     6237 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/codon.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/
--rw-r--r--   0 sweaver    (501) staff       (20)      302 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Equal
--rw-r--r--   0 sweaver    (501) staff       (20)     1834 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Codon
--rw-r--r--   0 sweaver    (501) staff       (20)     2236 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 3 params.
--rw-r--r--   0 sweaver    (501) staff       (20)     2314 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 9 params.
--rw-r--r--   0 sweaver    (501) staff       (20)     1486 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/dinuc.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/
--rw-r--r--   0 sweaver    (501) staff       (20)      392 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/2 Bin Discrete
--rw-r--r--   0 sweaver    (501) staff       (20)      559 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta
--rw-r--r--   0 sweaver    (501) staff       (20)      983 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta-Gamma
--rw-r--r--   0 sweaver    (501) staff       (20)     2033 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/General Discrete
--rw-r--r--   0 sweaver    (501) staff       (20)      973 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Half Normal
--rw-r--r--   0 sweaver    (501) staff       (20)      546 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Lognormal
--rw-r--r--   0 sweaver    (501) staff       (20)      467 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/nuc.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/
--rw-r--r--   0 sweaver    (501) staff       (20)       65 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/Equal
--rw-r--r--   0 sweaver    (501) staff       (20)      743 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/Estimated
--rw-r--r--   0 sweaver    (501) staff       (20)      157 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/Observed In Data Set
--rw-r--r--   0 sweaver    (501) staff       (20)      164 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/Observed In Partition
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/
--rw-r--r--   0 sweaver    (501) staff       (20)    11493 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Dayhoff.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    11447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/EIAA.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Fitness.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    34336 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Jones.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    65577 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/mtREV.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Binary/
--rw-r--r--   0 sweaver    (501) staff       (20)     1143 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Binary/F81.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/
--rw-r--r--   0 sweaver    (501) staff       (20)     6405 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/GY94_3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     6966 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/Lineage_MG94xHKY85.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5187 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5317 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     6785 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_HKY85x3_4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    13590 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl copy
--rw-r--r--   0 sweaver    (501) staff       (20)    13893 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94REVOmegaCF3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     6331 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xHKY85_3x4_2Rates.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    11704 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    16141 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV_GDD.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    13510 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xTN93_3x4.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/
--rw-r--r--   0 sweaver    (501) staff       (20)      896 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/EFVEstimated.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1908 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/F81.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2421 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/HKY85.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2470 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/REV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3137 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/REVBetaGamma.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2202 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/TrN.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/Nucleotide/
--rw-r--r--   0 sweaver    (501) staff       (20)      586 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/Nucleotide/JC69
--rw-r--r--   0 sweaver    (501) staff       (20)      585 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/Nucleotide/K2P
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/
--rw-r--r--   0 sweaver    (501) staff       (20)     5319 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGenerator.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3582 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGeneratorNoPS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      532 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma1.def
--rw-r--r--   0 sweaver    (501) staff       (20)      929 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2+Inv.def
--rw-r--r--   0 sweaver    (501) staff       (20)      521 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2.def
--rw-r--r--   0 sweaver    (501) staff       (20)     8050 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/GY94.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     8503 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94GY94xREV_PARRIS_syn3.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3921 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4608 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate_Multirate.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      327 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M1.def
--rw-r--r--   0 sweaver    (501) staff       (20)      490 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M2.def
--rw-r--r--   0 sweaver    (501) staff       (20)      558 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M3.def
--rw-r--r--   0 sweaver    (501) staff       (20)      758 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_syn3.def
--rw-r--r--   0 sweaver    (501) staff       (20)      611 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_synvar.def
--rw-r--r--   0 sweaver    (501) staff       (20)    14930 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/454.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4529 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_BMS_Aux.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     8855 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_CMS_Aux.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     6946 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_MFReader_.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1434 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_MSCOneStep.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1893 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_tipDater.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     5743 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AAModelComparison.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     8889 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AddABias.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1285 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonData.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1662 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonDataMPI.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      661 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeDiNucData.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      933 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1348 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      868 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2705 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    20444 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/bayesgraph.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     7847 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BGM.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1647 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/binomial.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     3040 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BivariateCodonRateAnalysis.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchClassDNDS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    39439 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSiteREL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    20586 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSiteRELMultiModel.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10067 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSwap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     8954 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/branchSwappingFunctions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9281 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BS2007.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    25244 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BUSTED-SRV.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    22782 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BUSTED.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4441 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/categoryEcho.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4025 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/chooseDistanceFormula.def
--rw-r--r--   0 sweaver    (501) staff       (20)     3199 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CleanGaps.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5357 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CleanStopCodons.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10610 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ClusterAnalysis.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    15352 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ClusterByDistanceRange.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12219 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonBivariateRateProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    26094 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonModelCompare.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5020 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonToProtein.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    17567 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonUsageBias.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    26595 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressure.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    28200 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressureIVL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2240 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ConvertDataFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    16520 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DatedTipsMolecularClock.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    17285 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DirectionalREL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    14633 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DirectionalREL_MF.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7993 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DistanceMatrix.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5987 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DistanceMatrix_Splits.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9696 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/distanceMethodNPBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7859 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/distanceRMethodNPBootstrap.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/
--rw-r--r--   0 sweaver    (501) staff       (20)      303 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools.def
--rw-r--r--   0 sweaver    (501) staff       (20)      639 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools2.def
--rw-r--r--   0 sweaver    (501) staff       (20)     9815 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/CodonToolsMain.def
--rw-r--r--   0 sweaver    (501) staff       (20)      648 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/JC69
--rw-r--r--   0 sweaver    (501) staff       (20)     1011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/K2P
--rw-r--r--   0 sweaver    (501) staff       (20)     1300 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/K2P_RV
--rw-r--r--   0 sweaver    (501) staff       (20)     3755 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Modified_Nei_Gojobori
--rw-r--r--   0 sweaver    (501) staff       (20)     3554 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Nei_Gojobori
--rw-r--r--   0 sweaver    (501) staff       (20)      478 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance
--rw-r--r--   0 sweaver    (501) staff       (20)      564 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_aa
--rw-r--r--   0 sweaver    (501) staff       (20)      426 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_binary
--rw-r--r--   0 sweaver    (501) staff       (20)     1802 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_codon
--rw-r--r--   0 sweaver    (501) staff       (20)      530 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC
--rw-r--r--   0 sweaver    (501) staff       (20)      663 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC_MH
--rw-r--r--   0 sweaver    (501) staff       (20)      797 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC_RV
--rw-r--r--   0 sweaver    (501) staff       (20)     1236 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/T3P
--rw-r--r--   0 sweaver    (501) staff       (20)     1330 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN84
--rw-r--r--   0 sweaver    (501) staff       (20)     2554 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN93
--rw-r--r--   0 sweaver    (501) staff       (20)     1925 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN93_RV
--rw-r--r--   0 sweaver    (501) staff       (20)      779 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ
--rw-r--r--   0 sweaver    (501) staff       (20)     2090 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ_FR
--rw-r--r--   0 sweaver    (501) staff       (20)    22019 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    21748 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis_CompareDS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    29296 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparison.bf
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonMF.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    27567 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonPartitions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    26791 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    22355 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis_MF.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    38053 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSResultProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3081 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/doNNISwap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2845 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/doSPRSwap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2661 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dSdNTreeTools.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    19450 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/F_ST.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    13594 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/files.lst
--rw-r--r--   0 sweaver    (501) staff       (20)     9512 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FitnessAAModels.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12603 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/
--rw-r--r--   0 sweaver    (501) staff       (20)      888 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_1.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5481 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10126 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_3.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4104 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_4.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     6078 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_5.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    13689 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_tools.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    11476 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    14350 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC_Binary.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    11098 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC_kernel.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    18602 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClock.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7512 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClock.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    11148 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12964 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessorM.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    34882 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARD.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    11689 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARD_GA_CHC.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    19257 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARDProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    21840 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARecomb.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     8282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Gateaux.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7298 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Gateaux2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7803 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GateauxMR.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      511 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/globalChecker.ibf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GUI/
--rw-r--r--   0 sweaver    (501) staff       (20)       17 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GUI/crayolaColors.def
--rw-r--r--   0 sweaver    (501) staff       (20)     5893 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/heuristicMethodNPBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5901 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_k_means.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1768 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_PCA.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3707 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_support.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     8139 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/KHTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)       15 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/last.date
--rw-r--r--   0 sweaver    (501) staff       (20)     6300 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LHT.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/
--rw-r--r--   0 sweaver    (501) staff       (20)     6190 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/IOFunctions.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/
--rw-r--r--   0 sweaver    (501) staff       (20)     6272 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/MG_REV.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3813 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/
--rw-r--r--   0 sweaver    (501) staff       (20)     2224 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/GTR.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10300 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/frequencies.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7701 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/model_functions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9533 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/parameters.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4691 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/rate_variation.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1582 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/terms.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/
--rw-r--r--   0 sweaver    (501) staff       (20)    14665 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/estimators.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4161 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/UtilityFunctions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    11442 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LocalBranchSiteTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5630 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LocalMolClock.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7823 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LRTRecombTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2276 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LZ_Complexity.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     6011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MaxChi2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    19047 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MEDS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    28108 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MEME_mf.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MergeSequences.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      966 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MergeSites.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    30660 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPositiveSelection.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    23831 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPositiveSelectionPooled.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2390 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPSreader.def
--rw-r--r--   0 sweaver    (501) staff       (20)    17424 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MGvsGY.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10597 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorAAProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    20242 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorBranch.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    27326 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1090 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    25639 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodonProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    15293 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    18886 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA_1.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    19567 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5904 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MolClockAllRoots.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5995 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/molclockBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3227 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MolecularClock.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4136 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NeighborJoining.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    32201 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NielsenYang.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    24628 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NucModelCompare.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10649 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimator.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)      180 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimatorCounter.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseDNDS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7411 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9879 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRatio.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5724 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseSiteDiversity.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    42655 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PARRIS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1794 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PartitionDataFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    21208 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PartitionRateComparison.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2013 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/partitionSequences.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)       99 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Phylohandbook.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9486 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Plato.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    56606 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PositiveSelectionLI.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      661 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_ancestors.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1215 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_counting.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1545 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_covariance.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2760 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_dNdS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      352 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_lfprofile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      359 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_npbs.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      324 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_pbs.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4839 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_sampler.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1396 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_saveResults.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2989 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_sns.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3903 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_variance.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_viewResults.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      880 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/postprocessors.lst
--rw-r--r--   0 sweaver    (501) staff       (20)    22914 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper1.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     7623 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper1_mf.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    13478 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper2.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    14145 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper2_mf.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     4409 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper3.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     4353 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper4.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     2857 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/queryTree.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    64552 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetection.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10529 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetectionMF.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    22326 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RateClassCounter.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/readIndexFile.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9107 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ReduceDataSetMatrix.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3530 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7196 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRateL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5504 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRatio.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    30183 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RELAX.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10172 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relrateBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7194 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relrateBootstrapL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4502 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relratioBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    37032 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SampleProcessor.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/
--rw-r--r--   0 sweaver    (501) staff       (20)     6523 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/lhc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1237 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/lhc_supp.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     3267 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/sir.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9016 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/srs.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     9437 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SandNSAmbigs.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10851 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SelectionLRT.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      438 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/selectModelParameters.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1615 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignment.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      169 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodon.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     8080 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodonShared.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    19136 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNuc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7277 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNucShared.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     5205 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentProt.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    51307 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentTop75.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    85186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignShared.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     5622 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SequentialAddition.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    15486 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SequentialAddition.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)    13154 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGASimProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    23306 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGEmulator.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    19432 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGEmulator_MF.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    18761 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGIvL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4634 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimilarityPlot.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     8321 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimmondsAI.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/simpleBootstrap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5283 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimpleMutationCounter.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    17630 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb-2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    29435 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5934 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SiteRates.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7392 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SiteRates2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9012 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison-2parts.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9952 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2436 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlidingNucWindow.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     6430 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlidingWindowAnalysis.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1294 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SplitSequencesByPattern.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5308 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SSRatesTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    13759 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StarDecomposition.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4667 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StrandGRMTest.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2321 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StripStopCodons.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9922 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SubtreeSelectionComparison.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/
--rw-r--r--   0 sweaver    (501) staff       (20)     1405 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/190
--rw-r--r--   0 sweaver    (501) staff       (20)     7115 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/BranchSiteTemplate.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2735 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/CF3x4.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    16966 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/chooseGeneticCode.def
--rw-r--r--   0 sweaver    (501) staff       (20)     9371 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/custm4x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3522 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4357 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA_empirical.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    34528 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    34043 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      867 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Default
--rw-r--r--   0 sweaver    (501) staff       (20)    10995 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineGamma.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    10198 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineHM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4155 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F+omega.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4153 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4634 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4305 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+MLFREQS.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4154 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1636 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAA.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2240 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAAFreq.mdl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/
--rw-r--r--   0 sweaver    (501) staff       (20)     6408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/BLOSUM62
--rw-r--r--   0 sweaver    (501) staff       (20)     6408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/cpREV
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/Dayhoff
--rw-r--r--   0 sweaver    (501) staff       (20)     8010 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/H5N1
--rw-r--r--   0 sweaver    (501) staff       (20)     3507 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVBetween
--rw-r--r--   0 sweaver    (501) staff       (20)     3233 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVWithin
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/IAV
--rw-r--r--   0 sweaver    (501) staff       (20)     8091 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/JTT
--rwxr-xr-x   0 sweaver    (501) staff       (20)    36640 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LCAP
--rw-r--r--   0 sweaver    (501) staff       (20)     6408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LG
--rw-r--r--   0 sweaver    (501) staff       (20)    10147 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/modellist.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     6408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/MtArt
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtMAM
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtREV24
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/rtREV
--rw-r--r--   0 sweaver    (501) staff       (20)     6408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/VT
--rw-r--r--   0 sweaver    (501) staff       (20)     6410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/WAG
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/
--rw-r--r--   0 sweaver    (501) staff       (20)    37977 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECM
--rw-r--r--   0 sweaver    (501) staff       (20)    38029 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECMu
--rw-r--r--   0 sweaver    (501) staff       (20)     2727 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.dat
--rw-r--r--   0 sweaver    (501) staff       (20)    34672 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1259 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1191 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81_binary.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2386 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3755 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84P.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1878 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/fitness.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1672 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GRM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4985 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1878 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     7177 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94customF3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     2179 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94w9.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      355 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween+F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     3949 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)      597 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      351 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin+F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     4072 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)      490 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1529 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HKY85.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1256 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1175 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69_binary.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    35087 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    34009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1422 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/K2P.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1513 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/K3ST.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     9171 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/LCAP.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     8013 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MEC.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5854 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     9572 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94custom.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     9771 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customCF3x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     9582 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customF1x4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     9067 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customFreqs.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     6082 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAA.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5353 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5584 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61multiple.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5499 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAFreqs.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5409 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAUserFreqs.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5496 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wEX.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     6441 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94with9freqs.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    11062 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94x2.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1533 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGFreqsEstimator.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     3356 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwAA.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     2688 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwEX.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)      800 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      546 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters2.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      659 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters3.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1699 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters4.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      660 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters5.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    10986 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/models.lst
--rw-r--r--   0 sweaver    (501) staff       (20)    16378 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    15997 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1474 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    28224 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    27857 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1584 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM+Freqs.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1739 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      867 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/PCH
--rw-r--r--   0 sweaver    (501) staff       (20)     3060 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/reducedREV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5828 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1480 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16A
--rw-r--r--   0 sweaver    (501) staff       (20)     3487 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16SvH.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAEqualInput
--rw-r--r--   0 sweaver    (501) staff       (20)      916 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAF81
--rw-r--r--   0 sweaver    (501) staff       (20)     3749 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAMuse95.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      809 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV
--rw-r--r--   0 sweaver    (501) staff       (20)      785 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV_1
--rw-r--r--   0 sweaver    (501) staff       (20)    28734 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    28346 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)      866 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/S4
--rw-r--r--   0 sweaver    (501) staff       (20)     1656 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/STGRM.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     1564 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/TrN.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)     5119 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/UniversalCode.def
--rw-r--r--   0 sweaver    (501) staff       (20)    28569 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    28123 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG_F.mdl
--rw-r--r--   0 sweaver    (501) staff       (20)    10677 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Yang2000Distributions.def
--rw-r--r--   0 sweaver    (501) staff       (20)    12310 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestBranchDNDS.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    23991 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestClade.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10295 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestCladeMeans.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    10783 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TopologySearch.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9153 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TopologySearchConstrained.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     7969 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TreeCorrelationCoefficients.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    20678 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TreeTools.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     1549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/UpperBound.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/
--rw-r--r--   0 sweaver    (501) staff       (20)    23866 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/AncestralMapper.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2716 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/BranchLengthFitters.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12371 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/CoalescentPostProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1667 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/CodonTools.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4505 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/DBTools.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     2773 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/DescriptiveStatistics.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    22537 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/GrabBag.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    20471 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/HXB2Mapper.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3190 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREV.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5349 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREVMLFreqs.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2617 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/MPITools.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     6228 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/NJ.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    12199 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/PostScript.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1814 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/ProbabilityDistributions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    51558 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/PS_Plotters.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    11502 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/ReadDelimitedFiles.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/TreeFunctions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1194 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/WriteDelimitedFiles.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9316 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/WANC.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5727 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/WebUpdate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    15337 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/YangNielsenBranchSite2005.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/
--rw-r--r--   0 sweaver    (501) staff       (20)     9261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Exhaustive_Search
--rw-r--r--   0 sweaver    (501) staff       (20)     3069 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Neighbor_Joining
--rw-r--r--   0 sweaver    (501) staff       (20)    17241 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Sequential_Addition
--rw-r--r--   0 sweaver    (501) staff       (20)    16065 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Star_Decomposition
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/
--rw-r--r--   0 sweaver    (501) staff       (20)     8954 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/branchSwappingFunctions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2102 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/doNNISwap.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2560 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/doSPRSwap.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/TreeAddIns/
--rw-r--r--   0 sweaver    (501) staff       (20)      865 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TreeAddIns/Splits
--rw-r--r--   0 sweaver    (501) staff       (20)     4101 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/TreeAddIns/Tree Statistics
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/
--rw-r--r--   0 sweaver    (501) staff       (20)      962 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/AAContent
--rw-r--r--   0 sweaver    (501) staff       (20)      143 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/BatchFileByURL
--rw-r--r--   0 sweaver    (501) staff       (20)     2301 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/BranchLengthCI
--rw-r--r--   0 sweaver    (501) staff       (20)     7494 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/CodonMutationToTreeMapper
--rw-r--r--   0 sweaver    (501) staff       (20)     2421 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/CountSubstitutions
--rw-r--r--   0 sweaver    (501) staff       (20)     1056 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/ExportLikelihoodFunction
--rw-r--r--   0 sweaver    (501) staff       (20)     1014 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/GenBankSequences
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/
--rw-r--r--   0 sweaver    (501) staff       (20)      503 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/ChooseALF.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     4912 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/MappersHelp.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     3617 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/MappersHelpAA.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)      577 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/ListUserFunctions
--rw-r--r--   0 sweaver    (501) staff       (20)      326 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/LRT
--rw-r--r--   0 sweaver    (501) staff       (20)     2593 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/MapSubstitutions
--rw-r--r--   0 sweaver    (501) staff       (20)     2242 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/MeanPairwiseDivergence
--rw-r--r--   0 sweaver    (501) staff       (20)     4399 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/MeanPairwiseDivergenceSubset
--rw-r--r--   0 sweaver    (501) staff       (20)      820 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/ModelCounter
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/
--rw-r--r--   0 sweaver    (501) staff       (20)     7682 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/AAMutationCounter
--rw-r--r--   0 sweaver    (501) staff       (20)    11071 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/CodonMutationToTreeMapper.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     5100 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ColorPSTree
--rw-r--r--   0 sweaver    (501) staff       (20)     7362 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ConvergentAndParallel
--rw-r--r--   0 sweaver    (501) staff       (20)      637 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/CopyBranchLengths
--rw-r--r--   0 sweaver    (501) staff       (20)     4422 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/DashPSTree
--rw-r--r--   0 sweaver    (501) staff       (20)     5382 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/dNanddSTrees.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      993 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/dS and dN factors
--rw-r--r--   0 sweaver    (501) staff       (20)     1240 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ExpsPerDirection
--rw-r--r--   0 sweaver    (501) staff       (20)      934 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/FilterAssignments
--rw-r--r--   0 sweaver    (501) staff       (20)    10154 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/InferredAASubstitutionsCounter
--rw-r--r--   0 sweaver    (501) staff       (20)     1650 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/LocaldNdS
--rw-r--r--   0 sweaver    (501) staff       (20)     1011 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ModelFitSummary
--rw-r--r--   0 sweaver    (501) staff       (20)     1511 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ModelFitSummaryAA
--rw-r--r--   0 sweaver    (501) staff       (20)     5024 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/Multiclass DN DS inference
--rw-r--r--   0 sweaver    (501) staff       (20)      990 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/PartitionBranchesByClasses
--rw-r--r--   0 sweaver    (501) staff       (20)     7047 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/PredictivePosteriorP
--rw-r--r--   0 sweaver    (501) staff       (20)     1058 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/RNARateMatrix
--rw-r--r--   0 sweaver    (501) staff       (20)     2768 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/SimulateAndTabDN_DS
--rw-r--r--   0 sweaver    (501) staff       (20)      907 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/SimulateFromLF
--rw-r--r--   0 sweaver    (501) staff       (20)     1850 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/TreeLengthConstraint
--rw-r--r--   0 sweaver    (501) staff       (20)    17476 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/RecombinationProcessor.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      664 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/SimulateFromLF
--rw-r--r--   0 sweaver    (501) staff       (20)      859 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/res/UserAddins/Tidbits
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/scripts/
--rw-r--r--   0 sweaver    (501) staff       (20)    11424 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/build.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     2449 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/build_mingw.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     3440 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/build_mingw_gui.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     2619 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/build_mingw_MEGA.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     2398 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/buildFromSVN.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     2195 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/buildMinGWFromSVN.sh
--rw-r--r--   0 sweaver    (501) staff       (20)     5703 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/gtk_build.sh
--rw-r--r--   0 sweaver    (501) staff       (20)      302 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/scripts/intelCCbuild.sh
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/src/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/core/
--rw-r--r--   0 sweaver    (501) staff       (20)     2532 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/_hyExecutionContext.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    70504 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/alignment.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    24278 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/avllist.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     4335 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/avllistx.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     4499 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/avllistxl.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    21889 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/baseobj.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   280975 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/batchlan.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   103816 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/batchlan2.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    12374 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/batchlanhelpers.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    59844 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/batchlanruntime.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   424517 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/calcnode.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   108848 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/calcnode2.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    44699 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/category.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    12941 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/classes.cp
--rw-r--r--   0 sweaver    (501) staff       (20)    23670 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/constant.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    12778 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/error.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    72077 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/fisher_exact.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    92271 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/formula.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    28192 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/fstring.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/
--rw-r--r--   0 sweaver    (501) staff       (20)     2155 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/_hyExecutionContext.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3945 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/alignment.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3319 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/avllist.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2288 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/avllistx.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2203 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/avllistxl.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4060 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/baseobj.h
--rw-r--r--   0 sweaver    (501) staff       (20)    25807 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/batchlan.h
--rw-r--r--   0 sweaver    (501) staff       (20)    35475 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/calcnode.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/category.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6116 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/classes.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4446 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/constant.h
--rw-r--r--   0 sweaver    (501) staff       (20)    14580 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/defines.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2684 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/errorfns.h
--rw-r--r--   0 sweaver    (501) staff       (20)     8893 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/formula.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4039 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/fstring.h
--rw-r--r--   0 sweaver    (501) staff       (20)    19044 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/gnuregex.h
--rw-r--r--   0 sweaver    (501) staff       (20)    31149 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/hy_strings.h
--rw-r--r--   0 sweaver    (501) staff       (20)    32307 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/likefunc.h
--rw-r--r--   0 sweaver    (501) staff       (20)    11141 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/list.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9005 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/mathobj.h
--rw-r--r--   0 sweaver    (501) staff       (20)    30760 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/matrix.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4748 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/mypthread.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4967 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/operation.h
--rw-r--r--   0 sweaver    (501) staff       (20)     7299 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/parser.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6990 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/polynoml.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3570 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/sequence.h
--rw-r--r--   0 sweaver    (501) staff       (20)    16440 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/simplelist.h
--rw-r--r--   0 sweaver    (501) staff       (20)    21529 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/site.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2215 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/stack.h
--rw-r--r--   0 sweaver    (501) staff       (20)    11816 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/trie.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5680 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/variable.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5767 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/include/variablecontainer.h
--rw-r--r--   0 sweaver    (501) staff       (20)   403092 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/likefunc.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    61517 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/likefunc2.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    50097 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/likefuncocl.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16832 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/list.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6388 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/mathobj.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   338060 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/matrix.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    59369 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/nexus.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    19891 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/operation.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    39732 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/parser.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    68320 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/parser2.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   105197 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/polynoml.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     2816 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/ptr_array.cp
--rw-r--r--   0 sweaver    (501) staff       (20)   179566 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/regex.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20668 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/sequence.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    44902 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/simplelist.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   213854 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/site.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     2955 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/stack.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    62152 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/strings.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16902 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/trie.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20453 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/variable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    37397 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/core/variablecontainer.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     4045 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYButton.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6258 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYButtonBar.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     2904 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYCheckBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     4444 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYLabel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6149 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYPullDown.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    50829 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYSequencePanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    71812 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6836 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYTextBox.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     9140 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformButton.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16910 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformButtonBar.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     7791 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformCheckBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     7456 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformLabel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16779 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformPullDown.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16680 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformSequencePane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    60674 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20953 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformTextBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    18725 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformComponent.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20757 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformGraphicPane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    23566 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformUtils.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    27342 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformWindow.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     2498 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformButton.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2697 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformButtonBar.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2257 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformCheckbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2321 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformLabel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2971 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformPullDown.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3033 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformTable.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3207 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformTextbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3434 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformComponent.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4506 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformGraphicPane.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6495 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformWindow.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/
--rw-r--r--   0 sweaver    (501) staff       (20)     2215 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformBootsrapWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    14800 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformChartWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    23442 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformConsoleWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    35368 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDataPanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     1785 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDBWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     3015 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformGWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6951 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformModelWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    12460 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformParameterTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     7278 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformPWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    39261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTreePanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    18555 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     5339 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYBaseGUI.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   156385 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYChartWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    12755 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYComponent.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    22083 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYConsoleWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   340254 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYDataPanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    42655 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYDBWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   149461 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYDialogDefs.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    10751 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYEventTypes.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16430 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYGraphicPane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   134951 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYModelWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    34422 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYObjectInspector.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   166170 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYParameterTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    15418 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYSharedMain.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   268500 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYTreePanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    22505 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/HYWindow.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     2072 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYButton.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2685 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYButtonBar.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1706 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYCanvas.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3562 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYComponent.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3018 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYLabel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYList.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2800 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYPullDown.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4285 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYSequencePanel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     8079 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYTableComponent.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3811 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYTextBox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2371 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYBaseGUI.h
--rw-r--r--   0 sweaver    (501) staff       (20)     9573 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYDialogs.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2654 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYEventTypes.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4321 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYGraphicPane.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1357 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYObjectInspector.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3659 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYSharedMain.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3124 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYTableWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3771 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYUtils.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/HYWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2838 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/preferences.h
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/shared_main.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/
--rw-r--r--   0 sweaver    (501) staff       (20)     8761 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYChartWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     3045 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYConsoleWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)    12813 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYDataPanel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2350 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYDBWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYGWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     6641 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYModelWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     8058 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYParameterTable.h
--rw-r--r--   0 sweaver    (501) staff       (20)    15151 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYTreePanel.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     9410 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformButton.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20124 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformButtonBar.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformCheckBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     5790 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformLabel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8223 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformList.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     9014 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformPullDown.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8580 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformSequencePane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    62184 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    35459 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformTextBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   169303 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Docs.icns
--rw-r--r--   0 sweaver    (501) staff       (20)    26364 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/hydialogs.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   169303 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPHY.icns
--rw-r--r--   0 sweaver    (501) staff       (20)   388670 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HyPhy.rsrc
--rw-r--r--   0 sweaver    (501) staff       (20)   169303 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPHYMP.icns
--rw-r--r--   0 sweaver    (501) staff       (20)    25014 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformComponent.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16752 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformGraphicPane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    31651 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformUtils.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    32566 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   388670 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/iHyPhyDebug.rsrc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     1136 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformButton.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1438 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformButtonBar.h
--rw-r--r--   0 sweaver    (501) staff       (20)      871 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformCheckbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1004 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformLabel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1147 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformList.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1599 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformPullDown.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1422 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformTable.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1932 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformTextbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5096 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformButtonMenu.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1798 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformComponent.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2636 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformGraphicPane.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4461 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1557 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/Info.plist
--rw-r--r--   0 sweaver    (501) staff       (20)       91 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/plist.r
--rw-r--r--   0 sweaver    (501) staff       (20)     1017 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/plist.xml
--rw-r--r--   0 sweaver    (501) staff       (20)       93 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/plistmp.r
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/
--rw-r--r--   0 sweaver    (501) staff       (20)      854 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformBootsrapWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    17835 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformChartWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    10084 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformConsoleWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    38052 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDataPanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)      722 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDBWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     9566 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformGWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6003 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformModelWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8400 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformParameterTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    11564 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformPWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    49772 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTreePanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16460 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    34864 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/preferences.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/
--rw-r--r--   0 sweaver    (501) staff       (20)     7009 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/helpers.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     2055 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphy_qt_utility.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     1698 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphyevents.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8105 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphyhierarchicalselector.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    17372 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphymain.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     2191 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphymessageoutput.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/
--rw-r--r--   0 sweaver    (501) staff       (20)     2513 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphy_qt_helpers.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1935 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphyevents.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2431 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphyhierarchicalselector.h
--rw-r--r--   0 sweaver    (501) staff       (20)     5120 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphymain.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1658 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphymessageoutput.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1227 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/qterminal.h
--rw-r--r--   0 sweaver    (501) staff       (20)      557 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/simplerequest.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1300 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/main.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     9282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/qterminal.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     1965 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/simplerequest.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/
--rw-r--r--   0 sweaver    (501) staff       (20)     1795 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphyhierarchicalselector.ui
--rw-r--r--   0 sweaver    (501) staff       (20)     1190 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphymain.ui
--rw-r--r--   0 sweaver    (501) staff       (20)     1186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphymessageoutput.ui
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/
--rw-r--r--   0 sweaver    (501) staff       (20)     1240 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/130.png
--rw-r--r--   0 sweaver    (501) staff       (20)      164 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/131.png
--rw-r--r--   0 sweaver    (501) staff       (20)      189 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/132.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1596 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/133.png
--rw-r--r--   0 sweaver    (501) staff       (20)      936 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4000.png
--rw-r--r--   0 sweaver    (501) staff       (20)      463 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4000.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)      184 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4001.png
--rw-r--r--   0 sweaver    (501) staff       (20)      463 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4001.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)      176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4002.png
--rw-r--r--   0 sweaver    (501) staff       (20)      447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4002.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)      177 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4003.png
--rw-r--r--   0 sweaver    (501) staff       (20)      447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4003.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)      899 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4011.png
--rw-r--r--   0 sweaver    (501) staff       (20)      918 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4020.png
--rw-r--r--   0 sweaver    (501) staff       (20)      288 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5000.png
--rw-r--r--   0 sweaver    (501) staff       (20)      277 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5001.png
--rw-r--r--   0 sweaver    (501) staff       (20)      295 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5002.png
--rw-r--r--   0 sweaver    (501) staff       (20)      271 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5003.png
--rw-r--r--   0 sweaver    (501) staff       (20)      267 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5004.png
--rw-r--r--   0 sweaver    (501) staff       (20)      274 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5005.png
--rw-r--r--   0 sweaver    (501) staff       (20)      152 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5006.png
--rw-r--r--   0 sweaver    (501) staff       (20)      231 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5007.png
--rw-r--r--   0 sweaver    (501) staff       (20)      918 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5020.png
--rw-r--r--   0 sweaver    (501) staff       (20)      935 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6000.png
--rw-r--r--   0 sweaver    (501) staff       (20)      922 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6001.png
--rw-r--r--   0 sweaver    (501) staff       (20)      900 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6002.png
--rw-r--r--   0 sweaver    (501) staff       (20)      968 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6003.png
--rw-r--r--   0 sweaver    (501) staff       (20)      927 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6004.png
--rw-r--r--   0 sweaver    (501) staff       (20)      952 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6005.png
--rw-r--r--   0 sweaver    (501) staff       (20)      946 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6006.png
--rw-r--r--   0 sweaver    (501) staff       (20)      208 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6007.png
--rw-r--r--   0 sweaver    (501) staff       (20)      217 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6008.png
--rw-r--r--   0 sweaver    (501) staff       (20)      191 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6009.png
--rw-r--r--   0 sweaver    (501) staff       (20)      913 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6010.png
--rw-r--r--   0 sweaver    (501) staff       (20)      945 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6011.png
--rw-r--r--   0 sweaver    (501) staff       (20)      198 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6012.png
--rw-r--r--   0 sweaver    (501) staff       (20)      191 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6013.png
--rw-r--r--   0 sweaver    (501) staff       (20)      202 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6014.png
--rw-r--r--   0 sweaver    (501) staff       (20)      963 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6016.png
--rw-r--r--   0 sweaver    (501) staff       (20)      307 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6017.png
--rw-r--r--   0 sweaver    (501) staff       (20)      271 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6018.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6019.png
--rw-r--r--   0 sweaver    (501) staff       (20)      205 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6020.png
--rw-r--r--   0 sweaver    (501) staff       (20)      291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6021.png
--rw-r--r--   0 sweaver    (501) staff       (20)      326 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6022.png
--rw-r--r--   0 sweaver    (501) staff       (20)      945 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6030.png
--rw-r--r--   0 sweaver    (501) staff       (20)      265 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6031.png
--rw-r--r--   0 sweaver    (501) staff       (20)      283 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6032.png
--rw-r--r--   0 sweaver    (501) staff       (20)      942 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6033.png
--rw-r--r--   0 sweaver    (501) staff       (20)      959 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6034.png
--rw-r--r--   0 sweaver    (501) staff       (20)      948 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6035.png
--rw-r--r--   0 sweaver    (501) staff       (20)      957 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6036.png
--rw-r--r--   0 sweaver    (501) staff       (20)      925 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6040.png
--rw-r--r--   0 sweaver    (501) staff       (20)      925 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6041.png
--rw-r--r--   0 sweaver    (501) staff       (20)      920 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6042.png
--rw-r--r--   0 sweaver    (501) staff       (20)      923 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7000.png
--rw-r--r--   0 sweaver    (501) staff       (20)      933 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7001.png
--rw-r--r--   0 sweaver    (501) staff       (20)      933 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7002.png
--rw-r--r--   0 sweaver    (501) staff       (20)      921 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7003.png
--rw-r--r--   0 sweaver    (501) staff       (20)      943 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7004.png
--rw-r--r--   0 sweaver    (501) staff       (20)      978 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7005.png
--rw-r--r--   0 sweaver    (501) staff       (20)      929 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7010.png
--rw-r--r--   0 sweaver    (501) staff       (20)      247 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7011.png
--rw-r--r--   0 sweaver    (501) staff       (20)      225 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7012.png
--rw-r--r--   0 sweaver    (501) staff       (20)      229 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7013.png
--rw-r--r--   0 sweaver    (501) staff       (20)      202 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7014.png
--rw-r--r--   0 sweaver    (501) staff       (20)      194 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7020.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1021 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7050.png
--rw-r--r--   0 sweaver    (501) staff       (20)      282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/striped.xpm
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/
--rw-r--r--   0 sweaver    (501) staff       (20)    24576 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.gtkrc.swp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton1.1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      142 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/active1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_down.png
--rw-r--r--   0 sweaver    (501) staff       (20)      261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_down1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_left.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_right.png
--rw-r--r--   0 sweaver    (501) staff       (20)      165 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_sub.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_up.png
--rw-r--r--   0 sweaver    (501) staff       (20)      355 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-2.0.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      673 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-panther1.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)     3668 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.png
--rw-r--r--   0 sweaver    (501) staff       (20)      147 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base2.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      427 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base3.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      148 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bc.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)     3669 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)     3669 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg1.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)     3669 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg2.xpm
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/blue.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button4.png
--rw-r--r--   0 sweaver    (501) staff       (20)      291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check-radio.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/clear.png
--rw-r--r--   0 sweaver    (501) staff       (20)       65 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/color.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/default.png
--rw-r--r--   0 sweaver    (501) staff       (20)       86 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/entry1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      507 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/ext1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      506 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/ext2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3258 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3201 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3087 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3258 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      426 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/exttop1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      426 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/exttop2.png
--rw-r--r--   0 sweaver    (501) staff       (20)       86 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/flat.png
--rw-r--r--   0 sweaver    (501) staff       (20)      551 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/gem.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/green.png
--rw-r--r--   0 sweaver    (501) staff       (20)      325 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/handle.png
--rw-r--r--   0 sweaver    (501) staff       (20)      113 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hline.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hscroll1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hscroll2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      643 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hstrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1119 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/htrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)       86 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/in.png
--rw-r--r--   0 sweaver    (501) staff       (20)      549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/insen.png
--rw-r--r--   0 sweaver    (501) staff       (20)       65 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/lineh.png
--rw-r--r--   0 sweaver    (501) staff       (20)      291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu-base.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu-item.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      549 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/normal1.png
--rw-r--r--   0 sweaver    (501) staff       (20)       86 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/note.png
--rw-r--r--   0 sweaver    (501) staff       (20)      500 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/obutton1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      500 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/obutton2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      175 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option_menu.png
--rw-r--r--   0 sweaver    (501) staff       (20)      175 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option_menu2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      153 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/paned1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      153 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/paned2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      673 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/pase-panther1
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      230 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/radio1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/radio2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/red.png
--rw-r--r--   0 sweaver    (501) staff       (20)      235 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll-base.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)     1119 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll4.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown.1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slide.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1026 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1026 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      187 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/small-base.xcf
--rw-r--r--   0 sweaver    (501) staff       (20)      261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup.1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/trough.png
--rw-r--r--   0 sweaver    (501) staff       (20)       86 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/up.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vscroll1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vscroll2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      468 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vslide.png
--rw-r--r--   0 sweaver    (501) staff       (20)      234 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vslide1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      643 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vstrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1025 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vtrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)      186 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/yellow.png
--rw-r--r--   0 sweaver    (501) staff       (20)      281 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_down1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      281 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_down2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      281 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_down3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      276 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_left1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      276 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_left2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      276 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_left3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_right1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_right2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      290 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_right3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      250 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_up1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      250 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_up2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      250 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/arrow_up3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/background.png
--rw-r--r--   0 sweaver    (501) staff       (20)       71 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/blank.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3873 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button0.png
--rw-r--r--   0 sweaver    (501) staff       (20)      811 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1928 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button11.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1967 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button11alpha.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1512 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button12.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1587 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button12alpha.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1586 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button13.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1586 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button13alpha.png
--rw-r--r--   0 sweaver    (501) staff       (20)     4194 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      803 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button3.png
--rw-r--r--   0 sweaver    (501) staff       (20)      822 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button4.png
--rw-r--r--   0 sweaver    (501) staff       (20)      621 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button5.png
--rw-r--r--   0 sweaver    (501) staff       (20)      605 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button6.png
--rw-r--r--   0 sweaver    (501) staff       (20)      822 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button7.png
--rw-r--r--   0 sweaver    (501) staff       (20)      822 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button8.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3873 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button9.png
--rw-r--r--   0 sweaver    (501) staff       (20)      695 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/check1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1525 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/check2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      162 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/empty.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/entry1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/entry2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     4018 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/focus.png
--rw-r--r--   0 sweaver    (501) staff       (20)     4181 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     4181 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     4181 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame_gap.png
--rw-r--r--   0 sweaver    (501) staff       (20)      163 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame_gap_top_end.png
--rw-r--r--   0 sweaver    (501) staff       (20)      162 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame_gap_top_start.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom_end.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom_start.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_left.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_left_end.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_left_start.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_right.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_right_end.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_right_start.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_top.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_top_end.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/gap_top_start.png
--rw-r--r--   0 sweaver    (501) staff       (20)      323 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/handle_vert_thumb.png
--rw-r--r--   0 sweaver    (501) staff       (20)      158 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/hline.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1427 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/htrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)      223 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/menu_selected.png
--rw-r--r--   0 sweaver    (501) staff       (20)      209 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/menu_shadow.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/menubar.png
--rw-r--r--   0 sweaver    (501) staff       (20)      144 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1766 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1133 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook3.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1754 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook4.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1113 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook5.png
--rw-r--r--   0 sweaver    (501) staff       (20)      180 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook_border.png
--rw-r--r--   0 sweaver    (501) staff       (20)      943 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1083 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     3279 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option_menu.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1797 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1355 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz2.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1796 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_vert1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      447 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/shadow1.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1061 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/shadow2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      482 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_horiz1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      353 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_hth1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      207 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_hth2.png
--rw-r--r--   0 sweaver    (501) staff       (20)      483 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_vert1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      311 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_vth1.png
--rw-r--r--   0 sweaver    (501) staff       (20)      192 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/slider_vth2.png
--rw-r--r--   0 sweaver    (501) staff       (20)    19898 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/theme.rc
--rw-r--r--   0 sweaver    (501) staff       (20)      173 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/vline.png
--rw-r--r--   0 sweaver    (501) staff       (20)     1318 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/vtrough.png
--rw-r--r--   0 sweaver    (501) staff       (20)      134 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/white.png
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/
--rw-r--r--   0 sweaver    (501) staff       (20)     2238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/128.cur
--rw-r--r--   0 sweaver    (501) staff       (20)     2238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/129.cur
--rw-r--r--   0 sweaver    (501) staff       (20)    12342 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/130.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/131.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/132.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     2238 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/132.cur
--rw-r--r--   0 sweaver    (501) staff       (20)    11958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/133.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1110 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/3000.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/333.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)    38454 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/400.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1224 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4000.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1222 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4001.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1222 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4002.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1222 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4003.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)    38454 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/401.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1286 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4011.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)    38454 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/402.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1222 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4020.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1466 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5000.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1478 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5001.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1466 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5002.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1478 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5003.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1464 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5004.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1432 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5005.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1314 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5006.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1464 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5007.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1266 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6000.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6001.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1178 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6002.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6003.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1310 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6004.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1304 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6005.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1324 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6006.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1298 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6007.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1312 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6008.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1246 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6009.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6010.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1308 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6011.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1226 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6012.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)      246 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6013.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)      246 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6014.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1336 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6016.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6017.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1258 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6018.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1314 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6019.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1294 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6020.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6021.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1314 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6022.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6030.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1260 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6031.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1318 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6032.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1330 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6033.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1318 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6034.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1314 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6035.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6036.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1282 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6040.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1316 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6041.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1226 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6042.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1326 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7000.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1308 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7001.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1296 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7002.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1286 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7003.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1294 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7004.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1300 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7005.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1270 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7010.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7011.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7012.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1258 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7013.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1246 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7014.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7020.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)     1334 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7050.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)   204862 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/desk.ico
--rw-r--r--   0 sweaver    (501) staff       (20)    91880 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/hyphy.bmp
--rw-r--r--   0 sweaver    (501) staff       (20)    69088 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/pthreadGC2.dll
--rw-r--r--   0 sweaver    (501) staff       (20)    86070 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/pthreadVC2.dll
--rw-r--r--   0 sweaver    (501) staff       (20)    10356 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/Win.rc
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)     6958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformButton.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    15026 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformButtonBar.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     6083 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformCheckBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     5558 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformLabel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    11842 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformPullDown.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     9125 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformSequencePane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    60118 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    22449 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformTextBox.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    20077 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformComponent.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    27696 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformGraphicPane.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    25331 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    22486 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatfromUtils.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/
--rw-r--r--   0 sweaver    (501) staff       (20)      959 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformButton.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1029 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformButtonBar.h
--rw-r--r--   0 sweaver    (501) staff       (20)      781 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformCheckbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)      958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformLabel.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1591 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformPullDown.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1654 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformTable.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1845 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformTextbox.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2644 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformButtonMenu.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1868 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformComponent.h
--rw-r--r--   0 sweaver    (501) staff       (20)     2778 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformGraphicPane.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4824 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformWindow.h
--rw-r--r--   0 sweaver    (501) staff       (20)    43645 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/pthread.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4910 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/sched.h
--rw-r--r--   0 sweaver    (501) staff       (20)     4739 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/include/semaphore.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/
--rw-r--r--   0 sweaver    (501) staff       (20)      709 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformBootsrapWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    15250 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformChartWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    16164 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformConsoleWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    38634 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformDataPanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)      637 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformDBWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     1922 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformGWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     4712 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformModelWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     9772 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformParameterTable.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    10669 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformPWindow.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    48283 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformTreePanel.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    13936 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformTWindow.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/
--rw-r--r--   0 sweaver    (501) staff       (20)    23530 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/batchfiles.list
--rw-r--r--   0 sweaver    (501) staff       (20)     4797 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/build.sh
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     3761 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/data/hiv.nuc
--rw-r--r--   0 sweaver    (501) staff       (20)     2055 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/F81.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      797 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/HKY85.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/Python/
--rw-r--r--   0 sweaver    (501) staff       (20)     3953 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/Python/BasicHyPhy.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/R/
--rw-r--r--   0 sweaver    (501) staff       (20)     4315 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Examples/R/BasicHyPhy.R
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/Python/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/Python/HyPhy/
--rw-r--r--   0 sweaver    (501) staff       (20)     2170 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/Python/HyPhy/__init__.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/R/
--rw-r--r--   0 sweaver    (501) staff       (20)    39161 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/R/HyPhy.R
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Link/
--rw-r--r--   0 sweaver    (501) staff       (20)    14450 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Link/THyPhy.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8815 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/Link/THyPhy.h
--rw-r--r--   0 sweaver    (501) staff       (20)     1188 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/README
--rw-r--r--   0 sweaver    (501) staff       (20)     3598 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/setup.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/
--rw-r--r--   0 sweaver    (501) staff       (20)   249527 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_py3.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   249527 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_python.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   100171 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_R.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/mains/
--rw-r--r--   0 sweaver    (501) staff       (20)    12925 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/mains/gtk.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    48912 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/mains/mac.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    25783 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/mains/unix.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    29309 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/mains/win.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/new/
--rw-r--r--   0 sweaver    (501) staff       (20)   102164 2017-12-11 15:17:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/bayesgraph.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    65762 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/bayesgraph2.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   114883 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/bgm.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)    71042 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/bgm2.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/new/include/
--rw-r--r--   0 sweaver    (501) staff       (20)     7135 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/include/bayesgraph.h
--rw-r--r--   0 sweaver    (501) staff       (20)     8202 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/include/bgm.h
--rw-r--r--   0 sweaver    (501) staff       (20)    27674 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/include/scfg.h
--rw-r--r--   0 sweaver    (501) staff       (20)    99243 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/new/scfg.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/ocl/
--rw-r--r--   0 sweaver    (501) staff       (20)    15170 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/ocl/opencl_kernels.cl
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/src/utils/
--rw-r--r--   0 sweaver    (501) staff       (20)    13348 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/src/utils/hyphyunixutils.cpp
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/tests/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/
--rwxr-xr-x   0 sweaver    (501) staff       (20)    14830 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_avllists.cpp
--rwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_avllists.h
--rwxr-xr-x   0 sweaver    (501) staff       (20)    12484 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_list.cpp
--rwxr-xr-x   0 sweaver    (501) staff       (20)      145 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_lists.h
--rwxr-xr-x   0 sweaver    (501) staff       (20)    14738 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_simplelists.cpp
--rwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_simplelists.h
--rw-r--r--   0 sweaver    (501) staff       (20)    38627 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_strings.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_strings.h
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/
--rw-r--r--   0 sweaver    (501) staff       (20)    35903 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/CodonAncestors.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    14184 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/LeafProbs.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    25160 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/NucAncestors.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    14926 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/NucRVAncestors.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BayesianGraphicalModels/
--rw-r--r--   0 sweaver    (501) staff       (20)    15356 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BayesianGraphicalModels/alarm.xml
--rw-r--r--   0 sweaver    (501) staff       (20)     4176 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BayesianGraphicalModels/TestBGM.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/
--rw-r--r--   0 sweaver    (501) staff       (20)  1722384 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/kernel.dump
--rw-r--r--   0 sweaver    (501) staff       (20)       32 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/Level1.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/Level2/
--rw-r--r--   0 sweaver    (501) staff       (20)       25 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/Level2/File1.bf
--rw-r--r--   0 sweaver    (501) staff       (20)       45 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/Level2/File2.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1408 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/TreeSplits.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/
--rw-r--r--   0 sweaver    (501) staff       (20)     1754 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/2.fas
--rw-r--r--   0 sweaver    (501) staff       (20)      590 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/2.prot
--rw-r--r--   0 sweaver    (501) staff       (20)        5 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/2.tree
--rw-r--r--   0 sweaver    (501) staff       (20)      375 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/5.fas
--rw-r--r--   0 sweaver    (501) staff       (20)     8291 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/CD2.nex
--rw-r--r--   0 sweaver    (501) staff       (20)   357257 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/fluHA.nex
--rw-r--r--   0 sweaver    (501) staff       (20)   362244 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/fluHA_codon.nex
--rw-r--r--   0 sweaver    (501) staff       (20)     4081 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HIVenvSweden.seq
--rw-r--r--   0 sweaver    (501) staff       (20)    11313 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HMM2_synthetic.fas
--rw-r--r--   0 sweaver    (501) staff       (20)    11313 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HMM4_synthetic.fas
--rw-r--r--   0 sweaver    (501) staff       (20)   677593 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/mtDNA.fas
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/
--rw-r--r--   0 sweaver    (501) staff       (20)     3706 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/RateHMM.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    14980 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/SmallNuc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    14562 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/SmallNucRel.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3213 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/TreeHMM.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/
--rw-r--r--   0 sweaver    (501) staff       (20)    51845 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/ClearConstraintsBug.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    77691 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/expModelCrash.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      197 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/LocalReferenceBug.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1547 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/ParseNexus.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/
--rw-r--r--   0 sweaver    (501) staff       (20)    42307 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex
--rw-r--r--   0 sweaver    (501) staff       (20)   314501 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.alternative.fit
--rw-r--r--   0 sweaver    (501) staff       (20)   314500 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.partitioned_descriptive.fit
--rw-r--r--   0 sweaver    (501) staff       (20)    25599 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.RELAX.json
--rw-r--r--   0 sweaver    (501) staff       (20)     3736 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.tre
--rw-r--r--   0 sweaver    (501) staff       (20)      295 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/wrapper.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/res/
--rw-r--r--   0 sweaver    (501) staff       (20)   113375 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/res/69genes.test.nex
--rw-r--r--   0 sweaver    (501) staff       (20)      107 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/unaryMinus.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/
--rw-r--r--   0 sweaver    (501) staff       (20)     1206 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/BS-REL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    18554 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/GTR_G_I.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    74958 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/IntermediateNucRel.bf
--rw-r--r--   0 sweaver    (501) staff       (20)   176502 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/ModelMixture.bf
--rw-r--r--   0 sweaver    (501) staff       (20)   302953 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/MultiplePartitions.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1484 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/NY.bf
--rw-r--r--   0 sweaver    (501) staff       (20)   143111 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/SmallNucRel.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Shared/
--rw-r--r--   0 sweaver    (501) staff       (20)      492 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Shared/REL_utils.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3346 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Shared/TestInstrumentation.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/
--rw-r--r--   0 sweaver    (501) staff       (20)    50376 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateCodon.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3022 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateNuc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)   181124 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateProtein.bf
--rw-r--r--   0 sweaver    (501) staff       (20)  3220152 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/LargeNuc.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    36022 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodon.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    36322 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodonLocal.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     2133 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/TwoSequenceTest.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SpecializedOptimizations/
--rw-r--r--   0 sweaver    (501) staff       (20)   354831 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SpecializedOptimizations/SingleSiteTemplate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)    67992 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/SpecializedOptimizations/SiteLikelihood.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Trickier/
--rw-r--r--   0 sweaver    (501) staff       (20)      897 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/Trickier/NonReversibleWithDynamicFrequencies.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/
--rw-r--r--   0 sweaver    (501) staff       (20)    16830 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/AllCommands.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     4647 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/BranchLength.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      713 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DeleteObject.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1339 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Differentiate.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      362 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DoSQL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1362 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Export.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1480 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetDataInfo.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     9970 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetString.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1577 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetURL.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     3653 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/HarvestFrequencies.bf
--rw-r--r--   0 sweaver    (501) staff       (20)      923 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/JSON.bf
--rw-r--r--   0 sweaver    (501) staff       (20)       49 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/RequireVersion.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/
--rw-r--r--   0 sweaver    (501) staff       (20)    12214 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/SCFG.ibf
--rw-r--r--   0 sweaver    (501) staff       (20)     2591 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/scfgG6c.bf
--rw-r--r--   0 sweaver    (501) staff       (20)     1453 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/small.txt
--rw-r--r--   0 sweaver    (501) staff       (20)    35241 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc.nex
--rw-r--r--   0 sweaver    (501) staff       (20)   180396 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc2.nex
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/
--rw-r--r--   0 sweaver    (501) staff       (20)  1091584 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/Chinook_Sqlite.sqlite
--rw-r--r--   0 sweaver    (501) staff       (20)     1261 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/TestTools.ibf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/tmp/
--rw-r--r--   0 sweaver    (501) staff       (20)        0 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/tmp/GetURL.txt
--rw-r--r--   0 sweaver    (501) staff       (20)     1096 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Type.bf
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/hyphy_python.egg-info/
--rw-r--r--   0 sweaver    (501) staff       (20)        1 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy_python.egg-info/dependency_links.txt
--rw-r--r--   0 sweaver    (501) staff       (20)      308 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy_python.egg-info/PKG-INFO
--rw-r--r--   0 sweaver    (501) staff       (20)    83870 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy_python.egg-info/SOURCES.txt
--rw-r--r--   0 sweaver    (501) staff       (20)       13 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/hyphy_python.egg-info/top_level.txt
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/Link/
--rw-r--r--   0 sweaver    (501) staff       (20)    14489 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/Link/THyPhy.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)     8827 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/Link/THyPhy.h
--rw-r--r--   0 sweaver    (501) staff       (20)       46 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/MANIFEST.in
--rw-r--r--   0 sweaver    (501) staff       (20)      308 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/PKG-INFO
--rw-r--r--   0 sweaver    (501) staff       (20)      273 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/README
--rw-r--r--   0 sweaver    (501) staff       (20)       38 2017-12-11 15:19:19.000000 hyphy-python-0.1.8/setup.cfg
--rw-r--r--   0 sweaver    (501) staff       (20)     4062 2017-12-11 15:18:26.000000 hyphy-python-0.1.8/setup.py
-drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2017-12-11 15:19:18.000000 hyphy-python-0.1.8/SWIGWrappers/
--rw-r--r--   0 sweaver    (501) staff       (20)   250687 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/SWIGWrappers/THyPhy_py3.cpp
--rw-r--r--   0 sweaver    (501) staff       (20)   249527 2017-12-08 20:53:56.000000 hyphy-python-0.1.8/SWIGWrappers/THyPhy_python.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/
+-rw-r--r--   0 sweaver    (501) staff       (20)      308 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/PKG-INFO
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/HyPhy/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2170 2015-11-08 23:32:25.000000 hyphy-python-0.1.9/HyPhy/__init__.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/res/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TreeAddIns/
+-rw-r--r--   0 sweaver    (501) staff       (20)      865 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TreeAddIns/Splits
+-rw-r--r--   0 sweaver    (501) staff       (20)     4101 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TreeAddIns/Tree Statistics
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6237 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/codon.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/
+-rw-r--r--   0 sweaver    (501) staff       (20)       65 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/Equal
+-rw-r--r--   0 sweaver    (501) staff       (20)      743 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/Estimated
+-rw-r--r--   0 sweaver    (501) staff       (20)      157 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/Observed In Data Set
+-rw-r--r--   0 sweaver    (501) staff       (20)      164 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/Observed In Partition
+-rw-r--r--   0 sweaver    (501) staff       (20)     2138 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/aa.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      467 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/nuc.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1834 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Codon
+-rw-r--r--   0 sweaver    (501) staff       (20)     2236 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 3 params.
+-rw-r--r--   0 sweaver    (501) staff       (20)      302 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Equal
+-rw-r--r--   0 sweaver    (501) staff       (20)     2314 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 9 params.
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/
+-rw-r--r--   0 sweaver    (501) staff       (20)      559 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta
+-rw-r--r--   0 sweaver    (501) staff       (20)     2033 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/General Discrete
+-rw-r--r--   0 sweaver    (501) staff       (20)      973 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Half Normal
+-rw-r--r--   0 sweaver    (501) staff       (20)      983 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta-Gamma
+-rw-r--r--   0 sweaver    (501) staff       (20)      546 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Lognormal
+-rw-r--r--   0 sweaver    (501) staff       (20)      392 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/2 Bin Discrete
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/
+-rw-r--r--   0 sweaver    (501) staff       (20)      129 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/Equal
+-rw-r--r--   0 sweaver    (501) staff       (20)    10410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/Estimated
+-rw-r--r--   0 sweaver    (501) staff       (20)      158 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/Observed In Data Set
+-rw-r--r--   0 sweaver    (501) staff       (20)      164 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/Observed In Partition
+-rw-r--r--   0 sweaver    (501) staff       (20)     1486 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/dinuc.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/
+-rw-r--r--   0 sweaver    (501) staff       (20)      779 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      806 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToConsole.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1119 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToChartWindow.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1093 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToTabFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      364 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/FromSQLFlatFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1370 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/DescriptiveStats.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2292 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToSQLFlatFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1478 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFrontierFastaFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2219 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFileFromPandit.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      984 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/HY_DBW_TemplateList
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/
+-rw-r--r--   0 sweaver    (501) staff       (20)      696 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/posteriors.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1571 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Most Likely Class Assignment
+-rw-r--r--   0 sweaver    (501) staff       (20)     1754 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Moments
+-rw-r--r--   0 sweaver    (501) staff       (20)      753 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Distribution
+-rw-r--r--   0 sweaver    (501) staff       (20)     1982 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Prior Moments
+-rw-r--r--   0 sweaver    (501) staff       (20)     2226 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Event Posteriors
+-rw-r--r--   0 sweaver    (501) staff       (20)     7062 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Profile Mean Clustering
+-rw-r--r--   0 sweaver    (501) staff       (20)     2232 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Mean Profile Plot
+-rw-r--r--   0 sweaver    (501) staff       (20)     2173 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Column Operations
+-rw-r--r--   0 sweaver    (501) staff       (20)      480 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Sort
+-rw-r--r--   0 sweaver    (501) staff       (20)     2548 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/K-Mean Clustering
+-rw-r--r--   0 sweaver    (501) staff       (20)     2354 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Select Cells By Value
+-rw-r--r--   0 sweaver    (501) staff       (20)     3177 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Contigency Table
+-rw-r--r--   0 sweaver    (501) staff       (20)     7009 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Poisson Mixture Fit
+-rw-r--r--   0 sweaver    (501) staff       (20)      560 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Running Sum
+-rw-r--r--   0 sweaver    (501) staff       (20)     3809 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Distribution Moments
+-rw-r--r--   0 sweaver    (501) staff       (20)     1344 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Covariance
+-rw-r--r--   0 sweaver    (501) staff       (20)      455 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/SingleColumn
+-rw-r--r--   0 sweaver    (501) staff       (20)     3746 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Complex Select Cells By Value
+-rw-r--r--   0 sweaver    (501) staff       (20)     2343 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/KH Resampler
+-rw-r--r--   0 sweaver    (501) staff       (20)     5473 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Gaussian Penalty Clustering
+-rw-r--r--   0 sweaver    (501) staff       (20)     3813 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Median Profile Plot
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2522 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/srs.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3267 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/sir.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1589 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/lhc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1095 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Select Cells By Index
+-rw-r--r--   0 sweaver    (501) staff       (20)      565 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Approximate_CDF
+-rw-r--r--   0 sweaver    (501) staff       (20)      617 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Populate Cells
+-rw-r--r--   0 sweaver    (501) staff       (20)     4135 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Linear Fit.orig
+-rw-r--r--   0 sweaver    (501) staff       (20)     2078 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Goodness of Fit
+-rw-r--r--   0 sweaver    (501) staff       (20)     1738 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Linear Fit
+-rw-r--r--   0 sweaver    (501) staff       (20)     2277 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Histogram
+-rw-r--r--   0 sweaver    (501) staff       (20)     2075 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Descriptive Statistics
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/
+-rw-r--r--   0 sweaver    (501) staff       (20)      804 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Echinoderm_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      782 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Blepharisma_Nuclear.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      762 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Yeast_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      786 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Mold_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)     1343 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Vertebratemtdna.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      800 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Flatworm_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      802 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Ascidian_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      807 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Invertebrate_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      799 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Euplotid_Nuclear.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      818 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Thraustochytrium_mtDNA.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      808 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Alt_Yeast_Nuclear.cod
+-rw-r--r--   0 sweaver    (501) staff       (20)      816 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Ciliate.cod
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/Nucleotide/
+-rw-r--r--   0 sweaver    (501) staff       (20)      585 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/Nucleotide/K2P
+-rw-r--r--   0 sweaver    (501) staff       (20)      586 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/Nucleotide/JC69
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/
+-rw-r--r--   0 sweaver    (501) staff       (20)    34336 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Jones.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    11447 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/EIAA.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2186 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Fitness.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    11493 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Dayhoff.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    65577 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/mtREV.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Binary/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1143 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Binary/F81.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6405 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/GY94_3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     6966 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/Lineage_MG94xHKY85.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5317 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     6785 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_HKY85x3_4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    13893 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94REVOmegaCF3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    11704 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    13590 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     6331 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xHKY85_3x4_2Rates.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl copy
+-rw-r--r--   0 sweaver    (501) staff       (20)    13510 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xTN93_3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    16141 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV_GDD.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5187 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2421 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/HKY85.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1908 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/F81.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2470 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/REV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      896 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/EFVEstimated.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2202 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/TrN.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     3137 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/REVBetaGamma.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/
+-rw-r--r--   0 sweaver    (501) staff       (20)    17241 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Sequential_Addition
+-rw-r--r--   0 sweaver    (501) staff       (20)     9261 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Exhaustive_Search
+-rw-r--r--   0 sweaver    (501) staff       (20)    16065 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Star_Decomposition
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2102 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/doNNISwap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2560 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/doSPRSwap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8954 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/branchSwappingFunctions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3069 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Neighbor_Joining
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/
+-rw-r--r--   0 sweaver    (501) staff       (20)      577 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/ListUserFunctions
+-rw-r--r--   0 sweaver    (501) staff       (20)      859 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/Tidbits
+-rw-r--r--   0 sweaver    (501) staff       (20)      820 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/ModelCounter
+-rw-r--r--   0 sweaver    (501) staff       (20)      326 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/LRT
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2768 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/SimulateAndTabDN_DS
+-rw-r--r--   0 sweaver    (501) staff       (20)     1240 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ExpsPerDirection
+-rw-r--r--   0 sweaver    (501) staff       (20)     7047 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/PredictivePosteriorP
+-rw-r--r--   0 sweaver    (501) staff       (20)     1650 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/LocaldNdS
+-rw-r--r--   0 sweaver    (501) staff       (20)     7362 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ConvergentAndParallel
+-rw-r--r--   0 sweaver    (501) staff       (20)      990 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/PartitionBranchesByClasses
+-rw-r--r--   0 sweaver    (501) staff       (20)     7682 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/AAMutationCounter
+-rw-r--r--   0 sweaver    (501) staff       (20)      637 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/CopyBranchLengths
+-rw-r--r--   0 sweaver    (501) staff       (20)      993 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/dS and dN factors
+-rw-r--r--   0 sweaver    (501) staff       (20)     1511 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ModelFitSummaryAA
+-rw-r--r--   0 sweaver    (501) staff       (20)     5100 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ColorPSTree
+-rw-r--r--   0 sweaver    (501) staff       (20)     1011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ModelFitSummary
+-rw-r--r--   0 sweaver    (501) staff       (20)      934 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/FilterAssignments
+-rw-r--r--   0 sweaver    (501) staff       (20)     1850 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/TreeLengthConstraint
+-rw-r--r--   0 sweaver    (501) staff       (20)     5024 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/Multiclass DN DS inference
+-rw-r--r--   0 sweaver    (501) staff       (20)     1058 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/RNARateMatrix
+-rw-r--r--   0 sweaver    (501) staff       (20)    11071 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/CodonMutationToTreeMapper.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10154 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/InferredAASubstitutionsCounter
+-rw-r--r--   0 sweaver    (501) staff       (20)     4422 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/DashPSTree
+-rw-r--r--   0 sweaver    (501) staff       (20)     5382 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/dNanddSTrees.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      907 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/SimulateFromLF
+-rw-r--r--   0 sweaver    (501) staff       (20)      962 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/AAContent
+-rw-r--r--   0 sweaver    (501) staff       (20)     1014 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/GenBankSequences
+-rw-r--r--   0 sweaver    (501) staff       (20)     2242 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/MeanPairwiseDivergence
+-rw-r--r--   0 sweaver    (501) staff       (20)     2301 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/BranchLengthCI
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/
+-rw-r--r--   0 sweaver    (501) staff       (20)      503 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/ChooseALF.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3617 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/MappersHelpAA.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4912 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/MappersHelp.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    17476 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/RecombinationProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2421 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/CountSubstitutions
+-rw-r--r--   0 sweaver    (501) staff       (20)     7494 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/CodonMutationToTreeMapper
+-rw-r--r--   0 sweaver    (501) staff       (20)     1056 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/ExportLikelihoodFunction
+-rw-r--r--   0 sweaver    (501) staff       (20)     2593 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/MapSubstitutions
+-rw-r--r--   0 sweaver    (501) staff       (20)      143 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/BatchFileByURL
+-rw-r--r--   0 sweaver    (501) staff       (20)     4399 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/MeanPairwiseDivergenceSubset
+-rw-r--r--   0 sweaver    (501) staff       (20)      664 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/UserAddins/SimulateFromLF
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/ibfs/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1154 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/ibfs/char_colors.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     5091 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Character Plot
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/TBD/
+-rw-r--r--   0 sweaver    (501) staff       (20)    11228 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/TBD/Character Plot By Sequence
+-rw-r--r--   0 sweaver    (501) staff       (20)     3863 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Compare Subsets
+-rw-r--r--   0 sweaver    (501) staff       (20)    11533 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Character Plot Two
+-rw-r--r--   0 sweaver    (501) staff       (20)     5719 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Sequence Plot
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8855 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_CMS_Aux.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7512 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClock.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    38053 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSResultProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    34882 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARD.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MaxChi2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5630 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LocalMolClock.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4634 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimilarityPlot.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7196 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRateL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12603 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    18602 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClock.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    11148 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19567 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5934 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SiteRates.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5308 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SSRatesTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7803 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GateauxMR.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    30183 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RELAX.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    17424 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MGvsGY.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseDNDS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2760 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_dNdS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7194 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relrateBootstrapL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7859 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/distanceRMethodNPBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5504 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRatio.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)       15 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/last.date
+-rw-r--r--   0 sweaver    (501) staff       (20)    17567 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonUsageBias.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3530 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRate.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19047 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MEDS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    26791 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    27326 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    16520 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DatedTipsMolecularClock.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5901 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_k_means.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    11442 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LocalBranchSiteTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10649 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimator.ibf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/
+-rw-r--r--   0 sweaver    (501) staff       (20)      327 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M1.def
+-rw-r--r--   0 sweaver    (501) staff       (20)      490 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M2.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     5011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      558 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M3.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     3921 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5319 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGenerator.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      611 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_synvar.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     8503 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94GY94xREV_PARRIS_syn3.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4608 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate_Multirate.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      521 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     8050 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/GY94.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      532 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma1.def
+-rw-r--r--   0 sweaver    (501) staff       (20)      929 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2+Inv.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     3582 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGeneratorNoPS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      758 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_syn3.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     4502 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relratioBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonMF.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3081 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/doNNISwap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4839 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_sampler.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      180 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimatorCounter.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    25639 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodonProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19257 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARDProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7969 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TreeCorrelationCoefficients.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7823 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LRTRecombTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    15293 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1434 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_MSCOneStep.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10783 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TopologySearch.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    32201 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NielsenYang.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      169 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodon.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    20678 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TreeTools.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4529 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_BMS_Aux.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6946 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_MFReader_.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    24628 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NucModelCompare.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    29435 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5987 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DistanceMatrix_Splits.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14145 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper2_mf.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)      511 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/globalChecker.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3040 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BivariateCodonRateAnalysis.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      447 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/readIndexFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19432 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGEmulator_MF.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2857 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/queryTree.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22355 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis_MF.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5283 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimpleMutationCounter.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8139 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/KHTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19450 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/F_ST.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    21840 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARecomb.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      933 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    29296 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparison.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      352 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_lfprofile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2321 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StripStopCodons.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3199 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CleanGaps.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/
+-rw-r--r--   0 sweaver    (501) staff       (20)      867 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/PCH
+-rw-r--r--   0 sweaver    (501) staff       (20)     1529 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HKY85.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    27857 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      549 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAEqualInput
+-rw-r--r--   0 sweaver    (501) staff       (20)     5584 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61multiple.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4155 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F+omega.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2240 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAAFreq.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9572 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94custom.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    28123 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1256 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      866 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/S4
+-rw-r--r--   0 sweaver    (501) staff       (20)     3060 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/reducedREV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     3755 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84P.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/
+-rw-r--r--   0 sweaver    (501) staff       (20)    37977 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECM
+-rw-r--r--   0 sweaver    (501) staff       (20)    38029 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECMu
+-rw-r--r--   0 sweaver    (501) staff       (20)    28346 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     3749 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAMuse95.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2735 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/CF3x4.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3487 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16SvH.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9771 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customCF3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    11062 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94x2.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    34672 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.mdl
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3507 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVBetween
+-rw-r--r--   0 sweaver    (501) staff       (20)     6408 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/VT
+-rw-r--r--   0 sweaver    (501) staff       (20)     8091 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/JTT
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtREV24
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    36640 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LCAP
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/Dayhoff
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtMAM
+-rw-r--r--   0 sweaver    (501) staff       (20)     6408 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/BLOSUM62
+-rw-r--r--   0 sweaver    (501) staff       (20)    10147 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/modellist.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6408 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/cpREV
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/IAV
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/WAG
+-rw-r--r--   0 sweaver    (501) staff       (20)     8010 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/H5N1
+-rw-r--r--   0 sweaver    (501) staff       (20)     6408 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/MtArt
+-rw-r--r--   0 sweaver    (501) staff       (20)     6410 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/rtREV
+-rw-r--r--   0 sweaver    (501) staff       (20)     6408 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LG
+-rw-r--r--   0 sweaver    (501) staff       (20)     3233 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVWithin
+-rw-r--r--   0 sweaver    (501) staff       (20)     1584 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM+Freqs.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5499 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAFreqs.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9582 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customF1x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1656 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/STGRM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9371 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/custm4x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1191 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81_binary.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2386 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2179 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94w9.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      809 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV
+-rw-r--r--   0 sweaver    (501) staff       (20)     5409 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAUserFreqs.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4305 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+MLFREQS.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4153 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      867 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Default
+-rw-r--r--   0 sweaver    (501) staff       (20)     1259 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5119 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/UniversalCode.def
+-rw-r--r--   0 sweaver    (501) staff       (20)    15997 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2727 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.dat
+-rw-r--r--   0 sweaver    (501) staff       (20)    28569 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     6441 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94with9freqs.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4634 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1672 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GRM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    34043 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    35087 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1422 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/K2P.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4357 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA_empirical.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    10986 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/models.lst
+-rw-r--r--   0 sweaver    (501) staff       (20)     3949 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1175 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69_binary.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      597 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     8013 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MEC.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1405 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/190
+-rw-r--r--   0 sweaver    (501) staff       (20)     3522 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1636 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAA.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     7177 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94customF3x4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      800 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9171 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/LCAP.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1878 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/fitness.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    34009 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones_F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    10677 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Yang2000Distributions.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     5828 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    16378 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      785 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV_1
+-rw-r--r--   0 sweaver    (501) staff       (20)     1564 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/TrN.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    28224 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      355 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween+F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     2688 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwEX.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1513 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/K3ST.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5496 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wEX.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    28734 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     3356 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwAA.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1533 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGFreqsEstimator.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10198 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineHM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     6082 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAA.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    34528 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     9067 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customFreqs.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4985 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7115 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/BranchSiteTemplate.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1878 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      659 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters3.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    16966 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/chooseGeneticCode.def
+-rw-r--r--   0 sweaver    (501) staff       (20)      546 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters2.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5353 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      490 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4072 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)      351 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin+F.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1739 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1480 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16A
+-rw-r--r--   0 sweaver    (501) staff       (20)    10995 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineGamma.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)      916 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAF81
+-rw-r--r--   0 sweaver    (501) staff       (20)      660 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters5.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     4154 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1699 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters4.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1474 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     5854 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)    17630 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb-2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8321 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimmondsAI.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5205 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentProt.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2705 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6430 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlidingWindowAnalysis.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    26595 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressure.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2845 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/doSPRSwap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12310 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestBranchDNDS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10172 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relrateBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9012 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison-2parts.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5743 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AAModelComparison.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8282 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Gateaux.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      958 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MergeSequences.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    39439 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSiteREL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4409 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper3.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10610 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ClusterAnalysis.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9153 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TopologySearchConstrained.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14350 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC_Binary.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9952 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5893 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/heuristicMethodNPBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    28108 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MEME_mf.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1348 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      880 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/postprocessors.lst
+-rw-r--r--   0 sweaver    (501) staff       (20)     5995 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/molclockBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    28200 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressureIVL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5904 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MolClockAllRoots.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4136 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NeighborJoining.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10529 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetectionMF.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/
+-rw-r--r--   0 sweaver    (501) staff       (20)     5481 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10126 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_3.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    13689 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_tools.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4104 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_4.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      888 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_1.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6078 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_5.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    13478 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper2.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2276 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LZ_Complexity.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    13759 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StarDecomposition.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    26094 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonModelCompare.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    21208 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PartitionRateComparison.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2390 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPSreader.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     9958 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/simpleBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1215 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_counting.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12009 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchClassDNDS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9879 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRatio.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    23991 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestClade.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5727 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/WebUpdate.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12964 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessorM.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10851 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SelectionLRT.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2013 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/partitionSequences.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)      966 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MergeSites.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14930 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/454.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      359 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_npbs.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22914 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper1.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9316 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/WANC.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    15337 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/YangNielsenBranchSite2005.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    27567 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonPartitions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1090 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5357 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CleanStopCodons.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1285 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonData.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3903 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_variance.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7993 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DistanceMatrix.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    20242 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorBranch.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3227 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MolecularClock.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    13154 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGASimProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1647 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/binomial.ibf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/
+-rw-r--r--   0 sweaver    (501) staff       (20)     9016 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/srs.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1237 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/lhc_supp.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3267 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/sir.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6523 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/lhc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      661 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_ancestors.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    15352 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ClusterByDistanceRange.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2436 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlidingNucWindow.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    20586 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSiteRELMultiModel.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8889 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AddABias.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1549 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/UpperBound.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GUI/
+-rw-r--r--   0 sweaver    (501) staff       (20)       17 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GUI/crayolaColors.def
+-rw-r--r--   0 sweaver    (501) staff       (20)    11476 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4353 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper4.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    56606 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PositiveSelectionLI.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4667 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StrandGRMTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8954 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/branchSwappingFunctions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3707 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_support.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    51307 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentTop75.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9107 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ReduceDataSetMatrix.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9696 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/distanceMethodNPBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    18761 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGIvL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9281 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BS2007.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     8080 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodonShared.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)      868 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1294 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SplitSequencesByPattern.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      324 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_pbs.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2989 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_sns.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    17285 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DirectionalREL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14633 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DirectionalREL_MF.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    20444 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/bayesgraph.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10067 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSwap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    18886 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA_1.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    11098 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC_kernel.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)    42655 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PARRIS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1396 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_saveResults.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1794 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PartitionDataFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    15486 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SequentialAddition.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)      661 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeDiNucData.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    21748 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis_CompareDS.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12219 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonBivariateRateProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    11689 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARD_GA_CHC.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5622 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SequentialAddition.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    19136 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNuc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22782 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BUSTED.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    30660 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPositiveSelection.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22326 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RateClassCounter.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    13594 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/files.lst
+-rw-r--r--   0 sweaver    (501) staff       (20)     1545 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_covariance.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7847 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BGM.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6300 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LHT.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    25244 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BUSTED-SRV.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4441 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/categoryEcho.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)       99 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Phylohandbook.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      438 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/selectModelParameters.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/
+-rw-r--r--   0 sweaver    (501) staff       (20)      530 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC
+-rw-r--r--   0 sweaver    (501) staff       (20)     1925 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN93_RV
+-rw-r--r--   0 sweaver    (501) staff       (20)     1802 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_codon
+-rw-r--r--   0 sweaver    (501) staff       (20)      426 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_binary
+-rw-r--r--   0 sweaver    (501) staff       (20)     1236 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/T3P
+-rw-r--r--   0 sweaver    (501) staff       (20)      478 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance
+-rw-r--r--   0 sweaver    (501) staff       (20)     9815 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/CodonToolsMain.def
+-rw-r--r--   0 sweaver    (501) staff       (20)      779 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ
+-rw-r--r--   0 sweaver    (501) staff       (20)     2554 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN93
+-rw-r--r--   0 sweaver    (501) staff       (20)      797 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC_RV
+-rw-r--r--   0 sweaver    (501) staff       (20)      639 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools2.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     3554 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Nei_Gojobori
+-rw-r--r--   0 sweaver    (501) staff       (20)     1330 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN84
+-rw-r--r--   0 sweaver    (501) staff       (20)     1300 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/K2P_RV
+-rw-r--r--   0 sweaver    (501) staff       (20)      303 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools.def
+-rw-r--r--   0 sweaver    (501) staff       (20)      663 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC_MH
+-rw-r--r--   0 sweaver    (501) staff       (20)     3755 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Modified_Nei_Gojobori
+-rw-r--r--   0 sweaver    (501) staff       (20)     1011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/K2P
+-rw-r--r--   0 sweaver    (501) staff       (20)     2090 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ_FR
+-rw-r--r--   0 sweaver    (501) staff       (20)      564 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_aa
+-rw-r--r--   0 sweaver    (501) staff       (20)      648 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/JC69
+-rw-r--r--   0 sweaver    (501) staff       (20)    37032 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SampleProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7392 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SiteRates2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    85186 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignShared.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1893 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_tipDater.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1615 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignment.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7623 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper1_mf.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9437 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SandNSAmbigs.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    23306 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGEmulator.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7298 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Gateaux2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2661 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dSdNTreeTools.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7411 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRate.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9486 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Plato.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9922 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SubtreeSelectionComparison.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1234 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_viewResults.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    64552 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetection.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1662 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonDataMPI.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    23831 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPositiveSelectionPooled.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/
+-rw-r--r--   0 sweaver    (501) staff       (20)    14665 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/estimators.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3813 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9533 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/parameters.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4691 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/rate_variation.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7701 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/model_functions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10300 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/frequencies.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1582 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/terms.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2291 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6272 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/MG_REV.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2224 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/GTR.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6190 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/IOFunctions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4161 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/UtilityFunctions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9512 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FitnessAAModels.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10295 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestCladeMeans.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     7277 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNucShared.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2240 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ConvertDataFile.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22019 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5724 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseSiteDiversity.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5020 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonToProtein.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1194 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/WriteDelimitedFiles.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    51558 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/PS_Plotters.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    22537 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/GrabBag.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5349 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREVMLFreqs.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4505 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/DBTools.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1176 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/TreeFunctions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3190 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREV.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    20471 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/HXB2Mapper.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12199 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/PostScript.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2773 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/DescriptiveStatistics.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    12371 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/CoalescentPostProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1814 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/ProbabilityDistributions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    11502 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/ReadDelimitedFiles.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     6228 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/NJ.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2716 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/BranchLengthFitters.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    23866 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/AncestralMapper.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1667 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/CodonTools.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2617 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/MPITools.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10597 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorAAProcessor.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4025 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/chooseDistanceFormula.def
+-rw-r--r--   0 sweaver    (501) staff       (20)     1768 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_PCA.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/res/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)    10605 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/data/integrase_BDA.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)    11176 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/data/p51.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)     4680 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/data/brown.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)     4222 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/res/data/p51.aa
+-rw-r--r--   0 sweaver    (501) staff       (20)    23928 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/CMakeLists.txt
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/CMakeWin32/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3499 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/CMakeWin32/CMakeLists.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)     1419 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/LICENSE
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/cmake/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1070 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/cmake/cmake_uninstall.cmake.in
+-rw-r--r--   0 sweaver    (501) staff       (20)     2829 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/cmake/FindOpenCL.cmake
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/tests/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BayesianGraphicalModels/
+-rw-r--r--   0 sweaver    (501) staff       (20)    15356 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BayesianGraphicalModels/alarm.xml
+-rw-r--r--   0 sweaver    (501) staff       (20)     4176 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BayesianGraphicalModels/TestBGM.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1408 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/TreeSplits.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/Level2/
+-rw-r--r--   0 sweaver    (501) staff       (20)       25 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/Level2/File1.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)       45 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/Level2/File2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)       32 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/Level1.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)  1722384 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/kernel.dump
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/
+-rw-r--r--   0 sweaver    (501) staff       (20)    25160 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/NucAncestors.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14184 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/LeafProbs.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14926 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/NucRVAncestors.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    35903 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/CodonAncestors.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/res/
+-rw-r--r--   0 sweaver    (501) staff       (20)   113375 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/res/69genes.test.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)      107 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/unaryMinus.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    51845 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/ClearConstraintsBug.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    77691 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/expModelCrash.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      197 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/LocalReferenceBug.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/
+-rw-r--r--   0 sweaver    (501) staff       (20)    42307 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)   314500 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.partitioned_descriptive.fit
+-rw-r--r--   0 sweaver    (501) staff       (20)   314501 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.alternative.fit
+-rw-r--r--   0 sweaver    (501) staff       (20)      295 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/wrapper.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3736 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.tre
+-rw-r--r--   0 sweaver    (501) staff       (20)    25599 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.RELAX.json
+-rw-r--r--   0 sweaver    (501) staff       (20)     1547 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/ParseNexus.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/
+-rw-r--r--   0 sweaver    (501) staff       (20)    16830 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/AllCommands.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1339 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Differentiate.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/
+-rw-r--r--   0 sweaver    (501) staff       (20)  1091584 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/Chinook_Sqlite.sqlite
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/
+-rw-r--r--   0 sweaver    (501) staff       (20)    12214 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/SCFG.ibf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1453 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/small.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)     2591 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/scfgG6c.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   180396 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc2.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)    35241 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)      362 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DoSQL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)       49 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/RequireVersion.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9970 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetString.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4647 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/BranchLength.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      923 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/JSON.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1480 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetDataInfo.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3653 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/HarvestFrequencies.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1577 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetURL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      713 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DeleteObject.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1096 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Type.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1362 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Export.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/tmp/
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/tmp/GetURL.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)     1261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/TestTools.ibf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Shared/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3346 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Shared/TestInstrumentation.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      492 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Shared/REL_utils.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1206 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/BS-REL.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    18554 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/GTR_G_I.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   176502 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/ModelMixture.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   302953 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/MultiplePartitions.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    74958 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/IntermediateNucRel.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1484 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/NY.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   143111 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/SmallNucRel.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/
+-rw-r--r--   0 sweaver    (501) staff       (20)    50376 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateCodon.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3022 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateNuc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    36022 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodon.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)  3220152 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/LargeNuc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2133 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/TwoSequenceTest.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    36322 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodonLocal.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   181124 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateProtein.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Trickier/
+-rw-r--r--   0 sweaver    (501) staff       (20)      897 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/Trickier/NonReversibleWithDynamicFrequencies.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/
+-rw-r--r--   0 sweaver    (501) staff       (20)    14980 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/SmallNuc.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3213 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/TreeHMM.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3706 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/RateHMM.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    14562 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/SmallNucRel.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4081 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HIVenvSweden.seq
+-rw-r--r--   0 sweaver    (501) staff       (20)        5 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/2.tree
+-rw-r--r--   0 sweaver    (501) staff       (20)     1754 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/2.fas
+-rw-r--r--   0 sweaver    (501) staff       (20)    11313 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HMM4_synthetic.fas
+-rw-r--r--   0 sweaver    (501) staff       (20)      375 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/5.fas
+-rw-r--r--   0 sweaver    (501) staff       (20)   357257 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/fluHA.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)      590 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/2.prot
+-rw-r--r--   0 sweaver    (501) staff       (20)    11313 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HMM2_synthetic.fas
+-rw-r--r--   0 sweaver    (501) staff       (20)   362244 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/fluHA_codon.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)     8291 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/CD2.nex
+-rw-r--r--   0 sweaver    (501) staff       (20)   677593 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/mtDNA.fas
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SpecializedOptimizations/
+-rw-r--r--   0 sweaver    (501) staff       (20)    67992 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SpecializedOptimizations/SiteLikelihood.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   354831 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/hbltests/SpecializedOptimizations/SingleSiteTemplate.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/
+-rwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_avllists.h
+-rwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_simplelists.h
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_strings.h
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    14738 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_simplelists.cpp
+-rwxr-xr-x   0 sweaver    (501) staff       (20)      145 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_lists.h
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    14830 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_avllists.cpp
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    12484 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_list.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    38627 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_strings.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/
+-rw-r--r--   0 sweaver    (501) staff       (20)  5143688 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c
+-rw-r--r--   0 sweaver    (501) staff       (20)   111311 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/shell.c
+-rw-r--r--   0 sweaver    (501) staff       (20)   353468 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    26110 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3ext.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/
+-rw-r--r--   0 sweaver    (501) staff       (20)      551 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/FrameworkTarget.xcconfig
+-rw-r--r--   0 sweaver    (501) staff       (20)      993 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/ReleaseProject.xcconfig
+-rw-r--r--   0 sweaver    (501) staff       (20)     1199 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/General.xcconfig
+-rw-r--r--   0 sweaver    (501) staff       (20)      238 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/TestTarget.xcconfig
+-rw-r--r--   0 sweaver    (501) staff       (20)      983 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/DebugProject.xcconfig
+-rw-r--r--   0 sweaver    (501) staff       (20)      587 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/StaticLibraryTarget.xcconfig
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1010 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/Info.plist
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2270 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2354 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/runtests.sh
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/
+-rw-r--r--   0 sweaver    (501) staff       (20)    16060 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     2669 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)      846 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/Info.plist
+-rw-r--r--   0 sweaver    (501) staff       (20)     2307 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.cc
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2587 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/runtests.sh
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4536 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/versiongenerate.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/
+-rw-r--r--   0 sweaver    (501) staff       (20)    50972 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/project.pbxproj
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    13998 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/install-sh
+-rw-r--r--   0 sweaver    (501) staff       (20)   283680 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/ltmain.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     1841 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.h.in
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    44826 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.guess
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    20334 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/depcomp
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    10346 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/missing
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    35454 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.sub
+-rw-r--r--   0 sweaver    (501) staff       (20)     2574 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/configure.ac
+-rw-r--r--   0 sweaver    (501) staff       (20)     9120 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CMakeLists.txt
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8580 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_main.cbproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     1865 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_all.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    10486 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.cbproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     8691 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_unittest.cbproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     2008 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.groupproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     1993 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_link.cc
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4515 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test-md.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     3508 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     2432 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.sln
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4009 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest-md.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     3371 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4003 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4509 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     3374 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.vcproj
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     2456 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.sln
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     3514 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main-md.vcproj
+-rw-r--r--   0 sweaver    (501) staff       (20)     1475 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/LICENSE
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/
+-rw-r--r--   0 sweaver    (501) staff       (20)     9783 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-listener_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    77378 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_pred_impl_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    39094 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-port_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3306 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3576 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test_.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    14580 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest.py
+-rw-r--r--   0 sweaver    (501) staff       (20)    28164 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_golden_lin.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)     5302 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-message_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     4710 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1888 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_main_unittest.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     2480 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     4911 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     7339 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     6606 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_environment_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     6143 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     9641 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_stress_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3679 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_ex_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1732 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/production.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile1_test_.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     5856 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    12549 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    21261 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     2209 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_prod_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     7282 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-test-part_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    43236 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    13207 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-unittest-api_test.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    10812 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_test_utils.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     8193 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_repeat_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    32438 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2251 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_all_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3564 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest_.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     9901 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     4772 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_premature_exit_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     4125 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-linked_ptr_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2011 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile2_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2343 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9250 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-tuple_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    49588 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-printers_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    23653 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-filepath_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2447 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_no_test_unittest.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     5340 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfiles_test.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     2485 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.h
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    12005 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     2888 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3104 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2131 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     8919 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test_.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     8876 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_test_utils.py
+-rw-r--r--   0 sweaver    (501) staff       (20)    33346 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2172 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/production.h
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     5766 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     3263 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest_.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)   239177 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2221 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_sole_header_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1921 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test_.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     6515 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     7938 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-options_test.cc
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     3487 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test.py
+-rw-r--r--   0 sweaver    (501) staff       (20)     2059 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test2_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    11369 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2884 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test2_test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3444 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_ex_test.cc
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/cmake/
+-rw-r--r--   0 sweaver    (501) staff       (20)     9548 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/cmake/internal_utils.cmake
+-rwxr-xr-x   0 sweaver    (501) staff       (20)   564464 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/configure
+-rw-r--r--   0 sweaver    (501) staff       (20)     6645 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CHANGES
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/
+-rw-r--r--   0 sweaver    (501) staff       (20)    11523 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-death-test.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9952 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-spi.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8101 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-linked_ptr.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6968 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-string.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9226 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h.pump
+-rw-r--r--   0 sweaver    (501) staff       (20)    13429 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-death-test-internal.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9317 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h.pump
+-rw-r--r--   0 sweaver    (501) staff       (20)    68796 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-port.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    44145 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-internal.h
+-rw-r--r--   0 sweaver    (501) staff       (20)   192176 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    24191 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util.h
+-rw-r--r--   0 sweaver    (501) staff       (20)   185666 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9603 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-filepath.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    28223 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9416 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h.pump
+-rw-r--r--   0 sweaver    (501) staff       (20)     9186 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-message.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    75864 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    10242 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-typed-test.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    15145 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_pred_impl.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2324 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_prod.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    18796 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h.pump
+-rw-r--r--   0 sweaver    (501) staff       (20)     6509 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-test-part.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    88434 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    31609 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-printers.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1765 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest_main.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)   830563 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest.h
+-rw-r--r--   0 sweaver    (501) staff       (20)   354360 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest-all.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    16090 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/README
+-rw-r--r--   0 sweaver    (501) staff       (20)     9739 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/Makefile.am
+-rw-r--r--   0 sweaver    (501) staff       (20)     1358 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CONTRIBUTORS
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8989 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample6_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     5351 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample3_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2083 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5951 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample9_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     5053 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample10_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     6590 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample5_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2298 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     4072 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/prime_tables.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5365 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample3-inl.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2502 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3926 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     5099 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample7_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3006 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1927 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1909 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     5129 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1_unittest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1937 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6944 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample8_unittest.cc
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    23673 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/pump.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)     8813 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/fuse_gtest_files.py
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    10087 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/gtest-config.in
+-rwxr-xr-x   0 sweaver    (501) staff       (20)    21986 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/gen_gtest_pred_impl.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/
+-rw-r--r--   0 sweaver    (501) staff       (20)      690 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltversion.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)   287004 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/libtool.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)    12347 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltoptions.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)     4372 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltsugar.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)     3217 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/gtest.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)    13302 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/acx_pthread.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)     6126 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/lt~obsolete.m4
+-rw-r--r--   0 sweaver    (501) staff       (20)    59044 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/Makefile.in
+-rw-r--r--   0 sweaver    (501) staff       (20)    43769 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/aclocal.m4
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4159 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-test-part.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)   184142 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1765 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest_main.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    46465 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-internal-inl.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    50949 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-death-test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    27466 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-port.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    12275 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-printers.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3762 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-typed-test.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2161 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-all.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)    14238 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-filepath.cc
+-rw-r--r--   0 sweaver    (501) staff       (20)     3851 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/contrib/cl2hdr.c
+-rw-r--r--   0 sweaver    (501) staff       (20)     2204 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/README.md
+-rw-r--r--   0 sweaver    (501) staff       (20)      415 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/.gitignore
+-rw-r--r--   0 sweaver    (501) staff       (20)      243 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/package.json
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/BatchLanguage/
+-rw-r--r--   0 sweaver    (501) staff       (20)      860 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/BatchLanguage/profile_test.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1490 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/BatchLanguage/MatrixIndexing.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2911 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint1.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1491 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/shared.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2274 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint3.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3773 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/data/hiv.seq
+-rw-r--r--   0 sweaver    (501) staff       (20)     3411 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint2.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3819 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/ParametricBootstrap.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4028 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/PBootstrapHetRates.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5061 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/RelativeRatePBS.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3762 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/data/hiv.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1436 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Simulation/data/3.seq
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2406 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/REVshared.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1958 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/JC69.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2115 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/K2Pshared.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2066 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/K2P.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2317 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/HKY85shared.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2182 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/REV.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2942 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/Non-Rev.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3761 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/data/hiv.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2055 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/F81.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2162 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/HKY85.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2739 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/HKY852blocks2models.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     2610 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/HKY852blocks.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)    13602 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/data/actin2.flt
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4797 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/HKY85relratio.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3660 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81relrate.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5741 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/HKY85relrate.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3800 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81relratio.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3534 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/MolecularClockHKY85.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     4824 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81K81uf_relratio.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2067 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/aspectrin2.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1607 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/aspectrin1.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)    22349 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/molclock.seq
+-rw-r--r--   0 sweaver    (501) staff       (20)     1436 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/3.seq
+-rw-r--r--   0 sweaver    (501) staff       (20)     3872 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/MolecularClockF81.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/
+-rw-r--r--   0 sweaver    (501) staff       (20)      614 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/displayFunction.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)    10367 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions2.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     1617 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions3.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     9290 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions+MLE.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)     5649 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1634 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/Categories/data/aspectrin.nuc
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3527 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/ExonIntron.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/Models/
+-rw-r--r--   0 sweaver    (501) staff       (20)      189 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/Models/EI.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     3246 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/Models/MG94x2.mdl
+-rw-r--r--   0 sweaver    (501) staff       (20)     1925 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/aa.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2982 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/ubiq.flt
+-rw-r--r--   0 sweaver    (501) staff       (20)      968 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/stewart.aa
+-rw-r--r--   0 sweaver    (501) staff       (20)     1147 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/3.seq
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/scripts/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2195 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/buildMinGWFromSVN.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     5703 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/gtk_build.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     2619 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/build_mingw_MEGA.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     3440 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/build_mingw_gui.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)    11424 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/build.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     2449 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/build_mingw.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)      302 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/intelCCbuild.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     2398 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/scripts/buildFromSVN.sh
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/installers/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/installers/Win/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4544 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/installers/Win/hyphy.nsi
+-rw-r--r--   0 sweaver    (501) staff       (20)     1432 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/installers/Win/license.rtf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/
+-rw-r--r--   0 sweaver    (501) staff       (20)  2146965 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/Disk Image
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/
+-rw-r--r--   0 sweaver    (501) staff       (20)    59967 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/Preview.jpg
+-rw-r--r--   0 sweaver    (501) staff       (20)   183895 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/installers/Mac/DMG.key
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/help/
+-rw-r--r--   0 sweaver    (501) staff       (20)  1058637 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/help/Getting Started With HyPhy.pdf
+-rw-r--r--   0 sweaver    (501) staff       (20)   966666 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/help/SelectionAnalyses.pdf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/help/Commands/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4309 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/help/Commands/query.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)   139264 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/help/Commands/reference.sql
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/src/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/core/
+-rw-r--r--   0 sweaver    (501) staff       (20)    12941 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/classes.cp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2532 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/_hyExecutionContext.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    19891 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/operation.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    68320 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/parser2.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   108848 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/calcnode2.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    37397 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/variablecontainer.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   213854 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/site.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    59844 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/batchlanruntime.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    12778 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/error.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    72077 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/fisher_exact.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     4335 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/avllistx.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    62152 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/strings.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8893 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/formula.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3319 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/avllist.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    19044 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/gnuregex.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2684 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/errorfns.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2155 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/_hyExecutionContext.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3945 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/alignment.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6990 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/polynoml.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     7299 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/parser.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    35475 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/calcnode.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    16440 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/simplelist.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4446 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/constant.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    21529 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/site.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4060 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/baseobj.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6116 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/classes.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    30760 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/matrix.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5680 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/variable.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    31149 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/hy_strings.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    14580 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/defines.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4039 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/fstring.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    11141 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/list.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3570 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/sequence.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2215 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/stack.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5767 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/variablecontainer.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6009 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/category.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2203 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/avllistxl.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9005 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/mathobj.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4748 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/mypthread.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4967 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/operation.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    11816 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/trie.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    32307 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/likefunc.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    25807 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/batchlan.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2288 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/include/avllistx.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    16902 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/trie.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   280975 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/batchlan.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    24278 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/avllist.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2955 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/stack.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2816 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/ptr_array.cp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6388 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/mathobj.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    44902 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/simplelist.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    20668 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/sequence.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    92271 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/formula.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    50097 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/likefuncocl.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     4499 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/avllistxl.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16832 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/list.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   103816 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/batchlan2.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   338060 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/matrix.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    59369 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/nexus.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    70504 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/alignment.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    20453 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/variable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   403092 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/likefunc.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    44699 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/category.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    23670 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/constant.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    21889 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/baseobj.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    39732 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/parser.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    12374 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/batchlanhelpers.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    61517 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/likefunc2.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   424517 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/calcnode.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   179566 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/regex.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    28192 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/hyphy-src/src/core/fstring.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   105197 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/core/polynoml.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/utils/
+-rw-r--r--   0 sweaver    (501) staff       (20)    13348 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/utils/hyphyunixutils.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/
+-rw-r--r--   0 sweaver    (501) staff       (20)   166170 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYParameterTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   149461 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYDialogDefs.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/
+-rw-r--r--   0 sweaver    (501) staff       (20)      184 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4001.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1021 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7050.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      927 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6004.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      913 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6010.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      945 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6011.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      952 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6005.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      936 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4000.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      176 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4002.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      191 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6013.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      208 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6007.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      946 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6006.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      198 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6012.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      177 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4003.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      963 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6016.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      900 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6002.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      968 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6003.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      307 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6017.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      922 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6001.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      202 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6014.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      935 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6000.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      899 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4011.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      918 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5020.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      194 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7020.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      225 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7012.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      271 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5003.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      295 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5002.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      229 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7013.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      282 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/striped.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      978 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7005.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      247 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7011.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      288 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5000.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      277 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5001.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      929 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7010.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      943 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7004.png
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/
+-rw-r--r--   0 sweaver    (501) staff       (20)      483 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_vert1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     4018 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/focus.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/entry1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      311 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_vth1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_top.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/entry2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      192 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_vth2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_right3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      158 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/hline.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_right2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      209 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/menu_shadow.png
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/
+-rw-r--r--   0 sweaver    (501) staff       (20)      507 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/ext1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      500 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/obutton1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       86 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/entry1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3669 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg1.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      235 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll-base.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      506 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/ext2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_right.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll4.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      500 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/obutton2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3258 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/plus1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_up.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu-item.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3669 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg2.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       86 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/note.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      291 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base2.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      673 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/pase-panther1
+-rw-r--r--   0 sweaver    (501) staff       (20)       86 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/flat.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      113 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hline.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      427 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base3.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      551 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/gem.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      187 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/small-base.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      549 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/normal1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_left.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sright3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       86 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/up.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      325 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/handle.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       86 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/in.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      186 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/clear.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      186 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/yellow.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1026 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/blue.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      549 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/active1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      673 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-panther1.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      147 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)     3669 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)     1026 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vslide1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      148 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bc.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown.1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/minus.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sleft1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      355 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-2.0.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      186 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/green.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3258 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/radio2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/trough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       65 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/color.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton1.1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3201 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3668 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/button4.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      291 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/check-radio.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/radio1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      175 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option_menu.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3087 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vscroll1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hscroll1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hslide.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      175 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/option_menu2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      153 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/paned2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      165 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_sub.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vscroll2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      643 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hstrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      549 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/insen.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hscroll2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/spin1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      643 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vstrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1025 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vtrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      153 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/paned1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sdown1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/sup.1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1119 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       65 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/lineh.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/default.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slide.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      426 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/exttop2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_down.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1119 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/htrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      142 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      468 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vslide.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/abutton1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      426 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/exttop1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      186 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/red.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/arrow_down1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      291 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/menu-base.xcf
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_right.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      180 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook_border.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      290 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_right1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      162 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/empty.png
+-rw-r--r--   0 sweaver    (501) staff       (20)       71 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/blank.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1113 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook5.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_left_start.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      207 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_hth2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1754 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook4.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      163 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame_gap_top_end.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1586 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button13alpha.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1587 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button12alpha.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3873 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button9.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      353 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_hth1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      173 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/vline.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom_start.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      822 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button8.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1797 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      250 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_up1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1133 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1766 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)    24576 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.gtkrc.swp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1355 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      250 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_up2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      250 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_up3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/background.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      803 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      695 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/check1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/menubar.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_right_end.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     4194 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3873 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button0.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_left_end.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1525 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/check2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     4181 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame_gap.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      811 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      621 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button5.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      276 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_left2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1796 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_vert1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      943 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      482 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/slider_horiz1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     4181 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      276 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_left3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      822 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button4.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      605 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button6.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     3279 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option_menu.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      323 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/handle_vert_thumb.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      276 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_left1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1083 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     4181 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      822 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button7.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      447 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/shadow1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      162 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame_gap_top_start.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_top_start.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_right_start.png
+-rw-r--r--   0 sweaver    (501) staff       (20)    19898 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/theme.rc
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_top_end.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1061 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/shadow2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_left.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1318 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/vtrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1512 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button12.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      281 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_down3.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      223 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/menu_selected.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1427 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/htrough.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      281 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_down2.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1586 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button13.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      134 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/white.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/gap_bottom_end.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1928 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button11.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      281 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/arrow_down1.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1967 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button11alpha.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      189 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/132.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      923 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7000.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      202 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7014.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      274 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5005.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      463 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4001.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      925 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6040.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      925 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6041.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      463 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4000.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      267 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5004.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      933 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7001.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1596 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/133.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      164 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/131.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      921 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7003.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      152 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5006.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      447 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4002.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      920 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6042.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      447 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4003.xpm
+-rw-r--r--   0 sweaver    (501) staff       (20)      231 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5007.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      933 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7002.png
+-rw-r--r--   0 sweaver    (501) staff       (20)     1240 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/130.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      918 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4020.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      265 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6031.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      230 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6019.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      271 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6018.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      945 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6030.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      283 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6032.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      942 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6033.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      326 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6022.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      957 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6036.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      217 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6008.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      205 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6020.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      959 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6034.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      948 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6035.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      291 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6021.png
+-rw-r--r--   0 sweaver    (501) staff       (20)      191 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6009.png
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1464 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5004.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1316 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6041.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    11958 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/133.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1308 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7001.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1246 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7014.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1326 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7000.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/132.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1282 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6040.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1432 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5005.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1464 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5007.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1226 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6042.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    12342 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/130.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1296 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7002.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1286 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7003.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/131.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/333.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1314 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5006.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1466 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5002.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1258 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7013.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7012.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1478 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5003.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1478 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5001.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1294 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7004.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1270 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7010.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7011.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1300 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7005.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1466 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5000.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1282 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6036.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1314 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6022.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    69088 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/pthreadGC2.dll
+-rw-r--r--   0 sweaver    (501) staff       (20)     1246 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6009.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6021.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1314 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6035.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1318 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6034.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1294 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6020.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1312 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6008.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6030.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1258 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6018.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1110 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/3000.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2238 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/132.cur
+-rw-r--r--   0 sweaver    (501) staff       (20)     1222 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4020.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1314 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6019.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1260 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6031.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1330 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6033.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1318 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6032.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    91880 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/hyphy.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6017.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6003.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    38454 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/401.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2238 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/129.cur
+-rw-r--r--   0 sweaver    (501) staff       (20)     2238 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/128.cur
+-rw-r--r--   0 sweaver    (501) staff       (20)    38454 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/400.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1178 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6002.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1336 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6016.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1266 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6000.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)      246 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6014.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    38454 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/402.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    10356 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/Win.rc
+-rw-r--r--   0 sweaver    (501) staff       (20)     1286 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4011.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    86070 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/pthreadVC2.dll
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6001.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1304 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6005.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1308 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6011.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1224 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4000.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7050.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1222 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4001.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6010.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1310 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6004.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)   204862 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/desk.ico
+-rw-r--r--   0 sweaver    (501) staff       (20)     1226 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6012.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1324 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6006.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1222 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4003.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1222 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4002.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1298 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6007.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)      246 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6013.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1334 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7020.bmp
+-rw-r--r--   0 sweaver    (501) staff       (20)    34422 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYObjectInspector.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     5339 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYBaseGUI.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   134951 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYModelWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    34864 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/preferences.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    22505 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/
+-rw-r--r--   0 sweaver    (501) staff       (20)    20077 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformComponent.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    22486 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatfromUtils.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4739 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/semaphore.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4824 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2644 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformButtonMenu.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1845 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformTextbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1029 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformButtonBar.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1654 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformTable.h
+-rw-r--r--   0 sweaver    (501) staff       (20)      959 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformButton.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1591 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformPullDown.h
+-rw-r--r--   0 sweaver    (501) staff       (20)      781 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformCheckbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)      958 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformLabel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1868 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformComponent.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4910 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/sched.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    43645 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/pthread.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2778 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformGraphicPane.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    25331 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)    15026 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformButtonBar.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    60118 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6083 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformCheckBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    11842 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformPullDown.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    22449 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformTextBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     5558 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformLabel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9125 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformSequencePane.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6958 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformButton.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    27696 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformGraphicPane.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4712 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformModelWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    38634 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformDataPanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9772 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformParameterTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    10669 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformPWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    48283 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformTreePanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)      637 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformDBWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)      709 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformBootsrapWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16164 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformConsoleWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    13936 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformTWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    15250 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformChartWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1922 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformGWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3124 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYTableWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2654 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYEventTypes.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2371 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYBaseGUI.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3771 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYUtils.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1357 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYObjectInspector.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2838 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/preferences.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3144 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4321 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYGraphicPane.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3018 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYLabel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3562 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYComponent.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4285 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYSequencePanel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2176 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYList.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2800 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYPullDown.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3811 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYTextBox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2072 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYButton.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1706 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYCanvas.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2685 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYButtonBar.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     8079 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYTableComponent.h
+-rw-r--r--   0 sweaver    (501) staff       (20)        0 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/shared_main.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3659 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYSharedMain.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9573 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/HYDialogs.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     8761 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYChartWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     6641 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYModelWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3045 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYConsoleWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     8058 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYParameterTable.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2350 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYDBWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2238 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYGWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    15151 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYTreePanel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    12813 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYDataPanel.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/
+-rw-r--r--   0 sweaver    (501) staff       (20)     7009 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/helpers.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1190 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphymain.ui
+-rw-r--r--   0 sweaver    (501) staff       (20)     1186 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphymessageoutput.ui
+-rw-r--r--   0 sweaver    (501) staff       (20)     1795 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphyhierarchicalselector.ui
+-rw-r--r--   0 sweaver    (501) staff       (20)    17372 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphymain.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)      557 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/simplerequest.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5120 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphymain.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2431 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphyhierarchicalselector.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1227 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/qterminal.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1658 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphymessageoutput.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2513 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphy_qt_helpers.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1935 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphyevents.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     9282 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/qterminal.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2055 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphy_qt_utility.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2191 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphymessageoutput.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8105 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphyhierarchicalselector.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1965 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/simplerequest.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1698 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphyevents.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1300 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/qt/main.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    22083 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYConsoleWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/
+-rw-r--r--   0 sweaver    (501) staff       (20)    25014 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformComponent.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   388670 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HyPhy.rsrc
+-rw-r--r--   0 sweaver    (501) staff       (20)    31651 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformUtils.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   169303 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPHYMP.icns
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4461 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformWindow.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     5096 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformButtonMenu.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)     1932 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformTextbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1147 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformList.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1438 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformButtonBar.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1422 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformTable.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1136 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformButton.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1599 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformPullDown.h
+-rw-r--r--   0 sweaver    (501) staff       (20)      871 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformCheckbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1004 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformLabel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1798 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformComponent.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2636 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformGraphicPane.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     1017 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/plist.xml
+-rw-r--r--   0 sweaver    (501) staff       (20)   388670 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/iHyPhyDebug.rsrc
+-rw-r--r--   0 sweaver    (501) staff       (20)    32566 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   169303 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Docs.icns
+-rw-r--r--   0 sweaver    (501) staff       (20)   169303 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPHY.icns
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)    20124 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformButtonBar.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    62184 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6234 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformCheckBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9014 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformPullDown.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8223 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformList.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    35459 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformTextBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     5790 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformLabel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8580 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformSequencePane.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9410 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformButton.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16752 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformGraphicPane.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    26364 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/hydialogs.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)       93 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/plistmp.r
+-rw-r--r--   0 sweaver    (501) staff       (20)     1557 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/Info.plist
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6003 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformModelWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    38052 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDataPanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8400 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformParameterTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    11564 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformPWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    49772 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTreePanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)      722 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDBWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)      854 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformBootsrapWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    10084 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformConsoleWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16460 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    17835 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformChartWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9566 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformGWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)       91 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/mac/plist.r
+-rw-r--r--   0 sweaver    (501) staff       (20)    12755 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYComponent.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4444 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYLabel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6836 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYTextBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     4045 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYButton.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6149 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYPullDown.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     6258 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYButtonBar.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    71812 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    50829 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYSequencePanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2904 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYCheckBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    10751 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYEventTypes.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16430 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYGraphicPane.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    15418 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYSharedMain.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/
+-rw-r--r--   0 sweaver    (501) staff       (20)    18725 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformComponent.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    23566 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformUtils.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6495 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformWindow.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3207 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformTextbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2697 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformButtonBar.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3033 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformTable.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2498 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformButton.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2971 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformPullDown.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2257 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformCheckbox.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     2321 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformLabel.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     3434 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformComponent.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     4506 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformGraphicPane.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    27342 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/
+-rw-r--r--   0 sweaver    (501) staff       (20)    16910 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformButtonBar.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    60674 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     7791 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformCheckBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16779 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformPullDown.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    20953 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformTextBox.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     7456 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformLabel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    16680 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformSequencePane.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     9140 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformButton.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    20757 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformGraphicPane.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:38.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/
+-rw-r--r--   0 sweaver    (501) staff       (20)     6951 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformModelWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    35368 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDataPanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    12460 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformParameterTable.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     7278 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformPWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    39261 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTreePanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     1785 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDBWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     2215 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformBootsrapWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    23442 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformConsoleWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    18555 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    14800 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformChartWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     3015 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformGWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   340254 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYDataPanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    42655 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYDBWindow.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   268500 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYTreePanel.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   156385 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/gui/HYChartWindow.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/new/
+-rw-r--r--   0 sweaver    (501) staff       (20)   102142 2018-02-16 16:13:37.000000 hyphy-python-0.1.9/hyphy-src/src/new/bayesgraph.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    65762 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/bayesgraph2.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    71042 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/bgm2.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/new/include/
+-rw-r--r--   0 sweaver    (501) staff       (20)    27674 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/include/scfg.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     7135 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/include/bayesgraph.h
+-rw-r--r--   0 sweaver    (501) staff       (20)     8202 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/include/bgm.h
+-rw-r--r--   0 sweaver    (501) staff       (20)    99243 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/scfg.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   114883 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/new/bgm.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/
+-rw-r--r--   0 sweaver    (501) staff       (20)    23530 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/batchfiles.list
+-rw-r--r--   0 sweaver    (501) staff       (20)     1188 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/README
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/
+-rw-r--r--   0 sweaver    (501) staff       (20)   249527 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_python.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   249527 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_py3.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   100171 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_R.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     4797 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/build.sh
+-rw-r--r--   0 sweaver    (501) staff       (20)     3598 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/setup.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Link/
+-rw-r--r--   0 sweaver    (501) staff       (20)    14450 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Link/THyPhy.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8815 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Link/THyPhy.h
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/Python/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3953 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/Python/BasicHyPhy.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/data/
+-rw-r--r--   0 sweaver    (501) staff       (20)     3761 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/data/hiv.nuc
+-rw-r--r--   0 sweaver    (501) staff       (20)     2055 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/F81.bf
+-rw-r--r--   0 sweaver    (501) staff       (20)      797 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/HKY85.bf
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/R/
+-rw-r--r--   0 sweaver    (501) staff       (20)     4315 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/Examples/R/BasicHyPhy.R
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/Python/
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/Python/HyPhy/
+-rw-r--r--   0 sweaver    (501) staff       (20)     2170 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/Python/HyPhy/__init__.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/R/
+-rw-r--r--   0 sweaver    (501) staff       (20)    39161 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/R/HyPhy.R
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/mains/
+-rw-r--r--   0 sweaver    (501) staff       (20)    25783 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/mains/unix.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    29309 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/mains/win.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    48912 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/mains/mac.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)    12925 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/mains/gtk.cpp
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy-src/src/ocl/
+-rw-r--r--   0 sweaver    (501) staff       (20)    15170 2018-02-16 16:10:15.000000 hyphy-python-0.1.9/hyphy-src/src/ocl/opencl_kernels.cl
+-rw-r--r--   0 sweaver    (501) staff       (20)       46 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/MANIFEST.in
+-rw-r--r--   0 sweaver    (501) staff       (20)      273 2015-11-08 23:32:25.000000 hyphy-python-0.1.9/README
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/SWIGWrappers/
+-rw-r--r--   0 sweaver    (501) staff       (20)   249527 2015-11-08 23:32:25.000000 hyphy-python-0.1.9/SWIGWrappers/THyPhy_python.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)   250687 2015-11-08 23:33:21.000000 hyphy-python-0.1.9/SWIGWrappers/THyPhy_py3.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     4062 2018-02-16 16:26:49.000000 hyphy-python-0.1.9/setup.py
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/Link/
+-rw-r--r--   0 sweaver    (501) staff       (20)    14489 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/Link/THyPhy.cpp
+-rw-r--r--   0 sweaver    (501) staff       (20)     8827 2018-02-16 16:10:14.000000 hyphy-python-0.1.9/Link/THyPhy.h
+-rw-r--r--   0 sweaver    (501) staff       (20)       38 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/setup.cfg
+drwxr-xr-x   0 sweaver    (501) staff       (20)        0 2018-02-16 16:27:39.000000 hyphy-python-0.1.9/hyphy_python.egg-info/
+-rw-r--r--   0 sweaver    (501) staff       (20)      308 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy_python.egg-info/PKG-INFO
+-rw-r--r--   0 sweaver    (501) staff       (20)    83402 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy_python.egg-info/SOURCES.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)       13 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy_python.egg-info/top_level.txt
+-rw-r--r--   0 sweaver    (501) staff       (20)        1 2018-02-16 16:27:37.000000 hyphy-python-0.1.9/hyphy_python.egg-info/dependency_links.txt
```

### Comparing `hyphy-python-0.1.8/HyPhy/__init__.py` & `hyphy-python-0.1.9/HyPhy/__init__.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/cmake/cmake_uninstall.cmake.in` & `hyphy-python-0.1.9/hyphy-src/cmake/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/cmake/FindOpenCL.cmake` & `hyphy-python-0.1.9/hyphy-src/cmake/FindOpenCL.cmake`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/CMakeLists.txt` & `hyphy-python-0.1.9/hyphy-src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/CMakeWin32/CMakeLists.txt` & `hyphy-python-0.1.9/hyphy-src/CMakeWin32/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/cl2hdr.c` & `hyphy-python-0.1.9/hyphy-src/contrib/cl2hdr.c`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/aclocal.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/aclocal.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.guess` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.guess`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.h.in` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.h.in`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/config.sub` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/config.sub`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/depcomp` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/depcomp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/install-sh` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/install-sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/ltmain.sh` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/ltmain.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/build-aux/missing` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/build-aux/missing`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CHANGES` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CHANGES`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/cmake/internal_utils.cmake` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/cmake/internal_utils.cmake`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CMakeLists.txt` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.cbproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.cbproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.groupproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest.groupproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_all.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_all.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_link.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_link.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_main.cbproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_main.cbproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_unittest.cbproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/codegear/gtest_unittest.cbproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/configure` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/configure`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/configure.ac` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/configure.ac`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/CONTRIBUTORS` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest-all.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest_main.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/fused-src/gtest/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-death-test.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-death-test.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-message.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-message.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h.pump` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-param-test.h.pump`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-printers.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-printers.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-spi.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-spi.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-test-part.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-test-part.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-typed-test.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest-typed-test.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_pred_impl.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_pred_impl.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_prod.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/gtest_prod.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-death-test-internal.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-death-test-internal.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-filepath.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-filepath.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-internal.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-internal.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-linked_ptr.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-linked_ptr.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h.pump` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util-generated.h.pump`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-param-util.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-port.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-port.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-string.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-string.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h.pump` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-tuple.h.pump`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h.pump` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/include/gtest/internal/gtest-type-util.h.pump`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/LICENSE` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/acx_pthread.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/acx_pthread.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/gtest.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/gtest.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/libtool.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltoptions.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltsugar.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/ltversion.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/m4/lt~obsolete.m4` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/Makefile.am` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/Makefile.am`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/Makefile.in` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/Makefile.in`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.sln` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.sln`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest-md.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.sln` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.sln`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main-md.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main-md.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_main.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test-md.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test-md.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_prod_test.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest-md.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest-md.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest.vcproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/msvc/gtest_unittest.vcproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/README` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/README`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/prime_tables.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/prime_tables.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample10_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample10_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample1_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample1_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample2_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample2_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample3-inl.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample3-inl.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample3_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample3_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample4_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample4_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample5_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample5_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample6_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample6_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample7_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample7_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample8_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample8_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/samples/sample9_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/samples/sample9_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/fuse_gtest_files.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/fuse_gtest_files.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/gen_gtest_pred_impl.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/gen_gtest_pred_impl.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/gtest-config.in` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/gtest-config.in`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/scripts/pump.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/scripts/pump.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-all.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-all.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-death-test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-death-test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-filepath.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-filepath.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-internal-inl.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-internal-inl.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-port.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-port.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-printers.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-printers.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-test-part.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-test-part.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest-typed-test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest-typed-test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/src/gtest_main.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/src/gtest_main.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_ex_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_ex_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-death-test_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-filepath_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-filepath_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-linked_ptr_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-linked_ptr_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-listener_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-listener_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-message_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-message_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-options_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-options_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test2_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test2_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-param-test_test.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-port_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-port_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-printers_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-printers_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-test-part_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-test-part_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-tuple_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-tuple_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test2_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test2_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-typed-test_test.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest-unittest-api_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest-unittest-api_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_all_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_all_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_break_on_failure_unittest_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_catch_exceptions_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_color_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_env_var_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_environment_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_environment_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_filter_unittest_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_help_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_list_tests_unittest_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_main_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_main_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_no_test_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_no_test_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_golden_lin.txt` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_output_test_golden_lin.txt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_pred_impl_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_pred_impl_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_premature_exit_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_premature_exit_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_prod_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_prod_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_repeat_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_repeat_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_shuffle_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_sole_header_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_sole_header_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_stress_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_stress_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_test_utils.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_test_utils.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_ex_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_ex_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_throw_on_failure_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_uninitialized_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_unittest.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_unittest.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile1_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile1_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile2_test_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfile2_test_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfiles_test.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_outfiles_test.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest_.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_output_unittest_.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_test_utils.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/gtest_xml_test_utils.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/production.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/production.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/test/production.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/test/production.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/DebugProject.xcconfig` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/DebugProject.xcconfig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/FrameworkTarget.xcconfig` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/FrameworkTarget.xcconfig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/General.xcconfig` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/General.xcconfig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/ReleaseProject.xcconfig` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/ReleaseProject.xcconfig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Config/StaticLibraryTarget.xcconfig` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Config/StaticLibraryTarget.xcconfig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/project.pbxproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/gtest.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/Info.plist` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Resources/Info.plist`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/Info.plist` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/Info.plist`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/runtests.sh` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/runtests.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.h` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget_test.cc` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/widget_test.cc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Samples/FrameworkSample/WidgetFramework.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/runtests.sh` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/runtests.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/versiongenerate.py` & `hyphy-python-0.1.9/hyphy-src/contrib/gtest-1.7.0/xcode/Scripts/versiongenerate.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/shell.c` & `hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/shell.c`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c` & `hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3.h` & `hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/contrib/SQLite-3.8.2/sqlite3ext.h` & `hyphy-python-0.1.9/hyphy-src/contrib/SQLite-3.8.2/sqlite3ext.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/BatchLanguage/MatrixIndexing.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/BatchLanguage/MatrixIndexing.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/BatchLanguage/profile_test.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/BatchLanguage/profile_test.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/data/aspectrin.nuc` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/data/aspectrin.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions+MLE.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions+MLE.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions2.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/definitions3.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/definitions3.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Categories/displayFunction.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Categories/displayFunction.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/data/hiv.seq` & `hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/data/hiv.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint1.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint1.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint2.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint3.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/ReplicateConstraint3.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/ConstraintDefinition/shared.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/ConstraintDefinition/shared.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/data/actin2.flt` & `hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/data/actin2.flt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/HKY852blocks.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/HKY852blocks.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/DataFilters/HKY852blocks2models.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/DataFilters/HKY852blocks2models.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/aa.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/aa.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/3.seq` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/3.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/stewart.aa` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/stewart.aa`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/data/ubiq.flt` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/data/ubiq.flt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/ExonIntron.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/ExonIntron.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/MoreComplexModels/Models/MG94x2.mdl` & `hyphy-python-0.1.9/hyphy-src/Examples/MoreComplexModels/Models/MG94x2.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/data/hiv.nuc` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/data/hiv.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/F81.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/F81.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/HKY85.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/HKY85.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/HKY85shared.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/HKY85shared.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/JC69.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/JC69.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/K2P.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/K2P.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/K2Pshared.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/K2Pshared.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/Non-Rev.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/Non-Rev.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/REV.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/REV.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleAnalyses/REVshared.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleAnalyses/REVshared.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/3.seq` & `hyphy-python-0.1.9/hyphy-src/Examples/Simulation/data/3.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/aspectrin1.nuc` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/aspectrin1.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/aspectrin2.nuc` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/aspectrin2.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/data/molclock.seq` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/molclock.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81K81uf_relratio.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81K81uf_relratio.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81relrate.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81relrate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/F81relratio.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/F81relratio.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/HKY85relrate.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/HKY85relrate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/HKY85relratio.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/HKY85relratio.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/MolecularClockF81.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/MolecularClockF81.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/SimpleConstraints/MolecularClockHKY85.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/MolecularClockHKY85.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Simulation/data/3.seq` & `hyphy-python-0.1.9/hyphy-src/Examples/SimpleConstraints/data/3.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Simulation/data/hiv.nuc` & `hyphy-python-0.1.9/hyphy-src/Examples/Simulation/data/hiv.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Simulation/ParametricBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Simulation/ParametricBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Simulation/PBootstrapHetRates.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Simulation/PBootstrapHetRates.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/Examples/Simulation/RelativeRatePBS.bf` & `hyphy-python-0.1.9/hyphy-src/Examples/Simulation/RelativeRatePBS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/help/Commands/query.bf` & `hyphy-python-0.1.9/hyphy-src/help/Commands/query.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/help/Commands/reference.sql` & `hyphy-python-0.1.9/hyphy-src/help/Commands/reference.sql`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/help/Getting Started With HyPhy.pdf` & `hyphy-python-0.1.9/hyphy-src/help/Getting Started With HyPhy.pdf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/help/SelectionAnalyses.pdf` & `hyphy-python-0.1.9/hyphy-src/help/SelectionAnalyses.pdf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/installers/Mac/DMG.key` & `hyphy-python-0.1.9/hyphy-src/installers/Mac/DMG.key`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/Disk Image` & `hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/Disk Image`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/Preview.jpg` & `hyphy-python-0.1.9/hyphy-src/installers/Mac/MAC_dmg_template.dmgCanvas/QuickLook/Preview.jpg`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/installers/Win/hyphy.nsi` & `hyphy-python-0.1.9/hyphy-src/installers/Win/hyphy.nsi`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/installers/Win/license.rtf` & `hyphy-python-0.1.9/hyphy-src/installers/Win/license.rtf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/LICENSE` & `hyphy-python-0.1.9/hyphy-src/LICENSE`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/README.md` & `hyphy-python-0.1.9/hyphy-src/README.md`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Approximate_CDF` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Approximate_CDF`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Column Operations` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Column Operations`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Complex Select Cells By Value` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Complex Select Cells By Value`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Contigency Table` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Contigency Table`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Covariance` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Covariance`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/DescriptiveStats.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/DescriptiveStats.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/HY_DBW_TemplateList` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/HY_DBW_TemplateList`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToChartWindow.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToChartWindow.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToConsole.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToConsole.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFileFromPandit.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFastaFileFromPandit.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToFrontierFastaFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToFrontierFastaFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToSQLFlatFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToSQLFlatFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DBAddIns/ToTabFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DBAddIns/ToTabFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Descriptive Statistics` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Descriptive Statistics`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Distribution Moments` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Distribution Moments`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Event Posteriors` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Event Posteriors`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/posteriors.ibf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Includes/posteriors.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Most Likely Class Assignment` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Most Likely Class Assignment`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Distribution` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Distribution`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Moments` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Posterior Moments`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/DistributionAddIns/Prior Moments` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/DistributionAddIns/Prior Moments`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Gaussian Penalty Clustering` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Gaussian Penalty Clustering`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Goodness of Fit` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Goodness of Fit`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Histogram` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Histogram`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/K-Mean Clustering` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/K-Mean Clustering`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/KH Resampler` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/KH Resampler`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Linear Fit` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Linear Fit`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Linear Fit.orig` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Linear Fit.orig`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Mean Profile Plot` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Mean Profile Plot`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Median Profile Plot` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Median Profile Plot`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Poisson Mixture Fit` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Poisson Mixture Fit`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Populate Cells` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Populate Cells`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Profile Mean Clustering` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Profile Mean Clustering`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Running Sum` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Running Sum`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/lhc.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/lhc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/sir.bf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/sir.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Samplers/srs.ibf` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Samplers/srs.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Select Cells By Index` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Select Cells By Index`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/ChartAddIns/Select Cells By Value` & `hyphy-python-0.1.9/hyphy-src/res/ChartAddIns/Select Cells By Value`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/data/brown.nuc` & `hyphy-python-0.1.9/hyphy-src/res/data/brown.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/data/integrase_BDA.nex` & `hyphy-python-0.1.9/hyphy-src/res/data/integrase_BDA.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/data/p51.aa` & `hyphy-python-0.1.9/hyphy-src/res/data/p51.aa`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/data/p51.nex` & `hyphy-python-0.1.9/hyphy-src/res/data/p51.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Character Plot` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Character Plot`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Character Plot Two` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Character Plot Two`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Compare Subsets` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Compare Subsets`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/ibfs/char_colors.def` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/ibfs/char_colors.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/Sequence Plot` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/Sequence Plot`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/DatapanelAddIns/TBD/Character Plot By Sequence` & `hyphy-python-0.1.9/hyphy-src/res/DatapanelAddIns/TBD/Character Plot By Sequence`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Alt_Yeast_Nuclear.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Alt_Yeast_Nuclear.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Ascidian_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Ascidian_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Blepharisma_Nuclear.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Blepharisma_Nuclear.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Ciliate.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Ciliate.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Echinoderm_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Echinoderm_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Euplotid_Nuclear.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Euplotid_Nuclear.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Flatworm_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Flatworm_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Invertebrate_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Invertebrate_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Mold_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Mold_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Thraustochytrium_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Thraustochytrium_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Vertebratemtdna.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Vertebratemtdna.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/GeneticCodes/Yeast_mtDNA.cod` & `hyphy-python-0.1.9/hyphy-src/res/GeneticCodes/Yeast_mtDNA.cod`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/aa.bf` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/aa.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/AAEFV/Estimated` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/AAEFV/Estimated`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/codon.bf` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/codon.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Codon` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Codon`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 3 params.` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 3 params.`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 9 params.` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/CodonEFV/Observed Nuc 9 params.`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/dinuc.bf` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/dinuc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta-Gamma` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Beta-Gamma`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/General Discrete` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/General Discrete`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Half Normal` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Half Normal`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/Heterogeneity/Lognormal` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/Heterogeneity/Lognormal`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionClasses/NucEFV/Estimated` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionClasses/NucEFV/Estimated`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Dayhoff.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Dayhoff.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/EIAA.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/EIAA.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Fitness.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Fitness.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/Jones.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/Jones.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Aminoacid/mtREV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Aminoacid/mtREV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Binary/F81.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Binary/F81.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/GY94_3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/GY94_3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/Lineage_MG94xHKY85.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/Lineage_MG94xHKY85.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_HKY85x3_4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_HKY85x3_4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94_REV_3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94REVOmegaCF3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94REVOmegaCF3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xHKY85_3x4_2Rates.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xHKY85_3x4_2Rates.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV_GDD.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xREV_3x4_DualRV_GDD.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Codon/MG94xTN93_3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Codon/MG94xTN93_3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/EFVEstimated.ibf` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/EFVEstimated.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/F81.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/F81.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/HKY85.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/HKY85.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/REV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/REV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/REVBetaGamma.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/REVBetaGamma.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/Nucleotide/TrN.mdl` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/Nucleotide/TrN.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/Nucleotide/JC69` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/Nucleotide/JC69`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/SubstitutionModels/User/Nucleotide/K2P` & `hyphy-python-0.1.9/hyphy-src/res/SubstitutionModels/User/Nucleotide/K2P`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGenerator.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGenerator.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGeneratorNoPS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/discreteGeneratorNoPS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma1.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma1.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2+Inv.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2+Inv.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/gamma2.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/GY94.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/GY94.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94GY94xREV_PARRIS_syn3.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94GY94xREV_PARRIS_syn3.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate_Multirate.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/MG94xREVxBivariate_Multirate.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M3.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_M3.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_syn3.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_syn3.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_synvar.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/2RatesAnalyses/PARRIS_synvar.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/454.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/454.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_BMS_Aux.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_BMS_Aux.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_CMS_Aux.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_CMS_Aux.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_MFReader_.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_MFReader_.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_MSCOneStep.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_MSCOneStep.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/_tipDater.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/_tipDater.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AAModelComparison.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AAModelComparison.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AddABias.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AddABias.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonData.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonData.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonDataMPI.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeCodonDataMPI.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeDiNucData.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeDiNucData.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucDataFreq2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/AnalyzeNucProtData2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/bayesgraph.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/bayesgraph.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BGM.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BGM.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/binomial.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/binomial.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BivariateCodonRateAnalysis.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BivariateCodonRateAnalysis.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchClassDNDS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchClassDNDS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSiteREL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSiteREL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSiteRELMultiModel.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSiteRELMultiModel.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BranchSwap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BranchSwap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/branchSwappingFunctions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/branchSwappingFunctions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BS2007.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BS2007.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BUSTED-SRV.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BUSTED-SRV.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/BUSTED.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/BUSTED.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/categoryEcho.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/categoryEcho.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/chooseDistanceFormula.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/chooseDistanceFormula.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CleanGaps.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CleanGaps.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CleanStopCodons.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CleanStopCodons.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ClusterAnalysis.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ClusterAnalysis.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ClusterByDistanceRange.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ClusterByDistanceRange.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonBivariateRateProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonBivariateRateProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonModelCompare.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonModelCompare.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonToProtein.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonToProtein.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CodonUsageBias.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CodonUsageBias.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressure.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressure.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressureIVL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/CompareSelectivePressureIVL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ConvertDataFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ConvertDataFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DatedTipsMolecularClock.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DatedTipsMolecularClock.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DirectionalREL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DirectionalREL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DirectionalREL_MF.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DirectionalREL_MF.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DistanceMatrix.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DistanceMatrix.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/DistanceMatrix_Splits.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/DistanceMatrix_Splits.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/distanceMethodNPBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/distanceMethodNPBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/distanceRMethodNPBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/distanceRMethodNPBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools2.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/CodonTools2.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/CodonToolsMain.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/CodonToolsMain.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/JC69` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/JC69`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/K2P` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/K2P`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/K2P_RV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/K2P_RV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Modified_Nei_Gojobori` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Modified_Nei_Gojobori`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Nei_Gojobori` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Nei_Gojobori`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_aa` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_aa`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_codon` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/p_Distance_codon`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC_MH` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC_MH`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/PC_RV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/PC_RV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/T3P` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/T3P`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN84` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN84`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN93` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN93`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/TN93_RV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/TN93_RV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ_FR` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Distances/Unaligned_LZ_FR`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis_CompareDS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSBivariateRateAnalysis_CompareDS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparison.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparison.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonPartitions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSDistributionComparisonPartitions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis_MF.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSRateAnalysis_MF.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dNdSResultProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dNdSResultProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/doNNISwap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/doNNISwap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/doSPRSwap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/doSPRSwap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/dSdNTreeTools.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/dSdNTreeTools.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/F_ST.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/F_ST.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/files.lst` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/files.lst`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FitnessAAModels.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FitnessAAModels.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_1.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_1.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_3.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_3.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_4.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_4.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_5.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_PHASE_5.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_tools.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/FUBAR_HBL/FUBAR_tools.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC_Binary.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC_Binary.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GA_CHC_kernel.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GA_CHC_kernel.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClock.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClock.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClock.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClock.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessorM.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GADatedClockProcessorM.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARD.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARD.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARD_GA_CHC.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARD_GA_CHC.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARDProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARDProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GARecomb.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GARecomb.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Gateaux.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Gateaux.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Gateaux2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Gateaux2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/GateauxMR.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/GateauxMR.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/heuristicMethodNPBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/heuristicMethodNPBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_k_means.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_k_means.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_PCA.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_PCA.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Kernel_support.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Kernel_support.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/KHTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/KHTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LHT.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LHT.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/IOFunctions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/IOFunctions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/MG_REV.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon/MG_REV.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/codon.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/GTR.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA/GTR.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/DNA.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/frequencies.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/frequencies.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/model_functions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/model_functions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/parameters.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/parameters.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/rate_variation.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/rate_variation.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/models/terms.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/models/terms.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/estimators.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/tasks/estimators.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/lib2014/UtilityFunctions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/lib2014/UtilityFunctions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LocalBranchSiteTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LocalBranchSiteTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LocalMolClock.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LocalMolClock.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LRTRecombTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LRTRecombTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/LZ_Complexity.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/LZ_Complexity.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MaxChi2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MaxChi2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MEDS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MEDS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MEME_mf.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MEME_mf.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MergeSequences.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MergeSequences.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MergeSites.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MergeSites.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPositiveSelection.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPositiveSelection.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPositiveSelectionPooled.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPositiveSelectionPooled.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MFPSreader.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MFPSreader.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MGvsGY.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MGvsGY.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorAAProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorAAProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorBranch.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorBranch.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodon.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodonProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorCodonProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA_1.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelSelectorRNA_1.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ModelTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ModelTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MolClockAllRoots.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MolClockAllRoots.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/molclockBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/molclockBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/MolecularClock.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/MolecularClock.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NeighborJoining.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NeighborJoining.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NielsenYang.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NielsenYang.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/NucModelCompare.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/NucModelCompare.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimator.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/pairwiseDistanceEstimator.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRate.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRatio.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseRelativeRatio.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PairwiseSiteDiversity.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PairwiseSiteDiversity.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PARRIS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PARRIS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PartitionDataFile.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PartitionDataFile.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PartitionRateComparison.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PartitionRateComparison.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/partitionSequences.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/partitionSequences.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Plato.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Plato.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/PositiveSelectionLI.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/PositiveSelectionLI.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_ancestors.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_ancestors.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_counting.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_counting.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_covariance.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_covariance.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_dNdS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_dNdS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_sampler.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_sampler.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_saveResults.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_saveResults.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_sns.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_sns.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_variance.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_variance.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/post_viewResults.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/post_viewResults.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/postprocessors.lst` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/postprocessors.lst`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper1.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper1.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper1_mf.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper1_mf.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper2.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper2.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper2_mf.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper2_mf.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper3.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper3.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/qndhelper4.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/qndhelper4.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/queryTree.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/queryTree.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetection.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetection.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetectionMF.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/QuickSelectionDetectionMF.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RateClassCounter.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RateClassCounter.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/ReduceDataSetMatrix.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/ReduceDataSetMatrix.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRate.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRateL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRateL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RelativeRatio.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RelativeRatio.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/RELAX.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/RELAX.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relrateBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relrateBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relrateBootstrapL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relrateBootstrapL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/relratioBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/relratioBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SampleProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SampleProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/lhc.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/lhc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/lhc_supp.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/lhc_supp.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/sir.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/sir.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Samplers/srs.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Samplers/srs.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SandNSAmbigs.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SandNSAmbigs.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SelectionLRT.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SelectionLRT.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignment.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignment.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodonShared.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentCodonShared.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNuc.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNuc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNucShared.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentNucShared.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentProt.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentProt.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignmentTop75.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignmentTop75.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SeqAlignShared.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SeqAlignShared.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SequentialAddition.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SequentialAddition.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SequentialAddition.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SequentialAddition.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGASimProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGASimProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGEmulator.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGEmulator.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGEmulator_MF.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGEmulator_MF.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SGIvL.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SGIvL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimilarityPlot.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimilarityPlot.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimmondsAI.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimmondsAI.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/simpleBootstrap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/simpleBootstrap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SimpleMutationCounter.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SimpleMutationCounter.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb-2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb-2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SingleBreakpointRecomb.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SiteRates.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SiteRates.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SiteRates2.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SiteRates2.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison-2parts.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison-2parts.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlatkinMaddison.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlidingNucWindow.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlidingNucWindow.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SlidingWindowAnalysis.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SlidingWindowAnalysis.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SplitSequencesByPattern.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SplitSequencesByPattern.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SSRatesTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SSRatesTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StarDecomposition.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StarDecomposition.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StrandGRMTest.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StrandGRMTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/StripStopCodons.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/StripStopCodons.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/SubtreeSelectionComparison.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/SubtreeSelectionComparison.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/190` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/190`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/BranchSiteTemplate.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/BranchSiteTemplate.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/CF3x4.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/CF3x4.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/chooseGeneticCode.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/chooseGeneticCode.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/custm4x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/custm4x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA_empirical.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Custom_AA_empirical.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Dayhoff_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Default` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Default`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineGamma.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineGamma.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineHM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/defineHM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F+omega.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F+omega.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+F3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+MLFREQS.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM+MLFREQS.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/ECM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAA.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAA.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAAFreq.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EIAAFreq.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/BLOSUM62` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/BLOSUM62`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/cpREV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/cpREV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/Dayhoff` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/Dayhoff`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/H5N1` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/H5N1`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVBetween` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVBetween`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVWithin` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/HIVWithin`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/IAV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/IAV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/JTT` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/JTT`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LCAP` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LCAP`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LG` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/LG`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/modellist.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/modellist.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/MtArt` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/MtArt`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtMAM` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtMAM`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtREV24` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/mtREV24`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/rtREV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/rtREV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/VT` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/VT`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/WAG` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalAA/WAG`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECM` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECM`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECMu` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EmpiricalCodon/KHG_ECMu`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.dat` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.dat`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/EX.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81_binary.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F81_binary.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84P.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/F84P.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/fitness.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/fitness.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GRM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GRM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94customF3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94customF3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94w9.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/GY94w9.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVbetween.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HIVwithin.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/HKY85.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/HKY85.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69_binary.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/JC69_binary.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Jones_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/K2P.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/K2P.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/K3ST.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/K3ST.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/LCAP.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/LCAP.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MEC.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MEC.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94custom.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94custom.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customCF3x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customCF3x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customF1x4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customF1x4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customFreqs.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94customFreqs.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAA.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAA.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61multiple.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAF61multiple.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAFreqs.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAFreqs.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAUserFreqs.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wAAUserFreqs.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wEX.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94wEX.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94with9freqs.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94with9freqs.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94x2.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MG94x2.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGFreqsEstimator.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGFreqsEstimator.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwAA.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwAA.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwEX.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/MGwEX.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters2.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters2.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters3.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters3.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters4.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters4.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters5.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/modelParameters5.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/models.lst` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/models.lst`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtMAM_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/mtREV_24_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM+Freqs.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM+Freqs.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/NRM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/PCH` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/PCH`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/reducedREV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/reducedREV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16A` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16A`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16SvH.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNA16SvH.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAMuse95.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAMuse95.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV_1` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/RNAREV_1`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/rtREV_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/S4` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/S4`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/STGRM.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/STGRM.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/TrN.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/TrN.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/UniversalCode.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/UniversalCode.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG_F.mdl` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/WAG_F.mdl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TemplateModels/Yang2000Distributions.def` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TemplateModels/Yang2000Distributions.def`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestBranchDNDS.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestBranchDNDS.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestClade.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestClade.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TestCladeMeans.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TestCladeMeans.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TopologySearch.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TopologySearch.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TopologySearchConstrained.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TopologySearchConstrained.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TreeCorrelationCoefficients.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TreeCorrelationCoefficients.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/TreeTools.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/TreeTools.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/UpperBound.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/UpperBound.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/AncestralMapper.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/AncestralMapper.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/BranchLengthFitters.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/BranchLengthFitters.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/CoalescentPostProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/CoalescentPostProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/CodonTools.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/CodonTools.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/DBTools.ibf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/DBTools.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/DescriptiveStatistics.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/DescriptiveStatistics.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/GrabBag.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/GrabBag.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/HXB2Mapper.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/HXB2Mapper.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREV.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREV.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREVMLFreqs.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/LocalMGREVMLFreqs.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/MPITools.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/MPITools.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/NJ.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/NJ.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/PostScript.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/PostScript.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/ProbabilityDistributions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/ProbabilityDistributions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/PS_Plotters.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/PS_Plotters.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/ReadDelimitedFiles.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/ReadDelimitedFiles.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/TreeFunctions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/TreeFunctions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/Utility/WriteDelimitedFiles.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/Utility/WriteDelimitedFiles.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/WANC.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/WANC.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/WebUpdate.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/WebUpdate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TemplateBatchFiles/YangNielsenBranchSite2005.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/YangNielsenBranchSite2005.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Exhaustive_Search` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Exhaustive_Search`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Neighbor_Joining` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Neighbor_Joining`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Sequential_Addition` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Sequential_Addition`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Star_Decomposition` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Star_Decomposition`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/branchSwappingFunctions.bf` & `hyphy-python-0.1.9/hyphy-src/res/TemplateBatchFiles/branchSwappingFunctions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/doNNISwap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/doNNISwap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TopologyInference/Support/doSPRSwap.bf` & `hyphy-python-0.1.9/hyphy-src/res/TopologyInference/Support/doSPRSwap.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TreeAddIns/Splits` & `hyphy-python-0.1.9/hyphy-src/res/TreeAddIns/Splits`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/TreeAddIns/Tree Statistics` & `hyphy-python-0.1.9/hyphy-src/res/TreeAddIns/Tree Statistics`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/AAContent` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/AAContent`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/BranchLengthCI` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/BranchLengthCI`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/CodonMutationToTreeMapper` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/CodonMutationToTreeMapper`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/CountSubstitutions` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/CountSubstitutions`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/ExportLikelihoodFunction` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/ExportLikelihoodFunction`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/GenBankSequences` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/GenBankSequences`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/MappersHelp.ibf` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/MappersHelp.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/Includes/MappersHelpAA.ibf` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/Includes/MappersHelpAA.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/ListUserFunctions` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/ListUserFunctions`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/MapSubstitutions` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/MapSubstitutions`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/MeanPairwiseDivergence` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/MeanPairwiseDivergence`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/MeanPairwiseDivergenceSubset` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/MeanPairwiseDivergenceSubset`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/ModelCounter` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/ModelCounter`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/AAMutationCounter` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/AAMutationCounter`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/CodonMutationToTreeMapper.bf` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/CodonMutationToTreeMapper.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ColorPSTree` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ColorPSTree`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ConvergentAndParallel` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ConvergentAndParallel`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/CopyBranchLengths` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/CopyBranchLengths`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/DashPSTree` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/DashPSTree`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/dNanddSTrees.bf` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/dNanddSTrees.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/dS and dN factors` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/dS and dN factors`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ExpsPerDirection` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ExpsPerDirection`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/FilterAssignments` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/FilterAssignments`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/InferredAASubstitutionsCounter` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/InferredAASubstitutionsCounter`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/LocaldNdS` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/LocaldNdS`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ModelFitSummary` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ModelFitSummary`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/ModelFitSummaryAA` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/ModelFitSummaryAA`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/Multiclass DN DS inference` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/Multiclass DN DS inference`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/PartitionBranchesByClasses` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/PartitionBranchesByClasses`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/PredictivePosteriorP` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/PredictivePosteriorP`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/RNARateMatrix` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/RNARateMatrix`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/SimulateAndTabDN_DS` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/SimulateAndTabDN_DS`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/SimulateFromLF` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/SimulateFromLF`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/OldAddins/TreeLengthConstraint` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/OldAddins/TreeLengthConstraint`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/RecombinationProcessor.bf` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/RecombinationProcessor.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/SimulateFromLF` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/SimulateFromLF`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/res/UserAddins/Tidbits` & `hyphy-python-0.1.9/hyphy-src/res/UserAddins/Tidbits`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/build.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/build.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/build_mingw.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/build_mingw.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/build_mingw_gui.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/build_mingw_gui.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/build_mingw_MEGA.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/build_mingw_MEGA.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/buildFromSVN.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/buildFromSVN.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/buildMinGWFromSVN.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/buildMinGWFromSVN.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/scripts/gtk_build.sh` & `hyphy-python-0.1.9/hyphy-src/scripts/gtk_build.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/_hyExecutionContext.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/_hyExecutionContext.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/alignment.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/alignment.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/avllist.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/avllist.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/avllistx.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/avllistx.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/avllistxl.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/avllistxl.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/baseobj.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/baseobj.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/batchlan.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/batchlan.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/batchlan2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/batchlan2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/batchlanhelpers.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/batchlanhelpers.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/batchlanruntime.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/batchlanruntime.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/calcnode.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/calcnode.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/calcnode2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/calcnode2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/category.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/category.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/classes.cp` & `hyphy-python-0.1.9/hyphy-src/src/core/classes.cp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/constant.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/constant.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/error.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/error.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/fisher_exact.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/fisher_exact.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/formula.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/formula.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/fstring.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/fstring.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/_hyExecutionContext.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/_hyExecutionContext.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/alignment.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/alignment.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/avllist.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/avllist.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/avllistx.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/avllistx.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/avllistxl.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/avllistxl.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/baseobj.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/baseobj.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/batchlan.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/batchlan.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/calcnode.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/calcnode.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/category.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/category.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/classes.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/classes.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/constant.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/constant.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/defines.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/defines.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/errorfns.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/errorfns.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/formula.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/formula.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/fstring.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/fstring.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/gnuregex.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/gnuregex.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/hy_strings.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/hy_strings.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/likefunc.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/likefunc.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/list.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/list.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/mathobj.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/mathobj.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/matrix.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/matrix.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/mypthread.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/mypthread.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/operation.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/operation.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/parser.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/parser.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/polynoml.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/polynoml.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/sequence.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/sequence.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/simplelist.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/simplelist.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/site.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/site.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/stack.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/stack.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/trie.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/trie.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/variable.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/variable.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/include/variablecontainer.h` & `hyphy-python-0.1.9/hyphy-src/src/core/include/variablecontainer.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/likefunc.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/likefunc.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/likefunc2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/likefunc2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/likefuncocl.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/likefuncocl.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/list.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/list.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/mathobj.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/mathobj.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/matrix.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/matrix.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/nexus.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/nexus.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/operation.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/operation.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/parser.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/parser.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/parser2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/parser2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/polynoml.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/polynoml.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/ptr_array.cp` & `hyphy-python-0.1.9/hyphy-src/src/core/ptr_array.cp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/regex.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/regex.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/sequence.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/sequence.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/simplelist.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/simplelist.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/site.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/site.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/stack.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/stack.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/strings.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/strings.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/trie.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/trie.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/variable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/variable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/core/variablecontainer.cpp` & `hyphy-python-0.1.9/hyphy-src/src/core/variablecontainer.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYButton.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYButton.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYButtonBar.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYButtonBar.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYCheckBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYCheckBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYLabel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYLabel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYPullDown.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYPullDown.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYSequencePanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYSequencePanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/Components/HYTextBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/Components/HYTextBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformButton.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformButton.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformButtonBar.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformButtonBar.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformCheckBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformCheckBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformLabel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformLabel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformPullDown.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformPullDown.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformSequencePane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformSequencePane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/Components/HYPlatformTextBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/Components/HYPlatformTextBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformComponent.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformComponent.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformGraphicPane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformGraphicPane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformUtils.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformUtils.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/HYPlatformWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/HYPlatformWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformButton.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformButton.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformButtonBar.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformButtonBar.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformCheckbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformCheckbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformLabel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformLabel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformPullDown.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformPullDown.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformTable.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformTable.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/Components/HYPlatformTextbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/Components/HYPlatformTextbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformComponent.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformComponent.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformGraphicPane.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformGraphicPane.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/include/HYPlatformWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/include/HYPlatformWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformBootsrapWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformBootsrapWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformChartWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformChartWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformConsoleWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformConsoleWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDataPanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDataPanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDBWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformDBWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformGWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformGWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformModelWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformModelWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformParameterTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformParameterTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformPWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformPWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTreePanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTreePanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/gtk/WindowClasses/HYPlatformTWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYBaseGUI.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYBaseGUI.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYChartWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYChartWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYComponent.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYComponent.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYConsoleWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYConsoleWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYDataPanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYDataPanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYDBWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYDBWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYDialogDefs.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYDialogDefs.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYEventTypes.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYEventTypes.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYGraphicPane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYGraphicPane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYModelWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYModelWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYObjectInspector.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYObjectInspector.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYParameterTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYParameterTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYSharedMain.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYSharedMain.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYTreePanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYTreePanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/HYWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/HYWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYButton.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYButton.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYButtonBar.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYButtonBar.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYCanvas.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYCanvas.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYComponent.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYComponent.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYLabel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYLabel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYList.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYList.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYPullDown.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYPullDown.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYSequencePanel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYSequencePanel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYTableComponent.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYTableComponent.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/Components/HYTextBox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/Components/HYTextBox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYBaseGUI.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYBaseGUI.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYDialogs.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYDialogs.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYEventTypes.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYEventTypes.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYGraphicPane.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYGraphicPane.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYObjectInspector.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYObjectInspector.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYSharedMain.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYSharedMain.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYTableWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYTableWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYUtils.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYUtils.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/HYWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/HYWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/preferences.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/preferences.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYChartWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYChartWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYConsoleWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYConsoleWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYDataPanel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYDataPanel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYDBWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYDBWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYGWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYGWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYModelWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYModelWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYParameterTable.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYParameterTable.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/include/WindowClasses/HYTreePanel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/include/WindowClasses/HYTreePanel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformButton.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformButton.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformButtonBar.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformButtonBar.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformCheckBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformCheckBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformLabel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformLabel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformList.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformList.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformPullDown.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformPullDown.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformSequencePane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformSequencePane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Components/HYPlatformTextBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Components/HYPlatformTextBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Docs.icns` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPHYMP.icns`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/hydialogs.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/hydialogs.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPHY.icns` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Docs.icns`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HyPhy.rsrc` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HyPhy.rsrc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPHYMP.icns` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPHY.icns`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformComponent.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformComponent.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformGraphicPane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformGraphicPane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformUtils.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformUtils.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/HYPlatformWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/HYPlatformWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/iHyPhyDebug.rsrc` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/iHyPhyDebug.rsrc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformButton.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformButton.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformButtonBar.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformButtonBar.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformCheckbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformCheckbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformLabel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformLabel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformList.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformList.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformPullDown.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformPullDown.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformTable.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformTable.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/Components/HYPlatformTextbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/Components/HYPlatformTextbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformButtonMenu.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformButtonMenu.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformComponent.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformComponent.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformGraphicPane.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformGraphicPane.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/include/HYPlatformWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/include/HYPlatformWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/Info.plist` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/Info.plist`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/plist.xml` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/plist.xml`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformBootsrapWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformBootsrapWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformChartWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformChartWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformConsoleWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformConsoleWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDataPanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDataPanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDBWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformDBWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformGWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformGWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformModelWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformModelWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformParameterTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformParameterTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformPWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformPWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTreePanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTreePanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/mac/WindowClasses/HYPlatformTWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/preferences.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/preferences.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/helpers.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/helpers.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphy_qt_utility.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphy_qt_utility.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphyevents.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphyevents.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphyhierarchicalselector.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphyhierarchicalselector.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphymain.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphymain.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/hyphymessageoutput.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/hyphymessageoutput.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphy_qt_helpers.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphy_qt_helpers.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphyevents.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphyevents.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphyhierarchicalselector.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphyhierarchicalselector.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphymain.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphymain.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/hyphymessageoutput.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/hyphymessageoutput.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/qterminal.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/qterminal.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/include/simplerequest.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/include/simplerequest.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/main.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/main.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/qterminal.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/qterminal.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/simplerequest.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/simplerequest.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphyhierarchicalselector.ui` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphyhierarchicalselector.ui`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphymain.ui` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphymain.ui`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/qt/ui/hyphymessageoutput.ui` & `hyphy-python-0.1.9/hyphy-src/src/gui/qt/ui/hyphymessageoutput.ui`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/130.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/130.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/133.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/133.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4000.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4000.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4011.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4011.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/4020.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/5020.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/5020.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/4020.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6000.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6000.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6001.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6001.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6002.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6002.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6003.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6003.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6004.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6004.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6005.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6005.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6006.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6006.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6010.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6010.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6011.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6011.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6016.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6016.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6030.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6030.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6033.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6033.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6034.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6034.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6035.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6035.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6036.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6036.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6040.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6040.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6041.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6041.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/6042.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/6042.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7000.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7000.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7001.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7001.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7002.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7002.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7003.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7003.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7004.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7004.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7005.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7005.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7010.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7010.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/7050.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/7050.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.gtkrc.swp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.gtkrc.swp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/active1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/active1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-panther1.xcf` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/pase-panther1`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg.xpm` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg.xpm`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg1.xpm` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg1.xpm`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg2.xpm` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/bg2.xpm`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extbottom2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extleft2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/extright2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/gem.xcf` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/gem.xcf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hstrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/hstrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/htrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/htrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/insen.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/insen.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/normal1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/normal1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/pase-panther1` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/base-panther1.xcf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/scroll.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/slider2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vstrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vstrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vtrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/.xvpics/vtrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button0.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button9.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button11.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button11.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button11alpha.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button11alpha.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button12.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button12.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button12alpha.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button12alpha.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button13.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button13alpha.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button13alpha.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button13.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button3.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button3.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button4.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button8.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button5.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button5.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button6.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button6.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button7.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button4.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button8.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button7.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/button9.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/button0.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/check1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/check1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/check2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/check2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/focus.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/focus.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame_gap.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/frame_gap.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/frame1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/htrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/htrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook3.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook3.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook4.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook4.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/notebook5.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/notebook5.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/option_menu.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/option_menu.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_horiz2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_vert1.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/scrollbar_vert1.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/shadow2.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/shadow2.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/theme.rc` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/theme.rc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/GTKResources/theme/vtrough.png` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/GTKResources/theme/vtrough.png`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/128.cur` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/128.cur`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/129.cur` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/129.cur`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/130.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/130.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/131.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/131.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/132.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/132.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/132.cur` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/132.cur`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/133.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/133.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/3000.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/3000.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/333.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/333.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/400.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/400.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4000.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4000.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4001.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4001.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4002.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4002.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4003.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4003.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/401.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/401.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4011.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4011.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/402.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/402.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/4020.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/4020.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5000.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5000.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5001.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5001.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5002.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5002.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5003.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5003.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5004.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5004.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5005.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5005.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5006.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5006.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/5007.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/5007.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6000.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6000.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6001.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6001.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6002.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6002.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6003.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6003.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6004.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6004.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6005.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6005.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6006.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6006.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6007.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6007.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6008.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6008.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6009.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6009.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6010.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6010.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6011.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6011.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6012.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6012.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6016.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6016.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6017.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6017.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6018.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6018.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6019.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6019.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6020.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6020.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6021.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6021.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6022.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6022.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6030.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6030.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6031.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6031.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6032.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6032.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6033.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6033.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6034.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6034.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6035.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6035.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6036.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6036.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6040.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6040.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6041.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6041.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/6042.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/6042.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7000.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7000.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7001.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7001.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7002.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7002.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7003.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7003.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7004.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7004.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7005.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7005.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7010.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7010.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7011.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7011.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7012.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7012.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7013.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7013.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7014.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7014.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7020.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7020.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/7050.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/7050.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/desk.ico` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/desk.ico`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/hyphy.bmp` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/hyphy.bmp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/pthreadGC2.dll` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/pthreadGC2.dll`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/pthreadVC2.dll` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/pthreadVC2.dll`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/res/Windows/Win.rc` & `hyphy-python-0.1.9/hyphy-src/src/gui/res/Windows/Win.rc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformButton.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformButton.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformButtonBar.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformButtonBar.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformCheckBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformCheckBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformLabel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformLabel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformPullDown.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformPullDown.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformSequencePane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformSequencePane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/Components/HYPlatformTextBox.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/Components/HYPlatformTextBox.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformComponent.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformComponent.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformGraphicPane.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformGraphicPane.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatformWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatformWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/HYPlatfromUtils.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/HYPlatfromUtils.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformButton.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformButton.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformButtonBar.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformButtonBar.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformCheckbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformCheckbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformLabel.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformLabel.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformPullDown.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformPullDown.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformTable.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformTable.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/Components/HYPlatformTextbox.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/Components/HYPlatformTextbox.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformButtonMenu.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformButtonMenu.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformComponent.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformComponent.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformGraphicPane.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformGraphicPane.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/HYPlatformWindow.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/HYPlatformWindow.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/pthread.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/pthread.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/sched.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/sched.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/include/semaphore.h` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/include/semaphore.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformBootsrapWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformBootsrapWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformChartWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformChartWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformConsoleWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformConsoleWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformDataPanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformDataPanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformDBWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformDBWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformGWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformGWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformModelWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformModelWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformParameterTable.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformParameterTable.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformPWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformPWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformTreePanel.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformTreePanel.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/gui/win/WindowClasses/HYPlatformTWindow.cpp` & `hyphy-python-0.1.9/hyphy-src/src/gui/win/WindowClasses/HYPlatformTWindow.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/batchfiles.list` & `hyphy-python-0.1.9/hyphy-src/src/lib/batchfiles.list`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/build.sh` & `hyphy-python-0.1.9/hyphy-src/src/lib/build.sh`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/data/hiv.nuc` & `hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/data/hiv.nuc`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/F81.bf` & `hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/F81.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Examples/HBL/HKY85.bf` & `hyphy-python-0.1.9/hyphy-src/src/lib/Examples/HBL/HKY85.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Examples/Python/BasicHyPhy.py` & `hyphy-python-0.1.9/hyphy-src/src/lib/Examples/Python/BasicHyPhy.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Examples/R/BasicHyPhy.R` & `hyphy-python-0.1.9/hyphy-src/src/lib/Examples/R/BasicHyPhy.R`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/Python/HyPhy/__init__.py` & `hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/Python/HyPhy/__init__.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/LibraryModules/R/HyPhy.R` & `hyphy-python-0.1.9/hyphy-src/src/lib/LibraryModules/R/HyPhy.R`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Link/THyPhy.cpp` & `hyphy-python-0.1.9/hyphy-src/src/lib/Link/THyPhy.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/Link/THyPhy.h` & `hyphy-python-0.1.9/hyphy-src/src/lib/Link/THyPhy.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/README` & `hyphy-python-0.1.9/hyphy-src/src/lib/README`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/setup.py` & `hyphy-python-0.1.9/hyphy-src/src/lib/setup.py`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_py3.cpp` & `hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_python.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_python.cpp` & `hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_py3.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/lib/SWIGWrappers/THyPhy_R.cpp` & `hyphy-python-0.1.9/hyphy-src/src/lib/SWIGWrappers/THyPhy_R.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/mains/gtk.cpp` & `hyphy-python-0.1.9/hyphy-src/src/mains/gtk.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/mains/mac.cpp` & `hyphy-python-0.1.9/hyphy-src/src/mains/mac.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/mains/unix.cpp` & `hyphy-python-0.1.9/hyphy-src/src/mains/unix.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/mains/win.cpp` & `hyphy-python-0.1.9/hyphy-src/src/mains/win.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/bayesgraph.cpp` & `hyphy-python-0.1.9/hyphy-src/src/new/bayesgraph.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -343,30 +343,30 @@
         }
 
 
         // prior precision (Gaussian)
         if ((avl_val = (_Constant *) (this_avl->GetByKey (_HYBgm_PRIOR_PRECISION, NUMBER)))) {
             prior_precision.Store (node, 0, (_Parameter) (avl_val->Value()));
 
-            if (avl_val != nullptr) {
+            if (avl_val) {
                 errorMessage = _String ("PriorPrecision must be greater than zero, received ") & prior_precision(node,0) & " for node " & node;
                 break;
             }
             // ReportWarning (_String("prior_precision[") & node & "] set to " & prior_precision(node,0) );
         } else if (!avl_val && node_type.lData[node] == 1) {
             errorMessage = _String ("Missing PriorPrecision in associative array for node ") & node;
             break;
         }
 
 
         // prior scale (Gaussian)
         if ((avl_val = (_Constant *) (this_avl->GetByKey (_HYBgm_PRIOR_SCALE, NUMBER)))) {
             prior_scale.Store (node, 0, (_Parameter) (avl_val->Value()));
 
-            if (avl_val != nullptr) {
+            if (avl_val) {
                 errorMessage = _String ("PriorScale must be greater than zero, received ") & prior_scale(node,0) & " for node " & node;
                 break;
             }
         } else if (!avl_val && node_type.lData[node] == 1) {
             errorMessage = _String ("Missing PriorScale in associative array for node ") & node;
             break;
         }
```

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/bayesgraph2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/new/bayesgraph2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/bgm.cpp` & `hyphy-python-0.1.9/hyphy-src/src/new/bgm.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/bgm2.cpp` & `hyphy-python-0.1.9/hyphy-src/src/new/bgm2.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/include/bayesgraph.h` & `hyphy-python-0.1.9/hyphy-src/src/new/include/bayesgraph.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/include/bgm.h` & `hyphy-python-0.1.9/hyphy-src/src/new/include/bgm.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/include/scfg.h` & `hyphy-python-0.1.9/hyphy-src/src/new/include/scfg.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/new/scfg.cpp` & `hyphy-python-0.1.9/hyphy-src/src/new/scfg.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/ocl/opencl_kernels.cl` & `hyphy-python-0.1.9/hyphy-src/src/ocl/opencl_kernels.cl`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/src/utils/hyphyunixutils.cpp` & `hyphy-python-0.1.9/hyphy-src/src/utils/hyphyunixutils.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_avllists.cpp` & `hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_avllists.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_list.cpp` & `hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_list.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_simplelists.cpp` & `hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_simplelists.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/gtests/ut_strings.cpp` & `hyphy-python-0.1.9/hyphy-src/tests/gtests/ut_strings.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/CodonAncestors.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/CodonAncestors.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/LeafProbs.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/LeafProbs.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/NucAncestors.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/NucAncestors.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Ancestors/NucRVAncestors.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Ancestors/NucRVAncestors.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/BayesianGraphicalModels/alarm.xml` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/BayesianGraphicalModels/alarm.xml`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/BayesianGraphicalModels/TestBGM.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/BayesianGraphicalModels/TestBGM.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/kernel.dump` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/kernel.dump`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/BFFeatures/TreeSplits.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/BFFeatures/TreeSplits.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/2.fas` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/2.fas`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/2.prot` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/2.prot`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/CD2.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/CD2.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/fluHA.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/fluHA.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/fluHA_codon.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/fluHA_codon.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HIVenvSweden.seq` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HIVenvSweden.seq`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HMM2_synthetic.fas` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HMM2_synthetic.fas`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/HMM4_synthetic.fas` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/HMM4_synthetic.fas`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/data/mtDNA.fas` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/data/mtDNA.fas`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/RateHMM.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/RateHMM.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/SmallNuc.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/SmallNuc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/SmallNucRel.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/SmallNucRel.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/HMM/TreeHMM.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/HMM/TreeHMM.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/ClearConstraintsBug.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/ClearConstraintsBug.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/expModelCrash.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/expModelCrash.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/ParseNexus.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/ParseNexus.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.alternative.fit` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.alternative.fit`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.partitioned_descriptive.fit` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.partitioned_descriptive.fit`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.RELAX.json` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.RELAX.json`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.tre` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/RELAX/segfault.nex.tre`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/RegressionTesting/res/69genes.test.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/RegressionTesting/res/69genes.test.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/BS-REL.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/BS-REL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/GTR_G_I.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/GTR_G_I.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/IntermediateNucRel.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/IntermediateNucRel.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/ModelMixture.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/ModelMixture.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/MultiplePartitions.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/MultiplePartitions.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/NY.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/NY.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/REL/SmallNucRel.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/REL/SmallNucRel.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Shared/TestInstrumentation.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Shared/TestInstrumentation.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateCodon.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateCodon.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateNuc.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateNuc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateProtein.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/IntermediateProtein.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/LargeNuc.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/LargeNuc.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodon.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodon.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodonLocal.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/SmallCodonLocal.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SimpleOptimizations/TwoSequenceTest.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SimpleOptimizations/TwoSequenceTest.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SpecializedOptimizations/SingleSiteTemplate.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SpecializedOptimizations/SingleSiteTemplate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/SpecializedOptimizations/SiteLikelihood.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/SpecializedOptimizations/SiteLikelihood.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/Trickier/NonReversibleWithDynamicFrequencies.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/Trickier/NonReversibleWithDynamicFrequencies.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/AllCommands.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/AllCommands.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/BranchLength.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/BranchLength.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DeleteObject.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/DeleteObject.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Differentiate.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Differentiate.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Export.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Export.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetDataInfo.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetDataInfo.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetString.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetString.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetURL.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/GetURL.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/HarvestFrequencies.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/HarvestFrequencies.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/JSON.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/JSON.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/SCFG.ibf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/SCFG.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/scfgG6c.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/SCFG/scfgG6c.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc2.nex` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/res/test_likefunc2.nex`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/Chinook_Sqlite.sqlite` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/testdata/Chinook_Sqlite.sqlite`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/TestTools.ibf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/TestTools.ibf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Type.bf` & `hyphy-python-0.1.9/hyphy-src/tests/hbltests/UnitTests/HBLCommands/Type.bf`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/hyphy_python.egg-info/SOURCES.txt` & `hyphy-python-0.1.9/hyphy_python.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,59 +1,60 @@
 MANIFEST.in
 README
 setup.py
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/Link/THyPhy.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/SWIGWrappers/THyPhy_py3.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/contrib/SQLite-3.8.2/shell.c
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/_hyExecutionContext.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/alignment.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/avllist.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/avllistx.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/avllistxl.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/baseobj.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/batchlan.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/batchlan2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/batchlanhelpers.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/batchlanruntime.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/calcnode.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/calcnode2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/category.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/constant.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/error.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/fisher_exact.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/formula.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/fstring.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/likefunc.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/likefunc2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/likefuncocl.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/list.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/mathobj.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/matrix.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/nexus.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/operation.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/parser.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/parser2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/polynoml.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/regex.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/sequence.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/simplelist.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/site.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/stack.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/strings.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/trie.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/variable.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/core/variablecontainer.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/gui/preferences.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/new/bayesgraph.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/new/bayesgraph2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/new/bgm.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/new/bgm2.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/new/scfg.cpp
-/Users/sweaver/Programming/hivtrace/hyphy-python-2/hyphy-src/src/utils/hyphyunixutils.cpp
+/Users/sweaver/Programming/hyphy-python/Link/THyPhy.cpp
+/Users/sweaver/Programming/hyphy-python/SWIGWrappers/THyPhy_py3.cpp
+/Users/sweaver/Programming/hyphy-python/SWIGWrappers/THyPhy_python.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/contrib/SQLite-3.8.2/shell.c
+/Users/sweaver/Programming/hyphy-python/hyphy-src/contrib/SQLite-3.8.2/sqlite3.c
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/_hyExecutionContext.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/alignment.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/avllist.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/avllistx.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/avllistxl.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/baseobj.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/batchlan.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/batchlan2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/batchlanhelpers.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/batchlanruntime.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/calcnode.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/calcnode2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/category.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/constant.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/error.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/fisher_exact.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/formula.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/fstring.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/likefunc.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/likefunc2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/likefuncocl.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/list.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/mathobj.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/matrix.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/nexus.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/operation.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/parser.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/parser2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/polynoml.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/regex.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/sequence.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/simplelist.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/site.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/stack.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/strings.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/trie.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/variable.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/core/variablecontainer.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/gui/preferences.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/new/bayesgraph.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/new/bayesgraph2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/new/bgm.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/new/bgm2.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/new/scfg.cpp
+/Users/sweaver/Programming/hyphy-python/hyphy-src/src/utils/hyphyunixutils.cpp
 HyPhy/__init__.py
 Link/THyPhy.cpp
 Link/THyPhy.h
 SWIGWrappers/THyPhy_py3.cpp
 SWIGWrappers/THyPhy_python.cpp
 hyphy-src/.gitignore
 hyphy-src/CMakeLists.txt
```

### Comparing `hyphy-python-0.1.8/Link/THyPhy.cpp` & `hyphy-python-0.1.9/Link/THyPhy.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/Link/THyPhy.h` & `hyphy-python-0.1.9/Link/THyPhy.h`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/setup.py` & `hyphy-python-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     return result
 
 openmp = ['-fopenmp'] if check_for_openmp() == 0 else []
 
 setup(
     name = 'hyphy-python',
-    version = '0.1.8',
+    version = '0.1.9',
     description = 'HyPhy package interface library',
     author = 'Sergei L Kosakovsky Pond and Steven Weaver',
     author_email = 'spond@temple.edu',
     url = 'http://github.com/veg/hyphy',
     packages = ['HyPhy'],
     package_dir = {'HyPhy': 'HyPhy'},
     ext_modules = [Extension('_HyPhy',
```

### Comparing `hyphy-python-0.1.8/SWIGWrappers/THyPhy_py3.cpp` & `hyphy-python-0.1.9/SWIGWrappers/THyPhy_py3.cpp`

 * *Files identical despite different names*

### Comparing `hyphy-python-0.1.8/SWIGWrappers/THyPhy_python.cpp` & `hyphy-python-0.1.9/SWIGWrappers/THyPhy_python.cpp`

 * *Files identical despite different names*

