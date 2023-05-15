# Comparing `tmp/irails-1.3.14.tar.gz` & `tmp/irails-1.3.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.14.tar", last modified: Mon May 15 09:30:27 2023, max compression
+gzip compressed data, was "irails-1.3.15.tar", last modified: Mon May 15 11:56:31 2023, max compression
```

## Comparing `irails-1.3.14.tar` & `irails-1.3.15.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.043065 irails-1.3.14/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.14/MANIFEST.in
--rw-rw-rw-   0        0        0     5518 2023-05-15 09:30:27.043065 irails-1.3.14/PKG-INFO
--rw-rw-rw-   0        0        0     4734 2023-05-15 07:02:13.000000 irails-1.3.14/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.964274 irails-1.3.14/irails/
--rw-rw-rw-   0        0        0      307 2023-05-15 09:30:09.000000 irails-1.3.14/irails/__init__.py
--rw-rw-rw-   0        0        0     3409 2023-05-13 06:08:26.000000 irails-1.3.14/irails/_i18n.py
--rw-rw-rw-   0        0        0     2883 2023-05-15 06:36:25.000000 irails-1.3.14/irails/_loader.py
--rw-rw-rw-   0        0        0     3563 2023-05-14 13:31:31.000000 irails-1.3.14/irails/_utils.py
--rw-rw-rw-   0        0        0    11802 2023-05-13 14:57:32.000000 irails-1.3.14/irails/auth.py
--rw-rw-rw-   0        0        0    12679 2023-05-13 15:01:43.000000 irails-1.3.14/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.975245 irails-1.3.14/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.976243 irails-1.3.14/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.14/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.14/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.14/irails/cbv.py
--rw-rw-rw-   0        0        0     6118 2023-05-15 06:53:38.000000 irails-1.3.14/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.14/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24553 2023-05-15 08:05:16.000000 irails-1.3.14/irails/core.py
--rw-rw-rw-   0        0        0     6903 2023-05-14 14:13:03.000000 irails-1.3.14/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.14/irails/log.py
--rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.14/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.14/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.14/irails/midware_session.py
--rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.14/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.987213 irails-1.3.14/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.14/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.14/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6898 2023-05-14 13:32:08.000000 irails-1.3.14/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.14/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.14/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.14/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.14/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.14/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4042 2023-05-15 06:46:20.000000 irails-1.3.14/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2426 2023-05-15 07:00:43.000000 irails-1.3.14/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.931362 irails-1.3.14/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.999182 irails-1.3.14/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.14/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.14/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.14/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.14/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0      999 2023-05-14 14:07:15.000000 irails-1.3.14/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1014 2023-05-14 14:04:24.000000 irails-1.3.14/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.14/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.14/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.14/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.002174 irails-1.3.14/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.14/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.004168 irails-1.3.14/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.14/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.016135 irails-1.3.14/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.14/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.14/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.14/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.14/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.14/irails/scripts/tpls/project/configs/casbin-model.conf
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.14/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.14/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.14/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.14/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.933357 irails-1.3.14/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.022121 irails-1.3.14/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.14/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.14/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.14/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.14/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.025112 irails-1.3.14/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.14/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.14/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.029107 irails-1.3.14/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.936350 irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.032093 irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.037080 irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.14/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.14/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.937347 irails-1.3.14/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:27.039076 irails-1.3.14/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.14/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.14/irails/unit_test.py
--rw-rw-rw-   0        0        0     2887 2023-05-12 05:35:40.000000 irails-1.3.14/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-15 09:30:26.972253 irails-1.3.14/irails.egg-info/
--rw-rw-rw-   0        0        0     5518 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2455 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      777 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-15 09:30:26.000000 irails-1.3.14/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 09:30:27.044062 irails-1.3.14/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.14/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.062375 irails-1.3.15/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     5518 2023-05-15 11:56:31.061379 irails-1.3.15/PKG-INFO
+-rw-rw-rw-   0        0        0     4734 2023-05-15 07:02:13.000000 irails-1.3.15/README.md
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.975525 irails-1.3.15/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-15 11:56:20.000000 irails-1.3.15/irails/__init__.py
+-rw-rw-rw-   0        0        0     3409 2023-05-13 06:08:26.000000 irails-1.3.15/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2883 2023-05-15 06:36:25.000000 irails-1.3.15/irails/_loader.py
+-rw-rw-rw-   0        0        0     3563 2023-05-14 13:31:31.000000 irails-1.3.15/irails/_utils.py
+-rw-rw-rw-   0        0        0    11802 2023-05-13 14:57:32.000000 irails-1.3.15/irails/auth.py
+-rw-rw-rw-   0        0        0    12679 2023-05-13 15:01:43.000000 irails-1.3.15/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.988142 irails-1.3.15/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.990125 irails-1.3.15/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.15/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.15/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.15/irails/cbv.py
+-rw-rw-rw-   0        0        0     6118 2023-05-15 06:53:38.000000 irails-1.3.15/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.15/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24553 2023-05-15 08:05:16.000000 irails-1.3.15/irails/core.py
+-rw-rw-rw-   0        0        0     6903 2023-05-14 14:13:03.000000 irails-1.3.15/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.15/irails/log.py
+-rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.15/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.15/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9341 2023-05-11 15:20:39.000000 irails-1.3.15/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4200 2023-04-27 11:53:07.000000 irails-1.3.15/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.003846 irails-1.3.15/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.15/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.15/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6898 2023-05-14 13:32:08.000000 irails-1.3.15/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.15/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.15/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.15/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.15/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.15/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4042 2023-05-15 06:46:20.000000 irails-1.3.15/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2426 2023-05-15 07:00:43.000000 irails-1.3.15/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.933583 irails-1.3.15/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.017513 irails-1.3.15/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.15/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.15/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.15/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.15/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0      999 2023-05-14 14:07:15.000000 irails-1.3.15/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1014 2023-05-14 14:04:24.000000 irails-1.3.15/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.15/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.15/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.15/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.020489 irails-1.3.15/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.15/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.022483 irails-1.3.15/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.15/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.036445 irails-1.3.15/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.15/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.15/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.15/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.15/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.15/irails/scripts/tpls/project/configs/casbin-model.conf
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.15/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.15/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.15/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.15/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.936577 irails-1.3.15/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.042439 irails-1.3.15/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.15/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.15/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.045421 irails-1.3.15/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.15/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.15/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.048412 irails-1.3.15/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.939569 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.051406 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.056393 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.941563 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:31.059384 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.15/irails/unit_test.py
+-rw-rw-rw-   0        0        0     2887 2023-05-12 05:35:40.000000 irails-1.3.15/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-15 11:56:30.985140 irails-1.3.15/irails.egg-info/
+-rw-rw-rw-   0        0        0     5518 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2455 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      340 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-15 11:56:30.000000 irails-1.3.15/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 11:56:31.062375 irails-1.3.15/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.15/setup.py
```

### Comparing `irails-1.3.14/PKG-INFO` & `irails-1.3.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.14
+Version: 1.3.15
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.14/README.md` & `irails-1.3.15/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/_i18n.py` & `irails-1.3.15/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/_loader.py` & `irails-1.3.15/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/_utils.py` & `irails-1.3.15/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/auth.py` & `irails-1.3.15/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/base_controller.py` & `irails-1.3.15/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.15/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.15/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/cbv.py` & `irails-1.3.15/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/config.py` & `irails-1.3.15/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/controller_utils.py` & `irails-1.3.15/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/core.py` & `irails-1.3.15/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/database.py` & `irails-1.3.15/irails/database.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/log.py` & `irails-1.3.15/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/midware.py` & `irails-1.3.15/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/midware_casbin.py` & `irails-1.3.15/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/midware_session.py` & `irails-1.3.15/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/mvc_router.py` & `irails-1.3.15/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_app.py` & `irails-1.3.15/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_controller.py` & `irails-1.3.15/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_i18n.py` & `irails-1.3.15/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_model.py` & `irails-1.3.15/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_project.py` & `irails-1.3.15/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_run.py` & `irails-1.3.15/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_shell.py` & `irails-1.3.15/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/_test.py` & `irails-1.3.15/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/main.py` & `irails-1.3.15/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.15/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/app/home.tpl` & `irails-1.3.15/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/app/model.jinja` & `irails-1.3.15/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/app/service.jinja` & `irails-1.3.15/irails/scripts/tpls/app/service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.15/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.15/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.15/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.15/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.15/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.15/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.15/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.15/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.15/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.15/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/unit_test.py` & `irails-1.3.15/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails/view.py` & `irails-1.3.15/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/irails.egg-info/PKG-INFO` & `irails-1.3.15/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.14
+Version: 1.3.15
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.14/irails.egg-info/SOURCES.txt` & `irails-1.3.15/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.14/setup.py` & `irails-1.3.15/setup.py`

 * *Files identical despite different names*

