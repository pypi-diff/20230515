# Comparing `tmp/justbases-0.6.tar.gz` & `tmp/justbases-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/justbases-0.6.tar", last modified: Thu Mar 17 15:04:13 2016, max compression
+gzip compressed data, was "dist/justbases-0.9.tar", last modified: Tue Aug  2 12:37:48 2016, max compression
```

## Comparing `justbases-0.6.tar` & `justbases-0.9.tar`

### file list

```diff
@@ -1,109 +1,118 @@
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1953 2016-03-17 15:01:01.000000 justbases-0.6/README.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2016-01-05 13:41:16.000000 justbases-0.6/tests/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1213 2016-03-03 16:09:50.000000 justbases-0.6/tests/test_constants.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3689 2016-02-23 16:10:15.000000 justbases-0.6/tests/test_nats.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1186 2016-02-23 16:10:15.000000 justbases-0.6/tests/_utils.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6790 2016-03-03 16:09:50.000000 justbases-0.6/tests/test_rationals.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7999 2016-03-03 16:09:50.000000 justbases-0.6/tests/test_division.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11388 2016-03-17 15:01:01.000000 justbases-0.6/tests/test_radix.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3159 2016-03-17 15:04:13.000000 justbases-0.6/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    18047 2016-01-05 13:41:16.000000 justbases-0.6/LICENSE
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       59 2016-03-17 15:04:13.000000 justbases-0.6/setup.cfg
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/src/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/src/justbases.egg-info/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3159 2016-03-17 15:03:00.000000 justbases-0.6/src/justbases.egg-info/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2016-03-17 15:03:00.000000 justbases-0.6/src/justbases.egg-info/requires.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4547 2016-03-17 15:03:00.000000 justbases-0.6/src/justbases.egg-info/SOURCES.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2016-03-17 15:03:00.000000 justbases-0.6/src/justbases.egg-info/dependency_links.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       10 2016-03-17 15:03:00.000000 justbases-0.6/src/justbases.egg-info/top_level.txt
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/src/justbases/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1256 2016-03-17 15:01:01.000000 justbases-0.6/src/justbases/version.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1826 2016-03-03 16:09:50.000000 justbases-0.6/src/justbases/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2421 2016-02-16 13:47:42.000000 justbases-0.6/src/justbases/_errors.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11498 2016-03-14 14:54:06.000000 justbases-0.6/src/justbases/_division.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    21109 2016-03-17 15:01:01.000000 justbases-0.6/src/justbases/_rationals.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4946 2016-03-14 14:54:06.000000 justbases-0.6/src/justbases/_nats.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2277 2016-03-14 14:54:06.000000 justbases-0.6/src/justbases/_constants.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      541 2016-02-23 16:10:15.000000 justbases-0.6/tox.ini
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2077 2016-03-14 14:54:06.000000 justbases-0.6/setup.py
--rwxrwxr-x   0 mulhern   (1000) mulhern   (1000)     1445 2016-03-14 13:54:29.000000 justbases-0.6/check.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      225 2016-03-17 15:01:01.000000 justbases-0.6/MANIFEST.in
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/_build/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/_build/html/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    31558 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/usage.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6539 2016-03-17 14:58:17.000000 justbases-0.6/doc/_build/html/index.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3419 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/search.html
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/_build/html/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5693 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.test_constants.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6893 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.test_nats.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5362 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/modules.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    12138 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.test_radix.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7584 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.test_division.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5117 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests._utils.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6911 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.test_rationals.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5778 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/tests/tests.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6703 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/py-modindex.html
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/_build/html/justbases/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8893 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases._division.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5198 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases.version.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5421 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/modules.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8160 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases._constants.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    12556 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases._nats.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6781 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    14136 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases._rationals.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7425 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/justbases/justbases._errors.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    19263 2016-03-17 14:58:18.000000 justbases-0.6/doc/_build/html/genindex.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5850 2016-03-17 14:58:17.000000 justbases-0.6/doc/_build/html/intro.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7245 2016-03-03 16:09:50.000000 justbases-0.6/doc/usage.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.test_constants.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.test_nats.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      305 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       52 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/modules.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      127 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests._utils.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.test_rationals.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      148 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.test_division.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      139 2016-03-17 14:58:15.000000 justbases-0.6/doc/tests/tests.test_radix.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9256 2016-01-05 13:51:19.000000 justbases-0.6/doc/conf.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/.hypothesis/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/.hypothesis/eval_source/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_3f7411c21a40bfdc1d4a385395abcf8f35bfc403.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      222 2016-02-16 13:52:44.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_c0dbfca2f61e160f27c3d04f89f8449ac48e812c.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      138 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_f921b2988402df61d5f91622b67a9e50eddd05fc.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_ad3b1319e5371eb5b80a0f4b62a10c1d78021704.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      280 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_157a06c7111ab0b1f1a33822a57773ed79d45d30.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_b73c993cdef867012386b0a19d203d196a83d57e.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_84deb0667079aa1ef02457217332c31964ecca97.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_5a7bc10d8015157dedbac1465811f364be31ca17.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_1eba03841185292c6018ae372c9f399bb5b99054.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      166 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_b36dd06da9eb78c3d228115624957bc5c74f5af3.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_575c46161da71f5baee220ccac6c2069d30f4506.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      126 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_0338617ff66788f1ab9d5142f849106ae9b38d15.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      208 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_cdc3a7a5201e39632a956c5967c0a91af8267df9.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      264 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_302a2bf2b98d37c182da92de76c16ff408d9447c.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      260 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_e7ac20823eddd3e706aaf44693170920005cb871.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      130 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_319ade46afdab08a61611170bc661bd6b6fd0507.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      122 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_2cea1af442c7f053fe19b734be9a6a80bbafb877.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_0529b12987b897d7290f83bcbcc804e28602383d.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2016-02-16 13:52:44.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_dadf8f3e0c156227cf67f0925dd68724db27fc13.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_9345cdfcc00c612f74fd583fd23cd20cd7a11cc7.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_a993f5cddd9d22f6beea0e79bc1785a8f6f492c7.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      244 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_2e71923a5f523fc7899142bce080a648f473d503.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_53115b42a52392c3b9505509489ca172fd59d631.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      116 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_9abd2800900986980ad8f68a32f0005fc05800d8.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2016-03-03 16:10:49.000000 justbases-0.6/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8478d2d985b5b4bb830f8419c093e22c692e027.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      431 2016-01-05 13:51:19.000000 justbases-0.6/doc/index.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-03-17 15:04:13.000000 justbases-0.6/doc/justbases/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases._nats.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases._rationals.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases.version.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       64 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/modules.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      148 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases._division.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      323 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases._errors.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-03-17 14:58:15.000000 justbases-0.6/doc/justbases/justbases._constants.rst
-lrwxrwxrwx   0 mulhern   (1000) mulhern   (1000)        0 2016-01-05 13:51:19.000000 justbases-0.6/doc/intro.rst -> ../README.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2016-01-05 13:41:16.000000 justbases-0.6/requirements.txt
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1957 2016-08-02 12:07:18.000000 justbases-0.9/README.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2016-01-05 13:41:16.000000 justbases-0.9/tests/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1213 2016-03-03 16:09:50.000000 justbases-0.9/tests/test_constants.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3783 2016-08-02 12:06:04.000000 justbases-0.9/tests/test_nats.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4546 2016-08-01 19:07:08.000000 justbases-0.9/tests/test_display.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3561 2016-05-12 15:25:44.000000 justbases-0.9/tests/_utils.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6796 2016-05-09 13:09:52.000000 justbases-0.9/tests/test_rationals.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8109 2016-05-12 15:25:44.000000 justbases-0.9/tests/test_division.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8645 2016-05-12 15:25:44.000000 justbases-0.9/tests/test_radix.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3190 2016-08-02 12:37:48.000000 justbases-0.9/PKG-INFO
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    18047 2016-01-05 13:41:16.000000 justbases-0.9/LICENSE
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       59 2016-08-02 12:37:48.000000 justbases-0.9/setup.cfg
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/src/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/src/justbases.egg-info/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3190 2016-08-02 12:37:45.000000 justbases-0.9/src/justbases.egg-info/PKG-INFO
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2016-08-02 12:37:45.000000 justbases-0.9/src/justbases.egg-info/requires.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4871 2016-08-02 12:37:46.000000 justbases-0.9/src/justbases.egg-info/SOURCES.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2016-08-02 12:37:45.000000 justbases-0.9/src/justbases.egg-info/dependency_links.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       10 2016-08-02 12:37:45.000000 justbases-0.9/src/justbases.egg-info/top_level.txt
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/src/justbases/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1256 2016-08-02 12:35:50.000000 justbases-0.9/src/justbases/version.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2058 2016-05-13 12:28:28.000000 justbases-0.9/src/justbases/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2421 2016-03-18 14:51:49.000000 justbases-0.9/src/justbases/_errors.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11498 2016-04-21 19:46:16.000000 justbases-0.9/src/justbases/_division.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5671 2016-05-13 12:28:28.000000 justbases-0.9/src/justbases/_config.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    21751 2016-05-24 14:06:47.000000 justbases-0.9/src/justbases/_rationals.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4946 2016-04-21 12:30:34.000000 justbases-0.9/src/justbases/_nats.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2277 2016-04-21 12:30:34.000000 justbases-0.9/src/justbases/_constants.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9317 2016-08-01 19:07:08.000000 justbases-0.9/src/justbases/_display.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      568 2016-08-01 19:07:08.000000 justbases-0.9/tox.ini
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2072 2016-08-02 12:35:50.000000 justbases-0.9/setup.py
+-rwxrwxr-x   0 mulhern   (1000) mulhern   (1000)     1445 2016-03-14 13:54:29.000000 justbases-0.9/check.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      225 2016-03-18 14:53:03.000000 justbases-0.9/MANIFEST.in
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/_build/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/_build/html/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    31563 2016-05-09 14:26:43.000000 justbases-0.9/doc/_build/html/usage.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6658 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/index.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3424 2016-05-09 14:26:43.000000 justbases-0.9/doc/_build/html/search.html
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/_build/html/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5690 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.test_constants.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6951 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.test_nats.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8111 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.test_display.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5486 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/modules.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    10500 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.test_radix.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7573 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.test_division.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9217 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests._utils.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6916 2016-05-09 14:26:43.000000 justbases-0.9/doc/_build/html/tests/tests.test_rationals.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5902 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/tests/tests.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7385 2016-05-09 14:26:43.000000 justbases-0.9/doc/_build/html/py-modindex.html
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/_build/html/justbases/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8882 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._division.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5203 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases.version.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5662 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/modules.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8217 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._constants.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    12561 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._nats.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    15633 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._display.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6998 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    15085 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._rationals.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9509 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._config.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7430 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/justbases/justbases._errors.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    24438 2016-05-09 14:26:43.000000 justbases-0.9/doc/_build/html/genindex.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7435 2016-05-09 14:26:42.000000 justbases-0.9/doc/_build/html/intro.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7692 2016-08-02 12:28:37.000000 justbases-0.9/doc/usage.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_constants.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      145 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_display.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_nats.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      327 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       52 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/modules.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      127 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests._utils.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_rationals.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      148 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_division.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      139 2016-05-09 14:26:39.000000 justbases-0.9/doc/tests/tests.test_radix.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9256 2016-01-05 13:51:19.000000 justbases-0.9/doc/conf.py
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/.hypothesis/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/.hypothesis/eval_source/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_3f7411c21a40bfdc1d4a385395abcf8f35bfc403.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      222 2016-02-16 13:52:44.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_c0dbfca2f61e160f27c3d04f89f8449ac48e812c.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      138 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f921b2988402df61d5f91622b67a9e50eddd05fc.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_ad3b1319e5371eb5b80a0f4b62a10c1d78021704.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      280 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_157a06c7111ab0b1f1a33822a57773ed79d45d30.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_b73c993cdef867012386b0a19d203d196a83d57e.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_84deb0667079aa1ef02457217332c31964ecca97.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_5a7bc10d8015157dedbac1465811f364be31ca17.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_1eba03841185292c6018ae372c9f399bb5b99054.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      166 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_b36dd06da9eb78c3d228115624957bc5c74f5af3.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_575c46161da71f5baee220ccac6c2069d30f4506.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      126 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_0338617ff66788f1ab9d5142f849106ae9b38d15.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      208 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_cdc3a7a5201e39632a956c5967c0a91af8267df9.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      264 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_302a2bf2b98d37c182da92de76c16ff408d9447c.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      260 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e7ac20823eddd3e706aaf44693170920005cb871.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      130 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_319ade46afdab08a61611170bc661bd6b6fd0507.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      122 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_2cea1af442c7f053fe19b734be9a6a80bbafb877.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_0529b12987b897d7290f83bcbcc804e28602383d.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2016-02-16 13:52:44.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_dadf8f3e0c156227cf67f0925dd68724db27fc13.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9345cdfcc00c612f74fd583fd23cd20cd7a11cc7.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_a993f5cddd9d22f6beea0e79bc1785a8f6f492c7.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      244 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_2e71923a5f523fc7899142bce080a648f473d503.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_53115b42a52392c3b9505509489ca172fd59d631.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      116 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9abd2800900986980ad8f68a32f0005fc05800d8.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2016-03-03 16:10:49.000000 justbases-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8478d2d985b5b4bb830f8419c093e22c692e027.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      431 2016-01-05 13:51:19.000000 justbases-0.9/doc/index.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-08-02 12:37:48.000000 justbases-0.9/doc/justbases/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._nats.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      145 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._display.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._rationals.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._config.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases.version.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       64 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/modules.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      148 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._division.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      366 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._errors.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:39.000000 justbases-0.9/doc/justbases/justbases._constants.rst
+lrwxrwxrwx   0 mulhern   (1000) mulhern   (1000)        0 2016-01-05 13:51:19.000000 justbases-0.9/doc/intro.rst -> ../README.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2016-01-05 13:41:16.000000 justbases-0.9/requirements.txt
```

### Comparing `justbases-0.6/README.rst` & `justbases-0.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,24 +24,28 @@
 With respect to division in an arbitrary base, the complexity is bounded
 by the value of the divisor, unless a precision limit is set.
 
 Related Packages
 ----------------
 
 * allyourbase: https://pypi.python.org/pypi/allyourbase
+
   Converts a variety of numeric types to str in arbitrary bases.
   Does not require one character to digit encoding, uses a digit separator.
   Requires rounding, does not do precise conversion, but does do
   conversion to any specified precision.
 
 * python-baseconv: https://pypi.python.org/pypi/allyourbase
+
   Converts an int to a string using a one character to digit encoding.
   Also converts in the opposite direction.
   Does not handle arbitrary rationals and does not really handle conversion to
   large bases, e.g., 1024, as such conversion would require 1024 distinct
   characters.
 
 * python-radix: https://pypi.python.org/pypi/python-radix
+
   Does not handle arbitrary bases. Converts int or int as str to str.
 
 * numpy: http://docs.scipy.org/doc/numpy/reference/
+
   Converts int to str in bases between 2 and 36.
```

### Comparing `justbases-0.6/tests/test_constants.py` & `justbases-0.9/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/tests/test_nats.py` & `justbases-0.9/tests/test_nats.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,16 +36,18 @@
     @given(
        strategies.integers(min_value=0),
        strategies.integers(min_value=2),
     )
     def testFromInt(self, value, to_base):
         """
         convert_to_int(convert_from_int(value, to_base), 10) == value
+        No leading zeros in convert_from_int(value, to_base)
         """
         result = Nats.convert_from_int(value, to_base)
+        assert result[:1] != [0]
         assert Nats.convert_to_int(result, to_base) == value
 
     @given(
        _NATS_STRATEGY,
        strategies.integers(min_value=2, max_value=64)
     )
     def testFromOther(self, nat, to_base):
```

### Comparing `justbases-0.6/tests/test_rationals.py` & `justbases-0.9/tests/test_rationals.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     )
     @settings(max_examples=50)
     def testInverses(self, value, to_base):
         """
         Test that functions are inverses of each other.
         """
         (result, relation) = Radices.from_rational(value, to_base)
-        assert result.positive or value < 0
+        assert result.sign in (0, 1) or value < 0
         assert relation == 0
         assert result.as_rational() == value
 
     @given(
        strategies.fractions().map(lambda x: x.limit_denominator(100)),
        strategies.integers(min_value=2, max_value=64),
        strategies.integers(min_value=0, max_value=64),
```

### Comparing `justbases-0.6/tests/test_division.py` & `justbases-0.9/tests/test_division.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
         (denominator, numerator) = NatDivision.undivision(
            integer_part,
            non_repeating_part,
            repeating_part,
            base
         )
+        assert numerator == [] or numerator[0] != 0
+        assert denominator != [] and denominator[0] != 0
+
         original = fractions.Fraction(
            Nats.convert_to_int(dividend, base),
            Nats.convert_to_int(divisor, base)
         )
         result = fractions.Fraction(
            Nats.convert_to_int(numerator, base),
            Nats.convert_to_int(denominator, base)
```

### Comparing `justbases-0.6/tests/test_radix.py` & `justbases-0.9/tests/test_radix.py`

 * *Files 19% similar despite different names*

```diff
@@ -20,113 +20,109 @@
 import unittest
 
 from hypothesis import given
 from hypothesis import settings
 from hypothesis import strategies
 
 from justbases import BasesError
-from justbases import Radices
 from justbases import Radix
 from justbases import Rationals
 from justbases import RoundingMethods
 
+from ._utils import build_base
+from ._utils import build_radix
+
 
 class RadixTestCase(unittest.TestCase):
     """ Tests for radix. """
 
     @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2),
-       strategies.integers(min_value=2)
+       build_radix(16, 3),
+       build_base(16)
     )
     @settings(max_examples=50)
-    def testInBase(self, value, base1, base2):
-        """
-        Test that roundtrip is identity.
-        """
-        (radix, _) = Radices.from_rational(value, base1)
-        radix2 = radix.in_base(base2)
-        radix3 = radix2.in_base(base1)
-        assert radix == radix3
-
-    @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2)
-    )
-    def testInBase2(self, value, base):
+    def testInBase(self, radix, base):
         """
-        Test conversion to current base.
+        Test that roundtrip is identity modulo number of 0s in
+        non repeating part.
         """
-        (radix, _) = Radices.from_rational(value, base)
-        result = radix.in_base(base)
-        assert radix == result
+        result = radix.in_base(base).in_base(radix.base)
+        assert result.sign == radix.sign and \
+           result.integer_part == radix.integer_part and \
+           result.repeating_part == radix.repeating_part and \
+           result.base == radix.base
+
+        length = len(result.non_repeating_part)
+        assert result.non_repeating_part == radix.non_repeating_part[:length]
+        assert all(x == 0 for x in radix.non_repeating_part[length:])
 
     def testExceptions(self):
         """
         Test exceptions.
         """
         with self.assertRaises(BasesError):
-            Radix(True, [], [], [], 0)
+            Radix(0, [], [], [], 0)
         with self.assertRaises(BasesError):
-            Radix(True, [], [], [2], 2)
+            Radix(1, [], [], [2], 2)
         with self.assertRaises(BasesError):
-            Radix(True, [], [-1], [1], 2)
+            Radix(1, [], [-1], [1], 2)
         with self.assertRaises(BasesError):
-            Radix(True, [-300], [1], [1], 2)
+            Radix(1, [-300], [1], [1], 2)
         with self.assertRaises(BasesError):
-            Radix(True, [1], [0], [1], 2).in_base(0)
+            Radix(True, [1], [0], [1], 2)
+        with self.assertRaises(BasesError):
+            Radix(1, [1], [0], [1], 2).in_base(0)
 
-    def testStr(self):
+    @given(build_radix(36, 10))
+    @settings(max_examples=10)
+    def testStr(self, radix):
         """
-        Make sure that __str__ executes.
+        Check basic properties of __str__.
         """
-        assert str(Radix(True, [1], [2], [3], 4)) != ''
+        result = str(radix)
+        assert result.startswith("-") == (radix.sign == -1)
 
-    @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2)
-    )
+    @given(build_radix(1024, 10))
     @settings(max_examples=10)
-    def testRepr(self, value, base):
+    def testRepr(self, radix):
         """
         Make sure that result is evalable.
         """
-        (radix, _) = Radices.from_rational(value, base)
         assert eval(repr(radix)) == radix # pylint: disable=eval-used
 
     def testOptions(self):
         """
         Skip validation and canonicalization.
         """
-        self.assertIsNotNone(Radix(False, [], [], [], 4, False, False))
+        self.assertIsNotNone(Radix(-1, [], [], [], 4, False, False))
 
     def testEquality(self):
         """
         Test == operator.
         """
         self.assertEqual(
-           Radix(True, [1], [], [], 2),
-           Radix(True, [1], [], [], 2),
+           Radix(1, [1], [], [], 2),
+           Radix(1, [1], [], [], 2),
         )
 
     def testInEquality(self):
         """
         Test != operator.
         """
         self.assertNotEqual(
-           Radix(False, [], [], [], 3),
-           Radix(True, [], [], [], 2),
+           Radix(0, [], [], [], 3),
+           Radix(0, [], [], [], 2),
         )
 
     def testOperatorExceptions(self):
         """
         Test that comparsion operators yield exceptions.
         """
-        radix1 = Radix(False, [], [], [], 3)
-        radix2 = Radix(False, [], [], [], 2)
+        radix1 = Radix(0, [], [], [], 3)
+        radix2 = Radix(0, [], [], [], 2)
         # pylint: disable=pointless-statement
         with self.assertRaises(BasesError):
             radix1 > radix2
         with self.assertRaises(BasesError):
             radix1 < radix2
         with self.assertRaises(BasesError):
             radix1 <= radix2
@@ -135,52 +131,57 @@
         with self.assertRaises(BasesError):
             radix1 >= 1
         with self.assertRaises(BasesError):
             radix1 == 1
         with self.assertRaises(BasesError):
             radix1 != 1
 
+    def testCarryOnRepeatingPart(self):
+        """
+        Carry from non_repeating_part to integer_part and then out.
+        """
+        assert Radix(1, [3], [3], [3], 4) == Radix(1, [1, 0], [], [], 4)
+
     def testRepeatingRepeatPart(self):
         """
         Repeat part is made up of repeating parts.
         """
-        radix = Radix(True, [], [], [1, 1], 4)
+        radix = Radix(1, [], [], [1, 1], 4)
         self.assertEqual(radix.repeating_part, [1])
-        radix = Radix(True, [], [], [1, 1, 2], 4)
+        radix = Radix(1, [], [], [1, 1, 2], 4)
         self.assertEqual(radix.repeating_part, [1, 1, 2])
-        radix = Radix(True, [], [], [1, 2, 1, 2, 1, 2], 4)
+        radix = Radix(1, [], [], [1, 2, 1, 2, 1, 2], 4)
         self.assertEqual(radix.repeating_part, [1, 2])
-        radix = Radix(True, [], [3, 1, 2, 1, 2], [1, 2], 4)
+        radix = Radix(1, [], [3, 1, 2, 1, 2], [1, 2], 4)
         self.assertEqual(radix.non_repeating_part, [3])
         self.assertEqual(radix.repeating_part, [1, 2])
-        radix = Radix(True, [], [3, 2, 1, 2, 1, 2], [1, 2], 4)
+        radix = Radix(1, [], [3, 2, 1, 2, 1, 2], [1, 2], 4)
         self.assertEqual(radix.non_repeating_part, [3])
         self.assertEqual(radix.repeating_part, [2, 1])
-        radix = Radix(True, [], [3, 3, 2, 3, 1, 2, 3, 1, 2, 3], [1, 2, 3], 4)
+        radix = Radix(1, [], [3, 3, 2, 3, 1, 2, 3, 1, 2, 3], [1, 2, 3], 4)
         self.assertEqual(radix.non_repeating_part, [3, 3])
         self.assertEqual(radix.repeating_part, [2, 3, 1])
 
 
 class RoundingTestCase(unittest.TestCase):
     """ Tests for rounding Radixes. """
 
     @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2, max_value=64),
+       build_radix(16, 10),
        strategies.integers(min_value=0, max_value=64),
        strategies.sampled_from(RoundingMethods.METHODS())
     )
-    @settings(max_examples=500)
-    def testRoundFraction(self, value, base, precision, method):
+    @settings(max_examples=50)
+    def testRoundFraction(self, radix, precision, method):
         """
         Test that rounding yields the correct number of digits.
 
         Test that rounded values are in a good range.
         """
-        (radix, _) = Radices.from_rational(value, base)
+        value = radix.as_rational()
         (result, relation) = radix.rounded(precision, method)
         assert len(result.non_repeating_part) == precision
 
         ulp = Fraction(1, radix.base ** precision)
         rational_result = result.as_rational()
         assert value - ulp <= rational_result
         assert value + ulp >= rational_result
@@ -189,32 +190,31 @@
             assert relation == 1
         elif rational_result < value:
             assert relation == -1
         else:
             assert relation == 0
 
     @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2, max_value=64),
+       build_radix(16, 10),
        strategies.integers(min_value=0, max_value=64)
     )
     @settings(max_examples=50)
-    def testRoundRelation(self, value, base, precision):
+    def testRoundRelation(self, radix, precision):
         """
         Test that all results have the correct relation.
         """
-        (radix, _) = Radices.from_rational(value, base)
-
-
         results = dict(
            (method, radix.rounded(precision, method)[0]) for \
               method in RoundingMethods.METHODS()
         )
 
-        if radix.positive is True:
+        for _, result in results.items():
+            assert len(result.non_repeating_part) == precision
+
+        if radix.sign in (0, 1):
             assert results[RoundingMethods.ROUND_DOWN] == \
                results[RoundingMethods.ROUND_TO_ZERO]
             assert results[RoundingMethods.ROUND_HALF_DOWN] == \
                results[RoundingMethods.ROUND_HALF_ZERO]
         else:
             assert results[RoundingMethods.ROUND_UP] == \
                results[RoundingMethods.ROUND_TO_ZERO]
@@ -228,108 +228,33 @@
            RoundingMethods.ROUND_DOWN
         ]
         for index in range(len(order) - 1):
             assert results[order[index]].as_rational() >= \
                results[order[index + 1]].as_rational()
 
     @given(
-       strategies.fractions().map(lambda x: x.limit_denominator(100)),
-       strategies.integers(min_value=2, max_value=64),
+       build_radix(64, 5),
        strategies.sampled_from(RoundingMethods.METHODS())
     )
     @settings(max_examples=50)
-    def testAsInt(self, value, base, method):
+    def testAsInt(self, radix, method):
         """
         Test equivalence with two paths.
         """
-        (radix, _) = Radices.from_rational(value, base)
         result1 = Rationals.round_to_int(radix.as_rational(), method)
         result2 = radix.as_int(method)
         assert result1 == result2
 
-    def testOverflow(self):
-        """
-        Ensure that rounding causes overflow.
-        """
-        radix = Radix(True, [], [], [1], 2)
-        (result, relation) = radix.rounded(3, RoundingMethods.ROUND_UP)
-        assert relation == 1
-        assert result.integer_part == [1]
-        assert result.non_repeating_part == [0, 0, 0]
-        assert result.repeating_part == []
-
-    def testMiddles(self):
-        """
-        Ensure that there is no tie breaker.
-        """
-        radix = Radix(True, [], [1, 1, 1, 1], [], 2)
-        (result, relation) = radix.rounded(3, RoundingMethods.ROUND_HALF_UP)
-        assert relation == 1
-        assert result.integer_part == [1]
-        assert result.non_repeating_part == [0, 0, 0]
-        assert result.repeating_part == []
-
-    def testLeadingZeros(self):
-        """
-        Require conversion, but do not carry out of repeating_part.
-        """
-        radix = Radix(True, [], [0, 0, 1, 1], [], 2)
-        (result, relation) = radix.rounded(3, RoundingMethods.ROUND_UP)
-        assert relation == 1
-        assert result.integer_part == []
-        assert result.non_repeating_part == [0, 1, 0]
-        assert result.repeating_part == []
-
-    def testExactLength(self):
-        """
-        Require conversion, but do not carry out of repeating_part.
-        Ensure that the intermediate result is exactly the required
-        precision.
-        """
-        radix = Radix(True, [], [1, 0, 1, 1], [], 2)
-        (result, relation) = radix.rounded(3, RoundingMethods.ROUND_UP)
-        assert relation == 1
-        assert result.integer_part == []
-        assert result.non_repeating_part == [1, 1, 0]
-        assert result.repeating_part == []
-
     def testExceptions(self):
         """
         Test exception.
         """
         with self.assertRaises(BasesError):
-            Radix(True, [], [], [], 2).rounded(
+            Radix(0, [], [], [], 2).rounded(
                -1,
                RoundingMethods.ROUND_DOWN
             )
         with self.assertRaises(BasesError):
-            Radix(True, [], [], [], 2).rounded(
+            Radix(0, [], [], [], 2).rounded(
                0,
                None
             )
-
-    def testFiveEighths(self):
-        """
-        Test 5/8 in base 3.
-        """
-        value = Fraction(5, 8)
-        (radix, _) = Radices.from_rational(value, 3)
-        (rounded, relation) = radix.rounded(0, RoundingMethods.ROUND_HALF_UP)
-
-        assert relation == 1
-        assert rounded.as_rational() == 1
-
-    def testOneHalf(self):
-        """
-        Test 1/2 in base 3.
-        """
-        value = Fraction(1, 2)
-        (radix, _) = Radices.from_rational(value, 3)
-        (rounded, relation) = radix.rounded(0, RoundingMethods.ROUND_HALF_UP)
-
-        assert relation == 1
-        assert rounded.as_rational() == 1
-
-        (rounded, relation) = radix.rounded(0, RoundingMethods.ROUND_HALF_DOWN)
-
-        assert relation == -1
-        assert rounded.as_rational() == 0
```

### Comparing `justbases-0.6/PKG-INFO` & `justbases-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: justbases
-Version: 0.6
+Version: 0.9
 Summary: conversion of ints and rationals to any base
 Home-page: UNKNOWN
 Author: Anne Mulhern
 Author-email: mulhern@cs.wisc.edu
 License: GPL 2+
 Description: Justbases
         =========
@@ -32,34 +32,38 @@
         With respect to division in an arbitrary base, the complexity is bounded
         by the value of the divisor, unless a precision limit is set.
         
         Related Packages
         ----------------
         
         * allyourbase: https://pypi.python.org/pypi/allyourbase
+        
           Converts a variety of numeric types to str in arbitrary bases.
           Does not require one character to digit encoding, uses a digit separator.
           Requires rounding, does not do precise conversion, but does do
           conversion to any specified precision.
         
         * python-baseconv: https://pypi.python.org/pypi/allyourbase
+        
           Converts an int to a string using a one character to digit encoding.
           Also converts in the opposite direction.
           Does not handle arbitrary rationals and does not really handle conversion to
           large bases, e.g., 1024, as such conversion would require 1024 distinct
           characters.
         
         * python-radix: https://pypi.python.org/pypi/python-radix
+        
           Does not handle arbitrary bases. Converts int or int as str to str.
         
         * numpy: http://docs.scipy.org/doc/numpy/reference/
+        
           Converts int to str in bases between 2 and 36.
         
 Platform: Linux
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `justbases-0.6/LICENSE` & `justbases-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `justbases-0.6/src/justbases.egg-info/PKG-INFO` & `justbases-0.9/src/justbases.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: justbases
-Version: 0.6
+Version: 0.9
 Summary: conversion of ints and rationals to any base
 Home-page: UNKNOWN
 Author: Anne Mulhern
 Author-email: mulhern@cs.wisc.edu
 License: GPL 2+
 Description: Justbases
         =========
@@ -32,34 +32,38 @@
         With respect to division in an arbitrary base, the complexity is bounded
         by the value of the divisor, unless a precision limit is set.
         
         Related Packages
         ----------------
         
         * allyourbase: https://pypi.python.org/pypi/allyourbase
+        
           Converts a variety of numeric types to str in arbitrary bases.
           Does not require one character to digit encoding, uses a digit separator.
           Requires rounding, does not do precise conversion, but does do
           conversion to any specified precision.
         
         * python-baseconv: https://pypi.python.org/pypi/allyourbase
+        
           Converts an int to a string using a one character to digit encoding.
           Also converts in the opposite direction.
           Does not handle arbitrary rationals and does not really handle conversion to
           large bases, e.g., 1024, as such conversion would require 1024 distinct
           characters.
         
         * python-radix: https://pypi.python.org/pypi/python-radix
+        
           Does not handle arbitrary bases. Converts int or int as str to str.
         
         * numpy: http://docs.scipy.org/doc/numpy/reference/
+        
           Converts int to str in bases between 2 and 36.
         
 Platform: Linux
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `justbases-0.6/src/justbases.egg-info/SOURCES.txt` & `justbases-0.9/src/justbases.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -37,58 +37,67 @@
 doc/.hypothesis/eval_source/hypothesis_temporary_module_f921b2988402df61d5f91622b67a9e50eddd05fc.py
 doc/_build/html/genindex.html
 doc/_build/html/index.html
 doc/_build/html/intro.html
 doc/_build/html/py-modindex.html
 doc/_build/html/search.html
 doc/_build/html/usage.html
+doc/_build/html/justbases/justbases._config.html
 doc/_build/html/justbases/justbases._constants.html
+doc/_build/html/justbases/justbases._display.html
 doc/_build/html/justbases/justbases._division.html
 doc/_build/html/justbases/justbases._errors.html
 doc/_build/html/justbases/justbases._nats.html
 doc/_build/html/justbases/justbases._rationals.html
 doc/_build/html/justbases/justbases.html
 doc/_build/html/justbases/justbases.version.html
 doc/_build/html/justbases/modules.html
 doc/_build/html/tests/modules.html
 doc/_build/html/tests/tests._utils.html
 doc/_build/html/tests/tests.html
 doc/_build/html/tests/tests.test_constants.html
+doc/_build/html/tests/tests.test_display.html
 doc/_build/html/tests/tests.test_division.html
 doc/_build/html/tests/tests.test_nats.html
 doc/_build/html/tests/tests.test_radix.html
 doc/_build/html/tests/tests.test_rationals.html
+doc/justbases/justbases._config.rst
 doc/justbases/justbases._constants.rst
+doc/justbases/justbases._display.rst
 doc/justbases/justbases._division.rst
 doc/justbases/justbases._errors.rst
 doc/justbases/justbases._nats.rst
 doc/justbases/justbases._rationals.rst
 doc/justbases/justbases.rst
 doc/justbases/justbases.version.rst
 doc/justbases/modules.rst
 doc/tests/modules.rst
 doc/tests/tests._utils.rst
 doc/tests/tests.rst
 doc/tests/tests.test_constants.rst
+doc/tests/tests.test_display.rst
 doc/tests/tests.test_division.rst
 doc/tests/tests.test_nats.rst
 doc/tests/tests.test_radix.rst
 doc/tests/tests.test_rationals.rst
 src/justbases/__init__.py
+src/justbases/_config.py
 src/justbases/_constants.py
+src/justbases/_display.py
 src/justbases/_division.py
 src/justbases/_errors.py
 src/justbases/_nats.py
 src/justbases/_rationals.py
 src/justbases/version.py
 src/justbases.egg-info/PKG-INFO
 src/justbases.egg-info/SOURCES.txt
 src/justbases.egg-info/dependency_links.txt
 src/justbases.egg-info/requires.txt
 src/justbases.egg-info/top_level.txt
 tests/__init__.py
 tests/_utils.py
 tests/test_constants.py
+tests/test_display.py
 tests/test_division.py
 tests/test_nats.py
 tests/test_radix.py
 tests/test_rationals.py
```

### Comparing `justbases-0.6/src/justbases/version.py` & `justbases-0.9/src/justbases/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     =================
 
     Version information.
 
     .. moduleauthor::  mulhern  <amulhern@redhat.com>
 """
 
-__version__ = '0.06'
+__version__ = '0.09'
 __version_info__ = tuple(int(x) for x in __version__.split('.'))
```

### Comparing `justbases-0.6/src/justbases/__init__.py` & `justbases-0.9/src/justbases/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,17 +29,27 @@
     - conversion between non-negative ints and sequences
     - conversion between sequences in one base to sequences in another
   * Radix -- representation of rational number as string of digits
   * Rationals
 
     - conversion between Rational and Radix objects
     - conversion between Radix objects in any base
+  * String -- display of Radices
 """
 
 from ._constants import RoundingMethods
+
+from ._config import BasesConfig
+from ._config import BaseConfig
+from ._config import DigitsConfig
+from ._config import DisplayConfig
+from ._config import StripConfig
+
+from ._display import String
+
 from ._division import NatDivision
 
 from ._errors import BasesError
 
 from ._nats import Nats
 
 from ._rationals import Radices
```

### Comparing `justbases-0.6/src/justbases/_errors.py` & `justbases-0.9/src/justbases/_errors.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/src/justbases/_division.py` & `justbases-0.9/src/justbases/_division.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/src/justbases/_rationals.py` & `justbases-0.9/src/justbases/_rationals.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 """
 import copy
 import itertools
 
 from fractions import Fraction
 
 from ._constants import RoundingMethods
+from ._config import BasesConfig
+from ._display import String
 from ._division import NatDivision
 from ._errors import BasesAssertError
 from ._errors import BasesInvalidOperationError
 from ._errors import BasesValueError
 from ._nats import Nats
 
 
@@ -76,18 +78,26 @@
         """
         if to_base < 2:
             raise BasesValueError(to_base, "to_base", "must be at least 2")
 
         if precision is not None and precision < 0:
             raise BasesValueError(precision, "precision", "must be at least 0")
 
-        positive = True if value >= 0 else False
+        if value == 0:
+            non_repeating_part = [] if precision is None else precision * [0]
+            return (Radix(0, [], non_repeating_part, [], to_base), 0)
+
+        if value < 0:
+            sign = -1
+        else:
+            sign = 1
+
         div_method = method
 
-        if positive is False:
+        if sign == -1:
             value = abs(value)
             div_method = cls._reverse_rounding_method(method)
 
         numerator = Nats.convert_from_int(value.numerator, to_base)
         denominator = Nats.convert_from_int(value.denominator, to_base)
 
         (integer_part, non_repeating_part, repeating_part, relation) = \
@@ -95,25 +105,24 @@
               denominator,
               numerator,
               to_base,
               precision,
               div_method
            )
 
+        relation = relation * sign
+
         result = Radix(
-           positive,
+           sign,
            integer_part,
            non_repeating_part,
            repeating_part,
            to_base
         )
 
-        if not positive:
-            relation = relation * -1
-
         if precision is not None:
             (result, rel) = result.rounded(precision, method)
             relation = relation if rel == 0 else rel
 
         return (result, relation)
 
 
@@ -189,24 +198,24 @@
        "_",
        "%(base)s"
     ])
 
     @classmethod
     def _validate( # pylint: disable=too-many-arguments
         cls,
-        positive, # pylint: disable=unused-argument
+        sign,
         integer_part,
         non_repeating_part,
         repeating_part,
         base
     ):
         """
         Check if radix is valid.
 
-        :param bool positive: True if value is positive, otherwise False
+        :param int sign: -1, 0, or 1 as appropriate
         :param integer_part: the part on the left side of the radix
         :type integer_part: list of int
         :param non_repeating_part: non repeating part on left side
         :type non_repeating_part: list of int
         :param repeating_part: repeating part
         :type repeating_part: list of int
         :param int base: base of the radix, must be at least 2
@@ -232,14 +241,22 @@
             return BasesValueError(
                repeating_part,
                "repeating_part",
                "values must be between 0 and %s" % base
             )
         if base < 2:
             return BasesValueError(base, "base", "must be at least 2")
+
+        if sign not in (-1, 0, 1) or sign is True or sign is False:
+            return BasesValueError(
+               sign,
+               "sign",
+               "must be an int between -1 and 1"
+            )
+
         return None
 
     @classmethod
     def _repeat_length(cls, part):
         """
         The length of the repeated portions of ``part``.
 
@@ -308,26 +325,26 @@
         return (
            non_repeating[:(end - index)],
            repeating[-index:] + repeating[:-index]
         )
 
     def __init__( # pylint: disable=too-many-arguments
         self,
-        positive,
+        sign,
         integer_part,
         non_repeating_part,
         repeating_part,
         base,
         validate=True,
         canonicalize=True
     ):
         """
         Initializer.
 
-        :param bool positive: True if value is positive, otherwise False
+        :param int sign: -1, 0, or 1 as appropriate
         :param integer_part: the part on the left side of the radix
         :type integer_part: list of int
         :param non_repeating_part: non repeating part on left side
         :type non_repeating_part: list of int
         :param repeating_part: repeating part
         :type repeating_part: list of int
         :param int base: base of the radix, must be at least 2
@@ -337,79 +354,89 @@
         Validation and canonicalization are expensive and may be omitted.
 
         Complexity: polynomial in number of digits if canonicalize is True,
         linear if validate is True, otherwise constant time
         """
         if validate:
             error = self._validate(
-               positive,
+               sign,
                integer_part,
                non_repeating_part,
                repeating_part,
                base
             )
             if error is not None:
                 raise error
 
         if canonicalize:
             if all(x == 0 for x in integer_part):
                 integer_part = []
 
+            repeating_part = \
+               repeating_part[0:self._repeat_length(repeating_part)]
+            (non_repeating_part, repeating_part) = \
+                self._canonicalize_fraction(non_repeating_part, repeating_part)
             if all(x == 0 for x in repeating_part):
                 repeating_part = []
 
+            if repeating_part == [base - 1]:
+                repeating_part = []
+                (carry_out, non_repeating_part) = \
+                   Nats.carry_in(non_repeating_part, 1, base)
+                if carry_out != 0:
+                    (carry_out, integer_part) = \
+                       Nats.carry_in(integer_part, 1, base)
+                    if carry_out != 0:
+                        integer_part = [carry_out] + integer_part
+
             if integer_part == [] and repeating_part == [] and \
                all(x == 0 for x in non_repeating_part):
-                positive = True
-
-            repeating_part = repeating_part[0:self._repeat_length(repeating_part)]
-            (non_repeating_part, repeating_part) = \
-                self._canonicalize_fraction(non_repeating_part, repeating_part)
+                sign = 0
 
-        self.positive = positive
+        self.sign = sign
         self.base = base
         self.integer_part = integer_part
         self.non_repeating_part = non_repeating_part
         self.repeating_part = repeating_part
 
+    def getString(self, config, relation=0):
+        """
+        Return a representation of a Radix according to config.
+
+        :param DisplayConfig config: configuration
+        :param int relation: the relation of this value to actual value
+        """
+        return String(config, self.base).xform(self, relation)
+
     def __str__(self):
-        return self._FMT_STR % \
-           {
-              'sign' : '' if self.positive else '-',
-              'left': ':'.join(str(x) for x in self.integer_part) or '0',
-              'radix' :
-                 '.' if self.non_repeating_part or self.repeating_part  else '',
-              'non_repeat' : ':'.join(str(x) for x in self.non_repeating_part),
-              'repeat' : ':'.join(str(x) for x in self.repeating_part),
-              'base': self.base
-           }
+        return self.getString(BasesConfig.DISPLAY_CONFIG, 0)
 
     def __repr__(self):
         return 'Radix(%s,%s,%s,%s,%s)' % \
            (
-              self.positive,
+              self.sign,
               self.integer_part,
               self.non_repeating_part,
               self.repeating_part,
               self.base
            )
 
     def __eq__(self, other):
         if not isinstance(other, Radix):
             raise BasesInvalidOperationError("!=", other)
-        return self.positive == other.positive and \
+        return self.sign == other.sign and \
            self.integer_part == other.integer_part and \
            self.non_repeating_part == other.non_repeating_part and \
            self.repeating_part == other.repeating_part and \
            self.base == other.base
 
     def __ne__(self, other):
         if not isinstance(other, Radix):
             raise BasesInvalidOperationError("!=", other)
-        return self.positive != other.positive or \
+        return self.sign != other.sign or \
            self.integer_part != other.integer_part or \
            self.non_repeating_part != other.non_repeating_part or \
            self.repeating_part != other.repeating_part or \
            self.base != other.base
 
     def __lt__(self, other):
         raise BasesInvalidOperationError("<")
@@ -421,24 +448,24 @@
         raise BasesInvalidOperationError("<=")
 
     def __ge__(self, other):
         raise BasesInvalidOperationError(">=")
 
     def __copy__(self): # pragma: no cover
         return Radix(
-           self.positive,
+           self.sign,
            self.integer_part,
            self.non_repeating_part,
            self.repeating_part,
            self.base
         )
 
     def __deepcopy__(self, memo):
         return Radix(
-           self.positive,
+           self.sign,
            self.integer_part[:],
            self.non_repeating_part[:],
            self.repeating_part[:],
            self.base
         )
 
     def as_rational(self):
@@ -455,29 +482,29 @@
               self.repeating_part,
               self.base
            )
         result = Fraction(
            Nats.convert_to_int(numerator, self.base),
            Nats.convert_to_int(denominator, self.base)
         )
-        return result * (1 if self.positive else -1)
+        return result * self.sign
 
     def as_int(self, method):
         """
         This value as an int, rounded according to ``method``.
 
         :param method: rounding method
         :raises BasesValueError: on bad parameters
 
         :returns: corresponding int value
         :rtype: int
         """
         (new_radix, relation) = self.rounded(0, method)
         value = Nats.convert_to_int(new_radix.integer_part, new_radix.base)
-        return (value * (1 if self.positive else -1), relation)
+        return (value * self.sign, relation)
 
     def rounded(self, precision, method):
         """
         This value with fractional part rounded to ``precision`` digits
         according to ``method``.
 
         :param int precision: number of digits in total
@@ -508,34 +535,34 @@
     """
     Rounding of radix objects.
     """
     # pylint: disable=too-few-public-methods
 
 
     @staticmethod
-    def _conditional_toward_zero(method, positive):
+    def _conditional_toward_zero(method, sign):
         """
         Whether to round toward zero.
 
         :param method: rounding method
         :type method: element of RoundingMethods.METHODS()
-        :bool positive: if value is positive
+        :param int sign: -1, 0, or 1 as appropriate
 
         Complexity: O(1)
         """
         return method is RoundingMethods.ROUND_HALF_ZERO or \
-           (method is RoundingMethods.ROUND_HALF_DOWN and positive) or \
-           (method is RoundingMethods.ROUND_HALF_UP and not positive)
+           (method is RoundingMethods.ROUND_HALF_DOWN and sign == 1) or \
+           (method is RoundingMethods.ROUND_HALF_UP and sign == -1)
 
     @staticmethod
-    def _increment(positive, integer_part, non_repeating_part, base):
+    def _increment(sign, integer_part, non_repeating_part, base):
         """
         Return an increment radix.
 
-        :param bool positive: positive if Radix is positive
+        :param int sign: -1, 0, or 1 as appropriate
         :param integer_part: the integer part
         :type integer_part: list of int
         :param non_repeating_part: the fractional part
         :type non_repeating_part: list of int
         :param int base: the base
 
         :returns: a Radix object with ``non_repeating_part`` rounded up
@@ -544,15 +571,15 @@
         Complexity: O(len(non_repeating_part + integer_part)
         """
         (carry, non_repeating_part) = \
            Nats.carry_in(non_repeating_part, 1, base)
         (carry, integer_part) = \
            Nats.carry_in(integer_part, carry, base)
         return Radix(
-           positive,
+           sign,
            integer_part if carry == 0 else [carry] + integer_part,
            non_repeating_part,
            [],
            base,
            False
         )
 
@@ -583,70 +610,73 @@
         if method not in RoundingMethods.METHODS():
             raise BasesValueError(
                method,
                "method",
                "must be one of RoundingMethod.METHODS()"
             )
 
+        if value.sign == 0:
+            return (Radix(0, [], precision * [0], [], value.base), 0)
+
         digits = itertools.chain(
            value.non_repeating_part,
            itertools.cycle(value.repeating_part)
         )
         non_repeating_part = list(itertools.islice(digits, 0, precision))
         non_repeating_part += (precision - len(non_repeating_part)) * [0]
 
         truncated = lambda: Radix(
-           value.positive,
+           value.sign,
            value.integer_part,
            non_repeating_part,
            [],
            value.base,
            False
         )
 
         incremented = lambda: cls._increment(
-           value.positive,
+           value.sign,
            value.integer_part,
            non_repeating_part,
            value.base
         )
 
         if all(x == 0 for x in value.non_repeating_part[precision:]) and \
            len(value.repeating_part) == 0:
             return (truncated(), 0)
 
         if method is RoundingMethods.ROUND_TO_ZERO:
-            return (truncated(), -1 if value.positive else 1)
+            return (truncated(), -1 * value.sign)
 
         if method is RoundingMethods.ROUND_DOWN:
-            return (truncated() if value.positive else incremented(), -1)
+            return (truncated() if value.sign == 1 else incremented(), -1)
 
         if method is RoundingMethods.ROUND_UP:
-            return (incremented() if value.positive else truncated(), 1)
+            return (incremented() if value.sign == 1 else truncated(), 1)
 
         non_repeating_remainder = value.non_repeating_part[precision:]
         if non_repeating_remainder == []:
             repeating_part = \
                list(itertools.islice(digits, len(value.repeating_part)))
         else:
             repeating_part = value.repeating_part[:]
 
         remainder = Radix(
-           True,
+           1,
            [],
            non_repeating_remainder,
            repeating_part,
            value.base
         )
         remainder_fraction = remainder.as_rational()
         middle = Fraction(1, 2)
         if remainder_fraction < middle:
-            return (truncated(), -1 if value.positive else 1)
+            return (truncated(), -1 * value.sign)
         elif remainder_fraction > middle:
-            return (incremented(), 1 if value.positive else -1)
+            return (incremented(), value.sign)
         else:
-            if cls._conditional_toward_zero(method, value.positive):
-                return (truncated(), -1 if value.positive else 1)
+            if cls._conditional_toward_zero(method, value.sign):
+                return (truncated(), -1 * value.sign)
             else:
-                return (incremented(), 1 if value.positive else -1)
+                return (incremented(), value.sign)
 
         raise BasesAssertError() # pragma: no cover
```

### Comparing `justbases-0.6/src/justbases/_nats.py` & `justbases-0.9/src/justbases/_nats.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/src/justbases/_constants.py` & `justbases-0.9/src/justbases/_constants.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/tox.ini` & `justbases-0.9/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 [tox]
+envlist=lint,test,coverage
 
 [testenv:coverage]
 deps =
     coverage
     hypothesis
     pytest>=2.8
 commands =
```

### Comparing `justbases-0.6/setup.py` & `justbases-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     author='Anne Mulhern',
     author_email='mulhern@cs.wisc.edu',
     description='conversion of ints and rationals to any base',
     long_description=open(README, encoding='utf-8').read(),
     platforms=['Linux'],
     license='GPL 2+',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: GNU General Public License (GPL)',
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: Implementation :: CPython',
```

### Comparing `justbases-0.6/check.py` & `justbases-0.9/check.py`

 * *Files identical despite different names*

### Comparing `justbases-0.6/doc/_build/html/usage.html` & `justbases-0.9/doc/_build/html/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Usage &mdash; justbases 0.5 documentation</title>
+    <title>Usage &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="index.html" />
     <link rel="next" title="justbases" href="justbases/modules.html" />
     <link rel="prev" title="Justbases" href="intro.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases/modules.html" title="justbases"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbases"
              accesskey="P">previous</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -307,15 +307,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases/modules.html" title="justbases"
              >next</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbases"
              >previous</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Usage¶ ******
 The library can be used in several ways.
 ***** NatDivision: Precise Division of Natural Numbers in any Base¶ *****
 The method NatDivision.division() takes a divisor, a dividend, and a base. The
 divisor and dividend are numbers in the given base, represented as lists of
 ints. The result is a tuple consisting of the integer portion of the value, the
 non-repeating part after the radix, the repeating part after the radix and a
@@ -170,9 +170,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/index.html` & `justbases-0.9/doc/_build/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Justbases &mdash; justbases 0.5 documentation</title>
+    <title>Justbases &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="#" />
+    <link rel="top" title="justbases 0.07 documentation" href="#" />
     <link rel="next" title="Justbases" href="intro.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
@@ -35,15 +35,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbases"
              accesskey="N">next</a> |</li>
-        <li><a href="#">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="#">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -53,14 +53,15 @@
 <p>Contents:</p>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="intro.html">Justbases</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#purpose">Purpose</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#motivation">Motivation</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#algorithmic-complexity">Algorithmic Complexity</a></li>
+<li class="toctree-l2"><a class="reference internal" href="intro.html#related-packages">Related Packages</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="usage.html#natdivision-precise-division-of-natural-numbers-in-any-base">NatDivision: Precise Division of Natural Numbers in any Base</a></li>
 <li class="toctree-l2"><a class="reference internal" href="usage.html#nats-conversion-of-natural-numbers-between-arbitrary-bases">Nats: Conversion of Natural Numbers between Arbitrary Bases</a></li>
 <li class="toctree-l2"><a class="reference internal" href="usage.html#radix-non-fractional-representation-of-a-rational-number">Radix: Non-fractional Representation of a Rational Number</a></li>
 <li class="toctree-l2"><a class="reference internal" href="usage.html#rationals-conversion-of-rational-numbers-between-arbitrary-bases">Rationals: Conversion of Rational Numbers between Arbitrary Bases</a></li>
@@ -134,15 +135,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbases"
              >next</a> |</li>
-        <li><a href="#">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="#">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Justbases¶ ******
 Contents:
     * Justbases
           o Purpose
           o Motivation
           o Algorithmic_Complexity
+          o Related_Packages
     * Usage
           o NatDivision:_Precise_Division_of_Natural_Numbers_in_any_Base
           o Nats:_Conversion_of_Natural_Numbers_between_Arbitrary_Bases
           o Radix:_Non-fractional_Representation_of_a_Rational_Number
           o Rationals:_Conversion_of_Rational_Numbers_between_Arbitrary_Bases
           o Rounding:_Rounding_Rationals
           o Rounding:_Rounding_Radix_Values
@@ -38,9 +39,9 @@
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/search.html` & `justbases-0.9/doc/_build/html/search.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,33 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Search &mdash; justbases 0.5 documentation</title>
+    <title>Search &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="_static/searchtools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="index.html" />
   <script type="text/javascript">
     jQuery(function() { Search.loadIndex("searchindex.js"); });
   </script>
   
   <script type="text/javascript" id="searchindexloader"></script>
    
 
@@ -39,15 +39,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -90,15 +90,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
 
 
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 From here you can search these documents. Enter your search words into the box
 below and click "search". Note that the search function will automatically
 search for all of the words. Pages containing fewer words won't appear in the
 result list.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.test_constants.html` & `justbases-0.9/doc/_build/html/tests/tests.test_constants.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,53 +2,53 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.test_constants module &mdash; justbases 0.5 documentation</title>
+    <title>tests.test_constants module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
-    <link rel="next" title="tests.test_division module" href="tests.test_division.html" />
+    <link rel="next" title="tests.test_display module" href="tests.test_display.html" />
     <link rel="prev" title="tests._utils module" href="tests._utils.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests.test_division.html" title="tests.test_division module"
+          <a href="tests.test_display.html" title="tests.test_display module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests._utils.html" title="tests._utils module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -79,16 +79,16 @@
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
   <p class="topless"><a href="tests._utils.html"
                         title="previous chapter">tests._utils module</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="tests.test_division.html"
-                        title="next chapter">tests.test_division module</a></p>
+  <p class="topless"><a href="tests.test_display.html"
+                        title="next chapter">tests.test_display module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/tests/tests.test_constants.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
@@ -113,20 +113,20 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests.test_division.html" title="tests.test_division module"
+          <a href="tests.test_display.html" title="tests.test_display module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests._utils.html" title="tests._utils module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,35 +4,35 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 ****** tests.test_constants module¶ ******
 Test for integer conversions.
   classtests.test_constants.RoundingMethodsTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for RoundingMethods constants.
         testStr()¶
             Test __str__ and __repr__ method.
 *** Previous topic ***
 tests._utils_module
 *** Next topic ***
-tests.test_division_module
+tests.test_display_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.test_nats.html` & `justbases-0.9/doc/_build/html/tests/tests.test_nats.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.test_nats module &mdash; justbases 0.5 documentation</title>
+    <title>tests.test_nats module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.test_radix module" href="tests.test_radix.html" />
     <link rel="prev" title="tests.test_division module" href="tests.test_division.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_radix.html" title="tests.test_radix module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.test_division.html" title="tests.test_division module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -82,15 +82,16 @@
 <tt class="descname">testExceptions</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_nats.NatsTestCase.testExceptions" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test throwing exception.</p>
 </dd></dl>
 
 <dl class="method">
 <dt id="tests.test_nats.NatsTestCase.testFromInt">
 <tt class="descname">testFromInt</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_nats.NatsTestCase.testFromInt" title="Permalink to this definition">¶</a></dt>
-<dd><p>convert_to_int(convert_from_int(value, to_base), 10) == value</p>
+<dd><p>convert_to_int(convert_from_int(value, to_base), 10) == value
+No leading zeros in convert_from_int(value, to_base)</p>
 </dd></dl>
 
 <dl class="method">
 <dt id="tests.test_nats.NatsTestCase.testFromOther">
 <tt class="descname">testFromOther</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_nats.NatsTestCase.testFromOther" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test roundtrip from number in arbitrary base.</p>
 </dd></dl>
@@ -144,15 +145,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_radix.html" title="tests.test_radix module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.test_division.html" title="tests.test_division module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,29 +4,30 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 ****** tests.test_nats module¶ ******
 Test for integer conversions.
   classtests.test_nats.NatsTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for ints.
         testCarryIn()¶
             Test carry_in.
             Parameters: strategy – the strategy (tuple of value, carry, base)
         testExceptions()¶
             Test throwing exception.
         testFromInt()¶
-            convert_to_int(convert_from_int(value, to_base), 10) == value
+            convert_to_int(convert_from_int(value, to_base), 10) == value No
+            leading zeros in convert_from_int(value, to_base)
         testFromOther()¶
             Test roundtrip from number in arbitrary base.
 *** Previous topic ***
 tests.test_division_module
 *** Next topic ***
 tests.test_radix_module
 **** This Page ****
@@ -35,11 +36,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/modules.html` & `justbases-0.9/doc/_build/html/tests/modules.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests &mdash; justbases 0.5 documentation</title>
+    <title>tests &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="next" title="tests package" href="tests.html" />
     <link rel="prev" title="justbases.version module" href="../justbases/justbases.version.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.html" title="tests package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="../justbases/justbases.version.html" title="justbases.version module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -56,14 +56,15 @@
 <h1>tests<a class="headerlink" href="#tests" title="Permalink to this headline">¶</a></h1>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="tests.html">tests package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="tests.html#submodules">Submodules</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="tests._utils.html">tests._utils module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="tests.test_constants.html">tests.test_constants module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="tests.test_display.html">tests.test_display module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="tests.test_division.html">tests.test_division module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="tests.test_nats.html">tests.test_nats module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="tests.test_radix.html">tests.test_radix module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="tests.test_rationals.html">tests.test_rationals module</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="tests.html#module-tests">Module contents</a></li>
@@ -118,15 +119,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.html" title="tests package"
              >next</a> |</li>
         <li class="right" >
           <a href="../justbases/justbases.version.html" title="justbases.version module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -3,20 +3,21 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** tests¶ ******
     * tests_package
           o Submodules
                 # tests._utils_module
                 # tests.test_constants_module
+                # tests.test_display_module
                 # tests.test_division_module
                 # tests.test_nats_module
                 # tests.test_radix_module
                 # tests.test_rationals_module
           o Module_contents
 *** Previous topic ***
 justbases.version_module
@@ -28,9 +29,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.test_radix.html` & `justbases-0.9/doc/_build/html/tests/tests.test_radix.html`

 * *Files 13% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.test_radix module &mdash; justbases 0.5 documentation</title>
+    <title>tests.test_radix module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.test_rationals module" href="tests.test_rationals.html" />
     <link rel="prev" title="tests.test_nats module" href="tests.test_nats.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_rationals.html" title="tests.test_rationals module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.test_nats.html" title="tests.test_nats module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -60,35 +60,36 @@
 <p>Test for rational conversions.</p>
 <dl class="class">
 <dt id="tests.test_radix.RadixTestCase">
 <em class="property">class </em><tt class="descclassname">tests.test_radix.</tt><tt class="descname">RadixTestCase</tt><big>(</big><em>methodName='runTest'</em><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <tt class="xref py py-class docutils literal"><span class="pre">unittest.case.TestCase</span></tt></p>
 <p>Tests for radix.</p>
 <dl class="method">
+<dt id="tests.test_radix.RadixTestCase.testCarryOnRepeatingPart">
+<tt class="descname">testCarryOnRepeatingPart</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testCarryOnRepeatingPart" title="Permalink to this definition">¶</a></dt>
+<dd><p>Carry from non_repeating_part to integer_part and then out.</p>
+</dd></dl>
+
+<dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testEquality">
 <tt class="descname">testEquality</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testEquality" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test == operator.</p>
 </dd></dl>
 
 <dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testExceptions">
 <tt class="descname">testExceptions</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testExceptions" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test exceptions.</p>
 </dd></dl>
 
 <dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testInBase">
 <tt class="descname">testInBase</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testInBase" title="Permalink to this definition">¶</a></dt>
-<dd><p>Test that roundtrip is identity.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="tests.test_radix.RadixTestCase.testInBase2">
-<tt class="descname">testInBase2</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testInBase2" title="Permalink to this definition">¶</a></dt>
-<dd><p>Test conversion to current base.</p>
+<dd><p>Test that roundtrip is identity modulo number of 0s in
+non repeating part.</p>
 </dd></dl>
 
 <dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testInEquality">
 <tt class="descname">testInEquality</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testInEquality" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test != operator.</p>
 </dd></dl>
@@ -108,17 +109,23 @@
 <dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testRepeatingRepeatPart">
 <tt class="descname">testRepeatingRepeatPart</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testRepeatingRepeatPart" title="Permalink to this definition">¶</a></dt>
 <dd><p>Repeat part is made up of repeating parts.</p>
 </dd></dl>
 
 <dl class="method">
+<dt id="tests.test_radix.RadixTestCase.testRepr">
+<tt class="descname">testRepr</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testRepr" title="Permalink to this definition">¶</a></dt>
+<dd><p>Make sure that result is evalable.</p>
+</dd></dl>
+
+<dl class="method">
 <dt id="tests.test_radix.RadixTestCase.testStr">
 <tt class="descname">testStr</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RadixTestCase.testStr" title="Permalink to this definition">¶</a></dt>
-<dd><p>Make sure that __str__ executes.</p>
+<dd><p>Check basic properties of __str__.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="class">
 <dt id="tests.test_radix.RoundingTestCase">
 <em class="property">class </em><tt class="descclassname">tests.test_radix.</tt><tt class="descname">RoundingTestCase</tt><big>(</big><em>methodName='runTest'</em><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase" title="Permalink to this definition">¶</a></dt>
@@ -127,58 +134,20 @@
 <dl class="method">
 <dt id="tests.test_radix.RoundingTestCase.testAsInt">
 <tt class="descname">testAsInt</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testAsInt" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test equivalence with two paths.</p>
 </dd></dl>
 
 <dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testExactLength">
-<tt class="descname">testExactLength</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testExactLength" title="Permalink to this definition">¶</a></dt>
-<dd><p>Require conversion, but do not carry out of repeating_part.
-Ensure that the intermediate result is exactly the required
-precision.</p>
-</dd></dl>
-
-<dl class="method">
 <dt id="tests.test_radix.RoundingTestCase.testExceptions">
 <tt class="descname">testExceptions</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testExceptions" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test exception.</p>
 </dd></dl>
 
 <dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testFiveEighths">
-<tt class="descname">testFiveEighths</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testFiveEighths" title="Permalink to this definition">¶</a></dt>
-<dd><p>Test 5/8 in base 3.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testLeadingZeros">
-<tt class="descname">testLeadingZeros</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testLeadingZeros" title="Permalink to this definition">¶</a></dt>
-<dd><p>Require conversion, but do not carry out of repeating_part.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testMiddles">
-<tt class="descname">testMiddles</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testMiddles" title="Permalink to this definition">¶</a></dt>
-<dd><p>Ensure that there is no tie breaker.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testOneHalf">
-<tt class="descname">testOneHalf</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testOneHalf" title="Permalink to this definition">¶</a></dt>
-<dd><p>Test 1/2 in base 3.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="tests.test_radix.RoundingTestCase.testOverflow">
-<tt class="descname">testOverflow</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testOverflow" title="Permalink to this definition">¶</a></dt>
-<dd><p>Ensure that rounding causes overflow.</p>
-</dd></dl>
-
-<dl class="method">
 <dt id="tests.test_radix.RoundingTestCase.testRoundFraction">
 <tt class="descname">testRoundFraction</tt><big>(</big><big>)</big><a class="headerlink" href="#tests.test_radix.RoundingTestCase.testRoundFraction" title="Permalink to this definition">¶</a></dt>
 <dd><p>Test that rounding yields the correct number of digits.</p>
 <p>Test that rounded values are in a good range.</p>
 </dd></dl>
 
 <dl class="method">
@@ -236,15 +205,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_rationals.html" title="tests.test_rationals module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.test_nats.html" title="tests.test_nats module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,60 +4,50 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 ****** tests.test_radix module¶ ******
 Test for rational conversions.
   classtests.test_radix.RadixTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for radix.
+        testCarryOnRepeatingPart()¶
+            Carry from non_repeating_part to integer_part and then out.
         testEquality()¶
             Test == operator.
         testExceptions()¶
             Test exceptions.
         testInBase()¶
-            Test that roundtrip is identity.
-        testInBase2()¶
-            Test conversion to current base.
+            Test that roundtrip is identity modulo number of 0s in non
+            repeating part.
         testInEquality()¶
             Test != operator.
         testOperatorExceptions()¶
             Test that comparsion operators yield exceptions.
         testOptions()¶
             Skip validation and canonicalization.
         testRepeatingRepeatPart()¶
             Repeat part is made up of repeating parts.
+        testRepr()¶
+            Make sure that result is evalable.
         testStr()¶
-            Make sure that __str__ executes.
+            Check basic properties of __str__.
   classtests.test_radix.RoundingTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for rounding Radixes.
         testAsInt()¶
             Test equivalence with two paths.
-        testExactLength()¶
-            Require conversion, but do not carry out of repeating_part. Ensure
-            that the intermediate result is exactly the required precision.
         testExceptions()¶
             Test exception.
-        testFiveEighths()¶
-            Test 5/8 in base 3.
-        testLeadingZeros()¶
-            Require conversion, but do not carry out of repeating_part.
-        testMiddles()¶
-            Ensure that there is no tie breaker.
-        testOneHalf()¶
-            Test 1/2 in base 3.
-        testOverflow()¶
-            Ensure that rounding causes overflow.
         testRoundFraction()¶
             Test that rounding yields the correct number of digits.
             Test that rounded values are in a good range.
         testRoundRelation()¶
             Test that all results have the correct relation.
 *** Previous topic ***
 tests.test_nats_module
@@ -69,11 +59,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.test_division.html` & `justbases-0.9/doc/_build/html/tests/tests.test_division.html`

 * *Files 6% similar despite different names*

```diff
@@ -2,35 +2,35 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.test_division module &mdash; justbases 0.5 documentation</title>
+    <title>tests.test_division module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.test_nats module" href="tests.test_nats.html" />
-    <link rel="prev" title="tests.test_constants module" href="tests.test_constants.html" /> 
+    <link rel="prev" title="tests.test_display module" href="tests.test_display.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
@@ -38,17 +38,17 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_nats.html" title="tests.test_nats module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="tests.test_constants.html" title="tests.test_constants module"
+          <a href="tests.test_display.html" title="tests.test_display module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -107,16 +107,16 @@
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
-  <p class="topless"><a href="tests.test_constants.html"
-                        title="previous chapter">tests.test_constants module</a></p>
+  <p class="topless"><a href="tests.test_display.html"
+                        title="previous chapter">tests.test_display module</a></p>
   <h4>Next topic</h4>
   <p class="topless"><a href="tests.test_nats.html"
                         title="next chapter">tests.test_nats module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/tests/tests.test_division.txt"
            rel="nofollow">Show Source</a></li>
@@ -147,17 +147,17 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_nats.html" title="tests.test_nats module"
              >next</a> |</li>
         <li class="right" >
-          <a href="tests.test_constants.html" title="tests.test_constants module"
+          <a href="tests.test_display.html" title="tests.test_display module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 ****** tests.test_division module¶ ******
 Test for integer conversions.
   classtests.test_division.NatDivisionTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for division.
@@ -31,24 +31,24 @@
             calculated, then the non-repeating portion has precision digits and
             is a prefix of non-repeating-part + repeating part when precision
             is not bounded.
         testUpDown()¶
             Test that rounding up and rounding down have the right
             relationship.
 *** Previous topic ***
-tests.test_constants_module
+tests.test_display_module
 *** Next topic ***
 tests.test_nats_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests._utils.html` & `justbases-0.9/doc/_build/html/tests/tests.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,89 +2,107 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests._utils module &mdash; justbases 0.5 documentation</title>
+    <title>tests package &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
-    <link rel="up" title="tests package" href="tests.html" />
-    <link rel="next" title="tests.test_constants module" href="tests.test_constants.html" />
-    <link rel="prev" title="tests package" href="tests.html" /> 
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
+    <link rel="up" title="tests" href="modules.html" />
+    <link rel="next" title="tests._utils module" href="tests._utils.html" />
+    <link rel="prev" title="tests" href="modules.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests.test_constants.html" title="tests.test_constants module"
+          <a href="tests._utils.html" title="tests._utils module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="tests.html" title="tests package"
+          <a href="modules.html" title="tests"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" >tests</a> &raquo;</li>
-          <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" accesskey="U">tests</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
             
-  <div class="section" id="module-tests._utils">
-<span id="tests-utils-module"></span><h1>tests._utils module<a class="headerlink" href="#module-tests._utils" title="Permalink to this headline">¶</a></h1>
-<p>Test utilities.</p>
-<dl class="function">
-<dt id="tests._utils.build_nat">
-<tt class="descclassname">tests._utils.</tt><tt class="descname">build_nat</tt><big>(</big><em>base</em>, <em>max_len</em><big>)</big><a class="headerlink" href="#tests._utils.build_nat" title="Permalink to this definition">¶</a></dt>
-<dd><p>Build a well-formed nat strategy from <tt class="docutils literal"><span class="pre">base</span></tt>.</p>
-</dd></dl>
-
+  <div class="section" id="tests-package">
+<h1>tests package<a class="headerlink" href="#tests-package" title="Permalink to this headline">¶</a></h1>
+<div class="section" id="submodules">
+<h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this headline">¶</a></h2>
+<div class="toctree-wrapper compound">
+<ul>
+<li class="toctree-l1"><a class="reference internal" href="tests._utils.html">tests._utils module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_constants.html">tests.test_constants module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_display.html">tests.test_display module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_division.html">tests.test_division module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_nats.html">tests.test_nats module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_radix.html">tests.test_radix module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="tests.test_rationals.html">tests.test_rationals module</a></li>
+</ul>
+</div>
+</div>
+<div class="section" id="module-tests">
+<span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-tests" title="Permalink to this headline">¶</a></h2>
+</div>
 </div>
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
+  <h3><a href="../index.html">Table Of Contents</a></h3>
+  <ul>
+<li><a class="reference internal" href="#">tests package</a><ul>
+<li><a class="reference internal" href="#submodules">Submodules</a></li>
+<li><a class="reference internal" href="#module-tests">Module contents</a></li>
+</ul>
+</li>
+</ul>
+
   <h4>Previous topic</h4>
-  <p class="topless"><a href="tests.html"
-                        title="previous chapter">tests package</a></p>
+  <p class="topless"><a href="modules.html"
+                        title="previous chapter">tests</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="tests.test_constants.html"
-                        title="next chapter">tests.test_constants module</a></p>
+  <p class="topless"><a href="tests._utils.html"
+                        title="next chapter">tests._utils module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
-    <li><a href="../_sources/tests/tests._utils.txt"
+    <li><a href="../_sources/tests/tests.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" />
       <input type="submit" value="Go" />
@@ -106,22 +124,21 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests.test_constants.html" title="tests.test_constants module"
+          <a href="tests._utils.html" title="tests._utils module"
              >next</a> |</li>
         <li class="right" >
-          <a href="tests.html" title="tests package"
+          <a href="modules.html" title="tests"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" >tests</a> &raquo;</li>
-          <li><a href="tests.html" >tests package</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" >tests</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -4,32 +4,40 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
-    * tests_package »
-****** tests._utils module¶ ******
-Test utilities.
-  tests._utils.build_nat(base, max_len)¶
-      Build a well-formed nat strategy from base.
+****** tests package¶ ******
+***** Submodules¶ *****
+    * tests._utils_module
+    * tests.test_constants_module
+    * tests.test_display_module
+    * tests.test_division_module
+    * tests.test_nats_module
+    * tests.test_radix_module
+    * tests.test_rationals_module
+***** Module contents¶ *****
+**** Table_Of_Contents ****
+    * tests_package
+          o Submodules
+          o Module_contents
 *** Previous topic ***
-tests_package
+tests
 *** Next topic ***
-tests.test_constants_module
+tests._utils_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
-    * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.test_rationals.html` & `justbases-0.9/doc/_build/html/tests/tests.test_rationals.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.test_rationals module &mdash; justbases 0.5 documentation</title>
+    <title>tests.test_rationals module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="prev" title="tests.test_radix module" href="tests.test_radix.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -36,15 +36,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_radix.html" title="tests.test_radix module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -139,15 +139,15 @@
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.test_radix.html" title="tests.test_radix module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 ****** tests.test_rationals module¶ ******
 Test for rational conversions.
   classtests.test_rationals.RationalsTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Tests for rationals.
@@ -34,11 +34,11 @@
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/tests/tests.html` & `justbases-0.9/doc/_build/html/justbases/modules.html`

 * *Files 16% similar despite different names*

```diff
@@ -2,106 +2,101 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests package &mdash; justbases 0.5 documentation</title>
+    <title>justbases &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
-    <link rel="up" title="tests" href="modules.html" />
-    <link rel="next" title="tests._utils module" href="tests._utils.html" />
-    <link rel="prev" title="tests" href="modules.html" /> 
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
+    <link rel="next" title="justbases package" href="justbases.html" />
+    <link rel="prev" title="Usage" href="../usage.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests._utils.html" title="tests._utils module"
+          <a href="justbases.html" title="justbases package"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="modules.html" title="tests"
+          <a href="../usage.html" title="Usage"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" accesskey="U">tests</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
             
-  <div class="section" id="tests-package">
-<h1>tests package<a class="headerlink" href="#tests-package" title="Permalink to this headline">¶</a></h1>
-<div class="section" id="submodules">
-<h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this headline">¶</a></h2>
+  <div class="section" id="justbases">
+<h1>justbases<a class="headerlink" href="#justbases" title="Permalink to this headline">¶</a></h1>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="tests._utils.html">tests._utils module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="tests.test_constants.html">tests.test_constants module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="tests.test_division.html">tests.test_division module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="tests.test_nats.html">tests.test_nats module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="tests.test_radix.html">tests.test_radix module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="tests.test_rationals.html">tests.test_rationals module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases.html">justbases package</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="justbases.html#submodules">Submodules</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="justbases._config.html">justbases._config module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._constants.html">justbases._constants module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._display.html">justbases._display module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._division.html">justbases._division module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._errors.html">justbases._errors module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._nats.html">justbases._nats module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases._rationals.html">justbases._rationals module</a></li>
+<li class="toctree-l3"><a class="reference internal" href="justbases.version.html">justbases.version module</a><ul>
+<li class="toctree-l4"><a class="reference internal" href="justbases.version.html#justbases-version">justbases.version</a></li>
+</ul>
+</li>
+</ul>
+</li>
+<li class="toctree-l2"><a class="reference internal" href="justbases.html#module-justbases">Module contents</a></li>
+</ul>
+</li>
 </ul>
-</div>
-</div>
-<div class="section" id="module-tests">
-<span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-tests" title="Permalink to this headline">¶</a></h2>
 </div>
 </div>
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
-  <h3><a href="../index.html">Table Of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">tests package</a><ul>
-<li><a class="reference internal" href="#submodules">Submodules</a></li>
-<li><a class="reference internal" href="#module-tests">Module contents</a></li>
-</ul>
-</li>
-</ul>
-
   <h4>Previous topic</h4>
-  <p class="topless"><a href="modules.html"
-                        title="previous chapter">tests</a></p>
+  <p class="topless"><a href="../usage.html"
+                        title="previous chapter">Usage</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="tests._utils.html"
-                        title="next chapter">tests._utils module</a></p>
+  <p class="topless"><a href="justbases.html"
+                        title="next chapter">justbases package</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
-    <li><a href="../_sources/tests/tests.txt"
+    <li><a href="../_sources/justbases/modules.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" />
       <input type="submit" value="Go" />
@@ -123,21 +118,20 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="tests._utils.html" title="tests._utils module"
+          <a href="justbases.html" title="justbases package"
              >next</a> |</li>
         <li class="right" >
-          <a href="modules.html" title="tests"
+          <a href="../usage.html" title="Usage"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" >tests</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,42 +1,39 @@
 
 
 
 
-
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
-    * tests »
-****** tests package¶ ******
-***** Submodules¶ *****
-    * tests._utils_module
-    * tests.test_constants_module
-    * tests.test_division_module
-    * tests.test_nats_module
-    * tests.test_radix_module
-    * tests.test_rationals_module
-***** Module contents¶ *****
-**** Table_Of_Contents ****
-    * tests_package
+    * justbases_0.07_documentation »
+****** justbases¶ ******
+    * justbases_package
           o Submodules
+                # justbases._config_module
+                # justbases._constants_module
+                # justbases._display_module
+                # justbases._division_module
+                # justbases._errors_module
+                # justbases._nats_module
+                # justbases._rationals_module
+                # justbases.version_module
+                      # justbases.version
           o Module_contents
 *** Previous topic ***
-tests
+Usage
 *** Next topic ***
-tests._utils_module
+justbases_package
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
-    * tests »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/py-modindex.html` & `justbases-0.9/doc/_build/html/py-modindex.html`

 * *Files 20% similar despite different names*

```diff
@@ -2,47 +2,47 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Python Module Index &mdash; justbases 0.5 documentation</title>
+    <title>Python Module Index &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="index.html" />
  
 
 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -64,19 +64,29 @@
               id="toggle-1" style="display: none" alt="-" /></td>
        <td>
        <a href="justbases/justbases.html#module-justbases"><tt class="xref">justbases</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
+       <a href="justbases/justbases._config.html#module-justbases._config"><tt class="xref">justbases._config</tt></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&nbsp;&nbsp;&nbsp;
        <a href="justbases/justbases._constants.html#module-justbases._constants"><tt class="xref">justbases._constants</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
+       <a href="justbases/justbases._display.html#module-justbases._display"><tt class="xref">justbases._display</tt></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&nbsp;&nbsp;&nbsp;
        <a href="justbases/justbases._division.html#module-justbases._division"><tt class="xref">justbases._division</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
        <a href="justbases/justbases._errors.html#module-justbases._errors"><tt class="xref">justbases._errors</tt></a></td><td>
        <em></em></td></tr>
@@ -113,14 +123,19 @@
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
        <a href="tests/tests.test_constants.html#module-tests.test_constants"><tt class="xref">tests.test_constants</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-2">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
+       <a href="tests/tests.test_display.html#module-tests.test_display"><tt class="xref">tests.test_display</tt></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-2">
+       <td></td>
+       <td>&nbsp;&nbsp;&nbsp;
        <a href="tests/tests.test_division.html#module-tests.test_division"><tt class="xref">tests.test_division</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-2">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
        <a href="tests/tests.test_nats.html#module-tests.test_nats"><tt class="xref">tests.test_nats</tt></a></td><td>
        <em></em></td></tr>
@@ -164,15 +179,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,34 +1,37 @@
 
 
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Python Module Index ******
 j | t
      
     j
 [-] justbases
+        justbases._config
         justbases._constants
+        justbases._display
         justbases._division
         justbases._errors
         justbases._nats
         justbases._rationals
         justbases.version
      
     t
 [-] tests
         tests._utils
         tests.test_constants
+        tests.test_display
         tests.test_division
         tests.test_nats
         tests.test_radix
         tests.test_rationals
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases._division.html` & `justbases-0.9/doc/_build/html/justbases/justbases._division.html`

 * *Files 4% similar despite different names*

```diff
@@ -2,35 +2,35 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases._division module &mdash; justbases 0.5 documentation</title>
+    <title>justbases._division module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="justbases package" href="justbases.html" />
     <link rel="next" title="justbases._errors module" href="justbases._errors.html" />
-    <link rel="prev" title="justbases._constants module" href="justbases._constants.html" /> 
+    <link rel="prev" title="justbases._display module" href="justbases._display.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
@@ -38,17 +38,17 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases._errors.html" title="justbases._errors module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="justbases._constants.html" title="justbases._constants module"
+          <a href="justbases._display.html" title="justbases._display module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -131,16 +131,16 @@
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
-  <p class="topless"><a href="justbases._constants.html"
-                        title="previous chapter">justbases._constants module</a></p>
+  <p class="topless"><a href="justbases._display.html"
+                        title="previous chapter">justbases._display module</a></p>
   <h4>Next topic</h4>
   <p class="topless"><a href="justbases._errors.html"
                         title="next chapter">justbases._errors module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/justbases/justbases._division.txt"
            rel="nofollow">Show Source</a></li>
@@ -171,17 +171,17 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases._errors.html" title="justbases._errors module"
              >next</a> |</li>
         <li class="right" >
-          <a href="justbases._constants.html" title="justbases._constants module"
+          <a href="justbases._display.html" title="justbases._display module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 ****** justbases._division module¶ ******
 Long division in any bases.
   classjustbases._division.NatDivision¶
       Bases: object
       Methods for division in arbitrary bases.
@@ -44,24 +44,24 @@
                             * base (int) – the base
             Returns:    divisor and dividend in lowest terms
             Return      tuple of list of int * list of int
             type:
             Complexity: O(len(non_repeating_part + repeating_part +
             integer_part))
 *** Previous topic ***
-justbases._constants_module
+justbases._display_module
 *** Next topic ***
 justbases._errors_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases.version.html` & `justbases-0.9/doc/_build/html/justbases/justbases.version.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases.version module &mdash; justbases 0.5 documentation</title>
+    <title>justbases.version module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="justbases package" href="justbases.html" />
     <link rel="next" title="tests" href="../tests/modules.html" />
     <link rel="prev" title="justbases._rationals module" href="justbases._rationals.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../tests/modules.html" title="tests"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbases._rationals.html" title="justbases._rationals module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -116,15 +116,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../tests/modules.html" title="tests"
              >next</a> |</li>
         <li class="right" >
           <a href="justbases._rationals.html" title="justbases._rationals module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 ****** justbases.version module¶ ******
 ***** justbases.version¶ *****
 Version information.
 **** Table_Of_Contents ****
     * justbases.version_module
@@ -27,11 +27,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/modules.html` & `justbases-0.9/doc/_build/html/justbases/justbases.html`

 * *Files 22% similar despite different names*

```diff
@@ -2,99 +2,131 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases &mdash; justbases 0.5 documentation</title>
+    <title>justbases package &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
-    <link rel="next" title="justbases package" href="justbases.html" />
-    <link rel="prev" title="Usage" href="../usage.html" /> 
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
+    <link rel="up" title="justbases" href="modules.html" />
+    <link rel="next" title="justbases._config module" href="justbases._config.html" />
+    <link rel="prev" title="justbases" href="modules.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases.html" title="justbases package"
+          <a href="justbases._config.html" title="justbases._config module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="../usage.html" title="Usage"
+          <a href="modules.html" title="justbases"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" accesskey="U">justbases</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
             
-  <div class="section" id="justbases">
-<h1>justbases<a class="headerlink" href="#justbases" title="Permalink to this headline">¶</a></h1>
+  <div class="section" id="justbases-package">
+<h1>justbases package<a class="headerlink" href="#justbases-package" title="Permalink to this headline">¶</a></h1>
+<div class="section" id="submodules">
+<h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this headline">¶</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="justbases.html">justbases package</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="justbases.html#submodules">Submodules</a><ul>
-<li class="toctree-l3"><a class="reference internal" href="justbases._constants.html">justbases._constants module</a></li>
-<li class="toctree-l3"><a class="reference internal" href="justbases._division.html">justbases._division module</a></li>
-<li class="toctree-l3"><a class="reference internal" href="justbases._errors.html">justbases._errors module</a></li>
-<li class="toctree-l3"><a class="reference internal" href="justbases._nats.html">justbases._nats module</a></li>
-<li class="toctree-l3"><a class="reference internal" href="justbases._rationals.html">justbases._rationals module</a></li>
-<li class="toctree-l3"><a class="reference internal" href="justbases.version.html">justbases.version module</a><ul>
-<li class="toctree-l4"><a class="reference internal" href="justbases.version.html#justbases-version">justbases.version</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._config.html">justbases._config module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._constants.html">justbases._constants module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._display.html">justbases._display module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._division.html">justbases._division module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._errors.html">justbases._errors module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._nats.html">justbases._nats module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases._rationals.html">justbases._rationals module</a></li>
+<li class="toctree-l1"><a class="reference internal" href="justbases.version.html">justbases.version module</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="justbases.version.html#justbases-version">justbases.version</a></li>
 </ul>
 </li>
 </ul>
+</div>
+</div>
+<div class="section" id="module-justbases">
+<span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-justbases" title="Permalink to this headline">¶</a></h2>
+<p>The public interface of justbases.</p>
+<p>Contents:</p>
+<blockquote>
+<div><ul class="simple">
+<li>RoundingMethods &#8211; a list of available rounding methods</li>
+<li>NatDivision &#8211; long division of natural numbers and its inverse</li>
+<li>BasesError &#8211; supertype of errors raised by package methods</li>
+<li>Nats<ul>
+<li>conversion between non-negative ints and sequences</li>
+<li>conversion between sequences in one base to sequences in another</li>
+</ul>
 </li>
-<li class="toctree-l2"><a class="reference internal" href="justbases.html#module-justbases">Module contents</a></li>
+<li>Radix &#8211; representation of rational number as string of digits</li>
+<li>Rationals<ul>
+<li>conversion between Rational and Radix objects</li>
+<li>conversion between Radix objects in any base</li>
 </ul>
 </li>
 </ul>
+</div></blockquote>
 </div>
 </div>
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
+  <h3><a href="../index.html">Table Of Contents</a></h3>
+  <ul>
+<li><a class="reference internal" href="#">justbases package</a><ul>
+<li><a class="reference internal" href="#submodules">Submodules</a></li>
+<li><a class="reference internal" href="#module-justbases">Module contents</a></li>
+</ul>
+</li>
+</ul>
+
   <h4>Previous topic</h4>
-  <p class="topless"><a href="../usage.html"
-                        title="previous chapter">Usage</a></p>
+  <p class="topless"><a href="modules.html"
+                        title="previous chapter">justbases</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="justbases.html"
-                        title="next chapter">justbases package</a></p>
+  <p class="topless"><a href="justbases._config.html"
+                        title="next chapter">justbases._config module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
-    <li><a href="../_sources/justbases/modules.txt"
+    <li><a href="../_sources/justbases/justbases.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" />
       <input type="submit" value="Go" />
@@ -116,20 +148,21 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases.html" title="justbases package"
+          <a href="justbases._config.html" title="justbases._config module"
              >next</a> |</li>
         <li class="right" >
-          <a href="../usage.html" title="Usage"
+          <a href="modules.html" title="justbases"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" >justbases</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,37 +1,58 @@
 
 
 
 
+
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
-****** justbases¶ ******
+    * justbases_0.07_documentation »
+    * justbases »
+****** justbases package¶ ******
+***** Submodules¶ *****
+    * justbases._config_module
+    * justbases._constants_module
+    * justbases._display_module
+    * justbases._division_module
+    * justbases._errors_module
+    * justbases._nats_module
+    * justbases._rationals_module
+    * justbases.version_module
+          o justbases.version
+***** Module contents¶ *****
+The public interface of justbases.
+Contents:
+         * RoundingMethods – a list of available rounding methods
+         * NatDivision – long division of natural numbers and its inverse
+         * BasesError – supertype of errors raised by package methods
+         * Nats
+               o conversion between non-negative ints and sequences
+               o conversion between sequences in one base to sequences in
+                 another
+         * Radix – representation of rational number as string of digits
+         * Rationals
+               o conversion between Rational and Radix objects
+               o conversion between Radix objects in any base
+**** Table_Of_Contents ****
     * justbases_package
           o Submodules
-                # justbases._constants_module
-                # justbases._division_module
-                # justbases._errors_module
-                # justbases._nats_module
-                # justbases._rationals_module
-                # justbases.version_module
-                      # justbases.version
           o Module_contents
 *** Previous topic ***
-Usage
+justbases
 *** Next topic ***
-justbases_package
+justbases._config_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
+    * justbases »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases._constants.html` & `justbases-0.9/doc/_build/html/justbases/justbases._constants.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,53 +2,53 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases._constants module &mdash; justbases 0.5 documentation</title>
+    <title>justbases._constants module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="justbases package" href="justbases.html" />
-    <link rel="next" title="justbases._division module" href="justbases._division.html" />
-    <link rel="prev" title="justbases package" href="justbases.html" /> 
+    <link rel="next" title="justbases._display module" href="justbases._display.html" />
+    <link rel="prev" title="justbases._config module" href="justbases._config.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases._division.html" title="justbases._division module"
+          <a href="justbases._display.html" title="justbases._display module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="justbases.html" title="justbases package"
+          <a href="justbases._config.html" title="justbases._config module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -112,19 +112,19 @@
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
-  <p class="topless"><a href="justbases.html"
-                        title="previous chapter">justbases package</a></p>
+  <p class="topless"><a href="justbases._config.html"
+                        title="previous chapter">justbases._config module</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="justbases._division.html"
-                        title="next chapter">justbases._division module</a></p>
+  <p class="topless"><a href="justbases._display.html"
+                        title="next chapter">justbases._display module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/justbases/justbases._constants.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
@@ -149,20 +149,20 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases._division.html" title="justbases._division module"
+          <a href="justbases._display.html" title="justbases._display module"
              >next</a> |</li>
         <li class="right" >
-          <a href="justbases.html" title="justbases package"
+          <a href="justbases._config.html" title="justbases._config module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 ****** justbases._constants module¶ ******
 Constants required by the package.
   classjustbases._constants.RoundingMethods¶
       Bases: object
       Static class for accessing rounding methods.
@@ -23,24 +23,24 @@
         ROUND_DOWN= _RoundingMethod(Round down.)¶
         ROUND_HALF_DOWN= _RoundingMethod(Round to nearest, down on a tie.)¶
         ROUND_HALF_UP= _RoundingMethod(Round to nearest, up on a tie.)¶
         ROUND_HALF_ZERO= _RoundingMethod(Round to nearest, to zero on a tie.)¶
         ROUND_TO_ZERO= _RoundingMethod(Round to zero.)¶
         ROUND_UP= _RoundingMethod(Round up.)¶
 *** Previous topic ***
-justbases_package
+justbases._config_module
 *** Next topic ***
-justbases._division_module
+justbases._display_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases._nats.html` & `justbases-0.9/doc/_build/html/justbases/justbases._nats.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases._nats module &mdash; justbases 0.5 documentation</title>
+    <title>justbases._nats module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="justbases package" href="justbases.html" />
     <link rel="next" title="justbases._rationals module" href="justbases._rationals.html" />
     <link rel="prev" title="justbases._errors module" href="justbases._errors.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases._rationals.html" title="justbases._rationals module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbases._errors.html" title="justbases._errors module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -257,15 +257,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases._rationals.html" title="justbases._rationals module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbases._errors.html" title="justbases._errors module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 ****** justbases._nats module¶ ******
 Methods dealing exclusively with natural numbers.
   classjustbases._nats.Nats¶
       Bases: object
       Methods to convert non-negative ints.
@@ -75,11 +75,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases.html` & `justbases-0.9/doc/_build/html/justbases/justbases._errors.html`

 * *Files 24% similar despite different names*

```diff
@@ -2,129 +2,112 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases package &mdash; justbases 0.5 documentation</title>
+    <title>justbases._errors module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
-    <link rel="up" title="justbases" href="modules.html" />
-    <link rel="next" title="justbases._constants module" href="justbases._constants.html" />
-    <link rel="prev" title="justbases" href="modules.html" /> 
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
+    <link rel="up" title="justbases package" href="justbases.html" />
+    <link rel="next" title="justbases._nats module" href="justbases._nats.html" />
+    <link rel="prev" title="justbases._division module" href="justbases._division.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases._constants.html" title="justbases._constants module"
+          <a href="justbases._nats.html" title="justbases._nats module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="modules.html" title="justbases"
+          <a href="justbases._division.html" title="justbases._division module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" accesskey="U">justbases</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" >justbases</a> &raquo;</li>
+          <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
             
-  <div class="section" id="justbases-package">
-<h1>justbases package<a class="headerlink" href="#justbases-package" title="Permalink to this headline">¶</a></h1>
-<div class="section" id="submodules">
-<h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this headline">¶</a></h2>
-<div class="toctree-wrapper compound">
-<ul>
-<li class="toctree-l1"><a class="reference internal" href="justbases._constants.html">justbases._constants module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="justbases._division.html">justbases._division module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="justbases._errors.html">justbases._errors module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="justbases._nats.html">justbases._nats module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="justbases._rationals.html">justbases._rationals module</a></li>
-<li class="toctree-l1"><a class="reference internal" href="justbases.version.html">justbases.version module</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="justbases.version.html#justbases-version">justbases.version</a></li>
-</ul>
-</li>
-</ul>
-</div>
-</div>
-<div class="section" id="module-justbases">
-<span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-justbases" title="Permalink to this headline">¶</a></h2>
-<p>The public interface of justbases.</p>
-<p>Contents:</p>
-<blockquote>
-<div><ul class="simple">
-<li>RoundingMethods &#8211; a list of available rounding methods</li>
-<li>NatDivision &#8211; long division of natural numbers and its inverse</li>
-<li>BasesError &#8211; supertype of errors raised by package methods</li>
-<li>Nats<ul>
-<li>conversion between non-negative ints and sequences</li>
-<li>conversion between sequences in one base to sequences in another</li>
-</ul>
-</li>
-<li>Radix &#8211; representation of rational number as string of digits</li>
-<li>Rationals<ul>
-<li>conversion between Rational and Radix objects</li>
-<li>conversion between Radix objects in any base</li>
-</ul>
-</li>
-</ul>
-</div></blockquote>
-</div>
+  <div class="section" id="module-justbases._errors">
+<span id="justbases-errors-module"></span><h1>justbases._errors module<a class="headerlink" href="#module-justbases._errors" title="Permalink to this headline">¶</a></h1>
+<p>Errors.</p>
+<dl class="exception">
+<dt id="justbases._errors.BasesAssertError">
+<em class="property">exception </em><tt class="descclassname">justbases._errors.</tt><tt class="descname">BasesAssertError</tt><a class="headerlink" href="#justbases._errors.BasesAssertError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference internal" href="#justbases._errors.BasesError" title="justbases._errors.BasesError"><tt class="xref py py-class docutils literal"><span class="pre">justbases._errors.BasesError</span></tt></a></p>
+<p>For assertion failures.</p>
+</dd></dl>
+
+<dl class="exception">
+<dt id="justbases._errors.BasesError">
+<em class="property">exception </em><tt class="descclassname">justbases._errors.</tt><tt class="descname">BasesError</tt><a class="headerlink" href="#justbases._errors.BasesError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/exceptions.html#exceptions.Exception" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">exceptions.Exception</span></tt></a></p>
+<p>Supertype of all errors for this package.</p>
+</dd></dl>
+
+<dl class="exception">
+<dt id="justbases._errors.BasesInvalidOperationError">
+<em class="property">exception </em><tt class="descclassname">justbases._errors.</tt><tt class="descname">BasesInvalidOperationError</tt><big>(</big><em>op</em>, <em>other=None</em><big>)</big><a class="headerlink" href="#justbases._errors.BasesInvalidOperationError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference internal" href="#justbases._errors.BasesError" title="justbases._errors.BasesError"><tt class="xref py py-class docutils literal"><span class="pre">justbases._errors.BasesError</span></tt></a></p>
+<p>Invalid operation.</p>
+</dd></dl>
+
+<dl class="exception">
+<dt id="justbases._errors.BasesValueError">
+<em class="property">exception </em><tt class="descclassname">justbases._errors.</tt><tt class="descname">BasesValueError</tt><big>(</big><em>value</em>, <em>param</em>, <em>msg=None</em><big>)</big><a class="headerlink" href="#justbases._errors.BasesValueError" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <a class="reference internal" href="#justbases._errors.BasesError" title="justbases._errors.BasesError"><tt class="xref py py-class docutils literal"><span class="pre">justbases._errors.BasesError</span></tt></a></p>
+<p>Raised when a parameter has an unacceptable value.</p>
+<p>May also be raised when the parameter has an unacceptable type.</p>
+</dd></dl>
+
 </div>
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
-  <h3><a href="../index.html">Table Of Contents</a></h3>
-  <ul>
-<li><a class="reference internal" href="#">justbases package</a><ul>
-<li><a class="reference internal" href="#submodules">Submodules</a></li>
-<li><a class="reference internal" href="#module-justbases">Module contents</a></li>
-</ul>
-</li>
-</ul>
-
   <h4>Previous topic</h4>
-  <p class="topless"><a href="modules.html"
-                        title="previous chapter">justbases</a></p>
+  <p class="topless"><a href="justbases._division.html"
+                        title="previous chapter">justbases._division module</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="justbases._constants.html"
-                        title="next chapter">justbases._constants module</a></p>
+  <p class="topless"><a href="justbases._nats.html"
+                        title="next chapter">justbases._nats module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
-    <li><a href="../_sources/justbases/justbases.txt"
+    <li><a href="../_sources/justbases/justbases._errors.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
     <form class="search" action="../search.html" method="get">
       <input type="text" name="q" />
       <input type="submit" value="Go" />
@@ -146,21 +129,22 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbases._constants.html" title="justbases._constants module"
+          <a href="justbases._nats.html" title="justbases._nats module"
              >next</a> |</li>
         <li class="right" >
-          <a href="modules.html" title="justbases"
+          <a href="justbases._division.html" title="justbases._division module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
-          <li><a href="modules.html" >justbases</a> &raquo;</li> 
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
+          <li><a href="modules.html" >justbases</a> &raquo;</li>
+          <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -4,53 +4,43 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
-****** justbases package¶ ******
-***** Submodules¶ *****
-    * justbases._constants_module
-    * justbases._division_module
-    * justbases._errors_module
-    * justbases._nats_module
-    * justbases._rationals_module
-    * justbases.version_module
-          o justbases.version
-***** Module contents¶ *****
-The public interface of justbases.
-Contents:
-         * RoundingMethods – a list of available rounding methods
-         * NatDivision – long division of natural numbers and its inverse
-         * BasesError – supertype of errors raised by package methods
-         * Nats
-               o conversion between non-negative ints and sequences
-               o conversion between sequences in one base to sequences in
-                 another
-         * Radix – representation of rational number as string of digits
-         * Rationals
-               o conversion between Rational and Radix objects
-               o conversion between Radix objects in any base
-**** Table_Of_Contents ****
-    * justbases_package
-          o Submodules
-          o Module_contents
+    * justbases_package »
+****** justbases._errors module¶ ******
+Errors.
+  exceptionjustbases._errors.BasesAssertError¶
+      Bases: justbases._errors.BasesError
+      For assertion failures.
+  exceptionjustbases._errors.BasesError¶
+      Bases: exceptions.Exception
+      Supertype of all errors for this package.
+  exceptionjustbases._errors.BasesInvalidOperationError(op, other=None)¶
+      Bases: justbases._errors.BasesError
+      Invalid operation.
+  exceptionjustbases._errors.BasesValueError(value, param, msg=None)¶
+      Bases: justbases._errors.BasesError
+      Raised when a parameter has an unacceptable value.
+      May also be raised when the parameter has an unacceptable type.
 *** Previous topic ***
-justbases
+justbases._division_module
 *** Next topic ***
-justbases._constants_module
+justbases._nats_module
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
+    * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/justbases/justbases._rationals.html` & `justbases-0.9/doc/_build/html/justbases/justbases._rationals.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbases._rationals module &mdash; justbases 0.5 documentation</title>
+    <title>justbases._rationals module &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="../index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="../index.html" />
     <link rel="up" title="justbases package" href="justbases.html" />
     <link rel="next" title="justbases.version module" href="justbases.version.html" />
     <link rel="prev" title="justbases._nats module" href="justbases._nats.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases.version.html" title="justbases.version module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbases._nats.html" title="justbases._nats module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" accesskey="U">justbases package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -94,15 +94,15 @@
 <p>Complexity: Uncalculated.</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="class">
 <dt id="justbases._rationals.Radix">
-<em class="property">class </em><tt class="descclassname">justbases._rationals.</tt><tt class="descname">Radix</tt><big>(</big><em>positive</em>, <em>integer_part</em>, <em>non_repeating_part</em>, <em>repeating_part</em>, <em>base</em>, <em>validate=True</em>, <em>canonicalize=True</em><big>)</big><a class="headerlink" href="#justbases._rationals.Radix" title="Permalink to this definition">¶</a></dt>
+<em class="property">class </em><tt class="descclassname">justbases._rationals.</tt><tt class="descname">Radix</tt><big>(</big><em>sign</em>, <em>integer_part</em>, <em>non_repeating_part</em>, <em>repeating_part</em>, <em>base</em>, <em>validate=True</em>, <em>canonicalize=True</em><big>)</big><a class="headerlink" href="#justbases._rationals.Radix" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
 <p>An object containing information about a rational representation.</p>
 <p>Such values can not be ordered, but can be compared for equality.</p>
 <dl class="method">
 <dt id="justbases._rationals.Radix.as_int">
 <tt class="descname">as_int</tt><big>(</big><em>method</em><big>)</big><a class="headerlink" href="#justbases._rationals.Radix.as_int" title="Permalink to this definition">¶</a></dt>
 <dd><p>This value as an int, rounded according to <tt class="docutils literal"><span class="pre">method</span></tt>.</p>
@@ -136,14 +136,32 @@
 <tr class="field-even field"><th class="field-name">Return type:</th><td class="field-body">Rational</td>
 </tr>
 </tbody>
 </table>
 </dd></dl>
 
 <dl class="method">
+<dt id="justbases._rationals.Radix.getString">
+<tt class="descname">getString</tt><big>(</big><em>config</em>, <em>relation=0</em><big>)</big><a class="headerlink" href="#justbases._rationals.Radix.getString" title="Permalink to this definition">¶</a></dt>
+<dd><p>Return a representation of a Radix according to config.</p>
+<table class="docutils field-list" frame="void" rules="none">
+<col class="field-name" />
+<col class="field-body" />
+<tbody valign="top">
+<tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first last simple">
+<li><strong>config</strong> (<em>DisplayConfig</em>) &#8211; configuration</li>
+<li><strong>relation</strong> (<a class="reference external" href="http://docs.python.org/library/functions.html#int" title="(in Python v2.7)"><em>int</em></a>) &#8211; the relation of this value to actual value</li>
+</ul>
+</td>
+</tr>
+</tbody>
+</table>
+</dd></dl>
+
+<dl class="method">
 <dt id="justbases._rationals.Radix.in_base">
 <tt class="descname">in_base</tt><big>(</big><em>base</em><big>)</big><a class="headerlink" href="#justbases._rationals.Radix.in_base" title="Permalink to this definition">¶</a></dt>
 <dd><p>Return value in <tt class="docutils literal"><span class="pre">base</span></tt>.</p>
 <table class="docutils field-list" frame="void" rules="none">
 <col class="field-name" />
 <col class="field-body" />
 <tbody valign="top">
@@ -264,15 +282,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbases.version.html" title="justbases.version module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbases._nats.html" title="justbases._nats module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbases 0.5 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbases 0.07 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbases</a> &raquo;</li>
           <li><a href="justbases.html" >justbases package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 ****** justbases._rationals module¶ ******
 Methods dealing with rationals.
   classjustbases._rationals.Radices¶
       Bases: object
       Methods for Radices.
@@ -27,15 +27,15 @@
                               method
             Returns:    the conversion result and its relation to actual result
             Return      Radix * int
             type:
             Raises BasesValueError:
                        if to_base is less than 2
             Complexity: Uncalculated.
-  classjustbases._rationals.Radix(positive, integer_part, non_repeating_part,
+  classjustbases._rationals.Radix(sign, integer_part, non_repeating_part,
   repeating_part, base, validate=True, canonicalize=True)¶
       Bases: object
       An object containing information about a rational representation.
       Such values can not be ordered, but can be compared for equality.
         as_int(method)¶
             This value as an int, rounded according to method.
             Parameters:  method – rounding method
@@ -43,14 +43,19 @@
                         on bad parameters
             Returns:     corresponding int value
             Return type: int
         as_rational()¶
             Return this value as a Rational.
             Returns:     this radix as a rational
             Return type: Rational
+        getString(config, relation=0)¶
+            Return a representation of a Radix according to config.
+                            * config (DisplayConfig) – configuration
+            Parameters:     * relation (int) – the relation of this value to actual
+                              value
         in_base(base)¶
             Return value in base.
             Returns:     Radix in base
             Return type: Radix
             Raises ConvertError:
                         if base is less than 2
         rounded(precision, method)¶
@@ -84,11 +89,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
     * justbases »
     * justbases_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/genindex.html` & `justbases-0.9/doc/_build/html/genindex.html`

 * *Files 26% similar despite different names*

```diff
@@ -3,44 +3,44 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Index &mdash; justbases 0.5 documentation</title>
+    <title>Index &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="index.html" /> 
+    <link rel="top" title="justbases 0.07 documentation" href="index.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -50,21 +50,24 @@
 
 <div class="genindex-jumpbox">
  <a href="#A"><strong>A</strong></a>
  | <a href="#B"><strong>B</strong></a>
  | <a href="#C"><strong>C</strong></a>
  | <a href="#D"><strong>D</strong></a>
  | <a href="#F"><strong>F</strong></a>
+ | <a href="#G"><strong>G</strong></a>
  | <a href="#I"><strong>I</strong></a>
  | <a href="#J"><strong>J</strong></a>
  | <a href="#M"><strong>M</strong></a>
  | <a href="#N"><strong>N</strong></a>
  | <a href="#R"><strong>R</strong></a>
+ | <a href="#S"><strong>S</strong></a>
  | <a href="#T"><strong>T</strong></a>
  | <a href="#U"><strong>U</strong></a>
+ | <a href="#X"><strong>X</strong></a>
  
 </div>
 <h2 id="A">A</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbases/justbases._rationals.html#justbases._rationals.Radix.as_int">as_int() (justbases._rationals.Radix method)</a>
@@ -79,35 +82,71 @@
   </dl></td>
 </tr></table>
 
 <h2 id="B">B</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
+  <dt><a href="justbases/justbases._config.html#justbases._config.BaseConfig">BaseConfig (class in justbases._config)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._errors.html#justbases._errors.BasesAssertError">BasesAssertError</a>
   </dt>
 
       
+  <dt><a href="justbases/justbases._config.html#justbases._config.BasesConfig">BasesConfig (class in justbases._config)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._errors.html#justbases._errors.BasesError">BasesError</a>
   </dt>
 
       
   <dt><a href="justbases/justbases._errors.html#justbases._errors.BasesInvalidOperationError">BasesInvalidOperationError</a>
   </dt>
 
+      
+  <dt><a href="justbases/justbases._errors.html#justbases._errors.BasesValueError">BasesValueError</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_base">build_base() (in module tests._utils)</a>
+  </dt>
+
   </dl></td>
   <td style="width: 33%" valign="top"><dl>
       
-  <dt><a href="justbases/justbases._errors.html#justbases._errors.BasesValueError">BasesValueError</a>
+  <dt><a href="tests/tests._utils.html#tests._utils.build_base_config">build_base_config() (in module tests._utils)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_display_config">build_display_config() (in module tests._utils)</a>
   </dt>
 
       
   <dt><a href="tests/tests._utils.html#tests._utils.build_nat">build_nat() (in module tests._utils)</a>
   </dt>
 
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_radix">build_radix() (in module tests._utils)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_relation">build_relation() (in module tests._utils)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_sign">build_sign() (in module tests._utils)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests._utils.html#tests._utils.build_strip_config">build_strip_config() (in module tests._utils)</a>
+  </dt>
+
   </dl></td>
 </tr></table>
 
 <h2 id="C">C</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
@@ -135,14 +174,40 @@
   </dl></td>
 </tr></table>
 
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
+  <dt><a href="justbases/justbases._display.html#justbases._display.Decorators">Decorators (class in justbases._display)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.Decorators.decorators">decorators() (justbases._display.Decorators class method)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.Digits">Digits (class in justbases._display)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._config.html#justbases._config.DigitsConfig">DigitsConfig (class in justbases._config)</a>
+  </dt>
+
+  </dl></td>
+  <td style="width: 33%" valign="top"><dl>
+      
+  <dt><a href="justbases/justbases._config.html#justbases._config.BasesConfig.DISPLAY_CONFIG">DISPLAY_CONFIG (justbases._config.BasesConfig attribute)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._config.html#justbases._config.DisplayConfig">DisplayConfig (class in justbases._config)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._division.html#justbases._division.NatDivision.division">division() (justbases._division.NatDivision class method)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
 <h2 id="F">F</h2>
@@ -151,14 +216,24 @@
       
   <dt><a href="justbases/justbases._rationals.html#justbases._rationals.Radices.from_rational">from_rational() (justbases._rationals.Radices class method)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
+<h2 id="G">G</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%" valign="top"><dl>
+      
+  <dt><a href="justbases/justbases._rationals.html#justbases._rationals.Radix.getString">getString() (justbases._rationals.Radix method)</a>
+  </dt>
+
+  </dl></td>
+</tr></table>
+
 <h2 id="I">I</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbases/justbases._rationals.html#justbases._rationals.Radix.in_base">in_base() (justbases._rationals.Radix method)</a>
   </dt>
 
@@ -169,28 +244,36 @@
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbases/justbases.html#module-justbases">justbases (module)</a>
   </dt>
 
       
+  <dt><a href="justbases/justbases._config.html#module-justbases._config">justbases._config (module)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._constants.html#module-justbases._constants">justbases._constants (module)</a>
   </dt>
 
       
-  <dt><a href="justbases/justbases._division.html#module-justbases._division">justbases._division (module)</a>
+  <dt><a href="justbases/justbases._display.html#module-justbases._display">justbases._display (module)</a>
   </dt>
 
       
-  <dt><a href="justbases/justbases._errors.html#module-justbases._errors">justbases._errors (module)</a>
+  <dt><a href="justbases/justbases._division.html#module-justbases._division">justbases._division (module)</a>
   </dt>
 
   </dl></td>
   <td style="width: 33%" valign="top"><dl>
       
+  <dt><a href="justbases/justbases._errors.html#module-justbases._errors">justbases._errors (module)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._nats.html#module-justbases._nats">justbases._nats (module)</a>
   </dt>
 
       
   <dt><a href="justbases/justbases._rationals.html#module-justbases._rationals">justbases._rationals (module)</a>
   </dt>
 
@@ -218,24 +301,28 @@
   <dt><a href="justbases/justbases._division.html#justbases._division.NatDivision">NatDivision (class in justbases._division)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_division.html#tests.test_division.NatDivisionTestCase">NatDivisionTestCase (class in tests.test_division)</a>
   </dt>
 
-  </dl></td>
-  <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbases/justbases._nats.html#justbases._nats.Nats">Nats (class in justbases._nats)</a>
   </dt>
 
+  </dl></td>
+  <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="tests/tests.test_nats.html#tests.test_nats.NatsTestCase">NatsTestCase (class in tests.test_nats)</a>
   </dt>
 
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.Number">Number (class in justbases._display)</a>
+  </dt>
+
   </dl></td>
 </tr></table>
 
 <h2 id="R">R</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
@@ -255,14 +342,18 @@
   </dt>
 
       
   <dt><a href="tests/tests.test_rationals.html#tests.test_rationals.RationalsTestCase">RationalsTestCase (class in tests.test_rationals)</a>
   </dt>
 
       
+  <dt><a href="justbases/justbases._display.html#justbases._display.Decorators.relation_to_symbol">relation_to_symbol() (justbases._display.Decorators static method)</a>
+  </dt>
+
+      
   <dt><a href="justbases/justbases._constants.html#justbases._constants.RoundingMethods.ROUND_DOWN">ROUND_DOWN (justbases._constants.RoundingMethods attribute)</a>
   </dt>
 
       
   <dt><a href="justbases/justbases._constants.html#justbases._constants.RoundingMethods.ROUND_HALF_DOWN">ROUND_HALF_DOWN (justbases._constants.RoundingMethods attribute)</a>
   </dt>
 
@@ -303,39 +394,71 @@
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase">RoundingTestCase (class in tests.test_radix)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
+<h2 id="S">S</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%" valign="top"><dl>
+      
+  <dt><a href="justbases/justbases._config.html#justbases._config.BasesConfig.set_display_config">set_display_config() (justbases._config.BasesConfig class method)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.String">String (class in justbases._display)</a>
+  </dt>
+
+  </dl></td>
+  <td style="width: 33%" valign="top"><dl>
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.Strip">Strip (class in justbases._display)</a>
+  </dt>
+
+      
+  <dt><a href="justbases/justbases._config.html#justbases._config.StripConfig">StripConfig (class in justbases._config)</a>
+  </dt>
+
+  </dl></td>
+</tr></table>
+
 <h2 id="T">T</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testAsInt">testAsInt() (tests.test_radix.RoundingTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_nats.html#tests.test_nats.NatsTestCase.testCarryIn">testCarryIn() (tests.test_nats.NatsTestCase method)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testEquality">testEquality() (tests.test_radix.RadixTestCase method)</a>
+  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testCarryOnRepeatingPart">testCarryOnRepeatingPart() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testExactLength">testExactLength() (tests.test_radix.RoundingTestCase method)</a>
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestDigits">TestDigits (class in tests.test_display)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_nats.html#tests.test_nats.NatsTestCase.testExceptions">testExceptions() (tests.test_nats.NatsTestCase method)</a>
+  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testEquality">testEquality() (tests.test_radix.RadixTestCase method)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestDigits.testExceptions">testExceptions() (tests.test_display.TestDigits method)</a>
   </dt>
 
       <dd><dl>
         
+  <dt><a href="tests/tests.test_nats.html#tests.test_nats.NatsTestCase.testExceptions">(tests.test_nats.NatsTestCase method)</a>
+  </dt>
+
+        
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testExceptions">(tests.test_radix.RadixTestCase method)</a>
   </dt>
 
         
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testExceptions">(tests.test_radix.RoundingTestCase method)</a>
   </dt>
 
@@ -349,15 +472,15 @@
   </dt>
 
       
   <dt><a href="tests/tests.test_division.html#tests.test_division.NatDivisionTestCase.testExceptionsUndivision">testExceptionsUndivision() (tests.test_division.NatDivisionTestCase method)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testFiveEighths">testFiveEighths() (tests.test_radix.RoundingTestCase method)</a>
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestString.testFormat">testFormat() (tests.test_display.TestString method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_nats.html#tests.test_nats.NatsTestCase.testFromInt">testFromInt() (tests.test_nats.NatsTestCase method)</a>
   </dt>
 
       
@@ -365,65 +488,53 @@
   </dt>
 
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testInBase">testInBase() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testInBase2">testInBase2() (tests.test_radix.RadixTestCase method)</a>
-  </dt>
-
-      
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testInEquality">testInEquality() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_division.html#tests.test_division.NatDivisionTestCase.testInverses">testInverses() (tests.test_division.NatDivisionTestCase method)</a>
   </dt>
 
       <dd><dl>
         
   <dt><a href="tests/tests.test_rationals.html#tests.test_rationals.RationalsTestCase.testInverses">(tests.test_rationals.RationalsTestCase method)</a>
   </dt>
 
       </dl></dd>
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testLeadingZeros">testLeadingZeros() (tests.test_radix.RoundingTestCase method)</a>
-  </dt>
-
-      
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testMiddles">testMiddles() (tests.test_radix.RoundingTestCase method)</a>
-  </dt>
-
-      
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testOneHalf">testOneHalf() (tests.test_radix.RoundingTestCase method)</a>
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestNumber">TestNumber (class in tests.test_display)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testOperatorExceptions">testOperatorExceptions() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testOptions">testOptions() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
-  </dl></td>
-  <td style="width: 33%" valign="top"><dl>
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testOverflow">testOverflow() (tests.test_radix.RoundingTestCase method)</a>
+  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testRepeatingRepeatPart">testRepeatingRepeatPart() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
-  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testRepeatingRepeatPart">testRepeatingRepeatPart() (tests.test_radix.RadixTestCase method)</a>
+  <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testRepr">testRepr() (tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RoundingTestCase.testRoundFraction">testRoundFraction() (tests.test_radix.RoundingTestCase method)</a>
   </dt>
 
+  </dl></td>
+  <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="tests/tests.test_rationals.html#tests.test_rationals.RationalsTestCase.testRounding">testRounding() (tests.test_rationals.RationalsTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_rationals.html#tests.test_rationals.RationalsTestCase.testRoundingConversion">testRoundingConversion() (tests.test_rationals.RationalsTestCase method)</a>
   </dt>
@@ -449,14 +560,18 @@
   </dt>
 
       
   <dt><a href="tests/tests.test_constants.html#module-tests.test_constants">tests.test_constants (module)</a>
   </dt>
 
       
+  <dt><a href="tests/tests.test_display.html#module-tests.test_display">tests.test_display (module)</a>
+  </dt>
+
+      
   <dt><a href="tests/tests.test_division.html#module-tests.test_division">tests.test_division (module)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_nats.html#module-tests.test_nats">tests.test_nats (module)</a>
   </dt>
 
@@ -475,34 +590,76 @@
       <dd><dl>
         
   <dt><a href="tests/tests.test_radix.html#tests.test_radix.RadixTestCase.testStr">(tests.test_radix.RadixTestCase method)</a>
   </dt>
 
       </dl></dd>
       
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestString">TestString (class in tests.test_display)</a>
+  </dt>
+
+      
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestStrip">TestStrip (class in tests.test_display)</a>
+  </dt>
+
+      
   <dt><a href="tests/tests.test_division.html#tests.test_division.NatDivisionTestCase.testTruncation">testTruncation() (tests.test_division.NatDivisionTestCase method)</a>
   </dt>
 
       
   <dt><a href="tests/tests.test_division.html#tests.test_division.NatDivisionTestCase.testUpDown">testUpDown() (tests.test_division.NatDivisionTestCase method)</a>
   </dt>
 
+      
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestNumber.testXform">testXform() (tests.test_display.TestNumber method)</a>
+  </dt>
+
+      <dd><dl>
+        
+  <dt><a href="tests/tests.test_display.html#tests.test_display.TestStrip.testXform">(tests.test_display.TestStrip method)</a>
+  </dt>
+
+      </dl></dd>
   </dl></td>
 </tr></table>
 
 <h2 id="U">U</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbases/justbases._division.html#justbases._division.NatDivision.undivision">undivision() (justbases._division.NatDivision class method)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
+<h2 id="X">X</h2>
+<table style="width: 100%" class="indextable genindextable"><tr>
+  <td style="width: 33%" valign="top"><dl>
+      
+  <dt><a href="justbases/justbases._display.html#justbases._display.Digits.xform">xform() (justbases._display.Digits class method)</a>
+  </dt>
+
+      <dd><dl>
+        
+  <dt><a href="justbases/justbases._display.html#justbases._display.Number.xform">(justbases._display.Number class method)</a>
+  </dt>
+
+        
+  <dt><a href="justbases/justbases._display.html#justbases._display.String.xform">(justbases._display.String class method)</a>
+  </dt>
+
+        
+  <dt><a href="justbases/justbases._display.html#justbases._display.Strip.xform">(justbases._display.Strip class method)</a>
+  </dt>
+
+      </dl></dd>
+  </dl></td>
+</tr></table>
+
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
@@ -531,15 +688,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -1,122 +1,154 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Index ******
-A | B | C | D | F | I | J | M | N | R | T | U
+A | B | C | D | F | G | I | J | M | N | R | S | T | U | X
 ***** A *****
   as_int()_(justbases._rationals.Radix   as_rational()_
   method)                                (justbases._rationals.Radix_method)
 ***** B *****
-  BasesAssertError             BasesValueError
-  BasesError                   build_nat()_(in_module_tests._utils)
-  BasesInvalidOperationError
+  BaseConfig_(class_in                    build_base_config()_(in_module
+  justbases._config)                      tests._utils)
+  BasesAssertError                        build_display_config()_(in_module
+  BasesConfig_(class_in                   tests._utils)
+  justbases._config)                      build_nat()_(in_module_tests._utils)
+  BasesError                              build_radix()_(in_module
+  BasesInvalidOperationError              tests._utils)
+  BasesValueError                         build_relation()_(in_module
+  build_base()_(in_module_tests._utils)   tests._utils)
+                                          build_sign()_(in_module_tests._utils)
+                                          build_strip_config()_(in_module
+                                          tests._utils)
 ***** C *****
   carry_in()_(justbases._nats.Nats        convert_from_int()_
   static_method)                          (justbases._nats.Nats_static_method)
   CONDITIONAL_METHODS()_                  convert_to_int()_
   (justbases._constants.RoundingMethods   (justbases._nats.Nats_static_method)
   class_method)
   convert()_(justbases._nats.Nats_class
   method)
 ***** D *****
-  division()_(justbases._division.NatDivision_class_method)
+  Decorators_(class_in                   DISPLAY_CONFIG_
+  justbases._display)                    (justbases._config.BasesConfig
+  decorators()_                          attribute)
+  (justbases._display.Decorators_class   DisplayConfig_(class_in
+  method)                                justbases._config)
+  Digits_(class_in_justbases._display)   division()_
+  DigitsConfig_(class_in                 (justbases._division.NatDivision_class
+  justbases._config)                     method)
 ***** F *****
   from_rational()_(justbases._rationals.Radices_class_method)
+***** G *****
+  getString()_(justbases._rationals.Radix_method)
 ***** I *****
   in_base()_(justbases._rationals.Radix_method)
 ***** J *****
-  justbases_(module)              justbases._nats_(module)
+  justbases_(module)              justbases._errors_(module)
+  justbases._config_(module)      justbases._nats_(module)
   justbases._constants_(module)   justbases._rationals_(module)
-  justbases._division_(module)    justbases.version_(module)
-  justbases._errors_(module)
+  justbases._display_(module)     justbases.version_(module)
+  justbases._division_(module)
 ***** M *****
   METHODS()_(justbases._constants.RoundingMethods_class_method)
 ***** N *****
-  NatDivision_(class_in           Nats_(class_in_justbases._nats)
-  justbases._division)            NatsTestCase_(class_in_tests.test_nats)
+  NatDivision_(class_in             NatsTestCase_(class_in_tests.test_nats)
+  justbases._division)              Number_(class_in_justbases._display)
   NatDivisionTestCase_(class_in
   tests.test_division)
+  Nats_(class_in_justbases._nats)
 ***** R *****
   Radices_(class_in                       ROUND_HALF_ZERO_
   justbases._rationals)                   (justbases._constants.RoundingMethods
   Radix_(class_in_justbases._rationals)   attribute)
   RadixTestCase_(class_in                 round_to_int()_
   tests.test_radix)                       (justbases._rationals.Rationals
   Rationals_(class_in                     static_method)
   justbases._rationals)                   ROUND_TO_ZERO_
   RationalsTestCase_(class_in             (justbases._constants.RoundingMethods
   tests.test_rationals)                   attribute)
-  ROUND_DOWN_                             ROUND_UP_
-  (justbases._constants.RoundingMethods   (justbases._constants.RoundingMethods
-  attribute)                              attribute)
-  ROUND_HALF_DOWN_                        rounded()_(justbases._rationals.Radix
+  relation_to_symbol()_                   ROUND_UP_
+  (justbases._display.Decorators_static   (justbases._constants.RoundingMethods
+  method)                                 attribute)
+  ROUND_DOWN_                             rounded()_(justbases._rationals.Radix
   (justbases._constants.RoundingMethods   method)
   attribute)                              RoundingMethods_(class_in
-  ROUND_HALF_UP_                          justbases._constants)
+  ROUND_HALF_DOWN_                        justbases._constants)
   (justbases._constants.RoundingMethods   RoundingMethodsTestCase_(class_in
   attribute)                              tests.test_constants)
-                                          RoundingTestCase_(class_in
-                                          tests.test_radix)
+  ROUND_HALF_UP_                          RoundingTestCase_(class_in
+  (justbases._constants.RoundingMethods   tests.test_radix)
+  attribute)
+***** S *****
+  set_display_config()_                  Strip_(class_in_justbases._display)
+  (justbases._config.BasesConfig_class   StripConfig_(class_in
+  method)                                justbases._config)
+  String_(class_in_justbases._display)
 ***** T *****
-  testAsInt()_                                    testOverflow()_
-  (tests.test_radix.RoundingTestCase_method)      (tests.test_radix.RoundingTestCase_method)
-  testCarryIn()_(tests.test_nats.NatsTestCase     testRepeatingRepeatPart()_
-  method)                                         (tests.test_radix.RadixTestCase_method)
-  testEquality()_                                 testRoundFraction()_
-  (tests.test_radix.RadixTestCase_method)         (tests.test_radix.RoundingTestCase_method)
-  testExactLength()_                              testRounding()_
+  testAsInt()_                                    testRounding()_
   (tests.test_radix.RoundingTestCase_method)      (tests.test_rationals.RationalsTestCase
-  testExceptions()_                               method)
-  (tests.test_nats.NatsTestCase_method)           testRoundingConversion()_
-        (tests.test_radix.RadixTestCase_method)   (tests.test_rationals.RationalsTestCase
-        (tests.test_radix.RoundingTestCase        method)
-        method)                                   testRoundingExceptions()_
-        (tests.test_rationals.RationalsTestCase   (tests.test_rationals.RationalsTestCase
-        method)                                   method)
-  testExceptionsDivision()_                       testRoundingPrecise()_
-  (tests.test_division.NatDivisionTestCase        (tests.test_rationals.RationalsTestCase
-  method)                                         method)
-  testExceptionsUndivision()_                     testRoundRelation()_
-  (tests.test_division.NatDivisionTestCase        (tests.test_radix.RoundingTestCase_method)
-  method)                                         tests_(module)
-  testFiveEighths()_                              tests._utils_(module)
-  (tests.test_radix.RoundingTestCase_method)      tests.test_constants_(module)
-  testFromInt()_(tests.test_nats.NatsTestCase     tests.test_division_(module)
+  testCarryIn()_(tests.test_nats.NatsTestCase     method)
+  method)                                         testRoundingConversion()_
+  testCarryOnRepeatingPart()_                     (tests.test_rationals.RationalsTestCase
+  (tests.test_radix.RadixTestCase_method)         method)
+  TestDigits_(class_in_tests.test_display)        testRoundingExceptions()_
+  testEquality()_                                 (tests.test_rationals.RationalsTestCase
+  (tests.test_radix.RadixTestCase_method)         method)
+  testExceptions()_                               testRoundingPrecise()_
+  (tests.test_display.TestDigits_method)          (tests.test_rationals.RationalsTestCase
+        (tests.test_nats.NatsTestCase_method)     method)
+        (tests.test_radix.RadixTestCase_method)   testRoundRelation()_
+        (tests.test_radix.RoundingTestCase        (tests.test_radix.RoundingTestCase_method)
+        method)                                   tests_(module)
+        (tests.test_rationals.RationalsTestCase   tests._utils_(module)
+        method)                                   tests.test_constants_(module)
+  testExceptionsDivision()_                       tests.test_display_(module)
+  (tests.test_division.NatDivisionTestCase        tests.test_division_(module)
   method)                                         tests.test_nats_(module)
-  testFromOther()_(tests.test_nats.NatsTestCase   tests.test_radix_(module)
-  method)                                         tests.test_rationals_(module)
-  testInBase()_(tests.test_radix.RadixTestCase    testStr()_
-  method)                                         (tests.test_constants.RoundingMethodsTestCase
-  testInBase2()_(tests.test_radix.RadixTestCase   method)
-  method)                                               (tests.test_radix.RadixTestCase_method)
-  testInEquality()_                               testTruncation()_
+  testExceptionsUndivision()_                     tests.test_radix_(module)
+  (tests.test_division.NatDivisionTestCase        tests.test_rationals_(module)
+  method)                                         testStr()_
+  testFormat()_(tests.test_display.TestString     (tests.test_constants.RoundingMethodsTestCase
+  method)                                         method)
+  testFromInt()_(tests.test_nats.NatsTestCase           (tests.test_radix.RadixTestCase_method)
+  method)                                         TestString_(class_in_tests.test_display)
+  testFromOther()_(tests.test_nats.NatsTestCase   TestStrip_(class_in_tests.test_display)
+  method)                                         testTruncation()_
+  testInBase()_(tests.test_radix.RadixTestCase    (tests.test_division.NatDivisionTestCase
+  method)                                         method)
+  testInEquality()_                               testUpDown()_
   (tests.test_radix.RadixTestCase_method)         (tests.test_division.NatDivisionTestCase
   testInverses()_                                 method)
-  (tests.test_division.NatDivisionTestCase        testUpDown()_
-  method)                                         (tests.test_division.NatDivisionTestCase
-        (tests.test_rationals.RationalsTestCase   method)
+  (tests.test_division.NatDivisionTestCase        testXform()_(tests.test_display.TestNumber
+  method)                                         method)
+        (tests.test_rationals.RationalsTestCase         (tests.test_display.TestStrip_method)
         method)
-  testLeadingZeros()_
-  (tests.test_radix.RoundingTestCase_method)
-  testMiddles()_
-  (tests.test_radix.RoundingTestCase_method)
-  testOneHalf()_
-  (tests.test_radix.RoundingTestCase_method)
+  TestNumber_(class_in_tests.test_display)
   testOperatorExceptions()_
   (tests.test_radix.RadixTestCase_method)
   testOptions()_(tests.test_radix.RadixTestCase
   method)
+  testRepeatingRepeatPart()_
+  (tests.test_radix.RadixTestCase_method)
+  testRepr()_(tests.test_radix.RadixTestCase
+  method)
+  testRoundFraction()_
+  (tests.test_radix.RoundingTestCase_method)
 ***** U *****
   undivision()_(justbases._division.NatDivision_class_method)
+***** X *****
+  xform()_(justbases._display.Digits_class_method)
+        (justbases._display.Number_class_method)
+        (justbases._display.String_class_method)
+        (justbases._display.Strip_class_method)
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/_build/html/intro.html` & `justbases-0.9/doc/_build/html/intro.html`

 * *Files 27% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Justbases &mdash; justbases 0.5 documentation</title>
+    <title>Justbases &mdash; justbases 0.07 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.5',
+        VERSION:     '0.07',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbases 0.5 documentation" href="index.html" />
+    <link rel="top" title="justbases 0.07 documentation" href="index.html" />
     <link rel="next" title="Usage" href="usage.html" />
     <link rel="prev" title="Justbases" href="index.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Justbases"
              accesskey="P">previous</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -73,28 +73,53 @@
 <p>The complexity of operations that perform division in an arbitrary base
 can be quite high. Most methods are annotated with an estimate of their
 expected complexity in terms of the number of Python operations that they
 make use of. No differentiation is made among different Python operations.
 With respect to division in an arbitrary base, the complexity is bounded
 by the value of the divisor, unless a precision limit is set.</p>
 </div>
+<div class="section" id="related-packages">
+<h2>Related Packages<a class="headerlink" href="#related-packages" title="Permalink to this headline">¶</a></h2>
+<ul>
+<li><p class="first">allyourbase: <a class="reference external" href="https://pypi.python.org/pypi/allyourbase">https://pypi.python.org/pypi/allyourbase</a></p>
+<p>Converts a variety of numeric types to str in arbitrary bases.
+Does not require one character to digit encoding, uses a digit separator.
+Requires rounding, does not do precise conversion, but does do
+conversion to any specified precision.</p>
+</li>
+<li><p class="first">python-baseconv: <a class="reference external" href="https://pypi.python.org/pypi/allyourbase">https://pypi.python.org/pypi/allyourbase</a></p>
+<p>Converts an int to a string using a one character to digit encoding.
+Also converts in the opposite direction.
+Does not handle arbitrary rationals and does not really handle conversion to
+large bases, e.g., 1024, as such conversion would require 1024 distinct
+characters.</p>
+</li>
+<li><p class="first">python-radix: <a class="reference external" href="https://pypi.python.org/pypi/python-radix">https://pypi.python.org/pypi/python-radix</a></p>
+<p>Does not handle arbitrary bases. Converts int or int as str to str.</p>
+</li>
+<li><p class="first">numpy: <a class="reference external" href="http://docs.scipy.org/doc/numpy/reference/">http://docs.scipy.org/doc/numpy/reference/</a>
+Converts int to str in bases between 2 and 36.</p>
+</li>
+</ul>
+</div>
 </div>
 
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h3><a href="index.html">Table Of Contents</a></h3>
   <ul>
 <li><a class="reference internal" href="#">Justbases</a><ul>
 <li><a class="reference internal" href="#purpose">Purpose</a></li>
 <li><a class="reference internal" href="#motivation">Motivation</a></li>
 <li><a class="reference internal" href="#algorithmic-complexity">Algorithmic Complexity</a></li>
+<li><a class="reference internal" href="#related-packages">Related Packages</a></li>
 </ul>
 </li>
 </ul>
 
   <h4>Previous topic</h4>
   <p class="topless"><a href="index.html"
                         title="previous chapter">Justbases</a></p>
@@ -134,15 +159,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="usage.html" title="Usage"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Justbases"
              >previous</a> |</li>
-        <li><a href="index.html">justbases 0.5 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbases 0.07 documentation</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 ****** Justbases¶ ******
 ***** Purpose¶ *****
 Conversion of a rational number to a representation in any base. Any rational
 number can be represented as a repeating sequence in any base. Any integer is
 representable as a terminating sequence in any base.
 ***** Motivation¶ *****
 This facility does not seem to exist in standard Python numerical packages or
@@ -21,28 +21,44 @@
 ***** Algorithmic Complexity¶ *****
 The complexity of operations that perform division in an arbitrary base can be
 quite high. Most methods are annotated with an estimate of their expected
 complexity in terms of the number of Python operations that they make use of.
 No differentiation is made among different Python operations. With respect to
 division in an arbitrary base, the complexity is bounded by the value of the
 divisor, unless a precision limit is set.
+***** Related Packages¶ *****
+    * allyourbase: https://pypi.python.org/pypi/allyourbase
+      Converts a variety of numeric types to str in arbitrary bases. Does not
+      require one character to digit encoding, uses a digit separator. Requires
+      rounding, does not do precise conversion, but does do conversion to any
+      specified precision.
+    * python-baseconv: https://pypi.python.org/pypi/allyourbase
+      Converts an int to a string using a one character to digit encoding. Also
+      converts in the opposite direction. Does not handle arbitrary rationals
+      and does not really handle conversion to large bases, e.g., 1024, as such
+      conversion would require 1024 distinct characters.
+    * python-radix: https://pypi.python.org/pypi/python-radix
+      Does not handle arbitrary bases. Converts int or int as str to str.
+    * numpy: http://docs.scipy.org/doc/numpy/reference/ Converts int to str in
+      bases between 2 and 36.
 **** Table_Of_Contents ****
     * Justbases
           o Purpose
           o Motivation
           o Algorithmic_Complexity
+          o Related_Packages
 *** Previous topic ***
 Justbases
 *** Next topic ***
 Usage
 **** This Page ****
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbases_0.5_documentation »
+    * justbases_0.07_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbases-0.6/doc/usage.rst` & `justbases-0.9/doc/usage.rst`

 * *Files 3% similar despite different names*

```diff
@@ -100,16 +100,16 @@
     >>> Radix(False, [1], [2], [1], 10)
     >>> -1.2[1]_10
     >>> Radix(True, [12, 13], [4], [], 16)
     >>> 12:13.4[]_16
 
 Note that the number after the underscore represents the base, and the
 digits within square brackets represent the repeating portion of the
-number. Individual digits, in a decimal representation, are separated by
-':''s. This approach supports arbitrary bases.
+number. Individual digits in a decimal representation require a separator,
+here a ':'. This approach supports arbitrary bases.
 
 The Radix constructor validates and canonicalizes the Radix.
 Validation ensures that the digits are within the appropriate range
 for the given base, and other digits. Canonicalization ensures a canonical
 representation for equivalent Radix values. For example, it reduces
 the repeating part to the smallest possible. ::
 
@@ -169,14 +169,25 @@
 If the goal is to obtain a radix value from a rounded rational quantity it is
 more efficient to use Rationals.convert_from_rational() with precision and
 method arguments set. ::
 
     >>> Rationals.convert_from_rational(Fraction(1, 3), 2, 1, RoundingMethods.ROUND_UP)
     >>> (.1[]_2, 1)
 
+
+Display
+-------
+Radix.getString() returns a string representing a Radix object. The form of
+this string can be modified using the config parameter. The justbases-gui
+library is useful for experimenting with the different configuration options,
+which control such things as the choice of representation for digits larger
+than 9, whether or not to strip trailing zeros, and so forth. Consult the
+justbases-gui documentation for its usage.
+
+
 Concrete Example: Geographic Coordinates
 ----------------------------------------
 Latitude and longitude are frequently expressed in degrees, minutes, and
 seconds, using the base 60. Below is a simple exercise to translate
 a given latitude into alternative formats. ::
 
     >>> latitude = (42, 38, 0) # latitude measurement
```

### Comparing `justbases-0.6/doc/conf.py` & `justbases-0.9/doc/conf.py`

 * *Files identical despite different names*

