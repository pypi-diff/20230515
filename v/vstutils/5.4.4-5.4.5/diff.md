# Comparing `tmp/vstutils-5.4.4.tar.gz` & `tmp/vstutils-5.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vstutils-5.4.4.tar", last modified: Fri May 12 21:40:56 2023, max compression
+gzip compressed data, was "vstutils-5.4.5.tar", last modified: Mon May 15 04:02:29 2023, max compression
```

## Comparing `vstutils-5.4.4.tar` & `vstutils-5.4.5.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/
--rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.4/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.4/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.4/NOTICE
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-12 21:40:56.159942 vstutils-5.4.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.4/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-18 02:33:32.000000 vstutils-5.4.4/requirements-doc.txt
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.4/requirements-git.txt
--rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.4/requirements-ldap.txt
--rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-13 03:48:29.000000 vstutils-5.4.4/requirements-prod.txt
--rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.4/requirements-rpc.txt
--rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.4/requirements-stubs.txt
--rw-rw-rw-   0 root         (0) root         (0)      135 2023-04-13 03:48:29.000000 vstutils-5.4.4/requirements-test.txt
--rw-rw-rw-   0 root         (0) root         (0)      539 2023-03-20 21:33:20.000000 vstutils-5.4.4/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-12 21:40:56.159942 vstutils-5.4.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.123942 vstutils-5.4.4/vstutils/
--rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-11 10:56:05.000000 vstutils-5.4.4/vstutils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.127942 vstutils-5.4.4/vstutils/api/
--rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/actions.py
--rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/apps.py
--rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/auth.py
--rw-rw-rw-   0 root         (0) root         (0)    27865 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)    24054 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/api/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/decorators.pyi
--rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/doc_generator.py
--rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.4/vstutils/api/endpoint.py
--rw-rw-rw-   0 root         (0) root         (0)    51728 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/api/fields.py
--rw-rw-rw-   0 root         (0) root         (0)    11397 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/filter_backends.py
--rw-rw-rw-   0 root         (0) root         (0)     4991 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/filters.py
--rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/health.py
--rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/meta.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/api/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0002_two_factor.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0003_tfa_indexes.py
--rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0004_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0005_db_translations.py
--rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/0006_fix_user_settings.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/models.py
--rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/renderers.py
--rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/responses.py
--rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/responses.pyi
--rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/routers.py
--rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/routers.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/api/schema/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/schema/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/schema/generators.py
--rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/api/schema/info.py
--rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.4/vstutils/api/schema/inspectors.py
--rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/schema/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/schema/views.py
--rw-rw-rw-   0 root         (0) root         (0)     7340 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/api/serializers.py
--rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/throttling.py
--rw-rw-rw-   0 root         (0) root         (0)    10784 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/views.py
--rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/api/views.pyi
--rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.4/vstutils/asgi.py
--rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/asgi_worker.py
--rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/auth.py
--rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/auth.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/celery_beat_scheduler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.111942 vstutils-5.4.4/vstutils/doc_themes/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/
--rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/layout.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/static/
--rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-12 21:40:56.167942 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
--rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/theme.conf
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/environment.py
--rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/environment.pyi
--rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/gui/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3476 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/context.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/gui/pwa_manifest.py
--rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/gui/views.py
--rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/ldap_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.131942 vstutils-5.4.4/vstutils/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.135942 vstutils-5.4.4/vstutils/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.4/vstutils/management/commands/_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/celery_inspect.py
--rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/dockermigrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/dockerrun.py
--rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/management/commands/newproject.py
--rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/run_task.py
--rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/management/commands/runrpc.py
--rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.4/vstutils/management/commands/runserver.py
--rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/management/commands/web.py
--rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.135942 vstutils-5.4.4/vstutils/models/
--rw-rw-rw-   0 root         (0) root         (0)    10704 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/models/cent_notify.py
--rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/models/custom_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/models/custom_model.pyi
--rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     7971 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/fields.py
--rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/model.py
--rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/models/queryset.py
--rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/session.py
--rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/settings.ini
--rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.4/vstutils/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.115942 vstutils-5.4.4/vstutils/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/bundle/
--rw-r--r--   0 root         (0) root         (0)      155 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/157.chunk.js
--rw-r--r--   0 root         (0) root         (0)   126295 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/281.chunk.js
--rw-r--r--   0 root         (0) root         (0)      171 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/281.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/296.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/296.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   136100 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/345.chunk.js
--rw-r--r--   0 root         (0) root         (0)    15726 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/368.chunk.js
--rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/421.js
--rw-r--r--   0 root         (0) root         (0)     1500 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/421.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      321 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/463.chunk.js
--rw-r--r--   0 root         (0) root         (0)      330 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/564.chunk.js
--rw-r--r--   0 root         (0) root         (0)    38336 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/618.js
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/618.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     2235 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/683.chunk.js
--rw-r--r--   0 root         (0) root         (0)      151 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/683.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    71086 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/686.js
--rw-r--r--   0 root         (0) root         (0)   536206 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/742.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    89997 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/755.js
--rw-r--r--   0 root         (0) root         (0)      476 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/755.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   355788 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/826.chunk.js
--rw-r--r--   0 root         (0) root         (0)     1142 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)   177828 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/844.js
--rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/959.js
--rw-r--r--   0 root         (0) root         (0)     2191 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils/static/bundle/959.js.LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)    77026 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/app_loader.js
--rw-r--r--   0 root         (0) root         (0)   303656 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/base.js
--rw-r--r--   0 root         (0) root         (0)    16276 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
--rw-r--r--   0 root         (0) root         (0)   101648 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
--rw-r--r--   0 root         (0) root         (0)      748 2023-05-12 21:40:55.000000 vstutils-5.4.4/vstutils/static/bundle/output.json
--rw-r--r--   0 root         (0) root         (0)     3597 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/spa.js
--rw-r--r--   0 root         (0) root         (0)   432610 2023-05-12 21:39:45.000000 vstutils-5.4.4/vstutils/static/bundle/vstutils.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/img/
--rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static/img/anonymous.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/static/img/logo/
--rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static/img/logo/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/static_files.py
--rw-rw-rw-   0 root         (0) root         (0)     5181 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.147942 vstutils-5.4.4/vstutils/templates/
--rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/400.html
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/403.html
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/404.html
--rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.4/vstutils/templates/500.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/auth/
--rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/base.html
--rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/language_selector.html
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/login.html
--rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/auth/tfa.html
--rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.4/vstutils/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.4/vstutils/templates/base_error.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/configs/
--rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/configs/config.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/drf-yasg/
--rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/drf-yasg/swagger-ui.html
--rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.4/vstutils/templates/go_back_button.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.151942 vstutils-5.4.4/vstutils/templates/gui/
--rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/base.html
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/gui.html
--rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/manifest.json
--rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/offline.html
--rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/gui/service-worker.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/
--rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.coveragerc.template
--rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.gitignore.template
--rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/.pep8.template
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/MANIFEST.in.template
--rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/README.rst.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/
--rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.babelrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.editorconfig.template
--rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
--rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.prettierrc.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/app/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/frontend_src/app/index.js.template
--rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/package.json.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/project_name/
--rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/__main__.py.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/newproject/project_name/models/
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/models/__init__.py.template
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.py.template
--rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/web.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/project_name/wsgi.py.template
--rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/requirements-test.txt.template
--rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/requirements.txt.template
--rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/setup.cfg.template
--rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.4/vstutils/templates/newproject/setup.py.template
--rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/test.py.template
--rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/tox.ini.template
--rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/tox_build.ini.template
--rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/newproject/webpack.config.js.default.template
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/base.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/base_agreements.html
--rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.4/vstutils/templates/registration/confirm_email.html
--rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/registration/user_registration.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.155942 vstutils-5.4.4/vstutils/templates/rest_framework/
--rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/rest_framework/admin.html
--rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
--rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templates/widgets/
--rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templates/widgets/agreement_widget.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/templatetags/request_static.py
--rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/translation.py
--rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/vst_gravatar.py
--rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.4/vstutils/templatetags/vst_html_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/templatetags/vstconfigs.py
--rw-rw-rw-   0 root         (0) root         (0)    17731 2023-02-13 06:24:20.000000 vstutils-5.4.4/vstutils/tests.py
--rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.159942 vstutils-5.4.4/vstutils/translations/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/translations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/cn.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/translations/en.py
--rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/ru.py
--rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.4/vstutils/translations/vi.py
--rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/urls.py
--rw-rw-rw-   0 root         (0) root         (0)    44646 2023-02-09 12:14:31.000000 vstutils-5.4.4/vstutils/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.4/vstutils/web.ini
--rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.4/vstutils/wsgi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-12 21:40:56.123942 vstutils-5.4.4/vstutils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4459 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7644 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       85 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-12 21:39:46.000000 vstutils-5.4.4/vstutils.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-12 21:40:56.000000 vstutils-5.4.4/vstutils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.814547 vstutils-5.4.5/
+-rw-rw-rw-   0 root         (0) root         (0)    11344 2022-12-19 05:43:06.000000 vstutils-5.4.5/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)      770 2023-02-03 10:03:13.000000 vstutils-5.4.5/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      592 2023-03-29 01:47:58.000000 vstutils-5.4.5/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-15 04:02:29.814547 vstutils-5.4.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2393 2022-12-19 05:43:06.000000 vstutils-5.4.5/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-03-18 02:33:32.000000 vstutils-5.4.5/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-12-19 05:43:06.000000 vstutils-5.4.5/requirements-git.txt
+-rw-rw-rw-   0 root         (0) root         (0)       51 2022-12-19 05:43:06.000000 vstutils-5.4.5/requirements-ldap.txt
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-05-13 04:11:10.000000 vstutils-5.4.5/requirements-prod.txt
+-rw-rw-rw-   0 root         (0) root         (0)       83 2023-03-18 02:33:32.000000 vstutils-5.4.5/requirements-rpc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      231 2023-03-29 01:47:58.000000 vstutils-5.4.5/requirements-stubs.txt
+-rw-rw-rw-   0 root         (0) root         (0)      135 2023-05-13 04:11:10.000000 vstutils-5.4.5/requirements-test.txt
+-rw-rw-rw-   0 root         (0) root         (0)      538 2023-05-13 04:11:10.000000 vstutils-5.4.5/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2313 2023-05-15 04:02:29.814547 vstutils-5.4.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)    16893 2023-04-13 03:48:29.000000 vstutils-5.4.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.770546 vstutils-5.4.5/vstutils/
+-rw-rw-rw-   0 root         (0) root         (0)       66 2023-05-13 04:11:10.000000 vstutils-5.4.5/vstutils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      158 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.778546 vstutils-5.4.5/vstutils/api/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15370 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/api/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1492 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/api/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      413 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)    13063 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)    27828 2023-05-13 04:11:10.000000 vstutils-5.4.5/vstutils/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    24054 2023-02-13 06:24:20.000000 vstutils-5.4.5/vstutils/api/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/api/decorators.pyi
+-rw-rw-rw-   0 root         (0) root         (0)    15852 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/doc_generator.py
+-rw-rw-rw-   0 root         (0) root         (0)    18802 2023-02-07 05:18:57.000000 vstutils-5.4.5/vstutils/api/endpoint.py
+-rw-rw-rw-   0 root         (0) root         (0)    51728 2023-03-15 02:43:46.000000 vstutils-5.4.5/vstutils/api/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)    11754 2023-05-13 04:11:10.000000 vstutils-5.4.5/vstutils/api/filter_backends.py
+-rw-rw-rw-   0 root         (0) root         (0)     4991 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/filters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2531 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/health.py
+-rw-rw-rw-   0 root         (0) root         (0)      574 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/meta.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.782546 vstutils-5.4.5/vstutils/api/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      554 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)     1285 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0002_two_factor.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0003_tfa_indexes.py
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0004_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      866 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0005_db_translations.py
+-rw-rw-rw-   0 root         (0) root         (0)      698 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/0006_fix_user_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/models.py
+-rw-rw-rw-   0 root         (0) root         (0)      869 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1509 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1596 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/renderers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/responses.py
+-rw-rw-rw-   0 root         (0) root         (0)    10364 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/responses.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     9015 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/routers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1998 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/api/routers.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.782546 vstutils-5.4.5/vstutils/api/schema/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/schema/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5850 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/schema/generators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1649 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/api/schema/info.py
+-rw-rw-rw-   0 root         (0) root         (0)    26465 2023-03-17 01:28:59.000000 vstutils-5.4.5/vstutils/api/schema/inspectors.py
+-rw-rw-rw-   0 root         (0) root         (0)     9648 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/schema/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      253 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/schema/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     7340 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/api/serializers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2289 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/throttling.py
+-rw-rw-rw-   0 root         (0) root         (0)    10784 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     5660 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      255 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/api/views.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     1363 2023-02-20 07:13:28.000000 vstutils-5.4.5/vstutils/asgi.py
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2023-02-13 06:24:20.000000 vstutils-5.4.5/vstutils/asgi_worker.py
+-rw-rw-rw-   0 root         (0) root         (0)     4232 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/auth.py
+-rw-rw-rw-   0 root         (0) root         (0)     2162 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/auth.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2790 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/celery_beat_scheduler.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.758546 vstutils-5.4.5/vstutils/doc_themes/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.782546 vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/
+-rw-rw-rw-   0 root         (0) root         (0)      927 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/layout.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.782546 vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/static/
+-rw-rw-rw-   0 root         (0) root         (0)      172 2023-05-15 04:02:29.822547 vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/static/basic.css
+-rw-rw-rw-   0 root         (0) root         (0)      147 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/theme.conf
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/environment.py
+-rw-rw-rw-   0 root         (0) root         (0)      355 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/environment.pyi
+-rw-rw-rw-   0 root         (0) root         (0)      743 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.782546 vstutils-5.4.5/vstutils/gui/
+-rwxrwxrwx   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3476 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/gui/context.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1026 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/gui/pwa_manifest.py
+-rw-rw-rw-   0 root         (0) root         (0)     5023 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/gui/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     6436 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/ldap_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.786547 vstutils-5.4.5/vstutils/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.786547 vstutils-5.4.5/vstutils/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7832 2023-03-16 06:05:23.000000 vstutils-5.4.5/vstutils/management/commands/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/celery_inspect.py
+-rw-rw-rw-   0 root         (0) root         (0)      367 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/dockermigrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1167 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/dockerrun.py
+-rw-rw-rw-   0 root         (0) root         (0)     4975 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/management/commands/newproject.py
+-rw-rw-rw-   0 root         (0) root         (0)     1670 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/run_task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1165 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/management/commands/runrpc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2023-03-17 01:28:59.000000 vstutils-5.4.5/vstutils/management/commands/runserver.py
+-rw-rw-rw-   0 root         (0) root         (0)     7286 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/management/commands/web.py
+-rw-rw-rw-   0 root         (0) root         (0)    10646 2023-02-13 06:24:20.000000 vstutils-5.4.5/vstutils/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.790547 vstutils-5.4.5/vstutils/models/
+-rw-rw-rw-   0 root         (0) root         (0)    10704 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    25308 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/models/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4130 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/models/cent_notify.py
+-rw-rw-rw-   0 root         (0) root         (0)    11620 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/models/custom_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2534 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/models/custom_model.pyi
+-rw-rw-rw-   0 root         (0) root         (0)     2344 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/models/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     7971 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/models/fields.py
+-rw-rw-rw-   0 root         (0) root         (0)      293 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/models/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     8200 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/models/queryset.py
+-rw-rw-rw-   0 root         (0) root         (0)       64 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)      472 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/session.py
+-rw-rw-rw-   0 root         (0) root         (0)     4270 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/settings.ini
+-rw-rw-rw-   0 root         (0) root         (0)    54947 2023-04-13 03:48:29.000000 vstutils-5.4.5/vstutils/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.762546 vstutils-5.4.5/vstutils/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.798547 vstutils-5.4.5/vstutils/static/bundle/
+-rw-r--r--   0 root         (0) root         (0)      155 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/157.chunk.js
+-rw-r--r--   0 root         (0) root         (0)   126295 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/281.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      171 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/281.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/296.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/296.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   136100 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/345.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    15726 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/368.chunk.js
+-rw-r--r--   0 root         (0) root         (0)  1066719 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/421.js
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/421.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/463.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      330 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/564.chunk.js
+-rw-r--r--   0 root         (0) root         (0)    38336 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/618.js
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/618.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     2235 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/683.chunk.js
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/683.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    71086 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/686.js
+-rw-r--r--   0 root         (0) root         (0)   536206 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/742.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/742.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    89997 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/755.js
+-rw-r--r--   0 root         (0) root         (0)      476 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/755.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   355788 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/826.chunk.js
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/826.chunk.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)   177828 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/844.js
+-rw-r--r--   0 root         (0) root         (0)  1798980 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/959.js
+-rw-r--r--   0 root         (0) root         (0)     2191 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/959.js.LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)    77026 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/app_loader.js
+-rw-r--r--   0 root         (0) root         (0)   303656 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/base.js
+-rw-r--r--   0 root         (0) root         (0)    16276 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/bb58e57c48a3e911f15f.woff
+-rw-r--r--   0 root         (0) root         (0)   101648 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff
+-rw-r--r--   0 root         (0) root         (0)      748 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils/static/bundle/output.json
+-rw-r--r--   0 root         (0) root         (0)     3597 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/spa.js
+-rw-r--r--   0 root         (0) root         (0)   432610 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils/static/bundle/vstutils.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.798547 vstutils-5.4.5/vstutils/static/img/
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/static/img/anonymous.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/static/img/logo/
+-rw-rw-rw-   0 root         (0) root         (0)      384 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/static/img/logo/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     2203 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/static_files.py
+-rw-rw-rw-   0 root         (0) root         (0)     5181 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/tasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      262 2023-02-21 08:49:07.000000 vstutils-5.4.5/vstutils/templates/400.html
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-02-21 08:49:07.000000 vstutils-5.4.5/vstutils/templates/403.html
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-02-21 08:49:07.000000 vstutils-5.4.5/vstutils/templates/404.html
+-rw-rw-rw-   0 root         (0) root         (0)      183 2023-02-21 08:00:17.000000 vstutils-5.4.5/vstutils/templates/500.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/templates/auth/
+-rwxrwxrwx   0 root         (0) root         (0)     2568 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/auth/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      729 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/auth/language_selector.html
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/auth/login.html
+-rw-rw-rw-   0 root         (0) root         (0)     1240 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/auth/tfa.html
+-rwxrwxrwx   0 root         (0) root         (0)     2845 2023-02-21 08:00:17.000000 vstutils-5.4.5/vstutils/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      313 2023-02-21 06:43:08.000000 vstutils-5.4.5/vstutils/templates/base_error.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/templates/configs/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/configs/config.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/templates/drf-yasg/
+-rw-rw-rw-   0 root         (0) root         (0)      134 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/drf-yasg/swagger-ui.html
+-rw-rw-rw-   0 root         (0) root         (0)      434 2023-02-21 08:49:07.000000 vstutils-5.4.5/vstutils/templates/go_back_button.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.802547 vstutils-5.4.5/vstutils/templates/gui/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/gui/base.html
+-rwxrwxrwx   0 root         (0) root         (0)       29 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/gui/gui.html
+-rw-rw-rw-   0 root         (0) root         (0)      154 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/gui/manifest.json
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/gui/offline.html
+-rw-rw-rw-   0 root         (0) root         (0)     1531 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/gui/service-worker.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.806547 vstutils-5.4.5/vstutils/templates/newproject/
+-rw-rw-rw-   0 root         (0) root         (0)      280 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/.coveragerc.template
+-rw-rw-rw-   0 root         (0) root         (0)     2290 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/.gitignore.template
+-rw-rw-rw-   0 root         (0) root         (0)      235 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/.pep8.template
+-rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/MANIFEST.in.template
+-rw-rw-rw-   0 root         (0) root         (0)      445 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/README.rst.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.806547 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/.babelrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      157 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/.editorconfig.template
+-rw-rw-rw-   0 root         (0) root         (0)      794 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/.eslintrc.js.template
+-rw-rw-rw-   0 root         (0) root         (0)      449 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/.prettierrc.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.806547 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/app/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/frontend_src/app/index.js.template
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/package.json.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.810546 vstutils-5.4.5/vstutils/templates/newproject/project_name/
+-rw-rw-rw-   0 root         (0) root         (0)      496 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      115 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/__main__.py.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.810546 vstutils-5.4.5/vstutils/templates/newproject/project_name/models/
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/models/__init__.py.template
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/settings.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      565 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/settings.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       66 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/web.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      120 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/project_name/wsgi.py.template
+-rw-rw-rw-   0 root         (0) root         (0)       75 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/requirements-test.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)      101 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/requirements.txt.template
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/setup.cfg.template
+-rw-rw-rw-   0 root         (0) root         (0)    14520 2022-12-19 06:05:53.000000 vstutils-5.4.5/vstutils/templates/newproject/setup.py.template
+-rw-rw-rw-   0 root         (0) root         (0)      572 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/test.py.template
+-rw-rw-rw-   0 root         (0) root         (0)     2234 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/tox.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)      705 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/tox_build.ini.template
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/newproject/webpack.config.js.default.template
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.810546 vstutils-5.4.5/vstutils/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/base_agreements.html
+-rw-rw-rw-   0 root         (0) root         (0)    11731 2022-12-29 11:28:36.000000 vstutils-5.4.5/vstutils/templates/registration/confirm_email.html
+-rw-rw-rw-   0 root         (0) root         (0)      352 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1618 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      463 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      831 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     1736 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/registration/user_registration.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.810546 vstutils-5.4.5/vstutils/templates/rest_framework/
+-rw-rw-rw-   0 root         (0) root         (0)     9228 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/rest_framework/admin.html
+-rw-rw-rw-   0 root         (0) root         (0)      225 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/rest_framework/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.810546 vstutils-5.4.5/vstutils/templates/vst_inclusion_tags/
+-rw-rw-rw-   0 root         (0) root         (0)      107 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/vst_inclusion_tags/b64_img_from_json_string.html
+-rw-rw-rw-   0 root         (0) root         (0)      834 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/vst_inclusion_tags/bootstrap_form.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.814547 vstutils-5.4.5/vstutils/templates/widgets/
+-rw-rw-rw-   0 root         (0) root         (0)     1405 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templates/widgets/agreement_widget.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.814547 vstutils-5.4.5/vstutils/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/templatetags/request_static.py
+-rw-rw-rw-   0 root         (0) root         (0)     2866 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templatetags/translation.py
+-rw-rw-rw-   0 root         (0) root         (0)      823 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templatetags/vst_gravatar.py
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2023-02-03 10:03:13.000000 vstutils-5.4.5/vstutils/templatetags/vst_html_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1133 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/templatetags/vstconfigs.py
+-rw-rw-rw-   0 root         (0) root         (0)    17731 2023-02-13 06:24:20.000000 vstutils-5.4.5/vstutils/tests.py
+-rw-rw-rw-   0 root         (0) root         (0)      612 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.814547 vstutils-5.4.5/vstutils/translations/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/translations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16196 2023-03-15 02:43:46.000000 vstutils-5.4.5/vstutils/translations/cn.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/translations/en.py
+-rw-rw-rw-   0 root         (0) root         (0)    23941 2023-03-15 02:43:46.000000 vstutils-5.4.5/vstutils/translations/ru.py
+-rw-rw-rw-   0 root         (0) root         (0)    18983 2023-03-15 02:43:46.000000 vstutils-5.4.5/vstutils/translations/vi.py
+-rw-rw-rw-   0 root         (0) root         (0)     2721 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)    44730 2023-05-13 04:11:10.000000 vstutils-5.4.5/vstutils/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-02-06 06:25:26.000000 vstutils-5.4.5/vstutils/web.ini
+-rw-rw-rw-   0 root         (0) root         (0)      843 2022-12-19 05:43:06.000000 vstutils-5.4.5/vstutils/wsgi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 04:02:29.774546 vstutils-5.4.5/vstutils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4459 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7644 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       85 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 04:01:14.000000 vstutils-5.4.5/vstutils.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-15 04:02:29.000000 vstutils-5.4.5/vstutils.egg-info/top_level.txt
```

### Comparing `vstutils-5.4.4/LICENSE` & `vstutils-5.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/MANIFEST.in` & `vstutils-5.4.5/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/NOTICE` & `vstutils-5.4.5/NOTICE`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/PKG-INFO` & `vstutils-5.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.4
+Version: 5.4.5
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.4/README.rst` & `vstutils-5.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/requirements.txt` & `vstutils-5.4.5/requirements.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # Main packages
 configparser~=5.3.0
-configparserc~=1.3.4
-django-cors-headers~=3.13.0
+configparserc~=1.4.0
+django-cors-headers~=4.0.0
 Markdown==3.4.1
 django-environ~=0.10.0
 
 # REST API packages
 djangorestframework~=3.14.0
 drf-yasg==1.21.5
 MarkupSafe==2.0.1  # Fix coreschema
-django-filter==22.1
+django-filter==23.2
 django-crispy-forms~=1.14.0
 drf_orjson_renderer~=1.7.1
-ormsgpack==1.2.5
+ormsgpack==1.2.6
 
 # web server
-uvicorn~=0.21.0
+uvicorn~=0.22.0
 pyuwsgi==2.0.21
-fastapi~=0.95.0
+fastapi~=0.95.1
 
 # Notifications
 cent~=4.1.0
-PyJWT~=2.6.0
+PyJWT~=2.7.0
 
 # Minificators
 jsmin~=3.0.1
 django-htmlmin~=0.11.0
 
 # 2fa
 pyotp~=2.8.0
```

### Comparing `vstutils-5.4.4/setup.cfg` & `vstutils-5.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/setup.py` & `vstutils-5.4.5/setup.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/actions.py` & `vstutils-5.4.5/vstutils/api/actions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/admin.py` & `vstutils-5.4.5/vstutils/api/admin.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/auth.py` & `vstutils-5.4.5/vstutils/api/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/base.py` & `vstutils-5.4.5/vstutils/api/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,27 @@
 from django.conf import settings
 from django.core import exceptions as djexcs
 from django.http.response import Http404, FileResponse, HttpResponseNotModified
 from django.db.models.query import QuerySet
 from django.db import transaction, models
 from django.utils.functional import cached_property, lazy
 from django.utils.http import urlencode
+from django.contrib.contenttypes.fields import GenericForeignKey
 from rest_framework.reverse import reverse
 from rest_framework import viewsets as vsets, views as rvs, mixins as drf_mixins, exceptions, status
 from rest_framework.serializers import BaseSerializer
 from rest_framework.response import Response as RestResponse
 from rest_framework.request import Request
 from rest_framework.decorators import action
 from rest_framework.schemas import AutoSchema as DRFAutoSchema
 from rest_framework.utils.serializer_helpers import ReturnList, ReturnDict
 
 from ..utils import classproperty, get_if_lazy, raise_context_decorator_with_default, patch_gzip_response_decorator
 from . import responses, fields
+from .filter_backends import get_serializer_readable_fields
 from .serializers import (
     ErrorSerializer,
     ValidationErrorSerializer,
     OtherErrorsSerializer,
     serializers
 )
 
@@ -333,27 +335,21 @@
         qs = super().filter_queryset(queryset)
 
         if self.action in ('list', 'retrieve') + self.optimize_get_by_values_actions and self.optimize_get_by_values:
             # pylint: disable=protected-access
 
             serializer_class = self.get_serializer_class()
             if issubclass(serializer_class, BaseSerializer):
-                serializer = serializer_class()
-                read_fields = {
-                    f.source if f.source and '.' not in f.source else f.field_name
-                    for f in serializer._readable_fields
-                }
-                model_fields = {
-                    f.name
-                    for f in queryset.model._meta.get_fields()
-                }
+                read_fields = get_serializer_readable_fields(serializer_class())
+                _fields = queryset.model._meta.get_fields()
+                model_fields = {f.name for f in _fields}
                 fk_related_fields = {
                     f.name
-                    for f in queryset.model._meta.get_fields()
-                    if isinstance(f, models.ForeignKey)
+                    for f in _fields
+                    if isinstance(f, (models.ForeignKey, models.ManyToManyField, GenericForeignKey))
                 }
                 deferable_fields = (
                         model_fields -
                         read_fields -
                         fk_related_fields -
                         set(getattr(queryset.model, '_required_fields', None) or set())
                 )
```

### Comparing `vstutils-5.4.4/vstutils/api/decorators.py` & `vstutils-5.4.5/vstutils/api/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/decorators.pyi` & `vstutils-5.4.5/vstutils/api/decorators.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/doc_generator.py` & `vstutils-5.4.5/vstutils/api/doc_generator.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/endpoint.py` & `vstutils-5.4.5/vstutils/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/fields.py` & `vstutils-5.4.5/vstutils/api/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/filter_backends.py` & `vstutils-5.4.5/vstutils/api/filter_backends.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,22 @@
 from django_filters.rest_framework.backends import DjangoFilterBackend as BaseDjangoFilterBackend
 from django_filters import compat, filters, filterset
 from vstutils.utils import raise_context, translate as _
 
 from .filters import extra_filter
 
 
+def get_serializer_readable_fields(serializer):
+    # pylint: disable=protected-access
+    return {
+        f.source if f.source and '.' not in f.source else f.field_name
+        for f in serializer._readable_fields
+    }
+
+
 class DjangoFilterBackend(BaseDjangoFilterBackend):
     def get_coreschema_field(self, field):
         kwargs = {
             'description': str(field.extra.get('help_text', '')),
         }
         if isinstance(field, filters.NumberFilter):
             field_cls = compat.coreschema.Number
@@ -151,18 +159,20 @@
     required = True
     fields_fetch_map = {
         'select': (models.ForeignKey,),
         'prefetch': (models.ManyToManyField, models.ManyToManyField.rel_class)
     }
 
     def filter_model_fields(self, view, field_types):
+        serializer = view.get_serializer_class()()
+        readable_fields = get_serializer_readable_fields(serializer)
         return tuple(
             f.name
-            for f in view.get_serializer_class().Meta.model()._meta.fields
-            if isinstance(f, field_types)
+            for f in serializer.Meta.model()._meta.fields
+            if isinstance(f, field_types) and f.name in readable_fields
         )
 
     def filter_by_func(self, queryset, queryset_func_name, related):
         if related:
             return getattr(queryset, queryset_func_name)(*related)
         return queryset
```

### Comparing `vstutils-5.4.4/vstutils/api/filters.py` & `vstutils-5.4.5/vstutils/api/filters.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/health.py` & `vstutils-5.4.5/vstutils/api/health.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/meta.py` & `vstutils-5.4.5/vstutils/api/meta.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/metrics.py` & `vstutils-5.4.5/vstutils/api/metrics.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0001_initial.py` & `vstutils-5.4.5/vstutils/api/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0002_two_factor.py` & `vstutils-5.4.5/vstutils/api/migrations/0002_two_factor.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0003_tfa_indexes.py` & `vstutils-5.4.5/vstutils/api/migrations/0003_tfa_indexes.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0004_user_settings.py` & `vstutils-5.4.5/vstutils/api/migrations/0004_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0005_db_translations.py` & `vstutils-5.4.5/vstutils/api/migrations/0005_db_translations.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/migrations/0006_fix_user_settings.py` & `vstutils-5.4.5/vstutils/api/migrations/0006_fix_user_settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/models.py` & `vstutils-5.4.5/vstutils/api/models.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/pagination.py` & `vstutils-5.4.5/vstutils/api/pagination.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/parsers.py` & `vstutils-5.4.5/vstutils/api/parsers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/permissions.py` & `vstutils-5.4.5/vstutils/api/permissions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/renderers.py` & `vstutils-5.4.5/vstutils/api/renderers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/responses.py` & `vstutils-5.4.5/vstutils/api/responses.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/responses.pyi` & `vstutils-5.4.5/vstutils/api/responses.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/routers.py` & `vstutils-5.4.5/vstutils/api/routers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/routers.pyi` & `vstutils-5.4.5/vstutils/api/routers.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/schema/generators.py` & `vstutils-5.4.5/vstutils/api/schema/generators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/schema/info.py` & `vstutils-5.4.5/vstutils/api/schema/info.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/schema/inspectors.py` & `vstutils-5.4.5/vstutils/api/schema/inspectors.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/schema/schema.py` & `vstutils-5.4.5/vstutils/api/schema/schema.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/serializers.py` & `vstutils-5.4.5/vstutils/api/serializers.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/throttling.py` & `vstutils-5.4.5/vstutils/api/throttling.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/validators.py` & `vstutils-5.4.5/vstutils/api/validators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/api/views.py` & `vstutils-5.4.5/vstutils/api/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/asgi.py` & `vstutils-5.4.5/vstutils/asgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/asgi_worker.py` & `vstutils-5.4.5/vstutils/asgi_worker.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/auth.py` & `vstutils-5.4.5/vstutils/auth.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/auth.pyi` & `vstutils-5.4.5/vstutils/auth.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/celery_beat_scheduler.py` & `vstutils-5.4.5/vstutils/celery_beat_scheduler.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/doc_themes/vst-sphinx-theme/layout.html` & `vstutils-5.4.5/vstutils/doc_themes/vst-sphinx-theme/layout.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/environment.py` & `vstutils-5.4.5/vstutils/environment.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/exceptions.py` & `vstutils-5.4.5/vstutils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/gui/context.py` & `vstutils-5.4.5/vstutils/gui/context.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/gui/forms.py` & `vstutils-5.4.5/vstutils/gui/forms.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/gui/pwa_manifest.py` & `vstutils-5.4.5/vstutils/gui/pwa_manifest.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/gui/views.py` & `vstutils-5.4.5/vstutils/gui/views.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/ldap_utils.py` & `vstutils-5.4.5/vstutils/ldap_utils.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/_base.py` & `vstutils-5.4.5/vstutils/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/celery_inspect.py` & `vstutils-5.4.5/vstutils/management/commands/celery_inspect.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/dockerrun.py` & `vstutils-5.4.5/vstutils/management/commands/dockerrun.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/newproject.py` & `vstutils-5.4.5/vstutils/management/commands/newproject.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/run_task.py` & `vstutils-5.4.5/vstutils/management/commands/run_task.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/runrpc.py` & `vstutils-5.4.5/vstutils/management/commands/runrpc.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/runserver.py` & `vstutils-5.4.5/vstutils/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/management/commands/web.py` & `vstutils-5.4.5/vstutils/management/commands/web.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/middleware.py` & `vstutils-5.4.5/vstutils/middleware.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/__init__.py` & `vstutils-5.4.5/vstutils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/base.py` & `vstutils-5.4.5/vstutils/models/base.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/cent_notify.py` & `vstutils-5.4.5/vstutils/models/cent_notify.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/custom_model.py` & `vstutils-5.4.5/vstutils/models/custom_model.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/custom_model.pyi` & `vstutils-5.4.5/vstutils/models/custom_model.pyi`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/decorators.py` & `vstutils-5.4.5/vstutils/models/decorators.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/fields.py` & `vstutils-5.4.5/vstutils/models/fields.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/models/queryset.py` & `vstutils-5.4.5/vstutils/models/queryset.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/settings.ini` & `vstutils-5.4.5/vstutils/settings.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/settings.py` & `vstutils-5.4.5/vstutils/settings.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/281.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/281.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/296.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/296.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/345.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/345.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/368.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/368.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/421.js` & `vstutils-5.4.5/vstutils/static/bundle/421.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/421.js.LICENSE.txt` & `vstutils-5.4.5/vstutils/static/bundle/421.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/618.js` & `vstutils-5.4.5/vstutils/static/bundle/618.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/683.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/683.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/686.js` & `vstutils-5.4.5/vstutils/static/bundle/686.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/742.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/742.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/742.chunk.js.LICENSE.txt` & `vstutils-5.4.5/vstutils/static/bundle/742.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/755.js` & `vstutils-5.4.5/vstutils/static/bundle/755.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/826.chunk.js` & `vstutils-5.4.5/vstutils/static/bundle/826.chunk.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/826.chunk.js.LICENSE.txt` & `vstutils-5.4.5/vstutils/static/bundle/826.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/844.js` & `vstutils-5.4.5/vstutils/static/bundle/844.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/959.js` & `vstutils-5.4.5/vstutils/static/bundle/959.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/959.js.LICENSE.txt` & `vstutils-5.4.5/vstutils/static/bundle/959.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/app_loader.js` & `vstutils-5.4.5/vstutils/static/bundle/app_loader.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/base.js` & `vstutils-5.4.5/vstutils/static/bundle/base.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/bb58e57c48a3e911f15f.woff` & `vstutils-5.4.5/vstutils/static/bundle/bb58e57c48a3e911f15f.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff` & `vstutils-5.4.5/vstutils/static/bundle/eeccf4f66002c6f2ba24.woff`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/output.json` & `vstutils-5.4.5/vstutils/static/bundle/output.json`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/spa.js` & `vstutils-5.4.5/vstutils/static/bundle/spa.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/bundle/vstutils.js` & `vstutils-5.4.5/vstutils/static/bundle/vstutils.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static/img/anonymous.png` & `vstutils-5.4.5/vstutils/static/img/anonymous.png`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/static_files.py` & `vstutils-5.4.5/vstutils/static_files.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/tasks.py` & `vstutils-5.4.5/vstutils/tasks.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/auth/base.html` & `vstutils-5.4.5/vstutils/templates/auth/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/auth/language_selector.html` & `vstutils-5.4.5/vstutils/templates/auth/language_selector.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/auth/tfa.html` & `vstutils-5.4.5/vstutils/templates/auth/tfa.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/base.html` & `vstutils-5.4.5/vstutils/templates/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/gui/base.html` & `vstutils-5.4.5/vstutils/templates/gui/base.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/gui/offline.html` & `vstutils-5.4.5/vstutils/templates/gui/offline.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/gui/service-worker.js` & `vstutils-5.4.5/vstutils/templates/gui/service-worker.js`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/.gitignore.template` & `vstutils-5.4.5/vstutils/templates/newproject/.gitignore.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/frontend_src/.eslintrc.js.template` & `vstutils-5.4.5/vstutils/templates/newproject/frontend_src/.eslintrc.js.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/package.json.template` & `vstutils-5.4.5/vstutils/templates/newproject/package.json.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/project_name/settings.py.template` & `vstutils-5.4.5/vstutils/templates/newproject/project_name/settings.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/setup.cfg.template` & `vstutils-5.4.5/vstutils/templates/newproject/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/setup.py.template` & `vstutils-5.4.5/vstutils/templates/newproject/setup.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/test.py.template` & `vstutils-5.4.5/vstutils/templates/newproject/test.py.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/tox.ini.template` & `vstutils-5.4.5/vstutils/templates/newproject/tox.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/tox_build.ini.template` & `vstutils-5.4.5/vstutils/templates/newproject/tox_build.ini.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/newproject/webpack.config.js.default.template` & `vstutils-5.4.5/vstutils/templates/newproject/webpack.config.js.default.template`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/registration/confirm_email.html` & `vstutils-5.4.5/vstutils/templates/registration/confirm_email.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/registration/password_reset_confirm.html` & `vstutils-5.4.5/vstutils/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/registration/password_reset_form.html` & `vstutils-5.4.5/vstutils/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/registration/user_registration.html` & `vstutils-5.4.5/vstutils/templates/registration/user_registration.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/rest_framework/admin.html` & `vstutils-5.4.5/vstutils/templates/rest_framework/admin.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/vst_inclusion_tags/bootstrap_form.html` & `vstutils-5.4.5/vstutils/templates/vst_inclusion_tags/bootstrap_form.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templates/widgets/agreement_widget.html` & `vstutils-5.4.5/vstutils/templates/widgets/agreement_widget.html`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templatetags/request_static.py` & `vstutils-5.4.5/vstutils/templatetags/request_static.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templatetags/translation.py` & `vstutils-5.4.5/vstutils/templatetags/translation.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templatetags/vst_gravatar.py` & `vstutils-5.4.5/vstutils/templatetags/vst_gravatar.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templatetags/vst_html_tags.py` & `vstutils-5.4.5/vstutils/templatetags/vst_html_tags.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/templatetags/vstconfigs.py` & `vstutils-5.4.5/vstutils/templatetags/vstconfigs.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/tests.py` & `vstutils-5.4.5/vstutils/tests.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/tools.py` & `vstutils-5.4.5/vstutils/tools.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/translations/cn.py` & `vstutils-5.4.5/vstutils/translations/cn.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/translations/ru.py` & `vstutils-5.4.5/vstutils/translations/ru.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/translations/vi.py` & `vstutils-5.4.5/vstutils/translations/vi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/urls.py` & `vstutils-5.4.5/vstutils/urls.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/utils.py` & `vstutils-5.4.5/vstutils/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 
 from . import exceptions as ex
 from .tools import multikeysort
 
 
 logger: logging.Logger = logging.getLogger('vstutils')
 ON_POSIX = 'posix' in sys.builtin_module_names
+_gzip_object = GZipMiddleware(lambda *args, **kwargs: None)  # type: ignore
 
 
 def deprecated(func: tp.Callable):
     """This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used."""
 
@@ -247,15 +248,15 @@
         from .tasks import SendEmailMessage
         SendEmailMessage.do(email_from=settings.EMAIL_FROM_ADDRESS, **kwargs)
 
 
 def patch_gzip_response(response, request):
     if not response.status_code == 200:
         return  # nocv
-    GZipMiddleware.process_response(None, request, response)
+    GZipMiddleware.process_response(_gzip_object, request, response)
     return response
 
 
 def patch_gzip_response_decorator(func):
     def gzip_response_wrapper(view, request, *args, **kwargs):
         response = func(view, request, *args, **kwargs)
         with raise_context():
```

### Comparing `vstutils-5.4.4/vstutils/web.ini` & `vstutils-5.4.5/vstutils/web.ini`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils/wsgi.py` & `vstutils-5.4.5/vstutils/wsgi.py`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils.egg-info/PKG-INFO` & `vstutils-5.4.5/vstutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vstutils
-Version: 5.4.4
+Version: 5.4.5
 Summary: VST Utils Framework for fast create web-application
 Home-page: https://github.com/vstconsulting/vstutils
 Author: VST Consulting
 Author-email: sergey.k@vstconsulting.net
 License: Apache License 2.0
 Project-URL: Issue Tracker, https://gitlab.com/vstconsulting/vstutils/issues
 Project-URL: Source Code, https://gitlab.com/vstconsulting/vstutils
```

### Comparing `vstutils-5.4.4/vstutils.egg-info/SOURCES.txt` & `vstutils-5.4.5/vstutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vstutils-5.4.4/vstutils.egg-info/requires.txt` & `vstutils-5.4.5/vstutils.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 django~=4.1.7
 configparser~=5.3.0
-configparserc~=1.3.4
-django-cors-headers~=3.13.0
+configparserc~=1.4.0
+django-cors-headers~=4.0.0
 Markdown==3.4.1
 django-environ~=0.10.0
 djangorestframework~=3.14.0
 drf-yasg==1.21.5
 MarkupSafe==2.0.1
-django-filter==22.1
+django-filter==23.2
 django-crispy-forms~=1.14.0
 drf_orjson_renderer~=1.7.1
-ormsgpack==1.2.5
-uvicorn~=0.21.0
+ormsgpack==1.2.6
+uvicorn~=0.22.0
 pyuwsgi==2.0.21
-fastapi~=0.95.0
+fastapi~=0.95.1
 cent~=4.1.0
-PyJWT~=2.6.0
+PyJWT~=2.7.0
 jsmin~=3.0.1
 django-htmlmin~=0.11.0
 pyotp~=2.8.0
 django-storages[libcloud]==1.13.2
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
 sphinxcontrib-httpdomain~=1.8.0
@@ -28,28 +28,28 @@
 sphinx-autodoc-typehints~=1.22.0
 sphinx-rtd-theme~=1.2.0
 
 [all]
 coverage~=7.2.3
 fakeldap==0.6.1
 tblib~=1.7.0
-beautifulsoup4==4.12.0
+beautifulsoup4~=4.12.2
 dj-inmemorystorage~=2.1.0
 httpx~=0.24.0
 celery[redis]==5.2.7
 django-celery-beat~=2.5.0
 python-ldap==3.4.0
 sphinx~=5.3.0
 sphinx-autobuild~=2021.3.14
 sphinxcontrib-httpdomain~=1.8.0
 sphinxcontrib-websupport~=1.2.4
 sphinxcontrib-mermaid~=0.7.1
 sphinx-autodoc-typehints~=1.22.0
 sphinx-rtd-theme~=1.2.0
-redis[hiredis]~=4.5.4
+redis[hiredis]~=4.5.5
 Pillow~=9.4.0
 django-storages[boto3,libcloud]==1.13.2
 
 [boto3]
 django-storages[boto3,libcloud]==1.13.2
 
 [doc]
@@ -68,15 +68,15 @@
 celery[librabbitmq,redis]==5.2.7
 django-celery-beat~=2.5.0
 
 [pil]
 Pillow~=9.4.0
 
 [prod]
-redis[hiredis]~=4.5.4
+redis[hiredis]~=4.5.5
 
 [rpc]
 celery[redis]==5.2.7
 django-celery-beat~=2.5.0
 
 [sqs]
 celery[redis,sqs]==5.2.7
@@ -92,10 +92,10 @@
 types-Markdown~=3.4.2.6
 types-docutils~=0.19.1.7
 
 [test]
 coverage~=7.2.3
 fakeldap==0.6.1
 tblib~=1.7.0
-beautifulsoup4==4.12.0
+beautifulsoup4~=4.12.2
 dj-inmemorystorage~=2.1.0
 httpx~=0.24.0
```

