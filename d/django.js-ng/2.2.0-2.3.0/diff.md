# Comparing `tmp/django.js-ng-2.2.0.tar.gz` & `tmp/django.js-ng-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django.js-ng-2.2.0.tar", last modified: Tue Feb  8 02:19:34 2022, max compression
+gzip compressed data, was "/home/ubuntu/django.js/dist/.tmp-7idyo06b/django.js-ng-2.3.0.tar", last modified: Mon May 15 02:43:08 2023, max compression
```

## Comparing `django.js-ng-2.2.0.tar` & `django.js-ng-2.3.0.tar`

### file list

```diff
@@ -1,155 +1,155 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       88 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11272 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/PKG-INFO
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        7 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    11272 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4818 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/django.js_ng.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      109 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/MANIFEST.in
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6915 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/CHANGELOG.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1635 2022-02-08 02:17:19.000000 django.js-ng-2.2.0/README.rst
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2183 2021-12-15 01:27:16.000000 django.js-ng-2.2.0/setup.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4639 2022-02-08 02:14:58.000000 django.js-ng-2.2.0/djangojs/context_serializer.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/tests/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    14243 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/test_tags.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      632 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1081 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/test_javascript.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2635 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/test_globber.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6186 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/test_tap.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1295 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tests/test_settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9528 2022-02-08 02:15:23.000000 django.js-ng-2.2.0/djangojs/tests/test_urls.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    12228 2022-02-08 02:15:43.000000 django.js-ng-2.2.0/djangojs/tests/test_context.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1442 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/conf.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/phantomjs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3264 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/phantomjs/qunit-runner.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2988 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/phantomjs/jasmine-runner.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1138 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/wsgi.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6446 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/settings.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       24 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/models.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    18756 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/django.specs.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    41355 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MatchersSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7200 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpySpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      914 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/BaseSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6036 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/ExceptionsSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1367 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/ReporterSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1947 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MultiReporterSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1027 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MockClockSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3818 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpecSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2063 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/NestedResultsSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      751 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/QueueSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    36711 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpecRunningSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8218 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/RunnerSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4742 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/PrettyPrintSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4594 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/WaitsForBlockSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3727 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SuiteSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3449 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/CustomMatchersSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4604 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/EnvSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1339 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/UtilSpec.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3836 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/jasmine/JsApiReporterSpec.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3928 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/ninja.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    10184 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit-tap.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6537 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4668 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5585 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-djangojs.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    70892 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15528 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-jquery.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3929 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/nv.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    58796 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    17882 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/gabe.css
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    20765 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-html.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/test/qunit/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19344 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/qunit/qunit-test.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    42673 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/test/qunit/qunit-deepEqual.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/libs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7251 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.0.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    93636 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.8.3.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    93107 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.2.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   242915 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.2.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7199 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.1.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   274080 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.1.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6911 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.0.0.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    93064 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.1.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   267320 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.0.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   240196 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.0.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83612 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.3.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7086 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.1.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16734 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.0.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83519 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.1.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   266057 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.8.3.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    92629 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.1.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   242727 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.1.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    93068 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.0.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   268381 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.1.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16621 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.1.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   242142 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.3.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83501 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.2.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    83095 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.0.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    15776 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.0.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)   273199 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.2.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    16178 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.1.js
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/static/js/djangojs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3033 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/djangojs/django.min.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7944 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/static/js/djangojs/django.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      370 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/context_processors.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5924 2022-01-25 03:12:35.000000 django.js-ng-2.2.0/djangojs/urls_serializer.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      249 2022-02-08 02:17:05.000000 django.js-ng-2.2.0/djangojs/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/templates/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      440 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/qunit-runner-body.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      147 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/qunit-runner-head.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      543 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/qunit-runner.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      375 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/jasmine-runner-head.html
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/test/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       95 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/test/qunit-test-runner.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      815 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/test/test-data.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      312 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/test/test1.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      520 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/test/djangojs-test-runner.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      791 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/jasmine-runner-body.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      107 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/init.js
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      403 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/django_js_init.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      173 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/django_js_tag.html
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      534 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templates/djangojs/jasmine-runner.html
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/templatetags/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5986 2022-01-25 03:12:52.000000 django.js-ng-2.2.0/djangojs/templatetags/js.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/templatetags/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/fake/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      638 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/fake/models.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/fake/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/fake/locale/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/fake/locale/en/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/fake/locale/en/LC_MESSAGES/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      686 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/fake/locale/en/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/contrib/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      297 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/contrib/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      590 2022-02-08 02:16:06.000000 django.js-ng-2.2.0/djangojs/contrib/social_auth.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2578 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/utils.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3566 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/test_urls.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9425 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/runners.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4715 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/views.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8525 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/tap.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/locale/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/locale/en/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/locale/en/LC_MESSAGES/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      674 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/locale/en/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/locale/fr/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      719 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/locale/fr/LC_MESSAGES/djangojs.po
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1142 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/urls.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/management/
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2022-02-08 02:19:34.000000 django.js-ng-2.2.0/djangojs/management/commands/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      588 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/js_launcher.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1101 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/js_bower.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4407 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/js_localize.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3209 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/js.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      700 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/commands/subparser.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/djangojs/management/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7651 2021-12-10 08:54:43.000000 django.js-ng-2.2.0/LICENSE
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6915 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/CHANGELOG.rst
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7651 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/LICENSE
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      109 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/MANIFEST.in
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8935 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1635 2023-03-10 12:49:59.000000 django.js-ng-2.3.0/README.rst
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8935 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4818 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        1 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        7 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        9 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/django.js_ng.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      249 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1442 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/conf.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      370 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/context_processors.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4633 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/context_serializer.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/contrib/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      297 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/contrib/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      607 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/contrib/social_auth.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/fake/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/fake/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/fake/locale/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/fake/locale/en/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/fake/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      686 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/fake/locale/en/LC_MESSAGES/djangojs.po
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      638 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/fake/models.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/locale/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/locale/en/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      674 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/locale/en/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/locale/fr/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      719 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/locale/fr/LC_MESSAGES/djangojs.po
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/management/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/__init__.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/management/commands/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3209 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/js.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1101 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/js_bower.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      588 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/js_launcher.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4407 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/js_localize.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      700 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/management/commands/subparser.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       24 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/models.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/phantomjs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2988 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/phantomjs/jasmine-runner.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3264 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/phantomjs/qunit-runner.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9425 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/runners.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6446 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/settings.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/djangojs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7944 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/djangojs/django.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3033 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/djangojs/django.min.js
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/libs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   274080 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.1.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    93064 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.1.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   273199 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.2.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    93107 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.2.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   266057 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.8.3.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    93636 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.8.3.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   267320 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.0.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    93068 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.0.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   268381 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.1.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    92629 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.1.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   240196 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.0.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    83095 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.0.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   242727 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.1.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    83519 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.1.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   242915 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.2.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    83501 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.2.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)   242142 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.3.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    83612 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.3.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6911 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.0.0.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    15776 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.0.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    16178 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.1.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7086 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.1.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    16734 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.0.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7251 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.0.min.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    16621 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.1.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7199 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.1.min.js
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/test/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    18756 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/django.specs.js
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      914 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/BaseSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3449 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/CustomMatchersSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4604 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/EnvSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6036 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/ExceptionsSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3836 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/JsApiReporterSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    41355 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MatchersSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1027 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MockClockSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1947 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MultiReporterSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2063 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/NestedResultsSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4742 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/PrettyPrintSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      751 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/QueueSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1367 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/ReporterSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8218 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/RunnerSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    36711 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpecRunningSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3818 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpecSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     7200 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpySpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3727 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SuiteSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1339 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/UtilSpec.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4594 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/jasmine/WaitsForBlockSpec.js
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    17882 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/gabe.css
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5585 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-djangojs.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    20765 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-html.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    15528 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-jquery.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6537 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine.css
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    70892 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3928 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/ninja.css
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3929 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/nv.css
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    10184 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit-tap.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4668 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit.css
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    58796 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit.js
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/static/js/test/qunit/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    42673 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/qunit/qunit-deepEqual.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    19344 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/static/js/test/qunit/qunit-test.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     8525 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tap.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/templates/
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      403 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/django_js_init.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      173 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/django_js_tag.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      107 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/init.js
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      791 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/jasmine-runner-body.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      375 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/jasmine-runner-head.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      534 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/jasmine-runner.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      440 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/qunit-runner-body.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      147 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/qunit-runner-head.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      543 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/qunit-runner.html
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/test/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      520 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/test/djangojs-test-runner.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       95 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/test/qunit-test-runner.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      815 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/test/test-data.html
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      312 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templates/djangojs/test/test1.html
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/templatetags/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)        0 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/templatetags/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6003 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/templatetags/js.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     3566 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/test_urls.py
+drwxrwxr-x   0 ubuntu    (1001) ubuntu    (1001)        0 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/djangojs/tests/
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)      632 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/__init__.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    12246 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/tests/test_context.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2635 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/test_globber.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1081 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/test_javascript.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1295 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/test_settings.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)    14243 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/test_tags.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     6186 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/tests/test_tap.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     9546 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/tests/test_urls.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1142 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/urls.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     5948 2023-05-15 02:30:54.000000 django.js-ng-2.3.0/djangojs/urls_serializer.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2578 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/utils.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     4715 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/views.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     1138 2023-03-10 12:49:09.000000 django.js-ng-2.3.0/djangojs/wsgi.py
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)       67 2023-05-15 02:43:07.000000 django.js-ng-2.3.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1001) ubuntu    (1001)     2183 2023-03-10 12:49:59.000000 django.js-ng-2.3.0/setup.py
```

### Comparing `django.js-ng-2.2.0/django.js_ng.egg-info/SOURCES.txt` & `django.js-ng-2.3.0/django.js_ng.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/CHANGELOG.rst` & `django.js-ng-2.3.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/README.rst` & `django.js-ng-2.3.0/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 - `Dimitri Gnidash's django-js-utils <https://github.com/Dimitri-Gnidash/django-js-utils>`_.
 
 This is currently a work in progress (API wil not be stable before 1.0) so don't expect it to be perfect but please `submit an issue <https://github.com/noirbizarre/django.js/issues>`_ for any bug you find or any feature you want.
 
 Compatibility
 =============
 
-Django.js requires Python 3.x and Django 3.x.
+Django.js requires Python 3.x and Django 2.x.
 
 
 Installation
 ============
 
 You can install Django.js with pip:
```

### Comparing `django.js-ng-2.2.0/setup.py` & `django.js-ng-2.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/context_serializer.py` & `django.js-ng-2.3.0/djangojs/context_serializer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 import json
 import logging
-import six
 
 from django.conf import settings
 from django.template.context import RequestContext
-from django.utils import translation
+from django.utils import translation, six
 
 from djangojs.conf import settings
 from djangojs.utils import LazyJsonEncoder
 
 logger = logging.getLogger(__name__)
```

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_tags.py` & `django.js-ng-2.3.0/djangojs/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/__init__.py` & `django.js-ng-2.3.0/djangojs/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_javascript.py` & `django.js-ng-2.3.0/djangojs/tests/test_javascript.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_globber.py` & `django.js-ng-2.3.0/djangojs/tests/test_globber.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_tap.py` & `django.js-ng-2.3.0/djangojs/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_settings.py` & `django.js-ng-2.3.0/djangojs/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_urls.py` & `django.js-ng-2.3.0/djangojs/tests/test_urls.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
-import six
 
 from django.core.cache import cache
 from django.core.urlresolvers import reverse
 from django.test import TestCase
 from django.test.utils import override_settings
+from django.utils import six
 
 
 class UrlsTestMixin(object):
     urls = 'djangojs.test_urls'
 
     def setUp(self):
         self.result = self.get_result()
```

### Comparing `django.js-ng-2.2.0/djangojs/tests/test_context.py` & `django.js-ng-2.3.0/djangojs/tests/test_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 import json
-import six
 
 from django import VERSION as DJANGO_VERSION
 from django.conf import global_settings
 from django.contrib.auth.management import create_permissions
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.management import update_contenttypes
 from django.contrib.sessions.middleware import SessionMiddleware
 from django.core.urlresolvers import reverse
 from django.db.models import get_app
 from django.middleware.locale import LocaleMiddleware
 from django.test import TestCase
 from django.test.client import RequestFactory
 from django.test.utils import override_settings
+from django.utils import six
 from django.utils import translation
 from django.utils import unittest
 
 from djangojs.conf import settings
 from djangojs.utils import class_from_string
 
 TEST_CONTEXT_PROCESSORS = global_settings.TEMPLATE_CONTEXT_PROCESSORS + (
```

### Comparing `django.js-ng-2.2.0/djangojs/conf.py` & `django.js-ng-2.3.0/djangojs/conf.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/phantomjs/qunit-runner.js` & `django.js-ng-2.3.0/djangojs/phantomjs/qunit-runner.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/phantomjs/jasmine-runner.js` & `django.js-ng-2.3.0/djangojs/phantomjs/jasmine-runner.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/wsgi.py` & `django.js-ng-2.3.0/djangojs/wsgi.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/settings.py` & `django.js-ng-2.3.0/djangojs/settings.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/django.specs.js` & `django.js-ng-2.3.0/djangojs/static/js/test/django.specs.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MatchersSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MatchersSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpySpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpySpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/BaseSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/BaseSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/ExceptionsSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/ExceptionsSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/ReporterSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/ReporterSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MultiReporterSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MultiReporterSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/MockClockSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/MockClockSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpecSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpecSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/NestedResultsSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/NestedResultsSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/QueueSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/QueueSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SpecRunningSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SpecRunningSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/RunnerSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/RunnerSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/PrettyPrintSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/PrettyPrintSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/WaitsForBlockSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/WaitsForBlockSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/SuiteSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/SuiteSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/CustomMatchersSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/CustomMatchersSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/EnvSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/EnvSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/UtilSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/UtilSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/jasmine/JsApiReporterSpec.js` & `django.js-ng-2.3.0/djangojs/static/js/test/jasmine/JsApiReporterSpec.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/ninja.css` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/ninja.css`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit-tap.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit-tap.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine.css` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine.css`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit.css` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit.css`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-djangojs.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-djangojs.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-jquery.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-jquery.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/nv.css` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/nv.css`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/qunit.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/qunit.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/gabe.css` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/gabe.css`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/libs/jasmine-html.js` & `django.js-ng-2.3.0/djangojs/static/js/test/libs/jasmine-html.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/qunit/qunit-test.js` & `django.js-ng-2.3.0/djangojs/static/js/test/qunit/qunit-test.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/test/qunit/qunit-deepEqual.js` & `django.js-ng-2.3.0/djangojs/static/js/test/qunit/qunit-deepEqual.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.0.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.0.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.8.3.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.8.3.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.2.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.2.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.2.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.2.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.1.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.1.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.1.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.0.0.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.0.0.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.1.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.1.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.0.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.0.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.0.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.0.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.3.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.3.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.1.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.1.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.0.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.0.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.1.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.1.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.8.3.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.8.3.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.1.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.1.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.1.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.0.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.0.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.9.1.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.9.1.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.2.1.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.2.1.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.3.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.3.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.2.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.2.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-2.0.0.min.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-2.0.0.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.0.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.0.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-1.10.2.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-1.10.2.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/libs/jquery-migrate-1.1.1.js` & `django.js-ng-2.3.0/djangojs/static/js/libs/jquery-migrate-1.1.1.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/djangojs/django.min.js` & `django.js-ng-2.3.0/djangojs/static/js/djangojs/django.min.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/static/js/djangojs/django.js` & `django.js-ng-2.3.0/djangojs/static/js/djangojs/django.js`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/urls_serializer.py` & `django.js-ng-2.3.0/djangojs/urls_serializer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 from __future__ import unicode_literals
 
 import json
 import logging
 import re
-import six
 import sys
 import types
 
 from django.core.serializers.json import DjangoJSONEncoder
 from django.urls import URLPattern, URLResolver, get_script_prefix
+from django.utils import six
 
 from djangojs.conf import settings
 
 logger = logging.getLogger(__name__)
 
 
 __all__ = (
@@ -83,15 +83,15 @@
             if settings.JS_URLS and pattern_name not in settings.JS_URLS:
                 return {}
             if settings.JS_URLS_EXCLUDE and pattern_name in settings.JS_URLS_EXCLUDE:
                 return {}
             if namespace:
                 pattern_name = ':'.join((namespace, pattern_name))
             full_url = prefix + pattern.pattern.regex.pattern
-            for char in ['^', '$']:
+            for char in ['^', '$', '\Z']:
                 full_url = full_url.replace(char, '')
             # remove optionnal non capturing groups
             opt_grp_matches = RE_OPT_GRP.findall(full_url)
             if opt_grp_matches:
                 for match in opt_grp_matches:
                     full_url = full_url.replace(match, '')
             # remove optionnal characters
```

### Comparing `django.js-ng-2.2.0/djangojs/templates/djangojs/qunit-runner.html` & `django.js-ng-2.3.0/djangojs/templates/djangojs/qunit-runner.html`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/templates/djangojs/test/test-data.html` & `django.js-ng-2.3.0/djangojs/templates/djangojs/test/test-data.html`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/templates/djangojs/test/djangojs-test-runner.html` & `django.js-ng-2.3.0/djangojs/templates/djangojs/test/djangojs-test-runner.html`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/templates/djangojs/jasmine-runner-body.html` & `django.js-ng-2.3.0/djangojs/templates/djangojs/jasmine-runner-body.html`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/templates/djangojs/jasmine-runner.html` & `django.js-ng-2.3.0/djangojs/templates/djangojs/jasmine-runner.html`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/templatetags/js.py` & `django.js-ng-2.3.0/djangojs/templatetags/js.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # -*- coding: utf-8 -*-
 '''
 Provide template tags to help with Javascript/Django integration.
 '''
 from __future__ import unicode_literals
 
-import six
-
 from django import template
 from django.contrib.staticfiles.storage import staticfiles_storage
+from django.utils import six
 from django.utils.safestring import mark_safe
 
 from djangojs import JQUERY_MIGRATE_VERSION
 from djangojs.conf import settings
 
 register = template.Library()
```

### Comparing `django.js-ng-2.2.0/djangojs/fake/models.py` & `django.js-ng-2.3.0/djangojs/fake/models.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/fake/locale/en/LC_MESSAGES/djangojs.po` & `django.js-ng-2.3.0/djangojs/fake/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/contrib/social_auth.py` & `django.js-ng-2.3.0/djangojs/contrib/social_auth.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
-import six
-
+from django.utils import six
 from djangojs.context_serializer import ContextSerializer
 
 
 class SocialAuthContextMixin(object):
     '''Handle django_social_auth context specifics'''
     def process_social_auth(self, social_auth, data):
         """ Just force social_auth's LazyDict to be converted to a dict for the
```

### Comparing `django.js-ng-2.2.0/djangojs/utils.py` & `django.js-ng-2.3.0/djangojs/utils.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/test_urls.py` & `django.js-ng-2.3.0/djangojs/test_urls.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/runners.py` & `django.js-ng-2.3.0/djangojs/runners.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/views.py` & `django.js-ng-2.3.0/djangojs/views.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/tap.py` & `django.js-ng-2.3.0/djangojs/tap.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/locale/en/LC_MESSAGES/djangojs.po` & `django.js-ng-2.3.0/djangojs/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/locale/fr/LC_MESSAGES/djangojs.po` & `django.js-ng-2.3.0/djangojs/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/urls.py` & `django.js-ng-2.3.0/djangojs/urls.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/management/commands/js_launcher.py` & `django.js-ng-2.3.0/djangojs/management/commands/js_launcher.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/management/commands/js_bower.py` & `django.js-ng-2.3.0/djangojs/management/commands/js_bower.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/management/commands/js_localize.py` & `django.js-ng-2.3.0/djangojs/management/commands/js_localize.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/management/commands/js.py` & `django.js-ng-2.3.0/djangojs/management/commands/js.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/djangojs/management/commands/subparser.py` & `django.js-ng-2.3.0/djangojs/management/commands/subparser.py`

 * *Files identical despite different names*

### Comparing `django.js-ng-2.2.0/LICENSE` & `django.js-ng-2.3.0/LICENSE`

 * *Files identical despite different names*

