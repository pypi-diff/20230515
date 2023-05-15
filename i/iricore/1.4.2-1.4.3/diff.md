# Comparing `tmp/iricore-1.4.2.tar.gz` & `tmp/iricore-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iricore-1.4.2.tar", max compression
+gzip compressed data, was "iricore-1.4.3.tar", max compression
```

## Comparing `iricore-1.4.2.tar` & `iricore-1.4.3.tar`

### file list

```diff
@@ -1,208 +1,143 @@
--rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.4.2/LICENSE
--rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.4.2/README.md
--rwxr-xr-x   0        0        0      463 2022-11-10 03:07:50.807105 iricore-1.4.2/build.py
--rwxr-xr-x   0        0        0      621 2023-05-15 20:34:36.569891 iricore-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     2444 2023-05-10 17:38:12.864418 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeCCompiler.cmake
--rw-r--r--   0        0        0     5442 2023-05-10 17:38:12.932418 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeCXXCompiler.cmake
--rwxr-xr-x   0        0        0    15968 2023-05-10 17:38:12.852419 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_C.bin
--rwxr-xr-x   0        0        0    15992 2023-05-10 17:38:12.920418 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_CXX.bin
--rwxr-xr-x   0        0        0    16312 2023-05-10 17:38:13.084416 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeDetermineCompilerABI_Fortran.bin
--rw-r--r--   0        0        0     2124 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeFortranCompiler.cmake
--rw-r--r--   0        0        0      402 2023-05-10 17:38:12.660420 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CMakeSystem.cmake
--rw-r--r--   0        0        0    26502 2023-05-10 17:38:12.668420 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdC/CMakeCCompilerId.c
--rwxr-xr-x   0        0        0    16088 2023-05-10 17:38:12.720420 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdC/a.out
--rw-r--r--   0        0        0    26276 2023-05-10 17:38:12.736420 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdCXX/CMakeCXXCompilerId.cpp
--rwxr-xr-x   0        0        0    16096 2023-05-10 17:38:12.788419 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdCXX/a.out
--rw-r--r--   0        0        0    43184 2023-05-10 17:38:12.932418 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdFortran/CMakeFortranCompilerId.F
--rwxr-xr-x   0        0        0    16224 2023-05-10 17:38:13.004417 iricore-1.4.2/src/iricore/CMakeFiles/3.26.3/CompilerIdFortran/a.out
--rw-r--r--   0        0        0    94029 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/CMakeConfigureLog.yaml
--rw-r--r--   0        0        0      664 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/CMakeDirectoryInformation.cmake
--rw-r--r--   0        0        0    18118 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/Makefile.cmake
--rw-r--r--   0        0        0     5252 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/Makefile2
--rw-r--r--   0        0        0      281 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/TargetDirectories.txt
--rw-r--r--   0        0        0     2867 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/VerifyGlobs.cmake
--rw-r--r--   0        0        0       85 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/cmake.check_cache
--rw-r--r--   0        0        0       77 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/cmake.verify_globs
--rw-r--r--   0        0        0     2455 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/DependInfo.cmake
--rw-r--r--   0        0        0    17918 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/build.make
--rw-r--r--   0        0        0      695 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/cmake_clean.cmake
--rw-r--r--   0        0        0      110 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/compiler_depend.make
--rw-r--r--   0        0        0      114 2023-05-10 17:38:13.096416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/compiler_depend.ts
--rw-r--r--   0        0        0     1186 2023-05-10 17:38:14.332404 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/depend.internal
--rw-r--r--   0        0        0      190 2023-05-10 17:38:14.332404 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/depend.make
--rw-r--r--   0        0        0      238 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/flags.make
--rw-r--r--   0        0        0       56 2023-05-10 17:38:14.332404 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/fortran.internal
--rw-r--r--   0        0        0   193048 2023-05-10 17:38:14.496403 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/cira.for.o
--rw-r--r--   0        0        0   182056 2023-05-10 17:38:14.696401 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/igrf.for.o
--rw-r--r--   0        0        0   714704 2023-05-10 17:38:15.580392 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/iridreg.for.o
--rw-r--r--   0        0        0   132472 2023-05-10 17:38:15.716391 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/iriflip.for.o
--rw-r--r--   0        0        0   476088 2023-05-10 17:38:16.204387 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/irifun.for.o
--rw-r--r--   0        0        0    11904 2023-05-10 17:38:16.228386 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/irirtam.for.o
--rw-r--r--   0        0        0   192592 2023-05-10 17:38:16.344385 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/irisub.for.o
--rw-r--r--   0        0        0    24400 2023-05-10 17:38:16.372385 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/iri2016/iritec.for.o
--rw-r--r--   0        0        0      514 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/link.txt
--rw-r--r--   0        0        0      236 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/progress.make
--rw-r--r--   0        0        0     6896 2023-05-10 17:38:16.392385 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/python_interface.f90.o
--rw-r--r--   0        0        0     6920 2023-05-10 17:38:16.412385 iricore-1.4.2/src/iricore/CMakeFiles/iri2016.dir/python_stec.f90.o
--rw-r--r--   0        0        0     2618 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/DependInfo.cmake
--rw-r--r--   0        0        0    19416 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/build.make
--rw-r--r--   0        0        0      745 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/cmake_clean.cmake
--rw-r--r--   0        0        0      110 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/compiler_depend.make
--rw-r--r--   0        0        0      114 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/compiler_depend.ts
--rw-r--r--   0        0        0     1299 2023-05-10 17:38:16.492384 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/depend.internal
--rw-r--r--   0        0        0      190 2023-05-10 17:38:16.492384 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/depend.make
--rw-r--r--   0        0        0      238 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/flags.make
--rw-r--r--   0        0        0       56 2023-05-10 17:38:16.492384 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/fortran.internal
--rw-r--r--   0        0        0   193048 2023-05-10 17:38:16.632382 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/cira.for.o
--rw-r--r--   0        0        0   182056 2023-05-10 17:38:16.808381 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/igrf.for.o
--rw-r--r--   0        0        0   656384 2023-05-10 17:38:17.676373 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/iridreg.for.o
--rw-r--r--   0        0        0   132472 2023-05-10 17:38:17.808371 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/iriflip.for.o
--rw-r--r--   0        0        0   525232 2023-05-10 17:38:18.340366 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/irifun.for.o
--rw-r--r--   0        0        0    11904 2023-05-10 17:38:18.364366 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/irirtam.for.o
--rw-r--r--   0        0        0   198576 2023-05-10 17:38:18.484365 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/irisub.for.o
--rw-r--r--   0        0        0    24400 2023-05-10 17:38:18.508365 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/iritec.for.o
--rw-r--r--   0        0        0   270520 2023-05-10 17:38:18.840362 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/iri2020/rocdrift.for.o
--rw-r--r--   0        0        0      560 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/link.txt
--rw-r--r--   0        0        0      268 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/progress.make
--rw-r--r--   0        0        0     6896 2023-05-10 17:38:18.860361 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/python_interface.f90.o
--rw-r--r--   0        0        0     6920 2023-05-10 17:38:18.880361 iricore-1.4.2/src/iricore/CMakeFiles/iri2020.dir/python_stec.f90.o
--rw-r--r--   0        0        0        3 2023-05-10 17:38:13.100416 iricore-1.4.2/src/iricore/CMakeFiles/progress.marks
--rwxr-xr-x   0        0        0      431 2023-03-30 01:46:08.763487 iricore-1.4.2/src/iricore/CMakeLists.txt
--rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.4.2/src/iricore/__init__.py
--rw-r--r--   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.4.2/src/iricore/config.py
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.4.2/src/iricore/data/data16/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.4.2/src/iricore/data/data16/igrf/igrf2020s.dat
--rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.4.2/src/iricore/data/data16/index/apf107.dat
--rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.4.2/src/iricore/data/data16/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data16/ursi/ursi22.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir11.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir12.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir13.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir14.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir15.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir16.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir17.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir18.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir19.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir20.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir21.asc
--rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ccir/ccir22.asc
--rw-r--r--   0        0        0      443 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1945.dat
--rw-r--r--   0        0        0      445 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1950.dat
--rw-r--r--   0        0        0      437 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1955.dat
--rw-r--r--   0        0        0      431 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1960.dat
--rw-r--r--   0        0        0      435 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1965.dat
--rw-r--r--   0        0        0      435 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1970.dat
--rw-r--r--   0        0        0      439 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1975.dat
--rw-r--r--   0        0        0      436 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1980.dat
--rw-r--r--   0        0        0      433 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1985.dat
--rw-r--r--   0        0        0      434 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1990.dat
--rw-r--r--   0        0        0      438 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf1995.dat
--rw-r--r--   0        0        0     1015 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2000.dat
--rw-r--r--   0        0        0     1219 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2005.dat
--rw-r--r--   0        0        0     1218 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2010.dat
--rw-r--r--   0        0        0     1188 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2015.dat
--rw-r--r--   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/igrf2020.dat
--rw-r--r--   0        0        0      598 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/igrf/igrf2020s.dat
--rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:07.732843 iricore-1.4.2/src/iricore/data/data20/index/apf107.dat
--rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.888841 iricore-1.4.2/src/iricore/data/data20/index/ig_rz.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat11.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat12.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat13.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat14.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat15.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat16.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat17.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat18.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat19.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat20.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat21.dat
--rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat22.dat
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi11.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi12.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi13.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi14.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi15.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi16.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi17.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi18.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi19.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi20.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi21.asc
--rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.2/src/iricore/data/data20/ursi/ursi22.asc
--rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.4.2/src/iricore/data_update.py
--rwxr-xr-x   0        0        0     9308 2023-05-10 18:13:43.181093 iricore-1.4.2/src/iricore/iri.py
--rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.4.2/src/iricore/iri2016/cira.for
--rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.4.2/src/iricore/iri2016/igrf.for
--rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.4.2/src/iricore/iri2016/iridreg.for
--rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.4.2/src/iricore/iri2016/iriflip.for
--rwxr-xr-x   0        0        0   485000 2022-12-13 18:56:28.397951 iricore-1.4.2/src/iricore/iri2016/irifun.for
--rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.4.2/src/iricore/iri2016/irirtam.for
--rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.4.2/src/iricore/iri2016/irisub.for
--rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.4.2/src/iricore/iri2016/iritec.for
--rwxr-xr-x   0        0        0      787 2022-10-05 19:17:08.132334 iricore-1.4.2/src/iricore/iri2016/test.f90
--rw-r--r--   0        0        0   112771 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/iri2020/cira.for
--rw-r--r--   0        0        0   161170 2023-05-05 23:11:51.859023 iricore-1.4.2/src/iricore/iri2020/igrf.for
--rw-r--r--   0        0        0  1315925 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/iri2020/iridreg.for
--rw-r--r--   0        0        0    87909 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/iri2020/iriflip.for
--rw-r--r--   0        0        0   576757 2023-05-05 23:11:51.947023 iricore-1.4.2/src/iricore/iri2020/irifun.for
--rw-r--r--   0        0        0     6147 2023-05-05 23:11:51.875023 iricore-1.4.2/src/iricore/iri2020/irirtam.for
--rw-r--r--   0        0        0    85341 2023-05-05 23:14:27.781737 iricore-1.4.2/src/iricore/iri2020/irisub.for
--rw-r--r--   0        0        0     9441 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/iri2020/iritec.for
--rw-r--r--   0        0        0   623932 2022-10-02 13:54:08.000000 iricore-1.4.2/src/iricore/iri2020/rocdrift.for
--rw-r--r--   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.4.2/src/iricore/modules.py
--rwxr-xr-x   0        0        0     1260 2023-03-30 01:44:21.528128 iricore-1.4.2/src/iricore/python_interface.f90
--rw-r--r--   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.4.2/src/iricore/python_stec.f90
--rw-r--r--   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.4.2/src/iricore/read_iri_data.py
--rw-r--r--   0        0        0     2846 1970-01-01 00:00:00.000000 iricore-1.4.2/setup.py
--rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 iricore-1.4.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1276 2022-05-03 16:22:41.008931 iricore-1.4.3/LICENSE
+-rwxr-xr-x   0        0        0     1254 2023-03-28 01:11:06.672275 iricore-1.4.3/README.md
+-rwxr-xr-x   0        0        0      463 2022-11-10 03:07:50.807105 iricore-1.4.3/build.py
+-rwxr-xr-x   0        0        0      621 2023-05-15 20:38:47.647304 iricore-1.4.3/pyproject.toml
+-rwxr-xr-x   0        0        0      431 2023-03-30 01:46:08.763487 iricore-1.4.3/src/iricore/CMakeLists.txt
+-rwxr-xr-x   0        0        0      112 2023-05-05 20:40:56.755640 iricore-1.4.3/src/iricore/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-05 22:32:51.315676 iricore-1.4.3/src/iricore/config.py
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir11.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir12.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir13.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir14.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir15.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir16.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir17.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir18.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir19.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir20.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir21.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ccir/ccir22.asc
+-rw-r--r--   0        0        0      443 2016-02-04 05:04:35.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1945.dat
+-rw-r--r--   0        0        0      445 2016-02-04 05:04:44.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1950.dat
+-rw-r--r--   0        0        0      437 2016-02-04 05:04:50.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1955.dat
+-rw-r--r--   0        0        0      431 2016-02-04 05:04:58.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1960.dat
+-rw-r--r--   0        0        0      435 2016-02-04 05:05:13.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1965.dat
+-rw-r--r--   0        0        0      435 2016-02-04 05:05:18.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1970.dat
+-rw-r--r--   0        0        0      439 2016-02-04 05:05:25.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1975.dat
+-rw-r--r--   0        0        0      436 2016-02-04 05:05:31.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1980.dat
+-rw-r--r--   0        0        0      433 2016-02-04 05:05:40.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1985.dat
+-rw-r--r--   0        0        0      434 2016-02-04 05:05:58.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1990.dat
+-rw-r--r--   0        0        0      438 2016-02-04 05:06:08.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf1995.dat
+-rw-r--r--   0        0        0     1015 2016-02-04 05:06:15.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2000.dat
+-rw-r--r--   0        0        0     1219 2016-02-04 05:06:22.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2005.dat
+-rw-r--r--   0        0        0     1218 2016-02-04 05:06:32.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2010.dat
+-rw-r--r--   0        0        0     1188 2020-04-06 19:51:12.000000 iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2015.dat
+-rw-r--r--   0        0        0     1018 2021-09-21 01:36:47.000000 iricore-1.4.3/src/iricore/data/data16/igrf/igrf2020.dat
+-rw-r--r--   0        0        0      598 2021-09-21 01:37:16.000000 iricore-1.4.3/src/iricore/data/data16/igrf/igrf2020s.dat
+-rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:06.976848 iricore-1.4.3/src/iricore/data/data16/index/apf107.dat
+-rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.132847 iricore-1.4.3/src/iricore/data/data16/index/ig_rz.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:17.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat11.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:21.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat12.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:26.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat13.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:31.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat14.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:35.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat15.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:47.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat16.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 04:59:56.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat17.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:05.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat18.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:12.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat19.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:19.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat20.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:27.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat21.dat
+-rw-r--r--   0        0        0    88224 2016-02-04 05:00:33.000000 iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat22.dat
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi11.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi12.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi13.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi14.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi15.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi16.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi17.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi18.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi19.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi20.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi21.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data16/ursi/ursi22.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir11.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir12.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir13.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir14.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir15.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir16.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir17.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir18.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir19.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir20.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir21.asc
+-rw-r--r--   0        0        0    44300 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ccir/ccir22.asc
+-rw-r--r--   0        0        0      443 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1945.dat
+-rw-r--r--   0        0        0      445 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1950.dat
+-rw-r--r--   0        0        0      437 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1955.dat
+-rw-r--r--   0        0        0      431 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1960.dat
+-rw-r--r--   0        0        0      435 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1965.dat
+-rw-r--r--   0        0        0      435 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1970.dat
+-rw-r--r--   0        0        0      439 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1975.dat
+-rw-r--r--   0        0        0      436 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1980.dat
+-rw-r--r--   0        0        0      433 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1985.dat
+-rw-r--r--   0        0        0      434 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1990.dat
+-rw-r--r--   0        0        0      438 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf1995.dat
+-rw-r--r--   0        0        0     1015 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2000.dat
+-rw-r--r--   0        0        0     1219 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2005.dat
+-rw-r--r--   0        0        0     1218 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2010.dat
+-rw-r--r--   0        0        0     1188 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2015.dat
+-rw-r--r--   0        0        0     1018 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/igrf2020.dat
+-rw-r--r--   0        0        0      598 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/igrf/igrf2020s.dat
+-rwxr-xr-x   0        0        0  1312575 2023-05-05 22:25:07.732843 iricore-1.4.3/src/iricore/data/data20/index/apf107.dat
+-rwxr-xr-x   0        0        0     9681 2023-05-05 22:25:07.888841 iricore-1.4.3/src/iricore/data/data20/index/ig_rz.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat11.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat12.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat13.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat14.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat15.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat16.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat17.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat18.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat19.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat20.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat21.dat
+-rw-r--r--   0        0        0    88224 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat22.dat
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi11.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi12.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi13.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi14.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi15.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi16.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi17.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi18.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi19.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi20.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi21.asc
+-rw-r--r--   0        0        0    30628 2011-12-16 22:39:00.000000 iricore-1.4.3/src/iricore/data/data20/ursi/ursi22.asc
+-rwxr-xr-x   0        0        0      725 2022-11-10 03:07:50.835105 iricore-1.4.3/src/iricore/data_update.py
+-rwxr-xr-x   0        0        0     9308 2023-05-10 18:13:43.181093 iricore-1.4.3/src/iricore/iri.py
+-rwxr-xr-x   0        0        0   112771 2022-11-10 03:07:50.835105 iricore-1.4.3/src/iricore/iri2016/cira.for
+-rwxr-xr-x   0        0        0   161141 2022-11-10 03:07:50.835105 iricore-1.4.3/src/iricore/iri2016/igrf.for
+-rwxr-xr-x   0        0        0  1409825 2022-11-10 03:07:50.839105 iricore-1.4.3/src/iricore/iri2016/iridreg.for
+-rwxr-xr-x   0        0        0    87973 2022-11-10 03:07:50.839105 iricore-1.4.3/src/iricore/iri2016/iriflip.for
+-rwxr-xr-x   0        0        0   485000 2022-12-13 18:56:28.397951 iricore-1.4.3/src/iricore/iri2016/irifun.for
+-rwxr-xr-x   0        0        0     6147 2022-12-13 16:30:02.547302 iricore-1.4.3/src/iricore/iri2016/irirtam.for
+-rwxr-xr-x   0        0        0    82092 2022-12-13 16:30:02.539301 iricore-1.4.3/src/iricore/iri2016/irisub.for
+-rwxr-xr-x   0        0        0     9441 2022-11-10 03:07:50.843105 iricore-1.4.3/src/iricore/iri2016/iritec.for
+-rwxr-xr-x   0        0        0      787 2022-10-05 19:17:08.132334 iricore-1.4.3/src/iricore/iri2016/test.f90
+-rw-r--r--   0        0        0   112771 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/iri2020/cira.for
+-rw-r--r--   0        0        0   161170 2023-05-05 23:11:51.859023 iricore-1.4.3/src/iricore/iri2020/igrf.for
+-rw-r--r--   0        0        0  1315925 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/iri2020/iridreg.for
+-rw-r--r--   0        0        0    87909 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/iri2020/iriflip.for
+-rw-r--r--   0        0        0   576757 2023-05-05 23:11:51.947023 iricore-1.4.3/src/iricore/iri2020/irifun.for
+-rw-r--r--   0        0        0     6147 2023-05-05 23:11:51.875023 iricore-1.4.3/src/iricore/iri2020/irirtam.for
+-rw-r--r--   0        0        0    85341 2023-05-05 23:14:27.781737 iricore-1.4.3/src/iricore/iri2020/irisub.for
+-rw-r--r--   0        0        0     9441 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/iri2020/iritec.for
+-rw-r--r--   0        0        0   623932 2022-10-02 13:54:08.000000 iricore-1.4.3/src/iricore/iri2020/rocdrift.for
+-rw-r--r--   0        0        0      652 2023-05-05 20:54:12.161524 iricore-1.4.3/src/iricore/modules.py
+-rwxr-xr-x   0        0        0     1260 2023-03-30 01:44:21.528128 iricore-1.4.3/src/iricore/python_interface.f90
+-rw-r--r--   0        0        0     1194 2023-03-30 01:44:21.552128 iricore-1.4.3/src/iricore/python_stec.f90
+-rw-r--r--   0        0        0     1020 2023-05-05 22:34:39.878513 iricore-1.4.3/src/iricore/read_iri_data.py
+-rw-r--r--   0        0        0     2449 1970-01-01 00:00:00.000000 iricore-1.4.3/setup.py
+-rw-r--r--   0        0        0     1814 1970-01-01 00:00:00.000000 iricore-1.4.3/PKG-INFO
```

### Comparing `iricore-1.4.2/LICENSE` & `iricore-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/README.md` & `iricore-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/pyproject.toml` & `iricore-1.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iricore"
-version = "1.4.2"
+version = "1.4.3"
 description = ""
 authors = ["Vadym Bidula <vadym.bidula@gmail.com>"]
 readme = "README.md"
 build = "build.py"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <4.0"
```

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir11.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir12.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir13.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir14.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir15.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir16.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir17.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir18.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir19.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir20.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir21.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ccir/ccir22.asc` & `iricore-1.4.3/src/iricore/data/data16/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2000.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2005.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2010.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/dgrf2015.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/igrf2020.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/igrf/igrf2020s.dat` & `iricore-1.4.3/src/iricore/data/data16/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/index/apf107.dat` & `iricore-1.4.3/src/iricore/data/data16/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/index/ig_rz.dat` & `iricore-1.4.3/src/iricore/data/data16/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat11.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat12.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat13.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat14.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat15.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat16.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat17.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat18.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat19.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat20.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat21.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/mcsat/mcsat22.dat` & `iricore-1.4.3/src/iricore/data/data16/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi11.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi12.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi13.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi14.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi15.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi16.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi17.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi18.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi19.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi20.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi21.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data16/ursi/ursi22.asc` & `iricore-1.4.3/src/iricore/data/data16/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir11.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir12.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir13.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir14.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir15.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir16.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir17.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir18.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir19.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir20.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir21.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ccir/ccir22.asc` & `iricore-1.4.3/src/iricore/data/data20/ccir/ccir22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2000.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2000.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2005.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2005.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2010.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2010.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/dgrf2015.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/dgrf2015.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/igrf2020.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/igrf2020.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/igrf/igrf2020s.dat` & `iricore-1.4.3/src/iricore/data/data20/igrf/igrf2020s.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/index/apf107.dat` & `iricore-1.4.3/src/iricore/data/data20/index/apf107.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/index/ig_rz.dat` & `iricore-1.4.3/src/iricore/data/data20/index/ig_rz.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat11.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat11.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat12.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat12.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat13.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat13.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat14.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat14.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat15.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat15.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat16.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat16.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat17.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat17.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat18.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat18.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat19.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat19.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat20.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat20.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat21.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat21.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/mcsat/mcsat22.dat` & `iricore-1.4.3/src/iricore/data/data20/mcsat/mcsat22.dat`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi11.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi11.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi12.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi12.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi13.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi13.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi14.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi14.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi15.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi15.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi16.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi16.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi17.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi17.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi18.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi18.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi19.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi19.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi20.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi20.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi21.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi21.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data/data20/ursi/ursi22.asc` & `iricore-1.4.3/src/iricore/data/data20/ursi/ursi22.asc`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/data_update.py` & `iricore-1.4.3/src/iricore/data_update.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri.py` & `iricore-1.4.3/src/iricore/iri.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/cira.for` & `iricore-1.4.3/src/iricore/iri2016/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/igrf.for` & `iricore-1.4.3/src/iricore/iri2016/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/iridreg.for` & `iricore-1.4.3/src/iricore/iri2016/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/iriflip.for` & `iricore-1.4.3/src/iricore/iri2016/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/irifun.for` & `iricore-1.4.3/src/iricore/iri2016/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/irirtam.for` & `iricore-1.4.3/src/iricore/iri2016/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/irisub.for` & `iricore-1.4.3/src/iricore/iri2016/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/iritec.for` & `iricore-1.4.3/src/iricore/iri2016/iritec.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2016/test.f90` & `iricore-1.4.3/src/iricore/iri2016/test.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/cira.for` & `iricore-1.4.3/src/iricore/iri2020/cira.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/igrf.for` & `iricore-1.4.3/src/iricore/iri2020/igrf.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/iridreg.for` & `iricore-1.4.3/src/iricore/iri2020/iridreg.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/iriflip.for` & `iricore-1.4.3/src/iricore/iri2020/iriflip.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/irifun.for` & `iricore-1.4.3/src/iricore/iri2020/irifun.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/irirtam.for` & `iricore-1.4.3/src/iricore/iri2020/irirtam.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/irisub.for` & `iricore-1.4.3/src/iricore/iri2020/irisub.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/iritec.for` & `iricore-1.4.3/src/iricore/iri2020/iritec.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/iri2020/rocdrift.for` & `iricore-1.4.3/src/iricore/iri2020/rocdrift.for`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/modules.py` & `iricore-1.4.3/src/iricore/modules.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/python_interface.f90` & `iricore-1.4.3/src/iricore/python_interface.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/python_stec.f90` & `iricore-1.4.3/src/iricore/python_stec.f90`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/src/iricore/read_iri_data.py` & `iricore-1.4.3/src/iricore/read_iri_data.py`

 * *Files identical despite different names*

### Comparing `iricore-1.4.2/setup.py` & `iricore-1.4.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,24 +5,15 @@
 {'': 'src'}
 
 packages = \
 ['iricore']
 
 package_data = \
 {'': ['*'],
- 'iricore': ['CMakeFiles/*',
-             'CMakeFiles/3.26.3/*',
-             'CMakeFiles/3.26.3/CompilerIdC/*',
-             'CMakeFiles/3.26.3/CompilerIdCXX/*',
-             'CMakeFiles/3.26.3/CompilerIdFortran/*',
-             'CMakeFiles/iri2016.dir/*',
-             'CMakeFiles/iri2016.dir/iri2016/*',
-             'CMakeFiles/iri2020.dir/*',
-             'CMakeFiles/iri2020.dir/iri2020/*',
-             'data/data16/ccir/*',
+ 'iricore': ['data/data16/ccir/*',
              'data/data16/igrf/*',
              'data/data16/index/*',
              'data/data16/mcsat/*',
              'data/data16/ursi/*',
              'data/data20/ccir/*',
              'data/data20/igrf/*',
              'data/data20/index/*',
@@ -32,15 +23,15 @@
              'iri2020/*']}
 
 install_requires = \
 ['fortranformat>=1.2.2,<2.0.0', 'numpy>=1.22,<2.0', 'pymap3d>=3.0.1,<4.0.0']
 
 setup_kwargs = {
     'name': 'iricore',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': '',
     'long_description': '# iricore\nA Python interface to IRI-2016 and IRI-2020 using `ctypes` communication.\n\n**Important!** Because this package is mainly used for the [MIST experiment](http://www.physics.mcgill.ca/mist/), \nthe `iricore` cuts off calculation of unnecessary atmospheric parameters available in IRI-2016, leaving only electron density\nand electron temperature. All other parameters can be restored on demand (please contact me).\n\n## Installation\n\nThis package proved to work under Linux only (due to compilation difficulties in Windows). \nIf you are using Windows - consider installing [WSL](https://docs.microsoft.com/en-us/windows/wsl/install).\n\n### Prerequisites\n- CMAKE\n```\nsudo apt instal cmake\n```\n\n- Fortran compiler, e.g. `gfortran`\n```\nsudo apt isntall gfortran\n```\n\n### Installing package\nNow you can simply install it via `pip`:\n\n```\npython3 -m pip install iricore\n```\n\n## Data files\n`IRI2016` model depends on [data files](http://irimodel.org/indices/) which are regularly updated.\n`iricore` does not autoupdate those, but provides tool for quick update. You can run from terminal\n```\npython3 -c "import iricore; iricore.update()"\n```\n\nor add\n\n```\nimport iricore\niricore.update()\n```\nto any Python script.\n\n## Usage\nFor usage examples see `examples/`.',
     'author': 'Vadym Bidula',
     'author_email': 'vadym.bidula@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `iricore-1.4.2/PKG-INFO` & `iricore-1.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iricore
-Version: 1.4.2
+Version: 1.4.3
 Summary: 
 Author: Vadym Bidula
 Author-email: vadym.bidula@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

