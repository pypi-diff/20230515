# Comparing `tmp/ersilia-0.1.1.tar.gz` & `tmp/ersilia-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ersilia-0.1.1.tar", last modified: Mon Oct 10 08:46:09 2022, max compression
+gzip compressed data, was "dist/ersilia-0.1.8.tar", last modified: Mon May 15 11:09:11 2023, max compression
```

## Comparing `ersilia-0.1.1.tar` & `ersilia-0.1.8.tar`

### file list

```diff
@@ -1,206 +1,236 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-10-10 08:46:00.000000 ersilia-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-10-10 08:46:09.000000 ersilia-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5374 2022-10-10 08:46:00.000000 ersilia-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/
--rw-r--r--   0 runner    (1001) docker     (121)     1600 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/_clean_static_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     1777 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/_clean_version.py
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/_static_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     6458 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/app/
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/app/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/app/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/app/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/app/blocks/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/auth/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      132 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1408 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (121)      763 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/api.py
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     1808 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/clear.py
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/close.py
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/delete.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/example.py
--rw-r--r--   0 runner    (1001) docker     (121)     1332 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/fetch.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     1442 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/serve.py
--rw-r--r--   0 runner    (1001) docker     (121)      817 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/cli/commands/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/commands/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      579 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/create_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      901 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/echo.py
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/cli/messages.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/core/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3803 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/core/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13984 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/core/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/core/modelbase.py
--rw-r--r--   0 runner    (1001) docker     (121)     1747 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/core/session.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/db/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/db/disk/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/disk/fetched.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/db/environments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4383 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/environments/localdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    10813 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/environments/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/db/hubdata/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/hubdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/hubdata/localslugs.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/db/hubdata/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3454 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/default.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/bundle/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/bundle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5129 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/bundle/bundle.py
--rw-r--r--   0 runner    (1001) docker     (121)    10524 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/bundle/repo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2718 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/bundle/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/content/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6087 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     5505 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/catalog.py
--rw-r--r--   0 runner    (1001) docker     (121)     3533 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     1855 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/slug.py
--rw-r--r--   0 runner    (1001) docker     (121)     2413 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/content/table_update.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/delete/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/delete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8217 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/delete/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/fetch/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/
--rw-r--r--   0 runner    (1001) docker     (121)      286 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1016 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3564 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/get.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/lake.py
--rw-r--r--   0 runner    (1001) docker     (121)     6420 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/modify.py
--rw-r--r--   0 runner    (1001) docker     (121)     1912 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/pack.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/prepare.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/sniff.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/actions/toolize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3028 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/fetch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/hub/fetch/pack/
--rw-r--r--   0 runner    (1001) docker     (121)     6155 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/pack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3955 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/pack/mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     7973 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/hub/fetch/pack/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/io/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1795 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (121)     7813 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/input.py
--rw-r--r--   0 runner    (1001) docker     (121)    12787 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2216 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/pure.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/io/readers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23662 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/readers/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     2089 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/readers/pyinput.py
--rw-r--r--   0 runner    (1001) docker     (121)      806 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/shape.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/io/types/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6120 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/compound.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/io/types/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      323 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/examples/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      799 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/examples/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)   461883 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/examples/compound.tsv
--rw-r--r--   0 runner    (1001) docker     (121)  2622625 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/examples/protein.tsv
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/naive.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/io/types/protein.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/lake/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/lake/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      779 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/lake/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/lake/interface.py
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/lake/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/publish/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7963 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/deploy.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/lake.py
--rw-r--r--   0 runner    (1001) docker     (121)     2709 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/publish.py
--rw-r--r--   0 runner    (1001) docker     (121)     2967 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/rebase.py
--rw-r--r--   0 runner    (1001) docker     (121)     2290 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/publish/store.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/serve/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12450 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/serve/api.py
--rw-r--r--   0 runner    (1001) docker     (121)    10811 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/serve/autoservice.py
--rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/serve/schema.py
--rw-r--r--   0 runner    (1001) docker     (121)    12214 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/serve/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/setup/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4087 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/baseconda.py
--rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/basedocker.py
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/setup/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)      472 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)      813 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/git.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/requirements/isaura.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/setup/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      949 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/setup/utils/clone.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/clear.py
--rw-r--r--   0 runner    (1001) docker     (121)    12603 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/conda.py
--rw-r--r--   0 runner    (1001) docker     (121)     7083 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/cron.py
--rw-r--r--   0 runner    (1001) docker     (121)      646 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     5454 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (121)     7889 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/dvc.py
--rw-r--r--   0 runner    (1001) docker     (121)      430 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/utils/identifiers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/arbitrary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3815 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/compound.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/file.py
--rw-r--r--   0 runner    (1001) docker     (121)      593 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/long.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/model.py
--rw-r--r--   0 runner    (1001) docker     (121)      800 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/protein.py
--rw-r--r--   0 runner    (1001) docker     (121)      931 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/short.py
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/identifiers/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/import.py
--rw-r--r--   0 runner    (1001) docker     (121)     9560 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/installers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     2307 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/ports.py
--rw-r--r--   0 runner    (1001) docker     (121)      494 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia/utils/supp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/supp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/supp/conda_env_resolve.py
--rw-r--r--   0 runner    (1001) docker     (121)     2358 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/terminal.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1607 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/venv.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/versioning.py
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-10 08:46:00.000000 ersilia-0.1.1/ersilia/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/ersilia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6953 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4793 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-10-10 08:46:08.000000 ersilia-0.1.1/ersilia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-10 08:46:09.000000 ersilia-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-10-10 08:46:00.000000 ersilia-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:09.000000 ersilia-0.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-10 08:46:00.000000 ersilia-0.1.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-10-10 08:46:00.000000 ersilia-0.1.1/test/test_content.py
--rw-r--r--   0 runner    (1001) docker     (121)     3829 2022-10-10 08:46:00.000000 ersilia-0.1.1/test/test_inputs.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-10-10 08:46:00.000000 ersilia-0.1.1/test/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 11:08:58.000000 ersilia-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 11:09:11.000000 ersilia-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-15 11:08:58.000000 ersilia-0.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 11:09:10.000000 ersilia-0.1.8/ersilia/_static_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/app/blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/app/blocks/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/close.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/cli/commands/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/commands/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/create_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/echo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/cli/messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14818 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/modelbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/core/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/disk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/disk/fetched.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/localdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/environments/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/db/hubdata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/localslugs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/db/hubdata/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/bundle/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/bundle/status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22669 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1855 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/slug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/content/table_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/delete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8299 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/delete/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/inform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/modify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/prepare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6157 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/sniff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/actions/toolize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5781 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/hub/fetch/pack/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13657 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/pure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23662 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/readers/pyinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/shape.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/types/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/compound.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/io/types/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)   461883 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/compound.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2622625 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/examples/protein.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/io/types/protein.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/lake/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/lake/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7963 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/dockerhub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/lake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/rebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/publish/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/serve/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13028 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/autoservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13366 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/serve/services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/baseconda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/basedocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/bentoml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/eospath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/isaura.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/requirements/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/setup/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/setup/utils/clone.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/cli_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13926 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12209 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/dvc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/card_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/catalog_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/clear_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/close_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/delete_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/example_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/fetch_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/handle_undecorated_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/issue_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/serve_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/setup_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/exceptions_utils/throw_ersilia_exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/identifiers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/arbitrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/identifiers/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9561 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/installers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia/utils/supp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/supp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/supp/conda_env_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-15 11:08:58.000000 ersilia-0.1.8/ersilia/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-15 11:09:11.000000 ersilia-0.1.8/ersilia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 11:09:11.000000 ersilia-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-15 11:08:58.000000 ersilia-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 11:09:11.000000 ersilia-0.1.8/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-15 11:08:58.000000 ersilia-0.1.8/test/test_models.py
```

### Comparing `ersilia-0.1.1/PKG-INFO` & `ersilia-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,435 +1,482 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6572 7369  : 2.1.Name: ersi
 00000020: 6c69 610a 5665 7273 696f 6e3a 2030 2e31  lia.Version: 0.1
-00000030: 2e31 0a53 756d 6d61 7279 3a20 4120 6875  .1.Summary: A hu
+00000030: 2e38 0a53 756d 6d61 7279 3a20 4120 6875  .8.Summary: A hu
 00000040: 6220 6f66 2041 492f 4d4c 206d 6f64 656c  b of AI/ML model
 00000050: 7320 666f 7220 6f70 656e 2073 6f75 7263  s for open sourc
 00000060: 6520 6472 7567 2064 6973 636f 7665 7279  e drug discovery
 00000070: 2061 6e64 2067 6c6f 6261 6c20 6865 616c   and global heal
 00000080: 7468 0a48 6f6d 652d 7061 6765 3a20 6874  th.Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f65 7273 696c 6961 2d6f 732f 6572 7369  /ersilia-os/ersi
 000000b0: 6c69 610a 4175 7468 6f72 3a20 4572 7369  lia.Author: Ersi
 000000c0: 6c69 6120 4f70 656e 2053 6f75 7263 6520  lia Open Source 
 000000d0: 496e 6974 6961 7469 7665 0a41 7574 686f  Initiative.Autho
-000000e0: 722d 656d 6169 6c3a 206d 6971 7565 6c40  r-email: miquel@
-000000f0: 6572 7369 6c69 612e 696f 0a4c 6963 656e  ersilia.io.Licen
-00000100: 7365 3a20 4d49 540a 5072 6f6a 6563 742d  se: MIT.Project-
-00000110: 5552 4c3a 204c 616e 6469 6e67 2070 6167  URL: Landing pag
-00000120: 652c 2068 7474 7073 3a2f 2f65 7273 696c  e, https://ersil
-00000130: 6961 2e69 6f0a 5072 6f6a 6563 742d 5552  ia.io.Project-UR
-00000140: 4c3a 204d 6f64 656c 732c 2068 7474 7073  L: Models, https
-00000150: 3a2f 2f65 7273 696c 6961 2e69 6f2f 6d6f  ://ersilia.io/mo
-00000160: 6465 6c2d 6875 620a 5072 6f6a 6563 742d  del-hub.Project-
-00000170: 5552 4c3a 2053 6f75 7263 6520 436f 6465  URL: Source Code
-00000180: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000190: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
-000001a0: 6572 7369 6c69 612f 0a44 6573 6372 6970  ersilia/.Descrip
-000001b0: 7469 6f6e 3a20 3c64 6976 2069 643d 2274  tion: <div id="t
-000001c0: 6f70 223e 3c2f 6469 763e 0a20 2020 2020  op"></div>.     
-000001d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000001e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001f0: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-00000200: 6961 2f62 6c6f 622f 6d61 7374 6572 2f61  ia/blob/master/a
-00000210: 7373 6574 732f 4572 7369 6c69 615f 506c  ssets/Ersilia_Pl
-00000220: 756d 2e70 6e67 2220 6865 6967 6874 3d22  um.png" height="
-00000230: 3730 223e 0a20 2020 2020 2020 200a 2020  70">.        .  
-00000240: 2020 2020 2020 2320 5765 6c63 6f6d 6520        # Welcome 
-00000250: 746f 2074 6865 2045 7273 696c 6961 204d  to the Ersilia M
-00000260: 6f64 656c 2048 7562 210a 2020 2020 2020  odel Hub!.      
-00000270: 2020 0a20 2020 2020 2020 205b 215b 446f    .        [![Do
-00000280: 6e61 7465 5d28 6874 7470 733a 2f2f 696d  nate](https://im
-00000290: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000002a0: 6765 2f44 6f6e 6174 652d 5061 7950 616c  ge/Donate-PayPal
-000002b0: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
-000002c0: 7073 3a2f 2f77 7777 2e70 6179 7061 6c2e  ps://www.paypal.
-000002d0: 636f 6d2f 756b 2f66 756e 6472 6169 7365  com/uk/fundraise
-000002e0: 722f 6368 6172 6974 792f 3431 3435 3031  r/charity/414501
-000002f0: 3229 205b 215b 436f 6e74 7269 6275 746f  2) [![Contributo
-00000300: 7220 436f 7665 6e61 6e74 5d28 6874 7470  r Covenant](http
-00000310: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000320: 696f 2f62 6164 6765 2f43 6f6e 7472 6962  io/badge/Contrib
-00000330: 7574 6f72 2532 3043 6f76 656e 616e 742d  utor%20Covenant-
-00000340: 7632 2e30 2532 3061 646f 7074 6564 2d66  v2.0%20adopted-f
-00000350: 6636 3962 342e 7376 6729 5d28 434f 4445  f69b4.svg)](CODE
-00000360: 5f4f 465f 434f 4e44 5543 542e 6d64 2920  _OF_CONDUCT.md) 
-00000370: 5b21 5b4c 6963 656e 7365 3a20 4147 504c  [![License: AGPL
+000000e0: 722d 656d 6169 6c3a 2068 656c 6c6f 4065  r-email: hello@e
+000000f0: 7273 696c 6961 2e69 6f0a 4c69 6365 6e73  rsilia.io.Licens
+00000100: 653a 2047 504c 7633 0a50 726f 6a65 6374  e: GPLv3.Project
+00000110: 2d55 524c 3a20 4c61 6e64 696e 6720 7061  -URL: Landing pa
+00000120: 6765 2c20 6874 7470 733a 2f2f 6572 7369  ge, https://ersi
+00000130: 6c69 612e 696f 0a50 726f 6a65 6374 2d55  lia.io.Project-U
+00000140: 524c 3a20 4d6f 6465 6c73 2c20 6874 7470  RL: Models, http
+00000150: 733a 2f2f 6572 7369 6c69 612e 696f 2f6d  s://ersilia.io/m
+00000160: 6f64 656c 2d68 7562 0a50 726f 6a65 6374  odel-hub.Project
+00000170: 2d55 524c 3a20 536f 7572 6365 2043 6f64  -URL: Source Cod
+00000180: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+00000190: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+000001a0: 2f65 7273 696c 6961 2f0a 4465 7363 7269  /ersilia/.Descri
+000001b0: 7074 696f 6e3a 203c 6469 7620 6964 3d22  ption: <div id="
+000001c0: 746f 7022 3e3c 2f64 6976 3e0a 2020 2020  top"></div>.    
+000001d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000001e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001f0: 2f65 7273 696c 6961 2d6f 732f 6572 7369  /ersilia-os/ersi
+00000200: 6c69 612f 626c 6f62 2f6d 6173 7465 722f  lia/blob/master/
+00000210: 6173 7365 7473 2f45 7273 696c 6961 5f50  assets/Ersilia_P
+00000220: 6c75 6d2e 706e 6722 2068 6569 6768 743d  lum.png" height=
+00000230: 2237 3022 3e0a 2020 2020 2020 2020 0a20  "70">.        . 
+00000240: 2020 2020 2020 2023 2057 656c 636f 6d65         # Welcome
+00000250: 2074 6f20 7468 6520 4572 7369 6c69 6120   to the Ersilia 
+00000260: 4d6f 6465 6c20 4875 6221 0a20 2020 2020  Model Hub!.     
+00000270: 2020 200a 2020 2020 2020 2020 5b21 5b44     .        [![D
+00000280: 6f6e 6174 655d 2868 7474 7073 3a2f 2f69  onate](https://i
+00000290: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002a0: 6467 652f 446f 6e61 7465 2d50 6179 5061  dge/Donate-PayPa
+000002b0: 6c2d 6772 6565 6e2e 7376 6729 5d28 6874  l-green.svg)](ht
+000002c0: 7470 733a 2f2f 7777 772e 7061 7970 616c  tps://www.paypal
+000002d0: 2e63 6f6d 2f75 6b2f 6675 6e64 7261 6973  .com/uk/fundrais
+000002e0: 6572 2f63 6861 7269 7479 2f34 3134 3530  er/charity/41450
+000002f0: 3132 2920 5b21 5b43 6f6e 7472 6962 7574  12) [![Contribut
+00000300: 6f72 2043 6f76 656e 616e 745d 2868 7474  or Covenant](htt
+00000310: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000320: 2e69 6f2f 6261 6467 652f 436f 6e74 7269  .io/badge/Contri
+00000330: 6275 746f 7225 3230 436f 7665 6e61 6e74  butor%20Covenant
+00000340: 2d76 322e 3025 3230 6164 6f70 7465 642d  -v2.0%20adopted-
+00000350: 6666 3639 6234 2e73 7667 295d 2843 4f44  ff69b4.svg)](COD
+00000360: 455f 4f46 5f43 4f4e 4455 4354 2e6d 6429  E_OF_CONDUCT.md)
+00000370: 205b 215b 4c69 6365 6e73 653a 2047 504c   [![License: GPL
 00000380: 2076 335d 2868 7474 7073 3a2f 2f69 6d67   v3](https://img
 00000390: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000003a0: 652f 4c69 6365 6e73 652d 4147 504c 2532  e/License-AGPL%2
-000003b0: 3076 332d 7965 6c6c 6f77 2e73 7667 295d  0v3-yellow.svg)]
-000003c0: 2868 7474 7073 3a2f 2f77 7777 2e67 6e75  (https://www.gnu
-000003d0: 2e6f 7267 2f6c 6963 656e 7365 732f 6167  .org/licenses/ag
-000003e0: 706c 2d33 2e30 290a 2020 2020 2020 2020  pl-3.0).        
-000003f0: 0a20 2020 2020 2020 205b 215b 646f 6375  .        [![docu
-00000400: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00000410: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000420: 6f2f 6261 6467 652f 2d44 6f63 756d 656e  o/badge/-Documen
-00000430: 7461 7469 6f6e 2d70 7572 706c 653f 6c6f  tation-purple?lo
-00000440: 676f 3d72 6561 642d 7468 652d 646f 6373  go=read-the-docs
-00000450: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00000460: 295d 2868 7474 7073 3a2f 2f65 7273 696c  )](https://ersil
-00000470: 6961 2e67 6974 626f 6f6b 2e69 6f2f 6572  ia.gitbook.io/er
-00000480: 7369 6c69 612d 626f 6f6b 2f29 205b 215b  silia-book/) [![
-00000490: 5079 5049 2076 6572 7369 6f6e 2066 7572  PyPI version fur
-000004a0: 792e 696f 5d28 6874 7470 733a 2f2f 6261  y.io](https://ba
-000004b0: 6467 652e 6675 7279 2e69 6f2f 7079 2f65  dge.fury.io/py/e
-000004c0: 7273 696c 6961 2e73 7667 295d 2868 7474  rsilia.svg)](htt
-000004d0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-000004e0: 2e6f 7267 2f70 7970 692f 6572 7369 6c69  .org/pypi/ersili
-000004f0: 612f 2920 5b21 5b50 7974 686f 6e20 332e  a/) [![Python 3.
-00000500: 375d 2868 7474 7073 3a2f 2f69 6d67 2e73  7](https://img.s
-00000510: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000520: 7079 7468 6f6e 2d33 2e37 2d62 6c75 652e  python-3.7-blue.
-00000530: 7376 6729 5d28 6874 7470 733a 2f2f 7777  svg)](https://ww
-00000540: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
-00000550: 6e6c 6f61 6473 2f72 656c 6561 7365 2f70  nloads/release/p
-00000560: 7974 686f 6e2d 3337 302f 2920 5b21 5b43  ython-370/) [![C
-00000570: 6f64 6520 7374 796c 653a 2062 6c61 636b  ode style: black
-00000580: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000590: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-000005a0: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-000005b0: 6b2d 3030 3030 3030 2e73 7667 3f6c 6f67  k-000000.svg?log
-000005c0: 6f3d 5079 7468 6f6e 266c 6f67 6f43 6f6c  o=Python&logoCol
-000005d0: 6f72 3d77 6869 7465 295d 2868 7474 7073  or=white)](https
-000005e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7073  ://github.com/ps
-000005f0: 662f 626c 6163 6b29 205b 215b 4769 7470  f/black) [![Gitp
-00000600: 6f64 2052 6561 6479 2d74 6f2d 436f 6465  od Ready-to-Code
-00000610: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000620: 6965 6c64 732e 696f 2f62 6164 6765 2f47  ields.io/badge/G
-00000630: 6974 706f 642d 7265 6164 792d 2d74 6f2d  itpod-ready--to-
-00000640: 2d63 6f64 652d 626c 7565 3f6c 6f67 6f3d  -code-blue?logo=
-00000650: 6769 7470 6f64 295d 2868 7474 7073 3a2f  gitpod)](https:/
-00000660: 2f67 6974 706f 642e 696f 2f23 6874 7470  /gitpod.io/#http
-00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00000680: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
-00000690: 6129 0a20 2020 2020 2020 200a 2020 2020  a).        .    
-000006a0: 2020 2020 2323 2320 5461 626c 6520 6f66      ### Table of
-000006b0: 2043 6f6e 7465 6e74 733a 0a20 2020 2020   Contents:.     
-000006c0: 2020 2031 2e20 5b50 726f 6a65 6374 2044     1. [Project D
-000006d0: 6573 6372 6970 7469 6f6e 5d28 6874 7470  escription](http
-000006e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-000006f0: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
-00000700: 6123 7072 6f6a 6563 742d 6465 7363 7269  a#project-descri
-00000710: 7074 696f 6e29 0a20 2020 2020 2020 2032  ption).        2
-00000720: 2e20 5b49 6e73 7461 6c6c 6174 696f 6e5d  . [Installation]
-00000730: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000740: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
-00000750: 7273 696c 6961 2369 6e73 7461 6c6c 6174  rsilia#installat
-00000760: 696f 6e29 0a20 2020 2020 2020 2033 2e20  ion).        3. 
-00000770: 5b43 6f6e 7472 6962 7574 655d 2868 7474  [Contribute](htt
-00000780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000790: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-000007a0: 6961 2363 6f6e 7472 6962 7574 6529 0a20  ia#contribute). 
-000007b0: 2020 2020 2020 2034 2e20 5b4c 6963 656e         4. [Licen
-000007c0: 7365 2061 6e64 2063 6974 6174 696f 6e5d  se and citation]
-000007d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007e0: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
-000007f0: 7273 696c 6961 236c 6963 656e 7365 2d61  rsilia#license-a
-00000800: 6e64 2d63 6974 6174 696f 6e29 0a20 2020  nd-citation).   
-00000810: 2020 2020 2035 2e20 5b41 626f 7574 2075       5. [About u
-00000820: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000830: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
-00000840: 2f65 7273 696c 6961 2361 626f 7574 2d75  /ersilia#about-u
-00000850: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
-00000860: 2020 2020 2320 5072 6f6a 6563 7420 4465      # Project De
-00000870: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
-00000880: 2020 5468 6520 4572 7369 6c69 6120 4d6f    The Ersilia Mo
-00000890: 6465 6c20 4875 6220 6973 2061 2075 6e69  del Hub is a uni
-000008a0: 6669 6564 2070 6c61 7466 6f72 6d20 6f66  fied platform of
-000008b0: 2070 7265 2d74 7261 696e 6564 2041 492f   pre-trained AI/
-000008c0: 4d4c 206d 6f64 656c 7320 666f 7220 696e  ML models for in
-000008d0: 6665 6374 696f 7573 2061 6e64 206e 6567  fectious and neg
-000008e0: 6c65 6374 6564 2064 6973 6561 7365 2072  lected disease r
-000008f0: 6573 6561 7263 682e 2054 6865 2065 6e64  esearch. The end
-00000900: 2067 6f61 6c20 6973 2074 6f20 7072 6f76   goal is to prov
-00000910: 6964 6520 616e 206f 7065 6e2d 736f 7572  ide an open-sour
-00000920: 6365 2c20 6e6f 2d63 6f64 6520 736f 6c75  ce, no-code solu
-00000930: 7469 6f6e 2074 6f20 6163 6365 7373 2041  tion to access A
-00000940: 492f 4d4c 206d 6f64 656c 7320 746f 2061  I/ML models to a
-00000950: 6363 656c 6572 6174 6520 6472 7567 2064  ccelerate drug d
-00000960: 6973 636f 7665 7279 2e20 5468 6520 6d6f  iscovery. The mo
-00000970: 6465 6c73 2065 6d62 6564 6465 6420 696e  dels embedded in
-00000980: 2074 6865 2068 7562 2069 6e63 6c75 6465   the hub include
-00000990: 2062 6f74 6820 6d6f 6465 6c73 2070 7562   both models pub
-000009a0: 6c69 7368 6564 2069 6e20 7468 6520 6c69  lished in the li
-000009b0: 7465 7261 7475 7265 2028 7769 7468 2061  terature (with a
-000009c0: 7070 726f 7072 6961 7465 2074 6869 7264  ppropriate third
-000009d0: 2070 6172 7479 2061 636b 6e6f 776c 6564   party acknowled
-000009e0: 6765 6d65 6e74 2920 616e 6420 6d6f 6465  gement) and mode
-000009f0: 6c73 2064 6576 656c 6f70 6564 2062 7920  ls developed by 
-00000a00: 7468 6520 4572 7369 6c69 6120 7465 616d  the Ersilia team
-00000a10: 206f 7220 636f 6e74 7269 6275 746f 7273   or contributors
-00000a20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00000a30: 2020 202a 2052 6561 6420 6d6f 7265 2061     * Read more a
-00000a40: 626f 7574 2074 6865 2070 726f 6a65 6374  bout the project
-00000a50: 2069 6e20 7468 6520 5b45 7273 696c 6961   in the [Ersilia
-00000a60: 2042 6f6f 6b5d 2868 7474 7073 3a2f 2f65   Book](https://e
-00000a70: 7273 696c 6961 2e67 6974 626f 6f6b 2e69  rsilia.gitbook.i
-00000a80: 6f2f 6572 7369 6c69 612d 626f 6f6b 2f29  o/ersilia-book/)
-00000a90: 0a20 2020 2020 2020 202a 2042 726f 7773  .        * Brows
-00000aa0: 6520 6176 6169 6c61 626c 6520 6d6f 6465  e available mode
-00000ab0: 6c73 2069 6e20 7468 6520 5b45 7273 696c  ls in the [Ersil
-00000ac0: 6961 204d 6f64 656c 2048 7562 5d28 6874  ia Model Hub](ht
-00000ad0: 7470 733a 2f2f 6572 7369 6c69 612e 696f  tps://ersilia.io
-00000ae0: 2f6d 6f64 656c 2d68 7562 2f29 0a20 2020  /model-hub/).   
-00000af0: 2020 2020 203c 7020 616c 6967 6e3d 2272       <p align="r
-00000b00: 6967 6874 223e 283c 6120 6872 6566 3d22  ight">(<a href="
-00000b10: 2374 6f70 223e 6261 636b 2074 6f20 746f  #top">back to to
-00000b20: 703c 2f61 3e29 3c2f 703e 0a20 2020 2020  p</a>)</p>.     
-00000b30: 2020 200a 2020 2020 2020 2020 2320 5175     .        # Qu
-00000b40: 6963 6b20 7374 6172 7420 6775 6964 650a  ick start guide.
-00000b50: 2020 2020 2020 2020 506c 6561 7365 2063          Please c
-00000b60: 6865 636b 2074 6865 2070 6163 6b61 6765  heck the package
-00000b70: 2072 6571 7569 7265 6d65 6e74 7320 696e   requirements in
-00000b80: 2074 6865 205b 496e 7374 616c 6c61 7469   the [Installati
-00000b90: 6f6e 2047 7569 6465 5d28 6874 7470 733a  on Guide](https:
-00000ba0: 2f2f 6572 7369 6c69 612e 6769 7462 6f6f  //ersilia.gitboo
-00000bb0: 6b2e 696f 2f65 7273 696c 6961 2d62 6f6f  k.io/ersilia-boo
-00000bc0: 6b2f 7175 6963 6b2d 7374 6172 742f 696e  k/quick-start/in
-00000bd0: 7374 616c 6c61 7469 6f6e 292e 2054 6865  stallation). The
-00000be0: 206e 6578 7420 7374 6570 7320 6172 6520   next steps are 
-00000bf0: 6120 7175 6963 6b73 7461 7274 2067 7569  a quickstart gui
-00000c00: 6465 2074 6f20 696e 7374 616c 6c69 6e67  de to installing
-00000c10: 2045 7273 696c 6961 2e0a 2020 2020 2020   Ersilia..      
-00000c20: 2020 0a20 2020 2020 2020 2031 2e20 4372    .        1. Cr
-00000c30: 6561 7465 2061 2063 6f6e 6461 2065 6e76  eate a conda env
-00000c40: 6972 6f6e 6d65 6e74 2061 6e64 2061 6374  ironment and act
-00000c50: 6976 6174 6520 6974 0a20 2020 2020 2020  ivate it.       
-00000c60: 2060 6060 0a20 2020 2020 2020 2063 6f6e   ```.        con
-00000c70: 6461 2063 7265 6174 6520 2d6e 2065 7273  da create -n ers
-00000c80: 696c 6961 2070 7974 686f 6e3d 332e 370a  ilia python=3.7.
-00000c90: 2020 2020 2020 2020 636f 6e64 6120 6163          conda ac
-00000ca0: 7469 7661 7465 2065 7273 696c 6961 0a20  tivate ersilia. 
-00000cb0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000cc0: 2020 2032 2e20 436c 6f6e 6520 7468 6973     2. Clone this
-00000cd0: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-00000ce0: 696e 7374 616c 6c20 7769 7468 2070 6970  install with pip
-00000cf0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00000d00: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
-00000d10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000d20: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
-00000d30: 696c 6961 2e67 6974 0a20 2020 2020 2020  ilia.git.       
-00000d40: 2063 6420 6572 7369 6c69 610a 2020 2020   cd ersilia.    
-00000d50: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-00000d60: 2d65 202e 0a20 2020 2020 2020 2060 6060  -e ..        ```
-00000d70: 200a 2020 2020 2020 2020 332e 204f 6e63   .        3. Onc
-00000d80: 6520 7468 6520 4572 7369 6c69 6120 4d6f  e the Ersilia Mo
-00000d90: 6465 6c20 4875 6220 6973 2069 6e73 7461  del Hub is insta
-00000da0: 6c6c 6564 2c20 796f 7520 6361 6e20 7573  lled, you can us
-00000db0: 6520 7468 6520 434c 4920 746f 2072 756e  e the CLI to run
-00000dc0: 2070 7265 6469 6374 696f 6e73 2e20 4669   predictions. Fi
-00000dd0: 7273 742c 2073 656c 6563 7420 6120 6d6f  rst, select a mo
-00000de0: 6465 6c20 6672 6f6d 2074 6865 205b 4572  del from the [Er
-00000df0: 7369 6c69 6120 4d6f 6465 6c20 4875 625d  silia Model Hub]
-00000e00: 2868 7474 7073 3a2f 2f65 7273 696c 6961  (https://ersilia
-00000e10: 2e69 6f2f 6d6f 6465 6c2d 6875 622f 2920  .io/model-hub/) 
-00000e20: 616e 6420 2a2a 6665 7463 682a 2a20 6974  and **fetch** it
-00000e30: 3a0a 2020 2020 2020 2020 6060 600a 2020  :.        ```.  
-00000e40: 2020 2020 2020 6572 7369 6c69 6120 6665        ersilia fe
-00000e50: 7463 6820 6368 656d 7072 6f70 2d61 6e74  tch chemprop-ant
-00000e60: 6962 696f 7469 630a 2020 2020 2020 2020  ibiotic.        
-00000e70: 6060 600a 2020 2020 2020 2020 342e 2047  ```.        4. G
-00000e80: 656e 6572 6174 6520 6120 6665 7720 2835  enerate a few (5
-00000e90: 2920 6578 616d 706c 6520 6d6f 6c65 6375  ) example molecu
-00000ea0: 6c65 732c 2074 6f20 6265 2075 7365 6420  les, to be used 
-00000eb0: 6173 2069 6e70 7574 2e20 5468 6520 2a2a  as input. The **
-00000ec0: 6578 616d 706c 652a 2a20 636f 6d6d 616e  example** comman
-00000ed0: 6420 7769 6c6c 2067 656e 6572 6174 6520  d will generate 
-00000ee0: 7468 6520 6164 6571 7561 7465 2069 6e70  the adequate inp
-00000ef0: 7574 2066 6f72 2074 6865 206d 6f64 656c  ut for the model
-00000f00: 2069 6e20 7573 650a 2020 2020 2020 2020   in use.        
-00000f10: 6060 600a 2020 2020 2020 2020 6572 7369  ```.        ersi
-00000f20: 6c69 6120 6578 616d 706c 6520 6368 656d  lia example chem
-00000f30: 7072 6f70 2d61 6e74 6962 696f 7469 6320  prop-antibiotic 
-00000f40: 2d6e 2035 202d 6620 6d79 5f6d 6f6c 6563  -n 5 -f my_molec
-00000f50: 756c 6573 2e63 7376 0a20 2020 2020 2020  ules.csv.       
-00000f60: 2060 6060 0a20 2020 2020 2020 2035 2e20   ```.        5. 
-00000f70: 5468 656e 2c20 2a2a 7365 7276 652a 2a20  Then, **serve** 
-00000f80: 796f 7572 206d 6f64 656c 3a0a 2020 2020  your model:.    
-00000f90: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000fa0: 6572 7369 6c69 6120 7365 7276 6520 6368  ersilia serve ch
-00000fb0: 656d 7072 6f70 2d61 6e74 6962 696f 7469  emprop-antibioti
-00000fc0: 630a 2020 2020 2020 2020 6060 600a 2020  c.        ```.  
-00000fd0: 2020 2020 2020 362e 2041 6e64 2072 756e        6. And run
-00000fe0: 2074 6865 2070 7265 6469 6374 696f 6e20   the prediction 
-00000ff0: 2a2a 4150 492a 2a3a 0a20 2020 2020 2020  **API**:.       
-00001000: 2060 6060 0a20 2020 2020 2020 2065 7273   ```.        ers
-00001010: 696c 6961 2061 7069 202d 6920 6d79 5f6d  ilia api -i my_m
-00001020: 6f6c 6563 756c 6573 2e63 7376 202d 6f20  olecules.csv -o 
-00001030: 6d79 5f70 7265 6469 6374 696f 6e73 2e63  my_predictions.c
-00001040: 7376 0a20 2020 2020 2020 2060 6060 0a20  sv.        ```. 
-00001050: 2020 2020 2020 2037 2e20 4669 6e61 6c6c         7. Finall
-00001060: 792c 202a 2a63 6c6f 7365 2a2a 2074 6865  y, **close** the
-00001070: 2073 6572 7669 6365 2077 6865 6e20 796f   service when yo
-00001080: 7520 6172 6520 646f 6e65 2e0a 2020 2020  u are done..    
-00001090: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000010a0: 6572 7369 6c69 6120 636c 6f73 650a 2020  ersilia close.  
-000010b0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-000010c0: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
-000010d0: 6520 7365 6520 7468 6520 5b45 7273 696c  e see the [Ersil
-000010e0: 6961 2042 6f6f 6b5d 2868 7474 7073 3a2f  ia Book](https:/
-000010f0: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
-00001100: 2e69 6f2f 6572 7369 6c69 612d 626f 6f6b  .io/ersilia-book
-00001110: 2f29 2066 6f72 206d 6f72 6520 6578 616d  /) for more exam
-00001120: 706c 6573 2061 6e64 2064 6574 6169 6c65  ples and detaile
-00001130: 6420 6578 706c 616e 6174 696f 6e73 2e0a  d explanations..
-00001140: 2020 2020 2020 2020 3c70 2061 6c69 676e          <p align
-00001150: 3d22 7269 6768 7422 3e28 3c61 2068 7265  ="right">(<a hre
-00001160: 663d 2223 746f 7022 3e62 6163 6b20 746f  f="#top">back to
-00001170: 2074 6f70 3c2f 613e 293c 2f70 3e0a 2020   top</a>)</p>.  
-00001180: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00001190: 2043 6f6e 7472 6962 7574 650a 2020 2020   Contribute.    
-000011a0: 2020 2020 5468 6520 4572 7369 6c69 6120      The Ersilia 
-000011b0: 4d6f 6465 6c20 4875 6220 6973 2061 2046  Model Hub is a F
-000011c0: 7265 652c 204f 7065 6e20 536f 7572 6365  ree, Open Source
-000011d0: 2053 6f66 7477 6172 6520 616e 6420 7765   Software and we
-000011e0: 2068 6967 686c 7920 7661 6c75 6520 6e65   highly value ne
-000011f0: 7720 636f 6e74 7269 6275 746f 7273 2e20  w contributors. 
-00001200: 5468 6572 6520 6172 6520 7365 7665 7261  There are severa
-00001210: 6c20 7761 7973 2069 6e20 7768 6963 6820  l ways in which 
-00001220: 796f 7520 6361 6e20 636f 6e74 7269 6275  you can contribu
-00001230: 7465 2074 6f20 7468 6520 7072 6f6a 6563  te to the projec
-00001240: 743a 0a20 2020 2020 2020 202a 2041 2067  t:.        * A g
-00001250: 6f6f 6420 706c 6163 6520 746f 2073 7461  ood place to sta
-00001260: 7274 2069 7320 6368 6563 6b69 6e67 206f  rt is checking o
-00001270: 7065 6e20 5b69 7373 7565 735d 2868 7474  pen [issues](htt
-00001280: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001290: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-000012a0: 6961 2f69 7373 7565 7329 2e20 0a20 2020  ia/issues). .   
-000012b0: 2020 2020 202a 2049 6620 796f 7520 6861       * If you ha
-000012c0: 7665 2069 6465 6e74 6966 6965 6420 6120  ve identified a 
-000012d0: 6275 6720 696e 2074 6865 2063 6f64 652c  bug in the code,
-000012e0: 2070 6c65 6173 6520 6f70 656e 2061 206e   please open a n
-000012f0: 6577 2069 7373 7565 2075 7369 6e67 2074  ew issue using t
-00001300: 6865 2062 7567 2074 656d 706c 6174 652e  he bug template.
-00001310: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
-00001320: 7520 7761 6e74 2074 6f20 696e 636f 7270  u want to incorp
-00001330: 6f72 6174 6520 6120 6e65 7720 6d6f 6465  orate a new mode
-00001340: 6c20 696e 2074 6865 2070 6c61 7466 6f72  l in the platfor
-00001350: 6d2c 206f 7065 6e20 6120 6e65 7720 6973  m, open a new is
-00001360: 7375 6520 7573 696e 6720 7468 6520 6d6f  sue using the mo
-00001370: 6465 6c20 7265 7175 6573 7420 7465 6d70  del request temp
-00001380: 6c61 7465 206f 7220 636f 6e74 6163 7420  late or contact 
-00001390: 7573 2075 7369 6e67 2074 6865 2066 6f6c  us using the fol
-000013a0: 6c6f 7769 6e67 205b 666f 726d 5d28 6874  lowing [form](ht
-000013b0: 7470 733a 2f2f 7777 772e 6572 7369 6c69  tps://www.ersili
-000013c0: 612e 696f 2f72 6571 7565 7374 2d6d 6f64  a.io/request-mod
-000013d0: 656c 290a 2020 2020 2020 2020 2a20 5368  el).        * Sh
-000013e0: 6172 6520 616e 7920 6665 6564 6261 636b  are any feedback
-000013f0: 2077 6974 6820 7468 6520 636f 6d6d 756e   with the commun
-00001400: 6974 7920 7573 696e 6720 5b47 6974 4875  ity using [GitHu
-00001410: 6220 4469 7363 7573 7369 6f6e 735d 2868  b Discussions](h
-00001420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001430: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
-00001440: 696c 6961 2f64 6973 6375 7373 696f 6e73  ilia/discussions
-00001450: 2920 666f 7220 7468 6520 7072 6f6a 6563  ) for the projec
-00001460: 740a 2020 2020 2020 2020 2a20 4368 6563  t.        * Chec
-00001470: 6b20 6f75 7220 5b43 6f6e 7472 6962 7574  k our [Contribut
-00001480: 696e 6720 4775 6964 655d 2868 7474 7073  ing Guide](https
-00001490: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
-000014a0: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
-000014b0: 2f62 6c6f 622f 6d61 7374 6572 2f43 4f4e  /blob/master/CON
-000014c0: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
-000014d0: 7220 6d6f 7265 2064 6574 6169 6c73 0a20  r more details. 
-000014e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000014f0: 5468 6520 4572 7369 6c69 6120 4f70 656e  The Ersilia Open
-00001500: 2053 6f75 7263 6520 496e 6974 6961 7469   Source Initiati
-00001510: 7665 2061 6468 6572 6573 2074 6f20 7468  ve adheres to th
-00001520: 6520 5b43 6f6e 7472 6962 7574 6f72 2043  e [Contributor C
-00001530: 6f76 656e 616e 745d 2868 7474 7073 3a2f  ovenant](https:/
-00001540: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
-00001550: 2e69 6f2f 6572 7369 6c69 612d 7769 6b69  .io/ersilia-wiki
-00001560: 2f63 6f64 652d 6f66 2d63 6f6e 6475 6374  /code-of-conduct
-00001570: 2920 636f 6465 206f 6620 636f 6e64 7563  ) code of conduc
-00001580: 742e 0a20 2020 2020 2020 203c 7020 616c  t..        <p al
-00001590: 6967 6e3d 2272 6967 6874 223e 283c 6120  ign="right">(<a 
-000015a0: 6872 6566 3d22 2374 6f70 223e 6261 636b  href="#top">back
-000015b0: 2074 6f20 746f 703c 2f61 3e29 3c2f 703e   to top</a>)</p>
-000015c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015d0: 2020 2320 4c69 6365 6e73 6520 616e 6420    # License and 
-000015e0: 6369 7461 7469 6f6e 0a20 2020 2020 2020  citation.       
-000015f0: 2054 6869 7320 7265 706f 7369 746f 7279   This repository
-00001600: 2069 7320 6f70 656e 2d73 6f75 7263 6564   is open-sourced
-00001610: 2075 6e64 6572 2074 6865 205b 4750 4c2d   under the [GPL-
-00001620: 3320 4c69 6365 6e73 655d 2868 7474 7073  3 License](https
-00001630: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
-00001640: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
-00001650: 2f62 6c6f 622f 6d61 7374 6572 2f4c 4943  /blob/master/LIC
-00001660: 454e 5345 292e 0a20 2020 2020 2020 2050  ENSE)..        P
-00001670: 6c65 6173 6520 5b63 6974 6520 7573 5d28  lease [cite us](
-00001680: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001690: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
-000016a0: 7369 6c69 612f 626c 6f62 2f6d 6173 7465  silia/blob/maste
-000016b0: 722f 4349 5441 5449 4f4e 2e63 6666 2920  r/CITATION.cff) 
-000016c0: 6966 2079 6f75 2075 7365 2069 742e 0a20  if you use it.. 
-000016d0: 2020 2020 2020 203c 7020 616c 6967 6e3d         <p align=
-000016e0: 2272 6967 6874 223e 283c 6120 6872 6566  "right">(<a href
-000016f0: 3d22 2374 6f70 223e 6261 636b 2074 6f20  ="#top">back to 
-00001700: 746f 703c 2f61 3e29 3c2f 703e 0a20 2020  top</a>)</p>.   
-00001710: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00001720: 4162 6f75 7420 7573 0a20 2020 2020 2020  About us.       
-00001730: 2054 6865 205b 4572 7369 6c69 6120 4f70   The [Ersilia Op
-00001740: 656e 2053 6f75 7263 6520 496e 6974 6961  en Source Initia
-00001750: 7469 7665 5d28 6874 7470 733a 2f2f 6572  tive](https://er
-00001760: 7369 6c69 612e 696f 2920 6973 2061 204e  silia.io) is a N
-00001770: 6f6e 2050 726f 6669 7420 4f72 6761 6e69  on Profit Organi
-00001780: 7a61 7469 6f6e 2028 5b31 3139 3232 3636  zation ([1192266
-00001790: 5d28 6874 7470 733a 2f2f 7265 6769 7374  ](https://regist
-000017a0: 6572 2d6f 662d 6368 6172 6974 6965 732e  er-of-charities.
-000017b0: 6368 6172 6974 7963 6f6d 6d69 7373 696f  charitycommissio
-000017c0: 6e2e 676f 762e 756b 2f63 6861 7269 7479  n.gov.uk/charity
-000017d0: 2d73 6561 7263 682f 2d2f 6368 6172 6974  -search/-/charit
-000017e0: 792d 6465 7461 696c 732f 3531 3730 3635  y-details/517065
-000017f0: 372f 6675 6c6c 2d70 7269 6e74 2929 2077  7/full-print)) w
-00001800: 6974 6820 7468 6520 6d69 7373 696f 6e20  ith the mission 
-00001810: 6973 2074 6f20 6571 7569 7020 6c61 6273  is to equip labs
-00001820: 2c20 756e 6976 6572 7369 7469 6573 2061  , universities a
-00001830: 6e64 2063 6c69 6e69 6373 2069 6e20 4c4d  nd clinics in LM
-00001840: 4943 2077 6974 6820 4149 2f4d 4c20 746f  IC with AI/ML to
-00001850: 6f6c 7320 666f 7220 696e 6665 6374 696f  ols for infectio
-00001860: 7573 2064 6973 6561 7365 2072 6573 6561  us disease resea
-00001870: 7263 682e 0a20 2020 2020 2020 200a 2020  rch..        .  
-00001880: 2020 2020 2020 5b48 656c 7020 7573 5d28        [Help us](
-00001890: 6874 7470 733a 2f2f 7777 772e 6572 7369  https://www.ersi
-000018a0: 6c69 612e 696f 2f64 6f6e 6174 6529 2061  lia.io/donate) a
-000018b0: 6368 6965 7665 206f 7572 206d 6973 7369  chieve our missi
-000018c0: 6f6e 206f 7220 5b76 6f6c 756e 7465 6572  on or [volunteer
-000018d0: 5d28 6874 7470 733a 2f2f 7777 772e 6572  ](https://www.er
-000018e0: 7369 6c69 612e 696f 2f76 6f6c 756e 7465  silia.io/volunte
-000018f0: 6572 2920 7769 7468 2075 7321 0a20 2020  er) with us!.   
-00001900: 2020 2020 200a 2020 2020 2020 2020 3c70       .        <p
-00001910: 2061 6c69 676e 3d22 7269 6768 7422 3e28   align="right">(
-00001920: 3c61 2068 7265 663d 2223 746f 7022 3e62  <a href="#top">b
-00001930: 6163 6b20 746f 2074 6f70 3c2f 613e 293c  ack to top</a>)<
-00001940: 2f70 3e0a 2020 2020 2020 2020 0a4b 6579  /p>.        .Key
-00001950: 776f 7264 733a 2064 7275 672d 6469 7363  words: drug-disc
-00001960: 6f76 6572 7920 6d61 6368 696e 652d 6c65  overy machine-le
-00001970: 6172 6e69 6e67 2065 7273 696c 6961 206f  arning ersilia o
-00001980: 7065 6e2d 7363 6965 6e63 6520 676c 6f62  pen-science glob
-00001990: 616c 2d68 6561 6c74 6820 6d6f 6465 6c2d  al-health model-
-000019a0: 6875 6220 696e 6665 6374 696f 7573 2d64  hub infectious-d
-000019b0: 6973 6561 7365 730a 506c 6174 666f 726d  iseases.Platform
-000019c0: 3a20 554e 4b4e 4f57 4e0a 436c 6173 7369  : UNKNOWN.Classi
-000019d0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000019e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000019f0: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
-00001a00: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00001a10: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00001a20: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
-00001a30: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00001a40: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00001a50: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
-00001a60: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00001a70: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
-00001a80: 6769 6e65 6572 696e 6720 3a3a 2041 7274  gineering :: Art
-00001a90: 6966 6963 6961 6c20 496e 7465 6c6c 6967  ificial Intellig
-00001aa0: 656e 6365 0a52 6571 7569 7265 732d 5079  ence.Requires-Py
-00001ab0: 7468 6f6e 3a20 3e3d 332e 370a 4465 7363  thon: >=3.7.Desc
-00001ac0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00001ad0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00001ae0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00001af0: 7261 3a20 646f 635f 6275 696c 6465 720a  ra: doc_builder.
-00001b00: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00001b10: 7465 7374 0a50 726f 7669 6465 732d 4578  test.Provides-Ex
-00001b20: 7472 613a 2064 6576 0a                   tra: dev.
+000003a0: 652f 4c69 6365 6e73 652d 4750 4c25 3230  e/License-GPL%20
+000003b0: 7633 2d79 656c 6c6f 772e 7376 6729 5d28  v3-yellow.svg)](
+000003c0: 6874 7470 733a 2f2f 7777 772e 676e 752e  https://www.gnu.
+000003d0: 6f72 672f 6c69 6365 6e73 6573 2f61 6770  org/licenses/agp
+000003e0: 6c2d 332e 3029 205b 215b 444f 495d 2868  l-3.0) [![DOI](h
+000003f0: 7474 7073 3a2f 2f7a 656e 6f64 6f2e 6f72  ttps://zenodo.or
+00000400: 672f 6261 6467 652f 3237 3730 3638 3938  g/badge/27706898
+00000410: 392e 7376 6729 5d28 6874 7470 733a 2f2f  9.svg)](https://
+00000420: 7a65 6e6f 646f 2e6f 7267 2f62 6164 6765  zenodo.org/badge
+00000430: 2f6c 6174 6573 7464 6f69 2f32 3737 3036  /latestdoi/27706
+00000440: 3839 3839 290a 2020 2020 2020 2020 0a20  8989).        . 
+00000450: 2020 2020 2020 205b 215b 646f 6375 6d65         [![docume
+00000460: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000470: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000480: 6261 6467 652f 2d44 6f63 756d 656e 7461  badge/-Documenta
+00000490: 7469 6f6e 2d70 7572 706c 653f 6c6f 676f  tion-purple?logo
+000004a0: 3d72 6561 642d 7468 652d 646f 6373 266c  =read-the-docs&l
+000004b0: 6f67 6f43 6f6c 6f72 3d77 6869 7465 295d  ogoColor=white)]
+000004c0: 2868 7474 7073 3a2f 2f65 7273 696c 6961  (https://ersilia
+000004d0: 2e67 6974 626f 6f6b 2e69 6f2f 6572 7369  .gitbook.io/ersi
+000004e0: 6c69 612d 626f 6f6b 2f29 205b 215b 5079  lia-book/) [![Py
+000004f0: 5049 2076 6572 7369 6f6e 2066 7572 792e  PI version fury.
+00000500: 696f 5d28 6874 7470 733a 2f2f 6261 6467  io](https://badg
+00000510: 652e 6675 7279 2e69 6f2f 7079 2f65 7273  e.fury.io/py/ers
+00000520: 696c 6961 2e73 7667 295d 2868 7474 7073  ilia.svg)](https
+00000530: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000540: 7267 2f70 7970 692f 6572 7369 6c69 612f  rg/pypi/ersilia/
+00000550: 2920 5b21 5b50 7974 686f 6e20 332e 375d  ) [![Python 3.7]
+00000560: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000570: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00000580: 7468 6f6e 2d33 2e37 2d62 6c75 652e 7376  thon-3.7-blue.sv
+00000590: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
+000005a0: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+000005b0: 6f61 6473 2f72 656c 6561 7365 2f70 7974  oads/release/pyt
+000005c0: 686f 6e2d 3337 302f 2920 5b21 5b43 6f64  hon-370/) [![Cod
+000005d0: 6520 7374 796c 653a 2062 6c61 636b 5d28  e style: black](
+000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000005f0: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
+00000600: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
+00000610: 3030 3030 3030 2e73 7667 3f6c 6f67 6f3d  000000.svg?logo=
+00000620: 5079 7468 6f6e 266c 6f67 6f43 6f6c 6f72  Python&logoColor
+00000630: 3d77 6869 7465 295d 2868 7474 7073 3a2f  =white)](https:/
+00000640: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
+00000650: 626c 6163 6b29 205b 215b 4769 7470 6f64  black) [![Gitpod
+00000660: 2052 6561 6479 2d74 6f2d 436f 6465 5d28   Ready-to-Code](
+00000670: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000680: 6c64 732e 696f 2f62 6164 6765 2f47 6974  lds.io/badge/Git
+00000690: 706f 642d 7265 6164 792d 2d74 6f2d 2d63  pod-ready--to--c
+000006a0: 6f64 652d 626c 7565 3f6c 6f67 6f3d 6769  ode-blue?logo=gi
+000006b0: 7470 6f64 295d 2868 7474 7073 3a2f 2f67  tpod)](https://g
+000006c0: 6974 706f 642e 696f 2f23 6874 7470 733a  itpod.io/#https:
+000006d0: 2f2f 6769 7468 7562 2e63 6f6d 2f65 7273  //github.com/ers
+000006e0: 696c 6961 2d6f 732f 6572 7369 6c69 6129  ilia-os/ersilia)
+000006f0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000700: 2020 2323 2054 6162 6c65 206f 6620 436f    ## Table of Co
+00000710: 6e74 656e 7473 0a20 2020 2020 2020 200a  ntents.        .
+00000720: 2020 2020 2020 2020 312e 205b 5072 6f6a          1. [Proj
+00000730: 6563 7420 4465 7363 7269 7074 696f 6e5d  ect Description]
+00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000750: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
+00000760: 7273 696c 6961 2370 726f 6a65 6374 2d64  rsilia#project-d
+00000770: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
+00000780: 2020 2020 322e 205b 5175 6963 6b20 7374      2. [Quick st
+00000790: 6172 7420 6775 6964 655d 2868 7474 7073  art guide](https
+000007a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
+000007b0: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
+000007c0: 2371 7569 636b 2d73 7461 7274 2d67 7569  #quick-start-gui
+000007d0: 6465 290a 2020 2020 2020 2020 332e 205b  de).        3. [
+000007e0: 436f 6e74 7269 6275 7465 5d28 6874 7470  Contribute](http
+000007f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000800: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
+00000810: 6123 636f 6e74 7269 6275 7465 290a 2020  a#contribute).  
+00000820: 2020 2020 2020 342e 205b 4c69 6365 6e73        4. [Licens
+00000830: 6520 616e 6420 6369 7461 7469 6f6e 5d28  e and citation](
+00000840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000850: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
+00000860: 7369 6c69 6123 6c69 6365 6e73 652d 616e  silia#license-an
+00000870: 642d 6369 7461 7469 6f6e 290a 2020 2020  d-citation).    
+00000880: 2020 2020 352e 205b 4162 6f75 7420 7573      5. [About us
+00000890: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008a0: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+000008b0: 6572 7369 6c69 6123 6162 6f75 742d 7573  ersilia#about-us
+000008c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000008d0: 2020 2023 2320 5072 6f6a 6563 7420 4465     ## Project De
+000008e0: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
+000008f0: 2020 0a20 2020 2020 2020 2054 6865 2045    .        The E
+00000900: 7273 696c 6961 204d 6f64 656c 2048 7562  rsilia Model Hub
+00000910: 2069 7320 6120 756e 6966 6965 6420 706c   is a unified pl
+00000920: 6174 666f 726d 206f 6620 7072 652d 7472  atform of pre-tr
+00000930: 6169 6e65 6420 4149 2f4d 4c20 6d6f 6465  ained AI/ML mode
+00000940: 6c73 2066 6f72 2069 6e66 6563 7469 6f75  ls for infectiou
+00000950: 7320 616e 6420 6e65 676c 6563 7465 6420  s and neglected 
+00000960: 6469 7365 6173 6520 7265 7365 6172 6368  disease research
+00000970: 2e20 5468 6520 656e 6420 676f 616c 2069  . The end goal i
+00000980: 7320 746f 2070 726f 7669 6465 2061 6e20  s to provide an 
+00000990: 6f70 656e 2d73 6f75 7263 652c 206e 6f2d  open-source, no-
+000009a0: 636f 6465 2073 6f6c 7574 696f 6e20 746f  code solution to
+000009b0: 2061 6363 6573 7320 4149 2f4d 4c20 6d6f   access AI/ML mo
+000009c0: 6465 6c73 2074 6f20 6163 6365 6c65 7261  dels to accelera
+000009d0: 7465 2064 7275 6720 6469 7363 6f76 6572  te drug discover
+000009e0: 792e 2054 6865 206d 6f64 656c 7320 656d  y. The models em
+000009f0: 6265 6464 6564 2069 6e20 7468 6520 6875  bedded in the hu
+00000a00: 6220 696e 636c 7564 6520 626f 7468 206d  b include both m
+00000a10: 6f64 656c 7320 7075 626c 6973 6865 6420  odels published 
+00000a20: 696e 2074 6865 206c 6974 6572 6174 7572  in the literatur
+00000a30: 6520 2877 6974 6820 6170 7072 6f70 7269  e (with appropri
+00000a40: 6174 6520 7468 6972 6420 7061 7274 7920  ate third party 
+00000a50: 6163 6b6e 6f77 6c65 6467 656d 656e 7429  acknowledgement)
+00000a60: 2061 6e64 206d 6f64 656c 7320 6465 7665   and models deve
+00000a70: 6c6f 7065 6420 6279 2074 6865 2045 7273  loped by the Ers
+00000a80: 696c 6961 2074 6561 6d20 6f72 2063 6f6e  ilia team or con
+00000a90: 7472 6962 7574 6f72 732e 0a20 2020 2020  tributors..     
+00000aa0: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
+00000ab0: 6164 206d 6f72 6520 6162 6f75 7420 7468  ad more about th
+00000ac0: 6520 7072 6f6a 6563 7420 696e 2074 6865  e project in the
+00000ad0: 205b 4572 7369 6c69 6120 426f 6f6b 5d28   [Ersilia Book](
+00000ae0: 6874 7470 733a 2f2f 6572 7369 6c69 612e  https://ersilia.
+00000af0: 6769 7462 6f6f 6b2e 696f 2f65 7273 696c  gitbook.io/ersil
+00000b00: 6961 2d62 6f6f 6b2f 290a 2020 2020 2020  ia-book/).      
+00000b10: 2020 2a20 4272 6f77 7365 2061 7661 696c    * Browse avail
+00000b20: 6162 6c65 206d 6f64 656c 7320 696e 2074  able models in t
+00000b30: 6865 205b 4572 7369 6c69 6120 4d6f 6465  he [Ersilia Mode
+00000b40: 6c20 4875 625d 2868 7474 7073 3a2f 2f65  l Hub](https://e
+00000b50: 7273 696c 6961 2e69 6f2f 6d6f 6465 6c2d  rsilia.io/model-
+00000b60: 6875 622f 290a 2020 2020 2020 2020 0a20  hub/).        . 
+00000b70: 2020 2020 2020 2023 2320 5175 6963 6b20         ## Quick 
+00000b80: 5374 6172 7420 4775 6964 650a 2020 2020  Start Guide.    
+00000b90: 2020 2020 0a20 2020 2020 2020 2050 6c65      .        Ple
+00000ba0: 6173 6520 6368 6563 6b20 7468 6520 7061  ase check the pa
+00000bb0: 636b 6167 6520 7265 7175 6972 656d 656e  ckage requiremen
+00000bc0: 7473 2069 6e20 7468 6520 5b49 6e73 7461  ts in the [Insta
+00000bd0: 6c6c 6174 696f 6e20 4775 6964 655d 2868  llation Guide](h
+00000be0: 7474 7073 3a2f 2f65 7273 696c 6961 2e67  ttps://ersilia.g
+00000bf0: 6974 626f 6f6b 2e69 6f2f 6572 7369 6c69  itbook.io/ersili
+00000c00: 612d 626f 6f6b 2f71 7569 636b 2d73 7461  a-book/quick-sta
+00000c10: 7274 2f69 6e73 7461 6c6c 6174 696f 6e29  rt/installation)
+00000c20: 2e20 5468 6520 6e65 7874 2073 7465 7073  . The next steps
+00000c30: 2061 7265 2061 2071 7569 636b 7374 6172   are a quickstar
+00000c40: 7420 6775 6964 6520 746f 2069 6e73 7461  t guide to insta
+00000c50: 6c6c 696e 6720 4572 7369 6c69 612e 0a20  lling Ersilia.. 
+00000c60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c70: 312e 2043 7265 6174 6520 6120 636f 6e64  1. Create a cond
+00000c80: 6120 656e 7669 726f 6e6d 656e 7420 616e  a environment an
+00000c90: 6420 6163 7469 7661 7465 2069 740a 2020  d activate it.  
+00000ca0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00000cb0: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00000cc0: 2020 2020 2020 2063 6f6e 6461 2063 7265         conda cre
+00000cd0: 6174 6520 2d6e 2065 7273 696c 6961 2070  ate -n ersilia p
+00000ce0: 7974 686f 6e3d 332e 370a 2020 2020 2020  ython=3.7.      
+00000cf0: 2020 2020 2020 636f 6e64 6120 6163 7469        conda acti
+00000d00: 7661 7465 2065 7273 696c 6961 0a20 2020  vate ersilia.   
+00000d10: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000d20: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00000d30: 2043 6c6f 6e65 2074 6869 7320 7265 706f   Clone this repo
+00000d40: 7369 746f 7279 2061 6e64 2069 6e73 7461  sitory and insta
+00000d50: 6c6c 2077 6974 6820 7069 700a 2020 2020  ll with pip.    
+00000d60: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00000d70: 2060 6060 6261 7368 0a20 2020 2020 2020   ```bash.       
+00000d80: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
+00000d90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000da0: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
+00000db0: 696c 6961 2e67 6974 0a20 2020 2020 2020  ilia.git.       
+00000dc0: 2020 2020 2063 6420 6572 7369 6c69 610a       cd ersilia.
+00000dd0: 2020 2020 2020 2020 2020 2020 7069 7020              pip 
+00000de0: 696e 7374 616c 6c20 2d65 202e 0a20 2020  install -e ..   
+00000df0: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000e00: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00000e10: 204f 6e63 6520 7468 6520 4572 7369 6c69   Once the Ersili
+00000e20: 6120 4d6f 6465 6c20 4875 6220 6973 2069  a Model Hub is i
+00000e30: 6e73 7461 6c6c 6564 2c20 796f 7520 6361  nstalled, you ca
+00000e40: 6e20 7573 6520 7468 6520 434c 4920 746f  n use the CLI to
+00000e50: 2072 756e 2070 7265 6469 6374 696f 6e73   run predictions
+00000e60: 2e20 4669 7273 742c 2073 656c 6563 7420  . First, select 
+00000e70: 6120 6d6f 6465 6c20 6672 6f6d 2074 6865  a model from the
+00000e80: 205b 4572 7369 6c69 6120 4d6f 6465 6c20   [Ersilia Model 
+00000e90: 4875 625d 2868 7474 7073 3a2f 2f65 7273  Hub](https://ers
+00000ea0: 696c 6961 2e69 6f2f 6d6f 6465 6c2d 6875  ilia.io/model-hu
+00000eb0: 622f 2920 616e 6420 2a2a 6665 7463 682a  b/) and **fetch*
+00000ec0: 2a20 6974 3a0a 2020 2020 2020 2020 0a20  * it:.        . 
+00000ed0: 2020 2020 2020 2020 2020 2060 6060 6261             ```ba
+00000ee0: 7368 0a20 2020 2020 2020 2020 2020 2065  sh.            e
+00000ef0: 7273 696c 6961 2066 6574 6368 2072 6574  rsilia fetch ret
+00000f00: 726f 7379 6e74 6865 7469 632d 6163 6365  rosynthetic-acce
+00000f10: 7373 6962 696c 6974 790a 2020 2020 2020  ssibility.      
+00000f20: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000f30: 2020 0a20 2020 2020 2020 2031 2e20 4765    .        1. Ge
+00000f40: 6e65 7261 7465 2061 2066 6577 2028 3529  nerate a few (5)
+00000f50: 2065 7861 6d70 6c65 206d 6f6c 6563 756c   example molecul
+00000f60: 6573 2c20 746f 2062 6520 7573 6564 2061  es, to be used a
+00000f70: 7320 696e 7075 742e 2054 6865 202a 2a65  s input. The **e
+00000f80: 7861 6d70 6c65 2a2a 2063 6f6d 6d61 6e64  xample** command
+00000f90: 2077 696c 6c20 6765 6e65 7261 7465 2074   will generate t
+00000fa0: 6865 2061 6465 7175 6174 6520 696e 7075  he adequate inpu
+00000fb0: 7420 666f 7220 7468 6520 6d6f 6465 6c20  t for the model 
+00000fc0: 696e 2075 7365 0a20 2020 2020 2020 200a  in use.        .
+00000fd0: 2020 2020 2020 2020 2020 2020 6060 6062              ```b
+00000fe0: 6173 680a 2020 2020 2020 2020 2020 2020  ash.            
+00000ff0: 6572 7369 6c69 6120 6578 616d 706c 6520  ersilia example 
+00001000: 7265 7472 6f73 796e 7468 6574 6963 2d61  retrosynthetic-a
+00001010: 6363 6573 7369 6269 6c69 7479 202d 6e20  ccessibility -n 
+00001020: 3520 2d66 206d 795f 6d6f 6c65 6375 6c65  5 -f my_molecule
+00001030: 732e 6373 760a 2020 2020 2020 2020 2020  s.csv.          
+00001040: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00001050: 2020 2020 2020 2031 2e20 5468 656e 2c20         1. Then, 
+00001060: 2a2a 7365 7276 652a 2a20 796f 7572 206d  **serve** your m
+00001070: 6f64 656c 3a0a 2020 2020 2020 2020 0a20  odel:.        . 
+00001080: 2020 2020 2020 2020 2020 2060 6060 6261             ```ba
+00001090: 7368 0a20 2020 2020 2020 2020 2020 2065  sh.            e
+000010a0: 7273 696c 6961 2073 6572 7665 2072 6574  rsilia serve ret
+000010b0: 726f 7379 6e74 6865 7469 632d 6163 6365  rosynthetic-acce
+000010c0: 7373 6962 696c 6974 790a 2020 2020 2020  ssibility.      
+000010d0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+000010e0: 2020 0a20 2020 2020 2020 2031 2e20 416e    .        1. An
+000010f0: 6420 7275 6e20 7468 6520 7072 6564 6963  d run the predic
+00001100: 7469 6f6e 202a 2a41 5049 2a2a 3a0a 2020  tion **API**:.  
+00001110: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00001120: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00001130: 2020 2020 2020 2065 7273 696c 6961 2061         ersilia a
+00001140: 7069 202d 6920 6d79 5f6d 6f6c 6563 756c  pi -i my_molecul
+00001150: 6573 2e63 7376 202d 6f20 6d79 5f70 7265  es.csv -o my_pre
+00001160: 6469 6374 696f 6e73 2e63 7376 0a20 2020  dictions.csv.   
+00001170: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00001180: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00001190: 2046 696e 616c 6c79 2c20 2a2a 636c 6f73   Finally, **clos
+000011a0: 652a 2a20 7468 6520 7365 7276 6963 6520  e** the service 
+000011b0: 7768 656e 2079 6f75 2061 7265 2064 6f6e  when you are don
+000011c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+000011d0: 2020 2020 2020 2020 6060 6062 6173 680a          ```bash.
+000011e0: 2020 2020 2020 2020 2020 2020 6572 7369              ersi
+000011f0: 6c69 6120 636c 6f73 650a 2020 2020 2020  lia close.      
+00001200: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001210: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
+00001220: 6520 7365 6520 7468 6520 5b45 7273 696c  e see the [Ersil
+00001230: 6961 2042 6f6f 6b5d 2868 7474 7073 3a2f  ia Book](https:/
+00001240: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
+00001250: 2e69 6f2f 6572 7369 6c69 612d 626f 6f6b  .io/ersilia-book
+00001260: 2f29 2066 6f72 206d 6f72 6520 6578 616d  /) for more exam
+00001270: 706c 6573 2061 6e64 2064 6574 6169 6c65  ples and detaile
+00001280: 6420 6578 706c 616e 6174 696f 6e73 2e0a  d explanations..
+00001290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000012a0: 2023 2320 436f 6e74 7269 6275 7465 0a20   ## Contribute. 
+000012b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000012c0: 5468 6520 4572 7369 6c69 6120 4d6f 6465  The Ersilia Mode
+000012d0: 6c20 4875 6220 6973 2061 2046 7265 652c  l Hub is a Free,
+000012e0: 204f 7065 6e20 536f 7572 6365 2053 6f66   Open Source Sof
+000012f0: 7477 6172 6520 616e 6420 7765 2068 6967  tware and we hig
+00001300: 686c 7920 7661 6c75 6520 6e65 7720 636f  hly value new co
+00001310: 6e74 7269 6275 746f 7273 2e20 5468 6572  ntributors. Ther
+00001320: 6520 6172 6520 7365 7665 7261 6c20 7761  e are several wa
+00001330: 7973 2069 6e20 7768 6963 6820 796f 7520  ys in which you 
+00001340: 6361 6e20 636f 6e74 7269 6275 7465 2074  can contribute t
+00001350: 6f20 7468 6520 7072 6f6a 6563 743a 0a20  o the project:. 
+00001360: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001370: 2a20 4120 676f 6f64 2070 6c61 6365 2074  * A good place t
+00001380: 6f20 7374 6172 7420 6973 2063 6865 636b  o start is check
+00001390: 696e 6720 6f70 656e 205b 6973 7375 6573  ing open [issues
+000013a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000013b0: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+000013c0: 6572 7369 6c69 612f 6973 7375 6573 292e  ersilia/issues).
+000013d0: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
+000013e0: 7520 6861 7665 2069 6465 6e74 6966 6965  u have identifie
+000013f0: 6420 6120 6275 6720 696e 2074 6865 2063  d a bug in the c
+00001400: 6f64 652c 2070 6c65 6173 6520 6f70 656e  ode, please open
+00001410: 2061 206e 6577 2069 7373 7565 2075 7369   a new issue usi
+00001420: 6e67 2074 6865 2062 7567 2074 656d 706c  ng the bug templ
+00001430: 6174 652e 0a20 2020 2020 2020 202a 2053  ate..        * S
+00001440: 6861 7265 2061 6e79 2066 6565 6462 6163  hare any feedbac
+00001450: 6b20 7769 7468 2074 6865 2063 6f6d 6d75  k with the commu
+00001460: 6e69 7479 2075 7369 6e67 205b 4769 7448  nity using [GitH
+00001470: 7562 2044 6973 6375 7373 696f 6e73 5d28  ub Discussions](
+00001480: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001490: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
+000014a0: 7369 6c69 612f 6469 7363 7573 7369 6f6e  silia/discussion
+000014b0: 7329 2066 6f72 2074 6865 2070 726f 6a65  s) for the proje
+000014c0: 6374 0a20 2020 2020 2020 202a 2043 6865  ct.        * Che
+000014d0: 636b 206f 7572 205b 436f 6e74 7269 6275  ck our [Contribu
+000014e0: 7469 6e67 2047 7569 6465 5d28 6874 7470  ting Guide](http
+000014f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00001500: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
+00001510: 612f 626c 6f62 2f6d 6173 7465 722f 434f  a/blob/master/CO
+00001520: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00001530: 6f72 206d 6f72 6520 6465 7461 696c 730a  or more details.
+00001540: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001550: 2054 6865 2045 7273 696c 6961 204f 7065   The Ersilia Ope
+00001560: 6e20 536f 7572 6365 2049 6e69 7469 6174  n Source Initiat
+00001570: 6976 6520 6164 6865 7265 7320 746f 2074  ive adheres to t
+00001580: 6865 205b 436f 6e74 7269 6275 746f 7220  he [Contributor 
+00001590: 436f 7665 6e61 6e74 5d28 6874 7470 733a  Covenant](https:
+000015a0: 2f2f 6572 7369 6c69 612e 6769 7462 6f6f  //ersilia.gitboo
+000015b0: 6b2e 696f 2f65 7273 696c 6961 2d77 696b  k.io/ersilia-wik
+000015c0: 692f 636f 6465 2d6f 662d 636f 6e64 7563  i/code-of-conduc
+000015d0: 7429 2063 6f64 6520 6f66 2063 6f6e 6475  t) code of condu
+000015e0: 6374 2e0a 2020 2020 2020 2020 0a20 2020  ct..        .   
+000015f0: 2020 2020 2023 2323 2053 7562 6d69 7420       ### Submit 
+00001600: 6120 4e65 7720 4d6f 6465 6c0a 2020 2020  a New Model.    
+00001610: 2020 2020 0a20 2020 2020 2020 2049 6620      .        If 
+00001620: 796f 7520 7761 6e74 2074 6f20 696e 636f  you want to inco
+00001630: 7270 6f72 6174 6520 6120 6e65 7720 6d6f  rporate a new mo
+00001640: 6465 6c20 696e 2074 6865 2070 6c61 7466  del in the platf
+00001650: 6f72 6d2c 206f 7065 6e20 6120 6e65 7720  orm, open a new 
+00001660: 6973 7375 6520 7573 696e 6720 7468 6520  issue using the 
+00001670: 5b6d 6f64 656c 2072 6571 7565 7374 2074  [model request t
+00001680: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
+00001690: 2f67 6974 6875 622e 636f 6d2f 6572 7369  /github.com/ersi
+000016a0: 6c69 612d 6f73 2f65 7273 696c 6961 2f69  lia-os/ersilia/i
+000016b0: 7373 7565 732f 6e65 773f 6173 7369 676e  ssues/new?assign
+000016c0: 6565 733d 266c 6162 656c 733d 6e65 772d  ees=&labels=new-
+000016d0: 6d6f 6465 6c26 7465 6d70 6c61 7465 3d6d  model&template=m
+000016e0: 6f64 656c 5f72 6571 7565 7374 2e79 6d6c  odel_request.yml
+000016f0: 2674 6974 6c65 3d25 4630 2539 4625 4136  &title=%F0%9F%A6
+00001700: 2541 302b 4d6f 6465 6c2b 5265 7175 6573  %A0+Model+Reques
+00001710: 7425 3341 2b25 3343 6e61 6d65 2533 4529  t%3A+%3Cname%3E)
+00001720: 206f 7220 636f 6e74 6163 7420 7573 2075   or contact us u
+00001730: 7369 6e67 2074 6865 2066 6f6c 6c6f 7769  sing the followi
+00001740: 6e67 205b 666f 726d 5d28 6874 7470 733a  ng [form](https:
+00001750: 2f2f 7777 772e 6572 7369 6c69 612e 696f  //www.ersilia.io
+00001760: 2f72 6571 7565 7374 2d6d 6f64 656c 292e  /request-model).
+00001770: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001780: 2020 4166 7465 7220 7375 626d 6974 7469    After submitti
+00001790: 6e67 2079 6f75 7220 6d6f 6465 6c20 7265  ng your model re
+000017a0: 7175 6573 7420 7669 6120 616e 2069 7373  quest via an iss
+000017b0: 7565 2028 7375 6767 6573 7465 6429 2c20  ue (suggested), 
+000017c0: 6120 6d61 696e 7461 696e 6572 2077 696c  a maintainer wil
+000017d0: 6c20 7265 7669 6577 2079 6f75 7220 7265  l review your re
+000017e0: 7175 6573 742e 2049 6620 7468 6579 2060  quest. If they `
+000017f0: 2f61 7070 726f 7665 6020 796f 7572 2072  /approve` your r
+00001800: 6571 7565 7374 2c20 6120 6e65 7720 6d6f  equest, a new mo
+00001810: 6465 6c20 7265 7370 6f73 6974 6f72 7920  del respository 
+00001820: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
+00001830: 666f 7220 796f 7520 746f 2066 6f72 6b20  for you to fork 
+00001840: 616e 6420 7573 6521 2054 6865 7265 2069  and use! There i
+00001850: 7320 6120 5b64 656d 6f20 7265 706f 7369  s a [demo reposi
+00001860: 746f 7279 5d28 6874 7470 733a 2f2f 6769  tory](https://gi
+00001870: 7468 7562 2e63 6f6d 2f65 7273 696c 6961  thub.com/ersilia
+00001880: 2d6f 732f 656f 732d 6465 6d6f 2920 6578  -os/eos-demo) ex
+00001890: 706c 6169 6e69 6e67 2074 6865 2073 7465  plaining the ste
+000018a0: 7073 206f 6e65 2d62 792d 6f6e 652e 0a20  ps one-by-one.. 
+000018b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000018c0: 2323 204c 6963 656e 7365 2061 6e64 2043  ## License and C
+000018d0: 6974 6174 696f 6e0a 2020 2020 2020 2020  itation.        
+000018e0: 0a20 2020 2020 2020 2054 6869 7320 7265  .        This re
+000018f0: 706f 7369 746f 7279 2069 7320 6f70 656e  pository is open
+00001900: 2d73 6f75 7263 6564 2075 6e64 6572 2074  -sourced under t
+00001910: 6865 205b 4750 4c2d 3320 4c69 6365 6e73  he [GPL-3 Licens
+00001920: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001930: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+00001940: 2f65 7273 696c 6961 2f62 6c6f 622f 6d61  /ersilia/blob/ma
+00001950: 7374 6572 2f4c 4943 454e 5345 292e 0a20  ster/LICENSE).. 
+00001960: 2020 2020 2020 2050 6c65 6173 6520 5b63         Please [c
+00001970: 6974 6520 7573 5d28 6874 7470 733a 2f2f  ite us](https://
+00001980: 6769 7468 7562 2e63 6f6d 2f65 7273 696c  github.com/ersil
+00001990: 6961 2d6f 732f 6572 7369 6c69 612f 626c  ia-os/ersilia/bl
+000019a0: 6f62 2f6d 6173 7465 722f 4349 5441 5449  ob/master/CITATI
+000019b0: 4f4e 2e63 6666 2920 6966 2079 6f75 2075  ON.cff) if you u
+000019c0: 7365 2069 7421 0a20 2020 2020 2020 200a  se it!.        .
+000019d0: 2020 2020 2020 2020 2323 2041 626f 7574          ## About
+000019e0: 2055 730a 2020 2020 2020 2020 0a20 2020   Us.        .   
+000019f0: 2020 2020 2054 6865 205b 4572 7369 6c69       The [Ersili
+00001a00: 6120 4f70 656e 2053 6f75 7263 6520 496e  a Open Source In
+00001a10: 6974 6961 7469 7665 5d28 6874 7470 733a  itiative](https:
+00001a20: 2f2f 6572 7369 6c69 612e 696f 2920 6973  //ersilia.io) is
+00001a30: 2061 204e 6f6e 2050 726f 6669 7420 4f72   a Non Profit Or
+00001a40: 6761 6e69 7a61 7469 6f6e 2028 5b31 3139  ganization ([119
+00001a50: 3232 3636 5d28 6874 7470 733a 2f2f 7265  2266](https://re
+00001a60: 6769 7374 6572 2d6f 662d 6368 6172 6974  gister-of-charit
+00001a70: 6965 732e 6368 6172 6974 7963 6f6d 6d69  ies.charitycommi
+00001a80: 7373 696f 6e2e 676f 762e 756b 2f63 6861  ssion.gov.uk/cha
+00001a90: 7269 7479 2d73 6561 7263 682f 2d2f 6368  rity-search/-/ch
+00001aa0: 6172 6974 792d 6465 7461 696c 732f 3531  arity-details/51
+00001ab0: 3730 3635 372f 6675 6c6c 2d70 7269 6e74  70657/full-print
+00001ac0: 2929 2077 6974 6820 7468 6520 6d69 7373  )) with the miss
+00001ad0: 696f 6e20 6973 2074 6f20 6571 7569 7020  ion is to equip 
+00001ae0: 6c61 6273 2c20 756e 6976 6572 7369 7469  labs, universiti
+00001af0: 6573 2061 6e64 2063 6c69 6e69 6373 2069  es and clinics i
+00001b00: 6e20 4c4d 4943 2077 6974 6820 4149 2f4d  n LMIC with AI/M
+00001b10: 4c20 746f 6f6c 7320 666f 7220 696e 6665  L tools for infe
+00001b20: 6374 696f 7573 2064 6973 6561 7365 2072  ctious disease r
+00001b30: 6573 6561 7263 682e 0a20 2020 2020 2020  esearch..       
+00001b40: 200a 2020 2020 2020 2020 5b48 656c 7020   .        [Help 
+00001b50: 7573 5d28 6874 7470 733a 2f2f 7777 772e  us](https://www.
+00001b60: 6572 7369 6c69 612e 696f 2f64 6f6e 6174  ersilia.io/donat
+00001b70: 6529 2061 6368 6965 7665 206f 7572 206d  e) achieve our m
+00001b80: 6973 7369 6f6e 206f 7220 5b76 6f6c 756e  ission or [volun
+00001b90: 7465 6572 5d28 6874 7470 733a 2f2f 7777  teer](https://ww
+00001ba0: 772e 6572 7369 6c69 612e 696f 2f76 6f6c  w.ersilia.io/vol
+00001bb0: 756e 7465 6572 2920 7769 7468 2075 7321  unteer) with us!
+00001bc0: 0a20 2020 2020 2020 200a 4b65 7977 6f72  .        .Keywor
+00001bd0: 6473 3a20 6472 7567 2d64 6973 636f 7665  ds: drug-discove
+00001be0: 7279 206d 6163 6869 6e65 2d6c 6561 726e  ry machine-learn
+00001bf0: 696e 6720 6572 7369 6c69 6120 6f70 656e  ing ersilia open
+00001c00: 2d73 6369 656e 6365 2067 6c6f 6261 6c2d  -science global-
+00001c10: 6865 616c 7468 206d 6f64 656c 2d68 7562  health model-hub
+00001c20: 2069 6e66 6563 7469 6f75 732d 6469 7365   infectious-dise
+00001c30: 6173 6573 0a50 6c61 7466 6f72 6d3a 2055  ases.Platform: U
+00001c40: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
+00001c50: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00001c60: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00001c70: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+00001c80: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00001c90: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00001ca0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00001cb0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00001cc0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00001cd0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00001ce0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00001cf0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00001d00: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00001d10: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00001d20: 3320 2847 504c 7633 290a 436c 6173 7369  3 (GPLv3).Classi
+00001d30: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00001d40: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00001d50: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00001d60: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00001d70: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00001d80: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
+00001d90: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
+00001da0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00001db0: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
+00001dc0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00001dd0: 2074 6578 742f 6d61 726b 646f 776e 0a50   text/markdown.P
+00001de0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+00001df0: 616b 650a 5072 6f76 6964 6573 2d45 7874  ake.Provides-Ext
+00001e00: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
+00001e10: 732d 4578 7472 613a 2074 6573 740a       s-Extra: test.
```

### Comparing `ersilia-0.1.1/README.md` & `ersilia-0.1.8/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -19,318 +19,349 @@
 00000120: 746f 7220 436f 7665 6e61 6e74 5d28 6874  tor Covenant](ht
 00000130: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
 00000140: 732e 696f 2f62 6164 6765 2f43 6f6e 7472  s.io/badge/Contr
 00000150: 6962 7574 6f72 2532 3043 6f76 656e 616e  ibutor%20Covenan
 00000160: 742d 7632 2e30 2532 3061 646f 7074 6564  t-v2.0%20adopted
 00000170: 2d66 6636 3962 342e 7376 6729 5d28 434f  -ff69b4.svg)](CO
 00000180: 4445 5f4f 465f 434f 4e44 5543 542e 6d64  DE_OF_CONDUCT.md
-00000190: 2920 5b21 5b4c 6963 656e 7365 3a20 4147  ) [![License: AG
-000001a0: 504c 2076 335d 2868 7474 7073 3a2f 2f69  PL v3](https://i
-000001b0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-000001c0: 6467 652f 4c69 6365 6e73 652d 4147 504c  dge/License-AGPL
-000001d0: 2532 3076 332d 7965 6c6c 6f77 2e73 7667  %20v3-yellow.svg
-000001e0: 295d 2868 7474 7073 3a2f 2f77 7777 2e67  )](https://www.g
-000001f0: 6e75 2e6f 7267 2f6c 6963 656e 7365 732f  nu.org/licenses/
-00000200: 6167 706c 2d33 2e30 290a 0a5b 215b 646f  agpl-3.0)..[![do
-00000210: 6375 6d65 6e74 6174 696f 6e5d 2868 7474  cumentation](htt
-00000220: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
-00000230: 2e69 6f2f 6261 6467 652f 2d44 6f63 756d  .io/badge/-Docum
-00000240: 656e 7461 7469 6f6e 2d70 7572 706c 653f  entation-purple?
-00000250: 6c6f 676f 3d72 6561 642d 7468 652d 646f  logo=read-the-do
-00000260: 6373 266c 6f67 6f43 6f6c 6f72 3d77 6869  cs&logoColor=whi
-00000270: 7465 295d 2868 7474 7073 3a2f 2f65 7273  te)](https://ers
-00000280: 696c 6961 2e67 6974 626f 6f6b 2e69 6f2f  ilia.gitbook.io/
-00000290: 6572 7369 6c69 612d 626f 6f6b 2f29 205b  ersilia-book/) [
-000002a0: 215b 5079 5049 2076 6572 7369 6f6e 2066  ![PyPI version f
-000002b0: 7572 792e 696f 5d28 6874 7470 733a 2f2f  ury.io](https://
-000002c0: 6261 6467 652e 6675 7279 2e69 6f2f 7079  badge.fury.io/py
-000002d0: 2f65 7273 696c 6961 2e73 7667 295d 2868  /ersilia.svg)](h
-000002e0: 7474 7073 3a2f 2f70 7970 692e 7079 7468  ttps://pypi.pyth
-000002f0: 6f6e 2e6f 7267 2f70 7970 692f 6572 7369  on.org/pypi/ersi
-00000300: 6c69 612f 2920 5b21 5b50 7974 686f 6e20  lia/) [![Python 
-00000310: 332e 375d 2868 7474 7073 3a2f 2f69 6d67  3.7](https://img
-00000320: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-00000330: 652f 7079 7468 6f6e 2d33 2e37 2d62 6c75  e/python-3.7-blu
-00000340: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
-00000350: 7777 772e 7079 7468 6f6e 2e6f 7267 2f64  www.python.org/d
-00000360: 6f77 6e6c 6f61 6473 2f72 656c 6561 7365  ownloads/release
-00000370: 2f70 7974 686f 6e2d 3337 302f 2920 5b21  /python-370/) [!
-00000380: 5b43 6f64 6520 7374 796c 653a 2062 6c61  [Code style: bla
-00000390: 636b 5d28 6874 7470 733a 2f2f 696d 672e  ck](https://img.
-000003a0: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-000003b0: 2f63 6f64 6525 3230 7374 796c 652d 626c  /code%20style-bl
-000003c0: 6163 6b2d 3030 3030 3030 2e73 7667 3f6c  ack-000000.svg?l
-000003d0: 6f67 6f3d 5079 7468 6f6e 266c 6f67 6f43  ogo=Python&logoC
-000003e0: 6f6c 6f72 3d77 6869 7465 295d 2868 7474  olor=white)](htt
-000003f0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000400: 7073 662f 626c 6163 6b29 205b 215b 4769  psf/black) [![Gi
-00000410: 7470 6f64 2052 6561 6479 2d74 6f2d 436f  tpod Ready-to-Co
-00000420: 6465 5d28 6874 7470 733a 2f2f 696d 672e  de](https://img.
-00000430: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
-00000440: 2f47 6974 706f 642d 7265 6164 792d 2d74  /Gitpod-ready--t
-00000450: 6f2d 2d63 6f64 652d 626c 7565 3f6c 6f67  o--code-blue?log
-00000460: 6f3d 6769 7470 6f64 295d 2868 7474 7073  o=gitpod)](https
-00000470: 3a2f 2f67 6974 706f 642e 696f 2f23 6874  ://gitpod.io/#ht
-00000480: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000490: 2f65 7273 696c 6961 2d6f 732f 6572 7369  /ersilia-os/ersi
-000004a0: 6c69 6129 0a0a 2323 2320 5461 626c 6520  lia)..### Table 
-000004b0: 6f66 2043 6f6e 7465 6e74 733a 0a31 2e20  of Contents:.1. 
-000004c0: 5b50 726f 6a65 6374 2044 6573 6372 6970  [Project Descrip
-000004d0: 7469 6f6e 5d28 6874 7470 733a 2f2f 6769  tion](https://gi
-000004e0: 7468 7562 2e63 6f6d 2f65 7273 696c 6961  thub.com/ersilia
-000004f0: 2d6f 732f 6572 7369 6c69 6123 7072 6f6a  -os/ersilia#proj
-00000500: 6563 742d 6465 7363 7269 7074 696f 6e29  ect-description)
-00000510: 0a32 2e20 5b49 6e73 7461 6c6c 6174 696f  .2. [Installatio
-00000520: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-00000530: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
-00000540: 2f65 7273 696c 6961 2369 6e73 7461 6c6c  /ersilia#install
-00000550: 6174 696f 6e29 0a33 2e20 5b43 6f6e 7472  ation).3. [Contr
-00000560: 6962 7574 655d 2868 7474 7073 3a2f 2f67  ibute](https://g
-00000570: 6974 6875 622e 636f 6d2f 6572 7369 6c69  ithub.com/ersili
-00000580: 612d 6f73 2f65 7273 696c 6961 2363 6f6e  a-os/ersilia#con
-00000590: 7472 6962 7574 6529 0a34 2e20 5b4c 6963  tribute).4. [Lic
-000005a0: 656e 7365 2061 6e64 2063 6974 6174 696f  ense and citatio
-000005b0: 6e5d 2868 7474 7073 3a2f 2f67 6974 6875  n](https://githu
-000005c0: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
-000005d0: 2f65 7273 696c 6961 236c 6963 656e 7365  /ersilia#license
-000005e0: 2d61 6e64 2d63 6974 6174 696f 6e29 0a35  -and-citation).5
-000005f0: 2e20 5b41 626f 7574 2075 735d 2868 7474  . [About us](htt
-00000600: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000610: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-00000620: 6961 2361 626f 7574 2d75 7329 0a0a 2320  ia#about-us)..# 
-00000630: 5072 6f6a 6563 7420 4465 7363 7269 7074  Project Descript
-00000640: 696f 6e0a 5468 6520 4572 7369 6c69 6120  ion.The Ersilia 
-00000650: 4d6f 6465 6c20 4875 6220 6973 2061 2075  Model Hub is a u
-00000660: 6e69 6669 6564 2070 6c61 7466 6f72 6d20  nified platform 
-00000670: 6f66 2070 7265 2d74 7261 696e 6564 2041  of pre-trained A
-00000680: 492f 4d4c 206d 6f64 656c 7320 666f 7220  I/ML models for 
-00000690: 696e 6665 6374 696f 7573 2061 6e64 206e  infectious and n
-000006a0: 6567 6c65 6374 6564 2064 6973 6561 7365  eglected disease
-000006b0: 2072 6573 6561 7263 682e 2054 6865 2065   research. The e
-000006c0: 6e64 2067 6f61 6c20 6973 2074 6f20 7072  nd goal is to pr
-000006d0: 6f76 6964 6520 616e 206f 7065 6e2d 736f  ovide an open-so
-000006e0: 7572 6365 2c20 6e6f 2d63 6f64 6520 736f  urce, no-code so
-000006f0: 6c75 7469 6f6e 2074 6f20 6163 6365 7373  lution to access
-00000700: 2041 492f 4d4c 206d 6f64 656c 7320 746f   AI/ML models to
-00000710: 2061 6363 656c 6572 6174 6520 6472 7567   accelerate drug
-00000720: 2064 6973 636f 7665 7279 2e20 5468 6520   discovery. The 
-00000730: 6d6f 6465 6c73 2065 6d62 6564 6465 6420  models embedded 
-00000740: 696e 2074 6865 2068 7562 2069 6e63 6c75  in the hub inclu
-00000750: 6465 2062 6f74 6820 6d6f 6465 6c73 2070  de both models p
-00000760: 7562 6c69 7368 6564 2069 6e20 7468 6520  ublished in the 
-00000770: 6c69 7465 7261 7475 7265 2028 7769 7468  literature (with
-00000780: 2061 7070 726f 7072 6961 7465 2074 6869   appropriate thi
-00000790: 7264 2070 6172 7479 2061 636b 6e6f 776c  rd party acknowl
-000007a0: 6564 6765 6d65 6e74 2920 616e 6420 6d6f  edgement) and mo
-000007b0: 6465 6c73 2064 6576 656c 6f70 6564 2062  dels developed b
-000007c0: 7920 7468 6520 4572 7369 6c69 6120 7465  y the Ersilia te
-000007d0: 616d 206f 7220 636f 6e74 7269 6275 746f  am or contributo
-000007e0: 7273 2e0a 0a2a 2052 6561 6420 6d6f 7265  rs...* Read more
-000007f0: 2061 626f 7574 2074 6865 2070 726f 6a65   about the proje
-00000800: 6374 2069 6e20 7468 6520 5b45 7273 696c  ct in the [Ersil
-00000810: 6961 2042 6f6f 6b5d 2868 7474 7073 3a2f  ia Book](https:/
-00000820: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
-00000830: 2e69 6f2f 6572 7369 6c69 612d 626f 6f6b  .io/ersilia-book
-00000840: 2f29 0a2a 2042 726f 7773 6520 6176 6169  /).* Browse avai
-00000850: 6c61 626c 6520 6d6f 6465 6c73 2069 6e20  lable models in 
-00000860: 7468 6520 5b45 7273 696c 6961 204d 6f64  the [Ersilia Mod
-00000870: 656c 2048 7562 5d28 6874 7470 733a 2f2f  el Hub](https://
-00000880: 6572 7369 6c69 612e 696f 2f6d 6f64 656c  ersilia.io/model
-00000890: 2d68 7562 2f29 0a3c 7020 616c 6967 6e3d  -hub/).<p align=
-000008a0: 2272 6967 6874 223e 283c 6120 6872 6566  "right">(<a href
-000008b0: 3d22 2374 6f70 223e 6261 636b 2074 6f20  ="#top">back to 
-000008c0: 746f 703c 2f61 3e29 3c2f 703e 0a0a 2320  top</a>)</p>..# 
-000008d0: 5175 6963 6b20 7374 6172 7420 6775 6964  Quick start guid
-000008e0: 650a 506c 6561 7365 2063 6865 636b 2074  e.Please check t
-000008f0: 6865 2070 6163 6b61 6765 2072 6571 7569  he package requi
-00000900: 7265 6d65 6e74 7320 696e 2074 6865 205b  rements in the [
-00000910: 496e 7374 616c 6c61 7469 6f6e 2047 7569  Installation Gui
-00000920: 6465 5d28 6874 7470 733a 2f2f 6572 7369  de](https://ersi
-00000930: 6c69 612e 6769 7462 6f6f 6b2e 696f 2f65  lia.gitbook.io/e
-00000940: 7273 696c 6961 2d62 6f6f 6b2f 7175 6963  rsilia-book/quic
-00000950: 6b2d 7374 6172 742f 696e 7374 616c 6c61  k-start/installa
-00000960: 7469 6f6e 292e 2054 6865 206e 6578 7420  tion). The next 
-00000970: 7374 6570 7320 6172 6520 6120 7175 6963  steps are a quic
-00000980: 6b73 7461 7274 2067 7569 6465 2074 6f20  kstart guide to 
-00000990: 696e 7374 616c 6c69 6e67 2045 7273 696c  installing Ersil
-000009a0: 6961 2e0a 0a31 2e20 4372 6561 7465 2061  ia...1. Create a
-000009b0: 2063 6f6e 6461 2065 6e76 6972 6f6e 6d65   conda environme
-000009c0: 6e74 2061 6e64 2061 6374 6976 6174 6520  nt and activate 
-000009d0: 6974 0a60 6060 0a63 6f6e 6461 2063 7265  it.```.conda cre
-000009e0: 6174 6520 2d6e 2065 7273 696c 6961 2070  ate -n ersilia p
-000009f0: 7974 686f 6e3d 332e 370a 636f 6e64 6120  ython=3.7.conda 
-00000a00: 6163 7469 7661 7465 2065 7273 696c 6961  activate ersilia
-00000a10: 0a60 6060 0a32 2e20 436c 6f6e 6520 7468  .```.2. Clone th
-00000a20: 6973 2072 6570 6f73 6974 6f72 7920 616e  is repository an
-00000a30: 6420 696e 7374 616c 6c20 7769 7468 2070  d install with p
-00000a40: 6970 0a60 6060 0a67 6974 2063 6c6f 6e65  ip.```.git clone
-00000a50: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000a60: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
-00000a70: 7273 696c 6961 2e67 6974 0a63 6420 6572  rsilia.git.cd er
-00000a80: 7369 6c69 610a 7069 7020 696e 7374 616c  silia.pip instal
-00000a90: 6c20 2d65 202e 0a60 6060 200a 332e 204f  l -e ..``` .3. O
-00000aa0: 6e63 6520 7468 6520 4572 7369 6c69 6120  nce the Ersilia 
-00000ab0: 4d6f 6465 6c20 4875 6220 6973 2069 6e73  Model Hub is ins
-00000ac0: 7461 6c6c 6564 2c20 796f 7520 6361 6e20  talled, you can 
-00000ad0: 7573 6520 7468 6520 434c 4920 746f 2072  use the CLI to r
-00000ae0: 756e 2070 7265 6469 6374 696f 6e73 2e20  un predictions. 
-00000af0: 4669 7273 742c 2073 656c 6563 7420 6120  First, select a 
-00000b00: 6d6f 6465 6c20 6672 6f6d 2074 6865 205b  model from the [
-00000b10: 4572 7369 6c69 6120 4d6f 6465 6c20 4875  Ersilia Model Hu
-00000b20: 625d 2868 7474 7073 3a2f 2f65 7273 696c  b](https://ersil
-00000b30: 6961 2e69 6f2f 6d6f 6465 6c2d 6875 622f  ia.io/model-hub/
-00000b40: 2920 616e 6420 2a2a 6665 7463 682a 2a20  ) and **fetch** 
-00000b50: 6974 3a0a 6060 600a 6572 7369 6c69 6120  it:.```.ersilia 
-00000b60: 6665 7463 6820 6368 656d 7072 6f70 2d61  fetch chemprop-a
-00000b70: 6e74 6962 696f 7469 630a 6060 600a 342e  ntibiotic.```.4.
-00000b80: 2047 656e 6572 6174 6520 6120 6665 7720   Generate a few 
-00000b90: 2835 2920 6578 616d 706c 6520 6d6f 6c65  (5) example mole
-00000ba0: 6375 6c65 732c 2074 6f20 6265 2075 7365  cules, to be use
-00000bb0: 6420 6173 2069 6e70 7574 2e20 5468 6520  d as input. The 
-00000bc0: 2a2a 6578 616d 706c 652a 2a20 636f 6d6d  **example** comm
-00000bd0: 616e 6420 7769 6c6c 2067 656e 6572 6174  and will generat
-00000be0: 6520 7468 6520 6164 6571 7561 7465 2069  e the adequate i
-00000bf0: 6e70 7574 2066 6f72 2074 6865 206d 6f64  nput for the mod
-00000c00: 656c 2069 6e20 7573 650a 6060 600a 6572  el in use.```.er
-00000c10: 7369 6c69 6120 6578 616d 706c 6520 6368  silia example ch
-00000c20: 656d 7072 6f70 2d61 6e74 6962 696f 7469  emprop-antibioti
-00000c30: 6320 2d6e 2035 202d 6620 6d79 5f6d 6f6c  c -n 5 -f my_mol
-00000c40: 6563 756c 6573 2e63 7376 0a60 6060 0a35  ecules.csv.```.5
-00000c50: 2e20 5468 656e 2c20 2a2a 7365 7276 652a  . Then, **serve*
-00000c60: 2a20 796f 7572 206d 6f64 656c 3a0a 6060  * your model:.``
-00000c70: 600a 6572 7369 6c69 6120 7365 7276 6520  `.ersilia serve 
-00000c80: 6368 656d 7072 6f70 2d61 6e74 6962 696f  chemprop-antibio
-00000c90: 7469 630a 6060 600a 362e 2041 6e64 2072  tic.```.6. And r
-00000ca0: 756e 2074 6865 2070 7265 6469 6374 696f  un the predictio
-00000cb0: 6e20 2a2a 4150 492a 2a3a 0a60 6060 0a65  n **API**:.```.e
-00000cc0: 7273 696c 6961 2061 7069 202d 6920 6d79  rsilia api -i my
-00000cd0: 5f6d 6f6c 6563 756c 6573 2e63 7376 202d  _molecules.csv -
-00000ce0: 6f20 6d79 5f70 7265 6469 6374 696f 6e73  o my_predictions
-00000cf0: 2e63 7376 0a60 6060 0a37 2e20 4669 6e61  .csv.```.7. Fina
-00000d00: 6c6c 792c 202a 2a63 6c6f 7365 2a2a 2074  lly, **close** t
-00000d10: 6865 2073 6572 7669 6365 2077 6865 6e20  he service when 
-00000d20: 796f 7520 6172 6520 646f 6e65 2e0a 6060  you are done..``
-00000d30: 600a 6572 7369 6c69 6120 636c 6f73 650a  `.ersilia close.
-00000d40: 6060 600a 0a50 6c65 6173 6520 7365 6520  ```..Please see 
-00000d50: 7468 6520 5b45 7273 696c 6961 2042 6f6f  the [Ersilia Boo
-00000d60: 6b5d 2868 7474 7073 3a2f 2f65 7273 696c  k](https://ersil
-00000d70: 6961 2e67 6974 626f 6f6b 2e69 6f2f 6572  ia.gitbook.io/er
-00000d80: 7369 6c69 612d 626f 6f6b 2f29 2066 6f72  silia-book/) for
-00000d90: 206d 6f72 6520 6578 616d 706c 6573 2061   more examples a
-00000da0: 6e64 2064 6574 6169 6c65 6420 6578 706c  nd detailed expl
-00000db0: 616e 6174 696f 6e73 2e0a 3c70 2061 6c69  anations..<p ali
-00000dc0: 676e 3d22 7269 6768 7422 3e28 3c61 2068  gn="right">(<a h
-00000dd0: 7265 663d 2223 746f 7022 3e62 6163 6b20  ref="#top">back 
-00000de0: 746f 2074 6f70 3c2f 613e 293c 2f70 3e0a  to top</a>)</p>.
-00000df0: 0a23 2043 6f6e 7472 6962 7574 650a 5468  .# Contribute.Th
-00000e00: 6520 4572 7369 6c69 6120 4d6f 6465 6c20  e Ersilia Model 
-00000e10: 4875 6220 6973 2061 2046 7265 652c 204f  Hub is a Free, O
-00000e20: 7065 6e20 536f 7572 6365 2053 6f66 7477  pen Source Softw
-00000e30: 6172 6520 616e 6420 7765 2068 6967 686c  are and we highl
-00000e40: 7920 7661 6c75 6520 6e65 7720 636f 6e74  y value new cont
-00000e50: 7269 6275 746f 7273 2e20 5468 6572 6520  ributors. There 
-00000e60: 6172 6520 7365 7665 7261 6c20 7761 7973  are several ways
-00000e70: 2069 6e20 7768 6963 6820 796f 7520 6361   in which you ca
-00000e80: 6e20 636f 6e74 7269 6275 7465 2074 6f20  n contribute to 
-00000e90: 7468 6520 7072 6f6a 6563 743a 0a2a 2041  the project:.* A
-00000ea0: 2067 6f6f 6420 706c 6163 6520 746f 2073   good place to s
-00000eb0: 7461 7274 2069 7320 6368 6563 6b69 6e67  tart is checking
-00000ec0: 206f 7065 6e20 5b69 7373 7565 735d 2868   open [issues](h
-00000ed0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000ee0: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
-00000ef0: 696c 6961 2f69 7373 7565 7329 2e20 0a2a  ilia/issues). .*
-00000f00: 2049 6620 796f 7520 6861 7665 2069 6465   If you have ide
-00000f10: 6e74 6966 6965 6420 6120 6275 6720 696e  ntified a bug in
-00000f20: 2074 6865 2063 6f64 652c 2070 6c65 6173   the code, pleas
-00000f30: 6520 6f70 656e 2061 206e 6577 2069 7373  e open a new iss
-00000f40: 7565 2075 7369 6e67 2074 6865 2062 7567  ue using the bug
-00000f50: 2074 656d 706c 6174 652e 0a2a 2049 6620   template..* If 
-00000f60: 796f 7520 7761 6e74 2074 6f20 696e 636f  you want to inco
-00000f70: 7270 6f72 6174 6520 6120 6e65 7720 6d6f  rporate a new mo
-00000f80: 6465 6c20 696e 2074 6865 2070 6c61 7466  del in the platf
-00000f90: 6f72 6d2c 206f 7065 6e20 6120 6e65 7720  orm, open a new 
-00000fa0: 6973 7375 6520 7573 696e 6720 7468 6520  issue using the 
-00000fb0: 6d6f 6465 6c20 7265 7175 6573 7420 7465  model request te
-00000fc0: 6d70 6c61 7465 206f 7220 636f 6e74 6163  mplate or contac
-00000fd0: 7420 7573 2075 7369 6e67 2074 6865 2066  t us using the f
-00000fe0: 6f6c 6c6f 7769 6e67 205b 666f 726d 5d28  ollowing [form](
-00000ff0: 6874 7470 733a 2f2f 7777 772e 6572 7369  https://www.ersi
-00001000: 6c69 612e 696f 2f72 6571 7565 7374 2d6d  lia.io/request-m
-00001010: 6f64 656c 290a 2a20 5368 6172 6520 616e  odel).* Share an
-00001020: 7920 6665 6564 6261 636b 2077 6974 6820  y feedback with 
-00001030: 7468 6520 636f 6d6d 756e 6974 7920 7573  the community us
-00001040: 696e 6720 5b47 6974 4875 6220 4469 7363  ing [GitHub Disc
-00001050: 7573 7369 6f6e 735d 2868 7474 7073 3a2f  ussions](https:/
-00001060: 2f67 6974 6875 622e 636f 6d2f 6572 7369  /github.com/ersi
-00001070: 6c69 612d 6f73 2f65 7273 696c 6961 2f64  lia-os/ersilia/d
-00001080: 6973 6375 7373 696f 6e73 2920 666f 7220  iscussions) for 
-00001090: 7468 6520 7072 6f6a 6563 740a 2a20 4368  the project.* Ch
-000010a0: 6563 6b20 6f75 7220 5b43 6f6e 7472 6962  eck our [Contrib
-000010b0: 7574 696e 6720 4775 6964 655d 2868 7474  uting Guide](htt
-000010c0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000010d0: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-000010e0: 6961 2f62 6c6f 622f 6d61 7374 6572 2f43  ia/blob/master/C
-000010f0: 4f4e 5452 4942 5554 494e 472e 6d64 2920  ONTRIBUTING.md) 
-00001100: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-00001110: 0a0a 5468 6520 4572 7369 6c69 6120 4f70  ..The Ersilia Op
-00001120: 656e 2053 6f75 7263 6520 496e 6974 6961  en Source Initia
-00001130: 7469 7665 2061 6468 6572 6573 2074 6f20  tive adheres to 
-00001140: 7468 6520 5b43 6f6e 7472 6962 7574 6f72  the [Contributor
-00001150: 2043 6f76 656e 616e 745d 2868 7474 7073   Covenant](https
-00001160: 3a2f 2f65 7273 696c 6961 2e67 6974 626f  ://ersilia.gitbo
-00001170: 6f6b 2e69 6f2f 6572 7369 6c69 612d 7769  ok.io/ersilia-wi
-00001180: 6b69 2f63 6f64 652d 6f66 2d63 6f6e 6475  ki/code-of-condu
-00001190: 6374 2920 636f 6465 206f 6620 636f 6e64  ct) code of cond
-000011a0: 7563 742e 0a3c 7020 616c 6967 6e3d 2272  uct..<p align="r
-000011b0: 6967 6874 223e 283c 6120 6872 6566 3d22  ight">(<a href="
-000011c0: 2374 6f70 223e 6261 636b 2074 6f20 746f  #top">back to to
-000011d0: 703c 2f61 3e29 3c2f 703e 0a0a 2320 4c69  p</a>)</p>..# Li
-000011e0: 6365 6e73 6520 616e 6420 6369 7461 7469  cense and citati
-000011f0: 6f6e 0a54 6869 7320 7265 706f 7369 746f  on.This reposito
-00001200: 7279 2069 7320 6f70 656e 2d73 6f75 7263  ry is open-sourc
-00001210: 6564 2075 6e64 6572 2074 6865 205b 4750  ed under the [GP
-00001220: 4c2d 3320 4c69 6365 6e73 655d 2868 7474  L-3 License](htt
-00001230: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001240: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-00001250: 6961 2f62 6c6f 622f 6d61 7374 6572 2f4c  ia/blob/master/L
-00001260: 4943 454e 5345 292e 0a50 6c65 6173 6520  ICENSE)..Please 
-00001270: 5b63 6974 6520 7573 5d28 6874 7470 733a  [cite us](https:
-00001280: 2f2f 6769 7468 7562 2e63 6f6d 2f65 7273  //github.com/ers
-00001290: 696c 6961 2d6f 732f 6572 7369 6c69 612f  ilia-os/ersilia/
-000012a0: 626c 6f62 2f6d 6173 7465 722f 4349 5441  blob/master/CITA
-000012b0: 5449 4f4e 2e63 6666 2920 6966 2079 6f75  TION.cff) if you
-000012c0: 2075 7365 2069 742e 0a3c 7020 616c 6967   use it..<p alig
-000012d0: 6e3d 2272 6967 6874 223e 283c 6120 6872  n="right">(<a hr
-000012e0: 6566 3d22 2374 6f70 223e 6261 636b 2074  ef="#top">back t
-000012f0: 6f20 746f 703c 2f61 3e29 3c2f 703e 0a0a  o top</a>)</p>..
-00001300: 2320 4162 6f75 7420 7573 0a54 6865 205b  # About us.The [
-00001310: 4572 7369 6c69 6120 4f70 656e 2053 6f75  Ersilia Open Sou
-00001320: 7263 6520 496e 6974 6961 7469 7665 5d28  rce Initiative](
-00001330: 6874 7470 733a 2f2f 6572 7369 6c69 612e  https://ersilia.
-00001340: 696f 2920 6973 2061 204e 6f6e 2050 726f  io) is a Non Pro
-00001350: 6669 7420 4f72 6761 6e69 7a61 7469 6f6e  fit Organization
-00001360: 2028 5b31 3139 3232 3636 5d28 6874 7470   ([1192266](http
-00001370: 733a 2f2f 7265 6769 7374 6572 2d6f 662d  s://register-of-
-00001380: 6368 6172 6974 6965 732e 6368 6172 6974  charities.charit
-00001390: 7963 6f6d 6d69 7373 696f 6e2e 676f 762e  ycommission.gov.
-000013a0: 756b 2f63 6861 7269 7479 2d73 6561 7263  uk/charity-searc
-000013b0: 682f 2d2f 6368 6172 6974 792d 6465 7461  h/-/charity-deta
-000013c0: 696c 732f 3531 3730 3635 372f 6675 6c6c  ils/5170657/full
-000013d0: 2d70 7269 6e74 2929 2077 6974 6820 7468  -print)) with th
-000013e0: 6520 6d69 7373 696f 6e20 6973 2074 6f20  e mission is to 
-000013f0: 6571 7569 7020 6c61 6273 2c20 756e 6976  equip labs, univ
-00001400: 6572 7369 7469 6573 2061 6e64 2063 6c69  ersities and cli
-00001410: 6e69 6373 2069 6e20 4c4d 4943 2077 6974  nics in LMIC wit
-00001420: 6820 4149 2f4d 4c20 746f 6f6c 7320 666f  h AI/ML tools fo
-00001430: 7220 696e 6665 6374 696f 7573 2064 6973  r infectious dis
-00001440: 6561 7365 2072 6573 6561 7263 682e 0a0a  ease research...
-00001450: 5b48 656c 7020 7573 5d28 6874 7470 733a  [Help us](https:
-00001460: 2f2f 7777 772e 6572 7369 6c69 612e 696f  //www.ersilia.io
-00001470: 2f64 6f6e 6174 6529 2061 6368 6965 7665  /donate) achieve
-00001480: 206f 7572 206d 6973 7369 6f6e 206f 7220   our mission or 
-00001490: 5b76 6f6c 756e 7465 6572 5d28 6874 7470  [volunteer](http
-000014a0: 733a 2f2f 7777 772e 6572 7369 6c69 612e  s://www.ersilia.
-000014b0: 696f 2f76 6f6c 756e 7465 6572 2920 7769  io/volunteer) wi
-000014c0: 7468 2075 7321 0a0a 3c70 2061 6c69 676e  th us!..<p align
-000014d0: 3d22 7269 6768 7422 3e28 3c61 2068 7265  ="right">(<a hre
-000014e0: 663d 2223 746f 7022 3e62 6163 6b20 746f  f="#top">back to
-000014f0: 2074 6f70 3c2f 613e 293c 2f70 3e0a        top</a>)</p>.
+00000190: 2920 5b21 5b4c 6963 656e 7365 3a20 4750  ) [![License: GP
+000001a0: 4c20 7633 5d28 6874 7470 733a 2f2f 696d  L v3](https://im
+000001b0: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
+000001c0: 6765 2f4c 6963 656e 7365 2d47 504c 2532  ge/License-GPL%2
+000001d0: 3076 332d 7965 6c6c 6f77 2e73 7667 295d  0v3-yellow.svg)]
+000001e0: 2868 7474 7073 3a2f 2f77 7777 2e67 6e75  (https://www.gnu
+000001f0: 2e6f 7267 2f6c 6963 656e 7365 732f 6167  .org/licenses/ag
+00000200: 706c 2d33 2e30 2920 5b21 5b44 4f49 5d28  pl-3.0) [![DOI](
+00000210: 6874 7470 733a 2f2f 7a65 6e6f 646f 2e6f  https://zenodo.o
+00000220: 7267 2f62 6164 6765 2f32 3737 3036 3839  rg/badge/2770689
+00000230: 3839 2e73 7667 295d 2868 7474 7073 3a2f  89.svg)](https:/
+00000240: 2f7a 656e 6f64 6f2e 6f72 672f 6261 6467  /zenodo.org/badg
+00000250: 652f 6c61 7465 7374 646f 692f 3237 3730  e/latestdoi/2770
+00000260: 3638 3938 3929 0a0a 5b21 5b64 6f63 756d  68989)..[![docum
+00000270: 656e 7461 7469 6f6e 5d28 6874 7470 733a  entation](https:
+00000280: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00000290: 2f62 6164 6765 2f2d 446f 6375 6d65 6e74  /badge/-Document
+000002a0: 6174 696f 6e2d 7075 7270 6c65 3f6c 6f67  ation-purple?log
+000002b0: 6f3d 7265 6164 2d74 6865 2d64 6f63 7326  o=read-the-docs&
+000002c0: 6c6f 676f 436f 6c6f 723d 7768 6974 6529  logoColor=white)
+000002d0: 5d28 6874 7470 733a 2f2f 6572 7369 6c69  ](https://ersili
+000002e0: 612e 6769 7462 6f6f 6b2e 696f 2f65 7273  a.gitbook.io/ers
+000002f0: 696c 6961 2d62 6f6f 6b2f 2920 5b21 5b50  ilia-book/) [![P
+00000300: 7950 4920 7665 7273 696f 6e20 6675 7279  yPI version fury
+00000310: 2e69 6f5d 2868 7474 7073 3a2f 2f62 6164  .io](https://bad
+00000320: 6765 2e66 7572 792e 696f 2f70 792f 6572  ge.fury.io/py/er
+00000330: 7369 6c69 612e 7376 6729 5d28 6874 7470  silia.svg)](http
+00000340: 733a 2f2f 7079 7069 2e70 7974 686f 6e2e  s://pypi.python.
+00000350: 6f72 672f 7079 7069 2f65 7273 696c 6961  org/pypi/ersilia
+00000360: 2f29 205b 215b 5079 7468 6f6e 2033 2e37  /) [![Python 3.7
+00000370: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000380: 6965 6c64 732e 696f 2f62 6164 6765 2f70  ields.io/badge/p
+00000390: 7974 686f 6e2d 332e 372d 626c 7565 2e73  ython-3.7-blue.s
+000003a0: 7667 295d 2868 7474 7073 3a2f 2f77 7777  vg)](https://www
+000003b0: 2e70 7974 686f 6e2e 6f72 672f 646f 776e  .python.org/down
+000003c0: 6c6f 6164 732f 7265 6c65 6173 652f 7079  loads/release/py
+000003d0: 7468 6f6e 2d33 3730 2f29 205b 215b 436f  thon-370/) [![Co
+000003e0: 6465 2073 7479 6c65 3a20 626c 6163 6b5d  de style: black]
+000003f0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000400: 656c 6473 2e69 6f2f 6261 6467 652f 636f  elds.io/badge/co
+00000410: 6465 2532 3073 7479 6c65 2d62 6c61 636b  de%20style-black
+00000420: 2d30 3030 3030 302e 7376 673f 6c6f 676f  -000000.svg?logo
+00000430: 3d50 7974 686f 6e26 6c6f 676f 436f 6c6f  =Python&logoColo
+00000440: 723d 7768 6974 6529 5d28 6874 7470 733a  r=white)](https:
+00000450: 2f2f 6769 7468 7562 2e63 6f6d 2f70 7366  //github.com/psf
+00000460: 2f62 6c61 636b 2920 5b21 5b47 6974 706f  /black) [![Gitpo
+00000470: 6420 5265 6164 792d 746f 2d43 6f64 655d  d Ready-to-Code]
+00000480: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000490: 656c 6473 2e69 6f2f 6261 6467 652f 4769  elds.io/badge/Gi
+000004a0: 7470 6f64 2d72 6561 6479 2d2d 746f 2d2d  tpod-ready--to--
+000004b0: 636f 6465 2d62 6c75 653f 6c6f 676f 3d67  code-blue?logo=g
+000004c0: 6974 706f 6429 5d28 6874 7470 733a 2f2f  itpod)](https://
+000004d0: 6769 7470 6f64 2e69 6f2f 2368 7474 7073  gitpod.io/#https
+000004e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
+000004f0: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
+00000500: 290a 0a23 2320 5461 626c 6520 6f66 2043  )..## Table of C
+00000510: 6f6e 7465 6e74 730a 0a31 2e20 5b50 726f  ontents..1. [Pro
+00000520: 6a65 6374 2044 6573 6372 6970 7469 6f6e  ject Description
+00000530: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000540: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+00000550: 6572 7369 6c69 6123 7072 6f6a 6563 742d  ersilia#project-
+00000560: 6465 7363 7269 7074 696f 6e29 0a32 2e20  description).2. 
+00000570: 5b51 7569 636b 2073 7461 7274 2067 7569  [Quick start gui
+00000580: 6465 5d28 6874 7470 733a 2f2f 6769 7468  de](https://gith
+00000590: 7562 2e63 6f6d 2f65 7273 696c 6961 2d6f  ub.com/ersilia-o
+000005a0: 732f 6572 7369 6c69 6123 7175 6963 6b2d  s/ersilia#quick-
+000005b0: 7374 6172 742d 6775 6964 6529 0a33 2e20  start-guide).3. 
+000005c0: 5b43 6f6e 7472 6962 7574 655d 2868 7474  [Contribute](htt
+000005d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000005e0: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
+000005f0: 6961 2363 6f6e 7472 6962 7574 6529 0a34  ia#contribute).4
+00000600: 2e20 5b4c 6963 656e 7365 2061 6e64 2063  . [License and c
+00000610: 6974 6174 696f 6e5d 2868 7474 7073 3a2f  itation](https:/
+00000620: 2f67 6974 6875 622e 636f 6d2f 6572 7369  /github.com/ersi
+00000630: 6c69 612d 6f73 2f65 7273 696c 6961 236c  lia-os/ersilia#l
+00000640: 6963 656e 7365 2d61 6e64 2d63 6974 6174  icense-and-citat
+00000650: 696f 6e29 0a35 2e20 5b41 626f 7574 2075  ion).5. [About u
+00000660: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000670: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+00000680: 2f65 7273 696c 6961 2361 626f 7574 2d75  /ersilia#about-u
+00000690: 7329 0a0a 2323 2050 726f 6a65 6374 2044  s)..## Project D
+000006a0: 6573 6372 6970 7469 6f6e 0a0a 5468 6520  escription..The 
+000006b0: 4572 7369 6c69 6120 4d6f 6465 6c20 4875  Ersilia Model Hu
+000006c0: 6220 6973 2061 2075 6e69 6669 6564 2070  b is a unified p
+000006d0: 6c61 7466 6f72 6d20 6f66 2070 7265 2d74  latform of pre-t
+000006e0: 7261 696e 6564 2041 492f 4d4c 206d 6f64  rained AI/ML mod
+000006f0: 656c 7320 666f 7220 696e 6665 6374 696f  els for infectio
+00000700: 7573 2061 6e64 206e 6567 6c65 6374 6564  us and neglected
+00000710: 2064 6973 6561 7365 2072 6573 6561 7263   disease researc
+00000720: 682e 2054 6865 2065 6e64 2067 6f61 6c20  h. The end goal 
+00000730: 6973 2074 6f20 7072 6f76 6964 6520 616e  is to provide an
+00000740: 206f 7065 6e2d 736f 7572 6365 2c20 6e6f   open-source, no
+00000750: 2d63 6f64 6520 736f 6c75 7469 6f6e 2074  -code solution t
+00000760: 6f20 6163 6365 7373 2041 492f 4d4c 206d  o access AI/ML m
+00000770: 6f64 656c 7320 746f 2061 6363 656c 6572  odels to acceler
+00000780: 6174 6520 6472 7567 2064 6973 636f 7665  ate drug discove
+00000790: 7279 2e20 5468 6520 6d6f 6465 6c73 2065  ry. The models e
+000007a0: 6d62 6564 6465 6420 696e 2074 6865 2068  mbedded in the h
+000007b0: 7562 2069 6e63 6c75 6465 2062 6f74 6820  ub include both 
+000007c0: 6d6f 6465 6c73 2070 7562 6c69 7368 6564  models published
+000007d0: 2069 6e20 7468 6520 6c69 7465 7261 7475   in the literatu
+000007e0: 7265 2028 7769 7468 2061 7070 726f 7072  re (with appropr
+000007f0: 6961 7465 2074 6869 7264 2070 6172 7479  iate third party
+00000800: 2061 636b 6e6f 776c 6564 6765 6d65 6e74   acknowledgement
+00000810: 2920 616e 6420 6d6f 6465 6c73 2064 6576  ) and models dev
+00000820: 656c 6f70 6564 2062 7920 7468 6520 4572  eloped by the Er
+00000830: 7369 6c69 6120 7465 616d 206f 7220 636f  silia team or co
+00000840: 6e74 7269 6275 746f 7273 2e0a 0a2a 2052  ntributors...* R
+00000850: 6561 6420 6d6f 7265 2061 626f 7574 2074  ead more about t
+00000860: 6865 2070 726f 6a65 6374 2069 6e20 7468  he project in th
+00000870: 6520 5b45 7273 696c 6961 2042 6f6f 6b5d  e [Ersilia Book]
+00000880: 2868 7474 7073 3a2f 2f65 7273 696c 6961  (https://ersilia
+00000890: 2e67 6974 626f 6f6b 2e69 6f2f 6572 7369  .gitbook.io/ersi
+000008a0: 6c69 612d 626f 6f6b 2f29 0a2a 2042 726f  lia-book/).* Bro
+000008b0: 7773 6520 6176 6169 6c61 626c 6520 6d6f  wse available mo
+000008c0: 6465 6c73 2069 6e20 7468 6520 5b45 7273  dels in the [Ers
+000008d0: 696c 6961 204d 6f64 656c 2048 7562 5d28  ilia Model Hub](
+000008e0: 6874 7470 733a 2f2f 6572 7369 6c69 612e  https://ersilia.
+000008f0: 696f 2f6d 6f64 656c 2d68 7562 2f29 0a0a  io/model-hub/)..
+00000900: 2323 2051 7569 636b 2053 7461 7274 2047  ## Quick Start G
+00000910: 7569 6465 0a0a 506c 6561 7365 2063 6865  uide..Please che
+00000920: 636b 2074 6865 2070 6163 6b61 6765 2072  ck the package r
+00000930: 6571 7569 7265 6d65 6e74 7320 696e 2074  equirements in t
+00000940: 6865 205b 496e 7374 616c 6c61 7469 6f6e  he [Installation
+00000950: 2047 7569 6465 5d28 6874 7470 733a 2f2f   Guide](https://
+00000960: 6572 7369 6c69 612e 6769 7462 6f6f 6b2e  ersilia.gitbook.
+00000970: 696f 2f65 7273 696c 6961 2d62 6f6f 6b2f  io/ersilia-book/
+00000980: 7175 6963 6b2d 7374 6172 742f 696e 7374  quick-start/inst
+00000990: 616c 6c61 7469 6f6e 292e 2054 6865 206e  allation). The n
+000009a0: 6578 7420 7374 6570 7320 6172 6520 6120  ext steps are a 
+000009b0: 7175 6963 6b73 7461 7274 2067 7569 6465  quickstart guide
+000009c0: 2074 6f20 696e 7374 616c 6c69 6e67 2045   to installing E
+000009d0: 7273 696c 6961 2e0a 0a31 2e20 4372 6561  rsilia...1. Crea
+000009e0: 7465 2061 2063 6f6e 6461 2065 6e76 6972  te a conda envir
+000009f0: 6f6e 6d65 6e74 2061 6e64 2061 6374 6976  onment and activ
+00000a00: 6174 6520 6974 0a0a 2020 2020 6060 6062  ate it..    ```b
+00000a10: 6173 680a 2020 2020 636f 6e64 6120 6372  ash.    conda cr
+00000a20: 6561 7465 202d 6e20 6572 7369 6c69 6120  eate -n ersilia 
+00000a30: 7079 7468 6f6e 3d33 2e37 0a20 2020 2063  python=3.7.    c
+00000a40: 6f6e 6461 2061 6374 6976 6174 6520 6572  onda activate er
+00000a50: 7369 6c69 610a 2020 2020 6060 600a 0a31  silia.    ```..1
+00000a60: 2e20 436c 6f6e 6520 7468 6973 2072 6570  . Clone this rep
+00000a70: 6f73 6974 6f72 7920 616e 6420 696e 7374  ository and inst
+00000a80: 616c 6c20 7769 7468 2070 6970 0a0a 2020  all with pip..  
+00000a90: 2020 6060 6062 6173 680a 2020 2020 6769    ```bash.    gi
+00000aa0: 7420 636c 6f6e 6520 6874 7470 733a 2f2f  t clone https://
+00000ab0: 6769 7468 7562 2e63 6f6d 2f65 7273 696c  github.com/ersil
+00000ac0: 6961 2d6f 732f 6572 7369 6c69 612e 6769  ia-os/ersilia.gi
+00000ad0: 740a 2020 2020 6364 2065 7273 696c 6961  t.    cd ersilia
+00000ae0: 0a20 2020 2070 6970 2069 6e73 7461 6c6c  .    pip install
+00000af0: 202d 6520 2e0a 2020 2020 6060 600a 0a31   -e ..    ```..1
+00000b00: 2e20 4f6e 6365 2074 6865 2045 7273 696c  . Once the Ersil
+00000b10: 6961 204d 6f64 656c 2048 7562 2069 7320  ia Model Hub is 
+00000b20: 696e 7374 616c 6c65 642c 2079 6f75 2063  installed, you c
+00000b30: 616e 2075 7365 2074 6865 2043 4c49 2074  an use the CLI t
+00000b40: 6f20 7275 6e20 7072 6564 6963 7469 6f6e  o run prediction
+00000b50: 732e 2046 6972 7374 2c20 7365 6c65 6374  s. First, select
+00000b60: 2061 206d 6f64 656c 2066 726f 6d20 7468   a model from th
+00000b70: 6520 5b45 7273 696c 6961 204d 6f64 656c  e [Ersilia Model
+00000b80: 2048 7562 5d28 6874 7470 733a 2f2f 6572   Hub](https://er
+00000b90: 7369 6c69 612e 696f 2f6d 6f64 656c 2d68  silia.io/model-h
+00000ba0: 7562 2f29 2061 6e64 202a 2a66 6574 6368  ub/) and **fetch
+00000bb0: 2a2a 2069 743a 0a0a 2020 2020 6060 6062  ** it:..    ```b
+00000bc0: 6173 680a 2020 2020 6572 7369 6c69 6120  ash.    ersilia 
+00000bd0: 6665 7463 6820 7265 7472 6f73 796e 7468  fetch retrosynth
+00000be0: 6574 6963 2d61 6363 6573 7369 6269 6c69  etic-accessibili
+00000bf0: 7479 0a20 2020 2060 6060 0a0a 312e 2047  ty.    ```..1. G
+00000c00: 656e 6572 6174 6520 6120 6665 7720 2835  enerate a few (5
+00000c10: 2920 6578 616d 706c 6520 6d6f 6c65 6375  ) example molecu
+00000c20: 6c65 732c 2074 6f20 6265 2075 7365 6420  les, to be used 
+00000c30: 6173 2069 6e70 7574 2e20 5468 6520 2a2a  as input. The **
+00000c40: 6578 616d 706c 652a 2a20 636f 6d6d 616e  example** comman
+00000c50: 6420 7769 6c6c 2067 656e 6572 6174 6520  d will generate 
+00000c60: 7468 6520 6164 6571 7561 7465 2069 6e70  the adequate inp
+00000c70: 7574 2066 6f72 2074 6865 206d 6f64 656c  ut for the model
+00000c80: 2069 6e20 7573 650a 0a20 2020 2060 6060   in use..    ```
+00000c90: 6261 7368 0a20 2020 2065 7273 696c 6961  bash.    ersilia
+00000ca0: 2065 7861 6d70 6c65 2072 6574 726f 7379   example retrosy
+00000cb0: 6e74 6865 7469 632d 6163 6365 7373 6962  nthetic-accessib
+00000cc0: 696c 6974 7920 2d6e 2035 202d 6620 6d79  ility -n 5 -f my
+00000cd0: 5f6d 6f6c 6563 756c 6573 2e63 7376 0a20  _molecules.csv. 
+00000ce0: 2020 2060 6060 0a0a 312e 2054 6865 6e2c     ```..1. Then,
+00000cf0: 202a 2a73 6572 7665 2a2a 2079 6f75 7220   **serve** your 
+00000d00: 6d6f 6465 6c3a 0a0a 2020 2020 6060 6062  model:..    ```b
+00000d10: 6173 680a 2020 2020 6572 7369 6c69 6120  ash.    ersilia 
+00000d20: 7365 7276 6520 7265 7472 6f73 796e 7468  serve retrosynth
+00000d30: 6574 6963 2d61 6363 6573 7369 6269 6c69  etic-accessibili
+00000d40: 7479 0a20 2020 2060 6060 0a0a 312e 2041  ty.    ```..1. A
+00000d50: 6e64 2072 756e 2074 6865 2070 7265 6469  nd run the predi
+00000d60: 6374 696f 6e20 2a2a 4150 492a 2a3a 0a0a  ction **API**:..
+00000d70: 2020 2020 6060 6062 6173 680a 2020 2020      ```bash.    
+00000d80: 6572 7369 6c69 6120 6170 6920 2d69 206d  ersilia api -i m
+00000d90: 795f 6d6f 6c65 6375 6c65 732e 6373 7620  y_molecules.csv 
+00000da0: 2d6f 206d 795f 7072 6564 6963 7469 6f6e  -o my_prediction
+00000db0: 732e 6373 760a 2020 2020 6060 600a 0a31  s.csv.    ```..1
+00000dc0: 2e20 4669 6e61 6c6c 792c 202a 2a63 6c6f  . Finally, **clo
+00000dd0: 7365 2a2a 2074 6865 2073 6572 7669 6365  se** the service
+00000de0: 2077 6865 6e20 796f 7520 6172 6520 646f   when you are do
+00000df0: 6e65 2e0a 0a20 2020 2060 6060 6261 7368  ne...    ```bash
+00000e00: 0a20 2020 2065 7273 696c 6961 2063 6c6f  .    ersilia clo
+00000e10: 7365 0a20 2020 2060 6060 0a0a 506c 6561  se.    ```..Plea
+00000e20: 7365 2073 6565 2074 6865 205b 4572 7369  se see the [Ersi
+00000e30: 6c69 6120 426f 6f6b 5d28 6874 7470 733a  lia Book](https:
+00000e40: 2f2f 6572 7369 6c69 612e 6769 7462 6f6f  //ersilia.gitboo
+00000e50: 6b2e 696f 2f65 7273 696c 6961 2d62 6f6f  k.io/ersilia-boo
+00000e60: 6b2f 2920 666f 7220 6d6f 7265 2065 7861  k/) for more exa
+00000e70: 6d70 6c65 7320 616e 6420 6465 7461 696c  mples and detail
+00000e80: 6564 2065 7870 6c61 6e61 7469 6f6e 732e  ed explanations.
+00000e90: 0a0a 2323 2043 6f6e 7472 6962 7574 650a  ..## Contribute.
+00000ea0: 0a54 6865 2045 7273 696c 6961 204d 6f64  .The Ersilia Mod
+00000eb0: 656c 2048 7562 2069 7320 6120 4672 6565  el Hub is a Free
+00000ec0: 2c20 4f70 656e 2053 6f75 7263 6520 536f  , Open Source So
+00000ed0: 6674 7761 7265 2061 6e64 2077 6520 6869  ftware and we hi
+00000ee0: 6768 6c79 2076 616c 7565 206e 6577 2063  ghly value new c
+00000ef0: 6f6e 7472 6962 7574 6f72 732e 2054 6865  ontributors. The
+00000f00: 7265 2061 7265 2073 6576 6572 616c 2077  re are several w
+00000f10: 6179 7320 696e 2077 6869 6368 2079 6f75  ays in which you
+00000f20: 2063 616e 2063 6f6e 7472 6962 7574 6520   can contribute 
+00000f30: 746f 2074 6865 2070 726f 6a65 6374 3a0a  to the project:.
+00000f40: 0a2a 2041 2067 6f6f 6420 706c 6163 6520  .* A good place 
+00000f50: 746f 2073 7461 7274 2069 7320 6368 6563  to start is chec
+00000f60: 6b69 6e67 206f 7065 6e20 5b69 7373 7565  king open [issue
+00000f70: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
+00000f80: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+00000f90: 2f65 7273 696c 6961 2f69 7373 7565 7329  /ersilia/issues)
+00000fa0: 2e0a 2a20 4966 2079 6f75 2068 6176 6520  ..* If you have 
+00000fb0: 6964 656e 7469 6669 6564 2061 2062 7567  identified a bug
+00000fc0: 2069 6e20 7468 6520 636f 6465 2c20 706c   in the code, pl
+00000fd0: 6561 7365 206f 7065 6e20 6120 6e65 7720  ease open a new 
+00000fe0: 6973 7375 6520 7573 696e 6720 7468 6520  issue using the 
+00000ff0: 6275 6720 7465 6d70 6c61 7465 2e0a 2a20  bug template..* 
+00001000: 5368 6172 6520 616e 7920 6665 6564 6261  Share any feedba
+00001010: 636b 2077 6974 6820 7468 6520 636f 6d6d  ck with the comm
+00001020: 756e 6974 7920 7573 696e 6720 5b47 6974  unity using [Git
+00001030: 4875 6220 4469 7363 7573 7369 6f6e 735d  Hub Discussions]
+00001040: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001050: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
+00001060: 7273 696c 6961 2f64 6973 6375 7373 696f  rsilia/discussio
+00001070: 6e73 2920 666f 7220 7468 6520 7072 6f6a  ns) for the proj
+00001080: 6563 740a 2a20 4368 6563 6b20 6f75 7220  ect.* Check our 
+00001090: 5b43 6f6e 7472 6962 7574 696e 6720 4775  [Contributing Gu
+000010a0: 6964 655d 2868 7474 7073 3a2f 2f67 6974  ide](https://git
+000010b0: 6875 622e 636f 6d2f 6572 7369 6c69 612d  hub.com/ersilia-
+000010c0: 6f73 2f65 7273 696c 6961 2f62 6c6f 622f  os/ersilia/blob/
+000010d0: 6d61 7374 6572 2f43 4f4e 5452 4942 5554  master/CONTRIBUT
+000010e0: 494e 472e 6d64 2920 666f 7220 6d6f 7265  ING.md) for more
+000010f0: 2064 6574 6169 6c73 0a0a 5468 6520 4572   details..The Er
+00001100: 7369 6c69 6120 4f70 656e 2053 6f75 7263  silia Open Sourc
+00001110: 6520 496e 6974 6961 7469 7665 2061 6468  e Initiative adh
+00001120: 6572 6573 2074 6f20 7468 6520 5b43 6f6e  eres to the [Con
+00001130: 7472 6962 7574 6f72 2043 6f76 656e 616e  tributor Covenan
+00001140: 745d 2868 7474 7073 3a2f 2f65 7273 696c  t](https://ersil
+00001150: 6961 2e67 6974 626f 6f6b 2e69 6f2f 6572  ia.gitbook.io/er
+00001160: 7369 6c69 612d 7769 6b69 2f63 6f64 652d  silia-wiki/code-
+00001170: 6f66 2d63 6f6e 6475 6374 2920 636f 6465  of-conduct) code
+00001180: 206f 6620 636f 6e64 7563 742e 0a0a 2323   of conduct...##
+00001190: 2320 5375 626d 6974 2061 204e 6577 204d  # Submit a New M
+000011a0: 6f64 656c 0a0a 4966 2079 6f75 2077 616e  odel..If you wan
+000011b0: 7420 746f 2069 6e63 6f72 706f 7261 7465  t to incorporate
+000011c0: 2061 206e 6577 206d 6f64 656c 2069 6e20   a new model in 
+000011d0: 7468 6520 706c 6174 666f 726d 2c20 6f70  the platform, op
+000011e0: 656e 2061 206e 6577 2069 7373 7565 2075  en a new issue u
+000011f0: 7369 6e67 2074 6865 205b 6d6f 6465 6c20  sing the [model 
+00001200: 7265 7175 6573 7420 7465 6d70 6c61 7465  request template
+00001210: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001220: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+00001230: 6572 7369 6c69 612f 6973 7375 6573 2f6e  ersilia/issues/n
+00001240: 6577 3f61 7373 6967 6e65 6573 3d26 6c61  ew?assignees=&la
+00001250: 6265 6c73 3d6e 6577 2d6d 6f64 656c 2674  bels=new-model&t
+00001260: 656d 706c 6174 653d 6d6f 6465 6c5f 7265  emplate=model_re
+00001270: 7175 6573 742e 796d 6c26 7469 746c 653d  quest.yml&title=
+00001280: 2546 3025 3946 2541 3625 4130 2b4d 6f64  %F0%9F%A6%A0+Mod
+00001290: 656c 2b52 6571 7565 7374 2533 412b 2533  el+Request%3A+%3
+000012a0: 436e 616d 6525 3345 2920 6f72 2063 6f6e  Cname%3E) or con
+000012b0: 7461 6374 2075 7320 7573 696e 6720 7468  tact us using th
+000012c0: 6520 666f 6c6c 6f77 696e 6720 5b66 6f72  e following [for
+000012d0: 6d5d 2868 7474 7073 3a2f 2f77 7777 2e65  m](https://www.e
+000012e0: 7273 696c 6961 2e69 6f2f 7265 7175 6573  rsilia.io/reques
+000012f0: 742d 6d6f 6465 6c29 2e0a 0a41 6674 6572  t-model)...After
+00001300: 2073 7562 6d69 7474 696e 6720 796f 7572   submitting your
+00001310: 206d 6f64 656c 2072 6571 7565 7374 2076   model request v
+00001320: 6961 2061 6e20 6973 7375 6520 2873 7567  ia an issue (sug
+00001330: 6765 7374 6564 292c 2061 206d 6169 6e74  gested), a maint
+00001340: 6169 6e65 7220 7769 6c6c 2072 6576 6965  ainer will revie
+00001350: 7720 796f 7572 2072 6571 7565 7374 2e20  w your request. 
+00001360: 4966 2074 6865 7920 602f 6170 7072 6f76  If they `/approv
+00001370: 6560 2079 6f75 7220 7265 7175 6573 742c  e` your request,
+00001380: 2061 206e 6577 206d 6f64 656c 2072 6573   a new model res
+00001390: 706f 7369 746f 7279 2077 696c 6c20 6265  pository will be
+000013a0: 2063 7265 6174 6564 2066 6f72 2079 6f75   created for you
+000013b0: 2074 6f20 666f 726b 2061 6e64 2075 7365   to fork and use
+000013c0: 2120 5468 6572 6520 6973 2061 205b 6465  ! There is a [de
+000013d0: 6d6f 2072 6570 6f73 6974 6f72 795d 2868  mo repository](h
+000013e0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000013f0: 6d2f 6572 7369 6c69 612d 6f73 2f65 6f73  m/ersilia-os/eos
+00001400: 2d64 656d 6f29 2065 7870 6c61 696e 696e  -demo) explainin
+00001410: 6720 7468 6520 7374 6570 7320 6f6e 652d  g the steps one-
+00001420: 6279 2d6f 6e65 2e0a 0a23 2320 4c69 6365  by-one...## Lice
+00001430: 6e73 6520 616e 6420 4369 7461 7469 6f6e  nse and Citation
+00001440: 0a0a 5468 6973 2072 6570 6f73 6974 6f72  ..This repositor
+00001450: 7920 6973 206f 7065 6e2d 736f 7572 6365  y is open-source
+00001460: 6420 756e 6465 7220 7468 6520 5b47 504c  d under the [GPL
+00001470: 2d33 204c 6963 656e 7365 5d28 6874 7470  -3 License](http
+00001480: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00001490: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
+000014a0: 612f 626c 6f62 2f6d 6173 7465 722f 4c49  a/blob/master/LI
+000014b0: 4345 4e53 4529 2e0a 506c 6561 7365 205b  CENSE)..Please [
+000014c0: 6369 7465 2075 735d 2868 7474 7073 3a2f  cite us](https:/
+000014d0: 2f67 6974 6875 622e 636f 6d2f 6572 7369  /github.com/ersi
+000014e0: 6c69 612d 6f73 2f65 7273 696c 6961 2f62  lia-os/ersilia/b
+000014f0: 6c6f 622f 6d61 7374 6572 2f43 4954 4154  lob/master/CITAT
+00001500: 494f 4e2e 6366 6629 2069 6620 796f 7520  ION.cff) if you 
+00001510: 7573 6520 6974 210a 0a23 2320 4162 6f75  use it!..## Abou
+00001520: 7420 5573 0a0a 5468 6520 5b45 7273 696c  t Us..The [Ersil
+00001530: 6961 204f 7065 6e20 536f 7572 6365 2049  ia Open Source I
+00001540: 6e69 7469 6174 6976 655d 2868 7474 7073  nitiative](https
+00001550: 3a2f 2f65 7273 696c 6961 2e69 6f29 2069  ://ersilia.io) i
+00001560: 7320 6120 4e6f 6e20 5072 6f66 6974 204f  s a Non Profit O
+00001570: 7267 616e 697a 6174 696f 6e20 285b 3131  rganization ([11
+00001580: 3932 3236 365d 2868 7474 7073 3a2f 2f72  92266](https://r
+00001590: 6567 6973 7465 722d 6f66 2d63 6861 7269  egister-of-chari
+000015a0: 7469 6573 2e63 6861 7269 7479 636f 6d6d  ties.charitycomm
+000015b0: 6973 7369 6f6e 2e67 6f76 2e75 6b2f 6368  ission.gov.uk/ch
+000015c0: 6172 6974 792d 7365 6172 6368 2f2d 2f63  arity-search/-/c
+000015d0: 6861 7269 7479 2d64 6574 6169 6c73 2f35  harity-details/5
+000015e0: 3137 3036 3537 2f66 756c 6c2d 7072 696e  170657/full-prin
+000015f0: 7429 2920 7769 7468 2074 6865 206d 6973  t)) with the mis
+00001600: 7369 6f6e 2069 7320 746f 2065 7175 6970  sion is to equip
+00001610: 206c 6162 732c 2075 6e69 7665 7273 6974   labs, universit
+00001620: 6965 7320 616e 6420 636c 696e 6963 7320  ies and clinics 
+00001630: 696e 204c 4d49 4320 7769 7468 2041 492f  in LMIC with AI/
+00001640: 4d4c 2074 6f6f 6c73 2066 6f72 2069 6e66  ML tools for inf
+00001650: 6563 7469 6f75 7320 6469 7365 6173 6520  ectious disease 
+00001660: 7265 7365 6172 6368 2e0a 0a5b 4865 6c70  research...[Help
+00001670: 2075 735d 2868 7474 7073 3a2f 2f77 7777   us](https://www
+00001680: 2e65 7273 696c 6961 2e69 6f2f 646f 6e61  .ersilia.io/dona
+00001690: 7465 2920 6163 6869 6576 6520 6f75 7220  te) achieve our 
+000016a0: 6d69 7373 696f 6e20 6f72 205b 766f 6c75  mission or [volu
+000016b0: 6e74 6565 725d 2868 7474 7073 3a2f 2f77  nteer](https://w
+000016c0: 7777 2e65 7273 696c 6961 2e69 6f2f 766f  ww.ersilia.io/vo
+000016d0: 6c75 6e74 6565 7229 2077 6974 6820 7573  lunteer) with us
+000016e0: 210a                                     !.
```

### Comparing `ersilia-0.1.1/ersilia/__init__.py` & `ersilia-0.1.8/ersilia/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,38 @@
-# Version
-from ._version import __version__
-
-del _version
-
 # External imports
 import os
+from ._version import __version__
 
 # Disable GPU
 os.environ["CUDA_VISIBLE_DEVICES"] = "-1"
 
 # Default variables
 from .default import EOS, CONFIG_JSON, INSTALL_STATUS_FILE
 
+# Logger
+from .utils.logging import logger
+
+# Config
 if not os.path.exists(os.path.join(EOS, CONFIG_JSON)):
     from .utils.config import Checker
 
     Checker().config()
 
-# Logger
-from .utils.logging import logger
+# Exceptions
+from .utils.exceptions_utils.throw_ersilia_exception import throw_ersilia_exception
 
 # Environmental variables
 os.environ["EOS_HOME"] = EOS
 
 # Global imports
 from .utils.config import Config
 from .core.base import ErsiliaBase
 from .core.modelbase import ModelBase
 from .core.model import ErsiliaModel
 
-# Clean version
-from ._clean_static_version import version
-
-script_path = os.path.dirname(os.path.abspath(__file__))
-clean_version_file = os.path.join(script_path, "_clean_static_version.py")
-if __version__[:7] == "unknown":
-    __version__ = version
-else:
-    ver = __version__.split(".")
-    ver = "{0}.{1}.{2}".format(ver[0], ver[1], ver[2].split("+")[0])
-    if ver != version:
-        with open(clean_version_file, "w") as f:
-            f.write('version = "{0}"'.format(ver))
-    __version__ = ver
-
-
 # User profile
 from .default import bashrc_cli_snippet
 
 bashrc_cli_snippet(overwrite=False)
 
 
 # Check status of installs
@@ -60,9 +44,7 @@
         with open(fn, "r") as f:
             status = f.read().strip()
     results = {"install_status_file": fn, "status": status}
     return results
 
 
 INSTALL_STATUS = check_install_status()["status"]
-
-__all__ = ["__version__"]
```

### Comparing `ersilia-0.1.1/ersilia/app/app.py` & `ersilia-0.1.8/ersilia/app/app.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/app/blocks/streamlit.py` & `ersilia-0.1.8/ersilia/app/blocks/streamlit.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/auth/auth.py` & `ersilia-0.1.8/ersilia/auth/auth.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/cmd.py` & `ersilia-0.1.8/ersilia/cli/cmd.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,22 +33,34 @@
         m = importlib.import_module("ersilia.cli.commands.delete")
         m.delete_cmd()
 
     def example(self):
         m = importlib.import_module("ersilia.cli.commands.example")
         m.example_cmd()
 
+    def info(self):
+        m = importlib.import_module("ersilia.cli.commands.info")
+        m.info_cmd()
+
     def fetch(self):
         m = importlib.import_module("ersilia.cli.commands.fetch")
         m.fetch_cmd()
 
     def publish(self):
         m = importlib.import_module("ersilia.cli.commands.publish")
         m.publish_cmd()
 
+    def sample(self):
+        m = importlib.import_module("ersilia.cli.commands.sample")
+        m.sample_cmd()
+
     def serve(self):
         m = importlib.import_module("ersilia.cli.commands.serve")
         m.serve_cmd()
 
     def setup(self):
         m = importlib.import_module("ersilia.cli.commands.setup")
         m.setup_cmd()
+
+    def test(self):
+        m = importlib.import_module("ersilia.cli.commands.test")
+        m.test_cmd()
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/__init__.py` & `ersilia-0.1.8/ersilia/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/commands/api.py` & `ersilia-0.1.8/ersilia/cli/commands/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .. import echo
 from ... import ErsiliaModel
 from ...core.session import Session
 
 
 def api_cmd():
     """Create api command"""
+
     # Example usage: ersilia api {API_NAME} -i {INPUT} [-o {OUTPUT} -b {BATCH_SIZE}]
     @ersilia_cli.command(
         short_help="Run API on a served model", help="Run API on a served model"
     )
     @click.argument("api_name", required=False, default=None, type=click.STRING)
     @click.option("-i", "--input", "input", required=True, type=click.STRING)
     @click.option(
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/card.py` & `ersilia-0.1.8/ersilia/cli/commands/card.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import click
-import json
 
 from . import ersilia_cli
 from ...hub.content.card import ModelCard, LakeCard
-from ...serve.schema import ApiSchema
 from ... import ModelBase
 
 
 def card_cmd():
     """Creates card command"""
+
     # Example usage: ersilia card {MODEL}
     @ersilia_cli.command(
         short_help="Get model info card",
         help="Get model info card from Ersilia Model Hub.",
     )
     @click.argument("model", type=click.STRING)
     @click.option(
@@ -29,17 +28,17 @@
         "-a", "--api", is_flag=True, default=False, help="Show a list of available API"
     )
     def card(model, schema, lake, api):
         mdl = ModelBase(model)
         model_id = mdl.model_id
         if schema:
             mc = ModelCard()
-            click.echo(mc.get(model_id, as_json=True))
+            click.echo(mc.get(model_id, as_json=True))  # TODO
             return
         if lake:
             mc = LakeCard()
             click.echo(mc.get(model_id, as_json=True))
             return
         if api:
             pass  # TODO
-        ac = ApiSchema(model_id, config_json=None)
-        click.echo(json.dumps(ac.get(), indent=4))
+        mc = ModelCard()
+        click.echo(mc.get(model_id, as_json=True))
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/catalog.py` & `ersilia-0.1.8/ersilia/cli/commands/catalog.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from ...hub.content.catalog import ModelCatalog
 from ...hub.content.search import ModelSearcher
 from ...hub.content.table_update import table
 
 
 def catalog_cmd():
     """Creates catalog command"""
+
     # Example usage: ersilia catalog
     @ersilia_cli.command(help="List a catalog of models")
     @click.option(
         "-l",
         "--local",
         is_flag=True,
         default=False,
@@ -37,15 +38,14 @@
     )
     @click.option(
         "-p", "--previous", is_flag=True, default=False, help="Shows previous table"
     )
     def catalog(
         local=False, search=None, text=None, mode=None, next=False, previous=False
     ):
-
         mc = ModelCatalog()
         if not (local or text or mode):
             catalog = mc.hub()
             if not (next or previous):
                 catalog = table(catalog).initialise()
 
             if next:
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/close.py` & `ersilia-0.1.8/ersilia/cli/commands/close.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/commands/delete.py` & `ersilia-0.1.8/ersilia/cli/commands/delete.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/commands/deploy.py` & `ersilia-0.1.8/ersilia/cli/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/commands/example.py` & `ersilia-0.1.8/ersilia/cli/commands/example.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import click
 import json
 
 from . import ersilia_cli
 from .. import echo
 from ...io.input import ExampleGenerator
+from ...core.session import Session
 from ... import ModelBase
 
 
 def example_cmd():
     """Create example command"""
 
     # Example usage: ersilia example {MODEL} -n 10 [--file_name {FILE_NAME} --simple/--complete]
     @ersilia_cli.command(
         short_help="Generate input examples for the model of interest",
         help="This command generates input examples to be tested for the model of interest. The number of examples can be specified, as well as a file name. Simple inputs only contain the essential information, while complete inputs contain key and other fields, potentially.",
     )
-    @click.argument("model", type=click.STRING)
+    @click.argument("model", required=False, default=None, type=click.STRING)
     @click.option("--n_samples", "-n", default=5, type=click.INT)
     @click.option("--file_name", "-f", default=None, type=click.STRING)
     @click.option("--simple/--complete", "-s/-c", default=True)
     def example(model, n_samples, file_name, simple):
-        model_id = ModelBase(model).model_id
-        eg = ExampleGenerator(model_id)
+        if model is not None:
+            model_id = ModelBase(model).model_id
+        else:
+            session = Session(config_json=None)
+            model_id = session.current_model_id()
+        eg = ExampleGenerator(model_id=model_id)
         if file_name is None:
             echo(json.dumps(eg.example(n_samples, file_name, simple), indent=4))
         else:
             eg.example(n_samples, file_name, simple)
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/fetch.py` & `ersilia-0.1.8/ersilia/cli/commands/fetch.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,17 +18,27 @@
         "downloaded from a file storage system such as the Open Science Framework. Model is downloaded to "
         "an EOS folder, then packed to a BentoML bundle",
     )
     @click.argument("model", type=click.STRING)
     @click.option("--repo_path", "-r", default=None, type=click.STRING)
     @click.option("--mode", "-m", default=None, type=click.STRING)
     @click.option("--dockerize/--not-dockerize", default=False)
-    def fetch(model, repo_path, mode, dockerize):
-        mdl = ModelBase(model)
+    @click.option(
+        "--overwrite/--reuse",
+        default=True,
+        help="Overwrite environment or reuse using already available environment for this model",
+    )
+    def fetch(model, repo_path, mode, dockerize, overwrite):
+        if repo_path is not None:
+            mdl = ModelBase(repo_path=repo_path)
+        else:
+            mdl = ModelBase(model_id_or_slug=model)
         model_id = mdl.model_id
         echo(
             ":down_arrow:  Fetching model {0}: {1}".format(model_id, mdl.slug),
             fg="blue",
         )
-        mf = ModelFetcher(repo_path=repo_path, mode=mode, dockerize=dockerize)
+        mf = ModelFetcher(
+            repo_path=repo_path, mode=mode, dockerize=dockerize, overwrite=overwrite
+        )
         _fetch(mf, model_id)
         echo(":thumbs_up: Model {0} fetched successfully!".format(model_id), fg="green")
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/publish.py` & `ersilia-0.1.8/ersilia/cli/commands/publish.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/commands/serve.py` & `ersilia-0.1.8/ersilia/cli/commands/serve.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,37 @@
 import click
-import os
-from ...utils import tmp_pid_file
 from . import ersilia_cli
 from .. import echo
 from ... import ErsiliaModel
 from ..messages import ModelNotFound
 
 
 def serve_cmd():
     """Creates serve command"""
+
     # Example usage: ersilia serve {MODEL}
     @ersilia_cli.command(short_help="Serve model", help="Serve model")
     @click.argument("model", type=click.STRING)
     @click.option("--lake/--no-lake", is_flag=True, default=True)
     @click.option("--docker/--no-docker", is_flag=True, default=False)
-    def serve(model, lake, docker):
+    @click.option(
+        "--port",
+        "-p",
+        default=None,
+        type=click.INT,
+        help="Preferred port to use (integer)",
+    )
+    def serve(model, lake, docker, port):
         if docker:
             service_class = "docker"
         else:
             service_class = None
-        mdl = ErsiliaModel(model, save_to_lake=lake, service_class=service_class)
+        mdl = ErsiliaModel(
+            model, save_to_lake=lake, service_class=service_class, preferred_port=port
+        )
         if not mdl.is_valid():
             ModelNotFound(mdl).echo()
         mdl.serve()
         if mdl.url is None:
             echo("No URL found. Service unsuccessful.", fg="red")
             return
         echo(
@@ -34,7 +42,10 @@
         echo("   PID: {0}".format(mdl.pid), fg="yellow")
         echo("   SRV: {0}".format(mdl.scl), fg="yellow")
         echo("")
         echo(":backhand_index_pointing_right: Available APIs:", fg="blue")
         apis = mdl.get_apis()
         for api in apis:
             echo("   - {0}".format(api), fg="blue")
+        echo("")
+        echo(":person_tipping_hand: Information:", fg="blue")
+        echo("   - info", fg="blue")
```

### Comparing `ersilia-0.1.1/ersilia/cli/commands/setup.py` & `ersilia-0.1.8/ersilia/cli/commands/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from . import ersilia_cli
 from ...utils.installers import base_installer, full_installer
 
 
 def setup_cmd():
     """Creates setup command"""
+
     # Example usage: ersilia setup
     @ersilia_cli.command(
         short_help="Setup ersilia",
         help="Setup ersilia, including building a model-server image, a base environment (eos), rdkit, etc.",
     )
     @click.option(
         "--base",
```

### Comparing `ersilia-0.1.1/ersilia/cli/create_cli.py` & `ersilia-0.1.8/ersilia/cli/create_cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 
 
 def create_ersilia_cli():
     is_contributor = Auth().is_contributor()
 
     cmd = Command()
 
-    cmd.auth()
-    cmd.fetch()
-    cmd.delete()
-    cmd.serve()
-    cmd.close()
     cmd.api()
-    cmd.example()
-    cmd.catalog()
+    cmd.auth()
     cmd.card()
+    cmd.catalog()
     cmd.clear()
+    cmd.close()
+    cmd.delete()
+    cmd.example()
+    cmd.fetch()
+    cmd.info()
+    cmd.test()
 
     # TODO: publishing functionalities
     if is_contributor:
         cmd.publish()
 
+    cmd.sample()
+    cmd.serve()
+
     # TODO: functions only for contributors
     # Functions only for contributors
     if is_contributor:
         cmd.setup()
 
     return ersilia_cli
```

### Comparing `ersilia-0.1.1/ersilia/cli/echo.py` & `ersilia-0.1.8/ersilia/cli/echo.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/cli/messages.py` & `ersilia-0.1.8/ersilia/cli/messages.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/core/base.py` & `ersilia-0.1.8/ersilia/core/base.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/core/model.py` & `ersilia-0.1.8/ersilia/core/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,16 +20,18 @@
 from ..io.readers.file import FileTyper, TabularFileReader
 from ..utils import tmp_pid_file
 from ..utils.hdf5 import Hdf5DataLoader
 from ..utils.csvfile import CsvDataLoader
 from ..utils.terminal import yes_no_input
 from ..lake.base import LakeBase
 
+from ..utils.exceptions_utils.api_exceptions import ApiSpecifiedOutputError
+
 from ..default import FETCHED_MODELS_FILENAME, MODEL_SIZE_FILE, CARD_FILE, EOS
-from ..default import DEFAULT_BATCH_SIZE
+from ..default import DEFAULT_BATCH_SIZE, APIS_LIST_FILE, INFORMATION_FILE
 
 try:
     import pandas as pd
 except ModuleNotFoundError:
     pd = None
 
 
@@ -39,14 +41,15 @@
         model,
         save_to_lake=True,
         service_class=None,
         config_json=None,
         credentials_json=None,
         verbose=None,
         fetch_if_not_available=True,
+        preferred_port=None,
     ):
         ErsiliaBase.__init__(
             self, config_json=config_json, credentials_json=credentials_json
         )
         self.logger = logger
         if verbose is not None:
             if verbose:
@@ -82,35 +85,41 @@
         self.config_json = config_json
         self.model_id = mdl.model_id
         self.slug = mdl.slug
         self.text = mdl.text
         self._is_available_locally = mdl.is_available_locally()
         if not self._is_available_locally and fetch_if_not_available:
             self.logger.info("Model is not available locally")
-            do_fetch = yes_no_input(
-                "Requested model {0} if not available locally. Do you want to fetch it? [Y/n]".format(
-                    self.model_id
-                ),
-                default_answer="Y",
-            )
+            try:
+                do_fetch = yes_no_input(
+                    "Requested model {0} is not available locally. Do you want to fetch it? [Y/n]".format(
+                        self.model_id
+                    ),
+                    default_answer="Y",
+                )
+            except:
+                self.logger.debug("Unable to capture user input. Fetching anyway.")
+                do_fetch = True
             if do_fetch:
                 fetch = importlib.import_module("ersilia.hub.fetch.fetch")
                 mf = fetch.ModelFetcher(
                     config_json=self.config_json, credentials_json=self.credentials_json
                 )
                 mf.fetch(self.model_id)
             else:
                 return
         self.api_schema = ApiSchema(
             model_id=self.model_id, config_json=self.config_json
         )
+        self.preferred_port = preferred_port
         self.autoservice = AutoService(
             model_id=self.model_id,
             service_class=self.service_class,
             config_json=self.config_json,
+            preferred_port=preferred_port,
         )
         self._set_apis()
         self.session = Session(config_json=self.config_json)
 
     def __enter__(self):
         self.serve()
         return self
@@ -125,15 +134,15 @@
         def _method(input=None, output=None, batch_size=DEFAULT_BATCH_SIZE):
             return self.api(api_name, input, output, batch_size)
 
         setattr(self, api_name, _method)
 
     def _set_apis(self):
         apis_list = os.path.join(
-            self._get_bundle_location(self.model_id), "apis_list.txt"
+            self._get_bundle_location(self.model_id), APIS_LIST_FILE
         )
         api_names = []
         if os.path.exists(apis_list):
             with open(apis_list, "r") as f:
                 for l in f:
                     api_name = l.rstrip()
                     api_names += [api_name]
@@ -264,14 +273,16 @@
     def _get_api_runner(self, output):
         if output is None:
             use_iter = True
         elif self.__output_is_file(output):
             use_iter = True
         elif self.__output_is_format(output):
             use_iter = False
+        else:
+            raise ApiSpecifiedOutputError
         if use_iter:
             return self._api_runner_iter
         else:
             return self._api_runner_return
 
     def _evaluate_do_cache_splits(self, input, output):
         if input is None:
@@ -307,28 +318,31 @@
         else:
             return False
 
     def api(
         self, api_name=None, input=None, output=None, batch_size=DEFAULT_BATCH_SIZE
     ):
         if self._do_cache_splits(input=input, output=output):
-            splitted_inputs = self.tfr.split_in_cache(input)
+            splitted_inputs = self.tfr.split_in_cache()
+            self.logger.debug("Split inputs:")
+            self.logger.debug(" ".join(splitted_inputs))
             splitted_outputs = self.tfr.name_cached_output_files(
                 splitted_inputs, output
             )
             for input_, output_ in zip(splitted_inputs, splitted_outputs):
                 self.api_task(
                     api_name=api_name,
                     input=input_,
                     output=output_,
                     batch_size=batch_size,
                 )
             TabularOutputStacker(splitted_outputs).stack(output)
             return output
         else:
+            self.logger.debug("No file splitting necessary!")
             return self.api_task(
                 api_name=api_name, input=input, output=output, batch_size=batch_size
             )
 
     def api_task(self, api_name, input, output, batch_size):
         api_instance = self._get_api_instance(api_name=api_name)
         api_runner = self._get_api_runner(output=output)
@@ -410,7 +424,14 @@
             os.path.join(self._model_path(self.model_id), MODEL_SIZE_FILE), "r"
         ) as f:
             return json.load(f)
 
     def example(self, n_samples, file_name=None, simple=True):
         eg = ExampleGenerator(model_id=self.model_id, config_json=self.config_json)
         return eg.example(n_samples=n_samples, file_name=file_name, simple=simple)
+
+    def info(self):
+        information_file = os.path.join(
+            self._model_path(self.model_id), INFORMATION_FILE
+        )
+        with open(information_file, "r") as f:
+            return json.load(f)
```

### Comparing `ersilia-0.1.1/ersilia/core/modelbase.py` & `ersilia-0.1.8/ersilia/core/session.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,51 +1,58 @@
-import os
-import sys
 import json
+import time
+import uuid
+import os
 
-from .. import ErsiliaBase
-from ..hub.content.slug import Slug
-from ..hub.fetch import STATUS_FILE, DONE_TAG
+from .base import ErsiliaBase
+from ..default import EOS
 
-from ..utils.exceptions import InvalidModelIdentifierError
 
+class Session(ErsiliaBase):
+    def __init__(self, config_json):
+        ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
+        self.session_file = os.path.join(EOS, "session.json")
 
-class ModelBase(ErsiliaBase):
-    """Base class of a Model."""
+    def current_model_id(self):
+        data = self.get()
+        if data is None:
+            return None
+        else:
+            return data["model_id"]
 
-    def __init__(self, model_id_or_slug, config_json=None):
-        ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
-        self.text = model_id_or_slug
-        slugger = Slug()
-        try:
-            if slugger.is_slug(model_id_or_slug):
-                self.slug = model_id_or_slug
-                self.model_id = slugger.encode(self.slug)
-            else:
-                self.model_id = model_id_or_slug
-                self.slug = slugger.decode(self.model_id)
-            if not self.is_valid():
-                raise InvalidModelIdentifierError(model=self.text)
-        except InvalidModelIdentifierError as err:
-            self.logger.error("Invalid model identifier!")
-            print(err)
-            sys.exit()
-        finally:
-            pass
-
-    def is_valid(self):
-        if self.model_id is None or self.slug is None:
-            return False
+    def current_service_class(self):
+        data = self.get()
+        if data is None:
+            return None
         else:
-            return True
+            return data["service_class"]
 
-    def is_available_locally(self):
-        fetch_status_file = os.path.join(self._dest_dir, self.model_id, STATUS_FILE)
-        if not os.path.exists(fetch_status_file):
-            self.logger.debug("No status file exists")
-            is_fetched = False
+    def register_service_class(self, service_class):
+        data = self.get()
+        data["service_class"] = service_class
+        with open(self.session_file, "w") as f:
+            json.dump(data, f, indent=4)
+
+    def open(self, model_id):
+        self.logger.debug("Opening session {0}".format(self.session_file))
+        session = {
+            "model_id": model_id,
+            "timestamp": str(time.time()),
+            "identifier": str(uuid.uuid4()),
+        }
+        with open(self.session_file, "w") as f:
+            json.dump(session, f, indent=4)
+
+    def get(self):
+        if os.path.isfile(self.session_file):
+            self.logger.debug("Getting session from {0}".format(self.session_file))
+            with open(self.session_file, "r") as f:
+                session = json.load(f)
+            return session
         else:
-            with open(fetch_status_file, "r") as f:
-                status = json.load(f)
-            is_fetched = status[DONE_TAG]
-        self.logger.debug("Is fetched: {0}".format(is_fetched))
-        return is_fetched
+            self.logger.debug("No session exists")
+            return None
+
+    def close(self):
+        self.logger.debug("Closing session {0}".format(self.session_file))
+        if os.path.isfile(self.session_file):
+            os.remove(self.session_file)
```

### Comparing `ersilia-0.1.1/ersilia/db/disk/fetched.py` & `ersilia-0.1.8/ersilia/db/disk/fetched.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/db/environments/localdb.py` & `ersilia-0.1.8/ersilia/db/environments/localdb.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/db/environments/managers.py` & `ersilia-0.1.8/ersilia/db/environments/managers.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,35 +10,39 @@
 from ...utils.docker import SimpleDocker, is_inside_docker
 from ...utils.identifiers.short import ShortIdentifier
 from ...utils.ports import find_free_port
 from .localdb import EnvironmentDb
 
 from ...default import DOCKERHUB_ORG, DOCKERHUB_LATEST_TAG, DEFAULT_DOCKER_PLATFORM
 
+
 BENTOML_DOCKERPORT = 5000
+INTERNAL_DOCKERPORT = 80
 
 
 class DockerManager(ErsiliaBase):
-    def __init__(self, config_json=None):
+    def __init__(self, config_json=None, preferred_port=None, with_bentoml=False):
         ErsiliaBase.__init__(self, config_json=config_json)
         self._eos_regex = Paths()._eos_regex()
         self._org_regex = re.compile(DOCKERHUB_ORG)
         self.inside_docker = is_inside_docker()
         self.docker = SimpleDocker()
         self.db = EnvironmentDb()
         self.db.table = "docker"
+        self.preferred_port = preferred_port
+        self.with_bentoml = with_bentoml
 
     def is_inside_docker(self):
         return self.inside_docker
 
     def is_installed(self):
         return DockerRequirement().is_installed()
 
     def image_exists(self, model_id):
-        if self._images_of_model(model_id, only_latest=True):
+        if self.images_of_model(model_id, only_latest=True):
             return True
         else:
             return False
 
     def container_exists(self, container_name):
         names = set(self.containers(only_run=False).keys())
         if container_name in names:
@@ -81,15 +85,15 @@
             valid_images.update([k])
         cnt_dict = {}
         for k, v in self.containers(only_run=only_run).items():
             if v in valid_images:
                 cnt_dict[k] = v
         return cnt_dict
 
-    def build(self, model_id, use_cache=True):
+    def build_with_bentoml(self, model_id, use_cache=True):
         bundle_path = self._get_bundle_location(model_id)
         tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
         tmp_file = os.path.join(tmp_folder, "build.sh")
         cmdlines = ["cd {0}".format(bundle_path)]
         if use_cache:
             cache_str = ""
         else:
@@ -106,14 +110,64 @@
         cmd = "bash {0}".format(tmp_file)
         run_command(cmd)
         self.db.insert(
             model_id=model_id,
             env="{0}/{1}:{2}".format(DOCKERHUB_ORG, model_id, DOCKERHUB_LATEST_TAG),
         )
 
+    @property
+    def _model_deploy_dockerfiles_url(self):
+        return "https://raw.githubusercontent.com/ersilia-os/ersilia/master/dockerfiles/model-deploy"
+
+    def _build_ersilia_base(self):
+        self.logger.debug("Creating docker image of ersilia base")
+        path = tempfile.mkdtemp(prefix="ersilia-")
+        base_folder = os.path.join(path, "base")
+        os.mkdir(base_folder)
+        base_files = ["Dockerfile", "docker-entrypoint.sh", "nginx.conf"]
+        for f in base_files:
+            cmd = "cd {0}; wget {2}/base/{1}".format(
+                base_folder, f, self._model_deploy_dockerfiles_url
+            )
+            run_command(cmd)
+        cmd = "cd {0}; docker build -t {1}/base:{2} .".format(
+            base_folder, DOCKERHUB_ORG, DOCKERHUB_LATEST_TAG
+        )
+        run_command(cmd)
+
+    def build_with_ersilia(self, model_id):
+        self.logger.debug("Creating docker image with ersilia incorporated")
+        if self.image_exists("base"):
+            pass
+        else:
+            self._build_ersilia_base()
+        path = tempfile.mkdtemp(prefix="ersilia-model")
+        model_folder = os.path.join(path, model_id)
+        os.mkdir(model_folder)
+        cmd = "cd {0}; wget {1}/model/Dockerfile".format(
+            model_folder, self._model_deploy_dockerfiles_url
+        )
+        run_command(cmd)
+        file_path = os.path.join(model_folder, "Dockerfile")
+        with open(file_path, "r") as f:
+            text = f.read()
+        text = text.replace("eos_identifier", model_id)
+        with open(file_path, "w") as f:
+            f.write(text)
+        cmd = "cd {0}; docker build -t {1}/{2}:{3} .".format(
+            model_folder, DOCKERHUB_ORG, model_id, DOCKERHUB_LATEST_TAG
+        )
+        run_command(cmd)
+
+    def build(self, model_id, use_cache=True):
+        if self.with_bentoml:
+            self.build_with_bentoml(model_id=model_id, use_cache=use_cache)
+        else:
+            self.build_with_ersilia(model_id=model_id)
+
     def remove(self, model_id):
         self.docker.delete(org=DOCKERHUB_ORG, img=model_id, tag=DOCKERHUB_LATEST_TAG)
         self.db.delete(
             model_id=model_id,
             env="{0}/{1}:{2}".format(DOCKERHUB_ORG, model_id, DOCKERHUB_LATEST_TAG),
         )
 
@@ -122,29 +176,27 @@
         imgs = self.images_of_model(model_id, only_latest=True)
         self.logger.debug("Available images: {0}".format(imgs))
         img = [k for k in imgs.keys()][0]
         if enable_microbatch:
             mb_string = "--enable-microbatch"
         else:
             mb_string = ""
-        port = find_free_port()
+        port = find_free_port(preferred_port=self.preferred_port)
         name = None
         si = ShortIdentifier()
         while not name:
             name_ = "{0}_{1}".format(model_id, si.encode())
             if not self.container_exists(name_):
                 name = name_
+        if self.with_bentoml:
+            dockerport = BENTOML_DOCKERPORT
+        else:
+            dockerport = INTERNAL_DOCKERPORT
         cmd = "docker run --platform {6} --name {0} -d -p {1}:{2} {3} --workers={4} {5}".format(
-            name,
-            port,
-            BENTOML_DOCKERPORT,
-            img,
-            workers,
-            mb_string,
-            DEFAULT_DOCKER_PLATFORM,
+            name, port, dockerport, img, workers, mb_string, DEFAULT_DOCKER_PLATFORM
         )
         self.logger.debug(cmd)
         run_command(cmd)
         return {"container_name": name, "port": port}
 
     def start(self, container_name):
         cmd = "docker start {0}".format(container_name)
```

### Comparing `ersilia-0.1.1/ersilia/db/hubdata/localslugs.py` & `ersilia-0.1.8/ersilia/db/hubdata/localslugs.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/default.py` & `ersilia-0.1.8/ersilia/default.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,33 +9,40 @@
 ROOT = os.path.dirname(os.path.realpath(__file__))
 BENTOML_PATH = os.path.join(str(Path.home()), "bentoml")
 CHECKSUM_NCHAR = 8
 CONDA_ENV_YML_FILE = "environment.yml"
 DOCKERFILE_FILE = "Dockerfile"
 GITHUB_ORG = "ersilia-os"
 GITHUB_ERSILIA_REPO = "ersilia"
+ERSILIA_MODELS_S3_BUCKET = "ersilia-models"
 CONFIG_JSON = "config.json"
 CREDENTIALS_JSON = "credentials.json"
 INSTALL_STATUS_FILE = ".install.status"
 DOCKER_BENTO_PATH = "/bento"
 DOCKERHUB_ORG = "ersiliaos"
 DOCKERHUB_LATEST_TAG = "latest"
 DEFAULT_DOCKER_PLATFORM = "linux/amd64"
 DEFAULT_MODEL_ID = "eos0zzz"
 DEFAULT_VENV = "env"
 PACKMODE_FILE = "pack_mode.txt"
 LOGGING_FILE = "console.log"
+CURRENT_LOGGING_FILE = "current.log"
 CARD_FILE = "card.json"
 SILENCE_FILE = ".silence.json"
 VERBOSE_FILE = ".verbose.json"
 API_SCHEMA_FILE = "api_schema.json"
 MODEL_SIZE_FILE = "size.json"
 DEFAULT_BATCH_SIZE = 100
 FETCHED_MODELS_FILENAME = "fetched_models.txt"
 MODEL_CONFIG_FILENAME = "config.json"
+DEFAULT_ERSILIA_ERROR_EXIT_CODE = 1
+METADATA_JSON_FILE = "metadata.json"
+SERVICE_CLASS_FILE = "service_class.txt"
+APIS_LIST_FILE = "apis_list.txt"
+INFORMATION_FILE = "information.json"
 
 # Isaura data lake
 H5_EXTENSION = ".h5"
 H5_DATA_FILE = "data.h5"
 ISAURA_FILE_TAG = "_public"
 ISAURA_FILE_TAG_LOCAL = "_local"
 ISAURA_GDRIVE = "1LSCMHrCuXUDNH3WRbrLMW2FoiwMCxF2n"
@@ -49,14 +56,16 @@
 AIRTABLE_READONLY_API_KEY = "keyVMAlJFOvu7vgMR"
 AIRTABLE_MODEL_HUB_BASE_ID = "appgxpCzCDNyGjWc8"
 AIRTABLE_MODEL_HUB_TABLE_NAME = "Models"
 
 # URLS
 ERSILIA_WEB_URL = "https://ersilia.io"
 ERSILIA_MODEL_HUB_URL = "https://ersilia.io/model-hub"
+AIRTABLE_MODEL_HUB_VIEW_URL = "https://airtable.com/shrNc3sTtTA3QeEZu"
+S3_BUCKET_URL = "https://ersilia-models.s3.eu-central-1.amazonaws.com"
 
 # EOS conda
 _resolve_script = "conda_env_resolve.py"
 resolve_script = os.path.join(EOS, _resolve_script)
 if not os.path.exists(resolve_script):
     shutil.copyfile(
         os.path.join(ROOT, "utils", "supp", _resolve_script), resolve_script
@@ -116,14 +125,16 @@
 
     Motivation behind this function is to define an ersilia CLI.
 
     Args:
         - overwrite (bool): Overwrite the current bash profile file if the eosconda string is found.
     """
     fn = bashrc_path()
+    if fn is None:
+        return
     with open(fn, "r") as f:
         text = f.read()
     if snippet in text:
         if overwrite:
             text = text.split(snippet)[0] + text.split(snippet)[1]
         else:
             return
```

### Comparing `ersilia-0.1.1/ersilia/hub/bundle/bundle.py` & `ersilia-0.1.8/ersilia/hub/bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/hub/bundle/repo.py` & `ersilia-0.1.8/ersilia/hub/bundle/repo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 import json
 from re import I
 from ... import ErsiliaBase
+from ... import logger
 from ...utils.paths import Paths
 from ...utils.docker import SimpleDockerfileParser
 from ...utils.conda import SimpleConda
+from ...utils.system import SystemChecker
 from ...default import (
     CONDA_ENV_YML_FILE,
     DOCKER_BENTO_PATH,
     DEFAULT_MODEL_ID,
     DOCKERFILE_FILE,
 )
 
@@ -63,14 +65,31 @@
         if add_text in text:
             return
         text += os.linesep
         text += add_text
         with open(file_name, "w") as f:
             f.write(text)
 
+    def add_info_api(self, information_file):
+        """Adds and info api to the service"""
+        file_name = self.get_file()
+        with open(file_name, "r") as f:
+            text = f.read()
+        splitter_string = "Service.__name__"
+        text = text.split(splitter_string)
+        a = text[0]
+        b = text[1]
+        a += "    @api(input=JsonInput(), batch=True)\n"
+        a += "    def info(self, input=None):\n"
+        a += "        data = json.load(open('{0}', 'r'))\n".format(information_file)
+        a += "        return [data]\n\n"
+        with open(file_name, "w") as f:
+            s = a + splitter_string + b
+            f.write(s)
+
     def check(self):
         """checks if the service.py contains the Service Class"""
         return self._has_service_class()
 
 
 class PackFile(object):
     def __init__(self, path):
@@ -149,14 +168,31 @@
             if len(tag) != 3:
                 return None
         else:
             tag = tag.split("-")
             if len(tag) != 2:
                 return None
         result = {"version": tag[0], "slim": slim, "python": tag[-1]}
+        if result["python"] in [
+            "py30",
+            "py31",
+            "py32",
+            "py33",
+            "py34",
+            "py35",
+            "py36",
+            "py37",
+            "py38",
+            "py39",
+        ]:
+            if SystemChecker().is_arm64():
+                logger.warning(
+                    "This model is trying to install to a python version in ARM64 that is below 3.10. Changing to 3.10."
+                )
+                result["python"] = "py310"
         return result
 
     def has_runs(self):
         if self.parser.get_runs():
             return True
         else:
             return False
@@ -177,16 +213,18 @@
         return runs
 
     def get_install_commands(self):
         fn = self.get_file()
         if fn is None:
             return None
         needs_conda = self.needs_conda()
-        runs = self.conda.get_conda_and_pip_install_commands_from_dockerfile_if_exclusive(
-            fn
+        runs = (
+            self.conda.get_conda_and_pip_install_commands_from_dockerfile_if_exclusive(
+                fn
+            )
         )
         if runs:
             exclusive_conda_and_pip = True
         else:
             exclusive_conda_and_pip = False
             runs = self.get_install_commands_from_dockerfile(fn)
         result = {
```

### Comparing `ersilia-0.1.1/ersilia/hub/bundle/status.py` & `ersilia-0.1.8/ersilia/hub/bundle/status.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/hub/content/card.py` & `ersilia-0.1.8/ersilia/hub/content/catalog.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,196 +1,179 @@
-import os
-import json
-import tempfile
+"""See available models in the Ersilia Model Hub"""
+
+import subprocess
 import requests
-from pyairtable import Table
+import os
+from .card import ModelCard
 from ... import ErsiliaBase
-from ...utils.terminal import run_command
+from ...utils.identifiers.model import ModelIdentifier
 from ...auth.auth import Auth
+from ...default import GITHUB_ORG
+from ... import logger
 
 try:
-    from isaura.core.hdf5 import Hdf5Explorer
-except:
-    Hdf5Explorer = None
-
-from ...default import (
-    AIRTABLE_MODEL_HUB_BASE_ID,
-    AIRTABLE_MODEL_HUB_TABLE_NAME,
-    ISAURA_DIR,
-    ISAURA_FILE_TAG,
-    ISAURA_FILE_TAG_LOCAL,
-    H5_EXTENSION,
-    CARD_FILE,
-)
+    import webbrowser
+except ModuleNotFoundError as err:
+    webbrowser = None
 
-AIRTABLE_MAX_ROWS = 100000
-AIRTABLE_PAGE_SIZE = 100
+try:
+    from github import Github
+except ModuleNotFoundError as err:
+    Github = None
 
+try:
+    from tabulate import tabulate
+except ModuleNotFoundError as err:
+    tabulate = None
 
-class ReadmeCard(ErsiliaBase):
-    def __init__(self, config_json):
-        ErsiliaBase.__init__(self, config_json=config_json)
 
-    def _raw_readme_url(self, model_id):
-        url = "https://raw.githubusercontent.com/ersilia-os/{0}/master/README.md".format(
-            model_id
-        )
-        return url
+class CatalogTable(object):
+    def __init__(self, data, columns):
+        self.data = data
+        self.columns = columns
 
-    def _gh_view(self, model_id):
-        tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
-        tmp_file = os.path.join(tmp_folder, "view.md")
-        cmd = "gh repo view {0}/{1} > {2}".format("ersilia-os", model_id, tmp_file)
-        run_command(cmd)
-        with open(tmp_file, "r") as f:
-            text = f.read()
-        return text
-
-    def _title(self, lines):
-        """Title is determined by the first main header in markdown"""
-        for l in lines:
-            if l[:2] == "# ":
-                s = l[2:].strip()
-                return s
-
-    def _description(self, lines):
-        """Description is what comes after the title and before the next header"""
-        text = "\n".join(lines)
-        return text.split("# ")[1].split("\n")[1].split("#")[0].strip()
-
-    def _mode(self, lines):
-        text = "\n".join(lines)
-        return text.split("# ")[1].split("\n")[1].split("#")[0].strip()
-
-    def _model_github_url(self, model_id):
-        return "https://github.com/ersilia-os/{0}".format(model_id)
-
-    def parse(self, model_id):
-        readme = os.path.join(self._dest_dir, model_id, "README.md")
-        if os.path.exists(readme):
-            with open(readme, "r") as f:
-                text = f.read()
+    def as_table(self):
+        if not tabulate:
+            return None
         else:
-            if Auth().is_contributor():
-                text = self._gh_view(model_id)
-                if not text:
-                    return None
-                text = "--".join(text.split("--")[1:])
-            else:
-                r = requests.get(self._raw_readme_url(model_id))
-                if r.status_code != 200:
-                    return None
-                text = r.text
-        lines = text.split(os.linesep)
-        title = self._title(lines)
-        descr = self._description(lines)
-        results = {
-            "model_id": model_id,
-            "title": self._title(lines),
-            "description": self._description(lines),
-            "mode": self._mode(lines),
-            "github_url": self._model_github_url(model_id),
-        }
-        return results
+            return tabulate(
+                self.data,
+                headers=self.columns,
+                tablefmt="fancy_grid",
+                colalign=("center", "center", "center"),
+            )
+
+    def __str__(self):
+        return self.as_table()
 
-    def get(self, model_id):
-        return self.parse(model_id)
+    def __repr__(self):
+        return self.__str__()
 
 
-class AirtableCard(ErsiliaBase):
-    def __init__(self, config_json):
+class ModelCatalog(ErsiliaBase):
+    def __init__(self, tabular_view=True, config_json=None):
         ErsiliaBase.__init__(self, config_json=config_json)
-        self.api_key = self._get_read_only_airtable_api_key()
-        self.base_id = AIRTABLE_MODEL_HUB_BASE_ID
-        self.table_name = AIRTABLE_MODEL_HUB_TABLE_NAME
-        self.max_rows = AIRTABLE_MAX_ROWS
-        self.page_size = AIRTABLE_PAGE_SIZE
-        self.table = Table(self.api_key, self.base_id, self.table_name)
-
-    @staticmethod
-    def _get_read_only_airtable_api_key():
-        url = "https://raw.githubusercontent.com/ersilia-os/ersilia/master/config/read_only_keys.json"
-        r = requests.get(url)
-        data = r.json()
-        return data["AIRTABLE_READONLY_API_KEY"]
-
-    def _find_card(self, text, field):
-        card = None
-        for records in self.table.iterate(
-            page_size=self.page_size, max_records=self.max_rows
-        ):
-            for record in records:
-                fields = record["fields"]
-                if field not in fields:
-                    continue
-                if text == record["fields"][field]:
-                    card = record["fields"]
-        return card
-
-    def find_card_by_model_id(self, model_id):
-        return self._find_card(model_id, "Identifier")
-
-    def find_card_by_slug(self, slug):
-        return self._find_card(slug, "Slug")
-
-    def find_card_by_mode(self, mode):
-        return self._find_card(mode, "Mode")
-
-    def get(self, model_id):
-        return self.find_card_by_model_id(model_id)
-
+        self.mi = ModelIdentifier()
+        self.tabular_view = tabular_view
 
-class LocalCard(ErsiliaBase):
-    def __init__(self, config_json):
-        ErsiliaBase.__init__(self, config_json=config_json)
+    def _is_eos(self, s):
+        if self.mi.is_valid(s):
+            if not self.mi.is_test(s):
+                return True
+        return False
+
+    def _get_title(self, card):
+        if "title" in card:
+            return card["title"]
+        if "Title" in card:
+            return card["Title"]
+        return None
+
+    def _get_slug(self, card):
+        if "slug" in card:
+            return card["slug"]
+        if "Slug" in card:
+            return card["Slug"]
+        return None
+
+    def _get_mode(self, card):
+        if "mode" in card:
+            return card["mode"]
+        if "Mode" in card:
+            return card["Mode"]
+
+    def airtable(self):
+        """List models available in AirTable Ersilia Model Hub base"""
+        if webbrowser:  # TODO: explore models online
+            if not self.tabular_view:
+                webbrowser.open(
+                    "https://airtable.com/shr9sYjL70nnHOUrP/tblZGe2a2XeBxrEHP"
+                )
+            else:
+                webbrowser.open("https://airtable.com/shrUcrUnd7jB9ChZV")
 
-    def get(self, model_id):
-        model_path = self._model_path(model_id)
-        card_path = os.path.join(model_path, CARD_FILE)
-        if os.path.exists(card_path):
-            with open(card_path, "r") as f:
-                card = json.load(f)
-            return card
+    def github(self):
+        """List models available in the GitHub model hub repository"""
+        if Github is None:
+            token = None
         else:
-            return None
-
-
-class LakeCard(ErsiliaBase):
-    def __init__(self, config_json=None):
-        ErsiliaBase.__init__(self, config_json=config_json)
-
-    def get(self, model_id, as_json=False):
-        if Hdf5Explorer is None:
-            self.logger.debug("No lake found")
-            return None
-        card = Hdf5Explorer(model_id=model_id).info()
-        if as_json:
-            return json.dumps(card, indent=4)
+            token = Auth().oauth_token()
+        logger.debug(
+            "Looking for model repositories in {0} organization".format(GITHUB_ORG)
+        )
+        if token:
+            g = Github(token)
+            repo_list = [i for i in g.get_user().get_repos()]
+            repos = []
+            for r in repo_list:
+                owner, name = r.full_name.split("/")
+                if owner != GITHUB_ORG:
+                    continue
+                repos += [name]
         else:
-            return card
-
+            repos = []
+            url = "https://api.github.com/users/{0}/repos".format(GITHUB_ORG)
+            results = requests.get(url).json()
+            for r in results:
+                repos += [r["name"]]
+        models = []
+        for repo in repos:
+            if self._is_eos(repo):
+                models += [repo]
+        logger.info("Found {0} models".format(len(models)))
+        return models
+
+    def hub(self):
+        """List models available in Ersilia model hub repository"""
+        mc = ModelCard()
+        models = self.github()
+        R = []
+        for model_id in models:
+            card = mc.get(model_id)
+            if card is None:
+                continue
+            slug = self._get_slug(card)
+            title = self._get_title(card)
+            mode = self._get_mode(card)
+            R += [[model_id, slug, title, mode]]
+        return CatalogTable(R, columns=["MODEL_ID", "SLUG", "TITLE", "MODE"])
+
+    def local(self):
+        """List models available locally"""
+        mc = ModelCard()
+        R = []
+        logger.debug("Looking for models in {0}".format(self._bundles_dir))
+        for model_id in os.listdir(self._bundles_dir):
+            if not self._is_eos(model_id):
+                continue
+            card = mc.get(model_id)
+            slug = self._get_slug(card)
+            title = self._get_title(card)
+            mode = self._get_mode(card)
+            R += [[model_id, slug, title, mode]]
+        logger.info("Found {0} models".format(len(R)))
+        if len(R) == 0:
+            return None
+        return CatalogTable(data=R, columns=["MODEL_ID", "SLUG", "TITLE", "MODE"])
 
-class ModelCard(object):
-    def __init__(self, config_json=None):
-        self.lc = LocalCard(config_json=config_json)
-        self.ac = AirtableCard(config_json=config_json)
-        self.rc = ReadmeCard(config_json=config_json)
-
-    def _get(self, model_id):
-        card = self.lc.get(model_id)
-        if card is not None:
-            return card
-        card = self.ac.get(model_id)
-        if card is not None:
-            return card
-        card = self.rc.get(model_id)
-        if card is not None:
-            return card
-
-    def get(self, model_id, as_json=False):
-        card = self._get(model_id)
-        if card is None:
+    def bentoml(self):
+        """List models available as BentoServices"""
+        result = subprocess.run(
+            ["bentoml", "list"], stdout=subprocess.PIPE, env=os.environ
+        )
+        result = [r for r in result.stdout.decode("utf-8").split("\n") if r]
+        if len(result) == 1:
             return
-        if as_json:
-            return json.dumps(card, indent=4)
-        else:
-            return card
+        columns = ["BENTO_SERVICE", "AGE", "APIS", "ARTIFACTS"]
+        header = result[0]
+        values = result[1:]
+        cut_idxs = []
+        for col in columns:
+            cut_idxs += [header.find(col)]
+        R = []
+        for row in values:
+            r = []
+            for i, idx in enumerate(zip(cut_idxs, cut_idxs[1:] + [None])):
+                r += [row[idx[0] : idx[1]].rstrip()]
+            R += [[r[0].split(":")[0]] + r]
+        columns = ["MODEL_ID"] + columns
+        return CatalogTable(data=R, columns=columns)
```

### Comparing `ersilia-0.1.1/ersilia/hub/content/catalog.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/get.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,139 @@
-"""See available models in the Ersilia Model Hub"""
-
-import subprocess
-import requests
 import os
-from .card import ModelCard
-from ... import ErsiliaBase
-from ...utils.identifiers.model import ModelIdentifier
-from ...auth.auth import Auth
-from ...default import GITHUB_ORG
-from ... import logger
-
-try:
-    import webbrowser
-except ModuleNotFoundError as err:
-    webbrowser = None
-
-try:
-    from github import Github
-except ModuleNotFoundError as err:
-    Github = None
-
-try:
-    from tabulate import tabulate
-except ModuleNotFoundError as err:
-    tabulate = None
-
-
-class CatalogTable(object):
-    def __init__(self, data, columns):
-        self.data = data
-        self.columns = columns
+import shutil
+from . import BaseAction
+from ....utils.download import GitHubDownloader
+from ....utils.paths import Paths
+from ...bundle.repo import PackFile, DockerfileFile
+from ....utils.exceptions_utils.throw_ersilia_exception import throw_ersilia_exception
+from ....utils.exceptions_utils.fetch_exceptions import FolderNotFoundError
+
+MODEL_DIR = "model"
 
-    def as_table(self):
-        if not tabulate:
-            return None
+
+class ModelRepositoryGetter(BaseAction):
+    def __init__(self, model_id, config_json):
+        BaseAction.__init__(
+            self, model_id=model_id, config_json=config_json, credentials_json=None
+        )
+        self.token = self.cfg.HUB.TOKEN
+        self.github_down = GitHubDownloader(self.token)
+        self.org = self.cfg.HUB.ORG
+
+    def _dev_model_path(self):
+        pt = Paths()
+        path = pt.models_development_path()
+        if path is not None:
+            path = os.path.join(path, self.model_id)
+        if pt.exists(path):
+            return path
         else:
-            return tabulate(
-                self.data,
-                headers=self.columns,
-                tablefmt="fancy_grid",
-                colalign=("center", "center", "center"),
-            )
+            path = pt.ersilia_development_path()
+            if path is not None:
+                path = os.path.join(path, "test", "models", self.model_id)
+            if pt.exists(path):
+                return path
+        return None
 
-    def __str__(self):
-        return self.as_table()
+    @staticmethod
+    def _copy_from_local(src, dst):
+        shutil.copytree(src, dst)
+
+    def _copy_from_github(self, dst):
+        self.github_down.clone(org=self.org, repo=self.model_id, destination=dst)
+
+    def _change_py_version_in_dockerfile_if_necessary(self):
+        path = self._model_path(model_id=self.model_id)
+        df = DockerfileFile(path=path)
+        version = df.get_bentoml_version()
+        self.logger.debug(version)
+        dockerfile_path = os.path.join(path, "Dockerfile")
+        with open(dockerfile_path, "r") as f:
+            R = f.readlines()
+        S = []
+        for r in R:
+            if r.startswith("FROM "):
+                r = r.split("-")
+                if r[-1].startswith("py"):
+                    p = version["python"]
+                    r = "-".join(r[:-1] + [p])
+                else:
+                    r = "-".join(r)
+            S += [r]
+        with open(dockerfile_path, "w") as f:
+            for s in S:
+                f.write(s + os.linesep)
+
+    def get(self):
+        """Copy model repository from local or download from GitHub"""
+        folder = self._model_path(self.model_id)
+        dev_model_path = self._dev_model_path()
+        if dev_model_path is not None:
+            self.logger.debug(
+                "Copying from local {0} to {1}".format(dev_model_path, folder)
+            )
+            self._copy_from_local(dev_model_path, folder)
+        else:
+            self.logger.debug("Cloning from github to {0}".format(folder))
+            self._copy_from_github(folder)
+        self._change_py_version_in_dockerfile_if_necessary()
 
-    def __repr__(self):
-        return self.__str__()
 
+#  TODO: work outside GIT LFS
+class ModelParametersGetter(BaseAction):
+    def __init__(self, model_id, config_json):
+        BaseAction.__init__(
+            self, model_id=model_id, config_json=config_json, credentials_json=None
+        )
 
-class ModelCatalog(ErsiliaBase):
-    def __init__(self, tabular_view=True, config_json=None):
-        ErsiliaBase.__init__(self, config_json=config_json)
-        self.mi = ModelIdentifier()
-        self.tabular_view = tabular_view
-
-    def _is_eos(self, s):
-        if self.mi.is_valid(s):
-            if not self.mi.is_test(s):
-                return True
-        return False
-
-    def _get_title(self, card):
-        if "title" in card:
-            return card["title"]
-        if "Title" in card:
-            return card["Title"]
-        return None
+    @staticmethod
+    def _requires_parameters(model_path):
+        pf = PackFile(model_path)
+        return pf.needs_model()
+
+    def _get_destination(self):
+        model_path = self._model_path(self.model_id)
+        return os.path.join(model_path, MODEL_DIR)
+
+    @throw_ersilia_exception
+    def get(self):
+        """Create a ./model folder in the model repository"""
+        model_path = self._model_path(self.model_id)
+        folder = self._get_destination()
+        if not os.path.exists(folder):
+            os.mkdir(folder)
+        if not self._requires_parameters(model_path):
+            return None
+        if not os.path.exists(folder):
+            raise FolderNotFoundError(folder)
 
-    def _get_slug(self, card):
-        if "slug" in card:
-            return card["slug"]
-        if "Slug" in card:
-            return card["Slug"]
-        return None
 
-    def _get_mode(self, card):
-        if "mode" in card:
-            return card["mode"]
-        if "Mode" in card:
-            return card["Mode"]
-
-    def airtable(self):
-        """List models available in AirTable Ersilia Model Hub base"""
-        if webbrowser:  # TODO: explore models online
-            if not self.tabular_view:
-                webbrowser.open(
-                    "https://airtable.com/shr9sYjL70nnHOUrP/tblZGe2a2XeBxrEHP"
-                )
-            else:
-                webbrowser.open("https://airtable.com/shrUcrUnd7jB9ChZV")
-
-    def github(self):
-        """List models available in the GitHub model hub repository"""
-        if Github is None:
-            token = None
-        else:
-            token = Auth().oauth_token()
-        logger.debug(
-            "Looking for model repositories in {0} organization".format(GITHUB_ORG)
+class ModelGetter(BaseAction):
+    def __init__(self, model_id, repo_path, config_json):
+        BaseAction.__init__(
+            self, model_id=model_id, config_json=config_json, credentials_json=None
         )
-        if token:
-            g = Github(token)
-            repo_list = [i for i in g.get_user().get_repos()]
-            repos = []
-            for r in repo_list:
-                owner, name = r.full_name.split("/")
-                if owner != GITHUB_ORG:
-                    continue
-                repos += [name]
+        self.model_id = model_id
+        self.repo_path = repo_path
+        self.mrg = ModelRepositoryGetter(model_id=model_id, config_json=config_json)
+        self.mpg = ModelParametersGetter(model_id=model_id, config_json=config_json)
+
+    def _get_repository(self):
+        self.mrg.get()
+
+    def _get_model_parameters(self):
+        self.mpg.get()
+
+    def _copy_from_repo_path(self):
+        dst = self._model_path(self.model_id)
+        src = self.repo_path
+        shutil.copytree(src, dst)
+
+    @throw_ersilia_exception
+    def get(self):
+        if self.repo_path is None:
+            self._get_repository()
+            self._get_model_parameters()
         else:
-            repos = []
-            url = "https://api.github.com/users/{0}/repos".format(GITHUB_ORG)
-            results = requests.get(url).json()
-            for r in results:
-                repos += [r["name"]]
-        models = []
-        for repo in repos:
-            if self._is_eos(repo):
-                models += [repo]
-        logger.info("Found {0} models".format(len(models)))
-        return models
-
-    def hub(self):
-        """List models available in Ersilia model hub repository"""
-        mc = ModelCard()
-        models = self.github()
-        R = []
-        for model_id in models:
-            card = mc.get(model_id)
-            if card is None:
-                continue
-            slug = self._get_slug(card)
-            title = self._get_title(card)
-            mode = self._get_mode(card)
-            R += [[model_id, slug, title, mode]]
-        return CatalogTable(R, columns=["MODEL_ID", "SLUG", "TITLE", "MODE"])
-
-    def local(self):
-        """List models available locally"""
-        mc = ModelCard()
-        mi = ModelIdentifier()
-        R = []
-        logger.debug("Looking for models in {0}".format(self._bundles_dir))
-        for model_id in os.listdir(self._bundles_dir):
-            if not self._is_eos(model_id):
-                continue
-            card = mc.get(model_id)
-            slug = self._get_slug(card)
-            title = self._get_title(card)
-            mode = self._get_mode(card)
-            R += [[model_id, slug, title, mode]]
-        logger.info("Found {0} models".format(len(R)))
-        return CatalogTable(data=R, columns=["MODEL_ID", "SLUG", "TITLE", "MODE"])
-
-    def bentoml(self):
-        """List models available as BentoServices"""
-        result = subprocess.run(
-            ["bentoml", "list"], stdout=subprocess.PIPE, env=os.environ
-        )
-        result = [r for r in result.stdout.decode("utf-8").split("\n") if r]
-        if len(result) == 1:
-            return
-        columns = ["BENTO_SERVICE", "AGE", "APIS", "ARTIFACTS"]
-        header = result[0]
-        values = result[1:]
-        cut_idxs = []
-        for col in columns:
-            cut_idxs += [header.find(col)]
-        R = []
-        for row in values:
-            r = []
-            for i, idx in enumerate(zip(cut_idxs, cut_idxs[1:] + [None])):
-                r += [row[idx[0] : idx[1]].rstrip()]
-            R += [[r[0].split(":")[0]] + r]
-        columns = ["MODEL_ID"] + columns
-        return CatalogTable(data=R, columns=columns)
+            self._copy_from_repo_path()
+        if not os.path.exists(self._model_path(self.model_id)):
+            raise FolderNotFoundError(os.path.exists(self._model_path(self.model_id)))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ersilia-0.1.1/ersilia/hub/content/search.py` & `ersilia-0.1.8/ersilia/hub/content/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,15 @@
                 distance[i][0] = i
                 distance[0][k] = k
 
         # Iterate over the matrix to compute the cost of deletions,insertions and/or substitutions
         for col in range(1, cols):
             for row in range(1, rows):
                 if s[row - 1] == t[col - 1]:
-                    cost = (
-                        0
-                    )  # If the characters are the same in the two strings in a given position [i,j] then the cost is 0
+                    cost = 0  # If the characters are the same in the two strings in a given position [i,j] then the cost is 0
                 else:
                     cost = 2
 
                 distance[row][col] = min(
                     distance[row - 1][col] + 1,  # Cost of deletions
                     distance[row][col - 1] + 1,  # Cost of insertions
                     distance[row - 1][col - 1] + cost,
```

### Comparing `ersilia-0.1.1/ersilia/hub/content/slug.py` & `ersilia-0.1.8/ersilia/hub/content/slug.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/hub/content/table_update.py` & `ersilia-0.1.8/ersilia/hub/content/table_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         R = data[table_no * page_size : table_no * page_size + page_size]
         # sets counter to next table i.e. table 1
         with open(counter_path, "w") as count_in:
             count_in.write(str(1))
         return CatalogTable(data=R, columns=self.catalog.columns)
 
     def next_table(self):
-
         table_no = counter
         data = self.catalog.data
         page_size = self.page_size
         R = data[table_no * page_size : table_no * page_size + page_size]
         if table_no * page_size + page_size > len(data) < len(data) / page_size:
             print("Last Table! ersilia catalog --previous to go back")
         with open(counter_path, "w") as count_out:
```

### Comparing `ersilia-0.1.1/ersilia/hub/delete/delete.py` & `ersilia-0.1.8/ersilia/hub/delete/delete.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,15 +220,16 @@
 
     def delete(self):
         os.rmdir(self._tmp_dir)
         os.makedirs(self._tmp_dir)
 
 
 class ModelFullDeleter(ErsiliaBase):
-    def __init__(self, config_json=None):
+    def __init__(self, config_json=None, overwrite=True):
+        self.overwrite = overwrite
         ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
 
     def needs_delete(self, model_id):
         ms = ModelStatus().status(model_id)
         for k, v in ms.items():
             if v:
                 return True
@@ -236,14 +237,15 @@
 
     def delete(self, model_id):
         self.logger.info("Starting delete of model {0}".format(model_id))
         ModelEosDeleter(self.config_json).delete(model_id)
         ModelSlugDeleter(self.config_json).delete(model_id)
         ModelBundleDeleter(self.config_json).delete(model_id)
         ModelBentoDeleter(self.config_json).delete(model_id)
-        ModelCondaDeleter(self.config_json).delete(model_id)
+        if self.overwrite:
+            ModelCondaDeleter(self.config_json).delete(model_id)
         ModelTmpDeleter(self.config_json).delete(model_id)
         ModelLakeDeleter(self.config_json).delete(model_id)
         ModelPipDeleter(self.config_json).delete(model_id)
         ModelDockerDeleter(self.config_json).delete(model_id)
         ModelFetchedEntryDeleter(self.config_json).delete(model_id)
         self.logger.success("Model {0} deleted successfully".format(model_id))
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/content.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/content.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/get.py` & `ersilia-0.1.8/ersilia/publish/metadata.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,112 +1,96 @@
 import os
-import shutil
+import tempfile
 
-from . import BaseAction
-from ....utils.download import GitHubDownloader
-from ....utils.paths import Paths
-from ...bundle.repo import PackFile
+from ..hub.content.card import ReadmeMetadata, AirtableMetadata, RepoMetadataFile
+from ..utils.terminal import run_command
+from .. import ErsiliaBase
 
+from ..default import GITHUB_ORG
 
-MODEL_DIR = "model"
 
-
-class ModelRepositoryGetter(BaseAction):
-    def __init__(self, model_id, config_json):
-        BaseAction.__init__(
-            self, model_id=model_id, config_json=config_json, credentials_json=None
+class ReadmeUpdater(ErsiliaBase):
+    def __init__(self, model_id=None, repo_path=None, commit=True, config_json=None):
+        self.model_id = model_id
+        if repo_path is not None:
+            self.repo_path = os.path.abspath(repo_path)
+        else:
+            self.repo_path = None
+        self.commit = commit
+        self.tmp_folder = tempfile.mkdtemp(prefix="ersilia-os")
+        self.cwd = os.getcwd()
+        ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
+
+    def _git_clone(self):
+        run_command(
+            "cd {0}; GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/{1}/{2}; cd {3}".format(
+                self.tmp_folder, GITHUB_ORG, self.model_id, self.cwd
+            )
         )
-        self.token = self.cfg.HUB.TOKEN
-        self.github_down = GitHubDownloader(self.token)
-        self.org = self.cfg.HUB.ORG
-
-    def _dev_model_path(self):
-        pt = Paths()
-        path = pt.models_development_path()
-        if path is not None:
-            path = os.path.join(path, self.model_id)
-        if pt.exists(path):
-            return path
+
+    def _git_push(self):
+        if self.repo_path is None:
+            run_command(
+                'cd {0}/{1}; GIT_LFS_SKIP_SMUDGE=1 git add .; git commit -m "Updating README file from AirTable [skip ci]"; git push; cd {2}'.format(
+                    self.tmp_folder, self.model_id, self.cwd
+                )
+            )
         else:
-            path = pt.ersilia_development_path()
-            if path is not None:
-                path = os.path.join(path, "test", "models", self.model_id)
-            if pt.exists(path):
-                return path
-        return None
-
-    @staticmethod
-    def _copy_from_local(src, dst):
-        shutil.copytree(src, dst)
-
-    def _copy_from_github(self, dst):
-        self.github_down.clone(org=self.org, repo=self.model_id, destination=dst)
-
-    def get(self):
-        """Copy model repository from local or download from GitHub"""
-        folder = self._model_path(self.model_id)
-        dev_model_path = self._dev_model_path()
-        if dev_model_path is not None:
-            self.logger.debug(
-                "Copying from local {0} to {1}".format(dev_model_path, folder)
+            run_command(
+                'cd {0}; GIT_LFS_SKIP_SMUDGE=1 git add .; git commit -m "Updating README file from AirTable [skip ci]"; git push; cd {1}'.format(
+                    self.repo_path, self.cwd
+                )
             )
-            self._copy_from_local(dev_model_path, folder)
+
+    def update_remote(self):
+        self._git_clone()
+        rm = ReadmeMetadata(model_id=self.model_id)
+        bi = rm.read_information()
+        tmp_file = os.path.join(self.tmp_folder, self.model_id, "README.md")
+        rm.write_information(data=bi, readme_path=tmp_file)
+        if self.commit:
+            self._git_push()
+
+    def update_local(self):
+        rm = ReadmeMetadata(model_id=self.model_id)
+        bi = rm.read_information()
+        readme_file = os.path.join(self.repo_path, "README.md")
+        rm.write_information(data=bi, readme_path=readme_file)
+        if self.commit:
+            self._git_push()
+
+    def update(self):
+        if self.repo_path is None:
+            self.update_remote()
         else:
-            self.logger.debug("Cloning from github to {0}".format(folder))
-            self._copy_from_github(folder)
+            self.update_local()
 
 
-#  TODO: work outside GIT LFS
-class ModelParametersGetter(BaseAction):
-    def __init__(self, model_id, config_json):
-        BaseAction.__init__(
-            self, model_id=model_id, config_json=config_json, credentials_json=None
+class JsonUpdater(ErsiliaBase):
+    def __init__(self, model_id, config_json=None):
+        self.model_id = model_id
+        self.tmp_folder = tempfile.mkdtemp(prefix="ersilia-os")
+        self.cwd = os.getcwd()
+        ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
+
+    def _git_clone(self):
+        run_command(
+            "cd {0}; GIT_LFS_SKIP_SMUDGE=1 git clone https://github.com/{1}/{2}; cd {3}".format(
+                self.tmp_folder, GITHUB_ORG, self.model_id, self.cwd
+            )
         )
 
-    @staticmethod
-    def _requires_parameters(model_path):
-        pf = PackFile(model_path)
-        return pf.needs_model()
-
-    def _get_destination(self):
-        model_path = self._model_path(self.model_id)
-        return os.path.join(model_path, MODEL_DIR)
-
-    def get(self):
-        """Create a ./model folder in the model repository"""
-        model_path = self._model_path(self.model_id)
-        folder = self._get_destination()
-        if not os.path.exists(folder):
-            os.mkdir(folder)
-        if not self._requires_parameters(model_path):
-            return None
-        if not os.path.exists(folder):
-            raise Exception
-
-
-class ModelGetter(BaseAction):
-    def __init__(self, model_id, repo_path, config_json):
-        BaseAction.__init__(
-            self, model_id=model_id, config_json=config_json, credentials_json=None
+    def _git_push(self):
+        run_command(
+            'cd {0}/{1}; GIT_LFS_SKIP_SMUDGE=1 git add .; git commit -m "Updating metadata file from AirTable [skip ci]"; git push; cd {2}'.format(
+                self.tmp_folder, self.model_id, self.cwd
+            )
         )
-        self.model_id = model_id
-        self.repo_path = repo_path
-        self.mrg = ModelRepositoryGetter(model_id=model_id, config_json=config_json)
-        self.mpg = ModelParametersGetter(model_id=model_id, config_json=config_json)
-
-    def _get_repository(self):
-        self.mrg.get()
-
-    def _get_model_parameters(self):
-        self.mpg.get()
-
-    def _copy_from_repo_path(self):
-        dst = self._model_path(self.model_id)
-        src = self.repo_path
-        shutil.copytree(src, dst)
 
-    def get(self):
-        if self.repo_path is None:
-            self._get_repository()
-            self._get_model_parameters()
-        else:
-            self._copy_from_repo_path()
+    def update(self):
+        self._git_clone()
+        ai = AirtableMetadata(model_id=self.model_id)
+        data = ai.read_information()
+        tmp_file = os.path.join(self.tmp_folder, self.model_id, "metadata.json")
+        rm = RepoMetadataFile(model_id=self.model_id)
+        rm.write_information(data, tmp_file)
+        self._git_push()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/modify.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/modify.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 import os
 import tempfile
 import yaml
 
 from ersilia.default import PACKMODE_FILE
 from . import BaseAction
 from .. import ENVIRONMENT_YML, DOCKERFILE
+from ....utils.conda import SimpleConda
 from ....utils.terminal import run_command
 from ...bundle.bundle import (
     BundleEnvironmentFile,
     BundleDockerfileFile,
     BundleRequirementsFile,
 )
+from ...bundle.repo import DockerfileFile
 
 
 class ModelModifier(BaseAction):
     def __init__(self, model_id, config_json):
         BaseAction.__init__(
             self, model_id=model_id, config_json=config_json, credentials_json=None
         )
@@ -128,14 +130,46 @@
 
     def _add_model_install_commands_to_requirements_txt(self, model_id):
         BundleRequirementsFile(model_id).add_model_install_commands()
 
     def _add_model_install_commands_to_environment_yml(self, model_id):
         BundleEnvironmentFile(model_id).add_model_install_commands()
 
+    def _explicit_conda_python_path_in_run(self, model_id):
+        dir = self._get_bundle_location(model_id)
+        framework_dir = os.path.join(dir, model_id, "artifacts", "framework")
+        if not os.path.exists(framework_dir):
+            return
+        run_files = []
+        for l in os.listdir(framework_dir):
+            if l.startswith("run") and l.endswith(".sh"):
+                run_files += [l]
+        if len(run_files) != 1:
+            return
+        run_file = os.path.join(framework_dir, run_files[0])
+        self.logger.debug("Run file found in framework: {0}".format(run_file))
+        with open(run_file, "r") as f:
+            for l in f:
+                if l.startswith("conda activate"):
+                    self.logger.debug(
+                        "A conda activate statement has been found. It is not advised to modify the conda path in this bash file."
+                    )
+                    return
+        python_exec = SimpleConda().get_python_path_env(model_id)
+        self.logger.debug("Python executable: {0}".format(python_exec))
+        R = []
+        with open(run_file, "r") as f:
+            for r in f:
+                if r.startswith("python "):
+                    r = python_exec + r[6:]
+                R += [r]
+        with open(run_file, "w") as f:
+            for r in R:
+                f.write(r)
+
     def modify(self):
         # Add installs to requirements and environment
         self._add_model_install_commands_to_requirements_txt(self.model_id)
         self._add_model_install_commands_to_environment_yml(self.model_id)
         # Slightly modify bundle environment YAML file, if exists
         self._modify_bundle_environment_yml(self.model_id)
         # Slightly modify bundle Dockerfile, if necessary.
@@ -143,14 +177,16 @@
         # Check if conda is really necessary, if not, use slim base docker image
         with open(
             os.path.join(self._model_path(self.model_id), PACKMODE_FILE), "r"
         ) as f:
             pack_mode = f.read()
         if pack_mode == "conda":
             needs_conda = True
+            # Redirect python path from run command to conda path (if necessary)
+            self._explicit_conda_python_path_in_run(self.model_id)
         else:
             needs_conda = BundleEnvironmentFile(self.model_id).needs_conda()
         dockerfile = BundleDockerfileFile(self.model_id)
         if needs_conda:
             self.logger.debug("Conda is needed")
             dockerfile.set_to_full()
         else:
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/pack.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/pack.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/prepare.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/prepare.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 from . import BaseAction
 from ...bundle.status import ModelStatus
 from ...delete.delete import ModelFullDeleter
 
+from ....utils.exceptions_utils.delete_exceptions import ModelDeleteError
+from .... import throw_ersilia_exception
+
 
 class ModelPreparer(BaseAction):
     def __init__(self, model_id, overwrite, config_json):
         BaseAction.__init__(
             self, model_id=model_id, config_json=config_json, credentials_json=None
         )
         self.overwrite = overwrite
         self.status = ModelStatus(config_json=self.config_json)
-        self.deleter = ModelFullDeleter(config_json=self.config_json)
+        self.deleter = ModelFullDeleter(
+            config_json=self.config_json, overwrite=self.overwrite
+        )
 
+    @throw_ersilia_exception
     def prepare(self):
-        if self.status.is_downloaded(self.model_id):
-            if not self.overwrite:
-                return
-        self.deleter.delete(self.model_id)
+        try:
+            self.deleter.delete(self.model_id)
+        except:
+            raise ModelDeleteError(model=self.model_id)
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/sniff.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/sniff.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import os
 import csv
 import sys
 import json
 import collections
 from pathlib import Path
 
+from .... import throw_ersilia_exception
+
 from . import BaseAction
 from .... import ErsiliaBase
 from .... import ErsiliaModel
 from ....io.input import ExampleGenerator
 from ....io.pure import PureDataTyper
 from ....default import API_SCHEMA_FILE, MODEL_SIZE_FILE
-from ....utils.exceptions import EmptyOutputError
+from ....utils.exceptions_utils.exceptions import EmptyOutputError
 
 
 N = 3
 
 BUILTIN_EXAMPLE_FILE_NAME = "example.csv"
 
 
@@ -84,15 +86,15 @@
         )
         return bytes
 
     def _get_size_in_mb(self):
         dest_dir = self._model_path(self.model_id)
         repo_dir = self._get_bundle_location(self.model_id)
         size = self._get_directory_size(dest_dir) + self._get_directory_size(repo_dir)
-        mbytes = size / (1024 ** 2)
+        mbytes = size / (1024**2)
         return mbytes
 
     def _get_schema(self, results):
         input_schema = collections.defaultdict(list)
         output_schema = collections.defaultdict(list)
         for res in results:
             inp = res["input"]
@@ -130,14 +132,15 @@
                 }  # TODO revise if type=None is the best option
             else:
                 output_schema_[k]["meta"] = meta[k]
         schema = {"input": input_schema_, "output": output_schema_}
         self.logger.debug("Schema: {0}".format(schema))
         return schema
 
+    @throw_ersilia_exception
     def sniff(self):
         self.logger.debug("Sniffing model")
         self.logger.debug("Getting model size")
         size = self._get_size_in_mb()
         self.logger.debug("Mode size is {0} MB".format(size))
         path = os.path.join(self._model_path(self.model_id), MODEL_SIZE_FILE)
         with open(path, "w") as f:
@@ -149,23 +152,17 @@
         for api_name in self.model.autoservice.get_apis():
             self.logger.debug("Running API: {0}".format(api_name))
             self.logger.debug(self.inputs)
             results = [
                 result for result in self.model.autoservice.api(api_name, self.inputs)
             ]
             self.logger.debug(results)
-            try:
-                for r in results:
-                    if not r["output"]:
-                        raise EmptyOutputError(
-                            model_id=self.model_id, api_name=api_name
-                        )
-            except EmptyOutputError as err:
-                print(err)
-                sys.exit()
+            for r in results:
+                if not r["output"]:
+                    raise EmptyOutputError(model_id=self.model_id, api_name=api_name)
             schema = self._get_schema(results)
             self.logger.debug(schema)
             all_schemas[api_name] = schema
         path = os.path.join(self._model_path(self.model_id), API_SCHEMA_FILE)
         with open(path, "w") as f:
             json.dump(all_schemas, f, indent=4)
         self.logger.debug("API schema saved at {0}".format(path))
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/actions/toolize.py` & `ersilia-0.1.8/ersilia/hub/fetch/actions/toolize.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,19 +24,18 @@
         """Containerize model using bentoml with docker"""
         req = DockerRequirement()
         if not req.is_installed():
             self.logger.info("Cannot dockerize. Please make sure docker is installed.")
             return
         self.logger.debug("Dockerizing")
         tag = self.cfg.ENV.DOCKER.LATEST_TAG
-        run_command(
-            "bentoml containerize {1}:{2} -t {0}/{1}:{2}".format(
-                self.docker_org, model_id, tag
-            )
+        cmd = "bentoml containerize {1}:{2} -t {0}/{1}:{2}".format(
+            self.docker_org, model_id, tag
         )
+        run_command(cmd)
         # store docker in the local environment database
         db = EnvironmentDb(config_json=self.config_json)
         db.table = "docker"
         db.insert(
             model_id=model_id, env="{0}/{1}:{2}".format(self.docker_org, model_id, tag)
         )
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/fetch.py` & `ersilia-0.1.8/ersilia/publish/publish.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,108 +1,85 @@
-"""Fetch model from the Ersilia Model Hub"""
-
-import json
 import os
-from timeit import default_timer as timer
-from datetime import timedelta
+import shutil
+
+from .rebase import TemplateRebaser
+from . import EOS_TEMPLATE_REPOSITORY
+
+from ..utils.terminal import run_command
+from .. import ErsiliaBase
+from ..utils.dvc import DVCSetup
+from ..default import GITHUB_ORG
 
-from ... import ErsiliaBase
-from ... import logger
-from .actions.prepare import ModelPreparer
-from .actions.get import ModelGetter
-from .actions.lake import LakeGetter
-from .actions.pack import ModelPacker
-from .actions.toolize import ModelToolizer
-from .actions.content import CardGetter
-from .actions.check import ModelChecker
-from .actions.sniff import ModelSniffer
-
-from . import STATUS_FILE, DONE_TAG
-
-
-class ModelFetcher(ErsiliaBase):
-    def __init__(
-        self,
-        config_json=None,
-        credentials_json=None,
-        overwrite=True,
-        repo_path=None,
-        mode=None,
-        pip=False,
-        dockerize=False,
-    ):
+
+class ModelPublisher(ErsiliaBase):
+    def __init__(self, model_id, config_json, credentials_json):
         ErsiliaBase.__init__(
             self, config_json=config_json, credentials_json=credentials_json
         )
-        self.overwrite = overwrite
-        self.mode = mode
-        self.do_pip = pip
-        self.repo_path = repo_path
-        if self.mode == "docker":
-            self.logger.debug("When packing mode is docker, dockerization is mandatory")
-            dockerize = True
-        self.do_docker = dockerize
+        self.model_id = model_id
+        self.template_repo = EOS_TEMPLATE_REPOSITORY
+        self.repo_remote_path = os.path.join(GITHUB_ORG, self.model_id)
+        self.template_path = os.path.join(GITHUB_ORG, self.template_repo)
+        self.cwd = os.path.abspath(os.getcwd())
+        self.repo_path = os.path.join(self.cwd, self.model_id)
+        self.message = "Commit from Ersilia"
 
-    def _prepare(self):
-        mp = ModelPreparer(
+    def rebase(self):
+        rb = TemplateRebaser(
             model_id=self.model_id,
-            overwrite=self.overwrite,
+            template_repo=self.template_repo,
             config_json=self.config_json,
+            credentials_json=self.credentials_json,
         )
-        mp.prepare()
-
-    def _get(self):
-        mg = ModelGetter(
-            model_id=self.model_id,
-            repo_path=self.repo_path,
-            config_json=self.config_json,
+        rb.rebase()
+        shutil.copytree(rb.model_path, self.repo_path)
+        self.logger.debug(
+            "Rebased repository {0} with template {1}. Local path: {2}".format(
+                self.model_id, self.template_repo, self.repo_path
+            )
         )
-        mg.get()
+        rb.clean()
+        self.message = "Rebased from template {0}".format(self.template_repo)
 
-    def _lake(self):
-        ml = LakeGetter(model_id=self.model_id, config_json=self.config_json)
-        ml.get()
-
-    def _pack(self):
-        mp = ModelPacker(
-            model_id=self.model_id, mode=self.mode, config_json=self.config_json
+    def create(self, public=True):
+        if public:
+            flag = "--public"
+        else:
+            flag = "--private"
+        cmd = "gh repo create {0} --confirm --template {1} {2}".format(
+            self.repo_remote_path, self.template_path, flag
+        )
+        self.logger.debug(cmd)
+        run_command(cmd)
+        shutil.rmtree(self.repo_path)
+        cmd = "gh repo clone {0}".format(self.repo_remote_path)
+        run_command(cmd)
+        self.logger.debug(
+            "Created repository in GitHub. Local path: {0}".format(self.repo_path)
         )
-        mp.pack()
+        self.message = "Initial commit"
 
-    def _toolize(self):
-        mt = ModelToolizer(model_id=self.model_id, config_json=self.config_json)
-        mt.toolize(do_pip=self.do_pip, do_docker=self.do_docker)
-
-    def _content(self):
-        cg = CardGetter(self.model_id, self.config_json)
-        cg.get()
-
-    def _check(self):
-        mc = ModelChecker(self.model_id, self.config_json)
-        mc.check()
-
-    def _sniff(self):
-        sn = ModelSniffer(self.model_id, self.config_json)
-        sn.sniff()
-
-    def _success(self):
-        done = {DONE_TAG: True}
-        status_file = os.path.join(self._dest_dir, self.model_id, STATUS_FILE)
-        with open(status_file, "w") as f:
-            json.dump(done, f, indent=4)
+    def dvc(self):
+        dvc = DVCSetup(local_repo_path=self.repo_path, model_id=self.model_id)
+        dvc.gdrive_setup()
+        dvc.set_dvc_gdrive()
+        dvc.git_add_and_commit()
+
+    def git_push(self, message=None):
+        if not message:
+            message = self.message
+        os.chdir(self.repo_path)
+        run_command("git add .")
+        run_command("git commit -m '{0}'".format(message))
+        run_command("git pull --rebase")
+        run_command("git push")
+        os.chdir(self.cwd)
+
+    def push(self):
+        self.dvc()
+        self.git_push()
 
-    def fetch(self, model_id):
-        start = timer()
-        self.model_id = model_id
-        self._prepare()
-        self._get()
-        self._pack()
-        self._toolize()
-        self._content()
-        self._check()
-        self._sniff()
-        self._success()
-        end = timer()
-        elapsed_time = timedelta(seconds=end - start)
-        logger.info(
-            "Fetching {0} done successfully: {1}".format(model_id, elapsed_time)
-        )
+    def test(self):
+        pass
+
+    def docker(self):
+        pass
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/pack/__init__.py` & `ersilia-0.1.8/ersilia/hub/fetch/pack/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -126,19 +126,23 @@
                     assert is_pip3 is not None
                     r = r.split(" ")
                     if is_pip3:
                         r = " ".join([r[0]] + [dis_warn] + r[1:])
                     else:
                         r = " ".join(r[:3] + [dis_warn] + r[3:])
                 f.write("{0}{1}".format(r, os.linesep))
-            f.write(
-                "python -m pip {2} install bentoml=={0}{1}".format(
+            if version["version"] == "0.11.0":
+                cmd = "python -m pip {1} install git+https://github.com/ersilia-os/bentoml-ersilia.git{0}".format(
+                    os.linesep, dis_warn
+                )
+            else:
+                cmd = "python -m pip {2} install bentoml=={0}{1}".format(
                     version["version"], os.linesep, dis_warn
                 )
-            )
+            f.write(cmd)
         return fn
 
 
 class BasePack(_Deleter, _Symlinker, _Writer):
     def __init__(self, model_id, config_json):
         _Deleter.__init__(self, model_id, config_json)
         _Symlinker.__init__(self, model_id, config_json)
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/pack/mode.py` & `ersilia-0.1.8/ersilia/hub/fetch/pack/mode.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 import os
 import json
 
 from .... import ErsiliaBase
 from ...bundle.repo import DockerfileFile
 from ....utils.versioning import Versioner
+from ....utils.system import SystemChecker
 from ....setup.requirements.conda import CondaRequirement
 from ....setup.requirements.docker import DockerRequirement
 from ....default import MODEL_CONFIG_FILENAME
 
 AVAILABLE_MODES = ["system", "venv", "conda", "docker"]
 
 
 class PackModeDecision(ErsiliaBase):
     def __init__(self, model_id, config_json):
         ErsiliaBase.__init__(self, config_json=config_json, credentials_json=None)
         self.model_id = model_id
         self.versioner = Versioner(config_json=config_json)
 
-    def _correct_protobuf(self, version, dockerfile):
+    def _correct_protobuf(self, version, dockerfile, protobuf_version="3.19.5"):
+        if version["version"] == "0.11.0":
+            self.logger.debug(
+                "Custom Ersilia BentoML is used, no need for modifying protobuf version"
+            )
+            return dockerfile
         if "0.11" in version["version"]:
-            dockerfile.append_run_command("pip install protobuf==3.19.0")
+            dockerfile.append_run_command(
+                "pip install protobuf=={0}".format(protobuf_version)
+            )
             self.logger.info(
-                "Since BentoML is version 0.11, protobuf will been downgraded to 3.19.0"
+                "Since BentoML is version 0.11, protobuf will been downgraded to {0}".format(
+                    protobuf_version
+                )
             )
         return dockerfile
 
     def decide_from_config_file_if_available(self):
         folder = self._model_path(self.model_id)
         if not os.path.exists(os.path.join(folder, MODEL_CONFIG_FILENAME)):
             return None
@@ -40,14 +50,20 @@
                     )
                 )
             else:
                 return default_mode
         return None
 
     def decide(self):
+        sc = SystemChecker()
+        if sc.is_github_action():
+            self.logger.debug(
+                "Code is being run inside a GitHub Actions workflow. Use conda as a by-default mode."
+            )
+            return "conda"
         mode = self.decide_from_config_file_if_available()
         if mode is not None:
             self.logger.debug("Mode is already specified in the model repository")
             self.logger.debug("Mode: {0}".format(mode))
             return mode
         folder = self._model_path(self.model_id)
         self.logger.debug(
@@ -79,14 +95,17 @@
                 self.logger.debug("Mode: venv")
                 return "venv"
             else:
                 self.logger.debug("Mode: conda")
                 return "conda"
         else:
             self.logger.debug(
-                "The python/conda installs are not sufficient, use docker"
+                "The python/conda installs may not be sufficient, trying docker"
             )
             self.logger.debug("Mode: docker")
             dockerreq = DockerRequirement()
-            assert not dockerreq.is_inside_docker()
-            assert dockerreq.is_installed()
-            return "docker"
+            if dockerreq.is_inside_docker():
+                return "conda"
+            if dockerreq.is_installed():
+                return "docker"
+            else:
+                return "conda"
```

### Comparing `ersilia-0.1.1/ersilia/hub/fetch/pack/runners.py` & `ersilia-0.1.8/ersilia/hub/fetch/pack/runners.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 from ....utils.venv import SimpleVenv
 from ....utils.conda import SimpleConda
 from ....utils.docker import SimpleDocker
 from ....setup.baseconda import SetupBaseConda
 
 from ....default import DEFAULT_VENV
 from .. import MODEL_INSTALL_COMMANDS_FILE
-
+from .... import throw_ersilia_exception
+from ....utils.exceptions_utils.fetch_exceptions import CondaEnvironmentExistsError
 
 USE_CHECKSUM = False
 
 
 class SystemPack(BasePack):
     def __init__(self, model_id, config_json):
         BasePack.__init__(self, model_id, config_json)
@@ -98,14 +99,18 @@
                 org = base_env.split("-")[1]
                 tag = "-".join(base_env.split("-")[-2:])
                 self.logger.debug("Setting up base environment {0}".format(base_env))
                 SetupBaseConda().setup(org=org, tag=tag)
             self.logger.info(
                 "Cloning base conda environment and adding model dependencies"
             )
+            if base_env is not None:
+                if not self.conda.exists(base_env):
+                    raise CondaEnvironmentExistsError(base_env)
+
             self.conda.clone(base_env, env)
             with open(installs_file, "r") as f:
                 commandlines = f.read()
             self.conda.run_commandlines(environment=env, commandlines=commandlines)
         else:
             self.logger.debug("Environment {0} does exist".format(env))
         # create environment yml file
@@ -113,14 +118,18 @@
         self.conda.export_env_yml(env, model_path)
         # store conda environment in the local environment database
         self.logger.debug("Storing Conda environment in the local environment database")
         db = EnvironmentDb(config_json=self.config_json)
         db.table = "conda"
         db.insert(model_id=model_id, env=env)
         self.logger.debug("Done with the Conda setup")
+
+        if env is not None:
+            if not self.conda.exists(env):
+                raise CondaEnvironmentExistsError(env)
         return env
 
     def _run(self):
         env = self._setup()
         pack_snippet = """
         python {0}
         """.format(
@@ -131,14 +140,15 @@
         self.conda.run_commandlines(environment=env, commandlines=pack_snippet)
         self.logger.debug(
             "Previous command successfully run inside {0} conda environment".format(env)
         )
         self.logger.debug("Now trying to establish symlinks")
         self._symlinks()
 
+    @throw_ersilia_exception
     def run(self):
         self.logger.debug("Packing model with Conda")
         self._write_model_install_commands()
         self._run()
 
 
 class DockerPack(BasePack):
```

### Comparing `ersilia-0.1.1/ersilia/io/dataframe.py` & `ersilia-0.1.8/ersilia/io/dataframe.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/input.py` & `ersilia-0.1.8/ersilia/io/input.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 import json
 import csv
 import importlib
 import itertools
 
 from ..hub.content.card import ModelCard
 from .. import ErsiliaBase
+from .. import throw_ersilia_exception
+
+from ..utils.exceptions_utils.exceptions import NullModelIdentifierError
 
 from .shape import InputShape
 from .shape import InputShapeSingle, InputShapeList, InputShapePairOfLists
 from .readers.pyinput import PyInputReader
 from .readers.file import TabularFileReader, JsonFileReader
 
 
@@ -169,27 +172,33 @@
         data = self.adapter.adapt(inp)
         for d in data:
             yield d
 
 
 class ExampleGenerator(ErsiliaBase):
     def __init__(self, model_id, config_json=None):
+        self.check_model_id(model_id)
         self.IO = BaseIOGetter(config_json=config_json).get(model_id)
         ErsiliaBase.__init__(self, config_json=config_json)
         self.input_shape = self.IO.input_shape
         self._string_delimiter = self.IO.string_delimiter()
         self._force_simple = True
         if type(self.input_shape) is InputShapeSingle:
             self._flatten = self._flatten_single
             self._force_simple = False
         if type(self.input_shape) is InputShapeList:
             self._flatten = self._flatten_list
         if type(self.input_shape) is InputShapePairOfLists:
             self._flatten = self._flatten_single
 
+    @throw_ersilia_exception
+    def check_model_id(self, model_id):
+        if model_id is None:
+            raise NullModelIdentifierError(model=model_id)
+
     @staticmethod
     def _get_delimiter(file_name):
         extension = file_name.split(".")[-1]
         if extension == "tsv":
             return "\t"
         else:
             return ","
```

### Comparing `ersilia-0.1.1/ersilia/io/output.py` & `ersilia-0.1.8/ersilia/io/output.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .dataframe import Dataframe
 from .readers.file import FileTyper
 from .pure import PureDataTyper
 from ..serve.schema import ApiSchema
 from .. import ErsiliaBase
 from ..utils.hdf5 import Hdf5Data, Hdf5DataStacker
 from ..default import FEATURE_MERGE_PATTERN
+from ..db.hubdata.interfaces import AirtableInterface
 
 
 class DataFrame(object):
     def __init__(self, data, columns):
         self.data = data
         self.columns = columns
 
@@ -209,29 +210,46 @@
                     ]
                 else:
                     output_keys_expanded += ["{0}".format(m_) for m_ in m]
             else:
                 output_keys_expanded += [ok]
         return output_keys_expanded
 
-    def _to_dataframe(self, result):
+    def _get_outputshape_from_airtable(self, model_id):
+        airtable_interface = AirtableInterface(config_json=self.config_json)
+        output_shape = " "
+        for record in airtable_interface.items():
+            model_idi = record["fields"]["Identifier"]
+            try:
+                if model_idi == model_id:
+                    output_shape = record["fields"]["Output Shape"]
+            except KeyError:
+                self.logger.warning("The Output Shape field is empty")
+        return output_shape
+
+    def _to_dataframe(self, result, model_id):
+        output_shape = self._get_outputshape_from_airtable(model_id)
         result = json.loads(result)
         R = []
         output_keys = None
         output_keys_expanded = None
         for r in result:
             inp = r["input"]
             out = r["output"]
-            if output_keys is None:
-                output_keys = [k for k in out.keys()]
-            vals = [out[k] for k in output_keys]
-            dtypes = [self.__pure_dtype(k) for k in output_keys]
-            if output_keys_expanded is None:
-                output_keys_expanded = self.__expand_output_keys(vals, output_keys)
-            vals = self.__cast_values(vals, dtypes, output_keys)
+            if output_shape == "Flexible List":
+                vals = [json.dumps(out)]
+                output_keys_expanded = ["outcome"]
+            else:
+                if output_keys is None:
+                    output_keys = [k for k in out.keys()]
+                vals = [out[k] for k in output_keys]
+                dtypes = [self.__pure_dtype(k) for k in output_keys]
+                if output_keys_expanded is None:
+                    output_keys_expanded = self.__expand_output_keys(vals, output_keys)
+                vals = self.__cast_values(vals, dtypes, output_keys)
             R += [[inp["key"], inp["input"]] + vals]
         columns = ["key", "input"] + output_keys_expanded
         df = DataFrame(data=R, columns=columns)
         return df
 
     def meta(self):
         if self._meta is None:
@@ -276,21 +294,21 @@
         if output is not None and self._schema is None:
             raise Exception
         if self._has_extension(output, "json"):
             data = json.loads(result)
             with open(output, "w") as f:
                 json.dump(data, f, indent=4)
         if self._has_extension(output, "csv"):
-            df = self._to_dataframe(result)
+            df = self._to_dataframe(result, model_id)
             df.write(output)
         if self._has_extension(output, "tsv"):
-            df = self._to_dataframe(result)
+            df = self._to_dataframe(result, model_id)
             df.write(output, delimiter="\t")
         if self._has_extension(output, "h5"):
-            df = self._to_dataframe(result)
+            df = self._to_dataframe(result, model_id)
             df.write(output)
         return result
 
 
 class DictlistDataframeConverter(GenericOutputAdapter):
     def __init__(self, config_json):
         GenericOutputAdapter.__init__(self, config_json=config_json)
```

### Comparing `ersilia-0.1.1/ersilia/io/pure.py` & `ersilia-0.1.8/ersilia/io/pure.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/readers/file.py` & `ersilia-0.1.8/ersilia/io/readers/file.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/readers/pyinput.py` & `ersilia-0.1.8/ersilia/io/readers/pyinput.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/shape.py` & `ersilia-0.1.8/ersilia/io/shape.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/types/compound.py` & `ersilia-0.1.8/ersilia/io/types/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/types/examples/compound.py` & `ersilia-0.1.8/ersilia/io/types/examples/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/types/examples/compound.tsv` & `ersilia-0.1.8/ersilia/io/types/examples/compound.tsv`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/io/types/examples/protein.tsv` & `ersilia-0.1.8/ersilia/io/types/examples/protein.tsv`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/lake/base.py` & `ersilia-0.1.8/ersilia/lake/base.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/lake/interface.py` & `ersilia-0.1.8/ersilia/lake/interface.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/lake/manager.py` & `ersilia-0.1.8/ersilia/lake/manager.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/publish/deploy.py` & `ersilia-0.1.8/ersilia/publish/deploy.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/publish/lake.py` & `ersilia-0.1.8/ersilia/publish/lake.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/publish/publish.py` & `ersilia-0.1.8/ersilia/publish/store.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,85 +1,69 @@
+"""
+Class used to store model when done developing it.
+
+This functionality is used when developing of a model is done.
+"""
 import os
 import shutil
-
-from .rebase import TemplateRebaser
-from . import EOS_TEMPLATE_REPOSITORY
-
-from ..utils.terminal import run_command
 from .. import ErsiliaBase
-from ..utils.dvc import DVCSetup
-from ..default import GITHUB_ORG
+from ..utils.zip import Zipper
+from ..utils.upload import OsfUploader
+from ..utils.remove import OsfRemover
 
 
-class ModelPublisher(ErsiliaBase):
-    def __init__(self, model_id, config_json, credentials_json):
+class ModelStorager(ErsiliaBase):
+    def __init__(self, config_json=None, credentials_json=None, overwrite=True):
         ErsiliaBase.__init__(
             self, config_json=config_json, credentials_json=credentials_json
         )
-        self.model_id = model_id
-        self.template_repo = EOS_TEMPLATE_REPOSITORY
-        self.repo_remote_path = os.path.join(GITHUB_ORG, self.model_id)
-        self.template_path = os.path.join(GITHUB_ORG, self.template_repo)
-        self.cwd = os.path.abspath(os.getcwd())
-        self.repo_path = os.path.join(self.cwd, self.model_id)
-        self.message = "Commit from Ersilia"
-
-    def rebase(self):
-        rb = TemplateRebaser(
-            model_id=self.model_id,
-            template_repo=self.template_repo,
-            config_json=self.config_json,
-            credentials_json=self.credentials_json,
+        self.overwrite = overwrite
+        self.osf_up = OsfUploader(
+            overwrite=overwrite, username=self.cred.OSF.USER, password=self.cred.OSF.PWD
         )
-        rb.rebase()
-        shutil.copytree(rb.model_path, self.repo_path)
-        self.logger.debug(
-            "Rebased repository {0} with template {1}. Local path: {2}".format(
-                self.model_id, self.template_repo, self.repo_path
-            )
-        )
-        rb.clean()
-        self.message = "Rebased from template {0}".format(self.template_repo)
 
-    def create(self, public=True):
-        if public:
-            flag = "--public"
+    def _data_path(self, model_id):
+        return os.path.join(self.cred.LOCAL.DATA, model_id)
+
+    def _copy_to_local(self, path, model_id):
+        dest_path = self._data_path(model_id)
+        if os.path.exists(dest_path):
+            if self.overwrite:
+                shutil.rmtree(dest_path)
+                os.makedirs(dest_path)
+            else:
+                return
         else:
-            flag = "--private"
-        cmd = "gh repo create {0} --confirm --template {1} {2}".format(
-            self.repo_remote_path, self.template_path, flag
-        )
-        self.logger.debug(cmd)
-        run_command(cmd)
-        shutil.rmtree(self.repo_path)
-        cmd = "gh repo clone {0}".format(self.repo_remote_path)
-        run_command(cmd)
-        self.logger.debug(
-            "Created repository in GitHub. Local path: {0}".format(self.repo_path)
-        )
-        self.message = "Initial commit"
+            os.makedirs(dest_path)
+        shutil.copytree(path, os.path.join(dest_path, "model"))
+
+    def _zip(self, model_id):
+        data_path = self._data_path(model_id)
+        zipper = Zipper(remove=False)
+        zip_file = data_path + ".zip"
+        zipper.zip(data_path, data_path)
+        return zip_file
+
+    def _upload_to_osf(self, model_id):
+        zip_file = self._zip(model_id)
+        destination = "models/" + model_id + ".zip"
+        self.osf_up.push(self.cfg.EXT.OSF_PROJECT, zip_file, destination)
+        os.remove(zip_file)
+
+    def store(self, path, model_id):
+        """Store model in the local data directory and in OSF."""
+        self._copy_to_local(path, model_id)
+        self._upload_to_osf(model_id)
 
-    def dvc(self):
-        dvc = DVCSetup(local_repo_path=self.repo_path, model_id=self.model_id)
-        dvc.gdrive_setup()
-        dvc.set_dvc_gdrive()
-        dvc.git_add_and_commit()
-
-    def git_push(self, message=None):
-        if not message:
-            message = self.message
-        os.chdir(self.repo_path)
-        run_command("git add .")
-        run_command("git commit -m '{0}'".format(message))
-        run_command("git pull --rebase")
-        run_command("git push")
-        os.chdir(self.cwd)
-
-    def push(self):
-        self.dvc()
-        self.git_push()
 
-    def test(self):
-        pass
+class ModelRemover(ErsiliaBase):
+    def __init__(self, config_json=None, credentials_json=None):
+        ErsiliaBase.__init__(
+            self, config_json=config_json, credentials_json=credentials_json
+        )
+        self.osf_rm = OsfRemover(
+            username=self.cred.OSF.USER, password=self.cred.OSF.PWD
+        )
 
-    def docker(self):
-        pass
+    def remove(self, model_id):
+        zip_file = "models/" + model_id + ".zip"
+        self.osf_rm.remove(self.cfg.EXT.OSF_PROJECT, zip_file)
```

### Comparing `ersilia-0.1.1/ersilia/publish/rebase.py` & `ersilia-0.1.8/ersilia/publish/rebase.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/serve/api.py` & `ersilia-0.1.8/ersilia/serve/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from ..io.input import GenericInputAdapter
 from ..io.output import GenericOutputAdapter
 from ..lake.interface import IsauraInterface
 from .. import logger
 from .. import ErsiliaBase
 from .schema import ApiSchema
 
+from ..utils.exceptions_utils.api_exceptions import InputFileNotFoundError
+
 
 class Api(object):
     def __init__(self, model_id, url, api_name, save_to_lake, config_json):
         self.config_json = config_json
         self.model_id = model_id
         self.input_adapter = GenericInputAdapter(self.model_id, config_json=config_json)
         self.output_adapter = GenericOutputAdapter(config_json=config_json)
@@ -290,15 +292,30 @@
         ):
             for res in self.post_only_calculations(input, output, batch_size):
                 yield res
         else:
             for res in self.post_amenable_to_h5(input, output, batch_size):
                 yield res
 
+    def _is_input_file(self, input):
+        if type(input) is str:
+            if input.endswith(".csv"):
+                return True
+            if input.endswith(".tst"):
+                return True
+            if input.endswith(".json"):
+                return True
+            if input.endswith(".txt"):
+                return True
+        return False
+
     def post(self, input, output, batch_size):
+        if self._is_input_file(input):
+            if not os.path.exists(input):
+                raise InputFileNotFoundError(file_name=input)
         self.logger.debug("Posting to {0}".format(self.api_name))
         self.logger.debug("Batch size {0}".format(batch_size))
         unique_input, mapping = self._unique_input(input)
         results_ = {}
         for res in self.post_unique_input(
             input=unique_input, output=None, batch_size=batch_size
         ):
```

### Comparing `ersilia-0.1.1/ersilia/serve/autoservice.py` & `ersilia-0.1.8/ersilia/serve/autoservice.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,30 +10,33 @@
     DummyService,
 )
 from .api import Api
 from ..db.environments.managers import DockerManager
 from .. import ErsiliaBase
 from ..utils import tmp_pid_file
 
-from ..default import DEFAULT_BATCH_SIZE
+from ..default import DEFAULT_BATCH_SIZE, SERVICE_CLASS_FILE, APIS_LIST_FILE
 
 DEFAULT_OUTPUT = None
 
 
 class AutoService(ErsiliaBase):
-    def __init__(self, model_id, service_class=None, config_json=None):
+    def __init__(
+        self, model_id, service_class=None, config_json=None, preferred_port=None
+    ):
         ErsiliaBase.__init__(self, config_json=config_json)
         self.logger.debug("Setting AutoService for {0}".format(model_id))
         self.config_json = config_json
         self.model_id = model_id
         self._meta = None
+        self._preferred_port = preferred_port
         if service_class is None:
             self.logger.debug("No service class provided, deciding automatically")
             service_class_file = os.path.join(
-                self._get_bundle_location(model_id), "service_class.txt"
+                self._get_bundle_location(model_id), SERVICE_CLASS_FILE
             )
             if os.path.exists(service_class_file):
                 self.logger.debug(
                     "Service class file exists in folder {0}".format(service_class_file)
                 )
                 with open(service_class_file, "r") as f:
                     s = f.read()
@@ -41,94 +44,112 @@
                     s = None
             else:
                 s = None
             if s is not None:
                 self.logger.debug("Service class: {0}".format(s))
                 if s == "system":
                     self.service = SystemBundleService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     )
                 elif s == "venv":
                     self.service = VenvEnvironmentService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     )
                 elif s == "conda":
                     self.service = CondaEnvironmentService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     )
                 elif s == "docker":
-                    self.service = DockerImageService(model_id, config_json=config_json)
+                    self.service = DockerImageService(
+                        model_id, config_json=config_json, preferred_port=preferred_port
+                    )
                 else:
                     self.service = None
                 self._service_class = s
             else:
                 self.logger.debug(
                     "No service class file exists in {0}".format(service_class_file)
                 )
                 with open(service_class_file, "w") as f:
                     if SystemBundleService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     ).is_available():
                         self.service = SystemBundleService(
-                            model_id, config_json=config_json
+                            model_id,
+                            config_json=config_json,
+                            preferred_port=preferred_port,
                         )
                         self.logger.debug("Service class: system")
                         f.write("system")
                         self._service_class = "system"
                     elif VenvEnvironmentService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     ).is_available():
                         self.service = VenvEnvironmentService(
-                            model_id, config_json=config_json
+                            model_id,
+                            config_json=config_json,
+                            preferred_port=preferred_port,
                         )
                         f.write("venv")
                         self.logger.debug("Service class: venv")
                         self._service_class = "venv"
                     elif CondaEnvironmentService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     ).is_available():
                         self.service = CondaEnvironmentService(
-                            model_id, config_json=config_json
+                            model_id,
+                            config_json=config_json,
+                            preferred_port=preferred_port,
                         )
                         f.write("conda")
                         self.logger.debug("Service class: conda")
                         self._service_class = "conda"
                     elif DockerImageService(
-                        model_id, config_json=config_json
+                        model_id, config_json=config_json, preferred_port=preferred_port
                     ).is_available():
                         self.service = DockerImageService(
-                            model_id, config_json=config_json
+                            model_id,
+                            config_json=config_json,
+                            preferred_port=preferred_port,
                         )
                         f.write("docker")
                         self.logger.debug("Service class: docker")
                         self._service_class = "docker"
                     else:
                         self.logger.debug("Service class: dummy")
-                        self.service = DummyService(model_id, config_json=config_json)
+                        self.service = DummyService(
+                            model_id,
+                            config_json=config_json,
+                            preferred_port=preferred_port,
+                        )
         else:
             self.logger.info("Service class provided")
             # predefined service class
             service_class = self._service_class_loader(service_class)
-            if service_class(model_id, config_json).is_available():
-                self.service = service_class(model_id, config_json=config_json)
+            if service_class(
+                model_id, config_json=config_json, preferred_port=preferred_port
+            ).is_available():
+                self.service = service_class(
+                    model_id, config_json=config_json, preferred_port=preferred_port
+                )
             else:
                 self.service = None
         self._set_apis()
 
     def _set_api(self, api_name):
         def _method(input, output=DEFAULT_OUTPUT, batch_size=DEFAULT_BATCH_SIZE):
             return self.api(api_name, input, output, batch_size)
 
         setattr(self, api_name, _method)
 
     def _set_apis(self):
         if self.service is None:
             return
         apis_list = os.path.join(
-            self._get_bundle_location(self.model_id), "apis_list.txt"
+            self._get_bundle_location(self.model_id), APIS_LIST_FILE
         )
         if os.path.exists(apis_list):
             with open(apis_list, "r") as f:
                 for l in f:
                     api_name = l.rstrip()
                     self._set_api(api_name)
         else:
```

### Comparing `ersilia-0.1.1/ersilia/serve/schema.py` & `ersilia-0.1.8/ersilia/serve/schema.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/serve/services.py` & `ersilia-0.1.8/ersilia/serve/services.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 from ..default import PACKMODE_FILE
 
 SLEEP_SECONDS = 1
 TIMEOUT_SECONDS = 1000
 
 
 class BaseServing(ErsiliaBase):
-    def __init__(self, model_id, config_json=None):
+    def __init__(self, model_id, config_json=None, preferred_port=None):
         ErsiliaBase.__init__(self, config_json=config_json)
         self.model_id = model_id
         self.bundle_tag = self._get_latest_bundle_tag(model_id=self.model_id)
+        self.port = preferred_port
 
     def _get_info_from_bento(self):
         """Get info available from the Bento"""
         tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
         tmp_file = os.path.join(tmp_folder, "info.json")
         cmd = "bentoml info --quiet {0}:{1} > {2}".format(
             self.model_id, self.bundle_tag, tmp_file
@@ -53,23 +54,35 @@
             return
         self.logger.debug("Using URL: {0}".format(self.url))
         response = requests.post("{0}/{1}".format(self.url, api_name), json=input)
         return response.json()
 
 
 class _BentoMLService(BaseServing):
-    def __init__(self, model_id, config_json=None):
-        BaseServing.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        BaseServing.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
         self.SEARCH_PRE_STRING = "* Running on "
         self.SEARCH_SUF_STRING = "Press CTRL+C to quit"
         self.ERROR_STRING = "error"
 
     def _bentoml_serve(self, runcommand_func=None):
         self.logger.debug("Trying to serve model with BentoML locally")
-        self.port = find_free_port()
+        preferred_port = self.port
+        self.port = find_free_port(preferred_port=preferred_port)
+        if self.port != preferred_port:
+            self.logger.warning(
+                "Port {0} was already in use. Using {1} instead".format(
+                    preferred_port, self.port
+                )
+            )
         self.logger.debug("Free port: {0}".format(self.port))
         tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
         tmp_script = os.path.join(tmp_folder, "serve.sh")
         tmp_file = os.path.join(tmp_folder, "serve.log")
         tmp_pid = os.path.join(tmp_folder, "serve.pid")
         sl = ["#!/bin/bash"]
         sl += [
@@ -146,16 +159,21 @@
         try:
             os.kill(self.pid, 9)
         except:
             self.logger.info("PID {0} is unassigned".format(self.pid))
 
 
 class SystemBundleService(_BentoMLService):
-    def __init__(self, model_id, config_json=None):
-        _BentoMLService.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        _BentoMLService.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
 
     def __enter__(self):
         self.serve()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         self.close()
@@ -181,16 +199,21 @@
         self._close()
 
     def api(self, api_name, input):
         return self._api_with_url(api_name, input)
 
 
 class VenvEnvironmentService(_BentoMLService):
-    def __init__(self, model_id, config_json=None):
-        _BentoMLService.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        _BentoMLService.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
         self.venv = SimpleVenv(self._model_path(model_id))
 
     def __enter__(self):
         self.serve()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
@@ -213,16 +236,21 @@
         self._close()
 
     def api(self, api_name, input):
         return self._api_with_url(api_name, input)
 
 
 class CondaEnvironmentService(_BentoMLService):
-    def __init__(self, model_id, config_json=None):
-        _BentoMLService.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        _BentoMLService.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
         self.db = EnvironmentDb()
         self.db.table = "conda"
         self.conda = SimpleConda()
 
     def __enter__(self):
         self.serve()
         return self
@@ -256,20 +284,25 @@
         self._close()
 
     def api(self, api_name, input):
         return self._api_with_url(api_name, input)
 
 
 class DockerImageService(BaseServing):
-    def __init__(self, model_id, config_json=None):
-        BaseServing.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        BaseServing.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
         self.db = EnvironmentDb()
         self.db.table = "docker"
         self.docker = SimpleDocker()
-        self.dm = DockerManager(config_json=config_json)
+        self.dm = DockerManager(config_json=config_json, preferred_port=preferred_port)
         self.pid = -1
 
     def __enter__(self):
         self.serve()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
@@ -305,16 +338,21 @@
 
     def api(self, api_name, input):
         return self._api_with_url(api_name, input)
 
 
 # TODO: Include 'pip' within available service_class
 class PipInstalledService(BaseServing):
-    def __init__(self, model_id, config_json=None):
-        BaseServing.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        BaseServing.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
         self.pid = -1
 
     def __enter__(self):
         self.serve()
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
@@ -343,16 +381,21 @@
 
     def api(self, api_name, input):
         method = getattr(self.mdl, api_name)
         return method(input)
 
 
 class DummyService(BaseServing):
-    def __init__(self, model_id, config_json=None):
-        BaseServing.__init__(self, model_id=model_id, config_json=config_json)
+    def __init__(self, model_id, config_json=None, preferred_port=None):
+        BaseServing.__init__(
+            self,
+            model_id=model_id,
+            config_json=config_json,
+            preferred_port=preferred_port,
+        )
 
     def __enter__(self):
         return self
 
     def __exit__(self, exception_type, exception_value, traceback):
         self.close()
```

### Comparing `ersilia-0.1.1/ersilia/setup/baseconda.py` & `ersilia-0.1.8/ersilia/setup/baseconda.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from packaging import version
 
 from ..utils.conda import SimpleConda
 from ..utils.terminal import run_command
 from ..utils.versioning import Versioner
 from .utils.clone import ErsiliaCloner
 
+from .. import logger
+
 
 class SetupBaseConda(object):
     def __init__(self, config_json=None):
         self.conda = SimpleConda()
         self.versions = Versioner()
         self.cloner = ErsiliaCloner(config_json=config_json)
 
@@ -36,17 +38,22 @@
             "python": self.versions.reformat_py(tag[1]),
         }
         return data
 
     def _install_command(self, org, tag):
         tag = self._parse_tag(tag)
         if self._is_bentoml(org):
-            cmd = "pip install bentoml=={0}".format(tag["ver"])
+            if tag["ver"] == "0.11.0":
+                logger.debug("Installing from ersilia's custom BentoML")
+                cmd = "python -m pip install git+https://github.com/ersilia-os/bentoml-ersilia.git"
+            else:
+                logger.debug("Installing from BentoML directly")
+                cmd = "python -m pip install bentoml=={0}".format(tag["ver"])
         elif self._is_ersiliaos(org):
-            cmd = "pip install -e ."
+            cmd = "python -m pip install -e ."
         else:
             raise Exception
         return cmd
 
     def _get_env_name(self, org, tag):
         return self.versions.base_conda_name(org, tag)
 
@@ -74,15 +81,15 @@
         kept = []
         for v in available_versions:
             if version.parse(v) >= version.parse(python_version):
                 kept += [v]
         return ".".join(kept[0].split(".")[:2])
 
     def setup(self, org, tag):
-        """Creates a conda enviornment to be used as base environment to be used as model server.
+        """Creates a conda environment to be used as base environment for the model server.
 
         Args:
             org: organisation (bentoml or ersiliaos)
             tag: 0.0.0-py37 format
         """
         env = self._get_env_name(org, tag)
         if self.conda.exists(env):
```

### Comparing `ersilia-0.1.1/ersilia/setup/basedocker.py` & `ersilia-0.1.8/ersilia/setup/basedocker.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import tempfile
 from ..utils.docker import SimpleDocker
 from ..utils.versioning import Versioner
 from .. import ErsiliaBase
 from .utils.clone import ErsiliaCloner
 
+
 # TODO: Make sure it is used.
 class SetupBaseDocker(ErsiliaBase):
     def __init__(self, config_json=None):
         ErsiliaBase.__init__(self, config_json=config_json)
         self.docker = SimpleDocker()
         self.versions = Versioner()
         self.cloner = ErsiliaCloner(config_json=config_json)
```

### Comparing `ersilia-0.1.1/ersilia/setup/requirements/compound.py` & `ersilia-0.1.8/ersilia/setup/requirements/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/setup/requirements/docker.py` & `ersilia-0.1.8/ersilia/setup/requirements/docker.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/setup/utils/clone.py` & `ersilia-0.1.8/ersilia/setup/utils/clone.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/clear.py` & `ersilia-0.1.8/ersilia/utils/clear.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/conda.py` & `ersilia-0.1.8/ersilia/utils/conda.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from collections import defaultdict, OrderedDict
 from .terminal import run_command, run_command_check_output
 from .docker import SimpleDockerfileParser
 from .versioning import Versioner
 from .supp.conda_env_resolve import CHECKSUM_NCHAR, CHECKSUM_FILE
 from ..default import CONDA_ENV_YML_FILE
 from .. import logger
-
+from ..utils.exceptions_utils.fetch_exceptions import ModelPackageInstallError
+from .. import throw_ersilia_exception
 
 BASE = "base"
 SPECS_JSON = ".specs.json"
 
 
 class BaseConda(object):
     def __init__(self):
@@ -269,14 +270,22 @@
         envs = self._env_list()
         envs_list = []
         for l in envs:
             if l.startswith(environment):
                 envs_list += [l.split(" ")[0]]
         return envs_list
 
+    def get_python_path_env(self, environment):
+        tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
+        tmp_file = os.path.join(tmp_folder, "tmp.txt")
+        self.run_commandlines(environment, "which python > {0}".format(tmp_file))
+        with open(tmp_file, "r") as f:
+            python_path = f.read().rstrip()
+        return python_path
+
     def delete_one(self, environment):
         if not self.exists(environment):
             return
         tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
         tmp_script = os.path.join(tmp_folder, "script.sh")
         bash_script = self.activate_base()
         bash_script += """
@@ -344,14 +353,24 @@
         """.format(
             self.conda_prefix(True), src_env, dst_env
         )
         with open(tmp_script, "w") as f:
             f.write(bash_script)
         run_command("bash {0}".format(tmp_script))
 
+    def _catch_critical_errors_in_conda(self, log):
+        log = log.split(os.linesep)
+        critical_errors = []
+        for l in log:
+            if l.startswith("ERROR"):
+                if "dependency resolver" not in l:
+                    critical_errors += [l]
+        return critical_errors
+
+    @throw_ersilia_exception
     def run_commandlines(self, environment, commandlines):
         """
         Run commands in a given conda environment.
         """
         logger.debug("Run commandlines on {0}".format(environment))
         logger.debug(commandlines)
         if not self.exists(environment):
@@ -367,11 +386,22 @@
         conda env list
         {2}
         """.format(
             self.conda_prefix(True), environment, commandlines
         )
         with open(tmp_script, "w") as f:
             f.write(bash_script)
-        cmd = "bash {0}".format(tmp_script)
+
+        tmp_folder = tempfile.mkdtemp(prefix="ersilia-")
+        tmp_log = os.path.join(tmp_folder, "command_outputs.log")
+        cmd = "bash {0} > {1} 2>&1".format(tmp_script, tmp_log)
         logger.debug("Running {0}".format(cmd))
         run_command(cmd)
+        with open(tmp_log, "r") as f:
+            log_file = f.read()
+        logger.debug(log_file)
+        if "ERROR" in log_file:
+            logger.debug("Error occurred while running: {0}".format(cmd))
+            critical_errors = self._catch_critical_errors_in_conda(log_file)
+            if len(critical_errors) > 0:
+                raise ModelPackageInstallError(cmd)
         logger.debug("Activation done")
```

### Comparing `ersilia-0.1.1/ersilia/utils/config.py` & `ersilia-0.1.8/ersilia/utils/config.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/cron.py` & `ersilia-0.1.8/ersilia/utils/cron.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/csvfile.py` & `ersilia-0.1.8/ersilia/utils/csvfile.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/docker.py` & `ersilia-0.1.8/ersilia/utils/docker.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/dvc.py` & `ersilia-0.1.8/ersilia/utils/dvc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from . import terminal
 import h5py
 import os
 from ..default import H5_DATA_FILE, ISAURA_GDRIVE, ISAURA_TEAM_GDRIVE
-from pydrive2.auth import GoogleAuth
-from pydrive2.drive import GoogleDrive
+
+try:
+    from pydrive2.auth import GoogleAuth
+    from pydrive2.drive import GoogleDrive
+except:
+    GoogleAuth = None
+    GoogleDrive = None
 
 from .config import Secrets
 
 
 def set_secrets_file():
     secrets = Secrets()
     if not os.path.exists(secrets.gdrive_client_secrets_json):
```

### Comparing `ersilia-0.1.1/ersilia/utils/hdf5.py` & `ersilia-0.1.8/ersilia/utils/hdf5.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/compound.py` & `ersilia-0.1.8/ersilia/utils/identifiers/compound.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/file.py` & `ersilia-0.1.8/ersilia/utils/identifiers/file.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/long.py` & `ersilia-0.1.8/ersilia/utils/identifiers/long.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/model.py` & `ersilia-0.1.8/ersilia/utils/identifiers/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         result_str += random.choice(self.numbers[1:])
         result_str += "".join(
             random.choice(self.letters + self.numbers) for _ in range(3)
         )
         return result_str
 
     def is_valid(self, s):
+        if len(s) != 7:
+            return False
         return Paths._eos_regex().match(s)
 
     def is_test(self, s):
         if s[3] == "0":
             return True
         else:
             return False
```

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/protein.py` & `ersilia-0.1.8/ersilia/utils/identifiers/protein.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/identifiers/short.py` & `ersilia-0.1.8/ersilia/utils/identifiers/short.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/installers.py` & `ersilia-0.1.8/ersilia/utils/installers.py`

 * *Files 0% similar despite different names*

```diff
@@ -297,15 +297,15 @@
         ins.rdkit()
         ins.config()
         with open(status["install_status_file"], "w") as f:
             f.write("base")
 
 
 def full_installer(ignore_status=False):
-    """The full installer does all the installations necessary to run ersila."""
+    """The full installer does all the installations necessary to run ersilia."""
     status = check_install_status()
     if status["status"] != "full" or ignore_status:
         ins = Installer()
         ins.profile()
         ins.conda()
         ins.git()
         ins.rdkit()
```

### Comparing `ersilia-0.1.1/ersilia/utils/logging.py` & `ersilia-0.1.8/ersilia/utils/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 import sys
 import os
 import json
 from loguru import logger
-from ..default import EOS, LOGGING_FILE, VERBOSE_FILE
+from ..default import EOS, LOGGING_FILE, CURRENT_LOGGING_FILE, VERBOSE_FILE
 
 
 ROTATION = "10 MB"
 
 
 class Logger(object):
     def __init__(self):
         self.logger = logger
         self.logger.remove()
         self._console = None
         self._file = None
         self.fmt = "{time:HH:mm:ss} | {level: <8} | {message}"
         self._verbose_file = os.path.join(EOS, VERBOSE_FILE)
-        self._log_to_file()
         self._log_to_console()
+        self._log_to_file()
+        self._log_to_current_file()
         self._log_terminal_commands_to_console()
 
     def _log_to_file(self):
         self._file = self.logger.add(
             os.path.join(EOS, LOGGING_FILE), format=self.fmt, rotation=ROTATION
         )
 
+    def _log_to_current_file(self):
+        current_log_file = os.path.join(EOS, CURRENT_LOGGING_FILE)
+        if os.path.exists(current_log_file):
+            os.remove(current_log_file)
+        self._current_file = self.logger.add(
+            os.path.join(EOS, CURRENT_LOGGING_FILE), format=self.fmt, rotation=ROTATION
+        )
+
     def _log_to_console(self):
         if self._console is None:
             self._console = self.logger.add(sys.stderr, format=self.fmt)
 
     def _unlog_from_console(self):
         if self._console is not None:
             # self.logger.remove(self._console)
```

### Comparing `ersilia-0.1.1/ersilia/utils/paths.py` & `ersilia-0.1.8/ersilia/utils/paths.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/supp/conda_env_resolve.py` & `ersilia-0.1.8/ersilia/utils/supp/conda_env_resolve.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/terminal.py` & `ersilia-0.1.8/ersilia/utils/terminal.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,14 @@
     return answer
 
 
 def yes_no_input(prompt, default_answer, timeout=5):
     ans = raw_input_with_timeout(
         prompt=prompt, default_answer=default_answer, timeout=timeout
     )
-    if ans is None:
+    if ans is None or ans == "":
         return default_answer
     ans = str(ans).lower()
     if ans[0] == "n":
         return False
     else:
         return True
```

### Comparing `ersilia-0.1.1/ersilia/utils/upload.py` & `ersilia-0.1.8/ersilia/utils/upload.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/ersilia/utils/versioning.py` & `ersilia-0.1.8/ersilia/utils/versioning.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     def ersilia_version_with_py(self):
         ver = self.ersilia_version()
         ver = "{0}-{1}".format(ver, self.python_version(py_format=True))
         return ver
 
     def ersilia_version_from_path(self, path):
-        static_version_file = "_clean_static_version.py"
+        static_version_file = "_static_version.py"
         fn = os.path.join(path, "ersilia", static_version_file)
         if not os.path.exists(fn):
             fn = os.path.join(path, static_version_file)
         if not os.path.exists(fn):
             raise Exception
         with open(fn, "r") as f:
             text = f.read()
@@ -59,10 +59,10 @@
             tag = self.ersilia_version_with_py()
         env = self.cfg.ENV.CONDA.EOS_BASE_ENV
         name = "{0}-{1}-{2}".format(env, org, tag)
         return name
 
     @staticmethod
     def reformat_py(v):
-        if len(v) != 4:
+        if len(v) < 4:
             raise Exception
-        return "{0}.{1}".format(v[2], v[3])
+        return "{0}.{1}".format(v[2], v[3:])
```

### Comparing `ersilia-0.1.1/ersilia.egg-info/PKG-INFO` & `ersilia-0.1.8/ersilia.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,435 +1,482 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6572 7369  : 2.1.Name: ersi
 00000020: 6c69 610a 5665 7273 696f 6e3a 2030 2e31  lia.Version: 0.1
-00000030: 2e31 0a53 756d 6d61 7279 3a20 4120 6875  .1.Summary: A hu
+00000030: 2e38 0a53 756d 6d61 7279 3a20 4120 6875  .8.Summary: A hu
 00000040: 6220 6f66 2041 492f 4d4c 206d 6f64 656c  b of AI/ML model
 00000050: 7320 666f 7220 6f70 656e 2073 6f75 7263  s for open sourc
 00000060: 6520 6472 7567 2064 6973 636f 7665 7279  e drug discovery
 00000070: 2061 6e64 2067 6c6f 6261 6c20 6865 616c   and global heal
 00000080: 7468 0a48 6f6d 652d 7061 6765 3a20 6874  th.Home-page: ht
 00000090: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 000000a0: 2f65 7273 696c 6961 2d6f 732f 6572 7369  /ersilia-os/ersi
 000000b0: 6c69 610a 4175 7468 6f72 3a20 4572 7369  lia.Author: Ersi
 000000c0: 6c69 6120 4f70 656e 2053 6f75 7263 6520  lia Open Source 
 000000d0: 496e 6974 6961 7469 7665 0a41 7574 686f  Initiative.Autho
-000000e0: 722d 656d 6169 6c3a 206d 6971 7565 6c40  r-email: miquel@
-000000f0: 6572 7369 6c69 612e 696f 0a4c 6963 656e  ersilia.io.Licen
-00000100: 7365 3a20 4d49 540a 5072 6f6a 6563 742d  se: MIT.Project-
-00000110: 5552 4c3a 204c 616e 6469 6e67 2070 6167  URL: Landing pag
-00000120: 652c 2068 7474 7073 3a2f 2f65 7273 696c  e, https://ersil
-00000130: 6961 2e69 6f0a 5072 6f6a 6563 742d 5552  ia.io.Project-UR
-00000140: 4c3a 204d 6f64 656c 732c 2068 7474 7073  L: Models, https
-00000150: 3a2f 2f65 7273 696c 6961 2e69 6f2f 6d6f  ://ersilia.io/mo
-00000160: 6465 6c2d 6875 620a 5072 6f6a 6563 742d  del-hub.Project-
-00000170: 5552 4c3a 2053 6f75 7263 6520 436f 6465  URL: Source Code
-00000180: 2c20 6874 7470 733a 2f2f 6769 7468 7562  , https://github
-00000190: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
-000001a0: 6572 7369 6c69 612f 0a44 6573 6372 6970  ersilia/.Descrip
-000001b0: 7469 6f6e 3a20 3c64 6976 2069 643d 2274  tion: <div id="t
-000001c0: 6f70 223e 3c2f 6469 763e 0a20 2020 2020  op"></div>.     
-000001d0: 2020 203c 696d 6720 7372 633d 2268 7474     <img src="htt
-000001e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001f0: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-00000200: 6961 2f62 6c6f 622f 6d61 7374 6572 2f61  ia/blob/master/a
-00000210: 7373 6574 732f 4572 7369 6c69 615f 506c  ssets/Ersilia_Pl
-00000220: 756d 2e70 6e67 2220 6865 6967 6874 3d22  um.png" height="
-00000230: 3730 223e 0a20 2020 2020 2020 200a 2020  70">.        .  
-00000240: 2020 2020 2020 2320 5765 6c63 6f6d 6520        # Welcome 
-00000250: 746f 2074 6865 2045 7273 696c 6961 204d  to the Ersilia M
-00000260: 6f64 656c 2048 7562 210a 2020 2020 2020  odel Hub!.      
-00000270: 2020 0a20 2020 2020 2020 205b 215b 446f    .        [![Do
-00000280: 6e61 7465 5d28 6874 7470 733a 2f2f 696d  nate](https://im
-00000290: 672e 7368 6965 6c64 732e 696f 2f62 6164  g.shields.io/bad
-000002a0: 6765 2f44 6f6e 6174 652d 5061 7950 616c  ge/Donate-PayPal
-000002b0: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
-000002c0: 7073 3a2f 2f77 7777 2e70 6179 7061 6c2e  ps://www.paypal.
-000002d0: 636f 6d2f 756b 2f66 756e 6472 6169 7365  com/uk/fundraise
-000002e0: 722f 6368 6172 6974 792f 3431 3435 3031  r/charity/414501
-000002f0: 3229 205b 215b 436f 6e74 7269 6275 746f  2) [![Contributo
-00000300: 7220 436f 7665 6e61 6e74 5d28 6874 7470  r Covenant](http
-00000310: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000320: 696f 2f62 6164 6765 2f43 6f6e 7472 6962  io/badge/Contrib
-00000330: 7574 6f72 2532 3043 6f76 656e 616e 742d  utor%20Covenant-
-00000340: 7632 2e30 2532 3061 646f 7074 6564 2d66  v2.0%20adopted-f
-00000350: 6636 3962 342e 7376 6729 5d28 434f 4445  f69b4.svg)](CODE
-00000360: 5f4f 465f 434f 4e44 5543 542e 6d64 2920  _OF_CONDUCT.md) 
-00000370: 5b21 5b4c 6963 656e 7365 3a20 4147 504c  [![License: AGPL
+000000e0: 722d 656d 6169 6c3a 2068 656c 6c6f 4065  r-email: hello@e
+000000f0: 7273 696c 6961 2e69 6f0a 4c69 6365 6e73  rsilia.io.Licens
+00000100: 653a 2047 504c 7633 0a50 726f 6a65 6374  e: GPLv3.Project
+00000110: 2d55 524c 3a20 4c61 6e64 696e 6720 7061  -URL: Landing pa
+00000120: 6765 2c20 6874 7470 733a 2f2f 6572 7369  ge, https://ersi
+00000130: 6c69 612e 696f 0a50 726f 6a65 6374 2d55  lia.io.Project-U
+00000140: 524c 3a20 4d6f 6465 6c73 2c20 6874 7470  RL: Models, http
+00000150: 733a 2f2f 6572 7369 6c69 612e 696f 2f6d  s://ersilia.io/m
+00000160: 6f64 656c 2d68 7562 0a50 726f 6a65 6374  odel-hub.Project
+00000170: 2d55 524c 3a20 536f 7572 6365 2043 6f64  -URL: Source Cod
+00000180: 652c 2068 7474 7073 3a2f 2f67 6974 6875  e, https://githu
+00000190: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+000001a0: 2f65 7273 696c 6961 2f0a 4465 7363 7269  /ersilia/.Descri
+000001b0: 7074 696f 6e3a 203c 6469 7620 6964 3d22  ption: <div id="
+000001c0: 746f 7022 3e3c 2f64 6976 3e0a 2020 2020  top"></div>.    
+000001d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
+000001e0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000001f0: 2f65 7273 696c 6961 2d6f 732f 6572 7369  /ersilia-os/ersi
+00000200: 6c69 612f 626c 6f62 2f6d 6173 7465 722f  lia/blob/master/
+00000210: 6173 7365 7473 2f45 7273 696c 6961 5f50  assets/Ersilia_P
+00000220: 6c75 6d2e 706e 6722 2068 6569 6768 743d  lum.png" height=
+00000230: 2237 3022 3e0a 2020 2020 2020 2020 0a20  "70">.        . 
+00000240: 2020 2020 2020 2023 2057 656c 636f 6d65         # Welcome
+00000250: 2074 6f20 7468 6520 4572 7369 6c69 6120   to the Ersilia 
+00000260: 4d6f 6465 6c20 4875 6221 0a20 2020 2020  Model Hub!.     
+00000270: 2020 200a 2020 2020 2020 2020 5b21 5b44     .        [![D
+00000280: 6f6e 6174 655d 2868 7474 7073 3a2f 2f69  onate](https://i
+00000290: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+000002a0: 6467 652f 446f 6e61 7465 2d50 6179 5061  dge/Donate-PayPa
+000002b0: 6c2d 6772 6565 6e2e 7376 6729 5d28 6874  l-green.svg)](ht
+000002c0: 7470 733a 2f2f 7777 772e 7061 7970 616c  tps://www.paypal
+000002d0: 2e63 6f6d 2f75 6b2f 6675 6e64 7261 6973  .com/uk/fundrais
+000002e0: 6572 2f63 6861 7269 7479 2f34 3134 3530  er/charity/41450
+000002f0: 3132 2920 5b21 5b43 6f6e 7472 6962 7574  12) [![Contribut
+00000300: 6f72 2043 6f76 656e 616e 745d 2868 7474  or Covenant](htt
+00000310: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000320: 2e69 6f2f 6261 6467 652f 436f 6e74 7269  .io/badge/Contri
+00000330: 6275 746f 7225 3230 436f 7665 6e61 6e74  butor%20Covenant
+00000340: 2d76 322e 3025 3230 6164 6f70 7465 642d  -v2.0%20adopted-
+00000350: 6666 3639 6234 2e73 7667 295d 2843 4f44  ff69b4.svg)](COD
+00000360: 455f 4f46 5f43 4f4e 4455 4354 2e6d 6429  E_OF_CONDUCT.md)
+00000370: 205b 215b 4c69 6365 6e73 653a 2047 504c   [![License: GPL
 00000380: 2076 335d 2868 7474 7073 3a2f 2f69 6d67   v3](https://img
 00000390: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
-000003a0: 652f 4c69 6365 6e73 652d 4147 504c 2532  e/License-AGPL%2
-000003b0: 3076 332d 7965 6c6c 6f77 2e73 7667 295d  0v3-yellow.svg)]
-000003c0: 2868 7474 7073 3a2f 2f77 7777 2e67 6e75  (https://www.gnu
-000003d0: 2e6f 7267 2f6c 6963 656e 7365 732f 6167  .org/licenses/ag
-000003e0: 706c 2d33 2e30 290a 2020 2020 2020 2020  pl-3.0).        
-000003f0: 0a20 2020 2020 2020 205b 215b 646f 6375  .        [![docu
-00000400: 6d65 6e74 6174 696f 6e5d 2868 7474 7073  mentation](https
-00000410: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
-00000420: 6f2f 6261 6467 652f 2d44 6f63 756d 656e  o/badge/-Documen
-00000430: 7461 7469 6f6e 2d70 7572 706c 653f 6c6f  tation-purple?lo
-00000440: 676f 3d72 6561 642d 7468 652d 646f 6373  go=read-the-docs
-00000450: 266c 6f67 6f43 6f6c 6f72 3d77 6869 7465  &logoColor=white
-00000460: 295d 2868 7474 7073 3a2f 2f65 7273 696c  )](https://ersil
-00000470: 6961 2e67 6974 626f 6f6b 2e69 6f2f 6572  ia.gitbook.io/er
-00000480: 7369 6c69 612d 626f 6f6b 2f29 205b 215b  silia-book/) [![
-00000490: 5079 5049 2076 6572 7369 6f6e 2066 7572  PyPI version fur
-000004a0: 792e 696f 5d28 6874 7470 733a 2f2f 6261  y.io](https://ba
-000004b0: 6467 652e 6675 7279 2e69 6f2f 7079 2f65  dge.fury.io/py/e
-000004c0: 7273 696c 6961 2e73 7667 295d 2868 7474  rsilia.svg)](htt
-000004d0: 7073 3a2f 2f70 7970 692e 7079 7468 6f6e  ps://pypi.python
-000004e0: 2e6f 7267 2f70 7970 692f 6572 7369 6c69  .org/pypi/ersili
-000004f0: 612f 2920 5b21 5b50 7974 686f 6e20 332e  a/) [![Python 3.
-00000500: 375d 2868 7474 7073 3a2f 2f69 6d67 2e73  7](https://img.s
-00000510: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
-00000520: 7079 7468 6f6e 2d33 2e37 2d62 6c75 652e  python-3.7-blue.
-00000530: 7376 6729 5d28 6874 7470 733a 2f2f 7777  svg)](https://ww
-00000540: 772e 7079 7468 6f6e 2e6f 7267 2f64 6f77  w.python.org/dow
-00000550: 6e6c 6f61 6473 2f72 656c 6561 7365 2f70  nloads/release/p
-00000560: 7974 686f 6e2d 3337 302f 2920 5b21 5b43  ython-370/) [![C
-00000570: 6f64 6520 7374 796c 653a 2062 6c61 636b  ode style: black
-00000580: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000590: 6965 6c64 732e 696f 2f62 6164 6765 2f63  ields.io/badge/c
-000005a0: 6f64 6525 3230 7374 796c 652d 626c 6163  ode%20style-blac
-000005b0: 6b2d 3030 3030 3030 2e73 7667 3f6c 6f67  k-000000.svg?log
-000005c0: 6f3d 5079 7468 6f6e 266c 6f67 6f43 6f6c  o=Python&logoCol
-000005d0: 6f72 3d77 6869 7465 295d 2868 7474 7073  or=white)](https
-000005e0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7073  ://github.com/ps
-000005f0: 662f 626c 6163 6b29 205b 215b 4769 7470  f/black) [![Gitp
-00000600: 6f64 2052 6561 6479 2d74 6f2d 436f 6465  od Ready-to-Code
-00000610: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000620: 6965 6c64 732e 696f 2f62 6164 6765 2f47  ields.io/badge/G
-00000630: 6974 706f 642d 7265 6164 792d 2d74 6f2d  itpod-ready--to-
-00000640: 2d63 6f64 652d 626c 7565 3f6c 6f67 6f3d  -code-blue?logo=
-00000650: 6769 7470 6f64 295d 2868 7474 7073 3a2f  gitpod)](https:/
-00000660: 2f67 6974 706f 642e 696f 2f23 6874 7470  /gitpod.io/#http
-00000670: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-00000680: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
-00000690: 6129 0a20 2020 2020 2020 200a 2020 2020  a).        .    
-000006a0: 2020 2020 2323 2320 5461 626c 6520 6f66      ### Table of
-000006b0: 2043 6f6e 7465 6e74 733a 0a20 2020 2020   Contents:.     
-000006c0: 2020 2031 2e20 5b50 726f 6a65 6374 2044     1. [Project D
-000006d0: 6573 6372 6970 7469 6f6e 5d28 6874 7470  escription](http
-000006e0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
-000006f0: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
-00000700: 6123 7072 6f6a 6563 742d 6465 7363 7269  a#project-descri
-00000710: 7074 696f 6e29 0a20 2020 2020 2020 2032  ption).        2
-00000720: 2e20 5b49 6e73 7461 6c6c 6174 696f 6e5d  . [Installation]
-00000730: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000740: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
-00000750: 7273 696c 6961 2369 6e73 7461 6c6c 6174  rsilia#installat
-00000760: 696f 6e29 0a20 2020 2020 2020 2033 2e20  ion).        3. 
-00000770: 5b43 6f6e 7472 6962 7574 655d 2868 7474  [Contribute](htt
-00000780: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00000790: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-000007a0: 6961 2363 6f6e 7472 6962 7574 6529 0a20  ia#contribute). 
-000007b0: 2020 2020 2020 2034 2e20 5b4c 6963 656e         4. [Licen
-000007c0: 7365 2061 6e64 2063 6974 6174 696f 6e5d  se and citation]
-000007d0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000007e0: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
-000007f0: 7273 696c 6961 236c 6963 656e 7365 2d61  rsilia#license-a
-00000800: 6e64 2d63 6974 6174 696f 6e29 0a20 2020  nd-citation).   
-00000810: 2020 2020 2035 2e20 5b41 626f 7574 2075       5. [About u
-00000820: 735d 2868 7474 7073 3a2f 2f67 6974 6875  s](https://githu
-00000830: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
-00000840: 2f65 7273 696c 6961 2361 626f 7574 2d75  /ersilia#about-u
-00000850: 7329 0a20 2020 2020 2020 200a 2020 2020  s).        .    
-00000860: 2020 2020 2320 5072 6f6a 6563 7420 4465      # Project De
-00000870: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
-00000880: 2020 5468 6520 4572 7369 6c69 6120 4d6f    The Ersilia Mo
-00000890: 6465 6c20 4875 6220 6973 2061 2075 6e69  del Hub is a uni
-000008a0: 6669 6564 2070 6c61 7466 6f72 6d20 6f66  fied platform of
-000008b0: 2070 7265 2d74 7261 696e 6564 2041 492f   pre-trained AI/
-000008c0: 4d4c 206d 6f64 656c 7320 666f 7220 696e  ML models for in
-000008d0: 6665 6374 696f 7573 2061 6e64 206e 6567  fectious and neg
-000008e0: 6c65 6374 6564 2064 6973 6561 7365 2072  lected disease r
-000008f0: 6573 6561 7263 682e 2054 6865 2065 6e64  esearch. The end
-00000900: 2067 6f61 6c20 6973 2074 6f20 7072 6f76   goal is to prov
-00000910: 6964 6520 616e 206f 7065 6e2d 736f 7572  ide an open-sour
-00000920: 6365 2c20 6e6f 2d63 6f64 6520 736f 6c75  ce, no-code solu
-00000930: 7469 6f6e 2074 6f20 6163 6365 7373 2041  tion to access A
-00000940: 492f 4d4c 206d 6f64 656c 7320 746f 2061  I/ML models to a
-00000950: 6363 656c 6572 6174 6520 6472 7567 2064  ccelerate drug d
-00000960: 6973 636f 7665 7279 2e20 5468 6520 6d6f  iscovery. The mo
-00000970: 6465 6c73 2065 6d62 6564 6465 6420 696e  dels embedded in
-00000980: 2074 6865 2068 7562 2069 6e63 6c75 6465   the hub include
-00000990: 2062 6f74 6820 6d6f 6465 6c73 2070 7562   both models pub
-000009a0: 6c69 7368 6564 2069 6e20 7468 6520 6c69  lished in the li
-000009b0: 7465 7261 7475 7265 2028 7769 7468 2061  terature (with a
-000009c0: 7070 726f 7072 6961 7465 2074 6869 7264  ppropriate third
-000009d0: 2070 6172 7479 2061 636b 6e6f 776c 6564   party acknowled
-000009e0: 6765 6d65 6e74 2920 616e 6420 6d6f 6465  gement) and mode
-000009f0: 6c73 2064 6576 656c 6f70 6564 2062 7920  ls developed by 
-00000a00: 7468 6520 4572 7369 6c69 6120 7465 616d  the Ersilia team
-00000a10: 206f 7220 636f 6e74 7269 6275 746f 7273   or contributors
-00000a20: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00000a30: 2020 202a 2052 6561 6420 6d6f 7265 2061     * Read more a
-00000a40: 626f 7574 2074 6865 2070 726f 6a65 6374  bout the project
-00000a50: 2069 6e20 7468 6520 5b45 7273 696c 6961   in the [Ersilia
-00000a60: 2042 6f6f 6b5d 2868 7474 7073 3a2f 2f65   Book](https://e
-00000a70: 7273 696c 6961 2e67 6974 626f 6f6b 2e69  rsilia.gitbook.i
-00000a80: 6f2f 6572 7369 6c69 612d 626f 6f6b 2f29  o/ersilia-book/)
-00000a90: 0a20 2020 2020 2020 202a 2042 726f 7773  .        * Brows
-00000aa0: 6520 6176 6169 6c61 626c 6520 6d6f 6465  e available mode
-00000ab0: 6c73 2069 6e20 7468 6520 5b45 7273 696c  ls in the [Ersil
-00000ac0: 6961 204d 6f64 656c 2048 7562 5d28 6874  ia Model Hub](ht
-00000ad0: 7470 733a 2f2f 6572 7369 6c69 612e 696f  tps://ersilia.io
-00000ae0: 2f6d 6f64 656c 2d68 7562 2f29 0a20 2020  /model-hub/).   
-00000af0: 2020 2020 203c 7020 616c 6967 6e3d 2272       <p align="r
-00000b00: 6967 6874 223e 283c 6120 6872 6566 3d22  ight">(<a href="
-00000b10: 2374 6f70 223e 6261 636b 2074 6f20 746f  #top">back to to
-00000b20: 703c 2f61 3e29 3c2f 703e 0a20 2020 2020  p</a>)</p>.     
-00000b30: 2020 200a 2020 2020 2020 2020 2320 5175     .        # Qu
-00000b40: 6963 6b20 7374 6172 7420 6775 6964 650a  ick start guide.
-00000b50: 2020 2020 2020 2020 506c 6561 7365 2063          Please c
-00000b60: 6865 636b 2074 6865 2070 6163 6b61 6765  heck the package
-00000b70: 2072 6571 7569 7265 6d65 6e74 7320 696e   requirements in
-00000b80: 2074 6865 205b 496e 7374 616c 6c61 7469   the [Installati
-00000b90: 6f6e 2047 7569 6465 5d28 6874 7470 733a  on Guide](https:
-00000ba0: 2f2f 6572 7369 6c69 612e 6769 7462 6f6f  //ersilia.gitboo
-00000bb0: 6b2e 696f 2f65 7273 696c 6961 2d62 6f6f  k.io/ersilia-boo
-00000bc0: 6b2f 7175 6963 6b2d 7374 6172 742f 696e  k/quick-start/in
-00000bd0: 7374 616c 6c61 7469 6f6e 292e 2054 6865  stallation). The
-00000be0: 206e 6578 7420 7374 6570 7320 6172 6520   next steps are 
-00000bf0: 6120 7175 6963 6b73 7461 7274 2067 7569  a quickstart gui
-00000c00: 6465 2074 6f20 696e 7374 616c 6c69 6e67  de to installing
-00000c10: 2045 7273 696c 6961 2e0a 2020 2020 2020   Ersilia..      
-00000c20: 2020 0a20 2020 2020 2020 2031 2e20 4372    .        1. Cr
-00000c30: 6561 7465 2061 2063 6f6e 6461 2065 6e76  eate a conda env
-00000c40: 6972 6f6e 6d65 6e74 2061 6e64 2061 6374  ironment and act
-00000c50: 6976 6174 6520 6974 0a20 2020 2020 2020  ivate it.       
-00000c60: 2060 6060 0a20 2020 2020 2020 2063 6f6e   ```.        con
-00000c70: 6461 2063 7265 6174 6520 2d6e 2065 7273  da create -n ers
-00000c80: 696c 6961 2070 7974 686f 6e3d 332e 370a  ilia python=3.7.
-00000c90: 2020 2020 2020 2020 636f 6e64 6120 6163          conda ac
-00000ca0: 7469 7661 7465 2065 7273 696c 6961 0a20  tivate ersilia. 
-00000cb0: 2020 2020 2020 2060 6060 0a20 2020 2020         ```.     
-00000cc0: 2020 2032 2e20 436c 6f6e 6520 7468 6973     2. Clone this
-00000cd0: 2072 6570 6f73 6974 6f72 7920 616e 6420   repository and 
-00000ce0: 696e 7374 616c 6c20 7769 7468 2070 6970  install with pip
-00000cf0: 0a20 2020 2020 2020 2060 6060 0a20 2020  .        ```.   
-00000d00: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
-00000d10: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000d20: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
-00000d30: 696c 6961 2e67 6974 0a20 2020 2020 2020  ilia.git.       
-00000d40: 2063 6420 6572 7369 6c69 610a 2020 2020   cd ersilia.    
-00000d50: 2020 2020 7069 7020 696e 7374 616c 6c20      pip install 
-00000d60: 2d65 202e 0a20 2020 2020 2020 2060 6060  -e ..        ```
-00000d70: 200a 2020 2020 2020 2020 332e 204f 6e63   .        3. Onc
-00000d80: 6520 7468 6520 4572 7369 6c69 6120 4d6f  e the Ersilia Mo
-00000d90: 6465 6c20 4875 6220 6973 2069 6e73 7461  del Hub is insta
-00000da0: 6c6c 6564 2c20 796f 7520 6361 6e20 7573  lled, you can us
-00000db0: 6520 7468 6520 434c 4920 746f 2072 756e  e the CLI to run
-00000dc0: 2070 7265 6469 6374 696f 6e73 2e20 4669   predictions. Fi
-00000dd0: 7273 742c 2073 656c 6563 7420 6120 6d6f  rst, select a mo
-00000de0: 6465 6c20 6672 6f6d 2074 6865 205b 4572  del from the [Er
-00000df0: 7369 6c69 6120 4d6f 6465 6c20 4875 625d  silia Model Hub]
-00000e00: 2868 7474 7073 3a2f 2f65 7273 696c 6961  (https://ersilia
-00000e10: 2e69 6f2f 6d6f 6465 6c2d 6875 622f 2920  .io/model-hub/) 
-00000e20: 616e 6420 2a2a 6665 7463 682a 2a20 6974  and **fetch** it
-00000e30: 3a0a 2020 2020 2020 2020 6060 600a 2020  :.        ```.  
-00000e40: 2020 2020 2020 6572 7369 6c69 6120 6665        ersilia fe
-00000e50: 7463 6820 6368 656d 7072 6f70 2d61 6e74  tch chemprop-ant
-00000e60: 6962 696f 7469 630a 2020 2020 2020 2020  ibiotic.        
-00000e70: 6060 600a 2020 2020 2020 2020 342e 2047  ```.        4. G
-00000e80: 656e 6572 6174 6520 6120 6665 7720 2835  enerate a few (5
-00000e90: 2920 6578 616d 706c 6520 6d6f 6c65 6375  ) example molecu
-00000ea0: 6c65 732c 2074 6f20 6265 2075 7365 6420  les, to be used 
-00000eb0: 6173 2069 6e70 7574 2e20 5468 6520 2a2a  as input. The **
-00000ec0: 6578 616d 706c 652a 2a20 636f 6d6d 616e  example** comman
-00000ed0: 6420 7769 6c6c 2067 656e 6572 6174 6520  d will generate 
-00000ee0: 7468 6520 6164 6571 7561 7465 2069 6e70  the adequate inp
-00000ef0: 7574 2066 6f72 2074 6865 206d 6f64 656c  ut for the model
-00000f00: 2069 6e20 7573 650a 2020 2020 2020 2020   in use.        
-00000f10: 6060 600a 2020 2020 2020 2020 6572 7369  ```.        ersi
-00000f20: 6c69 6120 6578 616d 706c 6520 6368 656d  lia example chem
-00000f30: 7072 6f70 2d61 6e74 6962 696f 7469 6320  prop-antibiotic 
-00000f40: 2d6e 2035 202d 6620 6d79 5f6d 6f6c 6563  -n 5 -f my_molec
-00000f50: 756c 6573 2e63 7376 0a20 2020 2020 2020  ules.csv.       
-00000f60: 2060 6060 0a20 2020 2020 2020 2035 2e20   ```.        5. 
-00000f70: 5468 656e 2c20 2a2a 7365 7276 652a 2a20  Then, **serve** 
-00000f80: 796f 7572 206d 6f64 656c 3a0a 2020 2020  your model:.    
-00000f90: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-00000fa0: 6572 7369 6c69 6120 7365 7276 6520 6368  ersilia serve ch
-00000fb0: 656d 7072 6f70 2d61 6e74 6962 696f 7469  emprop-antibioti
-00000fc0: 630a 2020 2020 2020 2020 6060 600a 2020  c.        ```.  
-00000fd0: 2020 2020 2020 362e 2041 6e64 2072 756e        6. And run
-00000fe0: 2074 6865 2070 7265 6469 6374 696f 6e20   the prediction 
-00000ff0: 2a2a 4150 492a 2a3a 0a20 2020 2020 2020  **API**:.       
-00001000: 2060 6060 0a20 2020 2020 2020 2065 7273   ```.        ers
-00001010: 696c 6961 2061 7069 202d 6920 6d79 5f6d  ilia api -i my_m
-00001020: 6f6c 6563 756c 6573 2e63 7376 202d 6f20  olecules.csv -o 
-00001030: 6d79 5f70 7265 6469 6374 696f 6e73 2e63  my_predictions.c
-00001040: 7376 0a20 2020 2020 2020 2060 6060 0a20  sv.        ```. 
-00001050: 2020 2020 2020 2037 2e20 4669 6e61 6c6c         7. Finall
-00001060: 792c 202a 2a63 6c6f 7365 2a2a 2074 6865  y, **close** the
-00001070: 2073 6572 7669 6365 2077 6865 6e20 796f   service when yo
-00001080: 7520 6172 6520 646f 6e65 2e0a 2020 2020  u are done..    
-00001090: 2020 2020 6060 600a 2020 2020 2020 2020      ```.        
-000010a0: 6572 7369 6c69 6120 636c 6f73 650a 2020  ersilia close.  
-000010b0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
-000010c0: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
-000010d0: 6520 7365 6520 7468 6520 5b45 7273 696c  e see the [Ersil
-000010e0: 6961 2042 6f6f 6b5d 2868 7474 7073 3a2f  ia Book](https:/
-000010f0: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
-00001100: 2e69 6f2f 6572 7369 6c69 612d 626f 6f6b  .io/ersilia-book
-00001110: 2f29 2066 6f72 206d 6f72 6520 6578 616d  /) for more exam
-00001120: 706c 6573 2061 6e64 2064 6574 6169 6c65  ples and detaile
-00001130: 6420 6578 706c 616e 6174 696f 6e73 2e0a  d explanations..
-00001140: 2020 2020 2020 2020 3c70 2061 6c69 676e          <p align
-00001150: 3d22 7269 6768 7422 3e28 3c61 2068 7265  ="right">(<a hre
-00001160: 663d 2223 746f 7022 3e62 6163 6b20 746f  f="#top">back to
-00001170: 2074 6f70 3c2f 613e 293c 2f70 3e0a 2020   top</a>)</p>.  
-00001180: 2020 2020 2020 0a20 2020 2020 2020 2023        .        #
-00001190: 2043 6f6e 7472 6962 7574 650a 2020 2020   Contribute.    
-000011a0: 2020 2020 5468 6520 4572 7369 6c69 6120      The Ersilia 
-000011b0: 4d6f 6465 6c20 4875 6220 6973 2061 2046  Model Hub is a F
-000011c0: 7265 652c 204f 7065 6e20 536f 7572 6365  ree, Open Source
-000011d0: 2053 6f66 7477 6172 6520 616e 6420 7765   Software and we
-000011e0: 2068 6967 686c 7920 7661 6c75 6520 6e65   highly value ne
-000011f0: 7720 636f 6e74 7269 6275 746f 7273 2e20  w contributors. 
-00001200: 5468 6572 6520 6172 6520 7365 7665 7261  There are severa
-00001210: 6c20 7761 7973 2069 6e20 7768 6963 6820  l ways in which 
-00001220: 796f 7520 6361 6e20 636f 6e74 7269 6275  you can contribu
-00001230: 7465 2074 6f20 7468 6520 7072 6f6a 6563  te to the projec
-00001240: 743a 0a20 2020 2020 2020 202a 2041 2067  t:.        * A g
-00001250: 6f6f 6420 706c 6163 6520 746f 2073 7461  ood place to sta
-00001260: 7274 2069 7320 6368 6563 6b69 6e67 206f  rt is checking o
-00001270: 7065 6e20 5b69 7373 7565 735d 2868 7474  pen [issues](htt
-00001280: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001290: 6572 7369 6c69 612d 6f73 2f65 7273 696c  ersilia-os/ersil
-000012a0: 6961 2f69 7373 7565 7329 2e20 0a20 2020  ia/issues). .   
-000012b0: 2020 2020 202a 2049 6620 796f 7520 6861       * If you ha
-000012c0: 7665 2069 6465 6e74 6966 6965 6420 6120  ve identified a 
-000012d0: 6275 6720 696e 2074 6865 2063 6f64 652c  bug in the code,
-000012e0: 2070 6c65 6173 6520 6f70 656e 2061 206e   please open a n
-000012f0: 6577 2069 7373 7565 2075 7369 6e67 2074  ew issue using t
-00001300: 6865 2062 7567 2074 656d 706c 6174 652e  he bug template.
-00001310: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
-00001320: 7520 7761 6e74 2074 6f20 696e 636f 7270  u want to incorp
-00001330: 6f72 6174 6520 6120 6e65 7720 6d6f 6465  orate a new mode
-00001340: 6c20 696e 2074 6865 2070 6c61 7466 6f72  l in the platfor
-00001350: 6d2c 206f 7065 6e20 6120 6e65 7720 6973  m, open a new is
-00001360: 7375 6520 7573 696e 6720 7468 6520 6d6f  sue using the mo
-00001370: 6465 6c20 7265 7175 6573 7420 7465 6d70  del request temp
-00001380: 6c61 7465 206f 7220 636f 6e74 6163 7420  late or contact 
-00001390: 7573 2075 7369 6e67 2074 6865 2066 6f6c  us using the fol
-000013a0: 6c6f 7769 6e67 205b 666f 726d 5d28 6874  lowing [form](ht
-000013b0: 7470 733a 2f2f 7777 772e 6572 7369 6c69  tps://www.ersili
-000013c0: 612e 696f 2f72 6571 7565 7374 2d6d 6f64  a.io/request-mod
-000013d0: 656c 290a 2020 2020 2020 2020 2a20 5368  el).        * Sh
-000013e0: 6172 6520 616e 7920 6665 6564 6261 636b  are any feedback
-000013f0: 2077 6974 6820 7468 6520 636f 6d6d 756e   with the commun
-00001400: 6974 7920 7573 696e 6720 5b47 6974 4875  ity using [GitHu
-00001410: 6220 4469 7363 7573 7369 6f6e 735d 2868  b Discussions](h
-00001420: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001430: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
-00001440: 696c 6961 2f64 6973 6375 7373 696f 6e73  ilia/discussions
-00001450: 2920 666f 7220 7468 6520 7072 6f6a 6563  ) for the projec
-00001460: 740a 2020 2020 2020 2020 2a20 4368 6563  t.        * Chec
-00001470: 6b20 6f75 7220 5b43 6f6e 7472 6962 7574  k our [Contribut
-00001480: 696e 6720 4775 6964 655d 2868 7474 7073  ing Guide](https
-00001490: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
-000014a0: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
-000014b0: 2f62 6c6f 622f 6d61 7374 6572 2f43 4f4e  /blob/master/CON
-000014c0: 5452 4942 5554 494e 472e 6d64 2920 666f  TRIBUTING.md) fo
-000014d0: 7220 6d6f 7265 2064 6574 6169 6c73 0a20  r more details. 
-000014e0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-000014f0: 5468 6520 4572 7369 6c69 6120 4f70 656e  The Ersilia Open
-00001500: 2053 6f75 7263 6520 496e 6974 6961 7469   Source Initiati
-00001510: 7665 2061 6468 6572 6573 2074 6f20 7468  ve adheres to th
-00001520: 6520 5b43 6f6e 7472 6962 7574 6f72 2043  e [Contributor C
-00001530: 6f76 656e 616e 745d 2868 7474 7073 3a2f  ovenant](https:/
-00001540: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
-00001550: 2e69 6f2f 6572 7369 6c69 612d 7769 6b69  .io/ersilia-wiki
-00001560: 2f63 6f64 652d 6f66 2d63 6f6e 6475 6374  /code-of-conduct
-00001570: 2920 636f 6465 206f 6620 636f 6e64 7563  ) code of conduc
-00001580: 742e 0a20 2020 2020 2020 203c 7020 616c  t..        <p al
-00001590: 6967 6e3d 2272 6967 6874 223e 283c 6120  ign="right">(<a 
-000015a0: 6872 6566 3d22 2374 6f70 223e 6261 636b  href="#top">back
-000015b0: 2074 6f20 746f 703c 2f61 3e29 3c2f 703e   to top</a>)</p>
-000015c0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-000015d0: 2020 2320 4c69 6365 6e73 6520 616e 6420    # License and 
-000015e0: 6369 7461 7469 6f6e 0a20 2020 2020 2020  citation.       
-000015f0: 2054 6869 7320 7265 706f 7369 746f 7279   This repository
-00001600: 2069 7320 6f70 656e 2d73 6f75 7263 6564   is open-sourced
-00001610: 2075 6e64 6572 2074 6865 205b 4750 4c2d   under the [GPL-
-00001620: 3320 4c69 6365 6e73 655d 2868 7474 7073  3 License](https
-00001630: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
-00001640: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
-00001650: 2f62 6c6f 622f 6d61 7374 6572 2f4c 4943  /blob/master/LIC
-00001660: 454e 5345 292e 0a20 2020 2020 2020 2050  ENSE)..        P
-00001670: 6c65 6173 6520 5b63 6974 6520 7573 5d28  lease [cite us](
-00001680: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001690: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
-000016a0: 7369 6c69 612f 626c 6f62 2f6d 6173 7465  silia/blob/maste
-000016b0: 722f 4349 5441 5449 4f4e 2e63 6666 2920  r/CITATION.cff) 
-000016c0: 6966 2079 6f75 2075 7365 2069 742e 0a20  if you use it.. 
-000016d0: 2020 2020 2020 203c 7020 616c 6967 6e3d         <p align=
-000016e0: 2272 6967 6874 223e 283c 6120 6872 6566  "right">(<a href
-000016f0: 3d22 2374 6f70 223e 6261 636b 2074 6f20  ="#top">back to 
-00001700: 746f 703c 2f61 3e29 3c2f 703e 0a20 2020  top</a>)</p>.   
-00001710: 2020 2020 200a 2020 2020 2020 2020 2320       .        # 
-00001720: 4162 6f75 7420 7573 0a20 2020 2020 2020  About us.       
-00001730: 2054 6865 205b 4572 7369 6c69 6120 4f70   The [Ersilia Op
-00001740: 656e 2053 6f75 7263 6520 496e 6974 6961  en Source Initia
-00001750: 7469 7665 5d28 6874 7470 733a 2f2f 6572  tive](https://er
-00001760: 7369 6c69 612e 696f 2920 6973 2061 204e  silia.io) is a N
-00001770: 6f6e 2050 726f 6669 7420 4f72 6761 6e69  on Profit Organi
-00001780: 7a61 7469 6f6e 2028 5b31 3139 3232 3636  zation ([1192266
-00001790: 5d28 6874 7470 733a 2f2f 7265 6769 7374  ](https://regist
-000017a0: 6572 2d6f 662d 6368 6172 6974 6965 732e  er-of-charities.
-000017b0: 6368 6172 6974 7963 6f6d 6d69 7373 696f  charitycommissio
-000017c0: 6e2e 676f 762e 756b 2f63 6861 7269 7479  n.gov.uk/charity
-000017d0: 2d73 6561 7263 682f 2d2f 6368 6172 6974  -search/-/charit
-000017e0: 792d 6465 7461 696c 732f 3531 3730 3635  y-details/517065
-000017f0: 372f 6675 6c6c 2d70 7269 6e74 2929 2077  7/full-print)) w
-00001800: 6974 6820 7468 6520 6d69 7373 696f 6e20  ith the mission 
-00001810: 6973 2074 6f20 6571 7569 7020 6c61 6273  is to equip labs
-00001820: 2c20 756e 6976 6572 7369 7469 6573 2061  , universities a
-00001830: 6e64 2063 6c69 6e69 6373 2069 6e20 4c4d  nd clinics in LM
-00001840: 4943 2077 6974 6820 4149 2f4d 4c20 746f  IC with AI/ML to
-00001850: 6f6c 7320 666f 7220 696e 6665 6374 696f  ols for infectio
-00001860: 7573 2064 6973 6561 7365 2072 6573 6561  us disease resea
-00001870: 7263 682e 0a20 2020 2020 2020 200a 2020  rch..        .  
-00001880: 2020 2020 2020 5b48 656c 7020 7573 5d28        [Help us](
-00001890: 6874 7470 733a 2f2f 7777 772e 6572 7369  https://www.ersi
-000018a0: 6c69 612e 696f 2f64 6f6e 6174 6529 2061  lia.io/donate) a
-000018b0: 6368 6965 7665 206f 7572 206d 6973 7369  chieve our missi
-000018c0: 6f6e 206f 7220 5b76 6f6c 756e 7465 6572  on or [volunteer
-000018d0: 5d28 6874 7470 733a 2f2f 7777 772e 6572  ](https://www.er
-000018e0: 7369 6c69 612e 696f 2f76 6f6c 756e 7465  silia.io/volunte
-000018f0: 6572 2920 7769 7468 2075 7321 0a20 2020  er) with us!.   
-00001900: 2020 2020 200a 2020 2020 2020 2020 3c70       .        <p
-00001910: 2061 6c69 676e 3d22 7269 6768 7422 3e28   align="right">(
-00001920: 3c61 2068 7265 663d 2223 746f 7022 3e62  <a href="#top">b
-00001930: 6163 6b20 746f 2074 6f70 3c2f 613e 293c  ack to top</a>)<
-00001940: 2f70 3e0a 2020 2020 2020 2020 0a4b 6579  /p>.        .Key
-00001950: 776f 7264 733a 2064 7275 672d 6469 7363  words: drug-disc
-00001960: 6f76 6572 7920 6d61 6368 696e 652d 6c65  overy machine-le
-00001970: 6172 6e69 6e67 2065 7273 696c 6961 206f  arning ersilia o
-00001980: 7065 6e2d 7363 6965 6e63 6520 676c 6f62  pen-science glob
-00001990: 616c 2d68 6561 6c74 6820 6d6f 6465 6c2d  al-health model-
-000019a0: 6875 6220 696e 6665 6374 696f 7573 2d64  hub infectious-d
-000019b0: 6973 6561 7365 730a 506c 6174 666f 726d  iseases.Platform
-000019c0: 3a20 554e 4b4e 4f57 4e0a 436c 6173 7369  : UNKNOWN.Classi
-000019d0: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-000019e0: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-000019f0: 7468 6f6e 203a 3a20 332e 370a 436c 6173  thon :: 3.7.Clas
-00001a00: 7369 6669 6572 3a20 4c69 6365 6e73 6520  sifier: License 
-00001a10: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00001a20: 3a3a 204d 4954 204c 6963 656e 7365 0a43  :: MIT License.C
-00001a30: 6c61 7373 6966 6965 723a 204f 7065 7261  lassifier: Opera
-00001a40: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-00001a50: 5320 496e 6465 7065 6e64 656e 740a 436c  S Independent.Cl
-00001a60: 6173 7369 6669 6572 3a20 546f 7069 6320  assifier: Topic 
-00001a70: 3a3a 2053 6369 656e 7469 6669 632f 456e  :: Scientific/En
-00001a80: 6769 6e65 6572 696e 6720 3a3a 2041 7274  gineering :: Art
-00001a90: 6966 6963 6961 6c20 496e 7465 6c6c 6967  ificial Intellig
-00001aa0: 656e 6365 0a52 6571 7569 7265 732d 5079  ence.Requires-Py
-00001ab0: 7468 6f6e 3a20 3e3d 332e 370a 4465 7363  thon: >=3.7.Desc
-00001ac0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-00001ad0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00001ae0: 6f77 6e0a 5072 6f76 6964 6573 2d45 7874  own.Provides-Ext
-00001af0: 7261 3a20 646f 635f 6275 696c 6465 720a  ra: doc_builder.
-00001b00: 5072 6f76 6964 6573 2d45 7874 7261 3a20  Provides-Extra: 
-00001b10: 7465 7374 0a50 726f 7669 6465 732d 4578  test.Provides-Ex
-00001b20: 7472 613a 2064 6576 0a                   tra: dev.
+000003a0: 652f 4c69 6365 6e73 652d 4750 4c25 3230  e/License-GPL%20
+000003b0: 7633 2d79 656c 6c6f 772e 7376 6729 5d28  v3-yellow.svg)](
+000003c0: 6874 7470 733a 2f2f 7777 772e 676e 752e  https://www.gnu.
+000003d0: 6f72 672f 6c69 6365 6e73 6573 2f61 6770  org/licenses/agp
+000003e0: 6c2d 332e 3029 205b 215b 444f 495d 2868  l-3.0) [![DOI](h
+000003f0: 7474 7073 3a2f 2f7a 656e 6f64 6f2e 6f72  ttps://zenodo.or
+00000400: 672f 6261 6467 652f 3237 3730 3638 3938  g/badge/27706898
+00000410: 392e 7376 6729 5d28 6874 7470 733a 2f2f  9.svg)](https://
+00000420: 7a65 6e6f 646f 2e6f 7267 2f62 6164 6765  zenodo.org/badge
+00000430: 2f6c 6174 6573 7464 6f69 2f32 3737 3036  /latestdoi/27706
+00000440: 3839 3839 290a 2020 2020 2020 2020 0a20  8989).        . 
+00000450: 2020 2020 2020 205b 215b 646f 6375 6d65         [![docume
+00000460: 6e74 6174 696f 6e5d 2868 7474 7073 3a2f  ntation](https:/
+00000470: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000480: 6261 6467 652f 2d44 6f63 756d 656e 7461  badge/-Documenta
+00000490: 7469 6f6e 2d70 7572 706c 653f 6c6f 676f  tion-purple?logo
+000004a0: 3d72 6561 642d 7468 652d 646f 6373 266c  =read-the-docs&l
+000004b0: 6f67 6f43 6f6c 6f72 3d77 6869 7465 295d  ogoColor=white)]
+000004c0: 2868 7474 7073 3a2f 2f65 7273 696c 6961  (https://ersilia
+000004d0: 2e67 6974 626f 6f6b 2e69 6f2f 6572 7369  .gitbook.io/ersi
+000004e0: 6c69 612d 626f 6f6b 2f29 205b 215b 5079  lia-book/) [![Py
+000004f0: 5049 2076 6572 7369 6f6e 2066 7572 792e  PI version fury.
+00000500: 696f 5d28 6874 7470 733a 2f2f 6261 6467  io](https://badg
+00000510: 652e 6675 7279 2e69 6f2f 7079 2f65 7273  e.fury.io/py/ers
+00000520: 696c 6961 2e73 7667 295d 2868 7474 7073  ilia.svg)](https
+00000530: 3a2f 2f70 7970 692e 7079 7468 6f6e 2e6f  ://pypi.python.o
+00000540: 7267 2f70 7970 692f 6572 7369 6c69 612f  rg/pypi/ersilia/
+00000550: 2920 5b21 5b50 7974 686f 6e20 332e 375d  ) [![Python 3.7]
+00000560: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000570: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00000580: 7468 6f6e 2d33 2e37 2d62 6c75 652e 7376  thon-3.7-blue.sv
+00000590: 6729 5d28 6874 7470 733a 2f2f 7777 772e  g)](https://www.
+000005a0: 7079 7468 6f6e 2e6f 7267 2f64 6f77 6e6c  python.org/downl
+000005b0: 6f61 6473 2f72 656c 6561 7365 2f70 7974  oads/release/pyt
+000005c0: 686f 6e2d 3337 302f 2920 5b21 5b43 6f64  hon-370/) [![Cod
+000005d0: 6520 7374 796c 653a 2062 6c61 636b 5d28  e style: black](
+000005e0: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+000005f0: 6c64 732e 696f 2f62 6164 6765 2f63 6f64  lds.io/badge/cod
+00000600: 6525 3230 7374 796c 652d 626c 6163 6b2d  e%20style-black-
+00000610: 3030 3030 3030 2e73 7667 3f6c 6f67 6f3d  000000.svg?logo=
+00000620: 5079 7468 6f6e 266c 6f67 6f43 6f6c 6f72  Python&logoColor
+00000630: 3d77 6869 7465 295d 2868 7474 7073 3a2f  =white)](https:/
+00000640: 2f67 6974 6875 622e 636f 6d2f 7073 662f  /github.com/psf/
+00000650: 626c 6163 6b29 205b 215b 4769 7470 6f64  black) [![Gitpod
+00000660: 2052 6561 6479 2d74 6f2d 436f 6465 5d28   Ready-to-Code](
+00000670: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000680: 6c64 732e 696f 2f62 6164 6765 2f47 6974  lds.io/badge/Git
+00000690: 706f 642d 7265 6164 792d 2d74 6f2d 2d63  pod-ready--to--c
+000006a0: 6f64 652d 626c 7565 3f6c 6f67 6f3d 6769  ode-blue?logo=gi
+000006b0: 7470 6f64 295d 2868 7474 7073 3a2f 2f67  tpod)](https://g
+000006c0: 6974 706f 642e 696f 2f23 6874 7470 733a  itpod.io/#https:
+000006d0: 2f2f 6769 7468 7562 2e63 6f6d 2f65 7273  //github.com/ers
+000006e0: 696c 6961 2d6f 732f 6572 7369 6c69 6129  ilia-os/ersilia)
+000006f0: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00000700: 2020 2323 2054 6162 6c65 206f 6620 436f    ## Table of Co
+00000710: 6e74 656e 7473 0a20 2020 2020 2020 200a  ntents.        .
+00000720: 2020 2020 2020 2020 312e 205b 5072 6f6a          1. [Proj
+00000730: 6563 7420 4465 7363 7269 7074 696f 6e5d  ect Description]
+00000740: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000750: 636f 6d2f 6572 7369 6c69 612d 6f73 2f65  com/ersilia-os/e
+00000760: 7273 696c 6961 2370 726f 6a65 6374 2d64  rsilia#project-d
+00000770: 6573 6372 6970 7469 6f6e 290a 2020 2020  escription).    
+00000780: 2020 2020 322e 205b 5175 6963 6b20 7374      2. [Quick st
+00000790: 6172 7420 6775 6964 655d 2868 7474 7073  art guide](https
+000007a0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6572  ://github.com/er
+000007b0: 7369 6c69 612d 6f73 2f65 7273 696c 6961  silia-os/ersilia
+000007c0: 2371 7569 636b 2d73 7461 7274 2d67 7569  #quick-start-gui
+000007d0: 6465 290a 2020 2020 2020 2020 332e 205b  de).        3. [
+000007e0: 436f 6e74 7269 6275 7465 5d28 6874 7470  Contribute](http
+000007f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00000800: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
+00000810: 6123 636f 6e74 7269 6275 7465 290a 2020  a#contribute).  
+00000820: 2020 2020 2020 342e 205b 4c69 6365 6e73        4. [Licens
+00000830: 6520 616e 6420 6369 7461 7469 6f6e 5d28  e and citation](
+00000840: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00000850: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
+00000860: 7369 6c69 6123 6c69 6365 6e73 652d 616e  silia#license-an
+00000870: 642d 6369 7461 7469 6f6e 290a 2020 2020  d-citation).    
+00000880: 2020 2020 352e 205b 4162 6f75 7420 7573      5. [About us
+00000890: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000008a0: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+000008b0: 6572 7369 6c69 6123 6162 6f75 742d 7573  ersilia#about-us
+000008c0: 290a 2020 2020 2020 2020 0a20 2020 2020  ).        .     
+000008d0: 2020 2023 2320 5072 6f6a 6563 7420 4465     ## Project De
+000008e0: 7363 7269 7074 696f 6e0a 2020 2020 2020  scription.      
+000008f0: 2020 0a20 2020 2020 2020 2054 6865 2045    .        The E
+00000900: 7273 696c 6961 204d 6f64 656c 2048 7562  rsilia Model Hub
+00000910: 2069 7320 6120 756e 6966 6965 6420 706c   is a unified pl
+00000920: 6174 666f 726d 206f 6620 7072 652d 7472  atform of pre-tr
+00000930: 6169 6e65 6420 4149 2f4d 4c20 6d6f 6465  ained AI/ML mode
+00000940: 6c73 2066 6f72 2069 6e66 6563 7469 6f75  ls for infectiou
+00000950: 7320 616e 6420 6e65 676c 6563 7465 6420  s and neglected 
+00000960: 6469 7365 6173 6520 7265 7365 6172 6368  disease research
+00000970: 2e20 5468 6520 656e 6420 676f 616c 2069  . The end goal i
+00000980: 7320 746f 2070 726f 7669 6465 2061 6e20  s to provide an 
+00000990: 6f70 656e 2d73 6f75 7263 652c 206e 6f2d  open-source, no-
+000009a0: 636f 6465 2073 6f6c 7574 696f 6e20 746f  code solution to
+000009b0: 2061 6363 6573 7320 4149 2f4d 4c20 6d6f   access AI/ML mo
+000009c0: 6465 6c73 2074 6f20 6163 6365 6c65 7261  dels to accelera
+000009d0: 7465 2064 7275 6720 6469 7363 6f76 6572  te drug discover
+000009e0: 792e 2054 6865 206d 6f64 656c 7320 656d  y. The models em
+000009f0: 6265 6464 6564 2069 6e20 7468 6520 6875  bedded in the hu
+00000a00: 6220 696e 636c 7564 6520 626f 7468 206d  b include both m
+00000a10: 6f64 656c 7320 7075 626c 6973 6865 6420  odels published 
+00000a20: 696e 2074 6865 206c 6974 6572 6174 7572  in the literatur
+00000a30: 6520 2877 6974 6820 6170 7072 6f70 7269  e (with appropri
+00000a40: 6174 6520 7468 6972 6420 7061 7274 7920  ate third party 
+00000a50: 6163 6b6e 6f77 6c65 6467 656d 656e 7429  acknowledgement)
+00000a60: 2061 6e64 206d 6f64 656c 7320 6465 7665   and models deve
+00000a70: 6c6f 7065 6420 6279 2074 6865 2045 7273  loped by the Ers
+00000a80: 696c 6961 2074 6561 6d20 6f72 2063 6f6e  ilia team or con
+00000a90: 7472 6962 7574 6f72 732e 0a20 2020 2020  tributors..     
+00000aa0: 2020 200a 2020 2020 2020 2020 2a20 5265     .        * Re
+00000ab0: 6164 206d 6f72 6520 6162 6f75 7420 7468  ad more about th
+00000ac0: 6520 7072 6f6a 6563 7420 696e 2074 6865  e project in the
+00000ad0: 205b 4572 7369 6c69 6120 426f 6f6b 5d28   [Ersilia Book](
+00000ae0: 6874 7470 733a 2f2f 6572 7369 6c69 612e  https://ersilia.
+00000af0: 6769 7462 6f6f 6b2e 696f 2f65 7273 696c  gitbook.io/ersil
+00000b00: 6961 2d62 6f6f 6b2f 290a 2020 2020 2020  ia-book/).      
+00000b10: 2020 2a20 4272 6f77 7365 2061 7661 696c    * Browse avail
+00000b20: 6162 6c65 206d 6f64 656c 7320 696e 2074  able models in t
+00000b30: 6865 205b 4572 7369 6c69 6120 4d6f 6465  he [Ersilia Mode
+00000b40: 6c20 4875 625d 2868 7474 7073 3a2f 2f65  l Hub](https://e
+00000b50: 7273 696c 6961 2e69 6f2f 6d6f 6465 6c2d  rsilia.io/model-
+00000b60: 6875 622f 290a 2020 2020 2020 2020 0a20  hub/).        . 
+00000b70: 2020 2020 2020 2023 2320 5175 6963 6b20         ## Quick 
+00000b80: 5374 6172 7420 4775 6964 650a 2020 2020  Start Guide.    
+00000b90: 2020 2020 0a20 2020 2020 2020 2050 6c65      .        Ple
+00000ba0: 6173 6520 6368 6563 6b20 7468 6520 7061  ase check the pa
+00000bb0: 636b 6167 6520 7265 7175 6972 656d 656e  ckage requiremen
+00000bc0: 7473 2069 6e20 7468 6520 5b49 6e73 7461  ts in the [Insta
+00000bd0: 6c6c 6174 696f 6e20 4775 6964 655d 2868  llation Guide](h
+00000be0: 7474 7073 3a2f 2f65 7273 696c 6961 2e67  ttps://ersilia.g
+00000bf0: 6974 626f 6f6b 2e69 6f2f 6572 7369 6c69  itbook.io/ersili
+00000c00: 612d 626f 6f6b 2f71 7569 636b 2d73 7461  a-book/quick-sta
+00000c10: 7274 2f69 6e73 7461 6c6c 6174 696f 6e29  rt/installation)
+00000c20: 2e20 5468 6520 6e65 7874 2073 7465 7073  . The next steps
+00000c30: 2061 7265 2061 2071 7569 636b 7374 6172   are a quickstar
+00000c40: 7420 6775 6964 6520 746f 2069 6e73 7461  t guide to insta
+00000c50: 6c6c 696e 6720 4572 7369 6c69 612e 0a20  lling Ersilia.. 
+00000c60: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000c70: 312e 2043 7265 6174 6520 6120 636f 6e64  1. Create a cond
+00000c80: 6120 656e 7669 726f 6e6d 656e 7420 616e  a environment an
+00000c90: 6420 6163 7469 7661 7465 2069 740a 2020  d activate it.  
+00000ca0: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00000cb0: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00000cc0: 2020 2020 2020 2063 6f6e 6461 2063 7265         conda cre
+00000cd0: 6174 6520 2d6e 2065 7273 696c 6961 2070  ate -n ersilia p
+00000ce0: 7974 686f 6e3d 332e 370a 2020 2020 2020  ython=3.7.      
+00000cf0: 2020 2020 2020 636f 6e64 6120 6163 7469        conda acti
+00000d00: 7661 7465 2065 7273 696c 6961 0a20 2020  vate ersilia.   
+00000d10: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000d20: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00000d30: 2043 6c6f 6e65 2074 6869 7320 7265 706f   Clone this repo
+00000d40: 7369 746f 7279 2061 6e64 2069 6e73 7461  sitory and insta
+00000d50: 6c6c 2077 6974 6820 7069 700a 2020 2020  ll with pip.    
+00000d60: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
+00000d70: 2060 6060 6261 7368 0a20 2020 2020 2020   ```bash.       
+00000d80: 2020 2020 2067 6974 2063 6c6f 6e65 2068       git clone h
+00000d90: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000da0: 6d2f 6572 7369 6c69 612d 6f73 2f65 7273  m/ersilia-os/ers
+00000db0: 696c 6961 2e67 6974 0a20 2020 2020 2020  ilia.git.       
+00000dc0: 2020 2020 2063 6420 6572 7369 6c69 610a       cd ersilia.
+00000dd0: 2020 2020 2020 2020 2020 2020 7069 7020              pip 
+00000de0: 696e 7374 616c 6c20 2d65 202e 0a20 2020  install -e ..   
+00000df0: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00000e00: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00000e10: 204f 6e63 6520 7468 6520 4572 7369 6c69   Once the Ersili
+00000e20: 6120 4d6f 6465 6c20 4875 6220 6973 2069  a Model Hub is i
+00000e30: 6e73 7461 6c6c 6564 2c20 796f 7520 6361  nstalled, you ca
+00000e40: 6e20 7573 6520 7468 6520 434c 4920 746f  n use the CLI to
+00000e50: 2072 756e 2070 7265 6469 6374 696f 6e73   run predictions
+00000e60: 2e20 4669 7273 742c 2073 656c 6563 7420  . First, select 
+00000e70: 6120 6d6f 6465 6c20 6672 6f6d 2074 6865  a model from the
+00000e80: 205b 4572 7369 6c69 6120 4d6f 6465 6c20   [Ersilia Model 
+00000e90: 4875 625d 2868 7474 7073 3a2f 2f65 7273  Hub](https://ers
+00000ea0: 696c 6961 2e69 6f2f 6d6f 6465 6c2d 6875  ilia.io/model-hu
+00000eb0: 622f 2920 616e 6420 2a2a 6665 7463 682a  b/) and **fetch*
+00000ec0: 2a20 6974 3a0a 2020 2020 2020 2020 0a20  * it:.        . 
+00000ed0: 2020 2020 2020 2020 2020 2060 6060 6261             ```ba
+00000ee0: 7368 0a20 2020 2020 2020 2020 2020 2065  sh.            e
+00000ef0: 7273 696c 6961 2066 6574 6368 2072 6574  rsilia fetch ret
+00000f00: 726f 7379 6e74 6865 7469 632d 6163 6365  rosynthetic-acce
+00000f10: 7373 6962 696c 6974 790a 2020 2020 2020  ssibility.      
+00000f20: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00000f30: 2020 0a20 2020 2020 2020 2031 2e20 4765    .        1. Ge
+00000f40: 6e65 7261 7465 2061 2066 6577 2028 3529  nerate a few (5)
+00000f50: 2065 7861 6d70 6c65 206d 6f6c 6563 756c   example molecul
+00000f60: 6573 2c20 746f 2062 6520 7573 6564 2061  es, to be used a
+00000f70: 7320 696e 7075 742e 2054 6865 202a 2a65  s input. The **e
+00000f80: 7861 6d70 6c65 2a2a 2063 6f6d 6d61 6e64  xample** command
+00000f90: 2077 696c 6c20 6765 6e65 7261 7465 2074   will generate t
+00000fa0: 6865 2061 6465 7175 6174 6520 696e 7075  he adequate inpu
+00000fb0: 7420 666f 7220 7468 6520 6d6f 6465 6c20  t for the model 
+00000fc0: 696e 2075 7365 0a20 2020 2020 2020 200a  in use.        .
+00000fd0: 2020 2020 2020 2020 2020 2020 6060 6062              ```b
+00000fe0: 6173 680a 2020 2020 2020 2020 2020 2020  ash.            
+00000ff0: 6572 7369 6c69 6120 6578 616d 706c 6520  ersilia example 
+00001000: 7265 7472 6f73 796e 7468 6574 6963 2d61  retrosynthetic-a
+00001010: 6363 6573 7369 6269 6c69 7479 202d 6e20  ccessibility -n 
+00001020: 3520 2d66 206d 795f 6d6f 6c65 6375 6c65  5 -f my_molecule
+00001030: 732e 6373 760a 2020 2020 2020 2020 2020  s.csv.          
+00001040: 2020 6060 600a 2020 2020 2020 2020 0a20    ```.        . 
+00001050: 2020 2020 2020 2031 2e20 5468 656e 2c20         1. Then, 
+00001060: 2a2a 7365 7276 652a 2a20 796f 7572 206d  **serve** your m
+00001070: 6f64 656c 3a0a 2020 2020 2020 2020 0a20  odel:.        . 
+00001080: 2020 2020 2020 2020 2020 2060 6060 6261             ```ba
+00001090: 7368 0a20 2020 2020 2020 2020 2020 2065  sh.            e
+000010a0: 7273 696c 6961 2073 6572 7665 2072 6574  rsilia serve ret
+000010b0: 726f 7379 6e74 6865 7469 632d 6163 6365  rosynthetic-acce
+000010c0: 7373 6962 696c 6974 790a 2020 2020 2020  ssibility.      
+000010d0: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+000010e0: 2020 0a20 2020 2020 2020 2031 2e20 416e    .        1. An
+000010f0: 6420 7275 6e20 7468 6520 7072 6564 6963  d run the predic
+00001100: 7469 6f6e 202a 2a41 5049 2a2a 3a0a 2020  tion **API**:.  
+00001110: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+00001120: 2020 2060 6060 6261 7368 0a20 2020 2020     ```bash.     
+00001130: 2020 2020 2020 2065 7273 696c 6961 2061         ersilia a
+00001140: 7069 202d 6920 6d79 5f6d 6f6c 6563 756c  pi -i my_molecul
+00001150: 6573 2e63 7376 202d 6f20 6d79 5f70 7265  es.csv -o my_pre
+00001160: 6469 6374 696f 6e73 2e63 7376 0a20 2020  dictions.csv.   
+00001170: 2020 2020 2020 2020 2060 6060 0a20 2020           ```.   
+00001180: 2020 2020 200a 2020 2020 2020 2020 312e       .        1.
+00001190: 2046 696e 616c 6c79 2c20 2a2a 636c 6f73   Finally, **clos
+000011a0: 652a 2a20 7468 6520 7365 7276 6963 6520  e** the service 
+000011b0: 7768 656e 2079 6f75 2061 7265 2064 6f6e  when you are don
+000011c0: 652e 0a20 2020 2020 2020 200a 2020 2020  e..        .    
+000011d0: 2020 2020 2020 2020 6060 6062 6173 680a          ```bash.
+000011e0: 2020 2020 2020 2020 2020 2020 6572 7369              ersi
+000011f0: 6c69 6120 636c 6f73 650a 2020 2020 2020  lia close.      
+00001200: 2020 2020 2020 6060 600a 2020 2020 2020        ```.      
+00001210: 2020 0a20 2020 2020 2020 2050 6c65 6173    .        Pleas
+00001220: 6520 7365 6520 7468 6520 5b45 7273 696c  e see the [Ersil
+00001230: 6961 2042 6f6f 6b5d 2868 7474 7073 3a2f  ia Book](https:/
+00001240: 2f65 7273 696c 6961 2e67 6974 626f 6f6b  /ersilia.gitbook
+00001250: 2e69 6f2f 6572 7369 6c69 612d 626f 6f6b  .io/ersilia-book
+00001260: 2f29 2066 6f72 206d 6f72 6520 6578 616d  /) for more exam
+00001270: 706c 6573 2061 6e64 2064 6574 6169 6c65  ples and detaile
+00001280: 6420 6578 706c 616e 6174 696f 6e73 2e0a  d explanations..
+00001290: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000012a0: 2023 2320 436f 6e74 7269 6275 7465 0a20   ## Contribute. 
+000012b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000012c0: 5468 6520 4572 7369 6c69 6120 4d6f 6465  The Ersilia Mode
+000012d0: 6c20 4875 6220 6973 2061 2046 7265 652c  l Hub is a Free,
+000012e0: 204f 7065 6e20 536f 7572 6365 2053 6f66   Open Source Sof
+000012f0: 7477 6172 6520 616e 6420 7765 2068 6967  tware and we hig
+00001300: 686c 7920 7661 6c75 6520 6e65 7720 636f  hly value new co
+00001310: 6e74 7269 6275 746f 7273 2e20 5468 6572  ntributors. Ther
+00001320: 6520 6172 6520 7365 7665 7261 6c20 7761  e are several wa
+00001330: 7973 2069 6e20 7768 6963 6820 796f 7520  ys in which you 
+00001340: 6361 6e20 636f 6e74 7269 6275 7465 2074  can contribute t
+00001350: 6f20 7468 6520 7072 6f6a 6563 743a 0a20  o the project:. 
+00001360: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00001370: 2a20 4120 676f 6f64 2070 6c61 6365 2074  * A good place t
+00001380: 6f20 7374 6172 7420 6973 2063 6865 636b  o start is check
+00001390: 696e 6720 6f70 656e 205b 6973 7375 6573  ing open [issues
+000013a0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000013b0: 2e63 6f6d 2f65 7273 696c 6961 2d6f 732f  .com/ersilia-os/
+000013c0: 6572 7369 6c69 612f 6973 7375 6573 292e  ersilia/issues).
+000013d0: 0a20 2020 2020 2020 202a 2049 6620 796f  .        * If yo
+000013e0: 7520 6861 7665 2069 6465 6e74 6966 6965  u have identifie
+000013f0: 6420 6120 6275 6720 696e 2074 6865 2063  d a bug in the c
+00001400: 6f64 652c 2070 6c65 6173 6520 6f70 656e  ode, please open
+00001410: 2061 206e 6577 2069 7373 7565 2075 7369   a new issue usi
+00001420: 6e67 2074 6865 2062 7567 2074 656d 706c  ng the bug templ
+00001430: 6174 652e 0a20 2020 2020 2020 202a 2053  ate..        * S
+00001440: 6861 7265 2061 6e79 2066 6565 6462 6163  hare any feedbac
+00001450: 6b20 7769 7468 2074 6865 2063 6f6d 6d75  k with the commu
+00001460: 6e69 7479 2075 7369 6e67 205b 4769 7448  nity using [GitH
+00001470: 7562 2044 6973 6375 7373 696f 6e73 5d28  ub Discussions](
+00001480: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00001490: 6f6d 2f65 7273 696c 6961 2d6f 732f 6572  om/ersilia-os/er
+000014a0: 7369 6c69 612f 6469 7363 7573 7369 6f6e  silia/discussion
+000014b0: 7329 2066 6f72 2074 6865 2070 726f 6a65  s) for the proje
+000014c0: 6374 0a20 2020 2020 2020 202a 2043 6865  ct.        * Che
+000014d0: 636b 206f 7572 205b 436f 6e74 7269 6275  ck our [Contribu
+000014e0: 7469 6e67 2047 7569 6465 5d28 6874 7470  ting Guide](http
+000014f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00001500: 7273 696c 6961 2d6f 732f 6572 7369 6c69  rsilia-os/ersili
+00001510: 612f 626c 6f62 2f6d 6173 7465 722f 434f  a/blob/master/CO
+00001520: 4e54 5249 4255 5449 4e47 2e6d 6429 2066  NTRIBUTING.md) f
+00001530: 6f72 206d 6f72 6520 6465 7461 696c 730a  or more details.
+00001540: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00001550: 2054 6865 2045 7273 696c 6961 204f 7065   The Ersilia Ope
+00001560: 6e20 536f 7572 6365 2049 6e69 7469 6174  n Source Initiat
+00001570: 6976 6520 6164 6865 7265 7320 746f 2074  ive adheres to t
+00001580: 6865 205b 436f 6e74 7269 6275 746f 7220  he [Contributor 
+00001590: 436f 7665 6e61 6e74 5d28 6874 7470 733a  Covenant](https:
+000015a0: 2f2f 6572 7369 6c69 612e 6769 7462 6f6f  //ersilia.gitboo
+000015b0: 6b2e 696f 2f65 7273 696c 6961 2d77 696b  k.io/ersilia-wik
+000015c0: 692f 636f 6465 2d6f 662d 636f 6e64 7563  i/code-of-conduc
+000015d0: 7429 2063 6f64 6520 6f66 2063 6f6e 6475  t) code of condu
+000015e0: 6374 2e0a 2020 2020 2020 2020 0a20 2020  ct..        .   
+000015f0: 2020 2020 2023 2323 2053 7562 6d69 7420       ### Submit 
+00001600: 6120 4e65 7720 4d6f 6465 6c0a 2020 2020  a New Model.    
+00001610: 2020 2020 0a20 2020 2020 2020 2049 6620      .        If 
+00001620: 796f 7520 7761 6e74 2074 6f20 696e 636f  you want to inco
+00001630: 7270 6f72 6174 6520 6120 6e65 7720 6d6f  rporate a new mo
+00001640: 6465 6c20 696e 2074 6865 2070 6c61 7466  del in the platf
+00001650: 6f72 6d2c 206f 7065 6e20 6120 6e65 7720  orm, open a new 
+00001660: 6973 7375 6520 7573 696e 6720 7468 6520  issue using the 
+00001670: 5b6d 6f64 656c 2072 6571 7565 7374 2074  [model request t
+00001680: 656d 706c 6174 655d 2868 7474 7073 3a2f  emplate](https:/
+00001690: 2f67 6974 6875 622e 636f 6d2f 6572 7369  /github.com/ersi
+000016a0: 6c69 612d 6f73 2f65 7273 696c 6961 2f69  lia-os/ersilia/i
+000016b0: 7373 7565 732f 6e65 773f 6173 7369 676e  ssues/new?assign
+000016c0: 6565 733d 266c 6162 656c 733d 6e65 772d  ees=&labels=new-
+000016d0: 6d6f 6465 6c26 7465 6d70 6c61 7465 3d6d  model&template=m
+000016e0: 6f64 656c 5f72 6571 7565 7374 2e79 6d6c  odel_request.yml
+000016f0: 2674 6974 6c65 3d25 4630 2539 4625 4136  &title=%F0%9F%A6
+00001700: 2541 302b 4d6f 6465 6c2b 5265 7175 6573  %A0+Model+Reques
+00001710: 7425 3341 2b25 3343 6e61 6d65 2533 4529  t%3A+%3Cname%3E)
+00001720: 206f 7220 636f 6e74 6163 7420 7573 2075   or contact us u
+00001730: 7369 6e67 2074 6865 2066 6f6c 6c6f 7769  sing the followi
+00001740: 6e67 205b 666f 726d 5d28 6874 7470 733a  ng [form](https:
+00001750: 2f2f 7777 772e 6572 7369 6c69 612e 696f  //www.ersilia.io
+00001760: 2f72 6571 7565 7374 2d6d 6f64 656c 292e  /request-model).
+00001770: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00001780: 2020 4166 7465 7220 7375 626d 6974 7469    After submitti
+00001790: 6e67 2079 6f75 7220 6d6f 6465 6c20 7265  ng your model re
+000017a0: 7175 6573 7420 7669 6120 616e 2069 7373  quest via an iss
+000017b0: 7565 2028 7375 6767 6573 7465 6429 2c20  ue (suggested), 
+000017c0: 6120 6d61 696e 7461 696e 6572 2077 696c  a maintainer wil
+000017d0: 6c20 7265 7669 6577 2079 6f75 7220 7265  l review your re
+000017e0: 7175 6573 742e 2049 6620 7468 6579 2060  quest. If they `
+000017f0: 2f61 7070 726f 7665 6020 796f 7572 2072  /approve` your r
+00001800: 6571 7565 7374 2c20 6120 6e65 7720 6d6f  equest, a new mo
+00001810: 6465 6c20 7265 7370 6f73 6974 6f72 7920  del respository 
+00001820: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
+00001830: 666f 7220 796f 7520 746f 2066 6f72 6b20  for you to fork 
+00001840: 616e 6420 7573 6521 2054 6865 7265 2069  and use! There i
+00001850: 7320 6120 5b64 656d 6f20 7265 706f 7369  s a [demo reposi
+00001860: 746f 7279 5d28 6874 7470 733a 2f2f 6769  tory](https://gi
+00001870: 7468 7562 2e63 6f6d 2f65 7273 696c 6961  thub.com/ersilia
+00001880: 2d6f 732f 656f 732d 6465 6d6f 2920 6578  -os/eos-demo) ex
+00001890: 706c 6169 6e69 6e67 2074 6865 2073 7465  plaining the ste
+000018a0: 7073 206f 6e65 2d62 792d 6f6e 652e 0a20  ps one-by-one.. 
+000018b0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+000018c0: 2323 204c 6963 656e 7365 2061 6e64 2043  ## License and C
+000018d0: 6974 6174 696f 6e0a 2020 2020 2020 2020  itation.        
+000018e0: 0a20 2020 2020 2020 2054 6869 7320 7265  .        This re
+000018f0: 706f 7369 746f 7279 2069 7320 6f70 656e  pository is open
+00001900: 2d73 6f75 7263 6564 2075 6e64 6572 2074  -sourced under t
+00001910: 6865 205b 4750 4c2d 3320 4c69 6365 6e73  he [GPL-3 Licens
+00001920: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00001930: 622e 636f 6d2f 6572 7369 6c69 612d 6f73  b.com/ersilia-os
+00001940: 2f65 7273 696c 6961 2f62 6c6f 622f 6d61  /ersilia/blob/ma
+00001950: 7374 6572 2f4c 4943 454e 5345 292e 0a20  ster/LICENSE).. 
+00001960: 2020 2020 2020 2050 6c65 6173 6520 5b63         Please [c
+00001970: 6974 6520 7573 5d28 6874 7470 733a 2f2f  ite us](https://
+00001980: 6769 7468 7562 2e63 6f6d 2f65 7273 696c  github.com/ersil
+00001990: 6961 2d6f 732f 6572 7369 6c69 612f 626c  ia-os/ersilia/bl
+000019a0: 6f62 2f6d 6173 7465 722f 4349 5441 5449  ob/master/CITATI
+000019b0: 4f4e 2e63 6666 2920 6966 2079 6f75 2075  ON.cff) if you u
+000019c0: 7365 2069 7421 0a20 2020 2020 2020 200a  se it!.        .
+000019d0: 2020 2020 2020 2020 2323 2041 626f 7574          ## About
+000019e0: 2055 730a 2020 2020 2020 2020 0a20 2020   Us.        .   
+000019f0: 2020 2020 2054 6865 205b 4572 7369 6c69       The [Ersili
+00001a00: 6120 4f70 656e 2053 6f75 7263 6520 496e  a Open Source In
+00001a10: 6974 6961 7469 7665 5d28 6874 7470 733a  itiative](https:
+00001a20: 2f2f 6572 7369 6c69 612e 696f 2920 6973  //ersilia.io) is
+00001a30: 2061 204e 6f6e 2050 726f 6669 7420 4f72   a Non Profit Or
+00001a40: 6761 6e69 7a61 7469 6f6e 2028 5b31 3139  ganization ([119
+00001a50: 3232 3636 5d28 6874 7470 733a 2f2f 7265  2266](https://re
+00001a60: 6769 7374 6572 2d6f 662d 6368 6172 6974  gister-of-charit
+00001a70: 6965 732e 6368 6172 6974 7963 6f6d 6d69  ies.charitycommi
+00001a80: 7373 696f 6e2e 676f 762e 756b 2f63 6861  ssion.gov.uk/cha
+00001a90: 7269 7479 2d73 6561 7263 682f 2d2f 6368  rity-search/-/ch
+00001aa0: 6172 6974 792d 6465 7461 696c 732f 3531  arity-details/51
+00001ab0: 3730 3635 372f 6675 6c6c 2d70 7269 6e74  70657/full-print
+00001ac0: 2929 2077 6974 6820 7468 6520 6d69 7373  )) with the miss
+00001ad0: 696f 6e20 6973 2074 6f20 6571 7569 7020  ion is to equip 
+00001ae0: 6c61 6273 2c20 756e 6976 6572 7369 7469  labs, universiti
+00001af0: 6573 2061 6e64 2063 6c69 6e69 6373 2069  es and clinics i
+00001b00: 6e20 4c4d 4943 2077 6974 6820 4149 2f4d  n LMIC with AI/M
+00001b10: 4c20 746f 6f6c 7320 666f 7220 696e 6665  L tools for infe
+00001b20: 6374 696f 7573 2064 6973 6561 7365 2072  ctious disease r
+00001b30: 6573 6561 7263 682e 0a20 2020 2020 2020  esearch..       
+00001b40: 200a 2020 2020 2020 2020 5b48 656c 7020   .        [Help 
+00001b50: 7573 5d28 6874 7470 733a 2f2f 7777 772e  us](https://www.
+00001b60: 6572 7369 6c69 612e 696f 2f64 6f6e 6174  ersilia.io/donat
+00001b70: 6529 2061 6368 6965 7665 206f 7572 206d  e) achieve our m
+00001b80: 6973 7369 6f6e 206f 7220 5b76 6f6c 756e  ission or [volun
+00001b90: 7465 6572 5d28 6874 7470 733a 2f2f 7777  teer](https://ww
+00001ba0: 772e 6572 7369 6c69 612e 696f 2f76 6f6c  w.ersilia.io/vol
+00001bb0: 756e 7465 6572 2920 7769 7468 2075 7321  unteer) with us!
+00001bc0: 0a20 2020 2020 2020 200a 4b65 7977 6f72  .        .Keywor
+00001bd0: 6473 3a20 6472 7567 2d64 6973 636f 7665  ds: drug-discove
+00001be0: 7279 206d 6163 6869 6e65 2d6c 6561 726e  ry machine-learn
+00001bf0: 696e 6720 6572 7369 6c69 6120 6f70 656e  ing ersilia open
+00001c00: 2d73 6369 656e 6365 2067 6c6f 6261 6c2d  -science global-
+00001c10: 6865 616c 7468 206d 6f64 656c 2d68 7562  health model-hub
+00001c20: 2069 6e66 6563 7469 6f75 732d 6469 7365   infectious-dise
+00001c30: 6173 6573 0a50 6c61 7466 6f72 6d3a 2055  ases.Platform: U
+00001c40: 4e4b 4e4f 574e 0a43 6c61 7373 6966 6965  NKNOWN.Classifie
+00001c50: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
+00001c60: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
+00001c70: 6e20 3a3a 2033 2e37 0a43 6c61 7373 6966  n :: 3.7.Classif
+00001c80: 6965 723a 2050 726f 6772 616d 6d69 6e67  ier: Programming
+00001c90: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00001ca0: 686f 6e20 3a3a 2033 2e38 0a43 6c61 7373  hon :: 3.8.Class
+00001cb0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00001cc0: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00001cd0: 7974 686f 6e20 3a3a 2033 2e39 0a43 6c61  ython :: 3.9.Cla
+00001ce0: 7373 6966 6965 723a 204c 6963 656e 7365  ssifier: License
+00001cf0: 203a 3a20 4f53 4920 4170 7072 6f76 6564   :: OSI Approved
+00001d00: 203a 3a20 474e 5520 4765 6e65 7261 6c20   :: GNU General 
+00001d10: 5075 626c 6963 204c 6963 656e 7365 2076  Public License v
+00001d20: 3320 2847 504c 7633 290a 436c 6173 7369  3 (GPLv3).Classi
+00001d30: 6669 6572 3a20 4f70 6572 6174 696e 6720  fier: Operating 
+00001d40: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+00001d50: 6570 656e 6465 6e74 0a43 6c61 7373 6966  ependent.Classif
+00001d60: 6965 723a 2054 6f70 6963 203a 3a20 5363  ier: Topic :: Sc
+00001d70: 6965 6e74 6966 6963 2f45 6e67 696e 6565  ientific/Enginee
+00001d80: 7269 6e67 203a 3a20 4172 7469 6669 6369  ring :: Artifici
+00001d90: 616c 2049 6e74 656c 6c69 6765 6e63 650a  al Intelligence.
+00001da0: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00001db0: 203e 3d33 2e37 0a44 6573 6372 6970 7469   >=3.7.Descripti
+00001dc0: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00001dd0: 2074 6578 742f 6d61 726b 646f 776e 0a50   text/markdown.P
+00001de0: 726f 7669 6465 732d 4578 7472 613a 206c  rovides-Extra: l
+00001df0: 616b 650a 5072 6f76 6964 6573 2d45 7874  ake.Provides-Ext
+00001e00: 7261 3a20 646f 6373 0a50 726f 7669 6465  ra: docs.Provide
+00001e10: 732d 4578 7472 613a 2074 6573 740a       s-Extra: test.
```

### Comparing `ersilia-0.1.1/ersilia.egg-info/SOURCES.txt` & `ersilia-0.1.8/ersilia.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 MANIFEST.in
 README.md
 setup.py
 ersilia/__init__.py
-ersilia/_clean_static_version.py
-ersilia/_clean_version.py
 ersilia/_static_version.py
 ersilia/_version.py
 ersilia/default.py
 ersilia.egg-info/PKG-INFO
 ersilia.egg-info/SOURCES.txt
 ersilia.egg-info/dependency_links.txt
 ersilia.egg-info/entry_points.txt
@@ -31,56 +29,64 @@
 ersilia/cli/commands/catalog.py
 ersilia/cli/commands/clear.py
 ersilia/cli/commands/close.py
 ersilia/cli/commands/delete.py
 ersilia/cli/commands/deploy.py
 ersilia/cli/commands/example.py
 ersilia/cli/commands/fetch.py
+ersilia/cli/commands/info.py
 ersilia/cli/commands/publish.py
+ersilia/cli/commands/sample.py
 ersilia/cli/commands/serve.py
 ersilia/cli/commands/setup.py
+ersilia/cli/commands/test.py
 ersilia/cli/commands/utils/__init__.py
 ersilia/cli/commands/utils/utils.py
 ersilia/core/__init__.py
 ersilia/core/base.py
 ersilia/core/model.py
 ersilia/core/modelbase.py
 ersilia/core/session.py
 ersilia/db/__init__.py
 ersilia/db/disk/__init__.py
 ersilia/db/disk/fetched.py
 ersilia/db/environments/__init__.py
 ersilia/db/environments/localdb.py
 ersilia/db/environments/managers.py
 ersilia/db/hubdata/__init__.py
+ersilia/db/hubdata/interfaces.py
 ersilia/db/hubdata/localslugs.py
+ersilia/db/hubdata/samplers.py
 ersilia/db/hubdata/tables.py
 ersilia/hub/__init__.py
 ersilia/hub/bundle/__init__.py
 ersilia/hub/bundle/bundle.py
 ersilia/hub/bundle/repo.py
 ersilia/hub/bundle/status.py
 ersilia/hub/content/__init__.py
 ersilia/hub/content/card.py
 ersilia/hub/content/catalog.py
+ersilia/hub/content/information.py
 ersilia/hub/content/search.py
 ersilia/hub/content/slug.py
 ersilia/hub/content/table_update.py
 ersilia/hub/delete/__init__.py
 ersilia/hub/delete/delete.py
 ersilia/hub/fetch/__init__.py
 ersilia/hub/fetch/fetch.py
 ersilia/hub/fetch/actions/__init__.py
 ersilia/hub/fetch/actions/check.py
 ersilia/hub/fetch/actions/content.py
 ersilia/hub/fetch/actions/get.py
+ersilia/hub/fetch/actions/inform.py
 ersilia/hub/fetch/actions/lake.py
 ersilia/hub/fetch/actions/modify.py
 ersilia/hub/fetch/actions/pack.py
 ersilia/hub/fetch/actions/prepare.py
+ersilia/hub/fetch/actions/setup.py
 ersilia/hub/fetch/actions/sniff.py
 ersilia/hub/fetch/actions/toolize.py
 ersilia/hub/fetch/pack/__init__.py
 ersilia/hub/fetch/pack/mode.py
 ersilia/hub/fetch/pack/runners.py
 ersilia/io/__init__.py
 ersilia/io/dataframe.py
@@ -102,60 +108,83 @@
 ersilia/io/types/examples/protein.tsv
 ersilia/lake/__init__.py
 ersilia/lake/base.py
 ersilia/lake/interface.py
 ersilia/lake/manager.py
 ersilia/publish/__init__.py
 ersilia/publish/deploy.py
+ersilia/publish/dockerhub.py
 ersilia/publish/lake.py
+ersilia/publish/metadata.py
 ersilia/publish/publish.py
 ersilia/publish/rebase.py
+ersilia/publish/s3.py
 ersilia/publish/store.py
+ersilia/publish/test.py
 ersilia/serve/__init__.py
 ersilia/serve/api.py
 ersilia/serve/autoservice.py
 ersilia/serve/schema.py
 ersilia/serve/services.py
 ersilia/setup/__init__.py
 ersilia/setup/baseconda.py
 ersilia/setup/basedocker.py
 ersilia/setup/conda.py
 ersilia/setup/config.py
 ersilia/setup/profile.py
 ersilia/setup/requirements/__init__.py
+ersilia/setup/requirements/bentoml.py
 ersilia/setup/requirements/compound.py
 ersilia/setup/requirements/conda.py
 ersilia/setup/requirements/docker.py
+ersilia/setup/requirements/eospath.py
 ersilia/setup/requirements/git.py
 ersilia/setup/requirements/isaura.py
+ersilia/setup/requirements/ping.py
 ersilia/setup/utils/__init__.py
 ersilia/setup/utils/clone.py
 ersilia/utils/__init__.py
 ersilia/utils/clear.py
+ersilia/utils/cli_query.py
 ersilia/utils/conda.py
 ersilia/utils/config.py
 ersilia/utils/cron.py
 ersilia/utils/csvfile.py
 ersilia/utils/docker.py
 ersilia/utils/download.py
 ersilia/utils/dvc.py
 ersilia/utils/environment.py
-ersilia/utils/exceptions.py
 ersilia/utils/hdf5.py
 ersilia/utils/import.py
 ersilia/utils/installers.py
 ersilia/utils/logging.py
 ersilia/utils/paths.py
 ersilia/utils/ports.py
 ersilia/utils/remove.py
+ersilia/utils/system.py
 ersilia/utils/terminal.py
 ersilia/utils/upload.py
 ersilia/utils/venv.py
 ersilia/utils/versioning.py
 ersilia/utils/zip.py
+ersilia/utils/exceptions_utils/__init__.py
+ersilia/utils/exceptions_utils/api_exceptions.py
+ersilia/utils/exceptions_utils/card_exceptions.py
+ersilia/utils/exceptions_utils/catalog_exceptions.py
+ersilia/utils/exceptions_utils/clear_exceptions.py
+ersilia/utils/exceptions_utils/close_exceptions.py
+ersilia/utils/exceptions_utils/delete_exceptions.py
+ersilia/utils/exceptions_utils/example_exceptions.py
+ersilia/utils/exceptions_utils/exceptions.py
+ersilia/utils/exceptions_utils/fetch_exceptions.py
+ersilia/utils/exceptions_utils/handle_undecorated_exception.py
+ersilia/utils/exceptions_utils/issue_reporting.py
+ersilia/utils/exceptions_utils/serve_exceptions.py
+ersilia/utils/exceptions_utils/setup_exceptions.py
+ersilia/utils/exceptions_utils/throw_ersilia_exception.py
 ersilia/utils/identifiers/__init__.py
 ersilia/utils/identifiers/arbitrary.py
 ersilia/utils/identifiers/compound.py
 ersilia/utils/identifiers/file.py
 ersilia/utils/identifiers/long.py
 ersilia/utils/identifiers/model.py
 ersilia/utils/identifiers/protein.py
```

### Comparing `ersilia-0.1.1/test/test_inputs.py` & `ersilia-0.1.8/test/test_inputs.py`

 * *Files identical despite different names*

### Comparing `ersilia-0.1.1/test/test_models.py` & `ersilia-0.1.8/test/test_models.py`

 * *Files identical despite different names*

