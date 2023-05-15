# Comparing `tmp/odoo-module-migrator-0.3.1.tar.gz` & `tmp/odoo-module-migrator-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/odoo-module-migrator-0.3.1.tar", last modified: Tue Nov 19 12:35:11 2019, max compression
+gzip compressed data, was "odoo-module-migrator-0.4.0.tar", last modified: Mon May 15 10:46:12 2023, max compression
```

## Comparing `odoo-module-migrator-0.3.1.tar` & `odoo-module-migrator-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,67 @@
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)    11855 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        1 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/dependency_links.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       75 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/entry_points.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       20 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/top_level.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       27 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/requires.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1084 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/SOURCES.txt
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)    11855 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/PKG-INFO
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     9249 2019-11-19 12:14:01.000000 odoo-module-migrator-0.3.1/README.rst
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1320 2019-11-19 12:34:28.000000 odoo-module-migrator-0.3.1/setup.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       38 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/setup.cfg
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       25 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/MANIFEST.in
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       27 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/requirements.txt
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/
-drwxrwxr-x   0 sylvain   (1000) sylvain   (1000)        0 2019-11-19 12:35:11.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1683 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_110_120.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3223 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_100_110.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1422 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_090_100.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1520 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_allways.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)        0 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      475 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_080_allways.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      984 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_120_130.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      258 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_100_allways.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2631 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_080_090.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     2161 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/log.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)      294 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/exception.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     8983 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/module_migration.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)       32 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/__init__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     3686 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/__main__.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1506 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/config.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     1596 2019-11-19 12:07:31.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/tools.py
--rw-rw-r--   0 sylvain   (1000) sylvain   (1000)     7184 2019-11-19 12:13:12.000000 odoo-module-migrator-0.3.1/odoo_module_migrate/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.497317 odoo-module-migrator-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-15 10:46:12.497317 odoo-module-migrator-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9268 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/base_migration_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/deprecated_modules/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/deprecated_modules/migrate_080_090/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/deprecated_modules/migrate_080_090/account_modules.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_080_090.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_080_allways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_090_100.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_100_110.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_100_allways.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_110_120.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_120_130.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_130_140.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_140_150.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_150_160.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_allways.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_remove_migration_folder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/python_scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/python_scripts/migrate_allways/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/python_scripts/migrate_allways/bump_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/removed_fields/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/removed_fields/migrate_150_160/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/removed_fields/migrate_150_160/product.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/renamed_fields/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/renamed_fields/migrate_150_160/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/renamed_fields/migrate_150_160/account.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_errors/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_errors/migrate_100_110/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_errors/migrate_100_110/unexisted_models.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_errors/migrate_150_160/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_errors/migrate_150_160/orm_methods.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_replaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_replaces/migrate_120_130/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_replaces/migrate_120_130/decorators.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_replaces/migrate_120_130/digits_precision.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.489317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_warnings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_warnings/migrate_120_130/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_warnings/migrate_120_130/company.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.493317 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_warnings/migrate_150_160/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/text_warnings/migrate_150_160/orm_methods.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/module_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/odoo_module_migrate/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.497317 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9983 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2259 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 10:46:12.000000 odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 10:46:12.497317 odoo-module-migrator-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:46:12.497317 odoo-module-migrator-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-15 10:46:01.000000 odoo-module-migrator-0.4.0/tests/test_migration.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrator.egg-info/PKG-INFO` & `odoo-module-migrator-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,251 +1,260 @@
 Metadata-Version: 2.1
 Name: odoo-module-migrator
-Version: 0.3.1
+Version: 0.4.0
 Summary: Small tools to migrate Odoo modules from a version to another
-Home-page: https://github.com/grap/odoo-module-migrator
+Home-page: https://github.com/OCA/odoo-module-migrator
 Author: GRAP, Groupement Régional Alimentaire de Proximité
 Author-email: informatique@grap.coop
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
-            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-            :alt: License: AGPL-3
-        .. image:: https://img.shields.io/badge/python-3.6-blue.svg
-            :alt: Python support: 3.6
-        .. image:: https://travis-ci.org/grap/odoo-module-migrator.svg?branch=master
-            :target: https://travis-ci.org/grap/odoo-module-migrator
-        .. image:: https://coveralls.io/repos/grap/odoo-module-migrator/badge.png?branch=master
-            :target: https://coveralls.io/r/grap/odoo-module-migrator?branch=master
-        
-        ====================
-        odoo-module-migrator
-        ====================
-        
-        ``odoo-module-migrator`` is a python3 library that allows you to realize automatically
-        recurring changes when migrating Odoo modules from a version to another.
-        for exemple: 
-        
-        * renaming ``__openerp__.py`` file into ``__manifest__.py``
-        * removing ``# -*- encoding: utf-8 -*-`` since V11.0
-        * replacing ``openerp`` import by ``odoo`` import
-        * removing ``migrations`` folders
-        * ...
-        
-        This library will so:
-        
-        * (optionnaly) get commits from the old branch (if format-patch is enabled)
-        * apply automatically changes. (renaming, replacing, etc.)
-        * (depending of the config and the version) black your code.
-        * commit your changes.
-        * Display warnings or errors in log if your code belong obsolete code patterns.
-        
-        **INFO log**
-        
-        It mentions that the lib automatically changed something.
-        *A priori* you have nothing to do. For example, for a migration from 8.0 to
-        a more recent version:
-        
-        .. code-block:: shell
-        
-            12:38:54 INFO Renaming file: '/my_module/__openerp__.py' by '/my_module/__manifest__.py'
-        
-        **WARNING log**
-        
-        It mentions that you should check something. There is *maybe* something to do
-        to make the module working. For exemple:
-        
-        .. code-block:: shell
-        
-            19:37:55 WARNING Replaced dependency of 'account_analytic_analysis' by 'contract' (Moved to OCA/contract)
-        
-        
-        **ERROR log**
-        
-        It mentions that you should change something in your code. It not, the module
-        will not work *for sure*. (not installable, or generating error during the
-        execution)
-        
-        For example, if you have a 8.0 module that depends on 'account_anglo_saxon',
-        that disappeared in more recent version, the following log will be displayed
-        
-        .. code-block:: shell
-        
-            12:38:54 ERROR Depends on removed module 'account_anglo_saxon'
-        
-        Development and improvment
-        ==========================
-        
-        If you want to improve or complete this library, please read the
-        ``DEVELOP.rst`` file and the 'Roadmap / Know issues' sections.
-        
-        Installation
-        ============
-        
-        .. code-block:: shell
-        
-            pip3 install odoo-module-migrator
-        
-        
-        Usage
-        =====
-        
-        Using Format Patch command
-        --------------------------
-        
-        (Recommanded by the OCA)
-        
-        If you want to migrate an Odoo module from a version 8.0 to 12.0, for exemple
-        the module ``pos_order_pricelist_change`` in the OCA "pos" repository.
-        
-        .. code-block:: shell
-        
-            git clone https://github.com/OCA/pos -b 12.0
-            cd pos
-            odoo-module-migrator
-                --directory             ./
-                --modules               pos_order_pricelist_change
-                --init-version-name     8.0
-                --target-version-name  12.0
-                --format-patch
-        
-        Without format Patch command
-        ----------------------------
-        
-        (Mainly for your custom modules)
-        
-        if you have created a new branch (for exemple 12.0) based on your 10.0 branch
-        you can run the following command
-        
-        .. code-block:: shell
-        
-            odoo-module-migrator
-                --directory             /path/to/repository
-                --modules               module_1,module_2,module_3
-                --init-version-name     10.0
-                --target-version-name   12.0
-        
-        This tools will operate the changes for each module.
-        
-        Available arguments
-        -------------------
-        
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |name                      | shortcut | Options         | description                                           |
-        +==========================+==========+=================+=======================================================+
-        |``--directory``           |``-d``    | Default:        | Local folder that belongs the module(s) to migrate.   |
-        |                          |          | ``./``          |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--init-version-name``   | ``-i``   | Required        | Initial version of your module(s) you want to migrate.|
-        |                          |          |                 |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--target-version-name`` | ``-t``   | Default:        | Final Version you want to migrate.                    |
-        |                          |          | the laster odoo |                                                       |
-        |                          |          | version         |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--modules``             | ``-m``   | Default:        | Module(s) to migrate. Note if format-patch option is  |
-        |                          |          | All modules     | enabled, you have to provide only one module.         |
-        |                          |          | present in the  |                                                       |
-        |                          |          | directory       |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--format-patch``        | ``-fp``  | disabled        | Recover code, using git format-patch command.         |
-        |                          |          | by default      |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--remote-name``         | ``-rn``  | Default:        | Name of the main remote, used by format-patch command.|
-        |                          |          | ``origin``      |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--force-black``         | ``-fb``  | depends on the  | Force to use black library.                           |
-        |                          |          | configuration   |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--log-level``           | ``-ll``  | Default:        | Possible value: ``DEBUG``, ``INFO``, ``WARNING``, etc.|
-        |                          |          | ``INFO``        |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--log-path``            | ``-lp``  | Default:        | If set, the logs will not be displayed at screen,     |
-        |                          |          | False           | but stored in a file                                  |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--no-commit``           | ``-nc``  | Default:        | If set the library will not git add and git commit    |
-        |                          |          | commit          | changes.                                              |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        
-        
-        Roadmap / Know issues
-        =====================
-        
-        * replacement of tag <openerp><data> by <odoo> will fail in the case
-          where there are many <data> occurency.
-          We could fix that, using ``lxml`` lib instead of regular expression.
-        
-        Changes
-        =======
-        
-        0.2.0 (October 13, 2019)
-        ------------------------
-        * Second release
-        
-        
-        0.1.4 (October 12, 2019)
-        ------------------------
-        * Test
-        
-        [ADD] test
-        
-        * framework
-        
-        [ADD] ``--file-path`` option.
-        [ADD] ``_DEPRECATED_MODULES`` syntax.
-        
-        * migration script
-        
-        [FIX] Incorrect syntax of regular expression, to remove python 2 header
-        [IMP] first release of all the steps from 8.0 to 13.0
-        
-        
-        0.1.3 (October 11, 2019)
-        ------------------------
-        
-        * framework
-        
-        [ADD] ``--no-commit`` option that disable git add and git commit calls
-        [FIX] do not commit many times if migration has many steps.
-        [REF] remove useless commented code
-        [REF] create _commit_changes() and _replace_in_file() functions
-        
-        * Meta
-        
-        [FIX] github url of the project in setup.py
-        [ADD] Travis file + links to coveralls
-        [ADD] test_requirements.txt
-        
-        * migration script
-        
-        [ADD] 12.0 to 13.0 and add a warning if reference to web_settings_dashboard are found. cortesy @yelizariev
-        [ADD] bump version in manifest file
-        [ADD] set installable to True
-        
-        
-        0.1.2 (October 10, 2019)
-        ------------------------
-        
-        * First release
-        
-        Credits
-        =======
-        
-        Authors
-        -------
-        
-        * GRAP, Groupement Régional Alimentaire de Proximité (http://www.grap.coop)
-        
-        Contributors
-        ------------
-        
-        * Sylvain LE GAL (https://www.twitter.com/legalsylvain)
-        
-        
 Keywords: Odoo Community Association (OCA),Odoo,Migration,Upgrade,Module
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Odoo
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Environment :: Console
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+    :alt: License: AGPL-3
+.. image:: https://img.shields.io/badge/python-3.6-blue.svg
+    :alt: Python support: 3.6
+.. image:: https://app.travis-ci.com/OCA/odoo-module-migrator.svg?branch=master
+    :target: https://app.travis-ci.com/OCA/odoo-module-migrator
+
+====================
+odoo-module-migrator
+====================
+
+``odoo-module-migrator`` is a python3 library that allows you to automatically migrate
+module code to make it compatible with newer Odoo version.
+for exemple:
+
+* renaming ``__openerp__.py`` file into ``__manifest__.py``
+* removing ``# -*- encoding: utf-8 -*-`` since V11.0
+* replacing ``openerp`` import by ``odoo`` import
+* removing ``migrations`` folders
+* changing <act_window> to <record model="ir.actions.window">
+* ...
+
+This library will so:
+
+* (optionnaly) get commits from the old branch (if format-patch is enabled)
+* apply automatically changes. (renaming, replacing, etc.)
+* commit your changes.
+* Display warnings or errors in log if your code belong obsolete code patterns.
+
+This project is about migrating code. If you're looking for database data migration
+between Odoo versions, take a look
+at the https://github.com/OCA/OpenUpgrade project.
+
+**INFO log**
+
+It mentions that the lib automatically changed something.
+*A priori* you have nothing to do. For example, for a migration from 8.0 to
+a more recent version:
+
+.. code-block:: shell
+
+    12:38:54 INFO Renaming file: '/my_module/__openerp__.py' by '/my_module/__manifest__.py'
+
+**WARNING log**
+
+It mentions that you should check something. There is *maybe* something to do
+to make the module working. For exemple:
+
+.. code-block:: shell
+
+    19:37:55 WARNING Replaced dependency of 'account_analytic_analysis' by 'contract' (Moved to OCA/contract)
+
+
+**ERROR log**
+
+It mentions that you should change something in your code. It not, the module
+will not work *for sure*. (not installable, or generating error during the
+execution)
+
+For example, if you have a 8.0 module that depends on 'account_anglo_saxon',
+that disappeared in more recent version, the following log will be displayed
+
+.. code-block:: shell
+
+    12:38:54 ERROR Depends on removed module 'account_anglo_saxon'
+
+Development and improvment
+==========================
+
+If you want to improve or complete this library, please read the
+``DEVELOP.rst`` file and the 'Roadmap / Know issues' sections.
+
+Installation
+============
+
+.. code-block:: shell
+
+    pip3 install odoo-module-migrator
+
+
+Usage
+=====
+
+Using Format Patch command
+--------------------------
+
+(Recommanded by the OCA)
+
+If you want to migrate an Odoo module from a version 8.0 to 12.0, for exemple
+the module ``pos_order_pricelist_change`` in the OCA "pos" repository.
+
+.. code-block:: shell
+
+    git clone https://github.com/OCA/pos -b 12.0
+    cd pos
+    odoo-module-migrate
+        --directory             ./
+        --modules               pos_order_pricelist_change
+        --init-version-name     8.0
+        --target-version-name  12.0
+        --format-patch
+
+Without format Patch command
+----------------------------
+
+(Mainly for your custom modules)
+
+if you have created a new branch (for exemple 12.0) based on your 10.0 branch
+you can run the following command
+
+.. code-block:: shell
+
+    odoo-module-migrate
+        --directory             /path/to/repository
+        --modules               module_1,module_2,module_3
+        --init-version-name     10.0
+        --target-version-name   12.0
+
+This tools will operate the changes for each module.
+
+Available arguments
+-------------------
+
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|name                      | shortcut | Options         | description                                           |
++==========================+==========+=================+=======================================================+
+|``--directory``           |``-d``    | Default:        | Local folder that belongs the module(s) to migrate.   |
+|                          |          | ``./``          |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--init-version-name``   | ``-i``   | Required        | Initial version of your module(s) you want to migrate.|
+|                          |          |                 |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--target-version-name`` | ``-t``   | Default:        | Final Version you want to migrate.                    |
+|                          |          | the laster odoo |                                                       |
+|                          |          | version         |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--modules``             | ``-m``   | Default:        | Module(s) to migrate. Note if format-patch option is  |
+|                          |          | All modules     | enabled, you have to provide only one module.         |
+|                          |          | present in the  |                                                       |
+|                          |          | directory       |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--format-patch``        | ``-fp``  | disabled        | Recover code, using git format-patch command.         |
+|                          |          | by default      |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--remote-name``         | ``-rn``  | Default:        | Name of the main remote, used by format-patch command.|
+|                          |          | ``origin``      |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--log-level``           | ``-ll``  | Default:        | Possible value: ``DEBUG``, ``INFO``, ``WARNING``, etc.|
+|                          |          | ``INFO``        |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--log-path``            | ``-lp``  | Default:        | If set, the logs will not be displayed at screen,     |
+|                          |          | False           | but stored in a file                                  |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--no-commit``           | ``-nc``  | Default:        | If set the library will not git add and git commit    |
+|                          |          | commit          | changes.                                              |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+
+
+Roadmap / Know issues
+=====================
+
+* replacement of tag <openerp><data> by <odoo> will fail in the case
+  where there are many <data> occurency.
+  We could fix that, using ``lxml`` lib instead of regular expression.
+
+* Add a call to ``pre-commit run -a``, if pre-commit is present in the
+  repository.
+
+Changes
+=======
+
+0.3.2 (December 04, 2019)
+-------------------------
+* [REM] Remove black call. (Add call to more generic tool pre-commit
+  in the roadmap)
+* [IMP] Add --no-verify option in ``git commit`` to avoid to fail if pre-commit
+  is present
+* [REF] Refactor ``_execute_shell`` function
+
+
+0.2.0 (October 13, 2019)
+------------------------
+* Second release
+
+
+0.1.4 (October 12, 2019)
+------------------------
+* Test
+
+[ADD] test
+
+* framework
+
+[ADD] ``--file-path`` option.
+[ADD] ``_DEPRECATED_MODULES`` syntax.
+
+* migration script
+
+[FIX] Incorrect syntax of regular expression, to remove python 2 header
+[IMP] first release of all the steps from 8.0 to 13.0
+
+
+0.1.3 (October 11, 2019)
+------------------------
+
+* framework
+
+[ADD] ``--no-commit`` option that disable git add and git commit calls
+[FIX] do not commit many times if migration has many steps.
+[REF] remove useless commented code
+[REF] create _commit_changes() and _replace_in_file() functions
+
+* Meta
+
+[FIX] github url of the project in setup.py
+[ADD] Travis file + links to coveralls
+[ADD] test_requirements.txt
+
+* migration script
+
+[ADD] 12.0 to 13.0 and add a warning if reference to web_settings_dashboard are found. cortesy @yelizariev
+[ADD] bump version in manifest file
+[ADD] set installable to True
+
+
+0.1.2 (October 10, 2019)
+------------------------
+
+* First release
+
+Credits
+=======
+
+Authors
+-------
+
+* GRAP, Groupement Régional Alimentaire de Proximité (http://www.grap.coop)
+
+Contributors
+------------
+
+* Sylvain LE GAL (https://www.twitter.com/legalsylvain)
```

### Comparing `odoo-module-migrator-0.3.1/PKG-INFO` & `odoo-module-migrator-0.4.0/odoo_module_migrator.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,251 +1,260 @@
 Metadata-Version: 2.1
 Name: odoo-module-migrator
-Version: 0.3.1
+Version: 0.4.0
 Summary: Small tools to migrate Odoo modules from a version to another
-Home-page: https://github.com/grap/odoo-module-migrator
+Home-page: https://github.com/OCA/odoo-module-migrator
 Author: GRAP, Groupement Régional Alimentaire de Proximité
 Author-email: informatique@grap.coop
-License: UNKNOWN
-Description: .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
-            :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
-            :alt: License: AGPL-3
-        .. image:: https://img.shields.io/badge/python-3.6-blue.svg
-            :alt: Python support: 3.6
-        .. image:: https://travis-ci.org/grap/odoo-module-migrator.svg?branch=master
-            :target: https://travis-ci.org/grap/odoo-module-migrator
-        .. image:: https://coveralls.io/repos/grap/odoo-module-migrator/badge.png?branch=master
-            :target: https://coveralls.io/r/grap/odoo-module-migrator?branch=master
-        
-        ====================
-        odoo-module-migrator
-        ====================
-        
-        ``odoo-module-migrator`` is a python3 library that allows you to realize automatically
-        recurring changes when migrating Odoo modules from a version to another.
-        for exemple: 
-        
-        * renaming ``__openerp__.py`` file into ``__manifest__.py``
-        * removing ``# -*- encoding: utf-8 -*-`` since V11.0
-        * replacing ``openerp`` import by ``odoo`` import
-        * removing ``migrations`` folders
-        * ...
-        
-        This library will so:
-        
-        * (optionnaly) get commits from the old branch (if format-patch is enabled)
-        * apply automatically changes. (renaming, replacing, etc.)
-        * (depending of the config and the version) black your code.
-        * commit your changes.
-        * Display warnings or errors in log if your code belong obsolete code patterns.
-        
-        **INFO log**
-        
-        It mentions that the lib automatically changed something.
-        *A priori* you have nothing to do. For example, for a migration from 8.0 to
-        a more recent version:
-        
-        .. code-block:: shell
-        
-            12:38:54 INFO Renaming file: '/my_module/__openerp__.py' by '/my_module/__manifest__.py'
-        
-        **WARNING log**
-        
-        It mentions that you should check something. There is *maybe* something to do
-        to make the module working. For exemple:
-        
-        .. code-block:: shell
-        
-            19:37:55 WARNING Replaced dependency of 'account_analytic_analysis' by 'contract' (Moved to OCA/contract)
-        
-        
-        **ERROR log**
-        
-        It mentions that you should change something in your code. It not, the module
-        will not work *for sure*. (not installable, or generating error during the
-        execution)
-        
-        For example, if you have a 8.0 module that depends on 'account_anglo_saxon',
-        that disappeared in more recent version, the following log will be displayed
-        
-        .. code-block:: shell
-        
-            12:38:54 ERROR Depends on removed module 'account_anglo_saxon'
-        
-        Development and improvment
-        ==========================
-        
-        If you want to improve or complete this library, please read the
-        ``DEVELOP.rst`` file and the 'Roadmap / Know issues' sections.
-        
-        Installation
-        ============
-        
-        .. code-block:: shell
-        
-            pip3 install odoo-module-migrator
-        
-        
-        Usage
-        =====
-        
-        Using Format Patch command
-        --------------------------
-        
-        (Recommanded by the OCA)
-        
-        If you want to migrate an Odoo module from a version 8.0 to 12.0, for exemple
-        the module ``pos_order_pricelist_change`` in the OCA "pos" repository.
-        
-        .. code-block:: shell
-        
-            git clone https://github.com/OCA/pos -b 12.0
-            cd pos
-            odoo-module-migrator
-                --directory             ./
-                --modules               pos_order_pricelist_change
-                --init-version-name     8.0
-                --target-version-name  12.0
-                --format-patch
-        
-        Without format Patch command
-        ----------------------------
-        
-        (Mainly for your custom modules)
-        
-        if you have created a new branch (for exemple 12.0) based on your 10.0 branch
-        you can run the following command
-        
-        .. code-block:: shell
-        
-            odoo-module-migrator
-                --directory             /path/to/repository
-                --modules               module_1,module_2,module_3
-                --init-version-name     10.0
-                --target-version-name   12.0
-        
-        This tools will operate the changes for each module.
-        
-        Available arguments
-        -------------------
-        
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |name                      | shortcut | Options         | description                                           |
-        +==========================+==========+=================+=======================================================+
-        |``--directory``           |``-d``    | Default:        | Local folder that belongs the module(s) to migrate.   |
-        |                          |          | ``./``          |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--init-version-name``   | ``-i``   | Required        | Initial version of your module(s) you want to migrate.|
-        |                          |          |                 |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--target-version-name`` | ``-t``   | Default:        | Final Version you want to migrate.                    |
-        |                          |          | the laster odoo |                                                       |
-        |                          |          | version         |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--modules``             | ``-m``   | Default:        | Module(s) to migrate. Note if format-patch option is  |
-        |                          |          | All modules     | enabled, you have to provide only one module.         |
-        |                          |          | present in the  |                                                       |
-        |                          |          | directory       |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--format-patch``        | ``-fp``  | disabled        | Recover code, using git format-patch command.         |
-        |                          |          | by default      |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--remote-name``         | ``-rn``  | Default:        | Name of the main remote, used by format-patch command.|
-        |                          |          | ``origin``      |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--force-black``         | ``-fb``  | depends on the  | Force to use black library.                           |
-        |                          |          | configuration   |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--log-level``           | ``-ll``  | Default:        | Possible value: ``DEBUG``, ``INFO``, ``WARNING``, etc.|
-        |                          |          | ``INFO``        |                                                       |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--log-path``            | ``-lp``  | Default:        | If set, the logs will not be displayed at screen,     |
-        |                          |          | False           | but stored in a file                                  |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        |``--no-commit``           | ``-nc``  | Default:        | If set the library will not git add and git commit    |
-        |                          |          | commit          | changes.                                              |
-        +--------------------------+----------+-----------------+-------------------------------------------------------+
-        
-        
-        Roadmap / Know issues
-        =====================
-        
-        * replacement of tag <openerp><data> by <odoo> will fail in the case
-          where there are many <data> occurency.
-          We could fix that, using ``lxml`` lib instead of regular expression.
-        
-        Changes
-        =======
-        
-        0.2.0 (October 13, 2019)
-        ------------------------
-        * Second release
-        
-        
-        0.1.4 (October 12, 2019)
-        ------------------------
-        * Test
-        
-        [ADD] test
-        
-        * framework
-        
-        [ADD] ``--file-path`` option.
-        [ADD] ``_DEPRECATED_MODULES`` syntax.
-        
-        * migration script
-        
-        [FIX] Incorrect syntax of regular expression, to remove python 2 header
-        [IMP] first release of all the steps from 8.0 to 13.0
-        
-        
-        0.1.3 (October 11, 2019)
-        ------------------------
-        
-        * framework
-        
-        [ADD] ``--no-commit`` option that disable git add and git commit calls
-        [FIX] do not commit many times if migration has many steps.
-        [REF] remove useless commented code
-        [REF] create _commit_changes() and _replace_in_file() functions
-        
-        * Meta
-        
-        [FIX] github url of the project in setup.py
-        [ADD] Travis file + links to coveralls
-        [ADD] test_requirements.txt
-        
-        * migration script
-        
-        [ADD] 12.0 to 13.0 and add a warning if reference to web_settings_dashboard are found. cortesy @yelizariev
-        [ADD] bump version in manifest file
-        [ADD] set installable to True
-        
-        
-        0.1.2 (October 10, 2019)
-        ------------------------
-        
-        * First release
-        
-        Credits
-        =======
-        
-        Authors
-        -------
-        
-        * GRAP, Groupement Régional Alimentaire de Proximité (http://www.grap.coop)
-        
-        Contributors
-        ------------
-        
-        * Sylvain LE GAL (https://www.twitter.com/legalsylvain)
-        
-        
 Keywords: Odoo Community Association (OCA),Odoo,Migration,Upgrade,Module
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Odoo
 Classifier: Topic :: Software Development :: Code Generators
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Environment :: Console
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+.. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
+    :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
+    :alt: License: AGPL-3
+.. image:: https://img.shields.io/badge/python-3.6-blue.svg
+    :alt: Python support: 3.6
+.. image:: https://app.travis-ci.com/OCA/odoo-module-migrator.svg?branch=master
+    :target: https://app.travis-ci.com/OCA/odoo-module-migrator
+
+====================
+odoo-module-migrator
+====================
+
+``odoo-module-migrator`` is a python3 library that allows you to automatically migrate
+module code to make it compatible with newer Odoo version.
+for exemple:
+
+* renaming ``__openerp__.py`` file into ``__manifest__.py``
+* removing ``# -*- encoding: utf-8 -*-`` since V11.0
+* replacing ``openerp`` import by ``odoo`` import
+* removing ``migrations`` folders
+* changing <act_window> to <record model="ir.actions.window">
+* ...
+
+This library will so:
+
+* (optionnaly) get commits from the old branch (if format-patch is enabled)
+* apply automatically changes. (renaming, replacing, etc.)
+* commit your changes.
+* Display warnings or errors in log if your code belong obsolete code patterns.
+
+This project is about migrating code. If you're looking for database data migration
+between Odoo versions, take a look
+at the https://github.com/OCA/OpenUpgrade project.
+
+**INFO log**
+
+It mentions that the lib automatically changed something.
+*A priori* you have nothing to do. For example, for a migration from 8.0 to
+a more recent version:
+
+.. code-block:: shell
+
+    12:38:54 INFO Renaming file: '/my_module/__openerp__.py' by '/my_module/__manifest__.py'
+
+**WARNING log**
+
+It mentions that you should check something. There is *maybe* something to do
+to make the module working. For exemple:
+
+.. code-block:: shell
+
+    19:37:55 WARNING Replaced dependency of 'account_analytic_analysis' by 'contract' (Moved to OCA/contract)
+
+
+**ERROR log**
+
+It mentions that you should change something in your code. It not, the module
+will not work *for sure*. (not installable, or generating error during the
+execution)
+
+For example, if you have a 8.0 module that depends on 'account_anglo_saxon',
+that disappeared in more recent version, the following log will be displayed
+
+.. code-block:: shell
+
+    12:38:54 ERROR Depends on removed module 'account_anglo_saxon'
+
+Development and improvment
+==========================
+
+If you want to improve or complete this library, please read the
+``DEVELOP.rst`` file and the 'Roadmap / Know issues' sections.
+
+Installation
+============
+
+.. code-block:: shell
+
+    pip3 install odoo-module-migrator
+
+
+Usage
+=====
+
+Using Format Patch command
+--------------------------
+
+(Recommanded by the OCA)
+
+If you want to migrate an Odoo module from a version 8.0 to 12.0, for exemple
+the module ``pos_order_pricelist_change`` in the OCA "pos" repository.
+
+.. code-block:: shell
+
+    git clone https://github.com/OCA/pos -b 12.0
+    cd pos
+    odoo-module-migrate
+        --directory             ./
+        --modules               pos_order_pricelist_change
+        --init-version-name     8.0
+        --target-version-name  12.0
+        --format-patch
+
+Without format Patch command
+----------------------------
+
+(Mainly for your custom modules)
+
+if you have created a new branch (for exemple 12.0) based on your 10.0 branch
+you can run the following command
+
+.. code-block:: shell
+
+    odoo-module-migrate
+        --directory             /path/to/repository
+        --modules               module_1,module_2,module_3
+        --init-version-name     10.0
+        --target-version-name   12.0
+
+This tools will operate the changes for each module.
+
+Available arguments
+-------------------
+
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|name                      | shortcut | Options         | description                                           |
++==========================+==========+=================+=======================================================+
+|``--directory``           |``-d``    | Default:        | Local folder that belongs the module(s) to migrate.   |
+|                          |          | ``./``          |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--init-version-name``   | ``-i``   | Required        | Initial version of your module(s) you want to migrate.|
+|                          |          |                 |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--target-version-name`` | ``-t``   | Default:        | Final Version you want to migrate.                    |
+|                          |          | the laster odoo |                                                       |
+|                          |          | version         |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--modules``             | ``-m``   | Default:        | Module(s) to migrate. Note if format-patch option is  |
+|                          |          | All modules     | enabled, you have to provide only one module.         |
+|                          |          | present in the  |                                                       |
+|                          |          | directory       |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--format-patch``        | ``-fp``  | disabled        | Recover code, using git format-patch command.         |
+|                          |          | by default      |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--remote-name``         | ``-rn``  | Default:        | Name of the main remote, used by format-patch command.|
+|                          |          | ``origin``      |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--log-level``           | ``-ll``  | Default:        | Possible value: ``DEBUG``, ``INFO``, ``WARNING``, etc.|
+|                          |          | ``INFO``        |                                                       |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--log-path``            | ``-lp``  | Default:        | If set, the logs will not be displayed at screen,     |
+|                          |          | False           | but stored in a file                                  |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+|``--no-commit``           | ``-nc``  | Default:        | If set the library will not git add and git commit    |
+|                          |          | commit          | changes.                                              |
++--------------------------+----------+-----------------+-------------------------------------------------------+
+
+
+Roadmap / Know issues
+=====================
+
+* replacement of tag <openerp><data> by <odoo> will fail in the case
+  where there are many <data> occurency.
+  We could fix that, using ``lxml`` lib instead of regular expression.
+
+* Add a call to ``pre-commit run -a``, if pre-commit is present in the
+  repository.
+
+Changes
+=======
+
+0.3.2 (December 04, 2019)
+-------------------------
+* [REM] Remove black call. (Add call to more generic tool pre-commit
+  in the roadmap)
+* [IMP] Add --no-verify option in ``git commit`` to avoid to fail if pre-commit
+  is present
+* [REF] Refactor ``_execute_shell`` function
+
+
+0.2.0 (October 13, 2019)
+------------------------
+* Second release
+
+
+0.1.4 (October 12, 2019)
+------------------------
+* Test
+
+[ADD] test
+
+* framework
+
+[ADD] ``--file-path`` option.
+[ADD] ``_DEPRECATED_MODULES`` syntax.
+
+* migration script
+
+[FIX] Incorrect syntax of regular expression, to remove python 2 header
+[IMP] first release of all the steps from 8.0 to 13.0
+
+
+0.1.3 (October 11, 2019)
+------------------------
+
+* framework
+
+[ADD] ``--no-commit`` option that disable git add and git commit calls
+[FIX] do not commit many times if migration has many steps.
+[REF] remove useless commented code
+[REF] create _commit_changes() and _replace_in_file() functions
+
+* Meta
+
+[FIX] github url of the project in setup.py
+[ADD] Travis file + links to coveralls
+[ADD] test_requirements.txt
+
+* migration script
+
+[ADD] 12.0 to 13.0 and add a warning if reference to web_settings_dashboard are found. cortesy @yelizariev
+[ADD] bump version in manifest file
+[ADD] set installable to True
+
+
+0.1.2 (October 10, 2019)
+------------------------
+
+* First release
+
+Credits
+=======
+
+Authors
+-------
+
+* GRAP, Groupement Régional Alimentaire de Proximité (http://www.grap.coop)
+
+Contributors
+------------
+
+* Sylvain LE GAL (https://www.twitter.com/legalsylvain)
```

### Comparing `odoo-module-migrator-0.3.1/README.rst` & `odoo-module-migrator-0.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 .. image:: https://img.shields.io/badge/licence-AGPL--3-blue.svg
     :target: http://www.gnu.org/licenses/agpl-3.0-standalone.html
     :alt: License: AGPL-3
 .. image:: https://img.shields.io/badge/python-3.6-blue.svg
     :alt: Python support: 3.6
-.. image:: https://travis-ci.org/grap/odoo-module-migrator.svg?branch=master
-    :target: https://travis-ci.org/grap/odoo-module-migrator
-.. image:: https://coveralls.io/repos/grap/odoo-module-migrator/badge.png?branch=master
-    :target: https://coveralls.io/r/grap/odoo-module-migrator?branch=master
+.. image:: https://app.travis-ci.com/OCA/odoo-module-migrator.svg?branch=master
+    :target: https://app.travis-ci.com/OCA/odoo-module-migrator
 
 ====================
 odoo-module-migrator
 ====================
 
-``odoo-module-migrator`` is a python3 library that allows you to realize automatically
-recurring changes when migrating Odoo modules from a version to another.
-for exemple: 
+``odoo-module-migrator`` is a python3 library that allows you to automatically migrate
+module code to make it compatible with newer Odoo version.
+for exemple:
 
 * renaming ``__openerp__.py`` file into ``__manifest__.py``
 * removing ``# -*- encoding: utf-8 -*-`` since V11.0
 * replacing ``openerp`` import by ``odoo`` import
 * removing ``migrations`` folders
+* changing <act_window> to <record model="ir.actions.window">
 * ...
 
 This library will so:
 
 * (optionnaly) get commits from the old branch (if format-patch is enabled)
 * apply automatically changes. (renaming, replacing, etc.)
-* (depending of the config and the version) black your code.
 * commit your changes.
 * Display warnings or errors in log if your code belong obsolete code patterns.
 
+This project is about migrating code. If you're looking for database data migration
+between Odoo versions, take a look
+at the https://github.com/OCA/OpenUpgrade project.
+
 **INFO log**
 
 It mentions that the lib automatically changed something.
 *A priori* you have nothing to do. For example, for a migration from 8.0 to
 a more recent version:
 
 .. code-block:: shell
@@ -88,15 +90,15 @@
 If you want to migrate an Odoo module from a version 8.0 to 12.0, for exemple
 the module ``pos_order_pricelist_change`` in the OCA "pos" repository.
 
 .. code-block:: shell
 
     git clone https://github.com/OCA/pos -b 12.0
     cd pos
-    odoo-module-migrator
+    odoo-module-migrate
         --directory             ./
         --modules               pos_order_pricelist_change
         --init-version-name     8.0
         --target-version-name  12.0
         --format-patch
 
 Without format Patch command
@@ -105,15 +107,15 @@
 (Mainly for your custom modules)
 
 if you have created a new branch (for exemple 12.0) based on your 10.0 branch
 you can run the following command
 
 .. code-block:: shell
 
-    odoo-module-migrator
+    odoo-module-migrate
         --directory             /path/to/repository
         --modules               module_1,module_2,module_3
         --init-version-name     10.0
         --target-version-name   12.0
 
 This tools will operate the changes for each module.
 
@@ -140,17 +142,14 @@
 +--------------------------+----------+-----------------+-------------------------------------------------------+
 |``--format-patch``        | ``-fp``  | disabled        | Recover code, using git format-patch command.         |
 |                          |          | by default      |                                                       |
 +--------------------------+----------+-----------------+-------------------------------------------------------+
 |``--remote-name``         | ``-rn``  | Default:        | Name of the main remote, used by format-patch command.|
 |                          |          | ``origin``      |                                                       |
 +--------------------------+----------+-----------------+-------------------------------------------------------+
-|``--force-black``         | ``-fb``  | depends on the  | Force to use black library.                           |
-|                          |          | configuration   |                                                       |
-+--------------------------+----------+-----------------+-------------------------------------------------------+
 |``--log-level``           | ``-ll``  | Default:        | Possible value: ``DEBUG``, ``INFO``, ``WARNING``, etc.|
 |                          |          | ``INFO``        |                                                       |
 +--------------------------+----------+-----------------+-------------------------------------------------------+
 |``--log-path``            | ``-lp``  | Default:        | If set, the logs will not be displayed at screen,     |
 |                          |          | False           | but stored in a file                                  |
 +--------------------------+----------+-----------------+-------------------------------------------------------+
 |``--no-commit``           | ``-nc``  | Default:        | If set the library will not git add and git commit    |
@@ -161,17 +160,29 @@
 Roadmap / Know issues
 =====================
 
 * replacement of tag <openerp><data> by <odoo> will fail in the case
   where there are many <data> occurency.
   We could fix that, using ``lxml`` lib instead of regular expression.
 
+* Add a call to ``pre-commit run -a``, if pre-commit is present in the
+  repository.
+
 Changes
 =======
 
+0.3.2 (December 04, 2019)
+-------------------------
+* [REM] Remove black call. (Add call to more generic tool pre-commit
+  in the roadmap)
+* [IMP] Add --no-verify option in ``git commit`` to avoid to fail if pre-commit
+  is present
+* [REF] Refactor ``_execute_shell`` function
+
+
 0.2.0 (October 13, 2019)
 ------------------------
 * Second release
 
 
 0.1.4 (October 12, 2019)
 ------------------------
@@ -226,8 +237,7 @@
 
 * GRAP, Groupement Régional Alimentaire de Proximité (http://www.grap.coop)
 
 Contributors
 ------------
 
 * Sylvain LE GAL (https://www.twitter.com/legalsylvain)
-
```

### Comparing `odoo-module-migrator-0.3.1/setup.py` & `odoo-module-migrator-0.4.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,33 +2,38 @@
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 import setuptools
 
 setuptools.setup(
     name="odoo-module-migrator",
-    version="0.3.1",
+    version="0.4.0",
     author="GRAP, Groupement Régional Alimentaire de Proximité",
     author_email="informatique@grap.coop",
-    description="Small tools to migrate Odoo modules from a version"
-    " to another",
-    long_description=open('README.rst').read(),
-    long_description_content_type='text/x-rst',
-    url="https://github.com/grap/odoo-module-migrator",
-    packages=['odoo_module_migrate', 'odoo_module_migrate.migration_scripts'],
+    description="Small tools to migrate Odoo modules from a version" " to another",
+    long_description=open("README.rst").read(),
+    long_description_content_type="text/x-rst",
+    url="https://github.com/OCA/odoo-module-migrator",
+    packages=["odoo_module_migrate", "odoo_module_migrate.migration_scripts"],
+    include_package_data=True,
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Framework :: Odoo",
         "Topic :: Software Development :: Code Generators",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Environment :: Console",
     ],
-    install_requires=open('requirements.txt').read().splitlines(),
-    entry_points=dict(console_scripts=[
-        'odoo-module-migrate=odoo_module_migrate.__main__:main',
-    ]),
+    install_requires=open("requirements.txt").read().splitlines(),
+    entry_points=dict(
+        console_scripts=[
+            "odoo-module-migrate=odoo_module_migrate.__main__:main",
+        ]
+    ),
     keywords=[
         "Odoo Community Association (OCA)",
-        "Odoo", "Migration", "Upgrade", "Module",
+        "Odoo",
+        "Migration",
+        "Upgrade",
+        "Module",
     ],
 )
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_110_120.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_090_100.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 # Copyright (C) 2019 - Today: GRAP (http://www.grap.coop)
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
-# TODO
-# All <label> elements in views must have a for="" attribute.
-# All <filter> elements in search views must have a name attribute.
-# All <button> elements in a tree view should have a string attribute
-#   for accessibility.
+from odoo_module_migrate.base_migration_script import BaseMigrationScript
 
 _TEXT_REPLACES = {
-    ".py": {
-        "from odoo.addons.base.res": "from odoo.addons.base.models",
-        "from odoo.addons.base.ir": "from odoo.addons.base.models",
-    }
+    "*": {
+        "base.group_configuration": "base.group_system",
+        "base.group_sale_salesman": "sales_team.group_sale_salesman",
+        "base.group_sale_salesman_all_leads": "sales_team.group_sale_salesman_all_leads",
+        "base.group_sale_manager": "sales_team.group_sale_manager",
+    },
 }
 
 _DEPRECATED_MODULES = [
-    ("account_asset", "oca_moved", "account_asset_management",
-        "Moved to OCA/account-financial-tools"),
-    ("account_budget", "removed"),
-    ("account_cash_basis_base_account", "merged", "account"),
-    ("account_invoicing", "merged", "account"),
-    ("anonymization", "removed"),
-    ("auth_crypt", "merged", "base"),
-    ("base_vat_autocomplete", "renamed", "partner_autocomplete"),
-    ("l10n_be_intrastat", "removed"),
-    ("l10n_be_intrastat_2019", "removed"),
-    ("mrp_repair", "removed"),
-    ("pos_data_drinks", "removed"),
-    ("product_extended", "removed"),
-    ("rating_project", "removed"),
-    ("report_intrastat", "removed"),
-    ("sale_order_dates", "merged", "sale"),
-    ("sale_payment", "merged", "sale"),
-    ("sale_service_rating", "merged", "sale_timesheet"),
-    ("web_planner", "merged", "web"),
-    ("website_forum_doc", "removed"),
-    ("website_quote", "merged", "sale_quotation_builder"),
-    ("website_rating_project", "removed"),
-    ("website_sale_options", "removed"),
-    ("website_sale_stock_options", "removed"),
+    ("account_extra_reports", "removed"),
+    ("account_full_reconcile", "removed"),
+    ("account_tax_adjustments", "removed"),
+    ("account_tax_exigible", "removed"),
+    ("claim_from_delivery", "removed"),
+    ("crm_claim", "removed"),
+    ("crm_partner_assign", "removed"),
+    ("im_odoo_support", "merged", "im_livechat"),
+    ("mail_tip", "merged", "mail"),
+    ("marketing", "merged", "marketing_campaign"),
+    ("mrp_operations", "merged", "mrp"),
+    ("product_uos", "removed"),
+    ("product_visible_discount", "removed"),
+    ("project_timesheet", "merged", "hr_timesheet"),
+    ("report_webkit", "removed"),
+    ("sale_layout", "merged", "sale"),
+    ("sale_service", "merged", "sale_timesheet"),
+    ("warning", "removed"),
+    ("web_analytics", "removed"),
+    ("web_tip", "removed"),
+    ("web_view_editor", "removed"),
+    ("website_crm_claim", "removed"),
 ]
+
+
+class MigrationScript(BaseMigrationScript):
+    _TEXT_REPLACES = _TEXT_REPLACES
+    _DEPRECATED_MODULES = _DEPRECATED_MODULES
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_100_110.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_100_110.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 # Copyright (C) 2019 - Today: GRAP (http://www.grap.coop)
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
+from odoo_module_migrate.base_migration_script import BaseMigrationScript
+
 # TODO: Call 2to3
 
 _TEXT_REPLACES = {
     "*": {
         r"ir.actions.report.xml": "ir.actions.report",
         r"report.external_layout": "web.external_layout",
         r"report.html_container": "web.html_container",
         r"report.layout": "web.report_layout",
         r"report.minimal_layout": "web.minimal_layout",
     },
     ".xml": {
         r"kanban_state_selection": "state_selection",
-    }
+    },
 }
 
 _TEXT_ERRORS = {
     "*": {
-        "('|\")ir.values('|\")":
-            "[V11] Reference to 'ir.values'."
-            " This model has been removed.",
-        "('|\")workflow('|\")":
-            "[V11] Reference to 'workflow'."
-            " This model has been removed.",
-        "('|\")workflow.activity('|\")":
-            "[V11] Reference to 'workflow.activity'."
-            " This model has been removed.",
-        "('|\")workflow.instance('|\")":
-            "[V11] Reference to'workflow.instance'."
-            " This model has been removed.",
-        "('|\")workflow.transition('|\")":
-            "[V11] Reference to 'workflow.transition'."
-            " This model has been removed.",
-        "('|\")workflow.triggers('|\")":
-            "[V11] Reference to 'workflow.triggers'."
-            " This model has been removed.",
-        "('|\")workflow.workitem('|\")":
-            "[V11] Reference to 'workflow.workitem'."
-            " This model has been removed.",
-        "report.external_layout_header":
-            "report.external_layout_header is obsolete.",
-        "report.external_layout_footer":
-            "report.external_layout_footer is obsolete.",
+        "('|\")workflow('|\")": "[V11] Reference to 'workflow'."
+        " This model has been removed.",
+        "('|\")workflow.activity('|\")": "[V11] Reference to 'workflow.activity'."
+        " This model has been removed.",
+        "('|\")workflow.instance('|\")": "[V11] Reference to'workflow.instance'."
+        " This model has been removed.",
+        "('|\")workflow.transition('|\")": "[V11] Reference to 'workflow.transition'."
+        " This model has been removed.",
+        "('|\")workflow.triggers('|\")": "[V11] Reference to 'workflow.triggers'."
+        " This model has been removed.",
+        "('|\")workflow.workitem('|\")": "[V11] Reference to 'workflow.workitem'."
+        " This model has been removed.",
+        "report.external_layout_header": "report.external_layout_header is obsolete.",
+        "report.external_layout_footer": "report.external_layout_footer is obsolete.",
     },
     ".xml": {
-        "<tree(\n|.|\t)*color=\"[^>]*":
-        "color attribute is deprecated in tree view. Use decoration- instead.",
-    }
+        r"<tree[\s][^>]*colors=": "colors attribute is deprecated in tree view."
+        " Use decoration- instead.",
+        r"<tree[\s][^>]*fonts=": "fonts attribute is deprecated in tree view."
+        " Use decoration- instead.",
+    },
 }
 
 _DEPRECATED_MODULES = [
     ("account_accountant", "removed"),
     ("account_tax_cash_basis", "removed"),
     ("base_action_rule", "renamed", "base_automation"),
     ("crm_project_issue", "renamed", "crm_project_issue"),
-    ("hr_timesheet_sheet", "oca_moved", "hr_timesheet_sheet",
-        "Moved to OCA/hr-timesheet"),
+    (
+        "hr_timesheet_sheet",
+        "oca_moved",
+        "hr_timesheet_sheet",
+        "Moved to OCA/hr-timesheet",
+    ),
     ("marketing_campaign", "removed"),
     ("marketing_campaign_crm_demo", "removed"),
     ("portal_gamification", "merged", "gamification"),
     ("portal_sale", "merged", "sale"),
     ("portal_stock", "merged", "portal"),
     ("procurement", "merged", "stock"),
     ("project_issue", "merged", "project"),
@@ -75,9 +72,15 @@
     ("web_kanban", "merged", "web"),
     ("website_issue", "renamed", "website_form_project"),
     ("website_portal", "merged", "website"),
     ("website_project", "merged", "project"),
     ("website_project_issue", "merged", "project"),
     ("website_project_timesheet", "merged", "hr_timesheet"),
     ("website_rating_project_issue", "renamed", "website_rating_project"),
-
 ]
+
+
+class MigrationScript(BaseMigrationScript):
+
+    _TEXT_REPLACES = _TEXT_REPLACES
+    _TEXT_ERRORS = _TEXT_ERRORS
+    _DEPRECATED_MODULES = _DEPRECATED_MODULES
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/migration_scripts/migrate_080_090.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/migration_scripts/migrate_080_090.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 # Copyright (C) 2019 - Today: GRAP (http://www.grap.coop)
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
+from odoo_module_migrate.base_migration_script import BaseMigrationScript
+
 _TEXT_REPLACES = {
     ".py": {"select=True": "index=True"},
 }
 
 _DEPRECATED_MODULES = [
-    ("account_analytic_analysis", "oca_moved", "contract",
-        "Moved to OCA/contract"),
-    ("account_analytic_plans", "oca_moved", "account_analytic_distribution",
-        "Moved to OCA/account_analytic"),
-    ("account_anglo_saxon", "removed"),
+    ("account_analytic_analysis", "oca_moved", "contract", "Moved to OCA/contract"),
+    (
+        "account_analytic_plans",
+        "oca_moved",
+        "account_analytic_distribution",
+        "Moved to OCA/account_analytic",
+    ),
     ("account_bank_statement_extensions", "removed"),
     ("account_chart", "merged", "account"),
     ("account_check_writing", "renamed", "account_check_printing"),
     ("account_followup", "removed"),
-    ("account_payment", "oca_moved", "account_payment_order",
-        "Moved to OCA/bank-payment"),
+    (
+        "account_payment",
+        "oca_moved",
+        "account_payment_order",
+        "Moved to OCA/bank-payment",
+    ),
     ("account_sequence", "removed"),
     ("analytic_contract_hr_expense", "removed"),
     ("analytic_user_function", "removed"),
     ("anglo_saxon_dropshipping", "removed"),
     ("auth_openid", "removed"),
     ("base_report_designer", "removed"),
     ("contacts", "merged", "mail"),
@@ -38,26 +46,40 @@
     ("l10n_fr_rib", "removed"),
     ("marketing_crm", "merged", "crm"),
     ("multi_company", "removed"),
     ("portal_claim", "renamed", "website_crm_claim"),
     ("portal_project", "merged", "project"),
     ("portal_project_issue", "merged", "project_issue"),
     ("procurement_jit_stock", "merged", "procurement_jit"),
-    ("purchase_analytic_plans", "oca_moved", "purchase_analytic_distribution",
-        "Moved to OCA/account-analytic"),
+    (
+        "purchase_analytic_plans",
+        "oca_moved",
+        "purchase_analytic_distribution",
+        "Moved to OCA/account-analytic",
+    ),
     ("purchase_double_validation", "removed"),
-    ("sale_analytic_plans", "oca_moved", "sale_analytic_distribution",
-        "Moved to OCA/account-analytic"),
+    (
+        "sale_analytic_plans",
+        "oca_moved",
+        "sale_analytic_distribution",
+        "Moved to OCA/account-analytic",
+    ),
     ("sale_journal", "removed"),
     ("share", "removed"),
     ("stock_invoice_directly", "removed"),
     ("web_api", "removed"),
     ("web_gantt", "merged", "web"),
     ("web_graph", "merged", "web"),
     ("web_kanban_sparkline", "merged", "web"),
     ("web_tests", "merged", "web"),
     ("web_tests_demo", "removed"),
     ("website_certification", "removed"),
     ("website_instantclick", "removed"),
     ("website_mail_group", "renamed", "website_mail_channel"),
     ("website_report", "merged", "report"),
 ]
+
+
+class MigrationScript(BaseMigrationScript):
+
+    _TEXT_REPLACES = _TEXT_REPLACES
+    _DEPRECATED_MODULES = _DEPRECATED_MODULES
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/module_migration.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/migration.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,222 +1,245 @@
 # Copyright (C) 2019 - Today: GRAP (http://www.grap.coop)
 # @author: Sylvain LE GAL (https://twitter.com/legalsylvain)
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
-import black
+import importlib
 import os
 import pathlib
-import re
+import pkgutil
+import inspect
+
+from .config import _AVAILABLE_MIGRATION_STEPS, _MANIFEST_NAMES
+from .exception import ConfigException
 from .log import logger
+from .tools import _execute_shell, _get_latest_version_code
+from .module_migration import ModuleMigration
+from .base_migration_script import BaseMigrationScript
+
+
+class Migration:
+    def __init__(
+        self,
+        relative_directory_path,
+        init_version_name,
+        target_version_name,
+        module_names=None,
+        format_patch=False,
+        remote_name="origin",
+        commit_enabled=True,
+        pre_commit=True,
+        remove_migration_folder=True,
+    ):
+        if not module_names:
+            module_names = []
+        self._commit_enabled = commit_enabled
+        self._pre_commit = pre_commit
+        self._remove_migration_folder = remove_migration_folder
+        self._migration_steps = []
+        self._migration_scripts = []
+        self._module_migrations = []
+        self._directory_path = False
+
+        # Get migration steps that will be runned
+        found = False
+        for item in _AVAILABLE_MIGRATION_STEPS:
+            if not found and item["init_version_name"] != init_version_name:
+                continue
+            else:
+                found = True
+            self._migration_steps.append(item)
+            if item["target_version_name"] == target_version_name:
+                # This is the last step, exiting
+                break
+
+        # Check consistency between format patch and module_names args
+        if format_patch and len(module_names) != 1:
+            raise ConfigException(
+                "Format patch option can only be used for a single module"
+            )
+        logger.debug("Module list: %s" % module_names)
+        logger.debug("format patch option : %s" % format_patch)
+
+        # convert relative or absolute directory into Path Object
+        if not os.path.exists(relative_directory_path):
+            raise ConfigException(
+                "Unable to find directory: %s" % relative_directory_path
+            )
+
+        root_path = pathlib.Path(relative_directory_path)
+        self._directory_path = pathlib.Path(root_path.resolve(strict=True))
+
+        # format-patch, if required
+        if format_patch:
+            if not (root_path / module_names[0]).is_dir():
+                self._get_code_from_previous_branch(module_names[0], remote_name)
+            else:
+                logger.warning(
+                    "Ignoring format-patch argument, as the module %s"
+                    " is still present in the repository" % (module_names[0])
+                )
+
+        # Guess modules if not provided, and check validity
+        if not module_names:
+            module_names = []
+            # Recover all submodules, if no modules list is provided
+            child_paths = [x for x in root_path.iterdir() if x.is_dir()]
+            for child_path in child_paths:
+                if self._is_module_path(child_path):
+                    module_names.append(child_path.name)
+        else:
+            child_paths = [root_path / x for x in module_names]
+            for child_path in child_paths:
+                if not self._is_module_path(child_path):
+                    module_names.remove(child_path.name)
+                    logger.warning(
+                        "No valid module found for '%s' in the directory '%s'"
+                        % (child_path.name, root_path.resolve())
+                    )
+
+        if not module_names:
+            raise ConfigException("No modules found to migrate. Exiting.")
+
+        for module_name in module_names:
+            self._module_migrations.append(ModuleMigration(self, module_name))
+
+        if os.path.exists(".pre-commit-config.yaml") and self._pre_commit:
+            self._run_pre_commit(module_names)
+
+        # get migration scripts, depending to the migration list
+        self._get_migration_scripts()
+
+    def _run_pre_commit(self, module_names):
+        logger.info("Run pre-commit")
+        _execute_shell(
+            "pre-commit run -a", path=self._directory_path, raise_error=False
+        )
+        if self._commit_enabled:
+            logger.info("Stage and commit changes done by pre-commit")
+            _execute_shell("git add -A", path=self._directory_path)
+            _execute_shell(
+                "git commit -m '[IMP] %s: pre-commit execution' --no-verify"
+                % ", ".join(module_names),
+                path=self._directory_path,
+                raise_error=False,  # Don't fail if there is nothing to commit
+            )
+
+    def _is_module_path(self, module_path):
+        return any([(module_path / x).exists() for x in _MANIFEST_NAMES])
+
+    def _get_code_from_previous_branch(self, module_name, remote_name):
+        init_version = self._migration_steps[0]["init_version_name"]
+        target_version = self._migration_steps[-1]["target_version_name"]
+        branch_name = "%(version)s-mig-%(module_name)s" % {
+            "version": target_version,
+            "module_name": module_name,
+        }
+
+        logger.info("Creating new branch '%s' ..." % (branch_name))
+        _execute_shell(
+            "git checkout --no-track -b %(branch)s %(remote)s/%(version)s"
+            % {
+                "branch": branch_name,
+                "remote": remote_name,
+                "version": target_version,
+            },
+            path=self._directory_path,
+        )
 
-from .config import _ALLOWED_EXTENSIONS, _BLACK_LINE_LENGTH, _MANIFEST_NAMES
-from .tools import _execute_shell
-from . import tools
+        logger.info("Getting latest changes from old branch")
+        # Depth is added just in case you had a shallow git history
+        _execute_shell(
+            "git fetch --depth 9999999 %(remote)s %(init)s"
+            % {
+                "remote": remote_name,
+                "init": init_version,
+            },
+            path=self._directory_path,
+        )
+
+        _execute_shell(
+            "git format-patch --keep-subject "
+            "--stdout %(remote)s/%(target)s..%(remote)s/%(init)s "
+            "-- %(module)s | git am -3 --keep"
+            % {
+                "remote": remote_name,
+                "init": init_version,
+                "target": target_version,
+                "module": module_name,
+            },
+            path=self._directory_path,
+        )
 
+    def _load_migration_script(self, full_name):
+        module = importlib.import_module(full_name)
+        result = [
+            x[1]()
+            for x in inspect.getmembers(module, inspect.isclass)
+            if x[0] != "BaseMigrationScript" and issubclass(x[1], BaseMigrationScript)
+        ]
+        return result
+
+    def _get_migration_scripts(self):
+        # Add the script that will be allways executed
+        self._migration_scripts.extend(
+            self._load_migration_script(
+                "odoo_module_migrate.migration_scripts.migrate_allways"
+            )
+        )
+        if self._remove_migration_folder:
+            self._migration_scripts.extend(
+                self._load_migration_script(
+                    "odoo_module_migrate.migration_scripts."
+                    "migrate_remove_migration_folder"
+                )
+            )
+        all_packages = importlib.import_module("odoo_module_migrate.migration_scripts")
 
-class ModuleMigration():
+        migration_start = float(self._migration_steps[0]["init_version_code"])
+        migration_end = float(self._migration_steps[-1]["target_version_code"])
 
-    _migration = False
-    _module_name = False
-    _module_path = False
+        for loader, name, is_pkg in pkgutil.walk_packages(all_packages.__path__):
+            # Ignore script that will be allways executed.
+            # this script will be added at the end.
+            if name in ("migrate_allways", "migrate_remove_migration_folder"):
+                continue
 
-    def __init__(self, migration, module_name):
-        self._migration = migration
-        self._module_name = module_name
-        self._module_path = self._migration._directory_path / module_name
+            # Filter migration scripts, depending of the configuration
+            full_name = all_packages.__name__ + "." + name
+            if "allways" in name:
+                # replace allways by the most recent version
+                real_name = name.replace("allways", _get_latest_version_code())
+            else:
+                real_name = name
+            splitted_name = real_name.split("_")
 
-    def run(self):
-        logger.info("[%s] Running migration from %s to %s" % (
-            self._module_name,
-            self._migration._migration_steps[0]["init_version_name"],
-            self._migration._migration_steps[-1]["target_version_name"],
-        ))
-
-        # Run Black, if required
-        self._run_black()
-        self._commit_changes(
-            "[REF] %s: Black python code" % (self._module_name))
-
-        # Apply migration script
-        for migration_script in self._migration._migration_scripts:
-            self._run_migration_scripts(migration_script)
-
-        # Rerun black, to avoid that automated changes broke black rules
-        self._run_black()
-        self._commit_changes("[MIG] %s: Migration to %s" % (
-            self._module_name,
-            self._migration._migration_steps[-1]["target_version_name"]))
-
-    def _run_black(self):
-        if not self._migration._use_black:
-            return
-
-        file_mode = black.FileMode()
-        file_mode.line_length = _BLACK_LINE_LENGTH
-
-        for root, directories, filenames in os.walk(
-                self._module_path.resolve()):
-            for filename in filenames:
-                # Skip useless file
-                if os.path.splitext(filename)[1] != ".py":
-                    continue
-
-                absolute_file_path = os.path.join(root, filename)
-
-                black.format_file_in_place(
-                    pathlib.Path(absolute_file_path), False, file_mode,
-                    black.WriteBack.YES)
-
-    def _run_migration_scripts(self, migration_script):
-        file_renames = getattr(migration_script, "_FILE_RENAMES", {})
-        text_replaces = getattr(migration_script, "_TEXT_REPLACES", {})
-        text_errors = getattr(migration_script, "_TEXT_ERRORS", {})
-        global_functions = getattr(migration_script, "_GLOBAL_FUNCTIONS", {})
-        deprecated_modules = getattr(
-            migration_script, "_DEPRECATED_MODULES", {})
-
-        for root, directories, filenames in os.walk(
-                self._module_path.resolve()):
-            for filename in filenames:
-                # Skip useless file
-                # TODO, skip files present in some folders. (for exemple 'lib')
-                extension = os.path.splitext(filename)[1]
-                if extension not in _ALLOWED_EXTENSIONS:
-                    continue
-
-                absolute_file_path = os.path.join(root, filename)
-                logger.debug("Migrate '%s' file" % absolute_file_path)
-
-                # Rename file, if required
-                new_name = file_renames.get(filename)
-                if new_name:
-                    self._rename_file(
-                        self._migration._directory_path,
-                        absolute_file_path,
-                        os.path.join(root, new_name))
-                    absolute_file_path = os.path.join(root, new_name)
-
-                # Operate changes in the file (replacements, removals)
-                replaces = text_replaces.get("*", {})
-                replaces.update(text_replaces.get(extension, {}))
-
-                new_text = tools._replace_in_file(
-                    absolute_file_path, replaces,
-                    "Change file content of %s" % filename)
-
-                # Display errors if the new content contains some obsolete
-                # pattern
-                errors = text_errors.get("*", {})
-                errors.update(text_errors.get(extension, {}))
-                for pattern, error_message in errors.items():
-                    if re.findall(pattern, new_text):
-                        logger.error(error_message)
-
-        # Handle deprecated modules
-        current_manifest_text = tools._read_content(self._get_manifest_path())
-        new_manifest_text = current_manifest_text
-        for items in deprecated_modules:
-            old_module, action = items[0:2]
-            new_module = len(items) > 2 and items[2]
-            old_module_pattern = r"('|\"){0}('|\")".format(old_module)
-            if new_module:
-                new_module_pattern = r"('|\"){0}('|\")".format(new_module)
-                replace_pattern = r"\1{0}\2".format(new_module)
+            script_start = float(splitted_name[1])
+            script_end = float(splitted_name[2])
 
-            if not re.findall(old_module_pattern, new_manifest_text):
+            # Exclude scripts
+            if script_start >= migration_end or script_end <= migration_start:
                 continue
 
-            if action == 'removed':
-                # The module has been removed, just log an error.
-                logger.error(
-                    "Depends on removed module '%s'" % (old_module))
-
-            elif action == 'renamed':
-                new_manifest_text = re.sub(
-                    old_module_pattern, replace_pattern, new_manifest_text)
-                logger.info(
-                    "Replaced dependency of '%s' by '%s'." % (
-                        old_module, new_module))
-
-            elif action == 'oca_moved':
-                new_manifest_text = re.sub(
-                    old_module_pattern, replace_pattern, new_manifest_text)
-                logger.warning(
-                    "Replaced dependency of '%s' by '%s' (%s)\n"
-                    "Check that '%s' is available on your system." % (
-                        old_module, new_module, items[3], new_module))
-
-            elif action == "merged":
-                if not re.findall(new_module_pattern, new_manifest_text):
-                    # adding dependency of the merged module
-                    new_manifest_text = re.sub(
-                        old_module_pattern, replace_pattern, new_manifest_text)
-                    logger.info(
-                        "'%s' merged in '%s'. Replacing dependency." % (
-                            old_module, new_module))
-                else:
-                    # TODO, improve me. we should remove the dependency
-                    # but it could generate coma trouble.
-                    # maybe handling this treatment by ast lib could fix
-                    # the problem.
-                    logger.error(
-                        "'%s' merged in '%s'. You should remove the"
-                        " dependency to '%s' manually." % (
-                            old_module, new_module, old_module))
-
-        if current_manifest_text != new_manifest_text:
-            tools._write_content(self._get_manifest_path(), new_manifest_text)
-
-        if global_functions:
-            for function in global_functions:
-                function(
-                    logger=logger,
-                    module_path=self._module_path,
-                    module_name=self._module_name,
-                    manifest_path=self._get_manifest_path(),
-                    migration_steps=self._migration._migration_steps,
-                    tools=tools,
-                )
+            self._migration_scripts.extend(self._load_migration_script(full_name))
 
-    def _get_manifest_path(self):
-        for manifest_name in _MANIFEST_NAMES:
-            manifest_path = self._module_path / manifest_name
-            if manifest_path.exists():
-                return manifest_path
-
-    def _rename_file(self, module_path, old_file_path, new_file_path):
-        """
-        Rename a file. try to execute 'git mv', to avoid huge diff.
-
-        if 'git mv' fails, make a classical rename
-        """
-        logger.info(
-            "Renaming file: '%s' by '%s' " % (
-                old_file_path.replace(str(module_path.resolve()), ""),
-                new_file_path.replace(str(module_path.resolve()), ""))
+        logger.debug(
+            "The following migration script will be"
+            " executed:\n- %s"
+            % "\n- ".join(
+                [
+                    inspect.getfile(x.__class__).split("/")[-1]
+                    for x in self._migration_scripts
+                ]
+            )
         )
-        if self._migration._commit_enabled:
-            _execute_shell(
-                "cd %s && git mv %s %s" % (
-                    str(module_path.resolve()), old_file_path, new_file_path
-                ))
-        else:
-            _execute_shell(
-                "cd %s && mv %s %s" % (
-                    str(module_path.resolve()), old_file_path, new_file_path
-                ))
-
-    def _commit_changes(self, commit_name):
-        if not self._migration._commit_enabled:
-            return
-
-        if _execute_shell("cd %s && git diff" % (
-                str(self._migration._directory_path.resolve()))):
-            logger.info(
-                "Commit changes for %s. commit name '%s'" % (
-                    self._module_name, commit_name
-                ))
 
-            _execute_shell(
-                "cd %s && git add . --all && git commit -m '%s'" % (
-                    str(self._migration._directory_path.resolve()), commit_name
-                ))
+    def run(self):
+        logger.debug(
+            "Running migration from: %s to: %s in '%s'"
+            % (
+                self._migration_steps[0]["init_version_name"],
+                self._migration_steps[-1]["target_version_name"],
+                self._directory_path.resolve(),
+            )
+        )
+        for module_migration in self._module_migrations:
+            module_migration.run()
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/__main__.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from . import tools
 from .log import setup_logger
 from .migration import Migration
 
 
 def get_parser():
 
-    main_parser = argparse.ArgumentParser(
-        formatter_class=argparse.RawTextHelpFormatter
-    )
+    main_parser = argparse.ArgumentParser(formatter_class=argparse.RawTextHelpFormatter)
 
     main_parser.add_argument(
         "-d",
         "--directory",
         dest="directory",
         default="./",
         type=str,
@@ -58,32 +56,24 @@
         " If 'latest' is set, the tool will try to migrate to the latest"
         " Odoo version.",
     )
 
     main_parser.add_argument(
         "-fp",
         "--format-patch",
-        action='store_true',
+        action="store_true",
         help="Enable this option, if you want to get the code from the"
-        " previous branch."
-    )
-
-    main_parser.add_argument(
-        "-fb",
-        "--force-black",
-        action='store_true',
-        default=True,
-        help="Enable this option, if you want to use 'black' to clean the code"
+        " previous branch.",
     )
 
     main_parser.add_argument(
         "-rn",
         "--remote-name",
         dest="remote_name",
-        default='origin',
+        default="origin",
         type=str,
     )
 
     main_parser.add_argument(
         "-ll",
         "--log-level",
         choices=["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"],
@@ -99,18 +89,36 @@
         default=False,
         type=str,
     )
 
     main_parser.add_argument(
         "-nc",
         "--no-commit",
-        action='store_true',
+        action="store_true",
         default=False,
         help="Enable this option, if you don't want that the library commits"
-        " the changes. (using git add and git commit command)"
+        " the changes. (using git add and git commit command)",
+    )
+
+    # TODO: Move to `argparse.BooleanOptionalAction` once in Python 3.9+
+    main_parser.add_argument(
+        "-npc",
+        "--no-pre-commit",
+        dest="pre_commit",
+        action="store_false",
+        help="Skip pre-commit execution",
+    )
+
+    # TODO: Move to `argparse.BooleanOptionalAction` once in Python 3.9+
+    main_parser.add_argument(
+        "-nrmf",
+        "--no-remove-migration-folder",
+        dest="remove_migration_folder",
+        action="store_false",
+        help="Skip removing migration folder",
     )
 
     return main_parser
 
 
 def main(args=False):
     # Parse Arguments
@@ -122,21 +130,30 @@
         args = parser.parse_args()
 
     # Set log level
     setup_logger(args.log_level, args.log_path)
 
     try:
         # Create a new Migration Object
-        module_names = args.modules\
-            and [x.strip() for x in args.modules.split(",") if x.strip()] or []
+        module_names = (
+            args.modules
+            and [x.strip() for x in args.modules.split(",") if x.strip()]
+            or []
+        )
 
         migration = Migration(
-            args.directory, args.init_version_name, args.target_version_name,
-            module_names, args.format_patch, args.remote_name,
-            args.force_black, not args.no_commit,
+            args.directory,
+            args.init_version_name,
+            args.target_version_name,
+            module_names,
+            args.format_patch,
+            args.remote_name,
+            not args.no_commit,
+            args.pre_commit,
+            args.remove_migration_folder,
         )
 
         # run Migration
         migration.run()
 
     except KeyboardInterrupt:
         pass
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/config.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/config.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,44 +3,62 @@
 # License AGPL-3.0 or later (http://www.gnu.org/licenses/agpl.html).
 
 # List of migrations steps handled by this library
 # * init and target name are friendly name used by the user, when calling
 #   the lib.
 # * init and target code are technical code used to name the migration script
 #   files.
-# * Optional : "use_black" (default=false) the migration will begin with
-#   a call of the library black.
+
 _AVAILABLE_MIGRATION_STEPS = [
     {
         "init_version_name": "8.0",
         "target_version_name": "9.0",
         "init_version_code": "080",
         "target_version_code": "090",
-    }, {
+    },
+    {
         "init_version_name": "9.0",
         "target_version_name": "10.0",
         "init_version_code": "090",
         "target_version_code": "100",
-    }, {
+    },
+    {
         "init_version_name": "10.0",
         "target_version_name": "11.0",
         "init_version_code": "100",
         "target_version_code": "110",
-    }, {
+    },
+    {
         "init_version_name": "11.0",
         "target_version_name": "12.0",
         "init_version_code": "110",
         "target_version_code": "120",
-    }, {
+    },
+    {
         "init_version_name": "12.0",
         "target_version_name": "13.0",
         "init_version_code": "120",
         "target_version_code": "130",
-        "use_black": True,
+    },
+    {
+        "init_version_name": "13.0",
+        "target_version_name": "14.0",
+        "init_version_code": "130",
+        "target_version_code": "140",
+    },
+    {
+        "init_version_name": "14.0",
+        "target_version_name": "15.0",
+        "init_version_code": "140",
+        "target_version_code": "150",
+    },
+    {
+        "init_version_name": "15.0",
+        "target_version_name": "16.0",
+        "init_version_code": "150",
+        "target_version_code": "160",
     },
 ]
 
 _ALLOWED_EXTENSIONS = [".py", ".xml", ".js"]
 
-_BLACK_LINE_LENGTH = 79
-
 _MANIFEST_NAMES = ["__openerp__.py", "__manifest__.py"]
```

### Comparing `odoo-module-migrator-0.3.1/odoo_module_migrate/tools.py` & `odoo-module-migrator-0.4.0/odoo_module_migrate/tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,17 +21,22 @@
     return _AVAILABLE_MIGRATION_STEPS[-1]["target_version_name"]
 
 
 def _get_latest_version_code():
     return _AVAILABLE_MIGRATION_STEPS[-1]["target_version_code"]
 
 
-def _execute_shell(shell_command):
+def _execute_shell(shell_command, path=False, raise_error=True):
+    if path:
+        shell_command = "cd %s && %s" % (str(path.resolve()), shell_command)
     logger.debug("Execute Shell:\n%s" % (shell_command))
-    return subprocess.check_output(shell_command, shell=True)
+    if raise_error:
+        return subprocess.check_output(shell_command, shell=True)
+    else:
+        return subprocess.run(shell_command, shell=True)
 
 
 def _read_content(file_path):
     f = open(file_path, "r")
     text = f.read()
     f.close()
     return text
@@ -44,15 +49,15 @@
 
 
 def _replace_in_file(file_path, replaces, log_message=False):
     current_text = _read_content(file_path)
     new_text = current_text
 
     for old_term, new_term in replaces.items():
-        new_text = re.sub(old_term, new_term, new_text)
+        new_text = re.sub(old_term, new_term or "", new_text)
 
     # Write file if changed
     if new_text != current_text:
         if not log_message:
             log_message = "Changing content of file: %s" % file_path.name
         logger.info(log_message)
         _write_content(file_path, new_text)
```

