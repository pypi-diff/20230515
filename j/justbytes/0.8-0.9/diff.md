# Comparing `tmp/justbytes-0.8.tar.gz` & `tmp/justbytes-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/justbytes-0.8.tar", last modified: Mon May  9 14:22:55 2016, max compression
+gzip compressed data, was "dist/justbytes-0.9.tar", last modified: Mon May 16 15:38:47 2016, max compression
```

## Comparing `justbytes-0.8.tar` & `justbytes-0.9.tar`

### file list

```diff
@@ -1,173 +1,171 @@
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6080 2016-05-09 14:21:42.000000 justbytes-0.8/README.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3563 2016-05-09 14:21:42.000000 justbytes-0.8/tests/config_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       32 2015-12-07 15:27:05.000000 justbytes-0.8/tests/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1535 2016-04-29 17:23:28.000000 justbytes-0.8/tests/utils.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1278 2016-05-09 14:21:42.000000 justbytes-0.8/tests/version_test.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/tests/size/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9934 2016-05-09 14:21:42.000000 justbytes-0.8/tests/size/size_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       35 2015-12-07 15:27:05.000000 justbytes-0.8/tests/size/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2843 2016-04-29 17:23:28.000000 justbytes-0.8/tests/size/initializer_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    17437 2016-05-09 14:21:42.000000 justbytes-0.8/tests/size/operations_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2808 2016-04-29 17:23:28.000000 justbytes-0.8/tests/size/conversions_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9342 2016-05-09 14:21:42.000000 justbytes-0.8/tests/size/named_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2020 2016-03-15 21:29:30.000000 justbytes-0.8/tests/constants_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2354 2016-04-29 17:23:28.000000 justbytes-0.8/tests/errors_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2821 2016-05-06 19:34:20.000000 justbytes-0.8/tests/util_test.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8038 2016-05-09 14:22:55.000000 justbytes-0.8/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    18027 2015-12-07 15:27:05.000000 justbytes-0.8/LICENSE
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       59 2016-05-09 14:22:55.000000 justbytes-0.8/setup.cfg
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/src/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/src/justbytes/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1256 2016-05-09 14:21:42.000000 justbytes-0.8/src/justbytes/version.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3641 2016-05-09 14:21:42.000000 justbytes-0.8/src/justbytes/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4235 2016-04-29 17:23:28.000000 justbytes-0.8/src/justbytes/_errors.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7277 2016-05-09 14:21:42.000000 justbytes-0.8/src/justbytes/_config.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/src/justbytes/_util/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2015-12-07 15:27:05.000000 justbytes-0.8/src/justbytes/_util/__init__.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1912 2016-04-29 17:23:28.000000 justbytes-0.8/src/justbytes/_util/generators.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    19163 2016-05-09 14:21:42.000000 justbytes-0.8/src/justbytes/_size.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3585 2016-03-15 21:29:30.000000 justbytes-0.8/src/justbytes/_constants.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1146 2016-04-29 17:23:28.000000 justbytes-0.8/src/justbytes/_sizes.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/src/justbytes.egg-info/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8038 2016-05-09 14:22:22.000000 justbytes-0.8/src/justbytes.egg-info/PKG-INFO
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       19 2016-05-09 14:22:22.000000 justbytes-0.8/src/justbytes.egg-info/requires.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9235 2016-05-09 14:22:22.000000 justbytes-0.8/src/justbytes.egg-info/SOURCES.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2016-05-09 14:22:22.000000 justbytes-0.8/src/justbytes.egg-info/dependency_links.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       10 2016-05-09 14:22:22.000000 justbytes-0.8/src/justbytes.egg-info/top_level.txt
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      541 2016-03-15 21:29:30.000000 justbytes-0.8/tox.ini
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2501 2016-05-09 14:21:42.000000 justbytes-0.8/setup.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      198 2016-04-29 17:23:28.000000 justbytes-0.8/MANIFEST.in
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/_build/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/_build/html/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7123 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/index.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3424 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/search.html
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/_build/html/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5815 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/modules.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7819 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.config_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4767 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.utils.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6443 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.constants_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    26993 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.operations_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7173 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.errors_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6398 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.initializer_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7078 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.util_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    10871 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.named_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6101 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5065 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.version_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7085 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7431 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.conversions_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13096 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tests/tests.size.size_test.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    15331 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/tutorial.html
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/_build/html/justbytes/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11220 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._errors.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5923 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/modules.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    14977 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._size.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    15829 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._util.display.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5753 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._util.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    10367 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13647 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._constants.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11690 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._config.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4867 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._sizes.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7410 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes._util.generators.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5171 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/justbytes/justbytes.version.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8805 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/py-modindex.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    44713 2016-04-15 17:44:59.000000 justbytes-0.8/doc/_build/html/genindex.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13191 2016-04-15 17:44:58.000000 justbytes-0.8/doc/_build/html/intro.html
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3324 2016-04-29 17:23:28.000000 justbytes-0.8/doc/tutorial.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/tests/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      169 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.operations_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      335 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.config_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      356 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.utils.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       52 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/modules.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.errors_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.initializer_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      145 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.version_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.conversions_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.util_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      154 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.named_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.constants_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-04-15 17:43:13.000000 justbytes-0.8/doc/tests/tests.size.size_test.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9256 2016-03-15 21:29:30.000000 justbytes-0.8/doc/conf.py
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/justbytes/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._constants.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._config.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._errors.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      139 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._sizes.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      169 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._util.generators.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       64 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/modules.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      377 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      266 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._util.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes.version.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      160 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._util.display.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-04-15 17:43:13.000000 justbytes-0.8/doc/justbytes/justbytes._size.rst
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/.hypothesis/
-drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-09 14:22:55.000000 justbytes-0.8/doc/.hypothesis/eval_source/
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_86084da96d1ac1368738e3e2ff43c55363adfa3d.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_3f7411c21a40bfdc1d4a385395abcf8f35bfc403.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      196 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_ef8990d92334f35ee5d335441130f46e6b79464f.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_122a8f9fcdccd59b90df58d0558e44bcca216ab8.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      138 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_f921b2988402df61d5f91622b67a9e50eddd05fc.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      190 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_a83549744edbd85f92b3c16526369cb62b7fc136.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_ad3b1319e5371eb5b80a0f4b62a10c1d78021704.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      280 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_157a06c7111ab0b1f1a33822a57773ed79d45d30.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_621300bdc0e0e7ac8e12999febbf3ed4b3ac337b.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_84deb0667079aa1ef02457217332c31964ecca97.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      164 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e8bacd0c79736e8f5e797f4edf92193cc4b99bd8.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_5a7bc10d8015157dedbac1465811f364be31ca17.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      200 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e5409415cc2bf86aa528c685966f3ccd004561d2.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_1eba03841185292c6018ae372c9f399bb5b99054.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_c0ae01439d37e01a7fda92c9ba026a063ed92e23.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      222 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_5acac66a6b63340044870297f67e1a822354f8d3.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_6a04bc0a5628023f3ef64d8e71c211628907422b.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_4388d4ebddbb3b9e35b6951c1c3e3ca47f2facce.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_575c46161da71f5baee220ccac6c2069d30f4506.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_27293c5549237bae7b26a5803947ff8c4f839122.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      184 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_8038dad65c575bf95673c527fc0a2ad06b1a3d5f.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      126 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_0338617ff66788f1ab9d5142f849106ae9b38d15.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e5efaf5ab73b5aef0d8286891a60db7cf3c1bf0f.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_080187190c9678ad026ff7798702777438a6c116.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      208 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_cdc3a7a5201e39632a956c5967c0a91af8267df9.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      264 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_302a2bf2b98d37c182da92de76c16ff408d9447c.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      170 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_bee2c2b7dfa97e6160a60eb0fe293d9a137fc063.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      260 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e7ac20823eddd3e706aaf44693170920005cb871.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      196 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_9f5459bf06b79adce8339658d6cc2fbdebf5cb57.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      130 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_319ade46afdab08a61611170bc661bd6b6fd0507.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_c181f408597ad7be0e17e78ecef893f7ee7054d6.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_12562534fc1cd5ce9e48ce9f6025a94d4071d7a1.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_2dea9c7498284093108163b15d385b516d6fb6c5.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      122 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_2cea1af442c7f053fe19b734be9a6a80bbafb877.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8e1c2f035c79eecc2fde6a0d9cb04a2361a73b6.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_0529b12987b897d7290f83bcbcc804e28602383d.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      168 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_d5195fa3907eabde9ac871a4541b194bc04459ba.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      184 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_18a332bae68cd42ec9a38dc0ba292cfef80615b6.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e205a47d7c6729bf54a35378da04fa1aa29ba947.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_63689e27bbbd0aadc198d0b4f6b46affd7502238.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      214 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_b2ac5d495d365a28966ba71ba676c697b620d516.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_6e3c8548c9c96d6a7dfceb69cbb7b364cd64b92e.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      146 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_3c94c71e9e33e081b43be6e2046f3a3f8fab3067.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_5c738403ba605385711d5acd8d7ef40c99df061a.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      236 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_157c02e78a2f3560de74aceff294a8477134e84e.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_6dac1361332e428a8c485a28763b2ae6d48fdf4e.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_65898f03aceece8bd7d2fd24071cd1c0822ad02e.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_9345cdfcc00c612f74fd583fd23cd20cd7a11cc7.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      178 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_f37fbe148cfea62250b5590c72f91c0d08cee669.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      164 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_e461492a44cac2c3de668fe6111541e94c1db2e5.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      220 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_5636994f6917eb8503acb6c08bc455bee0bec463.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_a993f5cddd9d22f6beea0e79bc1785a8f6f492c7.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      228 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_9498d7385a53736b109ba29dbe7c33e582824d55.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      244 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_2e71923a5f523fc7899142bce080a648f473d503.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_12c1d00d532807965223eb08a44fcda50c228e44.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      116 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_9abd2800900986980ad8f68a32f0005fc05800d8.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      178 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_d4221348178579011f4e86ab0abc6a1d645d59cd.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8478d2d985b5b4bb830f8419c093e22c692e027.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      198 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_d5a534972c3f8afbcb040ce52c7ea171022473c5.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      160 2015-12-16 14:32:03.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_734e196042ddeeb1fb8480a9c02b1e2ce68027b7.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      190 2015-12-16 14:21:00.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_31b625635c53e0532b2ea931ab0f3f201dd6cbc8.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      154 2015-12-16 14:21:01.000000 justbytes-0.8/doc/.hypothesis/eval_source/hypothesis_temporary_module_953f6bd03b9b7cae8f1b688acd38e85e602f309b.py
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      489 2015-12-07 15:35:49.000000 justbytes-0.8/doc/index.rst
-lrwxrwxrwx   0 mulhern   (1000) mulhern   (1000)        0 2015-12-07 15:27:05.000000 justbytes-0.8/doc/intro.rst -> ../README.rst
--rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2015-12-07 15:27:05.000000 justbytes-0.8/requirements.txt
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6080 2016-05-09 14:57:09.000000 justbytes-0.9/README.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3611 2016-05-16 15:37:35.000000 justbytes-0.9/tests/config_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       32 2015-12-07 15:27:05.000000 justbytes-0.9/tests/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1535 2016-05-09 14:56:28.000000 justbytes-0.9/tests/utils.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1278 2016-05-16 15:37:35.000000 justbytes-0.9/tests/version_test.py
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/tests/size/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9872 2016-05-16 15:37:35.000000 justbytes-0.9/tests/size/size_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       35 2015-12-07 15:27:05.000000 justbytes-0.9/tests/size/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2843 2016-05-09 14:56:28.000000 justbytes-0.9/tests/size/initializer_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    17437 2016-05-09 14:57:56.000000 justbytes-0.9/tests/size/operations_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2808 2016-05-09 14:56:28.000000 justbytes-0.9/tests/size/conversions_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9746 2016-05-16 15:37:35.000000 justbytes-0.9/tests/size/named_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2020 2016-03-15 21:29:30.000000 justbytes-0.9/tests/constants_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2354 2016-05-09 14:56:28.000000 justbytes-0.9/tests/errors_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2821 2016-05-09 14:56:01.000000 justbytes-0.9/tests/util_test.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8038 2016-05-16 15:38:47.000000 justbytes-0.9/PKG-INFO
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    18027 2015-12-07 15:27:05.000000 justbytes-0.9/LICENSE
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       59 2016-05-16 15:38:47.000000 justbytes-0.9/setup.cfg
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/src/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/src/justbytes/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1256 2016-05-16 15:37:35.000000 justbytes-0.9/src/justbytes/version.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3670 2016-05-16 15:37:35.000000 justbytes-0.9/src/justbytes/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4235 2016-05-09 14:56:28.000000 justbytes-0.9/src/justbytes/_errors.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8229 2016-05-16 15:37:35.000000 justbytes-0.9/src/justbytes/_config.py
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/src/justbytes/_util/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        0 2015-12-07 15:27:05.000000 justbytes-0.9/src/justbytes/_util/__init__.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1912 2016-05-09 14:56:01.000000 justbytes-0.9/src/justbytes/_util/generators.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    19072 2016-05-16 15:37:35.000000 justbytes-0.9/src/justbytes/_size.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3585 2016-03-15 21:29:30.000000 justbytes-0.9/src/justbytes/_constants.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     1146 2016-05-09 14:56:28.000000 justbytes-0.9/src/justbytes/_sizes.py
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/src/justbytes.egg-info/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8038 2016-05-16 15:38:35.000000 justbytes-0.9/src/justbytes.egg-info/PKG-INFO
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       19 2016-05-16 15:38:35.000000 justbytes-0.9/src/justbytes.egg-info/requires.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9138 2016-05-16 15:38:35.000000 justbytes-0.9/src/justbytes.egg-info/SOURCES.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        1 2016-05-16 15:38:35.000000 justbytes-0.9/src/justbytes.egg-info/dependency_links.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       10 2016-05-16 15:38:35.000000 justbytes-0.9/src/justbytes.egg-info/top_level.txt
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      568 2016-05-16 15:37:35.000000 justbytes-0.9/tox.ini
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     2501 2016-05-16 15:37:35.000000 justbytes-0.9/setup.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      198 2016-05-09 14:56:01.000000 justbytes-0.9/MANIFEST.in
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/_build/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/_build/html/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7145 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/index.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3424 2016-05-09 14:26:08.000000 justbytes-0.9/doc/_build/html/search.html
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/_build/html/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5815 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/modules.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7819 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.config_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4767 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.utils.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6443 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.constants_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    26993 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.operations_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7173 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.errors_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6398 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.initializer_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7078 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.util_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    10871 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.named_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     6101 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5065 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.version_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7085 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7431 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.conversions_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13096 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tests/tests.size.size_test.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    15331 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/tutorial.html
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/_build/html/justbytes/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11220 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._errors.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5923 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/modules.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    14977 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._size.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5648 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._util.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    10238 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13647 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._constants.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    11022 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._config.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     4867 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._sizes.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     7350 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes._util.generators.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     5171 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/justbytes/justbytes.version.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     8562 2016-05-09 14:26:08.000000 justbytes-0.9/doc/_build/html/py-modindex.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    42430 2016-05-09 14:26:08.000000 justbytes-0.9/doc/_build/html/genindex.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)    13389 2016-05-09 14:26:07.000000 justbytes-0.9/doc/_build/html/intro.html
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     3324 2016-05-09 14:56:28.000000 justbytes-0.9/doc/tutorial.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/tests/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      169 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.operations_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      335 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.config_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      356 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.utils.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       52 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/modules.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.errors_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.initializer_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      145 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.version_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.conversions_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.util_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      154 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.named_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.constants_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:04.000000 justbytes-0.9/doc/tests/tests.size.size_test.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)     9256 2016-03-15 21:29:30.000000 justbytes-0.9/doc/conf.py
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/justbytes/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      151 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._constants.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._config.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._errors.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      139 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._sizes.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      169 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._util.generators.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)       64 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/modules.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      377 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      239 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._util.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes.version.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      136 2016-05-09 14:26:03.000000 justbytes-0.9/doc/justbytes/justbytes._size.rst
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/.hypothesis/
+drwxrwxr-x   0 mulhern   (1000) mulhern   (1000)        0 2016-05-16 15:38:47.000000 justbytes-0.9/doc/.hypothesis/eval_source/
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_86084da96d1ac1368738e3e2ff43c55363adfa3d.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_3f7411c21a40bfdc1d4a385395abcf8f35bfc403.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      196 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_ef8990d92334f35ee5d335441130f46e6b79464f.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      158 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_122a8f9fcdccd59b90df58d0558e44bcca216ab8.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      138 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f921b2988402df61d5f91622b67a9e50eddd05fc.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      190 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_a83549744edbd85f92b3c16526369cb62b7fc136.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      142 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_ad3b1319e5371eb5b80a0f4b62a10c1d78021704.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      280 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_157a06c7111ab0b1f1a33822a57773ed79d45d30.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_621300bdc0e0e7ac8e12999febbf3ed4b3ac337b.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_84deb0667079aa1ef02457217332c31964ecca97.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      164 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e8bacd0c79736e8f5e797f4edf92193cc4b99bd8.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_5a7bc10d8015157dedbac1465811f364be31ca17.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      200 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e5409415cc2bf86aa528c685966f3ccd004561d2.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_1eba03841185292c6018ae372c9f399bb5b99054.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_c0ae01439d37e01a7fda92c9ba026a063ed92e23.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      222 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_5acac66a6b63340044870297f67e1a822354f8d3.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_6a04bc0a5628023f3ef64d8e71c211628907422b.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      192 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_4388d4ebddbb3b9e35b6951c1c3e3ca47f2facce.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_575c46161da71f5baee220ccac6c2069d30f4506.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_27293c5549237bae7b26a5803947ff8c4f839122.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      184 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_8038dad65c575bf95673c527fc0a2ad06b1a3d5f.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      126 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_0338617ff66788f1ab9d5142f849106ae9b38d15.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      176 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e5efaf5ab73b5aef0d8286891a60db7cf3c1bf0f.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_080187190c9678ad026ff7798702777438a6c116.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      208 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_cdc3a7a5201e39632a956c5967c0a91af8267df9.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      264 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_302a2bf2b98d37c182da92de76c16ff408d9447c.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      170 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_bee2c2b7dfa97e6160a60eb0fe293d9a137fc063.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      260 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e7ac20823eddd3e706aaf44693170920005cb871.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      196 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9f5459bf06b79adce8339658d6cc2fbdebf5cb57.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      130 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_319ade46afdab08a61611170bc661bd6b6fd0507.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_c181f408597ad7be0e17e78ecef893f7ee7054d6.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_12562534fc1cd5ce9e48ce9f6025a94d4071d7a1.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_2dea9c7498284093108163b15d385b516d6fb6c5.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      122 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_2cea1af442c7f053fe19b734be9a6a80bbafb877.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8e1c2f035c79eecc2fde6a0d9cb04a2361a73b6.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_0529b12987b897d7290f83bcbcc804e28602383d.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      168 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_d5195fa3907eabde9ac871a4541b194bc04459ba.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      184 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_18a332bae68cd42ec9a38dc0ba292cfef80615b6.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e205a47d7c6729bf54a35378da04fa1aa29ba947.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_63689e27bbbd0aadc198d0b4f6b46affd7502238.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      214 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_b2ac5d495d365a28966ba71ba676c697b620d516.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      188 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_6e3c8548c9c96d6a7dfceb69cbb7b364cd64b92e.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      146 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_3c94c71e9e33e081b43be6e2046f3a3f8fab3067.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      180 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_5c738403ba605385711d5acd8d7ef40c99df061a.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      236 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_157c02e78a2f3560de74aceff294a8477134e84e.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      172 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_6dac1361332e428a8c485a28763b2ae6d48fdf4e.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      186 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_65898f03aceece8bd7d2fd24071cd1c0822ad02e.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      182 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9345cdfcc00c612f74fd583fd23cd20cd7a11cc7.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      178 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f37fbe148cfea62250b5590c72f91c0d08cee669.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      164 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_e461492a44cac2c3de668fe6111541e94c1db2e5.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      220 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_5636994f6917eb8503acb6c08bc455bee0bec463.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      124 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_a993f5cddd9d22f6beea0e79bc1785a8f6f492c7.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      228 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9498d7385a53736b109ba29dbe7c33e582824d55.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      244 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_2e71923a5f523fc7899142bce080a648f473d503.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      144 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_12c1d00d532807965223eb08a44fcda50c228e44.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      116 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_9abd2800900986980ad8f68a32f0005fc05800d8.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      178 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_d4221348178579011f4e86ab0abc6a1d645d59cd.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      232 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_f8478d2d985b5b4bb830f8419c093e22c692e027.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      198 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_d5a534972c3f8afbcb040ce52c7ea171022473c5.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      160 2015-12-16 14:32:03.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_734e196042ddeeb1fb8480a9c02b1e2ce68027b7.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      190 2015-12-16 14:21:00.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_31b625635c53e0532b2ea931ab0f3f201dd6cbc8.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      154 2015-12-16 14:21:01.000000 justbytes-0.9/doc/.hypothesis/eval_source/hypothesis_temporary_module_953f6bd03b9b7cae8f1b688acd38e85e602f309b.py
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)      489 2015-12-07 15:35:49.000000 justbytes-0.9/doc/index.rst
+lrwxrwxrwx   0 mulhern   (1000) mulhern   (1000)        0 2015-12-07 15:27:05.000000 justbytes-0.9/doc/intro.rst -> ../README.rst
+-rw-rw-r--   0 mulhern   (1000) mulhern   (1000)        4 2015-12-07 15:27:05.000000 justbytes-0.9/requirements.txt
```

### Comparing `justbytes-0.8/README.rst` & `justbytes-0.9/README.rst`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/config_test.py` & `justbytes-0.9/tests/config_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 """ Test for configuration classes. """
 import unittest
 
 from hypothesis import given
 from hypothesis import settings
 from hypothesis import strategies
 
+from justbytes._config import Config
 from justbytes._config import DisplayConfig
-from justbytes._config import RangeConfig
 from justbytes._config import ValueConfig
 
 from justbytes._constants import UNITS
 
 from justbytes._errors import RangeValueError
 
 
 class ConfigTestCase(unittest.TestCase):
     """ Exercise methods of output configuration classes. """
     # pylint: disable=too-few-public-methods
 
     def testValueConfigObject(self):
         """ Miscellaneous tests for string configuration. """
-        self.assertIsInstance(str(RangeConfig.VALUE_CONFIG), str)
+        self.assertIsInstance(str(Config.STRING_CONFIG.VALUE_CONFIG), str)
 
     def testException(self):
         """ Test exceptions. """
         with self.assertRaises(RangeValueError):
             ValueConfig(min_value=-1)
         with self.assertRaises(RangeValueError):
             ValueConfig(min_value=3.2)
@@ -55,41 +55,41 @@
 
 
 class RangeTestCase(unittest.TestCase):
     """ Test Range configuration. """
     # pylint: disable=too-few-public-methods
 
     def setUp(self):
-        self.display_config = RangeConfig.DISPLAY_CONFIG
-        self.str_config = RangeConfig.VALUE_CONFIG
+        self.display_config = Config.STRING_CONFIG.DISPLAY_CONFIG
+        self.str_config = Config.STRING_CONFIG.VALUE_CONFIG
 
     def tearDown(self):
-        RangeConfig.DISPLAY_CONFIG = self.display_config
-        RangeConfig.VALUE_CONFIG = self.str_config
+        Config.STRING_CONFIG.DISPLAY_CONFIG = self.display_config
+        Config.STRING_CONFIG.VALUE_CONFIG = self.str_config
 
     @given(
        strategies.builds(
           DisplayConfig,
           show_approx_str=strategies.booleans()
        )
     )
     @settings(max_examples=30)
     def testSettingDisplayConfig(self, config):
         """ Test that new str config is the correct one. """
-        RangeConfig.set_display_config(config)
-        self.assertEqual(str(config), str(RangeConfig.DISPLAY_CONFIG))
+        Config.set_display_config(config)
+        self.assertEqual(str(config), str(Config.STRING_CONFIG.DISPLAY_CONFIG))
 
     @given(
        strategies.builds(
           ValueConfig,
           binary_units=strategies.booleans(),
           max_places=strategies.integers().filter(lambda x: x >= 0),
           min_value=strategies.fractions().filter(lambda x: x >= 0),
           exact_value=strategies.booleans(),
           unit=strategies.sampled_from(UNITS())
        )
     )
     @settings(max_examples=30)
     def testSettingValueConfig(self, config):
         """ Test that new str config is the correct one. """
-        RangeConfig.set_value_config(config)
-        self.assertEqual(str(config), str(RangeConfig.VALUE_CONFIG))
+        Config.set_value_config(config)
+        self.assertEqual(str(config), str(Config.STRING_CONFIG.VALUE_CONFIG))
```

### Comparing `justbytes-0.8/tests/utils.py` & `justbytes-0.9/tests/utils.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/version_test.py` & `justbytes-0.9/tests/version_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 
 
 class VersionTestCase(unittest.TestCase):
     """ Test version. """
 
     def testValue(self):
         """ That value is reasonable. """
-        self.assertEqual(justbytes.__version__, '0.08')
+        self.assertEqual(justbytes.__version__, '0.09')
```

### Comparing `justbytes-0.8/tests/size/size_test.py` & `justbytes-0.9/tests/size/size_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from justbytes import GiB
 from justbytes import TiB
 from justbytes import KB
 from justbytes import DisplayConfig
 from justbytes import ValueConfig
 from justbytes import StripConfig
 
-from justbytes._config import RangeConfig
+from justbytes._config import Config
 
 from justbytes._errors import RangeFractionalResultError
 from justbytes._errors import RangeValueError
 
 
 class ConstructionTestCase(unittest.TestCase):
     """ Test construction of Range objects. """
@@ -145,25 +145,25 @@
         self.assertEqual(s.components(ValueConfig(binary_units=False)), (1, KB))
 
 class ConfigurationTestCase(unittest.TestCase):
     """ Test setting configuration for display. """
 
     def setUp(self):
         """ Get current config. """
-        self.str_config = RangeConfig.VALUE_CONFIG
-        self.display_config = RangeConfig.DISPLAY_CONFIG
+        self.str_config = Config.STRING_CONFIG.VALUE_CONFIG
+        self.display_config = Config.STRING_CONFIG.DISPLAY_CONFIG
 
     def tearDown(self):
         """ Reset configuration to default. """
-        RangeConfig.set_value_config(self.str_config)
-        RangeConfig.set_display_config(self.display_config)
+        Config.set_value_config(self.str_config)
+        Config.set_display_config(self.display_config)
 
     def testValueConfigs(self):
         """ Test str with various configuration options. """
-        RangeConfig.set_display_config(
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=True)
            )
         )
 
         # exactly 4 Pi
         s = Range(0x10000000000000)
@@ -196,64 +196,64 @@
         self.assertEqual(str(s), "< 4 PiB")
 
         s = Range(0xffff)
         # value is not exactly 64 KiB, but w/ 2 places, value is 64.00 KiB
         # so the trailing 0s are stripped.
         self.assertEqual(str(s), "< 64 KiB")
 
-        RangeConfig.set_value_config(ValueConfig(max_places=3))
-        RangeConfig.set_display_config(
+        Config.set_value_config(ValueConfig(max_places=3))
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=True)
            )
         )
         s = Range('23.7874', TiB)
         self.assertEqual(str(s), "> 23.787 TiB")
 
-        RangeConfig.set_value_config(ValueConfig(min_value=10))
-        RangeConfig.set_display_config(
+        Config.set_value_config(ValueConfig(min_value=10))
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=True)
            )
         )
         s = Range(8193)
         self.assertEqual(str(s), ("8193 B"))
 
         # if max_places is set to None, all digits are displayed
-        RangeConfig.set_value_config(ValueConfig(max_places=None))
-        RangeConfig.set_display_config(
+        Config.set_value_config(ValueConfig(max_places=None))
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=True)
            )
         )
         s = Range(0xfffffffffffff)
         self.assertEqual(
            str(s),
            "3.99999999999999911182158029987476766109466552734375 PiB"
         )
         s = Range(0x10000)
         self.assertEqual(str(s), ("64 KiB"))
         s = Range(0x10001)
         self.assertEqual(str(s), "64.0009765625 KiB")
 
-        RangeConfig.set_value_config(ValueConfig(max_places=2))
-        RangeConfig.set_display_config(
+        Config.set_value_config(ValueConfig(max_places=2))
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=False)
            )
         )
         s = Range(1024**9 + 1)
         self.assertEqual(str(s), "> 1024.00 YiB")
 
         s = Range(0xfffff)
         self.assertEqual(str(s), "< 1024.00 KiB")
 
     def testStrWithSmallDeviations(self):
         """ Behavior when deviation from whole value is small. """
-        RangeConfig.set_display_config(
+        Config.set_display_config(
            DisplayConfig(
               strip_config=StripConfig(strip=True)
            )
         )
 
         eps = Decimal(1024)/100/2 # 1/2 of 1% of 1024
 
@@ -275,20 +275,20 @@
 
 
 class ComputationTestCase(unittest.TestCase):
     """ Test setting configuration for computation. """
 
     def setUp(self):
         """ Get current config. """
-        self.strict = RangeConfig.STRICT
+        self.strict = Config.STRICT
 
     def tearDown(self):
         """ Reset configuration to default. """
-        RangeConfig.STRICT = self.strict
+        Config.STRICT = self.strict
 
     def testFractionalBytes(self):
         """
         Test that error is raised on fractional bytes when EXACT is True.
         """
-        RangeConfig.STRICT = True
+        Config.STRICT = True
         with self.assertRaises(RangeFractionalResultError):
             Range(Fraction(1, 2))
```

### Comparing `justbytes-0.8/tests/size/initializer_test.py` & `justbytes-0.9/tests/size/initializer_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/size/operations_test.py` & `justbytes-0.9/tests/size/operations_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/size/conversions_test.py` & `justbytes-0.9/tests/size/conversions_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/size/named_test.py` & `justbytes-0.9/tests/size/named_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,28 +34,27 @@
 from justbytes import ROUND_DOWN
 from justbytes import ROUND_HALF_DOWN
 from justbytes import ROUND_HALF_UP
 from justbytes import ROUND_TO_ZERO
 from justbytes import ROUND_UP
 from justbytes import ROUNDING_METHODS
 from justbytes import BaseConfig
+from justbytes import Config
 from justbytes import DigitsConfig
 from justbytes import DisplayConfig
-from justbytes import RangeConfig
+from justbytes import StringConfig
 from justbytes import StripConfig
 from justbytes import ValueConfig
 
 from justbytes._constants import BinaryUnits
 from justbytes._constants import DecimalUnits
 from justbytes._constants import UNITS
 
 from justbytes._errors import RangeValueError
 
-from justbases import BasesError
-
 from tests.utils import SIZE_STRATEGY
 
 class ConversionTestCase(unittest.TestCase):
     """ Test conversion methods. """
 
     def testException(self):
         """ Test exceptions. """
@@ -128,15 +127,21 @@
        strategies.integers(min_value=2, max_value=16)
     )
     @settings(max_examples=100)
     def testConfig(self, a_size, config, base):
         """
         Test properties of configuration.
         """
-        result = a_size.getString(ValueConfig(base=base), config)
+        result = a_size.getString(
+           StringConfig(
+              ValueConfig(base=base),
+              config,
+              Config.STRING_CONFIG.DISPLAY_IMPL_CLASS
+           )
+        )
 
         if config.base_config.use_prefix and base == 16:
             self.assertNotEqual(result.find('0x'), -1)
 
 class DigitsConfigTestCase(unittest.TestCase):
     """
     Test digits config.
@@ -153,16 +158,19 @@
     )
     @settings(max_examples=50)
     def testConfig(self, a_size, config):
         """
         Test some basic configurations.
         """
         result = a_size.getString(
-           RangeConfig.VALUE_CONFIG,
-           DisplayConfig(digits_config=config)
+           StringConfig(
+              Config.STRING_CONFIG.VALUE_CONFIG,
+              DisplayConfig(digits_config=config),
+              Config.STRING_CONFIG.DISPLAY_IMPL_CLASS
+           )
         )
         if config.use_letters:
             (number, _, _) = result.partition(' ')
             letters = [r for r in number if r in string.ascii_letters]
             if config.use_caps:
                 self.assertTrue(
                    all(r in string.ascii_uppercase for r in letters)
@@ -172,16 +180,22 @@
                    all(r in string.ascii_lowercase for r in letters)
                 )
 
     def testExceptions(self):
         """
         Test exceptions.
         """
-        with self.assertRaises(BasesError):
-            Range(0).getString(ValueConfig(base=100), RangeConfig.DISPLAY_CONFIG)
+        with self.assertRaises(RangeValueError):
+            Range(0).getString(
+               StringConfig(
+                  ValueConfig(base=100),
+                  Config.STRING_CONFIG.DISPLAY_CONFIG,
+                  Config.STRING_CONFIG.DISPLAY_IMPL_CLASS
+               )
+            )
 
 
 class RoundingTestCase(unittest.TestCase):
     """ Test rounding methods. """
 
     @given(
        SIZE_STRATEGY,
```

### Comparing `justbytes-0.8/tests/constants_test.py` & `justbytes-0.9/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/errors_test.py` & `justbytes-0.9/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/tests/util_test.py` & `justbytes-0.9/tests/util_test.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/PKG-INFO` & `justbytes-0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: justbytes
-Version: 0.8
+Version: 0.9
 Summary: computing with and displaying bytes
 Home-page: http://pythonhosted.org/justbytes/
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
 License: GPL 2+
 Description: .. image:: https://secure.travis-ci.org/mulkieran/justbytes.png?branch=master
            :target: http://travis-ci.org/mulkieran/justbytes
```

### Comparing `justbytes-0.8/LICENSE` & `justbytes-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/src/justbytes/version.py` & `justbytes-0.9/src/justbytes/version.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,9 +22,9 @@
     =================
 
     Version information.
 
     .. moduleauthor::  mulhern  <amulhern@redhat.com>
 """
 
-__version__ = '0.08'
+__version__ = '0.09'
 __version_info__ = tuple(int(x) for x in __version__.split('.'))
```

### Comparing `justbytes-0.8/src/justbytes/__init__.py` & `justbytes-0.9/src/justbytes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,17 +114,18 @@
 ROUND_TO_ZERO = _RoundingMethods.ROUND_TO_ZERO
 ROUND_UP = _RoundingMethods.ROUND_UP
 
 from ._constants import ROUNDING_METHODS
 
 # CONFIGURATION
 from ._config import BaseConfig
+from ._config import Config
 from ._config import DigitsConfig
 from ._config import DisplayConfig
-from ._config import RangeConfig
+from ._config import StringConfig
 from ._config import StripConfig
 from ._config import ValueConfig
 
 # EXCEPTIONS
 from ._errors import RangeError
 
 # SIZE
```

### Comparing `justbytes-0.8/src/justbytes/_errors.py` & `justbytes-0.9/src/justbytes/_errors.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/src/justbytes/_config.py` & `justbytes-0.9/src/justbytes/_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -173,47 +173,78 @@
            'rounding_method' : self.rounding_method,
            'unit' : self.unit
         }
         return "ValueConfig(%s)" % (self._FMT_STR % values)
     __repr__ = __str__
 
 
-class RangeConfig(object):
+class StringConfig(object):
     """ Configuration for :class:`Range` class. """
+    # pylint: disable=too-few-public-methods
 
-    DISPLAY_CONFIG = DisplayConfig()
+    def __init__(self, value_config, display_config, display_impl):
+        """
+        Initializer.
+
+        :param ValueConfig value_config: the value configuration
+        :param DisplayConfig display_config: the display configuration
+        :param type display_impl: display implementation class
+        :raises RangeValueError: if configuration and implementation can't work
+        """
+        try:
+            self.DISPLAY_IMPL = display_impl(display_config, value_config.base)
+        except justbases.BasesError as err:
+            raise RangeValueError(display_config, "display_config", str(err))
+
+        self.DISPLAY_IMPL_CLASS = display_impl
+        self.VALUE_CONFIG = value_config
+        self.DISPLAY_CONFIG = display_config
+
+
+class Config(object):
+    """
+    The super top-level configuration class for ranges.
+    """
 
-    VALUE_CONFIG = ValueConfig()
-    """ Default configuration for string display. """
+    STRING_CONFIG = \
+       StringConfig(ValueConfig(), DisplayConfig(), justbases.String)
 
     STRICT = False
 
     @classmethod
+    def set_display_impl(cls, impl): # pragma: no cover
+        """
+        Set display implementation.
+
+        :param type impl: the display implementation class
+        """
+        cls.STRING_CONFIG = StringConfig(
+           cls.STRING_CONFIG.VALUE_CONFIG,
+           cls.STRING_CONFIG.DISPLAY_CONFIG,
+           impl
+        )
+
+    @classmethod
     def set_display_config(cls, config):
         """
         Set configuration for superficial aspects of display.
 
         :param DisplayConfig config: a configuration object
         """
-        cls.DISPLAY_CONFIG = DisplayConfig(
-            show_approx_str=config.show_approx_str,
-            base_config=config.base_config,
-            digits_config=config.digits_config,
-            strip_config=config.strip_config
+        cls.STRING_CONFIG = StringConfig(
+           cls.STRING_CONFIG.VALUE_CONFIG,
+           config,
+           cls.STRING_CONFIG.DISPLAY_IMPL_CLASS
         )
 
     @classmethod
     def set_value_config(cls, config):
         """
         Set the configuration for computing the value of string representation.
 
         :param :class:`ValueConfig` config: a configuration object
         """
-        cls.VALUE_CONFIG = ValueConfig(
-            base=config.base,
-            binary_units=config.binary_units,
-            max_places=config.max_places,
-            min_value=config.min_value,
-            exact_value=config.exact_value,
-            rounding_method=config.rounding_method,
-            unit=config.unit
+        cls.STRING_CONFIG = StringConfig(
+           config,
+           cls.STRING_CONFIG.DISPLAY_CONFIG,
+           cls.STRING_CONFIG.DISPLAY_IMPL_CLASS
         )
```

### Comparing `justbytes-0.8/src/justbytes/_util/generators.py` & `justbytes-0.9/src/justbytes/_util/generators.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/src/justbytes/_size.py` & `justbytes-0.9/src/justbytes/_size.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from fractions import Fraction
 
 import six
 
 import justbases
 
-from ._config import RangeConfig
+from ._config import Config
 
 from ._errors import RangeFractionalResultError
 from ._errors import RangeNonsensicalBinOpError
 from ._errors import RangeNonsensicalBinOpValueError
 from ._errors import RangePowerResultError
 from ._errors import RangeValueError
 
@@ -123,15 +123,15 @@
                    "units",
                    "meaningless when Range value is passed"
                 )
             magnitude = value.magnitude # pylint: disable=no-member
         else:
             raise RangeValueError(value, "value")
 
-        if RangeConfig.STRICT is True and magnitude.denominator != 1:
+        if Config.STRICT is True and magnitude.denominator != 1:
             raise RangeFractionalResultError()
         self._magnitude = magnitude
 
     @property
     def magnitude(self):
         """
         :returns: the number of bytes
@@ -147,33 +147,29 @@
         :returns: a tuple representing the number to display
         :rtype: tuple of Radix * int * unit
         """
         (magnitude, units) = self.components(config)
         (result, relation) = self._as_single_number(magnitude, config)
         return (result, relation, units)
 
-    def getString(self, config, display):
+    def getString(self, config):
         """
         Return a string representation of the size.
 
-        :param ValueConfig config: representation configuration
-        :param DisplayConfig display: configuration for display
+        :param StringConfig config: the configuration
         :returns: a string representation
         :rtype: str
-        :raises: RangeValueError
+        :raises RangeValueError: if configuration is not satisfiable
         """
-        (result, relation, units) = self.getStringInfo(config)
-        number = result.getString(display, relation)
+        (result, relation, units) = self.getStringInfo(config.VALUE_CONFIG)
+        number = config.DISPLAY_IMPL.xform(result, relation)
         return "%s %s" % (number, units.abbr + self._BYTES_SYMBOL)
 
     def __str__(self):
-        return self.getString(
-           RangeConfig.VALUE_CONFIG,
-           RangeConfig.DISPLAY_CONFIG
-        )
+        return self.getString(Config.STRING_CONFIG)
 
     def __repr__(self):
         """
         Displaying value to arbitrary precision could be time consuming.
 
         Instead, explicitly round to nearest integer, and display relation.
 
@@ -430,15 +426,15 @@
             :param bool binary_units: binary units if True, else SI
         """
         units = BinaryUnits if binary_units else DecimalUnits
 
         for unit in [B] + units.UNITS():
             yield (self.convertTo(unit), unit)
 
-    def components(self, config=RangeConfig.VALUE_CONFIG):
+    def components(self, config=Config.STRING_CONFIG.VALUE_CONFIG):
         """ Return a representation of this size, decomposed into a
             Fraction value and a unit specifier tuple.
 
             :param ValueConfig config: configuration
 
             :returns: a pair of a decimal value and a unit
             :rtype: tuple of Fraction and unit
```

### Comparing `justbytes-0.8/src/justbytes/_constants.py` & `justbytes-0.9/src/justbytes/_constants.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/src/justbytes/_sizes.py` & `justbytes-0.9/src/justbytes/_sizes.py`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/src/justbytes.egg-info/PKG-INFO` & `justbytes-0.9/src/justbytes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: justbytes
-Version: 0.8
+Version: 0.9
 Summary: computing with and displaying bytes
 Home-page: http://pythonhosted.org/justbytes/
 Author: Anne Mulhern
 Author-email: amulhern@redhat.com
 License: GPL 2+
 Description: .. image:: https://secure.travis-ci.org/mulkieran/justbytes.png?branch=master
            :target: http://travis-ci.org/mulkieran/justbytes
```

### Comparing `justbytes-0.8/src/justbytes.egg-info/SOURCES.txt` & `justbytes-0.9/src/justbytes.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -77,15 +77,14 @@
 doc/_build/html/search.html
 doc/_build/html/tutorial.html
 doc/_build/html/justbytes/justbytes._config.html
 doc/_build/html/justbytes/justbytes._constants.html
 doc/_build/html/justbytes/justbytes._errors.html
 doc/_build/html/justbytes/justbytes._size.html
 doc/_build/html/justbytes/justbytes._sizes.html
-doc/_build/html/justbytes/justbytes._util.display.html
 doc/_build/html/justbytes/justbytes._util.generators.html
 doc/_build/html/justbytes/justbytes._util.html
 doc/_build/html/justbytes/justbytes.html
 doc/_build/html/justbytes/justbytes.version.html
 doc/_build/html/justbytes/modules.html
 doc/_build/html/tests/modules.html
 doc/_build/html/tests/tests.config_test.html
@@ -102,15 +101,14 @@
 doc/_build/html/tests/tests.utils.html
 doc/_build/html/tests/tests.version_test.html
 doc/justbytes/justbytes._config.rst
 doc/justbytes/justbytes._constants.rst
 doc/justbytes/justbytes._errors.rst
 doc/justbytes/justbytes._size.rst
 doc/justbytes/justbytes._sizes.rst
-doc/justbytes/justbytes._util.display.rst
 doc/justbytes/justbytes._util.generators.rst
 doc/justbytes/justbytes._util.rst
 doc/justbytes/justbytes.rst
 doc/justbytes/justbytes.version.rst
 doc/justbytes/modules.rst
 doc/tests/modules.rst
 doc/tests/tests.config_test.rst
```

### Comparing `justbytes-0.8/tox.ini` & `justbytes-0.9/tox.ini`

 * *Files 19% similar despite different names*

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

### Comparing `justbytes-0.8/setup.py` & `justbytes-0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,13 +52,13 @@
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
         'Topic :: Software Development :: Libraries',
         'Topic :: System :: Hardware',
         'Topic :: System :: Operating System Kernels :: Linux',
     ],
     install_requires = [
-        'justbases>0.06',
+        'justbases>0.07',
         'six'
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages("src"),
     )
```

### Comparing `justbytes-0.8/doc/_build/html/index.html` & `justbytes-0.9/doc/_build/html/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Welcome to justbytes’s documentation! &mdash; justbytes 0.07 documentation</title>
+    <title>Welcome to justbytes’s documentation! &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="#" />
+    <link rel="top" title="justbytes 0.08 documentation" href="#" />
     <link rel="next" title="Justbytes" href="intro.html" /> 
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
           <a href="intro.html" title="Justbytes"
              accesskey="N">next</a> |</li>
-        <li><a href="#">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="#">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -58,15 +58,15 @@
 <li class="toctree-l2"><a class="reference internal" href="intro.html#operations">Operations</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#floating-point-numbers">Floating Point Numbers</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#computing-the-representation-of-a-range">Computing the Representation of a Range</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#displaying-ranges">Displaying Ranges</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#representing-units">Representing Units</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#constructing-ranges-programatically">Constructing Ranges Programatically</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#errors">Errors</a></li>
-<li class="toctree-l2"><a class="reference internal" href="intro.html#measures-of-bandwidth-vs-address-ranges">Measures of Bandwidth vs. Address Ranges</a></li>
+<li class="toctree-l2"><a class="reference internal" href="intro.html#memory-consumption-and-bandwidth-vs-address-ranges">Memory Consumption and Bandwidth vs. Address Ranges</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#user-input">User Input</a></li>
 <li class="toctree-l2"><a class="reference internal" href="intro.html#alternative-packages">Alternative Packages</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="tutorial.html">Tutorial</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="tutorial.html#creating">Creating</a></li>
 <li class="toctree-l2"><a class="reference internal" href="tutorial.html#displaying">Displaying</a></li>
@@ -140,15 +140,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbytes"
              >next</a> |</li>
-        <li><a href="#">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="#">justbytes 0.08 documentation</a> &raquo;</li> 
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
@@ -1,27 +1,27 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** Welcome to justbytes’s documentation!¶ ******
 Contents:
     * Justbytes
           o Practical_Computing_with_Address_Ranges
           o Operations
           o Floating_Point_Numbers
           o Computing_the_Representation_of_a_Range
           o Displaying_Ranges
           o Representing_Units
           o Constructing_Ranges_Programatically
           o Errors
-          o Measures_of_Bandwidth_vs._Address_Ranges
+          o Memory_Consumption_and_Bandwidth_vs._Address_Ranges
           o User_Input
           o Alternative_Packages
     * Tutorial
           o Creating
           o Displaying
           o Arithmetic
           o Miscellaneous_Examples
@@ -44,9 +44,9 @@
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/search.html` & `justbytes-0.9/doc/_build/html/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,33 +2,33 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Search &mdash; justbytes 0.07 documentation</title>
+    <title>Search &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="_static/searchtools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="index.html" />
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
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/modules.html` & `justbytes-0.9/doc/_build/html/tests/modules.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests &mdash; justbytes 0.07 documentation</title>
+    <title>tests &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="next" title="tests package" href="tests.html" />
     <link rel="prev" title="justbytes.version module" href="../justbytes/justbytes.version.html" /> 
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
           <a href="../justbytes/justbytes.version.html" title="justbytes.version module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -126,15 +126,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.html" title="tests package"
              >next</a> |</li>
         <li class="right" >
           <a href="../justbytes/justbytes.version.html" title="justbytes.version module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** tests¶ ******
     * tests_package
           o Subpackages
                 # tests.size_package
                       # Submodules
                       # Module_contents
           o Submodules
@@ -32,9 +32,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.config_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.config_test.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.config_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.config_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.constants_test module" href="tests.constants_test.html" />
     <link rel="prev" title="tests.size.size_test module" href="tests.size.size_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.constants_test.html" title="tests.constants_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.size_test.html" title="tests.size.size_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -153,15 +153,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.constants_test.html" title="tests.constants_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.size_test.html" title="tests.size.size_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.config_test module¶ ******
 Test for configuration classes.
   classtests.config_test.ConfigTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Exercise methods of output configuration classes.
@@ -39,11 +39,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.utils.html` & `justbytes-0.9/doc/_build/html/tests/tests.utils.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.utils module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.utils module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.version_test module" href="tests.version_test.html" />
     <link rel="prev" title="tests.util_test module" href="tests.util_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.version_test.html" title="tests.version_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.util_test.html" title="tests.util_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -105,15 +105,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.version_test.html" title="tests.version_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.util_test.html" title="tests.util_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.utils module¶ ******
 Utilities for testing.
 *** Previous topic ***
 tests.util_test_module
 *** Next topic ***
@@ -23,11 +23,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.constants_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.constants_test.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.constants_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.constants_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.errors_test module" href="tests.errors_test.html" />
     <link rel="prev" title="tests.config_test module" href="tests.config_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.errors_test.html" title="tests.errors_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.config_test.html" title="tests.config_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -130,15 +130,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.errors_test.html" title="tests.errors_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.config_test.html" title="tests.config_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.constants_test module¶ ******
 Test for constants classes.
   classtests.constants_test.ConstantsTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Exercise methods of constants classes.
@@ -32,11 +32,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.operations_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.operations_test.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size.operations_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size.operations_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests.size package" href="tests.size.html" />
     <link rel="next" title="tests.size.size_test module" href="tests.size.size_test.html" />
     <link rel="prev" title="tests.size.named_test module" href="tests.size.named_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.size_test.html" title="tests.size.size_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.named_test.html" title="tests.size.named_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" accesskey="U">tests.size package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -445,15 +445,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.size_test.html" title="tests.size.size_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.named_test.html" title="tests.size.named_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" >tests.size package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 ****** tests.size.operations_test module¶ ******
 Tests for operations on Range objects.
   classtests.size.operations_test.AdditionTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
@@ -148,12 +148,12 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.errors_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.errors_test.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.errors_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.errors_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.util_test module" href="tests.util_test.html" />
     <link rel="prev" title="tests.constants_test module" href="tests.constants_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.util_test.html" title="tests.util_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.constants_test.html" title="tests.constants_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -142,15 +142,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.util_test.html" title="tests.util_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.constants_test.html" title="tests.constants_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.errors_test module¶ ******
 Test for error classes.
   classtests.errors_test.ErrorTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Exercise methods of error classes.
@@ -36,11 +36,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.initializer_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.initializer_test.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size.initializer_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size.initializer_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests.size package" href="tests.size.html" />
     <link rel="next" title="tests.size.named_test module" href="tests.size.named_test.html" />
     <link rel="prev" title="tests.size.conversions_test module" href="tests.size.conversions_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.named_test.html" title="tests.size.named_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.conversions_test.html" title="tests.size.conversions_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" accesskey="U">tests.size package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -125,15 +125,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.named_test.html" title="tests.size.named_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.conversions_test.html" title="tests.size.conversions_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" >tests.size package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 ****** tests.size.initializer_test module¶ ******
 Tests for Range initialization.
   classtests.size.initializer_test.InitializerTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
@@ -31,12 +31,12 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.util_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.util_test.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.util_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.util_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.utils module" href="tests.utils.html" />
     <link rel="prev" title="tests.errors_test module" href="tests.errors_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.utils.html" title="tests.utils module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.errors_test.html" title="tests.errors_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -143,15 +143,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.utils.html" title="tests.utils module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.errors_test.html" title="tests.errors_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.util_test module¶ ******
 Test for utility functions.
   classtests.util_test.NextTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Test next_or_last.
@@ -37,11 +37,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.named_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.named_test.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size.named_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size.named_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests.size package" href="tests.size.html" />
     <link rel="next" title="tests.size.operations_test module" href="tests.size.operations_test.html" />
     <link rel="prev" title="tests.size.initializer_test module" href="tests.size.initializer_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.operations_test.html" title="tests.size.operations_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.initializer_test.html" title="tests.size.initializer_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" accesskey="U">tests.size package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -196,15 +196,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.operations_test.html" title="tests.size.operations_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.initializer_test.html" title="tests.size.initializer_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" >tests.size package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 ****** tests.size.named_test module¶ ******
 Tests for named methods of Range objects.
   classtests.size.named_test.ComponentsTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
@@ -58,12 +58,12 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size package &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size package &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="next" title="tests.size.conversions_test module" href="tests.size.conversions_test.html" />
     <link rel="prev" title="tests package" href="tests.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.conversions_test.html" title="tests.size.conversions_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.html" title="tests package"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -129,15 +129,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.conversions_test.html" title="tests.size.conversions_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.html" title="tests package"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.size package¶ ******
 ***** Submodules¶ *****
     * tests.size.conversions_test_module
     * tests.size.initializer_test_module
     * tests.size.named_test_module
@@ -34,11 +34,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.version_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.version_test.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.version_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.version_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests package" href="tests.html" />
     <link rel="prev" title="tests.utils module" href="tests.utils.html" /> 
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
           <a href="tests.utils.html" title="tests.utils module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" accesskey="U">tests package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -108,15 +108,15 @@
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.utils.html" title="tests.utils module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 ****** tests.version_test module¶ ******
 Test for version information.
   classtests.version_test.VersionTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
       Test version.
@@ -23,11 +23,11 @@
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.html` & `justbytes-0.9/doc/_build/html/tests/tests.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests package &mdash; justbytes 0.07 documentation</title>
+    <title>tests package &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests" href="modules.html" />
     <link rel="next" title="tests.size package" href="tests.size.html" />
     <link rel="prev" title="tests" href="modules.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.html" title="tests.size package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="modules.html" title="tests"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" accesskey="U">tests</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -149,15 +149,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.html" title="tests.size package"
              >next</a> |</li>
         <li class="right" >
           <a href="modules.html" title="tests"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
 ****** tests package¶ ******
 ***** Subpackages¶ *****
     * tests.size_package
           o Submodules
                 # tests.size.conversions_test_module
                 # tests.size.initializer_test_module
@@ -44,10 +44,10 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.conversions_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.conversions_test.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size.conversions_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size.conversions_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests.size package" href="tests.size.html" />
     <link rel="next" title="tests.size.initializer_test module" href="tests.size.initializer_test.html" />
     <link rel="prev" title="tests.size package" href="tests.size.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.initializer_test.html" title="tests.size.initializer_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.html" title="tests.size package"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" accesskey="U">tests.size package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -145,15 +145,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.size.initializer_test.html" title="tests.size.initializer_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.html" title="tests.size package"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" >tests.size package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 ****** tests.size.conversions_test module¶ ******
 Tests for operations on Range objects.
   classtests.size.conversions_test.ConversionTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
@@ -40,12 +40,12 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tests/tests.size.size_test.html` & `justbytes-0.9/doc/_build/html/tests/tests.size.size_test.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>tests.size.size_test module &mdash; justbytes 0.07 documentation</title>
+    <title>tests.size.size_test module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="tests.size package" href="tests.size.html" />
     <link rel="next" title="tests.config_test module" href="tests.config_test.html" />
     <link rel="prev" title="tests.size.operations_test module" href="tests.size.operations_test.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.config_test.html" title="tests.config_test module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tests.size.operations_test.html" title="tests.size.operations_test module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" accesskey="U">tests.size package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -236,15 +236,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tests.config_test.html" title="tests.config_test module"
              >next</a> |</li>
         <li class="right" >
           <a href="tests.size.operations_test.html" title="tests.size.operations_test module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >tests</a> &raquo;</li>
           <li><a href="tests.html" >tests package</a> &raquo;</li>
           <li><a href="tests.size.html" >tests.size package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 ****** tests.size.size_test module¶ ******
 Tests for behavior of Range objects.
   classtests.size.size_test.ComputationTestCase(methodName='runTest')¶
       Bases: unittest.case.TestCase
@@ -70,12 +70,12 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * tests »
     * tests_package »
     * tests.size_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/tutorial.html` & `justbytes-0.9/doc/_build/html/tutorial.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Tutorial &mdash; justbytes 0.07 documentation</title>
+    <title>Tutorial &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="index.html" />
     <link rel="next" title="justbytes" href="justbytes/modules.html" />
     <link rel="prev" title="Justbytes" href="intro.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes/modules.html" title="justbytes"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbytes"
              accesskey="P">previous</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -238,15 +238,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes/modules.html" title="justbytes"
              >next</a> |</li>
         <li class="right" >
           <a href="intro.html" title="Justbytes"
              >previous</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** Tutorial¶ ******
 ***** Creating¶ *****
 Import everything:
 >>> from justbytes import *
 Create a Range object from a numeric value and a unit specification:
 >>> size = Range(8, GiB)
 ***** Displaying¶ *****
@@ -104,9 +104,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._errors.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._errors.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._errors module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._errors module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="justbytes._size module" href="justbytes._size.html" />
     <link rel="prev" title="justbytes._constants module" href="justbytes._constants.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._size.html" title="justbytes._size module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes._constants.html" title="justbytes._constants module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -170,15 +170,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._size.html" title="justbytes._size module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes._constants.html" title="justbytes._constants module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._errors module¶ ******
 Exception types used by the justbytes class.
   exceptionjustbytes._errors.RangeError¶
       Bases: exceptions.Exception
       Generic Range error.
@@ -52,11 +52,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/modules.html` & `justbytes-0.9/doc/_build/html/justbytes/modules.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="next" title="justbytes package" href="justbytes.html" />
     <link rel="prev" title="Tutorial" href="../tutorial.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes.html" title="justbytes package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="../tutorial.html" title="Tutorial"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -129,15 +129,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes.html" title="justbytes package"
              >next</a> |</li>
         <li class="right" >
           <a href="../tutorial.html" title="Tutorial"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** justbytes¶ ******
     * justbytes_package
           o Subpackages
                 # justbytes._util_package
                       # Submodules
                       # Module_contents
           o Submodules
@@ -33,9 +33,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._size.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._size.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._size module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._size module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="justbytes._sizes module" href="justbytes._sizes.html" />
     <link rel="prev" title="justbytes._errors module" href="justbytes._errors.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._sizes.html" title="justbytes._sizes module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes._errors.html" title="justbytes._errors module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -272,15 +272,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._sizes.html" title="justbytes._sizes module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes._errors.html" title="justbytes._errors module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._size module¶ ******
 Range class, for creating instances of Range objects.
 Contains a few documented methods and a number of __*__ methods implementing
 arithmetic operations. Precise numeric types such as int and Decimal may also
 occur in some arithmetic expressions, but all occurrances of floating point
@@ -89,11 +89,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._util.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._util.html`

 * *Files 14% similar despite different names*

```diff
@@ -2,53 +2,53 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._util package &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._util package &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
-    <link rel="next" title="justbytes._util.display module" href="justbytes._util.display.html" />
+    <link rel="next" title="justbytes._util.generators module" href="justbytes._util.generators.html" />
     <link rel="prev" title="justbytes package" href="justbytes.html" /> 
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
-          <a href="justbytes._util.display.html" title="justbytes._util.display module"
+          <a href="justbytes._util.generators.html" title="justbytes._util.generators module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes.html" title="justbytes package"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -57,15 +57,14 @@
             
   <div class="section" id="justbytes-util-package">
 <h1>justbytes._util package<a class="headerlink" href="#justbytes-util-package" title="Permalink to this headline">¶</a></h1>
 <div class="section" id="submodules">
 <h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this headline">¶</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
-<li class="toctree-l1"><a class="reference internal" href="justbytes._util.display.html">justbytes._util.display module</a></li>
 <li class="toctree-l1"><a class="reference internal" href="justbytes._util.generators.html">justbytes._util.generators module</a></li>
 </ul>
 </div>
 </div>
 <div class="section" id="module-justbytes._util">
 <span id="module-contents"></span><h2>Module contents<a class="headerlink" href="#module-justbytes._util" title="Permalink to this headline">¶</a></h2>
 </div>
@@ -86,16 +85,16 @@
 </li>
 </ul>
 
   <h4>Previous topic</h4>
   <p class="topless"><a href="justbytes.html"
                         title="previous chapter">justbytes package</a></p>
   <h4>Next topic</h4>
-  <p class="topless"><a href="justbytes._util.display.html"
-                        title="next chapter">justbytes._util.display module</a></p>
+  <p class="topless"><a href="justbytes._util.generators.html"
+                        title="next chapter">justbytes._util.generators module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/justbytes/justbytes._util.txt"
            rel="nofollow">Show Source</a></li>
   </ul>
 <div id="searchbox" style="display: none">
   <h3>Quick search</h3>
@@ -120,20 +119,20 @@
         <li class="right" style="margin-right: 10px">
           <a href="../genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
-          <a href="justbytes._util.display.html" title="justbytes._util.display module"
+          <a href="justbytes._util.generators.html" title="justbytes._util.generators module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes.html" title="justbytes package"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,37 +4,36 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._util package¶ ******
 ***** Submodules¶ *****
-    * justbytes._util.display_module
     * justbytes._util.generators_module
 ***** Module contents¶ *****
 **** Table_Of_Contents ****
     * justbytes._util_package
           o Submodules
           o Module_contents
 *** Previous topic ***
 justbytes_package
 *** Next topic ***
-justbytes._util.display_module
+justbytes._util.generators_module
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes package &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes package &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes" href="modules.html" />
     <link rel="next" title="justbytes._util package" href="justbytes._util.html" />
     <link rel="prev" title="justbytes" href="modules.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._util.html" title="justbytes._util package"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="modules.html" title="justbytes"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" accesskey="U">justbytes</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -58,15 +58,14 @@
 <h1>justbytes package<a class="headerlink" href="#justbytes-package" title="Permalink to this headline">¶</a></h1>
 <div class="section" id="subpackages">
 <h2>Subpackages<a class="headerlink" href="#subpackages" title="Permalink to this headline">¶</a></h2>
 <div class="toctree-wrapper compound">
 <ul>
 <li class="toctree-l1"><a class="reference internal" href="justbytes._util.html">justbytes._util package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="justbytes._util.html#submodules">Submodules</a><ul>
-<li class="toctree-l3"><a class="reference internal" href="justbytes._util.display.html">justbytes._util.display module</a></li>
 <li class="toctree-l3"><a class="reference internal" href="justbytes._util.generators.html">justbytes._util.generators module</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="justbytes._util.html#module-justbytes._util">Module contents</a></li>
 </ul>
 </li>
 </ul>
@@ -249,15 +248,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._util.html" title="justbytes._util package"
              >next</a> |</li>
         <li class="right" >
           <a href="modules.html" title="justbytes"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
     </div>
```

#### html2text {}

```diff
@@ -4,21 +4,20 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
 ****** justbytes package¶ ******
 ***** Subpackages¶ *****
     * justbytes._util_package
           o Submodules
-                # justbytes._util.display_module
                 # justbytes._util.generators_module
           o Module_contents
 ***** Submodules¶ *****
     * justbytes._config_module
     * justbytes._constants_module
     * justbytes._errors_module
     * justbytes._size_module
@@ -89,10 +88,10 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._constants.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._constants.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._constants module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._constants module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="justbytes._errors module" href="justbytes._errors.html" />
     <link rel="prev" title="justbytes._config module" href="justbytes._config.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._errors.html" title="justbytes._errors module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes._config.html" title="justbytes._config module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -266,15 +266,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._errors.html" title="justbytes._errors module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes._config.html" title="justbytes._config module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._constants module¶ ******
 Constants used by the justbytes package.
   Categories of constants:
           * Rounding methods
           * Size units, e.g., Ki, Mi
@@ -67,11 +67,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._config.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._config.html`

 * *Files 12% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._config module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._config module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="justbytes._constants module" href="justbytes._constants.html" />
     <link rel="prev" title="justbytes._util.generators module" href="justbytes._util.generators.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,50 +40,51 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._constants.html" title="justbytes._constants module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes._util.generators.html" title="justbytes._util.generators module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
             
   <div class="section" id="module-justbytes._config">
 <span id="justbytes-config-module"></span><h1>justbytes._config module<a class="headerlink" href="#module-justbytes._config" title="Permalink to this headline">¶</a></h1>
 <p>Configuration of the justbytes package.</p>
 <dl class="class">
-<dt id="justbytes._config.DigitsConfig">
-<em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">DigitsConfig</tt><big>(</big><em>separator='~'</em>, <em>use_caps=False</em>, <em>use_letters=True</em><big>)</big><a class="headerlink" href="#justbytes._config.DigitsConfig" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
-<p>How to display digits.</p>
+<dt id="justbytes._config.BaseConfig">
+<em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">BaseConfig</tt><big>(</big><em>use_prefix=False</em>, <em>use_subscript=False</em><big>)</big><a class="headerlink" href="#justbytes._config.BaseConfig" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <tt class="xref py py-class docutils literal"><span class="pre">justbases._config.BaseConfig</span></tt></p>
+<p>Configuration for display of bases.</p>
+<p>Override defaults of justbases.BaseConfig.</p>
 </dd></dl>
 
 <dl class="class">
 <dt id="justbytes._config.DisplayConfig">
-<em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">DisplayConfig</tt><big>(</big><em>show_approx_str=True</em>, <em>show_base=False</em>, <em>digits_config=DigitsConfig(separator=~</em>, <em>use_caps=False</em>, <em>use_letters=True)</em>, <em>strip_config=StripConfig(strip=False</em>, <em>strip_exact=False</em>, <em>strip_whole=True)</em><big>)</big><a class="headerlink" href="#justbytes._config.DisplayConfig" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
-<p>Superficial aspects of display.</p>
+<em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">DisplayConfig</tt><big>(</big><em>show_approx_str=True</em>, <em>base_config=BaseConfig(use_prefix=False</em>, <em>use_subscript=False)</em>, <em>digits_config=DigitsConfig(separator=~</em>, <em>use_caps=False</em>, <em>use_letters=True)</em>, <em>strip_config=StripConfig(strip=False</em>, <em>strip_exact=False</em>, <em>strip_whole=True)</em><big>)</big><a class="headerlink" href="#justbytes._config.DisplayConfig" title="Permalink to this definition">¶</a></dt>
+<dd><p>Bases: <tt class="xref py py-class docutils literal"><span class="pre">justbases._config.DisplayConfig</span></tt></p>
+<p>DisplayConfig overrides justbases.DisplayConfig&#8217;s defaults.</p>
 </dd></dl>
 
 <dl class="class">
 <dt id="justbytes._config.RangeConfig">
 <em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">RangeConfig</tt><a class="headerlink" href="#justbytes._config.RangeConfig" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
 <p>Configuration for <tt class="xref py py-class docutils literal"><span class="pre">Range</span></tt> class.</p>
 <dl class="attribute">
 <dt id="justbytes._config.RangeConfig.DISPLAY_CONFIG">
-<tt class="descname">DISPLAY_CONFIG</tt><em class="property"> = DisplayConfig(show_approx_str=True, show_base=False, digits_config=DigitsConfig(separator=~, use_caps=False, use_letters=True), strip_config-StripConfig(strip=False, strip_exact=False, strip_whole=True))</em><a class="headerlink" href="#justbytes._config.RangeConfig.DISPLAY_CONFIG" title="Permalink to this definition">¶</a></dt>
+<tt class="descname">DISPLAY_CONFIG</tt><em class="property"> = DisplayConfig(show_approx_str=True, base_config=BaseConfig(use_prefix=False, use_subscript=False), digits_config=DigitsConfig(separator=~, use_caps=False, use_letters=True), strip_config-StripConfig(strip=False, strip_exact=False, strip_whole=True))</em><a class="headerlink" href="#justbytes._config.RangeConfig.DISPLAY_CONFIG" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="attribute">
 <dt id="justbytes._config.RangeConfig.STRICT">
 <tt class="descname">STRICT</tt><em class="property"> = False</em><a class="headerlink" href="#justbytes._config.RangeConfig.STRICT" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
@@ -113,21 +114,14 @@
 <dd><p>Set the configuration for computing the value of string representation.</p>
 <p>:param <a class="reference internal" href="#justbytes._config.ValueConfig" title="justbytes._config.ValueConfig"><tt class="xref py py-class docutils literal"><span class="pre">ValueConfig</span></tt></a> config: a configuration object</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="class">
-<dt id="justbytes._config.StripConfig">
-<em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">StripConfig</tt><big>(</big><em>strip=False</em>, <em>strip_exact=False</em>, <em>strip_whole=True</em><big>)</big><a class="headerlink" href="#justbytes._config.StripConfig" title="Permalink to this definition">¶</a></dt>
-<dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
-<p>Stripping trailing zeros.</p>
-</dd></dl>
-
-<dl class="class">
 <dt id="justbytes._config.ValueConfig">
 <em class="property">class </em><tt class="descclassname">justbytes._config.</tt><tt class="descname">ValueConfig</tt><big>(</big><em>max_places=2</em>, <em>min_value=1</em>, <em>binary_units=True</em>, <em>exact_value=False</em>, <em>unit=None</em>, <em>base=10</em>, <em>rounding_method=_RoundingMethod(Round to nearest</em>, <em>to zero on a tie.)</em><big>)</big><a class="headerlink" href="#justbytes._config.ValueConfig" title="Permalink to this definition">¶</a></dt>
 <dd><p>Bases: <a class="reference external" href="http://docs.python.org/library/functions.html#object" title="(in Python v2.7)"><tt class="xref py py-class docutils literal"><span class="pre">object</span></tt></a></p>
 <p>Configuration for __str__ method.</p>
 <p>If max_places is set to None, all non-zero digits after the
 decimal point will be shown.  Otherwise, max_places digits will
 be shown.</p>
@@ -187,15 +181,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._constants.html" title="justbytes._constants module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes._util.generators.html" title="justbytes._util.generators module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.2.3.
```

#### html2text {}

```diff
@@ -4,32 +4,34 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._config module¶ ******
 Configuration of the justbytes package.
-  classjustbytes._config.DigitsConfig(separator='~', use_caps=False,
-  use_letters=True)¶
-      Bases: object
-      How to display digits.
-  classjustbytes._config.DisplayConfig(show_approx_str=True, show_base=False,
+  classjustbytes._config.BaseConfig(use_prefix=False, use_subscript=False)¶
+      Bases: justbases._config.BaseConfig
+      Configuration for display of bases.
+      Override defaults of justbases.BaseConfig.
+  classjustbytes._config.DisplayConfig(show_approx_str=True,
+  base_config=BaseConfig(use_prefix=False, use_subscript=False),
   digits_config=DigitsConfig(separator=~, use_caps=False, use_letters=True),
   strip_config=StripConfig(strip=False, strip_exact=False, strip_whole=True))¶
-      Bases: object
-      Superficial aspects of display.
+      Bases: justbases._config.DisplayConfig
+      DisplayConfig overrides justbases.DisplayConfig’s defaults.
   classjustbytes._config.RangeConfig¶
       Bases: object
       Configuration for Range class.
-        DISPLAY_CONFIG= DisplayConfig(show_approx_str=True, show_base=False,
+        DISPLAY_CONFIG= DisplayConfig(show_approx_str=True,
+        base_config=BaseConfig(use_prefix=False, use_subscript=False),
         digits_config=DigitsConfig(separator=~, use_caps=False,
         use_letters=True), strip_config-StripConfig(strip=False,
         strip_exact=False, strip_whole=True))¶
         STRICT= False¶
         VALUE_CONFIG= ValueConfig(base=10, binary_units=True,
         exact_value=False, max_places=2, min_value=1,
         rounding_method=_RoundingMethod, unit=None)¶
@@ -37,18 +39,14 @@
         classmethodset_display_config(config)¶
             Set configuration for superficial aspects of display.
             Parameters: config (DisplayConfig) – a configuration object
         classmethodset_value_config(config)¶
             Set the configuration for computing the value of string
             representation.
             :param ValueConfig config: a configuration object
-  classjustbytes._config.StripConfig(strip=False, strip_exact=False,
-  strip_whole=True)¶
-      Bases: object
-      Stripping trailing zeros.
   classjustbytes._config.ValueConfig(max_places=2, min_value=1,
   binary_units=True, exact_value=False, unit=None, base=10,
   rounding_method=_RoundingMethod(Round to nearest, to zero on a tie.))¶
       Bases: object
       Configuration for __str__ method.
       If max_places is set to None, all non-zero digits after the decimal point
       will be shown. Otherwise, max_places digits will be shown.
@@ -68,11 +66,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._sizes.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._sizes.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._sizes module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._sizes module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="justbytes.version module" href="justbytes.version.html" />
     <link rel="prev" title="justbytes._size module" href="justbytes._size.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
@@ -40,15 +40,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes.version.html" title="justbytes.version module"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="justbytes._size.html" title="justbytes._size module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -105,15 +105,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes.version.html" title="justbytes.version module"
              >next</a> |</li>
         <li class="right" >
           <a href="justbytes._size.html" title="justbytes._size module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes._sizes module¶ ******
 Class for methods that do not properly belong in the Range class.
 *** Previous topic ***
 justbytes._size_module
 *** Next topic ***
@@ -23,11 +23,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes._util.generators.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes._util.generators.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,35 +2,35 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes._util.generators module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes._util.generators module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes._util package" href="justbytes._util.html" />
     <link rel="next" title="justbytes._config module" href="justbytes._config.html" />
-    <link rel="prev" title="justbytes._util.display module" href="justbytes._util.display.html" /> 
+    <link rel="prev" title="justbytes._util package" href="justbytes._util.html" /> 
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
           <a href="justbytes._config.html" title="justbytes._config module"
              accesskey="N">next</a> |</li>
         <li class="right" >
-          <a href="justbytes._util.display.html" title="justbytes._util.display module"
+          <a href="justbytes._util.html" title="justbytes._util package"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li>
           <li><a href="justbytes._util.html" accesskey="U">justbytes._util package</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
@@ -103,16 +103,16 @@
 
           </div>
         </div>
       </div>
       <div class="sphinxsidebar">
         <div class="sphinxsidebarwrapper">
   <h4>Previous topic</h4>
-  <p class="topless"><a href="justbytes._util.display.html"
-                        title="previous chapter">justbytes._util.display module</a></p>
+  <p class="topless"><a href="justbytes._util.html"
+                        title="previous chapter">justbytes._util package</a></p>
   <h4>Next topic</h4>
   <p class="topless"><a href="justbytes._config.html"
                         title="next chapter">justbytes._config module</a></p>
   <h3>This Page</h3>
   <ul class="this-page-menu">
     <li><a href="../_sources/justbytes/justbytes._util.generators.txt"
            rel="nofollow">Show Source</a></li>
@@ -143,17 +143,17 @@
         <li class="right" >
           <a href="../py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="justbytes._config.html" title="justbytes._config module"
              >next</a> |</li>
         <li class="right" >
-          <a href="justbytes._util.display.html" title="justbytes._util.display module"
+          <a href="justbytes._util.html" title="justbytes._util package"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li>
           <li><a href="justbytes._util.html" >justbytes._util package</a> &raquo;</li> 
       </ul>
     </div>
     <div class="footer">
         &copy; Copyright 2015, mulhern.
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
     * justbytes._util_package »
 ****** justbytes._util.generators module¶ ******
 Special purpose generators.
   justbytes._util.generators.next_or_last(pred, seq, default=None)¶
       Return the first element that matches the predicate or the last element
@@ -24,25 +24,25 @@
                       * default – returned if seq is empty, default is None
   justbytes._util.generators.take_until_satisfied(pred, seq)¶
       Like next(), but yields all values until the first matching value.
                       * pred (bool) – a predicate, return False if the value is not
       Parameters:       satisfactory
                       * seq – a sequence of values
 *** Previous topic ***
-justbytes._util.display_module
+justbytes._util_package
 *** Next topic ***
 justbytes._config_module
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
     * justbytes._util_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/justbytes/justbytes.version.html` & `justbytes-0.9/doc/_build/html/justbytes/justbytes.version.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>justbytes.version module &mdash; justbytes 0.07 documentation</title>
+    <title>justbytes.version module &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="../_static/default.css" type="text/css" />
     <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    '../',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="../_static/jquery.js"></script>
     <script type="text/javascript" src="../_static/underscore.js"></script>
     <script type="text/javascript" src="../_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="../index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="../index.html" />
     <link rel="up" title="justbytes package" href="justbytes.html" />
     <link rel="next" title="tests" href="../tests/modules.html" />
     <link rel="prev" title="justbytes._sizes module" href="justbytes._sizes.html" /> 
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
           <a href="justbytes._sizes.html" title="justbytes._sizes module"
              accesskey="P">previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" accesskey="U">justbytes package</a> &raquo;</li> 
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
           <a href="justbytes._sizes.html" title="justbytes._sizes module"
              >previous</a> |</li>
-        <li><a href="../index.html">justbytes 0.07 documentation</a> &raquo;</li>
+        <li><a href="../index.html">justbytes 0.08 documentation</a> &raquo;</li>
           <li><a href="modules.html" >justbytes</a> &raquo;</li>
           <li><a href="justbytes.html" >justbytes package</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 ****** justbytes.version module¶ ******
 ***** justbytes.version¶ *****
 Version information.
 **** Table_Of_Contents ****
     * justbytes.version_module
@@ -27,11 +27,11 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
     * justbytes »
     * justbytes_package »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/py-modindex.html` & `justbytes-0.9/doc/_build/html/py-modindex.html`

 * *Files 3% similar despite different names*

```diff
@@ -2,47 +2,47 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Python Module Index &mdash; justbytes 0.07 documentation</title>
+    <title>Python Module Index &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="index.html" />
  
 
 
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
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -94,19 +94,14 @@
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
        <a href="justbytes/justbytes._util.html#module-justbytes._util"><tt class="xref">justbytes._util</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
-       <a href="justbytes/justbytes._util.display.html#module-justbytes._util.display"><tt class="xref">justbytes._util.display</tt></a></td><td>
-       <em></em></td></tr>
-     <tr class="cg-1">
-       <td></td>
-       <td>&nbsp;&nbsp;&nbsp;
        <a href="justbytes/justbytes._util.generators.html#module-justbytes._util.generators"><tt class="xref">justbytes._util.generators</tt></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&nbsp;&nbsp;&nbsp;
        <a href="justbytes/justbytes.version.html#module-justbytes.version"><tt class="xref">justbytes.version</tt></a></td><td>
        <em></em></td></tr>
@@ -209,15 +204,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
@@ -1,25 +1,24 @@
 
 
 **** Navigation ****
     * index
     * modules |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** Python Module Index ******
 j | t
      
     j
 [-] justbytes
         justbytes._config
         justbytes._constants
         justbytes._errors
         justbytes._size
         justbytes._sizes
         justbytes._util
-        justbytes._util.display
         justbytes._util.generators
         justbytes.version
      
     t
 [-] tests
         tests.config_test
         tests.constants_test
@@ -35,9 +34,9 @@
         tests.version_test
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/genindex.html` & `justbytes-0.9/doc/_build/html/genindex.html`

 * *Files 4% similar despite different names*

```diff
@@ -3,44 +3,44 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Index &mdash; justbytes 0.07 documentation</title>
+    <title>Index &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="index.html" /> 
+    <link rel="top" title="justbytes 0.08 documentation" href="index.html" /> 
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
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -63,15 +63,14 @@
  | <a href="#N"><strong>N</strong></a>
  | <a href="#P"><strong>P</strong></a>
  | <a href="#R"><strong>R</strong></a>
  | <a href="#S"><strong>S</strong></a>
  | <a href="#T"><strong>T</strong></a>
  | <a href="#U"><strong>U</strong></a>
  | <a href="#V"><strong>V</strong></a>
- | <a href="#X"><strong>X</strong></a>
  | <a href="#Y"><strong>Y</strong></a>
  | <a href="#Z"><strong>Z</strong></a>
  
 </div>
 <h2 id="A">A</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
@@ -95,14 +94,18 @@
 <h2 id="B">B</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._constants.html#justbytes._constants.B">B (in module justbytes._constants)</a>
   </dt>
 
+      
+  <dt><a href="justbytes/justbytes._config.html#justbytes._config.BaseConfig">BaseConfig (class in justbytes._config)</a>
+  </dt>
+
   </dl></td>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._constants.html#justbytes._constants.BinaryUnits">BinaryUnits (class in justbytes._constants)</a>
   </dt>
 
   </dl></td>
@@ -166,43 +169,27 @@
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._constants.html#justbytes._constants.DecimalUnits">DecimalUnits (class in justbytes._constants)</a>
   </dt>
 
       
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Decorators">Decorators (class in justbytes._util.display)</a>
-  </dt>
-
-      
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Decorators.decorators">decorators() (justbytes._util.display.Decorators class method)</a>
-  </dt>
-
-      
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Digits">Digits (class in justbytes._util.display)</a>
-  </dt>
-
-      
-  <dt><a href="justbytes/justbytes._config.html#justbytes._config.DigitsConfig">DigitsConfig (class in justbytes._config)</a>
-  </dt>
-
-      
   <dt><a href="tests/tests.size.named_test.html#tests.size.named_test.DigitsConfigTestCase">DigitsConfigTestCase (class in tests.size.named_test)</a>
   </dt>
 
-  </dl></td>
-  <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._config.html#justbytes._config.RangeConfig.DISPLAY_CONFIG">DISPLAY_CONFIG (justbytes._config.RangeConfig attribute)</a>
   </dt>
 
       
   <dt><a href="justbytes/justbytes._config.html#justbytes._config.DisplayConfig">DisplayConfig (class in justbytes._config)</a>
   </dt>
 
+  </dl></td>
+  <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="tests/tests.size.named_test.html#tests.size.named_test.DisplayConfigTestCase">DisplayConfigTestCase (class in tests.size.named_test)</a>
   </dt>
 
       
   <dt><a href="tests/tests.size.size_test.html#tests.size.size_test.DisplayTestCase">DisplayTestCase (class in tests.size.size_test)</a>
   </dt>
@@ -324,18 +311,14 @@
   </dt>
 
       
   <dt><a href="justbytes/justbytes._util.html#module-justbytes._util">justbytes._util (module)</a>
   </dt>
 
       
-  <dt><a href="justbytes/justbytes._util.display.html#module-justbytes._util.display">justbytes._util.display (module)</a>
-  </dt>
-
-      
   <dt><a href="justbytes/justbytes._util.generators.html#module-justbytes._util.generators">justbytes._util.generators (module)</a>
   </dt>
 
       
   <dt><a href="justbytes/justbytes.version.html#module-justbytes.version">justbytes.version (module)</a>
   </dt>
 
@@ -389,22 +372,18 @@
 <h2 id="N">N</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._util.generators.html#justbytes._util.generators.next_or_last">next_or_last() (in module justbytes._util.generators)</a>
   </dt>
 
-      
-  <dt><a href="tests/tests.util_test.html#tests.util_test.NextTestCase">NextTestCase (class in tests.util_test)</a>
-  </dt>
-
   </dl></td>
   <td style="width: 33%" valign="top"><dl>
       
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Number">Number (class in justbytes._util.display)</a>
+  <dt><a href="tests/tests.util_test.html#tests.util_test.NextTestCase">NextTestCase (class in tests.util_test)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
 <h2 id="P">P</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
@@ -480,18 +459,14 @@
   </dt>
 
       
   <dt><a href="tests/tests.size.operations_test.html#tests.size.operations_test.RdivmodTestCase">RdivmodTestCase (class in tests.size.operations_test)</a>
   </dt>
 
       
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Decorators.relation_to_symbol">relation_to_symbol() (justbytes._util.display.Decorators static method)</a>
-  </dt>
-
-      
   <dt><a href="tests/tests.size.operations_test.html#tests.size.operations_test.RfloordivTestCase">RfloordivTestCase (class in tests.size.operations_test)</a>
   </dt>
 
       
   <dt><a href="tests/tests.size.operations_test.html#tests.size.operations_test.RmodTestCase">RmodTestCase (class in tests.size.operations_test)</a>
   </dt>
 
@@ -535,30 +510,18 @@
   </dt>
 
         
   <dt><a href="tests/tests.size.size_test.html#tests.size.size_test.ConfigurationTestCase.setUp">(tests.size.size_test.ConfigurationTestCase method)</a>
   </dt>
 
       </dl></dd>
-      
-  <dt><a href="justbytes/justbytes._config.html#justbytes._config.RangeConfig.STRICT">STRICT (justbytes._config.RangeConfig attribute)</a>
-  </dt>
-
   </dl></td>
   <td style="width: 33%" valign="top"><dl>
       
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.String">String (class in justbytes._util.display)</a>
-  </dt>
-
-      
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Strip">Strip (class in justbytes._util.display)</a>
-  </dt>
-
-      
-  <dt><a href="justbytes/justbytes._config.html#justbytes._config.StripConfig">StripConfig (class in justbytes._config)</a>
+  <dt><a href="justbytes/justbytes._config.html#justbytes._config.RangeConfig.STRICT">STRICT (justbytes._config.RangeConfig attribute)</a>
   </dt>
 
       
   <dt><a href="tests/tests.size.operations_test.html#tests.size.operations_test.SubtractionTestCase">SubtractionTestCase (class in tests.size.operations_test)</a>
   </dt>
 
   </dl></td>
@@ -1062,38 +1025,14 @@
       
   <dt><a href="tests/tests.version_test.html#tests.version_test.VersionTestCase">VersionTestCase (class in tests.version_test)</a>
   </dt>
 
   </dl></td>
 </tr></table>
 
-<h2 id="X">X</h2>
-<table style="width: 100%" class="indextable genindextable"><tr>
-  <td style="width: 33%" valign="top"><dl>
-      
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Digits.xform">xform() (justbytes._util.display.Digits class method)</a>
-  </dt>
-
-      <dd><dl>
-        
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Number.xform">(justbytes._util.display.Number class method)</a>
-  </dt>
-
-        
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.String.xform">(justbytes._util.display.String class method)</a>
-  </dt>
-
-        
-  <dt><a href="justbytes/justbytes._util.display.html#justbytes._util.display.Strip.xform">(justbytes._util.display.Strip class method)</a>
-  </dt>
-
-      </dl></dd>
-  </dl></td>
-</tr></table>
-
 <h2 id="Y">Y</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%" valign="top"><dl>
       
   <dt><a href="justbytes/justbytes._constants.html#justbytes._constants.DecimalUnits.YB">YB (justbytes._constants.DecimalUnits attribute)</a>
   </dt>
 
@@ -1154,15 +1093,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
@@ -1,51 +1,44 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 ****** Index ******
-A | B | C | D | E | F | G | I | J | K | M | N | P | R | S | T | U | V | X | Y |
-Z
+A | B | C | D | E | F | G | I | J | K | M | N | P | R | S | T | U | V | Y | Z
 ***** A *****
   abbr_(justbytes._constants.Unit   ArithmeticPropertiesTestCase_(class_in
   attribute)                        tests.size.operations_test)
   AdditionTestCase_(class_in
   tests.size.operations_test)
 ***** B *****
-  B_(in_module_justbytes._constants)   BinaryUnits_(class_in
-                                       justbytes._constants)
+  B_(in_module_justbytes._constants)        BinaryUnits_(class_in
+  BaseConfig_(class_in_justbytes._config)   justbytes._constants)
 ***** C *****
   components()_(justbytes._size.Range   ConfigurationTestCase_(class_in
   method)                               tests.size.size_test)
   componentsList()_                     ConstantsTestCase_(class_in
   (justbytes._size.Range_method)        tests.constants_test)
   ComponentsTestCase_(class_in          ConstructionTestCase_(class_in
   tests.size.named_test)                tests.size.size_test)
   ComputationTestCase_(class_in         ConversionTestCase_(class_in
   tests.size.size_test)                 tests.size.conversions_test)
   ConfigTestCase_(class_in                    (class_in_tests.size.named_test)
   tests.config_test)                    convertTo()_(justbytes._size.Range
                                         method)
 ***** D *****
-  DecimalUnits_(class_in                DISPLAY_CONFIG_
-  justbytes._constants)                 (justbytes._config.RangeConfig
-  Decorators_(class_in                  attribute)
-  justbytes._util.display)              DisplayConfig_(class_in
-  decorators()_                         justbytes._config)
-  (justbytes._util.display.Decorators   DisplayConfigTestCase_(class_in
-  class_method)                         tests.size.named_test)
-  Digits_(class_in                      DisplayTestCase_(class_in
-  justbytes._util.display)              tests.size.size_test)
-  DigitsConfig_(class_in                DivmodTestCase_(class_in
-  justbytes._config)                    tests.size.operations_test)
-  DigitsConfigTestCase_(class_in
-  tests.size.named_test)
+  DecimalUnits_(class_in                       DisplayConfigTestCase_(class_in
+  justbytes._constants)                        tests.size.named_test)
+  DigitsConfigTestCase_(class_in               DisplayTestCase_(class_in
+  tests.size.named_test)                       tests.size.size_test)
+  DISPLAY_CONFIG_                              DivmodTestCase_(class_in
+  (justbytes._config.RangeConfig_attribute)    tests.size.operations_test)
+  DisplayConfig_(class_in_justbytes._config)
 ***** E *****
   EB_(justbytes._constants.DecimalUnits   ErrorTestCase_(class_in
   attribute)                              tests.errors_test)
   EiB_(justbytes._constants.BinaryUnits
   attribute)
 ***** F *****
   FACTOR_(justbytes._constants.BinaryUnits       FloordivTestCase_(class_in
@@ -59,66 +52,61 @@
   getString()_(justbytes._size.Range      GiB_(justbytes._constants.BinaryUnits
   method)                                 attribute)
 ***** I *****
   InitializerTestCase_(class_in_tests.size.initializer_test)
 ***** J *****
   justbytes_(module)              justbytes._sizes_(module)
   justbytes._config_(module)      justbytes._util_(module)
-  justbytes._constants_(module)   justbytes._util.display_(module)
-  justbytes._errors_(module)      justbytes._util.generators_(module)
-  justbytes._size_(module)        justbytes.version_(module)
+  justbytes._constants_(module)   justbytes._util.generators_(module)
+  justbytes._errors_(module)      justbytes.version_(module)
+  justbytes._size_(module)
 ***** K *****
   KB_(justbytes._constants.DecimalUnits   KiB_(justbytes._constants.BinaryUnits
   attribute)                              attribute)
 ***** M *****
   magnitude_(justbytes._size.Range        ModTestCase_(class_in
   attribute)                              tests.size.operations_test)
   MB_(justbytes._constants.DecimalUnits   MultiplicationTestCase_(class_in
   attribute)                              tests.size.operations_test)
   MiB_(justbytes._constants.BinaryUnits
   attribute)
 ***** N *****
-  next_or_last()_(in_module                 Number_(class_in
-  justbytes._util.generators)               justbytes._util.display)
-  NextTestCase_(class_in_tests.util_test)
+  next_or_last()_(in_module     NextTestCase_(class_in_tests.util_test)
+  justbytes._util.generators)
 ***** P *****
   PB_(justbytes._constants.DecimalUnits   prefix_(justbytes._constants.Unit
   attribute)                              attribute)
   PiB_(justbytes._constants.BinaryUnits
   attribute)
 ***** R *****
   Range_(class_in_justbytes._size)   RangeUnsupportedOpError
   RangeConfig_(class_in              RangeValueError
   justbytes._config)                 RdivmodTestCase_(class_in
   RangeError                         tests.size.operations_test)
-  RangeFractionalResultError         relation_to_symbol()_
-  RangeNonsensicalBinOpError         (justbytes._util.display.Decorators
-  RangeNonsensicalBinOpValueError    static_method)
-  RangeNonsensicalOpError            RfloordivTestCase_(class_in
-  RangePowerResultError              tests.size.operations_test)
-  RangeTestCase_(class_in            RmodTestCase_(class_in
-  tests.config_test)                 tests.size.operations_test)
-  RangeUnrepresentableResultError    RoundingTestCase_(class_in
-                                     tests.size.named_test)
-                                     roundTo()_(justbytes._size.Range_method)
-                                     RsubTestCase_(class_in
+  RangeFractionalResultError         RfloordivTestCase_(class_in
+  RangeNonsensicalBinOpError         tests.size.operations_test)
+  RangeNonsensicalBinOpValueError    RmodTestCase_(class_in
+  RangeNonsensicalOpError            tests.size.operations_test)
+  RangePowerResultError              RoundingTestCase_(class_in
+  RangeTestCase_(class_in            tests.size.named_test)
+  tests.config_test)                 roundTo()_(justbytes._size.Range_method)
+  RangeUnrepresentableResultError    RsubTestCase_(class_in
                                      tests.size.operations_test)
                                      RtruedivTestCase_(class_in
                                      tests.size.operations_test)
 ***** S *****
-  set_display_config()_                               String_(class_in
-  (justbytes._config.RangeConfig_class_method)        justbytes._util.display)
-  set_value_config()_(justbytes._config.RangeConfig   Strip_(class_in
-  class_method)                                       justbytes._util.display)
-  setUp()_(tests.config_test.RangeTestCase_method)    StripConfig_(class_in
-        (tests.size.size_test.ComputationTestCase     justbytes._config)
-        method)                                       SubtractionTestCase_(class
-        (tests.size.size_test.ConfigurationTestCase   in
-        method)                                       tests.size.operations_test)
-  STRICT_(justbytes._config.RangeConfig_attribute)
+  set_display_config()_                               STRICT_
+  (justbytes._config.RangeConfig_class_method)        (justbytes._config.RangeConfig
+  set_value_config()_(justbytes._config.RangeConfig   attribute)
+  class_method)                                       SubtractionTestCase_(class_in
+  setUp()_(tests.config_test.RangeTestCase_method)    tests.size.operations_test)
+        (tests.size.size_test.ComputationTestCase
+        method)
+        (tests.size.size_test.ConfigurationTestCase
+        method)
 ***** T *****
   take_until_satisfied()_(in_module                          testRangePowerResultError()_
   justbytes._util.generators)                                (tests.errors_test.ErrorTestCase_method)
   TakeTestCase_(class_in_tests.util_test)                    testRangeValueError()_
   TB_(justbytes._constants.DecimalUnits_attribute)           (tests.errors_test.ErrorTestCase_method)
   tearDown()_(tests.config_test.RangeTestCase_method)        testRdivmodWithRange()_
         (tests.size.size_test.ComputationTestCase_method)    (tests.size.operations_test.RdivmodTestCase
@@ -245,26 +233,21 @@
                                            class_method)
                                      UtilityMethodsTestCase_(class_in
                                      tests.size.operations_test)
 ***** V *****
   VALUE_CONFIG_(justbytes._config.RangeConfig   VersionTestCase_(class_in
   attribute)                                    tests.version_test)
   ValueConfig_(class_in_justbytes._config)
-***** X *****
-  xform()_(justbytes._util.display.Digits_class_method)
-        (justbytes._util.display.Number_class_method)
-        (justbytes._util.display.String_class_method)
-        (justbytes._util.display.Strip_class_method)
 ***** Y *****
   YB_(justbytes._constants.DecimalUnits   YiB_(justbytes._constants.BinaryUnits
   attribute)                              attribute)
 ***** Z *****
   ZB_(justbytes._constants.DecimalUnits   ZiB_(justbytes._constants.BinaryUnits
   attribute)                              attribute)
 **** Quick search ****
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/_build/html/intro.html` & `justbytes-0.9/doc/_build/html/intro.html`

 * *Files 7% similar despite different names*

```diff
@@ -2,32 +2,32 @@
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
     
-    <title>Justbytes &mdash; justbytes 0.07 documentation</title>
+    <title>Justbytes &mdash; justbytes 0.08 documentation</title>
     
     <link rel="stylesheet" href="_static/default.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     
     <script type="text/javascript">
       var DOCUMENTATION_OPTIONS = {
         URL_ROOT:    './',
-        VERSION:     '0.07',
+        VERSION:     '0.08',
         COLLAPSE_INDEX: false,
         FILE_SUFFIX: '.html',
         HAS_SOURCE:  true
       };
     </script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
-    <link rel="top" title="justbytes 0.07 documentation" href="index.html" />
+    <link rel="top" title="justbytes 0.08 documentation" href="index.html" />
     <link rel="next" title="Tutorial" href="tutorial.html" />
     <link rel="prev" title="Welcome to justbytes’s documentation!" href="index.html" /> 
   </head>
   <body>
     <div class="related">
       <h3>Navigation</h3>
       <ul>
@@ -39,15 +39,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to justbytes’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body">
@@ -141,24 +141,26 @@
 for all numeric values, and to None for Range objects. The type of the
 unit specifier is a named prefix supplied by the size module or a Range object.</p>
 </div>
 <div class="section" id="errors">
 <h2>Errors<a class="headerlink" href="#errors" title="Permalink to this headline">¶</a></h2>
 <p>All errors raised by justbytes operations are subtypes of the RangeError class.</p>
 </div>
-<div class="section" id="measures-of-bandwidth-vs-address-ranges">
-<h2>Measures of Bandwidth vs. Address Ranges<a class="headerlink" href="#measures-of-bandwidth-vs-address-ranges" title="Permalink to this headline">¶</a></h2>
-<p>Bandwidth, e.g., KiB/second and address ranges, e.g., KiB, are related, as their
-units both contain bytes. This relationship is misleading; address ranges and
-bandwidth are far less similar than are volume and flow, e.g., gallons
-and gallons/minute. Bandwidth is simply a measure of the flow of a quantity,
-and there is no implied structure to that quantity. The usual choices for
-representation are appropriate in the case of operations on bandwidth;
-the precision required for manipulation and computation of address ranges
-is not necessary.</p>
+<div class="section" id="memory-consumption-and-bandwidth-vs-address-ranges">
+<h2>Memory Consumption and Bandwidth vs. Address Ranges<a class="headerlink" href="#memory-consumption-and-bandwidth-vs-address-ranges" title="Permalink to this headline">¶</a></h2>
+<p>Memory consumption, e.g., by a process during execution on a specified
+workload, is a quantity, that like address ranges, is specified in
+bytes. However, memory consumption is simply a measurement of the amount of
+a phsyical quantity consumed.  When bytes are used only to represent memory
+consumption, computations do not generally require the special handling
+supplied by this library. Generally, measurement of memory consumption can
+be treated like any other physical quantity. The same reasoning applies to
+bandwidth. For a physical analogy, one can imagine memory consumption to be
+analogous to volume, e.g., litres, and bandwidth to be analogous to flow,
+e.g., litres per minute.</p>
 </div>
 <div class="section" id="user-input">
 <h2>User Input<a class="headerlink" href="#user-input" title="Permalink to this headline">¶</a></h2>
 <p>This package does not handle arbitrary user input. It is expected that the
 client will transform any input, from whatever source, into a number and an
 optional unit specification which can be passed directly to the Range
 constructor.</p>
@@ -184,15 +186,15 @@
 <li><a class="reference internal" href="#operations">Operations</a></li>
 <li><a class="reference internal" href="#floating-point-numbers">Floating Point Numbers</a></li>
 <li><a class="reference internal" href="#computing-the-representation-of-a-range">Computing the Representation of a Range</a></li>
 <li><a class="reference internal" href="#displaying-ranges">Displaying Ranges</a></li>
 <li><a class="reference internal" href="#representing-units">Representing Units</a></li>
 <li><a class="reference internal" href="#constructing-ranges-programatically">Constructing Ranges Programatically</a></li>
 <li><a class="reference internal" href="#errors">Errors</a></li>
-<li><a class="reference internal" href="#measures-of-bandwidth-vs-address-ranges">Measures of Bandwidth vs. Address Ranges</a></li>
+<li><a class="reference internal" href="#memory-consumption-and-bandwidth-vs-address-ranges">Memory Consumption and Bandwidth vs. Address Ranges</a></li>
 <li><a class="reference internal" href="#user-input">User Input</a></li>
 <li><a class="reference internal" href="#alternative-packages">Alternative Packages</a></li>
 </ul>
 </li>
 </ul>
 
   <h4>Previous topic</h4>
@@ -234,15 +236,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to justbytes’s documentation!"
              >previous</a> |</li>
-        <li><a href="index.html">justbytes 0.07 documentation</a> &raquo;</li> 
+        <li><a href="index.html">justbytes 0.08 documentation</a> &raquo;</li> 
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
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 [https://secure.travis-ci.org/mulkieran/justbytes.png?branch=master]
 ****** Justbytes¶ ******
 Justbytes is a module for handling computation with address ranges expressed in
 bytes. Its principle feature is a Range class from which can be constructed
 Range objects which represent a precise and finite address range in bytes.
 Various arithmetic operations are defined for Range objects.
 Its sole purpose is the representation of real address ranges on real machines.
@@ -79,23 +79,24 @@
 used to represent fractional quantities, e.g., “1.2”, but floats are
 disallowed.
 The constructor takes an optional units specifier, which defaults to bytes for
 all numeric values, and to None for Range objects. The type of the unit
 specifier is a named prefix supplied by the size module or a Range object.
 ***** Errors¶ *****
 All errors raised by justbytes operations are subtypes of the RangeError class.
-***** Measures of Bandwidth vs. Address Ranges¶ *****
-Bandwidth, e.g., KiB/second and address ranges, e.g., KiB, are related, as
-their units both contain bytes. This relationship is misleading; address ranges
-and bandwidth are far less similar than are volume and flow, e.g., gallons and
-gallons/minute. Bandwidth is simply a measure of the flow of a quantity, and
-there is no implied structure to that quantity. The usual choices for
-representation are appropriate in the case of operations on bandwidth; the
-precision required for manipulation and computation of address ranges is not
-necessary.
+***** Memory Consumption and Bandwidth vs. Address Ranges¶ *****
+Memory consumption, e.g., by a process during execution on a specified
+workload, is a quantity, that like address ranges, is specified in bytes.
+However, memory consumption is simply a measurement of the amount of a phsyical
+quantity consumed. When bytes are used only to represent memory consumption,
+computations do not generally require the special handling supplied by this
+library. Generally, measurement of memory consumption can be treated like any
+other physical quantity. The same reasoning applies to bandwidth. For a
+physical analogy, one can imagine memory consumption to be analogous to volume,
+e.g., litres, and bandwidth to be analogous to flow, e.g., litres per minute.
 ***** User Input¶ *****
 This package does not handle arbitrary user input. It is expected that the
 client will transform any input, from whatever source, into a number and an
 optional unit specification which can be passed directly to the Range
 constructor.
 ***** Alternative Packages¶ *****
 If you are interested in computing in Python with physical, rather than
@@ -107,15 +108,15 @@
           o Operations
           o Floating_Point_Numbers
           o Computing_the_Representation_of_a_Range
           o Displaying_Ranges
           o Representing_Units
           o Constructing_Ranges_Programatically
           o Errors
-          o Measures_of_Bandwidth_vs._Address_Ranges
+          o Memory_Consumption_and_Bandwidth_vs._Address_Ranges
           o User_Input
           o Alternative_Packages
 *** Previous topic ***
 Welcome_to_justbytes’s_documentation!
 *** Next topic ***
 Tutorial
 **** This Page ****
@@ -124,9 +125,9 @@
 [q                   ] [Go]
 Enter search terms or a module, class or function name.
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * justbytes_0.07_documentation »
+    * justbytes_0.08_documentation »
 © Copyright 2015, mulhern. Created using Sphinx 1.2.3.
```

### Comparing `justbytes-0.8/doc/tutorial.rst` & `justbytes-0.9/doc/tutorial.rst`

 * *Files identical despite different names*

### Comparing `justbytes-0.8/doc/conf.py` & `justbytes-0.9/doc/conf.py`

 * *Files identical despite different names*

