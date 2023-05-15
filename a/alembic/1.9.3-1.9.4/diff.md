# Comparing `tmp/alembic-1.9.3.tar.gz` & `tmp/alembic-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alembic-1.9.3.tar", last modified: Tue Feb  7 20:47:19 2023, max compression
+gzip compressed data, was "alembic-1.9.4.tar", last modified: Thu Feb 16 17:35:43 2023, max compression
```

## Comparing `alembic-1.9.3.tar` & `alembic-1.9.4.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.407879 alembic-1.9.3/
--rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-02-07 20:46:41.000000 alembic-1.9.3/CHANGES
--rw-r--r--   0 classic   (1000) classic   (1000)     1058 2023-02-07 20:46:41.000000 alembic-1.9.3/LICENSE
--rw-r--r--   0 classic   (1000) classic   (1000)      330 2023-02-07 20:46:41.000000 alembic-1.9.3/MANIFEST.in
--rw-r--r--   0 classic   (1000) classic   (1000)     6967 2023-02-07 20:47:19.407879 alembic-1.9.3/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     5736 2023-02-07 20:46:41.000000 alembic-1.9.3/README.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    15001 2023-02-07 20:46:41.000000 alembic-1.9.3/README.unittests.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.382878 alembic-1.9.3/alembic/
--rw-r--r--   0 classic   (1000) classic   (1000)       74 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)       78 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/__main__.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.384878 alembic-1.9.3/alembic/autogenerate/
--rw-r--r--   0 classic   (1000) classic   (1000)      351 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/autogenerate/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20558 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/autogenerate/api.py
--rw-r--r--   0 classic   (1000) classic   (1000)    46034 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/autogenerate/compare.py
--rw-r--r--   0 classic   (1000) classic   (1000)    34698 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/autogenerate/render.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7466 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/autogenerate/rewriter.py
--rw-r--r--   0 classic   (1000) classic   (1000)    21077 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/command.py
--rw-r--r--   0 classic   (1000) classic   (1000)    20578 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/config.py
--rw-r--r--   0 classic   (1000) classic   (1000)      195 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/context.py
--rw-r--r--   0 classic   (1000) classic   (1000)    28807 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/context.pyi
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.384878 alembic-1.9.3/alembic/ddl/
--rw-r--r--   0 classic   (1000) classic   (1000)      137 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     9590 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/base.py
--rw-r--r--   0 classic   (1000) classic   (1000)    22926 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/impl.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13969 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/mssql.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16322 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/mysql.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6092 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/oracle.py
--rw-r--r--   0 classic   (1000) classic   (1000)    22234 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/postgresql.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7348 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/ddl/sqlite.py
--rw-r--r--   0 classic   (1000) classic   (1000)       43 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/environment.py
--rw-r--r--   0 classic   (1000) classic   (1000)       41 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/migration.py
--rw-r--r--   0 classic   (1000) classic   (1000)      167 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/op.py
--rw-r--r--   0 classic   (1000) classic   (1000)    45598 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/op.pyi
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.385878 alembic-1.9.3/alembic/operations/
--rw-r--r--   0 classic   (1000) classic   (1000)      184 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    19031 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/base.py
--rw-r--r--   0 classic   (1000) classic   (1000)    26466 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/batch.py
--rw-r--r--   0 classic   (1000) classic   (1000)    89338 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/ops.py
--rw-r--r--   0 classic   (1000) classic   (1000)     9022 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/schemaobj.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6545 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/operations/toimpl.py
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/py.typed
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.386878 alembic-1.9.3/alembic/runtime/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/runtime/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    39194 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/runtime/environment.py
--rw-r--r--   0 classic   (1000) classic   (1000)    49298 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/runtime/migration.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.386878 alembic-1.9.3/alembic/script/
--rw-r--r--   0 classic   (1000) classic   (1000)      100 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/script/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)    35931 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/script/base.py
--rw-r--r--   0 classic   (1000) classic   (1000)    61333 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/script/revision.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4212 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/script/write_hooks.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.379878 alembic-1.9.3/alembic/templates/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.387879 alembic-1.9.3/alembic/templates/async/
--rw-r--r--   0 classic   (1000) classic   (1000)       58 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/async/README
--rw-r--r--   0 classic   (1000) classic   (1000)     3137 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/async/alembic.ini.mako
--rw-r--r--   0 classic   (1000) classic   (1000)     2404 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/async/env.py
--rw-r--r--   0 classic   (1000) classic   (1000)      510 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/async/script.py.mako
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.387879 alembic-1.9.3/alembic/templates/generic/
--rw-r--r--   0 classic   (1000) classic   (1000)       38 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/generic/README
--rw-r--r--   0 classic   (1000) classic   (1000)     3246 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/generic/alembic.ini.mako
--rw-r--r--   0 classic   (1000) classic   (1000)     2099 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/generic/env.py
--rw-r--r--   0 classic   (1000) classic   (1000)      510 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/generic/script.py.mako
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.388878 alembic-1.9.3/alembic/templates/multidb/
--rw-r--r--   0 classic   (1000) classic   (1000)      606 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/multidb/README
--rw-r--r--   0 classic   (1000) classic   (1000)     3340 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/multidb/alembic.ini.mako
--rw-r--r--   0 classic   (1000) classic   (1000)     4222 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/multidb/env.py
--rw-r--r--   0 classic   (1000) classic   (1000)      965 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/templates/multidb/script.py.mako
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.388878 alembic-1.9.3/alembic/testing/
--rw-r--r--   0 classic   (1000) classic   (1000)     1159 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5018 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/assertions.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10752 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/env.py
--rw-r--r--   0 classic   (1000) classic   (1000)     9180 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/fixtures.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.389878 alembic-1.9.3/alembic/testing/plugin/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/plugin/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)       50 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/plugin/bootstrap.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4954 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/requirements.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4373 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/schemacompare.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.390879 alembic-1.9.3/alembic/testing/suite/
--rw-r--r--   0 classic   (1000) classic   (1000)      288 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     9881 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/_autogen_fixtures.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6283 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_autogen_comments.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6077 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_autogen_computed.py
--rw-r--r--   0 classic   (1000) classic   (1000)     8394 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_autogen_diffs.py
--rw-r--r--   0 classic   (1000) classic   (1000)    32927 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_autogen_fks.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6088 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_autogen_identity.py
--rw-r--r--   0 classic   (1000) classic   (1000)    11877 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_environment.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1343 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/suite/test_op.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3323 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/util.py
--rw-r--r--   0 classic   (1000) classic   (1000)      831 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/testing/warnings.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.390879 alembic-1.9.3/alembic/util/
--rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1701 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/compat.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2546 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/editor.py
--rw-r--r--   0 classic   (1000) classic   (1000)       98 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/exc.py
--rw-r--r--   0 classic   (1000) classic   (1000)     8517 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/langhelpers.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2853 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/messaging.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3374 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/pyfiles.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16348 2023-02-07 20:46:41.000000 alembic-1.9.3/alembic/util/sqla_compat.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.383878 alembic-1.9.3/alembic.egg-info/
--rw-r--r--   0 classic   (1000) classic   (1000)     6967 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/PKG-INFO
--rw-r--r--   0 classic   (1000) classic   (1000)     5788 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/SOURCES.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/dependency_links.txt
--rw-r--r--   0 classic   (1000) classic   (1000)       48 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/entry_points.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/not-zip-safe
--rw-r--r--   0 classic   (1000) classic   (1000)      111 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/requires.txt
--rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-02-07 20:47:19.000000 alembic-1.9.3/alembic.egg-info/top_level.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.393879 alembic-1.9.3/docs/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.393879 alembic-1.9.3/docs/_images/
--rw-r--r--   0 classic   (1000) classic   (1000)   123965 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_images/api_overview.png
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.395878 alembic-1.9.3/docs/_sources/
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.396879 alembic-1.9.3/docs/_sources/api/
--rw-r--r--   0 classic   (1000) classic   (1000)    24992 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/autogenerate.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1721 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/commands.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1232 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/config.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1090 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/ddl.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1013 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/index.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     6413 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/operations.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     3409 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/overview.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1505 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/runtime.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/api/script.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    38841 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/autogenerate.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    18671 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/batch.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    35227 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/branches.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)   192225 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/changelog.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    59179 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/cookbook.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     3904 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/front.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/index.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    10947 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/naming.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     5620 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/offline.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)     1961 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/ops.rst.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    26298 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_sources/tutorial.rst.txt
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.398879 alembic-1.9.3/docs/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/basic.css
--rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/changelog.css
--rw-r--r--   0 classic   (1000) classic   (1000)     9031 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/clipboard.min.js
--rw-r--r--   0 classic   (1000) classic   (1000)     2060 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/copybutton.css
--rw-r--r--   0 classic   (1000) classic   (1000)     8534 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/copybutton.js
--rw-r--r--   0 classic   (1000) classic   (1000)     2698 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/copybutton_funcs.js
--rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/doctools.js
--rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/documentation_options.js
--rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/file.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/language_data.js
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/minus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/nature.css
--rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/plus.png
--rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/pygments.css
--rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/searchtools.js
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/site_custom_css.css
--rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/sphinx_highlight.js
--rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/_static/sphinx_paramlinks.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.400879 alembic-1.9.3/docs/api/
--rw-r--r--   0 classic   (1000) classic   (1000)   140328 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/autogenerate.html
--rw-r--r--   0 classic   (1000) classic   (1000)    69822 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/commands.html
--rw-r--r--   0 classic   (1000) classic   (1000)    49475 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/config.html
--rw-r--r--   0 classic   (1000) classic   (1000)   274408 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/ddl.html
--rw-r--r--   0 classic   (1000) classic   (1000)    18869 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)   236384 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/operations.html
--rw-r--r--   0 classic   (1000) classic   (1000)    13402 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/overview.html
--rw-r--r--   0 classic   (1000) classic   (1000)   183554 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/runtime.html
--rw-r--r--   0 classic   (1000) classic   (1000)   109535 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/api/script.html
--rw-r--r--   0 classic   (1000) classic   (1000)   102084 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/autogenerate.html
--rw-r--r--   0 classic   (1000) classic   (1000)    51306 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/batch.html
--rw-r--r--   0 classic   (1000) classic   (1000)    67267 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/branches.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.401879 alembic-1.9.3/docs/build/
--rw-r--r--   0 classic   (1000) classic   (1000)     3560 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/Makefile
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.401879 alembic-1.9.3/docs/build/_static/
--rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/_static/nature_override.css
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/_static/site_custom_css.css
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.402879 alembic-1.9.3/docs/build/_templates/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/_templates/site_custom_sidebars.html
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.403879 alembic-1.9.3/docs/build/api/
--rw-r--r--   0 classic   (1000) classic   (1000)   123965 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/api_overview.png
--rw-r--r--   0 classic   (1000) classic   (1000)    24992 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/autogenerate.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1721 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/commands.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1232 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/config.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1090 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/ddl.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1013 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     6413 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/operations.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     3409 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/overview.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1505 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/runtime.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/api/script.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    38841 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/autogenerate.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    18671 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/batch.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    35227 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/branches.rst
--rw-------   0 classic   (1000) classic   (1000)   192225 2023-02-07 20:47:07.000000 alembic-1.9.3/docs/build/changelog.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     7894 2023-02-07 20:47:07.000000 alembic-1.9.3/docs/build/conf.py
--rw-r--r--   0 classic   (1000) classic   (1000)    59179 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/cookbook.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     3904 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/front.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/index.rst
--rw-r--r--   0 classic   (1000) classic   (1000)    10947 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/naming.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     5620 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/offline.rst
--rw-r--r--   0 classic   (1000) classic   (1000)     1961 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/ops.rst
--rw-r--r--   0 classic   (1000) classic   (1000)      360 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/requirements.txt
--rw-r--r--   0 classic   (1000) classic   (1000)    26298 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/tutorial.rst
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.403879 alembic-1.9.3/docs/build/unreleased/
--rw-r--r--   0 classic   (1000) classic   (1000)      413 2023-02-07 20:46:41.000000 alembic-1.9.3/docs/build/unreleased/README.txt
--rw-r--r--   0 classic   (1000) classic   (1000)   478184 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/changelog.html
--rw-r--r--   0 classic   (1000) classic   (1000)   168994 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/cookbook.html
--rw-r--r--   0 classic   (1000) classic   (1000)    12179 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/front.html
--rw-r--r--   0 classic   (1000) classic   (1000)   103755 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/genindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)    71764 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/index.html
--rw-r--r--   0 classic   (1000) classic   (1000)    38874 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/naming.html
--rw-r--r--   0 classic   (1000) classic   (1000)    19784 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/offline.html
--rw-r--r--   0 classic   (1000) classic   (1000)   263313 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/ops.html
--rw-r--r--   0 classic   (1000) classic   (1000)     7332 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/py-modindex.html
--rw-r--r--   0 classic   (1000) classic   (1000)     3671 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/search.html
--rw-r--r--   0 classic   (1000) classic   (1000)   166765 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/searchindex.js
--rw-r--r--   0 classic   (1000) classic   (1000)    56154 2023-02-07 20:47:18.000000 alembic-1.9.3/docs/tutorial.html
--rw-r--r--   0 classic   (1000) classic   (1000)      532 2023-02-07 20:46:41.000000 alembic-1.9.3/pyproject.toml
--rw-r--r--   0 classic   (1000) classic   (1000)     3189 2023-02-07 20:47:19.408879 alembic-1.9.3/setup.cfg
--rw-r--r--   0 classic   (1000) classic   (1000)      197 2023-02-07 20:46:41.000000 alembic-1.9.3/setup.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.407879 alembic-1.9.3/tests/
--rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/__init__.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7317 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/_large_map.py
--rwxr-xr-x   0 classic   (1000) classic   (1000)     1253 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/conftest.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13253 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/requirements.py
--rw-r--r--   0 classic   (1000) classic   (1000)    16494 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_autogen_composition.py
--rw-r--r--   0 classic   (1000) classic   (1000)    59970 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_autogen_diffs.py
--rw-r--r--   0 classic   (1000) classic   (1000)    46196 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_autogen_indexes.py
--rw-r--r--   0 classic   (1000) classic   (1000)    86197 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_autogen_render.py
--rw-r--r--   0 classic   (1000) classic   (1000)    86204 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_batch.py
--rw-r--r--   0 classic   (1000) classic   (1000)    10399 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_bulk_insert.py
--rw-r--r--   0 classic   (1000) classic   (1000)    43675 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_command.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7536 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_config.py
--rw-r--r--   0 classic   (1000) classic   (1000)     3844 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_editor.py
--rw-r--r--   0 classic   (1000) classic   (1000)     5142 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_environment.py
--rw-r--r--   0 classic   (1000) classic   (1000)     4095 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_external_dialect.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1296 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_impl.py
--rw-r--r--   0 classic   (1000) classic   (1000)    18388 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_mssql.py
--rw-r--r--   0 classic   (1000) classic   (1000)    22164 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_mysql.py
--rw-r--r--   0 classic   (1000) classic   (1000)     9782 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_offline_environment.py
--rw-r--r--   0 classic   (1000) classic   (1000)    46265 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_op.py
--rw-r--r--   0 classic   (1000) classic   (1000)     6194 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_op_naming_convention.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13259 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_oracle.py
--rw-r--r--   0 classic   (1000) classic   (1000)     7350 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_post_write.py
--rw-r--r--   0 classic   (1000) classic   (1000)    42929 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_postgresql.py
--rw-r--r--   0 classic   (1000) classic   (1000)    50768 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_revision.py
--rw-r--r--   0 classic   (1000) classic   (1000)    25938 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_script_consumption.py
--rw-r--r--   0 classic   (1000) classic   (1000)    43659 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_script_production.py
--rw-r--r--   0 classic   (1000) classic   (1000)     8995 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_sqlite.py
--rw-r--r--   0 classic   (1000) classic   (1000)     1347 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_stubs.py
--rw-r--r--   0 classic   (1000) classic   (1000)       44 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_suite.py
--rw-r--r--   0 classic   (1000) classic   (1000)    13640 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_version_table.py
--rw-r--r--   0 classic   (1000) classic   (1000)    46215 2023-02-07 20:46:41.000000 alembic-1.9.3/tests/test_version_traversal.py
-drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-07 20:47:19.407879 alembic-1.9.3/tools/
--rw-r--r--   0 classic   (1000) classic   (1000)     8812 2023-02-07 20:46:41.000000 alembic-1.9.3/tools/write_pyi.py
--rw-r--r--   0 classic   (1000) classic   (1000)     2736 2023-02-07 20:46:41.000000 alembic-1.9.3/tox.ini
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.869006 alembic-1.9.4/
+-rw-r--r--   0 classic   (1000) classic   (1000)      178 2023-02-16 17:35:04.000000 alembic-1.9.4/CHANGES
+-rw-r--r--   0 classic   (1000) classic   (1000)     1058 2023-02-16 17:35:04.000000 alembic-1.9.4/LICENSE
+-rw-r--r--   0 classic   (1000) classic   (1000)      330 2023-02-16 17:35:04.000000 alembic-1.9.4/MANIFEST.in
+-rw-r--r--   0 classic   (1000) classic   (1000)     6967 2023-02-16 17:35:43.869006 alembic-1.9.4/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     5736 2023-02-16 17:35:04.000000 alembic-1.9.4/README.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    15001 2023-02-16 17:35:04.000000 alembic-1.9.4/README.unittests.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.840005 alembic-1.9.4/alembic/
+-rw-r--r--   0 classic   (1000) classic   (1000)       74 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       78 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/__main__.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.841005 alembic-1.9.4/alembic/autogenerate/
+-rw-r--r--   0 classic   (1000) classic   (1000)      351 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/autogenerate/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20558 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/autogenerate/api.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    45836 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/autogenerate/compare.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    34698 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/autogenerate/render.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7466 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/autogenerate/rewriter.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    21075 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/command.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    20645 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/config.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      195 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/context.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    28807 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/context.pyi
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.842005 alembic-1.9.4/alembic/ddl/
+-rw-r--r--   0 classic   (1000) classic   (1000)      137 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     9590 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/base.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    22926 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/impl.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13639 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/mssql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16322 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/mysql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6092 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/oracle.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    22338 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/postgresql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7348 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/ddl/sqlite.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       43 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/environment.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       41 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/migration.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      167 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/op.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    45598 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/op.pyi
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.843006 alembic-1.9.4/alembic/operations/
+-rw-r--r--   0 classic   (1000) classic   (1000)      184 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    19031 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/base.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    26466 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/batch.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    89337 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/ops.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     9022 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/schemaobj.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6545 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/operations/toimpl.py
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/py.typed
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.843006 alembic-1.9.4/alembic/runtime/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/runtime/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    39194 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/runtime/environment.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    49298 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/runtime/migration.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.844005 alembic-1.9.4/alembic/script/
+-rw-r--r--   0 classic   (1000) classic   (1000)      100 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/script/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    35931 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/script/base.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    61333 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/script/revision.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4212 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/script/write_hooks.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.836005 alembic-1.9.4/alembic/templates/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.844005 alembic-1.9.4/alembic/templates/async/
+-rw-r--r--   0 classic   (1000) classic   (1000)       58 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/async/README
+-rw-r--r--   0 classic   (1000) classic   (1000)     3137 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/async/alembic.ini.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)     2389 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/async/env.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      510 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/async/script.py.mako
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.845005 alembic-1.9.4/alembic/templates/generic/
+-rw-r--r--   0 classic   (1000) classic   (1000)       38 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/generic/README
+-rw-r--r--   0 classic   (1000) classic   (1000)     3246 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/generic/alembic.ini.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)     2103 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/generic/env.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      510 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/generic/script.py.mako
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.845005 alembic-1.9.4/alembic/templates/multidb/
+-rw-r--r--   0 classic   (1000) classic   (1000)      606 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/multidb/README
+-rw-r--r--   0 classic   (1000) classic   (1000)     3340 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/multidb/alembic.ini.mako
+-rw-r--r--   0 classic   (1000) classic   (1000)     4230 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/multidb/env.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      965 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/templates/multidb/script.py.mako
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.846006 alembic-1.9.4/alembic/testing/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1159 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5018 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/assertions.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10752 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/env.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     9180 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/fixtures.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.847005 alembic-1.9.4/alembic/testing/plugin/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/plugin/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       50 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/plugin/bootstrap.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4954 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/requirements.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4373 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/schemacompare.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.848005 alembic-1.9.4/alembic/testing/suite/
+-rw-r--r--   0 classic   (1000) classic   (1000)      288 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     9881 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/_autogen_fixtures.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6283 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_autogen_comments.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6077 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_autogen_computed.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     8394 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_autogen_diffs.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    32927 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_autogen_fks.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6088 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_autogen_identity.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    11877 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_environment.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1343 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/suite/test_op.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3323 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/util.py
+-rw-r--r--   0 classic   (1000) classic   (1000)      831 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/testing/warnings.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.850005 alembic-1.9.4/alembic/util/
+-rw-r--r--   0 classic   (1000) classic   (1000)     1167 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1701 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/compat.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2546 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/editor.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       98 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/exc.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     8517 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/langhelpers.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2853 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/messaging.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3374 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/pyfiles.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16348 2023-02-16 17:35:04.000000 alembic-1.9.4/alembic/util/sqla_compat.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.840005 alembic-1.9.4/alembic.egg-info/
+-rw-r--r--   0 classic   (1000) classic   (1000)     6967 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/PKG-INFO
+-rw-r--r--   0 classic   (1000) classic   (1000)     5788 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/SOURCES.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/dependency_links.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)       48 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/entry_points.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        1 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/not-zip-safe
+-rw-r--r--   0 classic   (1000) classic   (1000)      111 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/requires.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)        8 2023-02-16 17:35:43.000000 alembic-1.9.4/alembic.egg-info/top_level.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.853006 alembic-1.9.4/docs/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.853006 alembic-1.9.4/docs/_images/
+-rw-r--r--   0 classic   (1000) classic   (1000)   123965 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_images/api_overview.png
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.854005 alembic-1.9.4/docs/_sources/
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.855006 alembic-1.9.4/docs/_sources/api/
+-rw-r--r--   0 classic   (1000) classic   (1000)    24992 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/autogenerate.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1721 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/commands.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1232 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/config.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1090 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/ddl.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1013 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     6413 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/operations.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     3409 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/overview.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1505 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/runtime.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/api/script.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    38841 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/autogenerate.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    18671 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/batch.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    35227 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/branches.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)   193821 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/changelog.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    58381 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/cookbook.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     3904 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/front.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/index.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    10947 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/naming.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     5620 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/offline.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)     1961 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/ops.rst.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    26298 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_sources/tutorial.rst.txt
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.857006 alembic-1.9.4/docs/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)    14813 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/basic.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      107 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/changelog.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     9031 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/clipboard.min.js
+-rw-r--r--   0 classic   (1000) classic   (1000)     2060 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/copybutton.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     8529 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/copybutton.js
+-rw-r--r--   0 classic   (1000) classic   (1000)     2698 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/copybutton_funcs.js
+-rw-r--r--   0 classic   (1000) classic   (1000)     4472 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/doctools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      420 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/documentation_options.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      286 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/file.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4758 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/language_data.js
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/minus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4208 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/nature.css
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)       90 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/plus.png
+-rw-r--r--   0 classic   (1000) classic   (1000)     4846 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/pygments.css
+-rw-r--r--   0 classic   (1000) classic   (1000)    18215 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/searchtools.js
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/site_custom_css.css
+-rw-r--r--   0 classic   (1000) classic   (1000)     4712 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 classic   (1000) classic   (1000)      204 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/_static/sphinx_paramlinks.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.859006 alembic-1.9.4/docs/api/
+-rw-r--r--   0 classic   (1000) classic   (1000)   140328 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/autogenerate.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    69822 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/commands.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    50041 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/config.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   274408 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/ddl.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    18869 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   236384 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/operations.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    13402 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/overview.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   183554 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/runtime.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   109535 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/api/script.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   102084 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/autogenerate.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    51306 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/batch.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    67267 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/branches.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.862006 alembic-1.9.4/docs/build/
+-rw-r--r--   0 classic   (1000) classic   (1000)     3560 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/Makefile
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.862006 alembic-1.9.4/docs/build/_static/
+-rw-r--r--   0 classic   (1000) classic   (1000)      507 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/_static/nature_override.css
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/_static/site_custom_css.css
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.862006 alembic-1.9.4/docs/build/_templates/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/_templates/site_custom_sidebars.html
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.864006 alembic-1.9.4/docs/build/api/
+-rw-r--r--   0 classic   (1000) classic   (1000)   123965 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/api_overview.png
+-rw-r--r--   0 classic   (1000) classic   (1000)    24992 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/autogenerate.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1721 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/commands.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1232 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/config.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1090 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/ddl.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1013 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     6413 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/operations.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     3409 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/overview.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1505 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/runtime.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/api/script.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    38841 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/autogenerate.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    18671 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/batch.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    35227 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/branches.rst
+-rw-------   0 classic   (1000) classic   (1000)   193821 2023-02-16 17:35:31.000000 alembic-1.9.4/docs/build/changelog.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     8077 2023-02-16 17:35:31.000000 alembic-1.9.4/docs/build/conf.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    58381 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/cookbook.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     3904 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/front.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      533 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/index.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)    10947 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/naming.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     5620 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/offline.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)     1961 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/ops.rst
+-rw-r--r--   0 classic   (1000) classic   (1000)      367 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/requirements.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)    26298 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/tutorial.rst
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.864006 alembic-1.9.4/docs/build/unreleased/
+-rw-r--r--   0 classic   (1000) classic   (1000)      413 2023-02-16 17:35:04.000000 alembic-1.9.4/docs/build/unreleased/README.txt
+-rw-r--r--   0 classic   (1000) classic   (1000)   481900 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/changelog.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   166309 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/cookbook.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    12179 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/front.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   103838 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/genindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    71983 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/index.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    38874 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/naming.html
+-rw-r--r--   0 classic   (1000) classic   (1000)    19784 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/offline.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   263310 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/ops.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     7332 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/py-modindex.html
+-rw-r--r--   0 classic   (1000) classic   (1000)     3671 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/search.html
+-rw-r--r--   0 classic   (1000) classic   (1000)   166959 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/searchindex.js
+-rw-r--r--   0 classic   (1000) classic   (1000)    56154 2023-02-16 17:35:43.000000 alembic-1.9.4/docs/tutorial.html
+-rw-r--r--   0 classic   (1000) classic   (1000)      532 2023-02-16 17:35:04.000000 alembic-1.9.4/pyproject.toml
+-rw-r--r--   0 classic   (1000) classic   (1000)     3189 2023-02-16 17:35:43.870006 alembic-1.9.4/setup.cfg
+-rw-r--r--   0 classic   (1000) classic   (1000)      197 2023-02-16 17:35:04.000000 alembic-1.9.4/setup.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.869006 alembic-1.9.4/tests/
+-rw-r--r--   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/__init__.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7317 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/_large_map.py
+-rwxr-xr-x   0 classic   (1000) classic   (1000)     1253 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/conftest.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13253 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/requirements.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    16494 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_autogen_composition.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    61012 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_autogen_diffs.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    46196 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_autogen_indexes.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    86197 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_autogen_render.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    86204 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_batch.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    10399 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_bulk_insert.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    43675 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_command.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7536 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_config.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     3844 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_editor.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     5142 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_environment.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     4095 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_external_dialect.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1296 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_impl.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    18388 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_mssql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    22164 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_mysql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     9782 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_offline_environment.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    46265 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_op.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     6194 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_op_naming_convention.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13259 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_oracle.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     7350 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_post_write.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    42929 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_postgresql.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    50768 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_revision.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    25938 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_script_consumption.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    43659 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_script_production.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     8995 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_sqlite.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     1347 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_stubs.py
+-rw-r--r--   0 classic   (1000) classic   (1000)       44 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_suite.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    13640 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_version_table.py
+-rw-r--r--   0 classic   (1000) classic   (1000)    46215 2023-02-16 17:35:04.000000 alembic-1.9.4/tests/test_version_traversal.py
+drwxr-xr-x   0 classic   (1000) classic   (1000)        0 2023-02-16 17:35:43.869006 alembic-1.9.4/tools/
+-rw-r--r--   0 classic   (1000) classic   (1000)     8812 2023-02-16 17:35:04.000000 alembic-1.9.4/tools/write_pyi.py
+-rw-r--r--   0 classic   (1000) classic   (1000)     2736 2023-02-16 17:35:04.000000 alembic-1.9.4/tox.ini
```

### Comparing `alembic-1.9.3/LICENSE` & `alembic-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/PKG-INFO` & `alembic-1.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic
-Version: 1.9.3
+Version: 1.9.4
 Summary: A database migration tool for SQLAlchemy.
 Home-page: https://alembic.sqlalchemy.org
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Source, https://github.com/sqlalchemy/alembic/
 Project-URL: Documentation, https://alembic.sqlalchemy.org/en/latest/
```

### Comparing `alembic-1.9.3/README.rst` & `alembic-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/README.unittests.rst` & `alembic-1.9.4/README.unittests.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/autogenerate/api.py` & `alembic-1.9.4/alembic/autogenerate/api.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/autogenerate/compare.py` & `alembic-1.9.4/alembic/autogenerate/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 from sqlalchemy import event
 from sqlalchemy import inspect
 from sqlalchemy import schema as sa_schema
 from sqlalchemy import types as sqltypes
 from sqlalchemy.util import OrderedSet
 
 from alembic.ddl.base import _fk_spec
-from .render import _user_defined_render
 from .. import util
 from ..operations import ops
 from ..util import sqla_compat
 
 if TYPE_CHECKING:
     from typing import Literal
 
@@ -999,19 +998,14 @@
 
 
 def _render_server_default_for_compare(
     metadata_default: Optional[Any],
     metadata_col: Column,
     autogen_context: AutogenContext,
 ) -> Optional[str]:
-    rendered = _user_defined_render(
-        "server_default", metadata_default, autogen_context
-    )
-    if rendered is not False:
-        return rendered
 
     if isinstance(metadata_default, sa_schema.DefaultClause):
         if isinstance(metadata_default.arg, str):
             metadata_default = metadata_default.arg
         else:
             metadata_default = str(
                 metadata_default.arg.compile(
```

### Comparing `alembic-1.9.3/alembic/autogenerate/render.py` & `alembic-1.9.4/alembic/autogenerate/render.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/autogenerate/rewriter.py` & `alembic-1.9.4/alembic/autogenerate/rewriter.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/command.py` & `alembic-1.9.4/alembic/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -318,15 +318,15 @@
 
         :ref:`branches`
 
     """
 
     script = ScriptDirectory.from_config(config)
     template_args = {
-        "config": "config"  # Let templates use config for
+        "config": config  # Let templates use config for
         # e.g. multiple databases
     }
     return script.generate_revision(
         rev_id or util.rev_id(),
         message,
         refresh=True,
         head=revisions,
```

### Comparing `alembic-1.9.3/alembic/config.py` & `alembic-1.9.4/alembic/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import inspect
 import os
 import sys
 from typing import Dict
 from typing import Optional
 from typing import overload
 from typing import TextIO
+from typing import Union
 
 from . import __version__
 from . import command
 from . import util
 from .util import compat
 
 
@@ -89,15 +90,15 @@
 
         :ref:`connection_sharing`
 
     """
 
     def __init__(
         self,
-        file_: Optional[str] = None,
+        file_: Union[str, os.PathLike[str], None] = None,
         ini_section: str = "alembic",
         output_buffer: Optional[TextIO] = None,
         stdout: TextIO = sys.stdout,
         cmd_opts: Optional[Namespace] = None,
         config_args: util.immutabledict = util.immutabledict(),
         attributes: Optional[dict] = None,
     ) -> None:
@@ -119,15 +120,15 @@
 
     .. seealso::
 
         :meth:`.EnvironmentContext.get_x_argument`
 
     """
 
-    config_file_name: Optional[str] = None
+    config_file_name: Union[str, os.PathLike[str], None] = None
     """Filesystem path to the .ini file in use."""
 
     config_ini_section: str = None  # type:ignore[assignment]
     """Name of the config file section to read basic configuration
     from.  Defaults to ``alembic``, that is the ``[alembic]`` section
     of the .ini file.  This value is modified using the ``-n/--name``
     option to the Alembic runner.
```

### Comparing `alembic-1.9.3/alembic/context.pyi` & `alembic-1.9.4/alembic/context.pyi`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/ddl/base.py` & `alembic-1.9.4/alembic/ddl/base.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/ddl/impl.py` & `alembic-1.9.4/alembic/ddl/impl.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/ddl/mssql.py` & `alembic-1.9.4/alembic/ddl/mssql.py`

 * *Files 1% similar despite different names*

```diff
@@ -229,34 +229,25 @@
         inspector_column,
         metadata_column,
         rendered_metadata_default,
         rendered_inspector_default,
     ):
 
         if rendered_metadata_default is not None:
-            rendered_metadata_default = re.sub(
-                r"^\((.+)\)$", r"\1", rendered_metadata_default
-            )
 
             rendered_metadata_default = re.sub(
-                r"^\"?'(.+)'\"?$", r"\1", rendered_metadata_default
+                r"[\(\) \"\']", "", rendered_metadata_default
             )
 
         if rendered_inspector_default is not None:
-
-            # the iteration is a quick hack to remove balanced parens only
-            # up to two levels deep, like ((foo)) but not (foo())
-            # see issue #1152
-            for i in range(2):
-                rendered_inspector_default = re.sub(
-                    r"^\((.+)\)$", r"\1", rendered_inspector_default
-                )
+            # SQL Server collapses whitespace and adds arbitrary parenthesis
+            # within expressions.   our only option is collapse all of it
 
             rendered_inspector_default = re.sub(
-                r"^\"?'(.+)'\"?$", r"\1", rendered_inspector_default
+                r"[\(\) \"\']", "", rendered_inspector_default
             )
 
         return rendered_inspector_default != rendered_metadata_default
 
     def _compare_identity_default(self, metadata_identity, inspector_identity):
         diff, ignored, is_alter = super()._compare_identity_default(
             metadata_identity, inspector_identity
```

### Comparing `alembic-1.9.3/alembic/ddl/mysql.py` & `alembic-1.9.4/alembic/ddl/mysql.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/ddl/oracle.py` & `alembic-1.9.4/alembic/ddl/oracle.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/ddl/postgresql.py` & `alembic-1.9.4/alembic/ddl/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from typing import Optional
 from typing import Sequence
 from typing import Tuple
 from typing import TYPE_CHECKING
 from typing import Union
 
 from sqlalchemy import Column
+from sqlalchemy import literal_column
 from sqlalchemy import Numeric
 from sqlalchemy import text
 from sqlalchemy import types as sqltypes
 from sqlalchemy.dialects.postgresql import BIGINT
 from sqlalchemy.dialects.postgresql import ExcludeConstraint
 from sqlalchemy.dialects.postgresql import INTEGER
 from sqlalchemy.schema import CreateIndex
@@ -108,30 +109,34 @@
 
         conn_col_default = rendered_inspector_default
 
         defaults_equal = conn_col_default == rendered_metadata_default
         if defaults_equal:
             return False
 
-        if None in (conn_col_default, rendered_metadata_default):
+        if None in (
+            conn_col_default,
+            rendered_metadata_default,
+            metadata_column.server_default,
+        ):
             return not defaults_equal
 
-        # check for unquoted string and quote for PG String types
-        if (
-            not isinstance(inspector_column.type, Numeric)
-            and metadata_column.server_default is not None
-            and isinstance(metadata_column.server_default.arg, str)
-            and not re.match(r"^'.*'$", rendered_metadata_default)
-        ):
-            rendered_metadata_default = "'%s'" % rendered_metadata_default
+        metadata_default = metadata_column.server_default.arg
+
+        if isinstance(metadata_default, str):
+            if not isinstance(inspector_column.type, Numeric):
+                metadata_default = re.sub(r"^'|'$", "", metadata_default)
+                metadata_default = f"'{metadata_default}'"
+
+            metadata_default = literal_column(metadata_default)
 
+        # run a real compare against the server
         return not self.connection.scalar(
-            text(
-                "SELECT %s = %s"
-                % (conn_col_default, rendered_metadata_default)
+            sqla_compat._select(
+                literal_column(conn_col_default) == metadata_default
             )
         )
 
     def alter_column(  # type:ignore[override]
         self,
         table_name: str,
         column_name: str,
```

### Comparing `alembic-1.9.3/alembic/ddl/sqlite.py` & `alembic-1.9.4/alembic/ddl/sqlite.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/op.pyi` & `alembic-1.9.4/alembic/op.pyi`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/operations/base.py` & `alembic-1.9.4/alembic/operations/base.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/operations/batch.py` & `alembic-1.9.4/alembic/operations/batch.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/operations/ops.py` & `alembic-1.9.4/alembic/operations/ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1908,15 +1908,15 @@
         as well as the following option(s):
 
         :param insert_before: String name of an existing column which this
          column should be placed before, when creating the new table.
 
          .. versionadded:: 1.4.0
 
-        :param insert_before: String name of an existing column which this
+        :param insert_after: String name of an existing column which this
          column should be placed after, when creating the new table.  If
          both :paramref:`.BatchOperations.alter_column.insert_before`
          and :paramref:`.BatchOperations.alter_column.insert_after` are
          omitted, the column is inserted after the last existing column
          in the table.
 
          .. versionadded:: 1.4.0
```

### Comparing `alembic-1.9.3/alembic/operations/schemaobj.py` & `alembic-1.9.4/alembic/operations/schemaobj.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/operations/toimpl.py` & `alembic-1.9.4/alembic/operations/toimpl.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/runtime/environment.py` & `alembic-1.9.4/alembic/runtime/environment.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/runtime/migration.py` & `alembic-1.9.4/alembic/runtime/migration.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/script/base.py` & `alembic-1.9.4/alembic/script/base.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/script/revision.py` & `alembic-1.9.4/alembic/script/revision.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/script/write_hooks.py` & `alembic-1.9.4/alembic/script/write_hooks.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/templates/async/alembic.ini.mako` & `alembic-1.9.4/alembic/templates/async/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/templates/async/env.py` & `alembic-1.9.4/alembic/templates/async/env.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 from logging.config import fileConfig
 
-from sqlalchemy import engine_from_config
 from sqlalchemy import pool
 from sqlalchemy.engine import Connection
-from sqlalchemy.ext.asyncio import AsyncEngine
+from sqlalchemy.ext.asyncio import async_engine_from_config
 
 from alembic import context
 
 # this is the Alembic Config object, which provides
 # access to the values within the .ini file in use.
 config = context.config
 
@@ -56,33 +55,35 @@
 def do_run_migrations(connection: Connection) -> None:
     context.configure(connection=connection, target_metadata=target_metadata)
 
     with context.begin_transaction():
         context.run_migrations()
 
 
-async def run_migrations_online() -> None:
-    """Run migrations in 'online' mode.
-
-    In this scenario we need to create an Engine
+async def run_async_migrations() -> None:
+    """In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
-    connectable = AsyncEngine(
-        engine_from_config(
-            config.get_section(config.config_ini_section),
-            prefix="sqlalchemy.",
-            poolclass=pool.NullPool,
-            future=True,
-        )
+
+    connectable = async_engine_from_config(
+        config.get_section(config.config_ini_section, {}),
+        prefix="sqlalchemy.",
+        poolclass=pool.NullPool,
     )
 
     async with connectable.connect() as connection:
         await connection.run_sync(do_run_migrations)
 
     await connectable.dispose()
 
 
+def run_migrations_online() -> None:
+    """Run migrations in 'online' mode."""
+
+    asyncio.run(run_async_migrations())
+
+
 if context.is_offline_mode():
     run_migrations_offline()
 else:
-    asyncio.run(run_migrations_online())
+    run_migrations_online()
```

### Comparing `alembic-1.9.3/alembic/templates/generic/alembic.ini.mako` & `alembic-1.9.4/alembic/templates/generic/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/templates/generic/env.py` & `alembic-1.9.4/alembic/templates/generic/env.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     """Run migrations in 'online' mode.
 
     In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
     connectable = engine_from_config(
-        config.get_section(config.config_ini_section),
+        config.get_section(config.config_ini_section, {}),
         prefix="sqlalchemy.",
         poolclass=pool.NullPool,
     )
 
     with connectable.connect() as connection:
         context.configure(
             connection=connection, target_metadata=target_metadata
```

### Comparing `alembic-1.9.3/alembic/templates/multidb/README` & `alembic-1.9.4/alembic/templates/multidb/README`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/templates/multidb/alembic.ini.mako` & `alembic-1.9.4/alembic/templates/multidb/alembic.ini.mako`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/templates/multidb/env.py` & `alembic-1.9.4/alembic/templates/multidb/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 if config.config_file_name is not None:
     fileConfig(config.config_file_name)
 logger = logging.getLogger("alembic.env")
 
 # gather section names referring to different
 # databases.  These are named "engine1", "engine2"
 # in the sample .ini file.
-db_names = config.get_main_option("databases")
+db_names = config.get_main_option("databases", "")
 
 # add your model's MetaData objects here
 # for 'autogenerate' support.  These must be set
 # up to hold just those tables targeting a
 # particular database. table.tometadata() may be
 # helpful here in case a "copy" of
 # a MetaData is needed.
@@ -90,15 +90,15 @@
     # for the direct-to-DB use case, start a transaction on all
     # engines, then run all migrations, then commit all transactions.
 
     engines = {}
     for name in re.split(r",\s*", db_names):
         engines[name] = rec = {}
         rec["engine"] = engine_from_config(
-            context.config.get_section(name),
+            context.config.get_section(name, {}),
             prefix="sqlalchemy.",
             poolclass=pool.NullPool,
         )
 
     for name, rec in engines.items():
         engine = rec["engine"]
         rec["connection"] = conn = engine.connect()
```

### Comparing `alembic-1.9.3/alembic/templates/multidb/script.py.mako` & `alembic-1.9.4/alembic/templates/multidb/script.py.mako`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/__init__.py` & `alembic-1.9.4/alembic/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/assertions.py` & `alembic-1.9.4/alembic/testing/assertions.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/env.py` & `alembic-1.9.4/alembic/testing/env.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/fixtures.py` & `alembic-1.9.4/alembic/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/requirements.py` & `alembic-1.9.4/alembic/testing/requirements.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/schemacompare.py` & `alembic-1.9.4/alembic/testing/schemacompare.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/_autogen_fixtures.py` & `alembic-1.9.4/alembic/testing/suite/_autogen_fixtures.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_autogen_comments.py` & `alembic-1.9.4/alembic/testing/suite/test_autogen_comments.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_autogen_computed.py` & `alembic-1.9.4/alembic/testing/suite/test_autogen_computed.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_autogen_diffs.py` & `alembic-1.9.4/alembic/testing/suite/test_autogen_diffs.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_autogen_fks.py` & `alembic-1.9.4/alembic/testing/suite/test_autogen_fks.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_autogen_identity.py` & `alembic-1.9.4/alembic/testing/suite/test_autogen_identity.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_environment.py` & `alembic-1.9.4/alembic/testing/suite/test_environment.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/suite/test_op.py` & `alembic-1.9.4/alembic/testing/suite/test_op.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/util.py` & `alembic-1.9.4/alembic/testing/util.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/testing/warnings.py` & `alembic-1.9.4/alembic/testing/warnings.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/__init__.py` & `alembic-1.9.4/alembic/util/__init__.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/compat.py` & `alembic-1.9.4/alembic/util/compat.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/editor.py` & `alembic-1.9.4/alembic/util/editor.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/langhelpers.py` & `alembic-1.9.4/alembic/util/langhelpers.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/messaging.py` & `alembic-1.9.4/alembic/util/messaging.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/pyfiles.py` & `alembic-1.9.4/alembic/util/pyfiles.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic/util/sqla_compat.py` & `alembic-1.9.4/alembic/util/sqla_compat.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/alembic.egg-info/PKG-INFO` & `alembic-1.9.4/alembic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alembic
-Version: 1.9.3
+Version: 1.9.4
 Summary: A database migration tool for SQLAlchemy.
 Home-page: https://alembic.sqlalchemy.org
 Author: Mike Bayer
 Author-email: mike_mp@zzzcomputing.com
 License: MIT
 Project-URL: Source, https://github.com/sqlalchemy/alembic/
 Project-URL: Documentation, https://alembic.sqlalchemy.org/en/latest/
```

### Comparing `alembic-1.9.3/alembic.egg-info/SOURCES.txt` & `alembic-1.9.4/alembic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_images/api_overview.png` & `alembic-1.9.4/docs/_images/api_overview.png`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/autogenerate.rst.txt` & `alembic-1.9.4/docs/_sources/api/autogenerate.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/commands.rst.txt` & `alembic-1.9.4/docs/_sources/api/commands.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/config.rst.txt` & `alembic-1.9.4/docs/_sources/api/config.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/ddl.rst.txt` & `alembic-1.9.4/docs/_sources/api/ddl.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/index.rst.txt` & `alembic-1.9.4/docs/_sources/api/index.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/operations.rst.txt` & `alembic-1.9.4/docs/_sources/api/operations.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/overview.rst.txt` & `alembic-1.9.4/docs/_sources/api/overview.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/runtime.rst.txt` & `alembic-1.9.4/docs/_sources/api/runtime.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/api/script.rst.txt` & `alembic-1.9.4/docs/_sources/api/script.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/autogenerate.rst.txt` & `alembic-1.9.4/docs/_sources/autogenerate.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/batch.rst.txt` & `alembic-1.9.4/docs/_sources/batch.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/branches.rst.txt` & `alembic-1.9.4/docs/_sources/branches.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/changelog.rst.txt` & `alembic-1.9.4/docs/_sources/changelog.rst.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,57 @@
 
 ==========
 Changelog
 ==========
 
 .. changelog::
+    :version: 1.9.4
+    :released: February 16, 2023
+
+    .. change::
+        :tags: bug, mssql
+        :tickets: 1177
+
+        Ongoing fixes for SQL Server server default comparisons under autogenerate,
+        adjusting for SQL Server's collapsing of whitespace between SQL function
+        arguments when reporting on a function-based server default, as well as its
+        arbitrary addition of parenthesis within arguments; the approach has now
+        been made more aggressive by stripping the two default strings to compare
+        of all whitespace, parenthesis, and quoting characters.
+
+
+    .. change::
+        :tags: bug, postgresql
+
+        Fixed PostgreSQL server default comparison to handle SQL expressions
+        sent as ``text()`` constructs, such as ``text("substring('name', 1, 3)")``,
+        which previously would raise errors when attempting to run a server-based
+        comparison.
+
+
+
+    .. change::
+        :tags: bug, autogenerate
+        :tickets: 1180
+
+        Removed a mis-use of the
+        :paramref:`.EnvironmentContext.configure.render_item` callable where the
+        "server_default" renderer would be erroneously used within the server
+        default comparison process, which is working against SQL expressions, not
+        Python code.
+
+    .. change::
+        :tags: bug, commands
+
+        Fixed regression introduced in 1.7.0 where the "config" object passed to
+        the template context when running the :func:`.merge` command
+        programmatically failed to be correctly populated. Pull request courtesy
+        Brendan Gann.
+
+.. changelog::
     :version: 1.9.3
     :released: February 7, 2023
 
     .. change::
         :tags: bug, autogenerate
         :tickets: 1167
```

### Comparing `alembic-1.9.3/docs/_sources/cookbook.rst.txt` & `alembic-1.9.4/docs/_sources/cookbook.rst.txt`

 * *Files 3% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     from alembic import command, config
 
     cfg = config.Config("/path/to/yourapp/alembic.ini")
     with engine.begin() as connection:
         cfg.attributes['connection'] = connection
         command.upgrade(cfg, "head")
 
-Then in ``env.py``::
+Then in ``env.py`` we can update ``run_migrations_online``::
 
     def run_migrations_online():
         connectable = config.attributes.get('connection', None)
 
         if connectable is None:
             # only create Engine if we don't have a Connection
             # from the outside
@@ -1479,84 +1479,54 @@
     def do_run_migrations(connection):
         context.configure(connection=connection, target_metadata=target_metadata)
 
         with context.begin_transaction():
             context.run_migrations()
 
 
-    async def run_migrations_online():
-        """Run migrations in 'online' mode.
-
-        In this scenario we need to create an Engine
+    async def run_async_migrations():
+        """In this scenario we need to create an Engine
         and associate a connection with the context.
 
         """
+
         connectable = async_engine_from_config(
             config.get_section(config.config_ini_section),
             prefix="sqlalchemy.",
             poolclass=pool.NullPool,
         )
 
         async with connectable.connect() as connection:
             await connection.run_sync(do_run_migrations)
 
         await connectable.dispose()
 
 
-    if context.is_offline_mode():
-        run_migrations_offline()
-    else:
-        asyncio.run(run_migrations_online())
+    def run_migrations_online():
+        """Run migrations in 'online' mode."""
+
+        asyncio.run(run_async_migrations())
 
 An async application can also interact with the Alembic api directly by using
 the SQLAlchemy ``run_sync`` method to adapt the non-async api of Alembic to
 an async consumer.
 
 
 .. _connection_sharing_plus_asyncio:
 
 Programmatic API use (connection sharing) With Asyncio
 ------------------------------------------------------
 
 Combining the examples of :ref:`connection_sharing` with :ref:`asyncio_recipe`
-together, and ``env.py`` as follows works::
-
-    import asyncio
-
-    from sqlalchemy.ext.asyncio import async_engine_from_config
-
-    # ... no change required to the rest of the code
-
-
-    def do_run_migrations(connection):
-        context.configure(connection=connection, target_metadata=target_metadata)
-
-        with context.begin_transaction():
-            context.run_migrations()
-
-
-    async def run_async_migrations():
-        connectable = async_engine_from_config(
-            config.get_section(config.config_ini_section),
-            prefix="sqlalchemy.",
-            poolclass=pool.NullPool,
-        )
-
-        async with connectable.connect() as connection:
-            await connection.run_sync(do_run_migrations)
-
-        await connectable.dispose()
+together, the  ``env.py`` listed above can be updated as follows works::
 
 
     def run_migrations_online():
         """Run migrations in 'online' mode.
 
-        In this scenario we need to create an Engine
-        and associate a connection with the context.
-
         """
 
         connectable = config.attributes.get("connection", None)
 
         if connectable is None:
             asyncio.run(run_async_migrations())
         else:
```

### Comparing `alembic-1.9.3/docs/_sources/front.rst.txt` & `alembic-1.9.4/docs/_sources/front.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/index.rst.txt` & `alembic-1.9.4/docs/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/naming.rst.txt` & `alembic-1.9.4/docs/_sources/naming.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/offline.rst.txt` & `alembic-1.9.4/docs/_sources/offline.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/ops.rst.txt` & `alembic-1.9.4/docs/_sources/ops.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_sources/tutorial.rst.txt` & `alembic-1.9.4/docs/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/basic.css` & `alembic-1.9.4/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/clipboard.min.js` & `alembic-1.9.4/docs/_static/clipboard.min.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/copybutton.css` & `alembic-1.9.4/docs/_static/copybutton.css`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/copybutton.js` & `alembic-1.9.4/docs/_static/copybutton.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -222,15 +222,15 @@
     }
 
 
     var copyTargetText = (trigger) => {
         var target = document.querySelector(trigger.attributes['data-clipboard-target'].value);
 
         // get filtered text
-        let exclude = '.linenos, .gp';
+        let exclude = '.linenos';
 
         let text = filterText(target, exclude);
         return formatCopyText(text, '>>> |\\.\\.\\. |\\$ |In \\[\\d*\\]: | {2,5}\\.\\.\\.: | {5,8}: ', true, true, true, true, '', '')
     }
 
     // Initialize with a callback so we can modify the text before copy
     const clipboard = new ClipboardJS('.copybtn', {
```

### Comparing `alembic-1.9.3/docs/_static/copybutton_funcs.js` & `alembic-1.9.4/docs/_static/copybutton_funcs.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/doctools.js` & `alembic-1.9.4/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/language_data.js` & `alembic-1.9.4/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/nature.css` & `alembic-1.9.4/docs/_static/nature.css`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/pygments.css` & `alembic-1.9.4/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/searchtools.js` & `alembic-1.9.4/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/_static/sphinx_highlight.js` & `alembic-1.9.4/docs/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/api/autogenerate.html` & `alembic-1.9.4/docs/api/autogenerate.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Autogeneration &#8212; Alembic 1.9.3 documentation</title>
+    <title>Autogeneration &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="script.html" title="Script Directory"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Operation Directives"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Autogeneration</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -1044,15 +1044,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="script.html" title="Script Directory"
              >next</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Operation Directives"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Autogeneration</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Autogeneration
 ****** AutogenerationÂ¶ ******
 Note
 this section discusses the internal API of Alembic as regards the
 autogeneration feature of the alembic revision command. This section is only
 useful for developers who wish to extend the capabilities of Alembic. For
@@ -774,11 +774,11 @@
 *** Next topic ***
 Script_Directory
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Autogeneration
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/commands.html` & `alembic-1.9.4/docs/api/commands.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Commands &#8212; Alembic 1.9.3 documentation</title>
+    <title>Commands &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Operation Directives"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="config.html" title="Configuration"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Commands</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -439,15 +439,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="operations.html" title="Operation Directives"
              >next</a> |</li>
         <li class="right" >
           <a href="config.html" title="Configuration"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Commands</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Commands
 ****** CommandsÂ¶ ******
 Note
 this section discusses the internal API of Alembic as regards its command
 invocation system. This section is only useful for developers who wish to
 extend the capabilities of Alembic. For documentation on using Alembic
@@ -200,11 +200,11 @@
 *** Next topic ***
 Operation_Directives
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Commands
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/config.html` & `alembic-1.9.4/docs/api/config.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Configuration &#8212; Alembic 1.9.3 documentation</title>
+    <title>Configuration &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="runtime.html" title="Runtime Objects"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Configuration</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -74,15 +74,15 @@
 <li><p>to instantiate a <a class="reference internal" href="runtime.html#alembic.runtime.migration.MigrationContext" title="alembic.runtime.migration.MigrationContext"><code class="xref py py-class docutils literal notranslate"><span class="pre">MigrationContext</span></code></a> directly - this object
 only needs a SQLAlchemy connection or dialect name.</p></li>
 <li><p>to instantiate a <a class="reference internal" href="../ops.html#alembic.operations.Operations" title="alembic.operations.Operations"><code class="xref py py-class docutils literal notranslate"><span class="pre">Operations</span></code></a> object - this object only
 needs a <a class="reference internal" href="runtime.html#alembic.runtime.migration.MigrationContext" title="alembic.runtime.migration.MigrationContext"><code class="xref py py-class docutils literal notranslate"><span class="pre">MigrationContext</span></code></a>.</p></li>
 </ul>
 <span class="target" id="module-alembic.config"></span><dl class="py class">
 <dt class="sig sig-object py" id="alembic.config.Config">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">alembic.config.</span></span><span class="sig-name descname"><span class="pre">Config</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">file_:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ini_section:</span> <span class="pre">str</span> <span class="pre">=</span> <span class="pre">'alembic'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">output_buffer:</span> <span class="pre">~typing.TextIO</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">stdout:</span> <span class="pre">~typing.TextIO</span> <span class="pre">=</span> <span class="pre">&lt;_io.TextIOWrapper</span> <span class="pre">name='&lt;stdout&gt;'</span> <span class="pre">mode='w'</span> <span class="pre">encoding='utf-8'&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cmd_opts:</span> <span class="pre">~argparse.Namespace</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">config_args:</span> <span class="pre">~sqlalchemy.cyextension.immutabledict.immutabledict</span> <span class="pre">=</span> <span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attributes:</span> <span class="pre">dict</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#alembic.config.Config" title="Permalink to this definition">¶</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">alembic.config.</span></span><span class="sig-name descname"><span class="pre">Config</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">file_:</span> <span class="pre">str</span> <span class="pre">|</span> <span class="pre">~os.PathLike[str]</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ini_section:</span> <span class="pre">str</span> <span class="pre">=</span> <span class="pre">'alembic'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">output_buffer:</span> <span class="pre">~typing.TextIO</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">stdout:</span> <span class="pre">~typing.TextIO</span> <span class="pre">=</span> <span class="pre">&lt;_io.TextIOWrapper</span> <span class="pre">name='&lt;stdout&gt;'</span> <span class="pre">mode='w'</span> <span class="pre">encoding='utf-8'&gt;</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cmd_opts:</span> <span class="pre">~argparse.Namespace</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">config_args:</span> <span class="pre">~sqlalchemy.cyextension.immutabledict.immutabledict</span> <span class="pre">=</span> <span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attributes:</span> <span class="pre">dict</span> <span class="pre">|</span> <span class="pre">None</span> <span class="pre">=</span> <span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#alembic.config.Config" title="Permalink to this definition">¶</a></dt>
 <dd><p>Represent an Alembic configuration.</p>
 <p>Within an <code class="docutils literal notranslate"><span class="pre">env.py</span></code> script, this is available
 via the <a class="reference internal" href="runtime.html#alembic.runtime.environment.EnvironmentContext.config" title="alembic.runtime.environment.EnvironmentContext.config"><code class="xref py py-attr docutils literal notranslate"><span class="pre">EnvironmentContext.config</span></code></a> attribute,
 which in turn is available at <code class="docutils literal notranslate"><span class="pre">alembic.context</span></code>:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">from</span> <span class="nn">alembic</span> <span class="kn">import</span> <span class="n">context</span>
 
 <span class="n">some_param</span> <span class="o">=</span> <span class="n">context</span><span class="o">.</span><span class="n">config</span><span class="o">.</span><span class="n">get_main_option</span><span class="p">(</span><span class="s2">&quot;my option&quot;</span><span class="p">)</span>
@@ -178,15 +178,15 @@
 <p class="admonition-title">See also</p>
 <p><a class="reference internal" href="runtime.html#alembic.runtime.environment.EnvironmentContext.get_x_argument" title="alembic.runtime.environment.EnvironmentContext.get_x_argument"><code class="xref py py-meth docutils literal notranslate"><span class="pre">EnvironmentContext.get_x_argument()</span></code></a></p>
 </div>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.config.Config.config_file_name">
-<span class="sig-name descname"><span class="pre">config_file_name</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#alembic.config.Config.config_file_name" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">config_file_name</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/os.html#os.PathLike" title="(in Python v3.11)"><span class="pre">PathLike</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#alembic.config.Config.config_file_name" title="Permalink to this definition">¶</a></dt>
 <dd><p>Filesystem path to the .ini file in use.</p>
 </dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.config.Config.config_ini_section">
 <span class="sig-name descname"><span class="pre">config_ini_section</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">None</span></em><a class="headerlink" href="#alembic.config.Config.config_ini_section" title="Permalink to this definition">¶</a></dt>
 <dd><p>Name of the config file section to read basic configuration
@@ -373,15 +373,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              >next</a> |</li>
         <li class="right" >
           <a href="runtime.html" title="Runtime Objects"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Configuration</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Configuration
 ****** ConfigurationÂ¶ ******
 Note
 this section discusses the internal API of Alembic as regards internal
 configuration constructs. This section is only useful for developers who wish
 to extend the capabilities of Alembic. For documentation on configuration of an
@@ -31,18 +31,18 @@
       env.py module within the migration environment
     * to programmatically run any of the commands in the Commands module.
 The Config is not needed for these cases:
     * to instantiate a MigrationContext directly - this object only needs a
       SQLAlchemy connection or dialect name.
     * to instantiate a Operations object - this object only needs a
       MigrationContext.
-  classalembic.config.Config(file_: str | None = None, ini_section: str =
-  'alembic', output_buffer: ~typing.TextIO | None = None, stdout:
-  ~typing.TextIO = <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-
-  8'>, cmd_opts: ~argparse.Namespace | None = None, config_args:
+  classalembic.config.Config(file_: str | ~os.PathLike[str] | None = None,
+  ini_section: str = 'alembic', output_buffer: ~typing.TextIO | None = None,
+  stdout: ~typing.TextIO = <_io.TextIOWrapper name='<stdout>' mode='w'
+  encoding='utf-8'>, cmd_opts: ~argparse.Namespace | None = None, config_args:
   ~sqlalchemy.cyextension.immutabledict.immutabledict = {}, attributes: dict |
   None = None)Â¶
       Represent an Alembic configuration.
       Within an env.py script, this is available via the
       EnvironmentContext.config attribute, which in turn is available at
       alembic.context:
       from alembic import context
@@ -85,15 +85,15 @@
             Config.attributes
         cmd_opts: Namespace | None= NoneÂ¶
             The command-line options passed to the alembic script.
             Within an env.py script this can be accessed via the
             EnvironmentContext.config attribute.
             See also
             EnvironmentContext.get_x_argument()
-        config_file_name: str | None= NoneÂ¶
+        config_file_name: str | PathLike[str] | None= NoneÂ¶
             Filesystem path to the .ini file in use.
         config_ini_section: str= NoneÂ¶
             Name of the config file section to read basic configuration from.
             Defaults to alembic, that is the [alembic] section of the .ini
             file. This value is modified using the -n/--name option to the
             Alembic runner.
         file_configÂ¶
@@ -179,11 +179,11 @@
 *** Next topic ***
 Commands
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Configuration
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/ddl.html` & `alembic-1.9.4/docs/api/ddl.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>DDL Internals &#8212; Alembic 1.9.3 documentation</title>
+    <title>DDL Internals &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../changelog.html" title="Changelog"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="script.html" title="Script Directory"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">DDL Internals</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -425,15 +425,15 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.impl.DefaultImpl.type_arg_extract">
 <span class="sig-name descname"><span class="pre">type_arg_extract</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Sequence" title="(in Python v3.11)"><span class="pre">Sequence</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">()</span></em><a class="headerlink" href="#alembic.ddl.impl.DefaultImpl.type_arg_extract" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.impl.DefaultImpl.type_synonyms">
-<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Set" title="(in Python v3.11)"><span class="pre">Set</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'NUMERIC',</span> <span class="pre">'DECIMAL'},)</span></em><a class="headerlink" href="#alembic.ddl.impl.DefaultImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Set" title="(in Python v3.11)"><span class="pre">Set</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'DECIMAL',</span> <span class="pre">'NUMERIC'},)</span></em><a class="headerlink" href="#alembic.ddl.impl.DefaultImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="alembic.ddl.impl.ImplMeta">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">alembic.ddl.impl.</span></span><span class="sig-name descname"><span class="pre">ImplMeta</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">classname</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">bases</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Tuple" title="(in Python v3.11)"><span class="pre">Tuple</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Type" title="(in Python v3.11)"><span class="pre">Type</span></a><span class="p"><span class="pre">[</span></span><a class="reference internal" href="#alembic.ddl.impl.DefaultImpl" title="alembic.ddl.impl.DefaultImpl"><span class="pre">DefaultImpl</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dict_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Dict" title="(in Python v3.11)"><span class="pre">Dict</span></a><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">,</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/typing.html#typing.Any" title="(in Python v3.11)"><span class="pre">Any</span></a><span class="p"><span class="pre">]</span></span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#alembic.ddl.impl.ImplMeta" title="Permalink to this definition">¶</a></dt>
@@ -536,15 +536,15 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.mysql.MySQLImpl.type_arg_extract">
 <span class="sig-name descname"><span class="pre">type_arg_extract</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Sequence</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">['character</span> <span class="pre">set</span> <span class="pre">([\\w\\-_]+)',</span> <span class="pre">'collate</span> <span class="pre">([\\w\\-_]+)']</span></em><a class="headerlink" href="#alembic.ddl.mysql.MySQLImpl.type_arg_extract" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.mysql.MySQLImpl.type_synonyms">
-<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'NUMERIC',</span> <span class="pre">'DECIMAL'},</span> <span class="pre">{'TINYINT',</span> <span class="pre">'BOOL'},</span> <span class="pre">{'JSON',</span> <span class="pre">'LONGTEXT'})</span></em><a class="headerlink" href="#alembic.ddl.mysql.MySQLImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'DECIMAL',</span> <span class="pre">'NUMERIC'},</span> <span class="pre">{'BOOL',</span> <span class="pre">'TINYINT'},</span> <span class="pre">{'JSON',</span> <span class="pre">'LONGTEXT'})</span></em><a class="headerlink" href="#alembic.ddl.mysql.MySQLImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="alembic.ddl.mysql.MySQLModifyColumn">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">alembic.ddl.mysql.</span></span><span class="sig-name descname"><span class="pre">MySQLModifyColumn</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">column_name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">schema</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">newname</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">type_</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">TypeEngine</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">nullable</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">default</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">_ServerDefault</span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="k"><span class="pre">False</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">autoincrement</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/functions.html#bool" title="(in Python v3.11)"><span class="pre">bool</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><span class="pre">Literal</span><span class="p"><span class="pre">[</span></span><span class="k"><span class="pre">False</span></span><span class="p"><span class="pre">]</span></span><span class="w"> </span><span class="p"><span class="pre">|</span></span><span class="w"> </span><a class="reference external" href="https://docs.python.org/3/library/constants.html#None" title="(in Python v3.11)"><span class="pre">None</span></a></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#alembic.ddl.mysql.MySQLModifyColumn" title="Permalink to this definition">¶</a></dt>
@@ -619,15 +619,15 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.mssql.MSSQLImpl.transactional_ddl">
 <span class="sig-name descname"><span class="pre">transactional_ddl</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">True</span></em><a class="headerlink" href="#alembic.ddl.mssql.MSSQLImpl.transactional_ddl" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.mssql.MSSQLImpl.type_synonyms">
-<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'NUMERIC',</span> <span class="pre">'DECIMAL'},</span> <span class="pre">{'NVARCHAR',</span> <span class="pre">'VARCHAR'})</span></em><a class="headerlink" href="#alembic.ddl.mssql.MSSQLImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'DECIMAL',</span> <span class="pre">'NUMERIC'},</span> <span class="pre">{'VARCHAR',</span> <span class="pre">'NVARCHAR'})</span></em><a class="headerlink" href="#alembic.ddl.mssql.MSSQLImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="alembic.ddl.mssql.mssql_add_column">
 <span class="sig-prename descclassname"><span class="pre">alembic.ddl.mssql.</span></span><span class="sig-name descname"><span class="pre">mssql_add_column</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">compiler</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">MSDDLCompiler</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">column</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Column</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#alembic.ddl.mssql.mssql_add_column" title="Permalink to this definition">¶</a></dt>
@@ -766,15 +766,15 @@
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.postgresql.PostgresqlImpl.transactional_ddl">
 <span class="sig-name descname"><span class="pre">transactional_ddl</span></span><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">True</span></em><a class="headerlink" href="#alembic.ddl.postgresql.PostgresqlImpl.transactional_ddl" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 <dl class="py attribute">
 <dt class="sig sig-object py" id="alembic.ddl.postgresql.PostgresqlImpl.type_synonyms">
-<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'NUMERIC',</span> <span class="pre">'DECIMAL'},</span> <span class="pre">{'FLOAT',</span> <span class="pre">'DOUBLE</span> <span class="pre">PRECISION'})</span></em><a class="headerlink" href="#alembic.ddl.postgresql.PostgresqlImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
+<span class="sig-name descname"><span class="pre">type_synonyms</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">Set</span><span class="p"><span class="pre">[</span></span><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="p"><span class="pre">...</span></span><span class="p"><span class="pre">]</span></span></em><em class="property"><span class="w"> </span><span class="p"><span class="pre">=</span></span><span class="w"> </span><span class="pre">({'DECIMAL',</span> <span class="pre">'NUMERIC'},</span> <span class="pre">{'DOUBLE</span> <span class="pre">PRECISION',</span> <span class="pre">'FLOAT'})</span></em><a class="headerlink" href="#alembic.ddl.postgresql.PostgresqlImpl.type_synonyms" title="Permalink to this definition">¶</a></dt>
 <dd></dd></dl>
 
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="alembic.ddl.postgresql.visit_column_comment">
 <span class="sig-prename descclassname"><span class="pre">alembic.ddl.postgresql.</span></span><span class="sig-name descname"><span class="pre">visit_column_comment</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">element</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><a class="reference internal" href="#alembic.ddl.base.ColumnComment" title="alembic.ddl.base.ColumnComment"><span class="pre">ColumnComment</span></a></span></em>, <em class="sig-param"><span class="n"><span class="pre">compiler</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">PGDDLCompiler</span></span></em>, <em class="sig-param"><span class="o"><span class="pre">**</span></span><span class="n"><span class="pre">kw</span></span></em><span class="sig-paren">)</span> <span class="sig-return"><span class="sig-return-icon">&#x2192;</span> <span class="sig-return-typehint"><a class="reference external" href="https://docs.python.org/3/library/stdtypes.html#str" title="(in Python v3.11)"><span class="pre">str</span></a></span></span><a class="headerlink" href="#alembic.ddl.postgresql.visit_column_comment" title="Permalink to this definition">¶</a></dt>
@@ -1094,15 +1094,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="../changelog.html" title="Changelog"
              >next</a> |</li>
         <li class="right" >
           <a href="script.html" title="Script Directory"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">DDL Internals</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * DDL Internals
 ****** DDL InternalsÂ¶ ******
 These are some of the constructs used to generate migration instructions. The
 APIs here build off of the sqlalchemy.schema.DDLElement and Custom_SQL
 Constructs_and_Compilation_Extension systems.
 For programmatic usage of Alembicâs migration directives, the easiest route
@@ -178,15 +178,15 @@
             add_column are present.
         start_migrations() &#x2192; NoneÂ¶
             A hook called when EnvironmentContext.run_migrations() is called.
             Implementations can set up per-migration-run state here.
         static_output(text: str) &#x2192; NoneÂ¶
         transactional_ddl= FalseÂ¶
         type_arg_extract: Sequence[str]= ()Â¶
-        type_synonyms: Tuple[Set[str], ...]= ({'NUMERIC', 'DECIMAL'},)Â¶
+        type_synonyms: Tuple[Set[str], ...]= ({'DECIMAL', 'NUMERIC'},)Â¶
   classalembic.ddl.impl.ImplMeta(classname: str, bases: Tuple[Type
   [DefaultImpl]], dict_: Dict[str, Any])Â¶
   classalembic.ddl.impl.Params(token0, tokens, args, kwargs)Â¶
       Create new instance of Params(token0, tokens, args, kwargs)
         argsÂ¶
             Alias for field number 2
         kwargsÂ¶
@@ -229,16 +229,16 @@
         metadata_unique_constraints, metadata_indexes)Â¶
         correct_for_autogen_foreignkeys(conn_fks, metadata_fks)Â¶
         drop_constraint(const: Constraint) &#x2192; NoneÂ¶
         memo: dictÂ¶
         transactional_ddl= FalseÂ¶
         type_arg_extract: Sequence[str]= ['character set ([\\w\\-_]+)',
         'collate ([\\w\\-_]+)']Â¶
-        type_synonyms: Tuple[Set[str], ...]= ({'NUMERIC', 'DECIMAL'},
-        {'TINYINT', 'BOOL'}, {'JSON', 'LONGTEXT'})Â¶
+        type_synonyms: Tuple[Set[str], ...]= ({'DECIMAL', 'NUMERIC'}, {'BOOL',
+        'TINYINT'}, {'JSON', 'LONGTEXT'})Â¶
   classalembic.ddl.mysql.MySQLModifyColumn(name: str, column_name: str, schema:
   str | None = None, newname: str | None = None, type_: TypeEngine | None =
   None, nullable: bool | None = None, default: _ServerDefault | Literal[False]
   | None = False, autoincrement: bool | None = None, comment: str | Literal
   [False] | None = False)Â¶
       Bases: MySQLChangeColumn
 
@@ -270,16 +270,16 @@
             This is used in offline mode and typically via
             EnvironmentContext.begin_transaction().
         identity_attrs_ignore: Tuple[str, ...]= ('minvalue', 'maxvalue',
         'nominvalue', 'nomaxvalue', 'cycle', 'cache', 'order', 'on_null',
         'order')Â¶
         memo: dictÂ¶
         transactional_ddl= TrueÂ¶
-        type_synonyms: Tuple[Set[str], ...]= ({'NUMERIC', 'DECIMAL'},
-        {'NVARCHAR', 'VARCHAR'})Â¶
+        type_synonyms: Tuple[Set[str], ...]= ({'DECIMAL', 'NUMERIC'},
+        {'VARCHAR', 'NVARCHAR'})Â¶
   alembic.ddl.mssql.mssql_add_column(compiler: MSDDLCompiler, column: Column,
   **kw) &#x2192; strÂ¶
   alembic.ddl.mssql.visit_add_column(element: AddColumn, compiler:
   MSDDLCompiler, **kw) &#x2192; strÂ¶
   alembic.ddl.mssql.visit_column_default(element: ColumnDefault, compiler:
   MSDDLCompiler, **kw) &#x2192; strÂ¶
   alembic.ddl.mssql.visit_column_nullable(element: ColumnNullable, compiler:
@@ -343,16 +343,16 @@
             perform any operations needed on a table before a new one is
             created to replace it in batch mode.
             the PG dialect uses this to drop constraints on the table before
             the new one uses those same names.
         render_type(type_: TypeEngine, autogen_context: AutogenContext)
         &#x2192; str | Literal[False]Â¶
         transactional_ddl= TrueÂ¶
-        type_synonyms: Tuple[Set[str], ...]= ({'NUMERIC', 'DECIMAL'}, {'FLOAT',
-        'DOUBLE PRECISION'})Â¶
+        type_synonyms: Tuple[Set[str], ...]= ({'DECIMAL', 'NUMERIC'}, {'DOUBLE
+        PRECISION', 'FLOAT'})Â¶
   alembic.ddl.postgresql.visit_column_comment(element: ColumnComment, compiler:
   PGDDLCompiler, **kw) &#x2192; strÂ¶
   alembic.ddl.postgresql.visit_column_type(element: PostgresqlColumnType,
   compiler: PGDDLCompiler, **kw) &#x2192; strÂ¶
   alembic.ddl.postgresql.visit_identity_column(element: IdentityColumnDefault,
   compiler: PGDDLCompiler, **kw)Â¶
   alembic.ddl.postgresql.visit_rename_table(element: RenameTable, compiler:
@@ -550,11 +550,11 @@
 *** Next topic ***
 Changelog
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * DDL Internals
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/index.html` & `alembic-1.9.4/docs/api/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>API Details &#8212; Alembic 1.9.3 documentation</title>
+    <title>API Details &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="../cookbook.html" title="Cookbook"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API Details</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -196,15 +196,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview"
              >next</a> |</li>
         <li class="right" >
           <a href="../cookbook.html" title="Cookbook"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">API Details</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API Details
 ****** API DetailsÂ¶ ******
 Alembicâs internal API has many public integration points that can be used to
 extend Alembicâs functionality as well as to re-use its functionality in new
 ways. As the project has grown, more APIs are created and exposed for this
 purpose.
 Direct use of the vast majority of API details discussed here is not needed for
@@ -108,10 +108,10 @@
 *** Next topic ***
 Overview
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API Details
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/operations.html` & `alembic-1.9.4/docs/api/operations.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Operation Directives &#8212; Alembic 1.9.3 documentation</title>
+    <title>Operation Directives &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Autogeneration"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Operation Directives</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -764,15 +764,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Autogeneration"
              >next</a> |</li>
         <li class="right" >
           <a href="commands.html" title="Commands"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Operation Directives</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Operation Directives
 ****** Operation DirectivesÂ¶ ******
 Note
 this section discusses the internal API of Alembic as regards the internal
 system of defining migration operation directives. This section is only useful
 for developers who wish to extend the capabilities of Alembic. For end-user
@@ -503,11 +503,11 @@
 *** Next topic ***
 Autogeneration
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Operation Directives
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/overview.html` & `alembic-1.9.4/docs/api/overview.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Overview &#8212; Alembic 1.9.3 documentation</title>
+    <title>Overview &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="runtime.html" title="Runtime Objects"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="API Details"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Overview</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -147,15 +147,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="runtime.html" title="Runtime Objects"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="API Details"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Overview</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Overview
 ****** OverviewÂ¶ ******
 Note
 this section is a technical overview of the internal API of Alembic. This
 section is only useful for developers who wish to extend the capabilities of
 Alembic; for regular users, reading this section is not necessary.
@@ -69,11 +69,11 @@
 *** Next topic ***
 Runtime_Objects
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Overview
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/runtime.html` & `alembic-1.9.4/docs/api/runtime.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Runtime Objects &#8212; Alembic 1.9.3 documentation</title>
+    <title>Runtime Objects &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="config.html" title="Configuration"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Runtime Objects</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -1184,15 +1184,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="config.html" title="Configuration"
              >next</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Runtime Objects</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Runtime Objects
 ****** Runtime ObjectsÂ¶ ******
 The âruntimeâ of Alembic involves the EnvironmentContext and
 MigrationContext objects. These are the objects that are in play once the
 env.py script is loaded up by a command and a migration operation proceeds.
 ***** The Environment ContextÂ¶ *****
@@ -528,11 +528,11 @@
 *** Next topic ***
 Configuration
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Runtime Objects
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/api/script.html` & `alembic-1.9.4/docs/api/script.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Script Directory &#8212; Alembic 1.9.3 documentation</title>
+    <title>Script Directory &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="../_static/sphinx_paramlinks.css" />
     <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
     <script src="../_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ddl.html" title="DDL Internals"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Autogeneration"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" accesskey="U">API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Script Directory</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
@@ -625,15 +625,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ddl.html" title="DDL Internals"
              >next</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Autogeneration"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="../index.html">Alembic 1.9.4 documentation</a> &#187;</li>
           <li class="nav-item nav-item-1"><a href="index.html" >API Details</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Script Directory</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Script Directory
 ****** Script DirectoryÂ¶ ******
 The ScriptDirectory object provides programmatic access to the Alembic version
 files present in the filesystem.
   classalembic.script.Script(module: module, rev_id: str, path: str)Â¶
       Represent a single revision file in a versions/ directory.
@@ -319,11 +319,11 @@
 *** Next topic ***
 DDL_Internals
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * API_Details »
     * Script Directory
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/autogenerate.html` & `alembic-1.9.4/docs/autogenerate.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Auto Generating Migrations &#8212; Alembic 1.9.3 documentation</title>
+    <title>Auto Generating Migrations &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="offline.html" title="Generating SQL Scripts (a.k.a. “Offline Mode”)"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Auto Generating Migrations</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1008,15 +1008,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="offline.html" title="Generating SQL Scripts (a.k.a. “Offline Mode”)"
              >next</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Auto Generating Migrations</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Auto Generating Migrations
 ****** Auto Generating MigrationsÂ¶ ******
 Alembic can view the status of the database and compare against the table
 metadata in the application, generating the âobviousâ migrations based on a
 comparison. This is achieved using the --autogenerate option to the alembic
 revision command, which places so-called candidate migrations into our new
 migrations file. We review and modify these by hand as needed, then proceed
@@ -761,10 +761,10 @@
 *** Next topic ***
 Generating_SQL_Scripts_(a.k.a._âOffline_Modeâ)
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Auto Generating Migrations
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/batch.html` & `alembic-1.9.4/docs/batch.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Running “Batch” Migrations for SQLite and Other Databases &#8212; Alembic 1.9.3 documentation</title>
+    <title>Running “Batch” Migrations for SQLite and Other Databases &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="branches.html" title="Working with Branches"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="naming.html" title="The Importance of Naming Constraints"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Running “Batch” Migrations for SQLite and Other Databases</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -475,15 +475,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="branches.html" title="Working with Branches"
              >next</a> |</li>
         <li class="right" >
           <a href="naming.html" title="The Importance of Naming Constraints"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Running “Batch” Migrations for SQLite and Other Databases</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Running âBatchâ Migrations for SQLite and Other Databases
 ****** Running âBatchâ Migrations for SQLite and Other DatabasesÂ¶ ******
 The SQLite database presents a challenge to migration tools in that it has
 almost no support for the ALTER statement which relational schema migrations
 rely upon. The rationale for this stems from philosophical and architectural
 concerns within SQLite, and they are unlikely to be changed.
 Migration tools are instead expected to produce copies of SQLite tables that
@@ -330,10 +330,10 @@
 *** Next topic ***
 Working_with_Branches
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Running âBatchâ Migrations for SQLite and Other Databases
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/branches.html` & `alembic-1.9.4/docs/branches.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Working with Branches &#8212; Alembic 1.9.3 documentation</title>
+    <title>Working with Branches &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ops.html" title="Operation Reference"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="batch.html" title="Running “Batch” Migrations for SQLite and Other Databases"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Working with Branches</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -888,15 +888,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="ops.html" title="Operation Reference"
              >next</a> |</li>
         <li class="right" >
           <a href="batch.html" title="Running “Batch” Migrations for SQLite and Other Databases"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Working with Branches</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Working with Branches
 ****** Working with BranchesÂ¶ ******
 A branch describes a point in a migration stream when two or more versions
 refer to the same parent migration as their anscestor. Branches occur naturally
 when two divergent source trees, both containing Alembic revision files created
 independently within those source trees, are merged together into one. When
 this occurs, the challenge of a branch is to merge the branches into a single
@@ -711,10 +711,10 @@
 *** Next topic ***
 Operation_Reference
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Working with Branches
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/build/Makefile` & `alembic-1.9.4/docs/build/Makefile`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/api_overview.png` & `alembic-1.9.4/docs/build/api/api_overview.png`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/autogenerate.rst` & `alembic-1.9.4/docs/build/api/autogenerate.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/commands.rst` & `alembic-1.9.4/docs/build/api/commands.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/config.rst` & `alembic-1.9.4/docs/build/api/config.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/ddl.rst` & `alembic-1.9.4/docs/build/api/ddl.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/index.rst` & `alembic-1.9.4/docs/build/api/index.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/operations.rst` & `alembic-1.9.4/docs/build/api/operations.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/overview.rst` & `alembic-1.9.4/docs/build/api/overview.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/runtime.rst` & `alembic-1.9.4/docs/build/api/runtime.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/api/script.rst` & `alembic-1.9.4/docs/build/api/script.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/autogenerate.rst` & `alembic-1.9.4/docs/build/autogenerate.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/batch.rst` & `alembic-1.9.4/docs/build/batch.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/branches.rst` & `alembic-1.9.4/docs/build/branches.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/changelog.rst` & `alembic-1.9.4/docs/build/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,57 @@
 
 ==========
 Changelog
 ==========
 
 .. changelog::
+    :version: 1.9.4
+    :released: February 16, 2023
+
+    .. change::
+        :tags: bug, mssql
+        :tickets: 1177
+
+        Ongoing fixes for SQL Server server default comparisons under autogenerate,
+        adjusting for SQL Server's collapsing of whitespace between SQL function
+        arguments when reporting on a function-based server default, as well as its
+        arbitrary addition of parenthesis within arguments; the approach has now
+        been made more aggressive by stripping the two default strings to compare
+        of all whitespace, parenthesis, and quoting characters.
+
+
+    .. change::
+        :tags: bug, postgresql
+
+        Fixed PostgreSQL server default comparison to handle SQL expressions
+        sent as ``text()`` constructs, such as ``text("substring('name', 1, 3)")``,
+        which previously would raise errors when attempting to run a server-based
+        comparison.
+
+
+
+    .. change::
+        :tags: bug, autogenerate
+        :tickets: 1180
+
+        Removed a mis-use of the
+        :paramref:`.EnvironmentContext.configure.render_item` callable where the
+        "server_default" renderer would be erroneously used within the server
+        default comparison process, which is working against SQL expressions, not
+        Python code.
+
+    .. change::
+        :tags: bug, commands
+
+        Fixed regression introduced in 1.7.0 where the "config" object passed to
+        the template context when running the :func:`.merge` command
+        programmatically failed to be correctly populated. Pull request courtesy
+        Brendan Gann.
+
+.. changelog::
     :version: 1.9.3
     :released: February 7, 2023
 
     .. change::
         :tags: bug, autogenerate
         :tickets: 1167
```

### Comparing `alembic-1.9.3/docs/build/conf.py` & `alembic-1.9.4/docs/build/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,14 +41,18 @@
     "sphinx_copybutton",
 ]
 
 copybutton_prompt_text = (
     r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
 )
 copybutton_prompt_is_regexp = True
+# workaround
+# https://sphinx-copybutton-exclude-issue.readthedocs.io/en/v0.5.1-go/
+# https://github.com/executablebooks/sphinx-copybutton/issues/185
+copybutton_exclude = ".linenos"
 
 
 # tags to sort on inside of sections
 changelog_sections = [
     "changed",
     "feature",
     "usecase",
@@ -91,16 +95,16 @@
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = alembic.__version__
 # The full version, including alpha/beta/rc tags.
-release = "1.9.3"
-release_date = "February 7, 2023"
+release = "1.9.4"
+release_date = "February 16, 2023"
 
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 # language = None
 
 # There are two options for replacing |today|: either, you set today to some
```

### Comparing `alembic-1.9.3/docs/build/cookbook.rst` & `alembic-1.9.4/docs/build/cookbook.rst`

 * *Files 3% similar despite different names*

```diff
@@ -218,15 +218,15 @@
     from alembic import command, config
 
     cfg = config.Config("/path/to/yourapp/alembic.ini")
     with engine.begin() as connection:
         cfg.attributes['connection'] = connection
         command.upgrade(cfg, "head")
 
-Then in ``env.py``::
+Then in ``env.py`` we can update ``run_migrations_online``::
 
     def run_migrations_online():
         connectable = config.attributes.get('connection', None)
 
         if connectable is None:
             # only create Engine if we don't have a Connection
             # from the outside
@@ -1479,84 +1479,54 @@
     def do_run_migrations(connection):
         context.configure(connection=connection, target_metadata=target_metadata)
 
         with context.begin_transaction():
             context.run_migrations()
 
 
-    async def run_migrations_online():
-        """Run migrations in 'online' mode.
-
-        In this scenario we need to create an Engine
+    async def run_async_migrations():
+        """In this scenario we need to create an Engine
         and associate a connection with the context.
 
         """
+
         connectable = async_engine_from_config(
             config.get_section(config.config_ini_section),
             prefix="sqlalchemy.",
             poolclass=pool.NullPool,
         )
 
         async with connectable.connect() as connection:
             await connection.run_sync(do_run_migrations)
 
         await connectable.dispose()
 
 
-    if context.is_offline_mode():
-        run_migrations_offline()
-    else:
-        asyncio.run(run_migrations_online())
+    def run_migrations_online():
+        """Run migrations in 'online' mode."""
+
+        asyncio.run(run_async_migrations())
 
 An async application can also interact with the Alembic api directly by using
 the SQLAlchemy ``run_sync`` method to adapt the non-async api of Alembic to
 an async consumer.
 
 
 .. _connection_sharing_plus_asyncio:
 
 Programmatic API use (connection sharing) With Asyncio
 ------------------------------------------------------
 
 Combining the examples of :ref:`connection_sharing` with :ref:`asyncio_recipe`
-together, and ``env.py`` as follows works::
-
-    import asyncio
-
-    from sqlalchemy.ext.asyncio import async_engine_from_config
-
-    # ... no change required to the rest of the code
-
-
-    def do_run_migrations(connection):
-        context.configure(connection=connection, target_metadata=target_metadata)
-
-        with context.begin_transaction():
-            context.run_migrations()
-
-
-    async def run_async_migrations():
-        connectable = async_engine_from_config(
-            config.get_section(config.config_ini_section),
-            prefix="sqlalchemy.",
-            poolclass=pool.NullPool,
-        )
-
-        async with connectable.connect() as connection:
-            await connection.run_sync(do_run_migrations)
-
-        await connectable.dispose()
+together, the  ``env.py`` listed above can be updated as follows works::
 
 
     def run_migrations_online():
         """Run migrations in 'online' mode.
 
-        In this scenario we need to create an Engine
-        and associate a connection with the context.
-
         """
 
         connectable = config.attributes.get("connection", None)
 
         if connectable is None:
             asyncio.run(run_async_migrations())
         else:
```

### Comparing `alembic-1.9.3/docs/build/front.rst` & `alembic-1.9.4/docs/build/front.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/index.rst` & `alembic-1.9.4/docs/build/index.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/naming.rst` & `alembic-1.9.4/docs/build/naming.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/offline.rst` & `alembic-1.9.4/docs/build/offline.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/ops.rst` & `alembic-1.9.4/docs/build/ops.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/build/tutorial.rst` & `alembic-1.9.4/docs/build/tutorial.rst`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/docs/changelog.html` & `alembic-1.9.4/docs/changelog.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Changelog &#8212; Alembic 1.9.3 documentation</title>
+    <title>Changelog &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -29,26 +29,65 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api/ddl.html" title="DDL Internals"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
             
   <section id="changelog">
 <h1>Changelog<a class="headerlink" href="#changelog" title="Permalink to this heading">¶</a></h1>
+<section id="change-1.9.4">
+<h2 class="release-version">1.9.4<a class="headerlink" href="#change-1.9.4" title="Permalink to this heading">¶</a></h2>
+Released: February 16, 2023<section id="change-1.9.4-bug">
+<h3>bug<a class="headerlink" href="#change-1.9.4-bug" title="Permalink to this heading">¶</a></h3>
+<ul class="simple">
+<li><p class="caption" id="change-1.9.4-0"><span class="target" id="change-5adf442f4e35b7f3e161817380fcda53"><strong>[bug] [mssql]</strong> <a class="changelog-reference headerlink reference internal" href="#change-5adf442f4e35b7f3e161817380fcda53">¶</a></span><p>Ongoing fixes for SQL Server server default comparisons under autogenerate,
+adjusting for SQL Server’s collapsing of whitespace between SQL function
+arguments when reporting on a function-based server default, as well as its
+arbitrary addition of parenthesis within arguments; the approach has now
+been made more aggressive by stripping the two default strings to compare
+of all whitespace, parenthesis, and quoting characters.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/alembic/issues/1177">#1177</a></p>
+</p>
+</li>
+<li><p class="caption" id="change-1.9.4-1"><span class="target" id="change-2064f89cc2081b8a0403d23a182e0647"><strong>[bug] [postgresql]</strong> <a class="changelog-reference headerlink reference internal" href="#change-2064f89cc2081b8a0403d23a182e0647">¶</a></span><p>Fixed PostgreSQL server default comparison to handle SQL expressions
+sent as <code class="docutils literal notranslate"><span class="pre">text()</span></code> constructs, such as <code class="docutils literal notranslate"><span class="pre">text(&quot;substring('name',</span> <span class="pre">1,</span> <span class="pre">3)&quot;)</span></code>,
+which previously would raise errors when attempting to run a server-based
+comparison.</p>
+<p></p>
+</p>
+</li>
+<li><p class="caption" id="change-1.9.4-2"><span class="target" id="change-aac9100697434b100c9c871f75da5d8b"><strong>[bug] [autogenerate]</strong> <a class="changelog-reference headerlink reference internal" href="#change-aac9100697434b100c9c871f75da5d8b">¶</a></span><p>Removed a mis-use of the
+<a class="reference internal" href="api/runtime.html#alembic.runtime.environment.EnvironmentContext.configure.params.render_item" title="alembic.runtime.environment.EnvironmentContext.configure"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">EnvironmentContext.configure.render_item</span></code></a> callable where the
+“server_default” renderer would be erroneously used within the server
+default comparison process, which is working against SQL expressions, not
+Python code.</p>
+<p>References: <a class="reference external" href="https://github.com/sqlalchemy/alembic/issues/1180">#1180</a></p>
+</p>
+</li>
+<li><p class="caption" id="change-1.9.4-3"><span class="target" id="change-2baf3527756a1ebc6274d402cdbac3fb"><strong>[bug] [commands]</strong> <a class="changelog-reference headerlink reference internal" href="#change-2baf3527756a1ebc6274d402cdbac3fb">¶</a></span><p>Fixed regression introduced in 1.7.0 where the “config” object passed to
+the template context when running the <a class="reference internal" href="api/commands.html#alembic.command.merge" title="alembic.command.merge"><code class="xref py py-func docutils literal notranslate"><span class="pre">merge()</span></code></a> command
+programmatically failed to be correctly populated. Pull request courtesy
+Brendan Gann.</p>
+<p></p>
+</p>
+</li>
+</ul>
+</section>
+</section>
 <section id="change-1.9.3">
 <h2 class="release-version">1.9.3<a class="headerlink" href="#change-1.9.3" title="Permalink to this heading">¶</a></h2>
 Released: February 7, 2023<section id="change-1.9.3-bug">
 <h3>bug<a class="headerlink" href="#change-1.9.3-bug" title="Permalink to this heading">¶</a></h3>
 <ul class="simple">
 <li><p class="caption" id="change-1.9.3-0"><span class="target" id="change-c43617ee3525ded9b8355029b357b918"><strong>[bug] [autogenerate]</strong> <a class="changelog-reference headerlink reference internal" href="#change-c43617ee3525ded9b8355029b357b918">¶</a></span><p>Fixed issue where rendering of user-defined types that then went onto use
 the <code class="docutils literal notranslate"><span class="pre">.with_variant()</span></code> method would fail to render, if using SQLAlchemy
@@ -5152,14 +5191,18 @@
       </div>
       <div class="sphinxsidebar" role="navigation" aria-label="main navigation">
         <div class="sphinxsidebarwrapper">
   <div>
     <h3><a href="index.html">Table of Contents</a></h3>
     <ul>
 <li><a class="reference internal" href="#">Changelog</a><ul>
+<li><a class="reference internal" href="#change-1.9.4">1.9.4</a><ul>
+<li><a class="reference internal" href="#change-1.9.4-bug">bug</a></li>
+</ul>
+</li>
 <li><a class="reference internal" href="#change-1.9.3">1.9.3</a><ul>
 <li><a class="reference internal" href="#change-1.9.3-bug">bug</a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#change-1.9.2">1.9.2</a><ul>
 <li><a class="reference internal" href="#change-1.9.2-bug">bug</a></li>
 </ul>
@@ -5674,15 +5717,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="api/ddl.html" title="DDL Internals"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Changelog</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -7,17 +7,44 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Changelog
 ****** ChangelogÂ¶ ******
+***** 1.9.4Â¶ *****
+Released: February 16, 2023
+**** bugÂ¶ ****
+    * [bug] [mssql] Â¶
+      Ongoing fixes for SQL Server server default comparisons under
+      autogenerate, adjusting for SQL Serverâs collapsing of whitespace
+      between SQL function arguments when reporting on a function-based server
+      default, as well as its arbitrary addition of parenthesis within
+      arguments; the approach has now been made more aggressive by stripping
+      the two default strings to compare of all whitespace, parenthesis, and
+      quoting characters.
+      References: #1177
+[bug] [postgresql] Â¶
+Fixed PostgreSQL server default comparison to handle SQL expressions sent as
+text() constructs, such as text("substring('name', 1, 3)"), which previously
+would raise errors when attempting to run a server-based comparison.
+[bug] [autogenerate] Â¶
+Removed a mis-use of the EnvironmentContext.configure.render_item callable
+where the âserver_defaultâ renderer would be erroneously used within the
+server default comparison process, which is working against SQL expressions,
+not Python code.
+References: #1180
+[bug] [commands] Â¶
+Fixed regression introduced in 1.7.0 where the âconfigâ object passed to
+the template context when running the merge() command programmatically failed
+to be correctly populated. Pull request courtesy Brendan Gann.
+
 ***** 1.9.3Â¶ *****
 Released: February 7, 2023
 **** bugÂ¶ ****
     * [bug] [autogenerate] Â¶
       Fixed issue where rendering of user-defined types that then went onto use
       the .with_variant() method would fail to render, if using SQLAlchemy
       2.0âs version of variants.
@@ -3482,14 +3509,16 @@
 Support for non-ASCII table, column and constraint names is mostly nonexistent.
 This is also a straightforward feature add as SQLAlchemy itself supports
 unicode identifiers; Alembic itself will likely need fixes to logging, column
 identification by key, etc. for full support here.
 
 **** Table_of_Contents ****
     * Changelog
+          o 1.9.4
+                # bug
           o 1.9.3
                 # bug
           o 1.9.2
                 # bug
           o 1.9.1
                 # bug
           o 1.9.0
@@ -3768,10 +3797,10 @@
 [q                   ] [Go]
 *** Previous topic ***
 DDL_Internals
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Changelog
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/cookbook.html` & `alembic-1.9.4/docs/cookbook.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Cookbook &#8212; Alembic 1.9.3 documentation</title>
+    <title>Cookbook &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api/index.html" title="API Details"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="ops.html" title="Operation Reference"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Cookbook</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -248,15 +248,15 @@
 
 <span class="n">cfg</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">Config</span><span class="p">(</span><span class="s2">&quot;/path/to/yourapp/alembic.ini&quot;</span><span class="p">)</span>
 <span class="k">with</span> <span class="n">engine</span><span class="o">.</span><span class="n">begin</span><span class="p">()</span> <span class="k">as</span> <span class="n">connection</span><span class="p">:</span>
     <span class="n">cfg</span><span class="o">.</span><span class="n">attributes</span><span class="p">[</span><span class="s1">&#39;connection&#39;</span><span class="p">]</span> <span class="o">=</span> <span class="n">connection</span>
     <span class="n">command</span><span class="o">.</span><span class="n">upgrade</span><span class="p">(</span><span class="n">cfg</span><span class="p">,</span> <span class="s2">&quot;head&quot;</span><span class="p">)</span>
 </pre></div>
 </div>
-<p>Then in <code class="docutils literal notranslate"><span class="pre">env.py</span></code>:</p>
+<p>Then in <code class="docutils literal notranslate"><span class="pre">env.py</span></code> we can update <code class="docutils literal notranslate"><span class="pre">run_migrations_online</span></code>:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">run_migrations_online</span><span class="p">():</span>
     <span class="n">connectable</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">attributes</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s1">&#39;connection&#39;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
 
     <span class="k">if</span> <span class="n">connectable</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
         <span class="c1"># only create Engine if we don&#39;t have a Connection</span>
         <span class="c1"># from the outside</span>
         <span class="n">connectable</span> <span class="o">=</span> <span class="n">engine_from_config</span><span class="p">(</span>
@@ -1453,79 +1453,48 @@
 <span class="k">def</span> <span class="nf">do_run_migrations</span><span class="p">(</span><span class="n">connection</span><span class="p">):</span>
     <span class="n">context</span><span class="o">.</span><span class="n">configure</span><span class="p">(</span><span class="n">connection</span><span class="o">=</span><span class="n">connection</span><span class="p">,</span> <span class="n">target_metadata</span><span class="o">=</span><span class="n">target_metadata</span><span class="p">)</span>
 
     <span class="k">with</span> <span class="n">context</span><span class="o">.</span><span class="n">begin_transaction</span><span class="p">():</span>
         <span class="n">context</span><span class="o">.</span><span class="n">run_migrations</span><span class="p">()</span>
 
 
-<span class="k">async</span> <span class="k">def</span> <span class="nf">run_migrations_online</span><span class="p">():</span>
-    <span class="sd">&quot;&quot;&quot;Run migrations in &#39;online&#39; mode.</span>
-
-<span class="sd">    In this scenario we need to create an Engine</span>
+<span class="k">async</span> <span class="k">def</span> <span class="nf">run_async_migrations</span><span class="p">():</span>
+    <span class="sd">&quot;&quot;&quot;In this scenario we need to create an Engine</span>
 <span class="sd">    and associate a connection with the context.</span>
 
 <span class="sd">    &quot;&quot;&quot;</span>
+
     <span class="n">connectable</span> <span class="o">=</span> <span class="n">async_engine_from_config</span><span class="p">(</span>
         <span class="n">config</span><span class="o">.</span><span class="n">get_section</span><span class="p">(</span><span class="n">config</span><span class="o">.</span><span class="n">config_ini_section</span><span class="p">),</span>
         <span class="n">prefix</span><span class="o">=</span><span class="s2">&quot;sqlalchemy.&quot;</span><span class="p">,</span>
         <span class="n">poolclass</span><span class="o">=</span><span class="n">pool</span><span class="o">.</span><span class="n">NullPool</span><span class="p">,</span>
     <span class="p">)</span>
 
     <span class="k">async</span> <span class="k">with</span> <span class="n">connectable</span><span class="o">.</span><span class="n">connect</span><span class="p">()</span> <span class="k">as</span> <span class="n">connection</span><span class="p">:</span>
         <span class="k">await</span> <span class="n">connection</span><span class="o">.</span><span class="n">run_sync</span><span class="p">(</span><span class="n">do_run_migrations</span><span class="p">)</span>
 
     <span class="k">await</span> <span class="n">connectable</span><span class="o">.</span><span class="n">dispose</span><span class="p">()</span>
 
 
-<span class="k">if</span> <span class="n">context</span><span class="o">.</span><span class="n">is_offline_mode</span><span class="p">():</span>
-    <span class="n">run_migrations_offline</span><span class="p">()</span>
-<span class="k">else</span><span class="p">:</span>
-    <span class="n">asyncio</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">run_migrations_online</span><span class="p">())</span>
+<span class="k">def</span> <span class="nf">run_migrations_online</span><span class="p">():</span>
+    <span class="sd">&quot;&quot;&quot;Run migrations in &#39;online&#39; mode.&quot;&quot;&quot;</span>
+
+    <span class="n">asyncio</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">run_async_migrations</span><span class="p">())</span>
 </pre></div>
 </div>
 <p>An async application can also interact with the Alembic api directly by using
 the SQLAlchemy <code class="docutils literal notranslate"><span class="pre">run_sync</span></code> method to adapt the non-async api of Alembic to
 an async consumer.</p>
 <section id="programmatic-api-use-connection-sharing-with-asyncio">
 <span id="connection-sharing-plus-asyncio"></span><h3>Programmatic API use (connection sharing) With Asyncio<a class="headerlink" href="#programmatic-api-use-connection-sharing-with-asyncio" title="Permalink to this heading">¶</a></h3>
 <p>Combining the examples of <a class="reference internal" href="#connection-sharing"><span class="std std-ref">Sharing a Connection across one or more programmatic migration commands</span></a> with <a class="reference internal" href="#asyncio-recipe"><span class="std std-ref">Using Asyncio with Alembic</span></a>
-together, and <code class="docutils literal notranslate"><span class="pre">env.py</span></code> as follows works:</p>
-<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">asyncio</span>
-
-<span class="kn">from</span> <span class="nn">sqlalchemy.ext.asyncio</span> <span class="kn">import</span> <span class="n">async_engine_from_config</span>
-
-<span class="c1"># ... no change required to the rest of the code</span>
-
-
-<span class="k">def</span> <span class="nf">do_run_migrations</span><span class="p">(</span><span class="n">connection</span><span class="p">):</span>
-    <span class="n">context</span><span class="o">.</span><span class="n">configure</span><span class="p">(</span><span class="n">connection</span><span class="o">=</span><span class="n">connection</span><span class="p">,</span> <span class="n">target_metadata</span><span class="o">=</span><span class="n">target_metadata</span><span class="p">)</span>
-
-    <span class="k">with</span> <span class="n">context</span><span class="o">.</span><span class="n">begin_transaction</span><span class="p">():</span>
-        <span class="n">context</span><span class="o">.</span><span class="n">run_migrations</span><span class="p">()</span>
-
-
-<span class="k">async</span> <span class="k">def</span> <span class="nf">run_async_migrations</span><span class="p">():</span>
-    <span class="n">connectable</span> <span class="o">=</span> <span class="n">async_engine_from_config</span><span class="p">(</span>
-        <span class="n">config</span><span class="o">.</span><span class="n">get_section</span><span class="p">(</span><span class="n">config</span><span class="o">.</span><span class="n">config_ini_section</span><span class="p">),</span>
-        <span class="n">prefix</span><span class="o">=</span><span class="s2">&quot;sqlalchemy.&quot;</span><span class="p">,</span>
-        <span class="n">poolclass</span><span class="o">=</span><span class="n">pool</span><span class="o">.</span><span class="n">NullPool</span><span class="p">,</span>
-    <span class="p">)</span>
-
-    <span class="k">async</span> <span class="k">with</span> <span class="n">connectable</span><span class="o">.</span><span class="n">connect</span><span class="p">()</span> <span class="k">as</span> <span class="n">connection</span><span class="p">:</span>
-        <span class="k">await</span> <span class="n">connection</span><span class="o">.</span><span class="n">run_sync</span><span class="p">(</span><span class="n">do_run_migrations</span><span class="p">)</span>
-
-    <span class="k">await</span> <span class="n">connectable</span><span class="o">.</span><span class="n">dispose</span><span class="p">()</span>
-
-
-<span class="k">def</span> <span class="nf">run_migrations_online</span><span class="p">():</span>
+together, the  <code class="docutils literal notranslate"><span class="pre">env.py</span></code> listed above can be updated as follows works:</p>
+<div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="k">def</span> <span class="nf">run_migrations_online</span><span class="p">():</span>
     <span class="sd">&quot;&quot;&quot;Run migrations in &#39;online&#39; mode.</span>
 
-<span class="sd">    In this scenario we need to create an Engine</span>
-<span class="sd">    and associate a connection with the context.</span>
-
 <span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="n">connectable</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">attributes</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;connection&quot;</span><span class="p">,</span> <span class="kc">None</span><span class="p">)</span>
 
     <span class="k">if</span> <span class="n">connectable</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
         <span class="n">asyncio</span><span class="o">.</span><span class="n">run</span><span class="p">(</span><span class="n">run_async_migrations</span><span class="p">())</span>
     <span class="k">else</span><span class="p">:</span>
@@ -1634,15 +1603,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="api/index.html" title="API Details"
              >next</a> |</li>
         <li class="right" >
           <a href="ops.html" title="Operation Reference"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Cookbook</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Cookbook
 ****** CookbookÂ¶ ******
 A collection of âHow-Tosâ highlighting popular ways to extend Alembic.
 Note
 This is a new section where we catalogue various âhow-tosâ based on user
 requests. It is often the case that users will request a feature only to learn
 it can be provided with a simple customization.
@@ -196,15 +196,15 @@
 Python file:
 from alembic import command, config
 
 cfg = config.Config("/path/to/yourapp/alembic.ini")
 with engine.begin() as connection:
     cfg.attributes['connection'] = connection
     command.upgrade(cfg, "head")
-Then in env.py:
+Then in env.py we can update run_migrations_online:
 def run_migrations_online():
     connectable = config.attributes.get('connection', None)
 
     if connectable is None:
         # only create Engine if we don't have a Connection
         # from the outside
         connectable = engine_from_config(
@@ -1316,77 +1316,46 @@
 def do_run_migrations(connection):
     context.configure(connection=connection, target_metadata=target_metadata)
 
     with context.begin_transaction():
         context.run_migrations()
 
 
-async def run_migrations_online():
-    """Run migrations in 'online' mode.
-
-    In this scenario we need to create an Engine
+async def run_async_migrations():
+    """In this scenario we need to create an Engine
     and associate a connection with the context.
 
     """
+
     connectable = async_engine_from_config(
         config.get_section(config.config_ini_section),
         prefix="sqlalchemy.",
         poolclass=pool.NullPool,
     )
 
     async with connectable.connect() as connection:
         await connection.run_sync(do_run_migrations)
 
     await connectable.dispose()
 
 
-if context.is_offline_mode():
-    run_migrations_offline()
-else:
-    asyncio.run(run_migrations_online())
+def run_migrations_online():
+    """Run migrations in 'online' mode."""
+
+    asyncio.run(run_async_migrations())
 An async application can also interact with the Alembic api directly by using
 the SQLAlchemy run_sync method to adapt the non-async api of Alembic to an
 async consumer.
 **** Programmatic API use (connection sharing) With AsyncioÂ¶ ****
 Combining the examples of Sharing_a_Connection_across_one_or_more_programmatic
-migration_commands with Using_Asyncio_with_Alembic together, and env.py as
-follows works:
-import asyncio
-
-from sqlalchemy.ext.asyncio import async_engine_from_config
-
-# ... no change required to the rest of the code
-
-
-def do_run_migrations(connection):
-    context.configure(connection=connection, target_metadata=target_metadata)
-
-    with context.begin_transaction():
-        context.run_migrations()
-
-
-async def run_async_migrations():
-    connectable = async_engine_from_config(
-        config.get_section(config.config_ini_section),
-        prefix="sqlalchemy.",
-        poolclass=pool.NullPool,
-    )
-
-    async with connectable.connect() as connection:
-        await connection.run_sync(do_run_migrations)
-
-    await connectable.dispose()
-
-
+migration_commands with Using_Asyncio_with_Alembic together, the env.py listed
+above can be updated as follows works:
 def run_migrations_online():
     """Run migrations in 'online' mode.
 
-    In this scenario we need to create an Engine
-    and associate a connection with the context.
-
     """
 
     connectable = config.attributes.get("connection", None)
 
     if connectable is None:
         asyncio.run(run_async_migrations())
     else:
@@ -1443,10 +1412,10 @@
 *** Next topic ***
 API_Details
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Cookbook
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/front.html` & `alembic-1.9.4/docs/front.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Front Matter &#8212; Alembic 1.9.3 documentation</title>
+    <title>Front Matter &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to Alembic’s documentation!"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -198,15 +198,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="tutorial.html" title="Tutorial"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="Welcome to Alembic’s documentation!"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Front Matter</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Front Matter
 ****** Front MatterÂ¶ ******
 Information about the Alembic project.
 ***** Project HomepageÂ¶ *****
 Alembic is hosted on GitHub at https://github.com/sqlalchemy/alembic under the
 SQLAlchemy organization.
 Releases and project status are available on Pypi at https://pypi.python.org/
@@ -94,10 +94,10 @@
 *** Next topic ***
 Tutorial
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Front Matter
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/genindex.html` & `alembic-1.9.4/docs/genindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Index &#8212; Alembic 1.9.3 documentation</title>
+    <title>Index &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -24,15 +24,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -990,15 +990,17 @@
         <li><a href="ops.html#alembic.operations.Operations.create_exclude_constraint.params.initially">(alembic.operations.Operations.create_exclude_constraint parameter)</a>
 </li>
         <li><a href="ops.html#alembic.operations.Operations.create_unique_constraint.params.initially">(alembic.operations.Operations.create_unique_constraint parameter)</a>
 </li>
       </ul></li>
       <li><a href="ops.html#alembic.operations.Operations.inline_literal">inline_literal() (alembic.operations.Operations method)</a>
 </li>
-      <li><a href="ops.html#alembic.operations.BatchOperations.alter_column.params.insert_before">insert_before (alembic.operations.BatchOperations.alter_column parameter)</a>, <a href="ops.html#alembic.operations.BatchOperations.alter_column.params.insert_before">[1]</a>
+      <li><a href="ops.html#alembic.operations.BatchOperations.alter_column.params.insert_after">insert_after (alembic.operations.BatchOperations.alter_column parameter)</a>
+</li>
+      <li><a href="ops.html#alembic.operations.BatchOperations.alter_column.params.insert_before">insert_before (alembic.operations.BatchOperations.alter_column parameter)</a>
 </li>
       <li><a href="ops.html#alembic.operations.Operations.invoke">invoke() (alembic.operations.Operations method)</a>
 </li>
       <li><a href="api/script.html#alembic.script.revision.Revision.is_base">is_base (alembic.script.revision.Revision property)</a>
 </li>
       <li><a href="api/script.html#alembic.script.revision.Revision.is_branch_point">is_branch_point (alembic.script.revision.Revision property)</a>
 </li>
@@ -1782,15 +1784,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Index
 ****** Index ******
 Symbols | A | B | C | D | E | F | G | H | I | K | L | M | N | O | P | Q | R | S
 | T | U | V | W
 ***** Symbols *****
     * **kw_(alembic.operations.Operations.create_index_parameter)
           o (alembic.operations.Operations.create_table_parameter)
@@ -298,39 +298,39 @@
     * head_(alembic.command.revision_parameter)                   * heads_
           o (alembic.script.ScriptDirectory.generate_revision       (alembic.script.revision.RevisionMap
             parameter)                                              attribute)
           o (alembic.script.ScriptDirectory.walk_revisions        * heads()_(in_module_alembic.command)
             parameter)                                            * history()_(in_module
                                                                     alembic.command)
 ***** I *****
-    * identity_attrs_ignore_(alembic.ddl.impl.DefaultImpl
-      attribute)                                                    * init()_(in_module_alembic.command)
-          o (alembic.ddl.mssql.MSSQLImpl_attribute)                 * initially_
-          o (alembic.ddl.postgresql.PostgresqlImpl_attribute)         (alembic.operations.Operations.create_check_constraint
-    * IdentityColumnDefault_(class_in_alembic.ddl.base)               parameter)
-    * implementation_for()_(alembic.operations.Operations_class           o (alembic.operations.Operations.create_exclude_constraint
-      method)                                                               parameter)
-    * ImplMeta_(class_in_alembic.ddl.impl)                                o (alembic.operations.Operations.create_unique_constraint
-    * imports_(alembic.autogenerate.api.AutogenContext                      parameter)
-      attribute)                                                    * inline_literal()_(alembic.operations.Operations_method)
-    * include_name_                                                 * insert_before_(alembic.operations.BatchOperations.alter_column
-      (alembic.runtime.environment.EnvironmentContext.configure       parameter), [1]
-      parameter)                                                    * invoke()_(alembic.operations.Operations_method)
-    * include_object_                                               * is_base_(alembic.script.revision.Revision_property)
-      (alembic.runtime.environment.EnvironmentContext.configure     * is_branch_point_(alembic.script.revision.Revision_property)
-      parameter)                                                    * is_head_(alembic.script.revision.Revision_property)
-    * include_schemas_                                              * is_merge_point_(alembic.script.revision.Revision_property)
-      (alembic.runtime.environment.EnvironmentContext.configure     * is_offline_mode()_
-      parameter)                                                      (alembic.runtime.environment.EnvironmentContext_method)
-    * index_name_(alembic.operations.Operations.create_index        * is_transactional_ddl()_
-      parameter)                                                      (alembic.runtime.environment.EnvironmentContext_method)
-          o (alembic.operations.Operations.drop_index               * iterate_revisions()_(alembic.script.revision.RevisionMap
-            parameter)                                                method)
-    * indicate_current_(alembic.command.history_parameter)                o (alembic.script.ScriptDirectory_method)
-    * info_(alembic.operations.ops.MigrateOperation_attribute)
+    * identity_attrs_ignore_(alembic.ddl.impl.DefaultImpl           * init()_(in_module_alembic.command)
+      attribute)                                                    * initially_
+          o (alembic.ddl.mssql.MSSQLImpl_attribute)                   (alembic.operations.Operations.create_check_constraint
+          o (alembic.ddl.postgresql.PostgresqlImpl_attribute)         parameter)
+    * IdentityColumnDefault_(class_in_alembic.ddl.base)                   o (alembic.operations.Operations.create_exclude_constraint
+    * implementation_for()_(alembic.operations.Operations_class             parameter)
+      method)                                                             o (alembic.operations.Operations.create_unique_constraint
+    * ImplMeta_(class_in_alembic.ddl.impl)                                  parameter)
+    * imports_(alembic.autogenerate.api.AutogenContext              * inline_literal()_(alembic.operations.Operations_method)
+      attribute)                                                    * insert_after_(alembic.operations.BatchOperations.alter_column
+    * include_name_                                                   parameter)
+      (alembic.runtime.environment.EnvironmentContext.configure     * insert_before_(alembic.operations.BatchOperations.alter_column
+      parameter)                                                      parameter)
+    * include_object_                                               * invoke()_(alembic.operations.Operations_method)
+      (alembic.runtime.environment.EnvironmentContext.configure     * is_base_(alembic.script.revision.Revision_property)
+      parameter)                                                    * is_branch_point_(alembic.script.revision.Revision_property)
+    * include_schemas_                                              * is_head_(alembic.script.revision.Revision_property)
+      (alembic.runtime.environment.EnvironmentContext.configure     * is_merge_point_(alembic.script.revision.Revision_property)
+      parameter)                                                    * is_offline_mode()_
+    * index_name_(alembic.operations.Operations.create_index          (alembic.runtime.environment.EnvironmentContext_method)
+      parameter)                                                    * is_transactional_ddl()_
+          o (alembic.operations.Operations.drop_index                 (alembic.runtime.environment.EnvironmentContext_method)
+            parameter)                                              * iterate_revisions()_(alembic.script.revision.RevisionMap
+    * indicate_current_(alembic.command.history_parameter)            method)
+    * info_(alembic.operations.ops.MigrateOperation_attribute)            o (alembic.script.ScriptDirectory_method)
     * ini_section_(alembic.config.Config_parameter)
 ***** K *****
     * kwargs_(alembic.ddl.impl.Params_attribute)
 ***** L *****
     * list_templates()_(in_module_alembic.command)                  * local_cols_
     * literal_binds_                                                  (alembic.operations.Operations.create_foreign_key
       (alembic.runtime.environment.EnvironmentContext.configure       parameter)
@@ -591,10 +591,10 @@
       (alembic.script.ScriptDirectory       (alembic.operations.Operations.create_exclude_constraint
       method)                               parameter)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Index
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/index.html` & `alembic-1.9.4/docs/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Welcome to Alembic’s documentation! &#8212; Alembic 1.9.3 documentation</title>
+    <title>Welcome to Alembic’s documentation! &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -29,15 +29,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to Alembic’s documentation!</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -305,14 +305,18 @@
 <li class="toctree-l3"><a class="reference internal" href="api/ddl.html#module-alembic.ddl.postgresql">Postgresql</a></li>
 <li class="toctree-l3"><a class="reference internal" href="api/ddl.html#module-alembic.ddl.sqlite">SQLite</a></li>
 </ul>
 </li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="changelog.html">Changelog</a><ul>
+<li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.9.4">1.9.4</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="changelog.html#change-1.9.4-bug">bug</a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.9.3">1.9.3</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="changelog.html#change-1.9.3-bug">bug</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="changelog.html#change-1.9.2">1.9.2</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="changelog.html#change-1.9.2-bug">bug</a></li>
 </ul>
@@ -853,15 +857,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="#">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Welcome to Alembic’s documentation!</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Welcome to Alembicâs documentation!
 ****** Welcome to Alembicâs documentation!Â¶ ******
 Alembic is a lightweight database migration tool for usage with the SQLAlchemy
 Database Toolkit for Python.
     * Front_Matter
           o Project_Homepage
           o Installation
@@ -217,14 +217,16 @@
                 # ImplMeta
                 # Params
                 # MySQL
                 # MS-SQL
                 # Postgresql
                 # SQLite
     * Changelog
+          o 1.9.4
+                # bug
           o 1.9.3
                 # bug
           o 1.9.2
                 # bug
           o 1.9.1
                 # bug
           o 1.9.0
@@ -511,10 +513,10 @@
 [q                   ] [Go]
 *** Next topic ***
 Front_Matter
 **** Navigation ****
     * index
     * modules |
     * next |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Welcome to Alembicâs documentation!
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/naming.html` & `alembic-1.9.4/docs/naming.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>The Importance of Naming Constraints &#8212; Alembic 1.9.3 documentation</title>
+    <title>The Importance of Naming Constraints &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="batch.html" title="Running “Batch” Migrations for SQLite and Other Databases"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="offline.html" title="Generating SQL Scripts (a.k.a. “Offline Mode”)"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">The Importance of Naming Constraints</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -351,15 +351,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="batch.html" title="Running “Batch” Migrations for SQLite and Other Databases"
              >next</a> |</li>
         <li class="right" >
           <a href="offline.html" title="Generating SQL Scripts (a.k.a. “Offline Mode”)"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">The Importance of Naming Constraints</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * The Importance of Naming Constraints
 ****** The Importance of Naming ConstraintsÂ¶ ******
 An important topic worth mentioning is that of constraint naming conventions.
 As weâve proceeded here, weâve talked about adding tables and columns, and
 weâve also hinted at lots of other operations listed in Operation_Reference
 such as those which support adding or dropping constraints like foreign keys
 and unique constraints. The way these constraints are referred to in migration
@@ -236,10 +236,10 @@
 *** Next topic ***
 Running_âBatchâ_Migrations_for_SQLite_and_Other_Databases
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * The Importance of Naming Constraints
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/offline.html` & `alembic-1.9.4/docs/offline.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Generating SQL Scripts (a.k.a. “Offline Mode”) &#8212; Alembic 1.9.3 documentation</title>
+    <title>Generating SQL Scripts (a.k.a. “Offline Mode”) &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="naming.html" title="The Importance of Naming Constraints"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Auto Generating Migrations"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Generating SQL Scripts (a.k.a. “Offline Mode”)</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -234,15 +234,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="naming.html" title="The Importance of Naming Constraints"
              >next</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Auto Generating Migrations"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Generating SQL Scripts (a.k.a. “Offline Mode”)</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Generating SQL Scripts (a.k.a. âOffline Modeâ)
 ****** Generating SQL Scripts (a.k.a. âOffline Modeâ)Â¶ ******
 A major capability of Alembic is to generate migrations as SQL scripts, instead
 of running them against the database - this is also referred to as offline
 mode. This is a critical feature when working in large organizations where
 access to DDL is restricted, and SQL scripts must be handed off to DBAs.
 Alembic makes this easy via the --sql option passed to any upgrade or downgrade
@@ -153,10 +153,10 @@
 *** Next topic ***
 The_Importance_of_Naming_Constraints
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Generating SQL Scripts (a.k.a. âOffline Modeâ)
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/ops.html` & `alembic-1.9.4/docs/ops.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Operation Reference &#8212; Alembic 1.9.3 documentation</title>
+    <title>Operation Reference &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="cookbook.html" title="Cookbook"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="branches.html" title="Working with Branches"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Operation Reference</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -1297,15 +1297,15 @@
 <dd class="field-odd"><ul class="simple">
 <li><p><span class="target" id="alembic.operations.BatchOperations.alter_column.params.insert_before"></span><strong>insert_before</strong><a class="paramlink headerlink reference internal" href="#alembic.operations.BatchOperations.alter_column.params.insert_before">¶</a> – <p>String name of an existing column which this
 column should be placed before, when creating the new table.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.4.0.</span></p>
 </div>
 </p></li>
-<li><p><span class="target" id="alembic.operations.BatchOperations.alter_column.params.insert_before"></span><strong>insert_before</strong><a class="paramlink headerlink reference internal" href="#alembic.operations.BatchOperations.alter_column.params.insert_before">¶</a> – <p>String name of an existing column which this
+<li><p><span class="target" id="alembic.operations.BatchOperations.alter_column.params.insert_after"></span><strong>insert_after</strong><a class="paramlink headerlink reference internal" href="#alembic.operations.BatchOperations.alter_column.params.insert_after">¶</a> – <p>String name of an existing column which this
 column should be placed after, when creating the new table.  If
 both <a class="reference internal" href="#alembic.operations.BatchOperations.alter_column.params.insert_before" title="alembic.operations.BatchOperations.alter_column"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">BatchOperations.alter_column.insert_before</span></code></a>
 and <a class="reference internal" href="#alembic.operations.BatchOperations.alter_column.params.insert_after" title="alembic.operations.BatchOperations.alter_column"><code class="xref py py-paramref docutils literal notranslate"><span class="pre">BatchOperations.alter_column.insert_after</span></code></a> are
 omitted, the column is inserted after the last existing column
 in the table.</p>
 <div class="versionadded">
 <p><span class="versionmodified added">New in version 1.4.0.</span></p>
@@ -1580,15 +1580,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="cookbook.html" title="Cookbook"
              >next</a> |</li>
         <li class="right" >
           <a href="branches.html" title="Working with Branches"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Operation Reference</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Operation Reference
 ****** Operation ReferenceÂ¶ ******
 This file provides documentation on Alembic migration directives.
 The directives here are used within user-defined migration files, within the
 upgrade() and downgrade() functions, as well as any functions further invoked
 by those.
 All directives exist as methods on a class called Operations. When migration
@@ -957,10 +957,10 @@
 *** Next topic ***
 Cookbook
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Operation Reference
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/py-modindex.html` & `alembic-1.9.4/docs/py-modindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Python Module Index &#8212; Alembic 1.9.3 documentation</title>
+    <title>Python Module Index &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -27,15 +27,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -166,15 +166,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Python Module Index</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Python Module Index
 ****** Python Module Index ******
 a
      
     a
 [-] alembic
         alembic.command
@@ -33,10 +33,10 @@
         alembic.script.revision
         alembic.script.write_hooks
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Python Module Index
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/search.html` & `alembic-1.9.4/docs/search.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Search &#8212; Alembic 1.9.3 documentation</title>
+    <title>Search &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -30,15 +30,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -90,15 +90,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Search</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -5,19 +5,19 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Search
 ****** Search ******
 Please activate JavaScript to enable the search functionality.
 Searching for multiple words only shows matches that contain all words.
 [q                   ] [search]
 **** Navigation ****
     * index
     * modules |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Search
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/docs/searchindex.js` & `alembic-1.9.4/docs/searchindex.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -719,14 +719,16 @@
         "delet": [1, 11, 12, 13, 18],
         "befor": [1, 2, 3, 7, 10, 11, 12, 13, 18, 19],
         "perspect": [2, 7, 11],
         "you": [2, 7, 8, 9, 11, 12, 13, 14, 16, 19],
         "instanti": [2, 6, 7],
         "oper": [2, 3, 4, 6, 7, 8, 10, 11, 12, 14, 15, 19],
         "file_": [2, 9, 17],
+        "o": [2, 11, 12, 17, 19],
+        "pathlik": 2,
         "ini_sect": 2,
         "output_buff": [2, 3, 7, 17],
         "textio": [2, 3, 7],
         "_io": 2,
         "textiowrapp": 2,
         "w": [2, 3, 9, 17],
         "encod": [2, 7, 12, 19],
@@ -945,16 +947,16 @@
         "recreat": [3, 10, 12, 13, 18],
         "proce": [3, 7, 9, 10, 11, 12, 13, 14, 18],
         "start_migr": 3,
         "run_migr": [3, 5, 7, 9, 12, 13, 17, 18],
         "per": [3, 6, 7, 9, 12, 18],
         "static_output": [3, 7],
         "type_arg_extract": 3,
-        "numer": [3, 9, 12, 18],
         "decim": [3, 9, 12, 19],
+        "numer": [3, 9, 12, 18],
         "implmeta": [3, 4, 15],
         "classnam": 3,
         "dict_": 3,
         "param": [3, 4, 15],
         "token0": 3,
         "alia": [3, 11],
         "field": [3, 12, 13, 19],
@@ -997,16 +999,16 @@
         "batchoper": [3, 5, 10, 12, 15, 18],
         "create_exclude_constraint": [3, 12, 15, 18],
         "constraint_typ": [3, 16],
         "from_constraint": 3,
         "to_constraint": 3,
         "postgresqlcolumntyp": 3,
         "postgresqlimpl": [3, 11, 13],
-        "float": [3, 12],
         "precis": [3, 9, 12],
+        "float": [3, 12],
         "visit_column_com": 3,
         "pgddlcompil": 3,
         "sqliteimpl": 3,
         "cast": [3, 12],
         "pysqlit": [3, 12],
         "http": [3, 12, 13, 14],
         "bug": [3, 15, 19],
@@ -1155,15 +1157,15 @@
         "_proxytransact": 7,
         "contextmanag": 7,
         "enclos": [7, 12],
         "right": [7, 11, 12, 16, 18],
         "regardless": [7, 9, 10, 12, 18, 19],
         "is_transactional_ddl": 7,
         "noth": [7, 8, 11, 12, 19],
-        "is_offline_mod": [7, 13, 17],
+        "is_offline_mod": [7, 17],
         "onlin": [7, 10, 12, 13, 17, 18],
         "roll": [7, 13],
         "manipul": [7, 10, 12],
         "dialect_nam": [7, 17],
         "dialect_opt": [7, 12],
         "transaction_per_migr": [7, 12],
         "template_arg": [7, 12],
@@ -1802,15 +1804,14 @@
         "delta": 11,
         "lineag": [11, 12, 13],
         "semi": 11,
         "network": 11,
         "sever": [11, 12, 19],
         "pertin": 11,
         "version_path_separ": [11, 12, 19],
-        "o": [11, 12, 17, 19],
         "pathsep": [11, 12, 19],
         "greater": [11, 12, 13, 18],
         "older": [11, 12, 13, 14, 18],
         "underneath": 11,
         "up_revis": [11, 13],
         "3cac04ae8714_create_networking_branch": 11,
         "didn": [11, 12],
@@ -1853,40 +1854,53 @@
         "29f8": 11,
         "2a95": 11,
         "crazi": 11,
         "henc": [11, 12],
         "carefulli": [11, 19],
         "thoughtfulli": 11,
         "februari": 12,
+        "16": [12, 13],
         "2023": 12,
+        "ongo": 12,
+        "collaps": 12,
+        "whitespac": 12,
+        "parenthesi": 12,
+        "aggress": 12,
+        "strip": 12,
+        "1177": 12,
+        "substr": 12,
+        "mi": 12,
+        "erron": 12,
+        "1180": 12,
+        "regress": 12,
+        "courtesi": 12,
+        "brendan": 12,
+        "gann": 12,
         "went": 12,
         "with_vari": 12,
         "variant": 12,
         "1167": 12,
         "januari": 12,
         "14": 12,
         "stub": [12, 13, 18],
         "overload": 12,
         "1146": 12,
         "1147": 12,
-        "regress": 12,
         "caus": [12, 13],
         "1145": 12,
         "transform": 12,
         "getdat": 12,
         "1152": 12,
         "decemb": 12,
         "23": 12,
         "2022": 12,
         "backslash": [12, 18],
-        "mi": 12,
         "better": [12, 16],
         "paren": 12,
         "15": [12, 18],
-        "courtesi": 12,
         "nathan": 12,
         "louie": 12,
         "724": 12,
         "tox": 12,
         "passenv": 12,
         "codebas": 12,
         "mypi": 12,
@@ -2057,15 +2071,14 @@
         "hold": [12, 13, 19],
         "honor": 12,
         "rollback": [12, 17],
         "829": 12,
         "alphabet": 12,
         "827": 12,
         "rewritten": 12,
-        "ongo": 12,
         "clariti": 12,
         "ambigu": 12,
         "huge": 12,
         "thank": 12,
         "simon": 12,
         "bowli": 12,
         "impress": 12,
@@ -2092,24 +2105,22 @@
         "prepend_sys_path": [12, 14, 19],
         "prepend": [12, 19],
         "channel": 12,
         "interpret": [12, 14, 19],
         "pytest": 12,
         "cli": 12,
         "797": 12,
-        "erron": 12,
         "789": 12,
         "29": 12,
         "786": 12,
         "assort": 12,
         "787": 12,
         "788": 12,
         "757": 12,
         "overlap": 12,
-        "substr": 12,
         "downrev": 12,
         "784": 12,
         "782": 12,
         "19": 12,
         "780": 12,
         "18": [12, 13],
         "surround": [12, 18],
@@ -2162,15 +2173,14 @@
         "append_column": 12,
         "disallow": 12,
         "mssql_drop_foreign_kei": [12, 18],
         "typo": 12,
         "oleg": 12,
         "shigorin": 12,
         "716": 12,
-        "16": [12, 13],
         "669": 12,
         "668": 12,
         "605": 12,
         "charset": [12, 13],
         "671": 12,
         "portion": 12,
         "reject": 12,
@@ -2275,15 +2285,14 @@
         "dev": 12,
         "5534": 12,
         "bump": 12,
         "minimum": 12,
         "leverag": 12,
         "june": 12,
         "25": [12, 13],
-        "parenthesi": 12,
         "constant": 12,
         "maximum": 12,
         "entail": 12,
         "elimin": 12,
         "round": 12,
         "trip": 12,
         "mariadb": 12,
@@ -2463,15 +2472,14 @@
         "appeas": 12,
         "flake8": 12,
         "393": 12,
         "affin": 12,
         "redund": 12,
         "391": 12,
         "pep8": 12,
-        "whitespac": 12,
         "symlink": 12,
         "jiri": 12,
         "kuncar": 12,
         "load_dialect_impl": 12,
         "significantli": 12,
         "395": 12,
         "asc": 12,
@@ -3134,20 +3142,19 @@
         "experiment": 13,
         "asyncpg": 13,
         "script_directory_her": 13,
         "ext": 13,
         "async_engine_from_config": 13,
         "rest": 13,
         "do_run_migr": 13,
+        "run_async_migr": 13,
         "await": 13,
         "run_sync": 13,
         "dispos": 13,
-        "run_migrations_offlin": [13, 17, 19],
         "interact": [13, 18],
-        "run_async_migr": 13,
         "create_async_engin": 13,
         "run_upgrad": 13,
         "run_async_upgrad": 13,
         "async_engin": 13,
         "aiosqlit": 13,
         "publish": 14,
         "virtual": [14, 19],
@@ -3228,14 +3235,15 @@
         "version_fil": 17,
         "dirnam": 17,
         "txt": 17,
         "current_vers": 17,
         "end_vers": 17,
         "design": [17, 18, 19],
         "hack": 17,
+        "run_migrations_offlin": [17, 19],
         "bottom": 17,
         "db_1": 17,
         "db_2": 17,
         "db1": 17,
         "stderr": [17, 19],
         "wrote": 17,
         "session": 17,
@@ -3739,14 +3747,15 @@
             [18, 2, 1, "", "create_unique_constraint"],
             [18, 2, 1, "", "drop_column"],
             [18, 2, 1, "", "drop_constraint"],
             [18, 2, 1, "", "drop_index"],
             [18, 2, 1, "", "drop_table_comment"]
         ],
         "alembic.operations.BatchOperations.alter_column.params": [
+            [18, 4, 1, "", "insert_after"],
             [18, 4, 1, "", "insert_before"]
         ],
         "alembic.operations.BatchOperations.create_table_comment.params": [
             [18, 4, 1, "", "comment"],
             [18, 4, 1, "", "existing_comment"]
         ],
         "alembic.operations.BatchOperations.drop_table_comment.params": [
@@ -4337,26 +4346,26 @@
         "syntax": 11,
         "set": 11,
         "up": [11, 13],
         "depend": [11, 14],
         "changelog": 12,
         "1": 12,
         "9": 12,
-        "3": 12,
+        "4": 12,
         "bug": [12, 14],
+        "3": 12,
         "2": 12,
         "0": 12,
         "featur": 12,
         "8": 12,
         "usecas": 12,
         "7": 12,
         "6": 12,
         "misc": 12,
         "5": 12,
-        "4": 12,
         "remov": 12,
         "11": 12,
         "10": 12,
         "cookbook": 13,
         "build": 13,
         "an": [13, 19],
         "date": 13,
@@ -4645,18 +4654,19 @@
         ],
         "Branch Dependencies": [
             [11, "branch-dependencies"]
         ],
         "Changelog": [
             [12, "changelog"]
         ],
-        "1.9.3": [
-            [12, "change-1.9.3"]
+        "1.9.4": [
+            [12, "change-1.9.4"]
         ],
         "bug": [
+            [12, "change-1.9.4-bug"],
             [12, "change-1.9.3-bug"],
             [12, "change-1.9.2-bug"],
             [12, "change-1.9.1-bug"],
             [12, "change-1.9.0-bug"],
             [12, "change-1.8.1-bug"],
             [12, "change-1.8.0-bug"],
             [12, "change-1.7.7-bug"],
@@ -4751,14 +4761,17 @@
             [12, "change-0.3.2-bug"],
             [12, "change-0.3.1-bug"],
             [12, "change-0.2.2-bug"],
             [12, "change-0.2.1-bug"],
             [12, "change-0.2.0-bug"],
             [12, "change-0.1.1-bug"]
         ],
+        "1.9.3": [
+            [12, "change-1.9.3"]
+        ],
         "1.9.2": [
             [12, "change-1.9.2"]
         ],
         "1.9.1": [
             [12, "change-1.9.1"]
         ],
         "1.9.0": [
```

### Comparing `alembic-1.9.3/docs/tutorial.html` & `alembic-1.9.4/docs/tutorial.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html>
 
 <html lang="en">
   <head>
     <meta charset="utf-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 
-    <title>Tutorial &#8212; Alembic 1.9.3 documentation</title>
+    <title>Tutorial &#8212; Alembic 1.9.4 documentation</title>
     <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/nature_override.css" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/changelog.css" />
     <link rel="stylesheet" type="text/css" href="_static/sphinx_paramlinks.css" />
     <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
     <script src="_static/doctools.js"></script>
@@ -33,15 +33,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Auto Generating Migrations"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Tutorial</a></li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
@@ -719,15 +719,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="autogenerate.html" title="Auto Generating Migrations"
              >next</a> |</li>
         <li class="right" >
           <a href="front.html" title="Front Matter"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.3 documentation</a> &#187;</li>
+        <li class="nav-item nav-item-0"><a href="index.html">Alembic 1.9.4 documentation</a> &#187;</li>
         <li class="nav-item nav-item-this"><a href="">Tutorial</a></li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2010-2023, Mike Bayer.
       Created using <a href="https://www.sphinx-doc.org/">Sphinx</a> 6.1.3.
     </div>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Tutorial
 ****** TutorialÂ¶ ******
 Alembic provides for the creation, management, and invocation of change
 management scripts for a relational database, using SQLAlchemy as the
 underlying engine. This tutorial will provide a full introduction to the theory
 and usage of this tool.
 To begin, make sure Alembic is installed as described at Installation. As
@@ -580,10 +580,10 @@
 *** Next topic ***
 Auto_Generating_Migrations
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * Alembic_1.9.3_documentation »
+    * Alembic_1.9.4_documentation »
     * Tutorial
 © Copyright 2010-2023, Mike Bayer. Created using Sphinx 6.1.3.
```

### Comparing `alembic-1.9.3/pyproject.toml` & `alembic-1.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/setup.cfg` & `alembic-1.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/_large_map.py` & `alembic-1.9.4/tests/_large_map.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/conftest.py` & `alembic-1.9.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/requirements.py` & `alembic-1.9.4/tests/requirements.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_autogen_composition.py` & `alembic-1.9.4/tests/test_autogen_composition.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_autogen_diffs.py` & `alembic-1.9.4/tests/test_autogen_diffs.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from sqlalchemy import DATE
 from sqlalchemy import DateTime
 from sqlalchemy import DECIMAL
 from sqlalchemy import Enum
 from sqlalchemy import FLOAT
 from sqlalchemy import ForeignKey
 from sqlalchemy import ForeignKeyConstraint
+from sqlalchemy import func
 from sqlalchemy import Index
 from sqlalchemy import inspect
 from sqlalchemy import INTEGER
 from sqlalchemy import Integer
 from sqlalchemy import JSON
 from sqlalchemy import LargeBinary
 from sqlalchemy import MetaData
@@ -909,14 +910,45 @@
         eq_(diff[0][0][0], "modify_default")
 
     @testing.combinations(
         (VARCHAR(30), text("'some default'")),
         (VARCHAR(30), "some default"),
         (VARCHAR(30), text("'//slash'")),
         (VARCHAR(30), text("'has '' quote'")),
+        (
+            VARCHAR(30),
+            func.substring("name", 1, 3),
+            testing.exclusions.only_on(["mssql", "postgresql"]),
+        ),  # note no space
+        (
+            VARCHAR(30),
+            text("substring('name',1,3)"),
+            testing.exclusions.only_on(["mssql", "postgresql"]),
+        ),  # note no space
+        (
+            VARCHAR(30),
+            text("substring('name', 1, 3)"),
+            testing.exclusions.only_on(["mssql", "postgresql"]),
+        ),  # note spaces
+        (
+            VARCHAR(50),
+            text(
+                "substring(user_name(),"  # note no space
+                "charindex('',user_name())+(1),len(user_name()))"
+            ),
+            testing.exclusions.only_on("mssql"),
+        ),
+        (
+            VARCHAR(50),
+            text(
+                "substring(user_name(), "  # note space
+                "charindex('',user_name())+(1),len(user_name()))"
+            ),
+            testing.exclusions.only_on("mssql"),
+        ),
         (DateTime(), text("(getdate())"), testing.exclusions.only_on("mssql")),
         (
             DateTime(),
             text("(now())"),
             testing.exclusions.only_on("postgresql", "sqlite"),
         ),
         (Integer(), text("15")),
```

### Comparing `alembic-1.9.3/tests/test_autogen_indexes.py` & `alembic-1.9.4/tests/test_autogen_indexes.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_autogen_render.py` & `alembic-1.9.4/tests/test_autogen_render.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_batch.py` & `alembic-1.9.4/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_bulk_insert.py` & `alembic-1.9.4/tests/test_bulk_insert.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_command.py` & `alembic-1.9.4/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_config.py` & `alembic-1.9.4/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_editor.py` & `alembic-1.9.4/tests/test_editor.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_environment.py` & `alembic-1.9.4/tests/test_environment.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_external_dialect.py` & `alembic-1.9.4/tests/test_external_dialect.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_impl.py` & `alembic-1.9.4/tests/test_impl.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_mssql.py` & `alembic-1.9.4/tests/test_mssql.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_mysql.py` & `alembic-1.9.4/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_offline_environment.py` & `alembic-1.9.4/tests/test_offline_environment.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_op.py` & `alembic-1.9.4/tests/test_op.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_op_naming_convention.py` & `alembic-1.9.4/tests/test_op_naming_convention.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_oracle.py` & `alembic-1.9.4/tests/test_oracle.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_post_write.py` & `alembic-1.9.4/tests/test_post_write.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_postgresql.py` & `alembic-1.9.4/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_revision.py` & `alembic-1.9.4/tests/test_revision.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_script_consumption.py` & `alembic-1.9.4/tests/test_script_consumption.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_script_production.py` & `alembic-1.9.4/tests/test_script_production.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_sqlite.py` & `alembic-1.9.4/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_stubs.py` & `alembic-1.9.4/tests/test_stubs.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_version_table.py` & `alembic-1.9.4/tests/test_version_table.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tests/test_version_traversal.py` & `alembic-1.9.4/tests/test_version_traversal.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tools/write_pyi.py` & `alembic-1.9.4/tools/write_pyi.py`

 * *Files identical despite different names*

### Comparing `alembic-1.9.3/tox.ini` & `alembic-1.9.4/tox.ini`

 * *Files identical despite different names*

