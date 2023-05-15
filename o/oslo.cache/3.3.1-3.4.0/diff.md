# Comparing `tmp/oslo.cache-3.3.1.tar.gz` & `tmp/oslo.cache-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oslo.cache-3.3.1.tar", last modified: Tue Feb 21 17:25:10 2023, max compression
+gzip compressed data, was "oslo.cache-3.4.0.tar", last modified: Mon May 15 08:42:54 2023, max compression
```

## Comparing `oslo.cache-3.3.1.tar` & `oslo.cache-3.4.0.tar`

### file list

```diff
@@ -1,176 +1,178 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1743 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3347 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14739 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/user/history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/doc/source/user/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.780510 oslo.cache-3.3.1/oslo.cache.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2332 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4336 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-02-21 17:25:10.000000 oslo.cache-3.3.1/oslo.cache.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/_bmemcache_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/_i18n.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10286 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/_memcache_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13108 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/_opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3290 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/backends/dictionary.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/backends/etcd3gw.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3220 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/backends/memcache_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24179 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/backends/mongo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19397 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/de/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/en_GB/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/es/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/fr/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/it/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/ko_KR/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/pt_BR/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/ru/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/tr_TR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/tr_TR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/tr_TR/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.784510 oslo.cache-3.3.1/oslo_cache/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/zh_CN/LC_MESSAGES/oslo_cache.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/oslo_cache/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/locale/zh_TW/LC_MESSAGES/oslo_cache.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/testing.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_bmemcached/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_bmemcached/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_bmemcached/test_cache_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_pymemcache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_pymemcache/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_pymemcache/test_cache_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/functional/etcd3gw/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/etcd3gw/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/etcd3gw/test_cache_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/functional/memcache_pool/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/memcache_pool/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/memcache_pool/test_cache_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9252 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/functional/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/test_cache.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/oslo_cache/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28035 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/unit/test_cache_backend_mongo.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27117 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/unit/test_cache_basics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6940 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/unit/test_connection_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/tests/unit/test_dict_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/oslo_cache/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/playbooks/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.788510 oslo.cache-3.3.1/playbooks/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/playbooks/tests/functional/pre.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.772510 oslo.cache-3.3.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.792510 oslo.cache-3.3.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/add-dogpile.cache.pymemcache-backend-627d31a76013f8e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/bug-1743036-320ed918d5fb4325.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/bug-1819957-ccff6b0ec9d1cbf2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/bug-1888394-5a53e7a9cb25375b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/enable-sasl-protocol-46d11530b87e7832.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/etcd3gw_driver-8ba4511ae9553a91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/fix-memcache-pool-backend-b9e6aaab08075d68.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/lower_socket_timeout-ff5680a6be23bdb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/memcache_socket_timeout-a7db772f052c107e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/pymemcache_hashclient_configure-f6f48c5ca38bce47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/pymemcache_retry_mecchanisms-fa969d1ac6f64096.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/pymemcache_socket_keepalive-f91c69770961e2b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/notes/switch-from-python-memcached-to-pymemcache-566e70b224f92b73.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9045 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.776510 oslo.cache-3.3.1/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.776510 oslo.cache-3.3.1/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.776510 oslo.cache-3.3.1/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12698 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.776510 oslo.cache-3.3.1/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.776510 oslo.cache-3.3.1/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-21 17:25:10.796510 oslo.cache-3.3.1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/tools/setup-etcd-env.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2023-02-21 17:24:44.000000 oslo.cache-3.3.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1363 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1734 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3383 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15003 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2383 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2826 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/user/history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/doc/source/user/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo.cache.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2383 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4420 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      454 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2023-05-15 08:42:54.000000 oslo.cache-3.4.0/oslo.cache.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2112 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/_bmemcache_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      851 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/_i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10286 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/_memcache_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13108 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/_opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3290 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/backends/dictionary.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/backends/etcd3gw.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3474 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/backends/memcache_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24179 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/backends/mongo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19397 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1859 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/de/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/en_GB/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1984 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/es/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/fr/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1905 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/it/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/ko_KR/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1980 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/pt_BR/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.215767 oslo.cache-3.4.0/oslo_cache/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2413 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/ru/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/tr_TR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/locale/tr_TR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/tr_TR/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1814 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/zh_CN/LC_MESSAGES/oslo_cache.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/oslo_cache/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1810 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/locale/zh_TW/LC_MESSAGES/oslo_cache.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/testing.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_bmemcached/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_bmemcached/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_bmemcached/test_cache_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_pymemcache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_pymemcache/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1133 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_pymemcache/test_cache_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/functional/etcd3gw/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/etcd3gw/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/etcd3gw/test_cache_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/functional/memcache_pool/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/memcache_pool/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1957 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/memcache_pool/test_cache_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9252 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/functional/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/test_cache.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/oslo_cache/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28035 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/unit/test_cache_backend_mongo.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27117 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/unit/test_cache_basics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6940 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/unit/test_connection_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4186 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/tests/unit/test_dict_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      690 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/oslo_cache/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/playbooks/tests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/playbooks/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/playbooks/tests/functional/pre.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.219766 oslo.cache-3.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/add-dogpile.cache.pymemcache-backend-627d31a76013f8e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/bug-1743036-320ed918d5fb4325.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/bug-1819957-ccff6b0ec9d1cbf2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/bug-1888394-5a53e7a9cb25375b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      306 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/bug-1991250-23bc3463273e5a91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/enable-sasl-protocol-46d11530b87e7832.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/etcd3gw_driver-8ba4511ae9553a91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/fix-memcache-pool-backend-b9e6aaab08075d68.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      378 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/lower_socket_timeout-ff5680a6be23bdb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/memcache_socket_timeout-a7db772f052c107e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/pymemcache_hashclient_configure-f6f48c5ca38bce47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/pymemcache_retry_mecchanisms-fa969d1ac6f64096.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/pymemcache_socket_keepalive-f91c69770961e2b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/notes/switch-from-python-memcached-to-pymemcache-566e70b224f92b73.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9045 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1351 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12696 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      963 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.211766 oslo.cache-3.4.0/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1471 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-15 08:42:54.223766 oslo.cache-3.4.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      724 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/tools/setup-etcd-env.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1551 2023-05-15 08:42:27.000000 oslo.cache-3.4.0/tox.ini
```

### Comparing `oslo.cache-3.3.1/.pre-commit-config.yaml` & `oslo.cache-3.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/.zuul.yaml` & `oslo.cache-3.4.0/.zuul.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
       tox_environment:
         OSLO_BACKEND: memcache_pool
 
 - project:
     templates:
       - check-requirements
       - lib-forward-testing-python3
-      - openstack-python3-antelope-jobs
+      - openstack-python3-jobs
       - periodic-stable-jobs
       - publish-openstack-docs-pti
       - release-notes-jobs-python3
     check:
       jobs:
         - oslo.cache-functional-etcd3gw
         - oslo.cache-functional-dogpile.cache.bmemcached
```

### Comparing `oslo.cache-3.3.1/AUTHORS` & `oslo.cache-3.4.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 Doug Hellmann <doug@doughellmann.com>
 Dougal Matthews <dougal@redhat.com>
 Eric Brown <browne@vmware.com>
 Eric Guo <eric.guo@easystack.cn>
 Eric Larson <eric.larson@rackspace.com>
 Flavio Percoco <flaper87@gmail.com>
 George Silvis, III <george.iii.silvis@gmail.com>
+Ghanshyam <gmann@ghanshyammann.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Hervé Beraud <hberaud@redhat.com>
 Ilya Pekelny <ipekelny@mirantis.com>
 James E. Blair <jeblair@hp.com>
 Jamie Lennox <jamielennox@gmail.com>
 Jamie Lennox <jamielennox@redhat.com>
 Jeremy Stanley <fungi@yuggoth.org>
```

### Comparing `oslo.cache-3.3.1/CONTRIBUTING.rst` & `oslo.cache-3.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/ChangeLog` & `oslo.cache-3.4.0/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 CHANGES
 =======
 
+3.4.0
+-----
+
+* Revert "Moves supported python runtimes from version 3.8 to 3.10"
+* Moves supported python runtimes from version 3.8 to 3.10
+* Update master for stable/2023.1
+* Allow bmemcached to be optional for memcache\_pool
+* Imported Translations from Zanata
+
 3.3.1
 -----
 
 * Fix issues related to tox4
 
 3.3.0
 -----
```

### Comparing `oslo.cache-3.3.1/LICENSE` & `oslo.cache-3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/PKG-INFO` & `oslo.cache-3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.cache
-Version: 3.3.1
+Version: 3.4.0
 Summary: Cache storage for OpenStack projects.
 Home-page: https://docs.openstack.org/oslo.cache/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -49,12 +49,13 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Provides-Extra: dogpile
 Provides-Extra: etcd3gw
 Provides-Extra: mongo
 Provides-Extra: test
```

### Comparing `oslo.cache-3.3.1/README.rst` & `oslo.cache-3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/doc/requirements.txt` & `oslo.cache-3.4.0/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/doc/source/conf.py` & `oslo.cache-3.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/doc/source/user/usage.rst` & `oslo.cache-3.4.0/doc/source/user/usage.rst`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo.cache.egg-info/PKG-INFO` & `oslo.cache-3.4.0/oslo.cache.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oslo.cache
-Version: 3.3.1
+Version: 3.4.0
 Summary: Cache storage for OpenStack projects.
 Home-page: https://docs.openstack.org/oslo.cache/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -49,12 +49,13 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.8
 Provides-Extra: dogpile
 Provides-Extra: etcd3gw
 Provides-Extra: mongo
 Provides-Extra: test
```

### Comparing `oslo.cache-3.3.1/oslo.cache.egg-info/SOURCES.txt` & `oslo.cache-3.4.0/oslo.cache.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -77,24 +77,26 @@
 oslo_cache/tests/unit/test_dict_backend.py
 playbooks/tests/functional/pre.yml
 releasenotes/notes/add-dogpile.cache.pymemcache-backend-627d31a76013f8e1.yaml
 releasenotes/notes/add_reno-3b4ae0789e9c45b4.yaml
 releasenotes/notes/bug-1743036-320ed918d5fb4325.yaml
 releasenotes/notes/bug-1819957-ccff6b0ec9d1cbf2.yaml
 releasenotes/notes/bug-1888394-5a53e7a9cb25375b.yaml
+releasenotes/notes/bug-1991250-23bc3463273e5a91.yaml
 releasenotes/notes/drop-python-2-7-73d3113c69d724d6.yaml
 releasenotes/notes/enable-sasl-protocol-46d11530b87e7832.yaml
 releasenotes/notes/etcd3gw_driver-8ba4511ae9553a91.yaml
 releasenotes/notes/fix-memcache-pool-backend-b9e6aaab08075d68.yaml
 releasenotes/notes/lower_socket_timeout-ff5680a6be23bdb2.yaml
 releasenotes/notes/memcache_socket_timeout-a7db772f052c107e.yaml
 releasenotes/notes/pymemcache_hashclient_configure-f6f48c5ca38bce47.yaml
 releasenotes/notes/pymemcache_retry_mecchanisms-fa969d1ac6f64096.yaml
 releasenotes/notes/pymemcache_socket_keepalive-f91c69770961e2b6.yaml
 releasenotes/notes/switch-from-python-memcached-to-pymemcache-566e70b224f92b73.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
```

### Comparing `oslo.cache-3.3.1/oslo_cache/__init__.py` & `oslo.cache-3.4.0/oslo_cache/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/_bmemcache_pool.py` & `oslo.cache-3.4.0/oslo_cache/_bmemcache_pool.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/_i18n.py` & `oslo.cache-3.4.0/oslo_cache/_i18n.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/_memcache_pool.py` & `oslo.cache-3.4.0/oslo_cache/_memcache_pool.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/_opts.py` & `oslo.cache-3.4.0/oslo_cache/_opts.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/backends/dictionary.py` & `oslo.cache-3.4.0/oslo_cache/backends/dictionary.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/backends/etcd3gw.py` & `oslo.cache-3.4.0/oslo_cache/backends/etcd3gw.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/backends/memcache_pool.py` & `oslo.cache-3.4.0/oslo_cache/backends/memcache_pool.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 
 """dogpile.cache backend that uses Memcached connection pool"""
 
 import functools
 
 from dogpile.cache.backends import memcached as memcached_backend
 
-from oslo_cache import _bmemcache_pool
+try:
+    from oslo_cache import _bmemcache_pool
+except ImportError as e:
+    if str(e) == "No module named 'bmemcached'":
+        _bmemcache_pool = None
+    else:
+        raise
 from oslo_cache import _memcache_pool
 
 
 # Helper to ease backend refactoring
 class ClientProxy(object):
     def __init__(self, client_pool):
         self.client_pool = client_pool
@@ -53,14 +59,16 @@
     picking the host to use (from the given server list) based on a key hash.
     """
 
     # Composed from GenericMemcachedBackend's and MemcacheArgs's __init__
     def __init__(self, arguments):
         super(PooledMemcachedBackend, self).__init__(arguments)
         if arguments.get('sasl_enabled', False):
+            if not _bmemcache_pool:
+                raise ImportError("python-binary-memcached package is missing")
             self.client_pool = _bmemcache_pool.BMemcacheClientPool(
                 self.url,
                 arguments,
                 maxsize=arguments.get('pool_maxsize', 10),
                 unused_timeout=arguments.get('pool_unused_timeout', 60),
                 conn_get_timeout=arguments.get('pool_connection_get_timeout',
                                                10),
```

### Comparing `oslo.cache-3.3.1/oslo_cache/backends/mongo.py` & `oslo.cache-3.4.0/oslo_cache/backends/mongo.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/core.py` & `oslo.cache-3.4.0/oslo_cache/core.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/exception.py` & `oslo.cache-3.4.0/oslo_cache/exception.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/de/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/de/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/en_GB/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/en_GB/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/es/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/es/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/fr/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/fr/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/it/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/it/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/ko_KR/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/ko_KR/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/pt_BR/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/pt_BR/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/ru/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/ru/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/tr_TR/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/tr_TR/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/zh_CN/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/zh_CN/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/locale/zh_TW/LC_MESSAGES/oslo_cache.po` & `oslo.cache-3.4.0/oslo_cache/locale/zh_TW/LC_MESSAGES/oslo_cache.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/testing.py` & `oslo.cache-3.4.0/oslo_cache/testing.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/__init__.py` & `oslo.cache-3.4.0/oslo_cache/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_bmemcached/test_cache_backend.py` & `oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_bmemcached/test_cache_backend.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/functional/dogpile_cache_pymemcache/test_cache_backend.py` & `oslo.cache-3.4.0/oslo_cache/tests/functional/dogpile_cache_pymemcache/test_cache_backend.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/functional/etcd3gw/test_cache_backend.py` & `oslo.cache-3.4.0/oslo_cache/tests/functional/etcd3gw/test_cache_backend.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/functional/memcache_pool/test_cache_backend.py` & `oslo.cache-3.4.0/oslo_cache/tests/functional/memcache_pool/test_cache_backend.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/functional/test_base.py` & `oslo.cache-3.4.0/oslo_cache/tests/functional/test_base.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/test_cache.py` & `oslo.cache-3.4.0/oslo_cache/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/unit/test_cache_backend_mongo.py` & `oslo.cache-3.4.0/oslo_cache/tests/unit/test_cache_backend_mongo.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/unit/test_cache_basics.py` & `oslo.cache-3.4.0/oslo_cache/tests/unit/test_cache_basics.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/unit/test_connection_pool.py` & `oslo.cache-3.4.0/oslo_cache/tests/unit/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/tests/unit/test_dict_backend.py` & `oslo.cache-3.4.0/oslo_cache/tests/unit/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/oslo_cache/version.py` & `oslo.cache-3.4.0/oslo_cache/version.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/playbooks/tests/functional/pre.yml` & `oslo.cache-3.4.0/playbooks/tests/functional/pre.yml`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/notes/bug-1819957-ccff6b0ec9d1cbf2.yaml` & `oslo.cache-3.4.0/releasenotes/notes/bug-1819957-ccff6b0ec9d1cbf2.yaml`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/notes/bug-1888394-5a53e7a9cb25375b.yaml` & `oslo.cache-3.4.0/releasenotes/notes/bug-1888394-5a53e7a9cb25375b.yaml`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/source/conf.py` & `oslo.cache-3.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `oslo.cache-3.4.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `oslo.cache-3.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 # Andi Chandler <andi@gowling.com>, 2019. #zanata
 # Andi Chandler <andi@gowling.com>, 2020. #zanata
 # Andi Chandler <andi@gowling.com>, 2022. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: oslo.cache Release Notes\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2022-09-09 16:01+0000\n"
+"POT-Creation-Date: 2023-02-17 17:10+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2022-09-05 10:56+0000\n"
+"PO-Revision-Date: 2022-10-12 01:14+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom)\n"
 "Language: en_GB\n"
 "X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 msgid "1.22.0"
@@ -45,17 +45,14 @@
 
 msgid "1.37.0"
 msgstr "1.37.0"
 
 msgid "1.37.1"
 msgstr "1.37.1"
 
-msgid "1.37.1-4"
-msgstr "1.37.1-4"
-
 msgid "1.9.0"
 msgstr "1.9.0"
 
 msgid "2.0.0"
 msgstr "2.0.0"
 
 msgid "2.1.0"
@@ -66,17 +63,14 @@
 
 msgid "2.2.0"
 msgstr "2.2.0"
 
 msgid "2.3.1"
 msgstr "2.3.1"
 
-msgid "2.3.1-4"
-msgstr "2.3.1-4"
-
 msgid "2.6.2"
 msgstr "2.6.2"
 
 msgid "2.6.3"
 msgstr "2.6.3"
 
 msgid "2.7.0"
@@ -272,14 +266,17 @@
 
 msgid "Xena Series Release Notes"
 msgstr "Xena Series Release Notes"
 
 msgid "Yoga Series Release Notes"
 msgstr "Yoga Series Release Notes"
 
+msgid "Zed Series Release Notes"
+msgstr "Zed Series Release Notes"
+
 msgid ""
 "[`bug 1743036 <https://bugs.launchpad.net/oslo.cache+bug/1743036>`_] The "
 "`backend_argument` value(s) for `url` when configuring memcache did not "
 "properly handle multiple servers. This is because the URL was passed as a "
 "string (comma delimited) instead of a list to the memcache library/client. "
 "The `url` argument is now special cased and will split the string on a comma "
 "so that it mirrors the behavior of the ListOpt used by `memcache_servers` "
```

### Comparing `oslo.cache-3.3.1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `oslo.cache-3.4.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `oslo.cache-3.4.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/setup.cfg` & `oslo.cache-3.4.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 
 [files]
 packages = 
 	oslo_cache
 
 [entry_points]
 oslo.config.opts =
```

### Comparing `oslo.cache-3.3.1/setup.py` & `oslo.cache-3.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/test-requirements.txt` & `oslo.cache-3.4.0/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/tools/setup-etcd-env.sh` & `oslo.cache-3.4.0/tools/setup-etcd-env.sh`

 * *Files identical despite different names*

### Comparing `oslo.cache-3.3.1/tox.ini` & `oslo.cache-3.4.0/tox.ini`

 * *Files identical despite different names*

