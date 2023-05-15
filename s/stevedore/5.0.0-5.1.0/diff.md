# Comparing `tmp/stevedore-5.0.0.tar.gz` & `tmp/stevedore-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stevedore-5.0.0.tar", last modified: Fri Feb 10 18:30:03 2023, max compression
+gzip compressed data, was "stevedore-5.1.0.tar", last modified: Mon May 15 08:16:29 2023, max compression
```

## Comparing `stevedore-5.0.0.tar` & `stevedore-5.1.0.tar`

### file list

```diff
@@ -1,126 +1,127 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.939116 stevedore-5.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-02-10 18:29:38.000000 stevedore-5.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-02-10 18:29:38.000000 stevedore-5.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-02-10 18:29:38.000000 stevedore-5.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-02-10 18:30:03.000000 stevedore-5.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-02-10 18:29:38.000000 stevedore-5.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13955 2023-02-10 18:30:03.000000 stevedore-5.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-02-10 18:29:38.000000 stevedore-5.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2023-02-10 18:30:03.939116 stevedore-5.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-02-10 18:29:38.000000 stevedore-5.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-02-10 18:29:38.000000 stevedore-5.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.915111 stevedore-5.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.915111 stevedore-5.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4157 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.915111 stevedore-5.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.915111 stevedore-5.0.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.919112 stevedore-5.0.0/doc/source/user/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.919112 stevedore-5.0.0/doc/source/user/essays/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    94102 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/api-enforcement.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    86198 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/ceilometer-design.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90088 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/discovery.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71190 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/enabling.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    86848 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/importing.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    82077 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/integration.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77662 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/invocation.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/essays/pycon2013.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/patterns_enabling.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4131 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/patterns_loading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/sphinxext.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.923112 stevedore-5.0.0/doc/source/user/tutorial/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/creating_plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1521 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/driver_output.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/extension_output.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/loading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1913 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/naming.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-02-10 18:29:38.000000 stevedore-5.0.0/doc/source/user/tutorial/testing.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.911110 stevedore-5.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.923112 stevedore-5.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/add-skip-caching-aa13be0299cc8b8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/drop-python2-support-3f0f717570cad8cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/entry-point-type-change-06ca3b301ba7aad1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/expose-entry-point-properties-6f2d868d4342fc0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/module-name-property-d3b2d092259dadec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/notes/remove-extension-extras-attribute-c2c542c9a4dcd304.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.927113 stevedore-5.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.927113 stevedore-5.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.927113 stevedore-5.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8928 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 18:29:38.000000 stevedore-5.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-02-10 18:29:38.000000 stevedore-5.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-02-10 18:30:03.939116 stevedore-5.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-02-10 18:29:38.000000 stevedore-5.0.0/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.931114 stevedore-5.0.0/stevedore/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6637 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9561 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/dispatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6225 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/enabled.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.935115 stevedore-5.0.0/stevedore/example/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/load_as_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/load_as_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example/simple.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.935115 stevedore-5.0.0/stevedore/example2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example2/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1722 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/example2/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13592 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7234 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/named.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/sphinxext.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.939116 stevedore-5.0.0/stevedore/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/extension_unimportable.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2152 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_callback.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_dispatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3325 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_enabled.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_example_fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_example_simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10332 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_named.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_sphinxext.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9561 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/test_test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-02-10 18:29:38.000000 stevedore-5.0.0/stevedore/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 18:30:03.931114 stevedore-5.0.0/stevedore.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2356 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3314 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-02-10 18:30:03.000000 stevedore-5.0.0/stevedore.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-02-10 18:29:38.000000 stevedore-5.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-02-10 18:29:38.000000 stevedore-5.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-15 08:16:03.000000 stevedore-5.1.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-05-15 08:16:03.000000 stevedore-5.1.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-15 08:16:03.000000 stevedore-5.1.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2770 2023-05-15 08:16:29.000000 stevedore-5.1.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      331 2023-05-15 08:16:03.000000 stevedore-5.1.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14163 2023-05-15 08:16:29.000000 stevedore-5.1.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-05-15 08:16:03.000000 stevedore-5.1.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2023-05-15 08:16:29.498132 stevedore-5.1.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2023-05-15 08:16:03.000000 stevedore-5.1.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2023-05-15 08:16:03.000000 stevedore-5.1.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5867 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4157 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      977 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1078 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      985 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/doc/source/user/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/doc/source/user/essays/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94102 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/api-enforcement.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    86198 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/ceilometer-design.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90088 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/discovery.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71190 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/enabling.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    86848 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/importing.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    82077 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/integration.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77662 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/invocation.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19240 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/essays/pycon2013.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/patterns_enabling.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4131 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/patterns_loading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1726 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/sphinxext.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/doc/source/user/tutorial/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/creating_plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1521 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/driver_output.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/extension_output.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5055 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/loading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1913 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/naming.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-05-15 08:16:03.000000 stevedore-5.1.0/doc/source/user/tutorial/testing.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.490131 stevedore-5.1.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/add-reno-996dd44974d53238.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/add-skip-caching-aa13be0299cc8b8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/drop-python2-support-3f0f717570cad8cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/entry-point-type-change-06ca3b301ba7aad1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/expose-entry-point-properties-6f2d868d4342fc0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/module-name-property-d3b2d092259dadec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/notes/remove-extension-extras-attribute-c2c542c9a4dcd304.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.494131 stevedore-5.1.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8928 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-15 08:16:03.000000 stevedore-5.1.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-15 08:16:03.000000 stevedore-5.1.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-05-15 08:16:29.498132 stevedore-5.1.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-05-15 08:16:03.000000 stevedore-5.1.0/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/stevedore/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6658 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9561 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/dispatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6225 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3570 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/enabled.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/stevedore/example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1345 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/load_as_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/load_as_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example/simple.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/stevedore/example2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example2/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1722 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/example2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13592 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7234 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/named.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3806 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/sphinxext.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/stevedore/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/extension_unimportable.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2152 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_callback.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_dispatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3325 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_enabled.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_example_fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_example_simple.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10332 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1713 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_named.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3994 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_sphinxext.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9561 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/test_test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2023-05-15 08:16:03.000000 stevedore-5.1.0/stevedore/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:16:29.498132 stevedore-5.1.0/stevedore.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3345 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-05-15 08:16:29.000000 stevedore-5.1.0/stevedore.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2023-05-15 08:16:03.000000 stevedore-5.1.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1609 2023-05-15 08:16:03.000000 stevedore-5.1.0/tox.ini
```

### Comparing `stevedore-5.0.0/.pre-commit-config.yaml` & `stevedore-5.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/AUTHORS` & `stevedore-5.1.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 Dirk Mueller <dirk@dmllr.de>
 Doug Hellmann <doug.hellmann@dreamhost.com>
 Doug Hellmann <doug.hellmann@gmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Elod Illes <elod.illes@est.tech>
 Evgeni Golov <evgeni@golov.de>
 Flavio Percoco <flaper87@gmail.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
 Ian Wienand <iwienand@redhat.com>
 Jamie Lennox <jamielennox@gmail.com>
 Jason R. Coombs <jaraco@jaraco.com>
 Jeremy Stanley <fungi@yuggoth.org>
 Joshua Harlow <harlowja@gmail.com>
```

### Comparing `stevedore-5.0.0/ChangeLog` & `stevedore-5.1.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+5.1.0
+-----
+
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Update master for stable/2023.1
+
 5.0.0
 -----
 
 
 4.1.1
 -----
 
@@ -12,14 +19,15 @@
 
 4.1.0
 -----
 
 * Remove Extension.extras
 * Fix compatibility with Python 3.12, importlib-metadata 5.0
 * Fix compatibility with Python 3.10, 3.9.11
+* Catch NotADirectoryError error
 * Add Python3 antelope unit tests
 * Update master for stable/zed
 * remove unicode from code
 
 4.0.0
 -----
```

### Comparing `stevedore-5.0.0/LICENSE` & `stevedore-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/PKG-INFO` & `stevedore-5.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: stevedore
-Version: 5.0.0
+Version: 5.1.0
 Summary: Manage dynamic plugins for Python applications
 Home-page: https://docs.openstack.org/stevedore/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===========================================================
         stevedore -- Manage dynamic plugins for Python applications
@@ -38,12 +38,13 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Requires-Python: >=3.8
```

### Comparing `stevedore-5.0.0/README.rst` & `stevedore-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/Makefile` & `stevedore-5.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/conf.py` & `stevedore-5.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/index.rst` & `stevedore-5.1.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/install/index.rst` & `stevedore-5.1.0/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/reference/index.rst` & `stevedore-5.1.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/api-enforcement.jpg` & `stevedore-5.1.0/doc/source/user/essays/api-enforcement.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/ceilometer-design.jpg` & `stevedore-5.1.0/doc/source/user/essays/ceilometer-design.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/discovery.jpg` & `stevedore-5.1.0/doc/source/user/essays/discovery.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/enabling.jpg` & `stevedore-5.1.0/doc/source/user/essays/enabling.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/importing.jpg` & `stevedore-5.1.0/doc/source/user/essays/importing.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/integration.jpg` & `stevedore-5.1.0/doc/source/user/essays/integration.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/invocation.jpg` & `stevedore-5.1.0/doc/source/user/essays/invocation.jpg`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/essays/pycon2013.rst` & `stevedore-5.1.0/doc/source/user/essays/pycon2013.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/patterns_enabling.rst` & `stevedore-5.1.0/doc/source/user/patterns_enabling.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/patterns_loading.rst` & `stevedore-5.1.0/doc/source/user/patterns_loading.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/sphinxext.rst` & `stevedore-5.1.0/doc/source/user/sphinxext.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/creating_plugins.rst` & `stevedore-5.1.0/doc/source/user/tutorial/creating_plugins.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/driver_output.txt` & `stevedore-5.1.0/doc/source/user/tutorial/driver_output.txt`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/extension_output.txt` & `stevedore-5.1.0/doc/source/user/tutorial/extension_output.txt`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/index.rst` & `stevedore-5.1.0/doc/source/user/tutorial/index.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/loading.rst` & `stevedore-5.1.0/doc/source/user/tutorial/loading.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/doc/source/user/tutorial/naming.rst` & `stevedore-5.1.0/doc/source/user/tutorial/naming.rst`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/releasenotes/notes/entry-point-type-change-06ca3b301ba7aad1.yaml` & `stevedore-5.1.0/releasenotes/notes/entry-point-type-change-06ca3b301ba7aad1.yaml`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/releasenotes/source/conf.py` & `stevedore-5.1.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/setup.cfg` & `stevedore-5.1.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 classifier = 
 	Development Status :: 5 - Production/Stable
 	License :: OSI Approved :: Apache Software License
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 	Intended Audience :: Developers
 	Environment :: Console
 
 [files]
 packages =
```

### Comparing `stevedore-5.0.0/setup.py` & `stevedore-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/__init__.py` & `stevedore-5.1.0/stevedore/__init__.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/_cache.py` & `stevedore-5.1.0/stevedore/_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 def _get_mtime(name):
     try:
         s = os.stat(name)
         return s.st_mtime
     except OSError as err:
-        if err.errno != errno.ENOENT:
+        if err.errno not in {errno.ENOENT, errno.ENOTDIR}:
             raise
     return -1.0
 
 
 def _ftobytes(f):
     return struct.Struct('f').pack(f)
```

### Comparing `stevedore-5.0.0/stevedore/dispatch.py` & `stevedore-5.1.0/stevedore/dispatch.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/driver.py` & `stevedore-5.1.0/stevedore/driver.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/enabled.py` & `stevedore-5.1.0/stevedore/enabled.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example/base.py` & `stevedore-5.1.0/stevedore/example/base.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example/load_as_driver.py` & `stevedore-5.1.0/stevedore/example/load_as_driver.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example/load_as_extension.py` & `stevedore-5.1.0/stevedore/example/load_as_extension.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example/setup.py` & `stevedore-5.1.0/stevedore/example/setup.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example/simple.py` & `stevedore-5.1.0/stevedore/example/simple.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example2/fields.py` & `stevedore-5.1.0/stevedore/example2/fields.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/example2/setup.py` & `stevedore-5.1.0/stevedore/example2/setup.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/exception.py` & `stevedore-5.1.0/stevedore/exception.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/extension.py` & `stevedore-5.1.0/stevedore/extension.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/hook.py` & `stevedore-5.1.0/stevedore/hook.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/named.py` & `stevedore-5.1.0/stevedore/named.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/sphinxext.py` & `stevedore-5.1.0/stevedore/sphinxext.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/manager.py` & `stevedore-5.1.0/stevedore/tests/manager.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_cache.py` & `stevedore-5.1.0/stevedore/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_callback.py` & `stevedore-5.1.0/stevedore/tests/test_callback.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_dispatch.py` & `stevedore-5.1.0/stevedore/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_driver.py` & `stevedore-5.1.0/stevedore/tests/test_driver.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_enabled.py` & `stevedore-5.1.0/stevedore/tests/test_enabled.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_example_fields.py` & `stevedore-5.1.0/stevedore/tests/test_example_fields.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_example_simple.py` & `stevedore-5.1.0/stevedore/tests/test_example_simple.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_extension.py` & `stevedore-5.1.0/stevedore/tests/test_extension.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_hook.py` & `stevedore-5.1.0/stevedore/tests/test_hook.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_named.py` & `stevedore-5.1.0/stevedore/tests/test_named.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_sphinxext.py` & `stevedore-5.1.0/stevedore/tests/test_sphinxext.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/test_test_manager.py` & `stevedore-5.1.0/stevedore/tests/test_test_manager.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore/tests/utils.py` & `stevedore-5.1.0/stevedore/tests/utils.py`

 * *Files identical despite different names*

### Comparing `stevedore-5.0.0/stevedore.egg-info/PKG-INFO` & `stevedore-5.1.0/stevedore.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: stevedore
-Version: 5.0.0
+Version: 5.1.0
 Summary: Manage dynamic plugins for Python applications
 Home-page: https://docs.openstack.org/stevedore/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ===========================================================
         stevedore -- Manage dynamic plugins for Python applications
@@ -38,12 +38,13 @@
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Requires-Python: >=3.8
```

### Comparing `stevedore-5.0.0/stevedore.egg-info/SOURCES.txt` & `stevedore-5.1.0/stevedore.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 releasenotes/notes/add-reno-996dd44974d53238.yaml
 releasenotes/notes/add-skip-caching-aa13be0299cc8b8c.yaml
 releasenotes/notes/drop-python2-support-3f0f717570cad8cb.yaml
 releasenotes/notes/entry-point-type-change-06ca3b301ba7aad1.yaml
 releasenotes/notes/expose-entry-point-properties-6f2d868d4342fc0d.yaml
 releasenotes/notes/module-name-property-d3b2d092259dadec.yaml
 releasenotes/notes/remove-extension-extras-attribute-c2c542c9a4dcd304.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
```

### Comparing `stevedore-5.0.0/tox.ini` & `stevedore-5.1.0/tox.ini`

 * *Files identical despite different names*

