# Comparing `tmp/kirui-0.5.8.tar.gz` & `tmp/kirui-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirui-0.5.8.tar", last modified: Mon May  1 06:14:59 2023, max compression
+gzip compressed data, was "kirui-0.5.9.tar", last modified: Mon May  1 06:21:10 2023, max compression
```

## Comparing `kirui-0.5.8.tar` & `kirui-0.5.9.tar`

### file list

```diff
@@ -1,608 +1,608 @@
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.272595 kirui-0.5.8/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1068 2020-11-26 19:27:17.000000 kirui-0.5.8/LICENSE
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2021-06-24 09:46:54.000000 kirui-0.5.8/MANIFEST.in
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1246 2023-05-01 06:14:59.272595 kirui-0.5.8/PKG-INFO
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      272 2022-01-14 08:18:51.000000 kirui-0.5.8/README.rst
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.120591 kirui-0.5.8/browser/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      711 2022-02-03 20:41:46.000000 kirui-0.5.8/browser/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1664 2022-02-03 20:41:46.000000 kirui-0.5.8/browser/document.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      244 2022-02-03 20:41:46.000000 kirui-0.5.8/browser/webcomponent.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.120591 kirui-0.5.8/django_kirui/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-03-11 18:57:03.000000 kirui-0.5.8/django_kirui/__init__.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.124591 kirui-0.5.8/django_kirui/components/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       66 2021-05-23 14:50:55.000000 kirui-0.5.8/django_kirui/components/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1017 2022-02-06 21:05:45.000000 kirui-0.5.8/django_kirui/components/apps.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5289 2022-09-04 19:24:13.000000 kirui-0.5.8/django_kirui/components/forms.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      943 2022-11-19 12:19:34.000000 kirui-0.5.8/django_kirui/context_processors.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1517 2023-02-06 19:58:57.000000 kirui-0.5.8/django_kirui/http.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.132592 kirui-0.5.8/django_kirui/static/django_kirui/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   629187 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/brython.min.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  4014149 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/brython_stdlib.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    59913 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/kirui.brython.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269328 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/kirui.css
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   209892 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/kirui.react.css
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   714854 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/static/django_kirui/kirui.react.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.132592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/icons/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.136592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/icons/default/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65906 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/icons/default/icons.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/models/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.136592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/models/dom/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    95810 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/models/dom/model.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.136592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/lists/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    23336 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/lists/plugin.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.136592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/table/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    47025 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/table/plugin.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/content/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.140592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/content/default/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/content/default/content.min.css
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.140592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    23289 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/content.min.css
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    62904 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.min.css
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      508 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.shadowdom.min.css
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/themes/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.140592 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/themes/silver/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   351095 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/themes/silver/theme.min.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   404769 2022-09-08 11:06:57.000000 kirui-0.5.8/django_kirui/static/django_kirui/tinymce/tinymce.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.140592 kirui-0.5.8/django_kirui/templates/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-03-15 12:39:09.000000 kirui-0.5.8/django_kirui/templates/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2919 2023-02-06 20:07:55.000000 kirui-0.5.8/django_kirui/templates/samon.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.140592 kirui-0.5.8/django_kirui/utils/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/utils/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      552 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/utils/paginator.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      189 2022-02-03 20:41:46.000000 kirui-0.5.8/django_kirui/widgets.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.144592 kirui-0.5.8/django_static_bundler/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       96 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.144592 kirui-0.5.8/django_static_bundler/templatetags/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/templatetags/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      348 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/templatetags/bundled_static.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      183 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/urls.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1515 2022-02-03 20:41:46.000000 kirui-0.5.8/django_static_bundler/views.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.144592 kirui-0.5.8/kirui/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       85 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.112591 kirui-0.5.8/kirui/static/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.108591 kirui-0.5.8/kirui/static/bootstrap/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.160592 kirui-0.5.8/kirui/static/bootstrap/font/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92240 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Italic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   101696 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Light.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92488 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    96932 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Regular.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   100820 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92180 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   120468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/bootstrap-icons.woff
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    90528 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/font/bootstrap-icons.woff2
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.164592 kirui-0.5.8/kirui/static/bootstrap/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      288 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/img/today_black_24dp.svg
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.164592 kirui-0.5.8/kirui/static/bootstrap/js/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    79665 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/js/bootstrap.bundle.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.176592 kirui-0.5.8/kirui/static/bootstrap/scss/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2621 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_accordion.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1474 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_alert.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      624 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_badge.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      923 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_breadcrumb.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2969 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_button-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2232 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_buttons.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4753 2022-09-03 05:43:23.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_card.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5623 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_carousel.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1127 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_close.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1196 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_containers.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5589 2022-04-24 21:33:18.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_dropdown.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      256 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_forms.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7906 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_functions.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      286 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      218 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_helpers.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1157 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_images.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4520 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_list-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      872 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_mixins.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5907 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_modal.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1147 2022-11-21 22:15:57.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_modal_side.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2668 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_nav.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6813 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_navbar.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_navbar_custom.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1761 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_offcanvas.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1681 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_pagination.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4402 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_popover.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1169 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_progress.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    12261 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_reboot.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      597 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_root.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1521 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_spinners.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4183 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_tables.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1631 2022-03-17 00:56:49.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_tables_custom.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1178 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_toasts.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2602 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_tooltip.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      320 2022-09-03 05:37:38.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_transitions.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1344 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_type.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    13405 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    63204 2022-09-02 16:40:13.000000 kirui-0.5.8/kirui/static/bootstrap/scss/_variables.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1334 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap-grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      693 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      393 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap-utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1203 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.176592 kirui-0.5.8/kirui/static/bootstrap/scss/forms/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2586 2023-01-04 08:00:48.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_datetime.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1709 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_floating-labels.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3865 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-check.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6729 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-control.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2795 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-range.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2039 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-select.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      219 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-text.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3364 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_input-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_labels.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       63 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_textbox.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      478 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/forms/_validation.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.180593 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       37 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_clearfix.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      326 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_colored-links.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      501 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_position.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_ratio.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_stretched-link.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       73 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_text-truncation.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      136 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/helpers/_visually-hidden.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.180593 kirui-0.5.8/kirui/static/bootstrap/scss/icons/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65703 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.184593 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      268 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_alert.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2031 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4484 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4224 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_buttons.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1473 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_caret.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      147 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      167 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_color-scheme.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      265 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_container.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3745 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_forms.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1965 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_gradients.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3973 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      395 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_image.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      509 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_list-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_lists.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      741 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_pagination.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      495 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      202 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_resize.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      980 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_table-variants.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      661 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_transition.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2286 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1011 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.184593 kirui-0.5.8/kirui/static/bootstrap/scss/utilities/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1737 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/utilities/_api.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.184593 kirui-0.5.8/kirui/static/bootstrap/scss/vendor/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8824 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui/static/bootstrap/scss/vendor/_rfs.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.184593 kirui-0.5.8/kirui/static/codemirror/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8544 2022-06-08 07:59:01.000000 kirui-0.5.8/kirui/static/codemirror/closetag.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  1147989 2022-07-01 13:17:33.000000 kirui-0.5.8/kirui/static/codemirror/codemirror.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.112591 kirui-0.5.8/kirui/static/kirui/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.188593 kirui-0.5.8/kirui/static/kirui/css/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269747 2023-05-01 06:14:58.000000 kirui-0.5.8/kirui/static/kirui/css/kirui.css
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.188593 kirui-0.5.8/kirui/static/kirui/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2238 2021-11-17 08:47:25.000000 kirui-0.5.8/kirui/static/kirui/img/favicon.ico
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.192593 kirui-0.5.8/kirui/static/kirui/js/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.192593 kirui-0.5.8/kirui/static/kirui/js/components/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      261 2023-01-29 18:51:20.000000 kirui-0.5.8/kirui/static/kirui/js/components/app.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2042 2023-01-14 05:21:22.000000 kirui-0.5.8/kirui/static/kirui/js/components/button.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.196593 kirui-0.5.8/kirui/static/kirui/js/components/charts/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   336739 2022-03-18 03:25:27.000000 kirui-0.5.8/kirui/static/kirui/js/components/charts/chart.esm.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.196593 kirui-0.5.8/kirui/static/kirui/js/components/charts/chunks/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    72331 2022-03-18 03:26:55.000000 kirui-0.5.8/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1163 2023-04-09 08:30:21.000000 kirui-0.5.8/kirui/static/kirui/js/components/charts/donut.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2022-09-30 02:44:06.000000 kirui-0.5.8/kirui/static/kirui/js/components/charts/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1360 2022-09-30 03:02:20.000000 kirui-0.5.8/kirui/static/kirui/js/components/charts/line.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.196593 kirui-0.5.8/kirui/static/kirui/js/components/forms/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6802 2023-02-06 20:17:08.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.196593 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      990 2022-02-07 04:59:21.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/checkbox.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5667 2023-01-08 22:54:28.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/date.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      842 2023-01-08 22:27:18.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/file.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      902 2022-02-06 19:56:33.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/input.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3923 2023-01-08 21:42:46.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      703 2022-02-06 19:56:47.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/select.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.200593 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/source_editor/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4966 2022-07-02 07:46:34.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      801 2022-07-02 07:51:41.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1756 2023-01-08 20:41:59.000000 kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/text.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.200593 kirui-0.5.8/kirui/static/kirui/js/components/kanban/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1261 2022-11-19 13:23:13.000000 kirui-0.5.8/kirui/static/kirui/js/components/kanban/board.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      541 2022-11-19 12:23:41.000000 kirui-0.5.8/kirui/static/kirui/js/components/kanban/card.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       76 2022-11-19 12:12:20.000000 kirui-0.5.8/kirui/static/kirui/js/components/kanban/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.200593 kirui-0.5.8/kirui/static/kirui/js/components/layout/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1523 2022-09-03 06:01:55.000000 kirui-0.5.8/kirui/static/kirui/js/components/layout/card.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       57 2022-09-02 13:19:07.000000 kirui-0.5.8/kirui/static/kirui/js/components/layout/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7921 2023-03-15 03:21:36.000000 kirui-0.5.8/kirui/static/kirui/js/components/layout/sidebar.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3415 2023-01-08 22:31:15.000000 kirui-0.5.8/kirui/static/kirui/js/components/modal.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.200593 kirui-0.5.8/kirui/static/kirui/js/components/tables/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      755 2022-03-18 01:00:06.000000 kirui-0.5.8/kirui/static/kirui/js/components/tables/filtered_table.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       89 2022-02-06 14:00:00.000000 kirui-0.5.8/kirui/static/kirui/js/components/tables/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3596 2022-03-18 01:24:06.000000 kirui-0.5.8/kirui/static/kirui/js/components/tables/table.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.204593 kirui-0.5.8/kirui/static/kirui/js/core/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      528 2023-01-08 18:14:24.000000 kirui-0.5.8/kirui/static/kirui/js/core/component.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1744 2022-07-22 08:30:59.000000 kirui-0.5.8/kirui/static/kirui/js/core/css-tag.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1410 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui/static/kirui/js/core/directive-helpers.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      481 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui/static/kirui/js/core/directive.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.204593 kirui-0.5.8/kirui/static/kirui/js/core/directives/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1128 2023-01-08 18:13:26.000000 kirui-0.5.8/kirui/static/kirui/js/core/directives/class-map.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      467 2022-12-11 11:05:37.000000 kirui-0.5.8/kirui/static/kirui/js/core/directives/keyed.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2735 2022-07-22 08:29:09.000000 kirui-0.5.8/kirui/static/kirui/js/core/lit-element.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1393 2022-07-22 08:25:51.000000 kirui-0.5.8/kirui/static/kirui/js/core/lit-element3_2_2.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8077 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui/static/kirui/js/core/lit-html.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7635 2022-07-22 08:23:55.000000 kirui-0.5.8/kirui/static/kirui/js/core/reactive-element.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2023-01-29 18:51:20.000000 kirui-0.5.8/kirui/static/kirui/js/entrypoint.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-04 07:04:25.000000 kirui-0.5.8/kirui/static/kirui/js/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.204593 kirui-0.5.8/kirui/static/kirui/js/pwa/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.212593 kirui-0.5.8/kirui/static/kirui/js/pwa/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6123 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    16805 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5812 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/apple-touch-icon.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      721 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon-16x16.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1227 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon-32x32.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    15086 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon.ico
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    33680 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/icon.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4778 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/img/mstile-150x150.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      452 2023-01-29 22:41:26.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/manifest.json
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      586 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/offline.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2649 2023-01-29 20:09:46.000000 kirui-0.5.8/kirui/static/kirui/js/pwa/service-worker.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.212593 kirui-0.5.8/kirui/static/kirui/js/utils/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1094 2022-03-16 07:48:55.000000 kirui-0.5.8/kirui/static/kirui/js/utils/http.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.144592 kirui-0.5.8/kirui.egg-info/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1246 2023-05-01 06:14:59.000000 kirui-0.5.8/kirui.egg-info/PKG-INFO
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    24005 2023-05-01 06:14:59.000000 kirui-0.5.8/kirui.egg-info/SOURCES.txt
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        1 2023-05-01 06:14:59.000000 kirui-0.5.8/kirui.egg-info/dependency_links.txt
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2023-05-01 06:14:59.000000 kirui-0.5.8/kirui.egg-info/top_level.txt
--rwxrwxr-x   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_dev
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.212593 kirui-0.5.8/kirui_devserver/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        7 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/__init__.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.224593 kirui-0.5.8/kirui_devserver/backend/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2020-12-07 07:48:35.000000 kirui-0.5.8/kirui_devserver/backend/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      106 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/backend/apps.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1778 2023-01-08 22:27:29.000000 kirui-0.5.8/kirui_devserver/backend/forms.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.224593 kirui-0.5.8/kirui_devserver/backend/management/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/backend/management/__init__.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.224593 kirui-0.5.8/kirui_devserver/backend/management/commands/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/backend/management/commands/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      895 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/backend/management/commands/proba.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.224593 kirui-0.5.8/kirui_devserver/backend/migrations/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      485 2021-08-12 11:42:33.000000 kirui-0.5.8/kirui_devserver/backend/migrations/0001_initial.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      517 2021-08-12 11:46:18.000000 kirui-0.5.8/kirui_devserver/backend/migrations/0002_activity.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      765 2021-08-14 13:16:38.000000 kirui-0.5.8/kirui_devserver/backend/migrations/0003_auto_20210814_1316.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-08-12 11:42:33.000000 kirui-0.5.8/kirui_devserver/backend/migrations/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      437 2021-08-14 13:16:35.000000 kirui-0.5.8/kirui_devserver/backend/models.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.112591 kirui-0.5.8/kirui_devserver/backend/templates/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.228594 kirui-0.5.8/kirui_devserver/backend/templates/backend/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1111 2022-09-03 05:28:07.000000 kirui-0.5.8/kirui_devserver/backend/templates/backend/card.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      796 2022-09-30 02:51:40.000000 kirui-0.5.8/kirui_devserver/backend/templates/backend/charts.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      565 2022-03-16 07:42:03.000000 kirui-0.5.8/kirui_devserver/backend/templates/backend/filtered_table.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1561 2022-03-18 01:23:33.000000 kirui-0.5.8/kirui_devserver/backend/templates/backend/filtered_table_data.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      588 2022-11-19 12:06:38.000000 kirui-0.5.8/kirui_devserver/backend/templates/backend/kanban.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      516 2022-11-19 11:48:49.000000 kirui-0.5.8/kirui_devserver/backend/urls.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4511 2023-02-06 20:09:41.000000 kirui-0.5.8/kirui_devserver/backend/views.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      254 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/context_processors.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.228594 kirui-0.5.8/kirui_devserver/django_static_bundler/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       96 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.228594 kirui-0.5.8/kirui_devserver/django_static_bundler/templatetags/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/templatetags/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      348 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/templatetags/bundled_static.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      183 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/urls.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1515 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/django_static_bundler/views.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.232594 kirui-0.5.8/kirui_devserver/kirui/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       85 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.112591 kirui-0.5.8/kirui_devserver/kirui/static/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.112591 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.232594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92240 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Italic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   101696 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Light.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92488 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    96932 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Regular.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   100820 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92180 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   120468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    90528 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff2
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.232594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      288 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/img/today_black_24dp.svg
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.232594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/js/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    79665 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/js/bootstrap.bundle.min.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.236594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2621 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_accordion.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1474 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_alert.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      624 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_badge.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      923 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_breadcrumb.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2969 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_button-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2232 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_buttons.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4753 2022-09-03 05:43:23.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_card.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5623 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_carousel.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1127 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_close.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1196 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_containers.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5589 2022-04-24 21:33:18.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_dropdown.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      256 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_forms.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7906 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_functions.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      286 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      218 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_helpers.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1157 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_images.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4520 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_list-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      872 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_mixins.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5907 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_modal.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1147 2022-11-21 22:15:57.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_modal_side.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2668 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_nav.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6813 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_navbar.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_navbar_custom.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1761 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_offcanvas.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1681 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_pagination.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4402 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_popover.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1169 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_progress.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    12261 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_reboot.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      597 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_root.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1521 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_spinners.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4183 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tables.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1631 2022-03-17 00:56:49.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tables_custom.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1178 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_toasts.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2602 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tooltip.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      320 2022-09-03 05:37:38.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_transitions.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1344 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_type.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    13405 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    63204 2022-09-02 16:40:13.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_variables.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1334 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      693 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-reboot.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      393 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1203 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.240594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2586 2023-01-04 08:00:48.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_datetime.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1709 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_floating-labels.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3865 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-check.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6729 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-control.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2795 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-range.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2039 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-select.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      219 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-text.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3364 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_input-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_labels.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2468 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       63 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_textbox.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      478 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_validation.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.240594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       37 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_clearfix.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      326 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_colored-links.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      501 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_position.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_ratio.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_stretched-link.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       73 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_text-truncation.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      136 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/helpers/_visually-hidden.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.240594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/icons/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65703 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      268 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_alert.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2031 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_border-radius.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_box-shadow.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4484 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_breakpoints.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4224 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_buttons.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1473 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_caret.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      147 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_clearfix.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      167 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_color-scheme.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      265 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_container.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_deprecate.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3745 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_forms.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1965 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_gradients.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3973 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_grid.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      395 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_image.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      509 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_list-group.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_lists.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      741 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_pagination.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      495 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_reset-text.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      202 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_resize.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      980 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_table-variants.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_text-truncate.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      661 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_transition.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2286 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_utilities.scss
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1011 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/utilities/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1737 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/utilities/_api.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/vendor/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8824 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/vendor/_rfs.scss
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/codemirror/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8544 2022-06-08 07:59:01.000000 kirui-0.5.8/kirui_devserver/kirui/static/codemirror/closetag.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  1147989 2022-07-01 13:17:33.000000 kirui-0.5.8/kirui_devserver/kirui/static/codemirror/codemirror.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.116591 kirui-0.5.8/kirui_devserver/kirui/static/kirui/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/css/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269747 2023-05-01 06:14:58.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/css/kirui.css
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2238 2021-11-17 08:47:25.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/img/favicon.ico
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      261 2023-01-29 18:51:20.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/app.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2042 2023-01-14 05:21:22.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/button.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.244594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   336739 2022-03-18 03:25:27.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/chart.esm.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    72331 2022-03-18 03:26:55.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1163 2023-04-09 08:30:21.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/donut.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2022-09-30 02:44:06.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1360 2022-09-30 03:02:20.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/line.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6802 2023-02-06 20:17:08.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      990 2022-02-07 04:59:21.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/checkbox.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5667 2023-01-08 22:54:28.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/date.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      842 2023-01-08 22:27:18.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/file.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      902 2022-02-06 19:56:33.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/input.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3923 2023-01-08 21:42:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      703 2022-02-06 19:56:47.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/select.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4966 2022-07-02 07:46:34.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      801 2022-07-02 07:51:41.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1756 2023-01-08 20:41:59.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/text.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1261 2022-11-19 13:23:13.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/board.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      541 2022-11-19 12:23:41.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/card.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       76 2022-11-19 12:12:20.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1523 2022-09-03 06:01:55.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/card.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       57 2022-09-02 13:19:07.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7921 2023-03-15 03:21:36.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/sidebar.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3415 2023-01-08 22:31:15.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/modal.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      755 2022-03-18 01:00:06.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/filtered_table.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       89 2022-02-06 14:00:00.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/index.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3596 2022-03-18 01:24:06.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/table.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      528 2023-01-08 18:14:24.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/component.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1744 2022-07-22 08:30:59.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/css-tag.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1410 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directive-helpers.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      481 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directive.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directives/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1128 2023-01-08 18:13:26.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directives/class-map.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      467 2022-12-11 11:05:37.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directives/keyed.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2735 2022-07-22 08:29:09.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-element.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1393 2022-07-22 08:25:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-element3_2_2.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8077 1985-10-26 08:15:00.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-html.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7635 2022-07-22 08:23:55.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/reactive-element.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2023-01-29 18:51:20.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/entrypoint.js
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-04 07:04:25.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/index.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.248594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.252594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6123 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    16805 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5812 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/apple-touch-icon.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      721 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-16x16.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1227 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-32x32.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    15086 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon.ico
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    33680 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/icon.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4778 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/mstile-150x150.png
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      452 2023-01-29 22:41:26.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/manifest.json
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      586 2023-01-29 19:10:51.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/offline.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2649 2023-01-29 20:09:46.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/service-worker.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.252594 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/utils/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1094 2022-03-16 07:48:55.000000 kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/utils/http.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.252594 kirui-0.5.8/kirui_devserver/livesync/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      792 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/.gitignore
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-06 08:05:43.000000 kirui-0.5.8/kirui_devserver/livesync/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       92 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.252594 kirui-0.5.8/kirui_devserver/livesync/asyncserver/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       62 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/asyncserver/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      730 2021-01-08 09:41:21.000000 kirui-0.5.8/kirui_devserver/livesync/asyncserver/dispatcher.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1558 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/asyncserver/handler.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      548 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/asyncserver/hub.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1386 2021-01-08 09:52:06.000000 kirui-0.5.8/kirui_devserver/livesync/asyncserver/server.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.252594 kirui-0.5.8/kirui_devserver/livesync/core/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/core/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      235 2021-01-08 09:41:07.000000 kirui-0.5.8/kirui_devserver/livesync/core/event.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1767 2021-01-08 09:45:16.000000 kirui-0.5.8/kirui_devserver/livesync/core/handler.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      935 2021-01-07 17:49:54.000000 kirui-0.5.8/kirui_devserver/livesync/core/middleware.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       94 2021-12-26 10:19:21.000000 kirui-0.5.8/kirui_devserver/livesync/core/signals.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/fswatcher/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       72 2021-01-05 08:45:24.000000 kirui-0.5.8/kirui_devserver/livesync/fswatcher/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1080 2021-01-06 12:22:12.000000 kirui-0.5.8/kirui_devserver/livesync/fswatcher/handlers.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      301 2021-02-26 18:11:03.000000 kirui-0.5.8/kirui_devserver/livesync/fswatcher/utils.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      546 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/fswatcher/watcher.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/management/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/management/__init__.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/management/commands/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/management/commands/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-12-28 19:00:12.000000 kirui-0.5.8/kirui_devserver/livesync/management/commands/liveserver.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-01-08 09:13:49.000000 kirui-0.5.8/kirui_devserver/livesync/management/commands/runserver.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/static/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      263 2021-01-04 13:04:14.000000 kirui-0.5.8/kirui_devserver/livesync/static/livesync.brython.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6555 2021-01-08 08:43:50.000000 kirui-0.5.8/kirui_devserver/livesync/static/livesync.js
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.116591 kirui-0.5.8/kirui_devserver/livesync/templates/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/templates/livesync/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      267 2021-01-07 11:27:59.000000 kirui-0.5.8/kirui_devserver/livesync/templates/livesync/livesync_scripts.html
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.256594 kirui-0.5.8/kirui_devserver/livesync/tests/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/tests/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2887 2021-01-05 08:14:32.000000 kirui-0.5.8/kirui_devserver/livesync/tests/test_asyncserver.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1775 2021-01-07 17:41:40.000000 kirui-0.5.8/kirui_devserver/livesync/tests/test_command.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4436 2021-01-08 09:46:50.000000 kirui-0.5.8/kirui_devserver/livesync/tests/test_handlers.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2133 2021-01-07 18:06:56.000000 kirui-0.5.8/kirui_devserver/livesync/tests/test_middleware.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1394 2021-01-06 08:46:26.000000 kirui-0.5.8/kirui_devserver/livesync/tests/test_watchers.py
--rwxrwxr-x   0 lovasb    (1000) lovasb    (1000)      662 2020-11-27 08:20:04.000000 kirui-0.5.8/kirui_devserver/manage.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.260594 kirui-0.5.8/kirui_devserver/server/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2020-11-27 08:20:04.000000 kirui-0.5.8/kirui_devserver/server/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      389 2020-11-27 08:20:04.000000 kirui-0.5.8/kirui_devserver/server/asgi.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3671 2022-07-22 08:27:19.000000 kirui-0.5.8/kirui_devserver/server/settings.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      374 2023-01-29 19:49:18.000000 kirui-0.5.8/kirui_devserver/server/urls.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      405 2020-12-26 15:08:46.000000 kirui-0.5.8/kirui_devserver/server/wsgi.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.116591 kirui-0.5.8/kirui_devserver/templates/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.260594 kirui-0.5.8/kirui_devserver/templates/html/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1200 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/html/base.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      255 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/html/index.html
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.260594 kirui-0.5.8/kirui_devserver/templates/html/livesync/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2021-03-06 03:49:34.000000 kirui-0.5.8/kirui_devserver/templates/html/livesync/livesync_scripts.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      207 2020-12-05 08:39:54.000000 kirui-0.5.8/kirui_devserver/templates/html/tests.html
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.116591 kirui-0.5.8/kirui_devserver/templates/samon/
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.260594 kirui-0.5.8/kirui_devserver/templates/samon/xml/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      808 2023-02-06 20:06:14.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/form.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      308 2022-03-17 06:32:41.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/form_data.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1533 2023-01-29 23:00:41.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/header.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      808 2023-01-29 22:45:56.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/index.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1554 2022-11-19 11:50:59.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/menu.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      513 2023-04-28 11:20:29.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/modal.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      824 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/sidebar_header.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      543 2022-04-24 13:34:28.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/table.html
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      965 2022-09-24 01:32:03.000000 kirui-0.5.8/kirui_devserver/templates/samon/xml/table_data.html
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.264594 kirui-0.5.8/kirui_devserver/templates/xml_react/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1326 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/base.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/form.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      415 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/header.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      555 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/index.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      574 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/modal.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      932 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/panel.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1675 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/panel_data.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      913 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/table.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      547 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/table_data.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1221 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/topbar.xml
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      289 2022-02-03 20:41:46.000000 kirui-0.5.8/kirui_devserver/templates/xml_react/valami.xml
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.264594 kirui-0.5.8/livesync/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-06 08:05:43.000000 kirui-0.5.8/livesync/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       92 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/apps.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/asyncserver/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       62 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/asyncserver/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      730 2021-01-08 09:41:21.000000 kirui-0.5.8/livesync/asyncserver/dispatcher.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1558 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/asyncserver/handler.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      548 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/asyncserver/hub.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1386 2021-01-08 09:52:06.000000 kirui-0.5.8/livesync/asyncserver/server.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/core/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/core/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      235 2021-01-08 09:41:07.000000 kirui-0.5.8/livesync/core/event.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1767 2021-01-08 09:45:16.000000 kirui-0.5.8/livesync/core/handler.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      935 2021-01-07 17:49:54.000000 kirui-0.5.8/livesync/core/middleware.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       94 2021-12-26 10:19:21.000000 kirui-0.5.8/livesync/core/signals.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/fswatcher/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       72 2021-01-05 08:45:24.000000 kirui-0.5.8/livesync/fswatcher/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1080 2021-01-06 12:22:12.000000 kirui-0.5.8/livesync/fswatcher/handlers.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      301 2021-02-26 18:11:03.000000 kirui-0.5.8/livesync/fswatcher/utils.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      546 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/fswatcher/watcher.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/management/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/management/__init__.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/management/commands/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/management/commands/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-12-28 19:00:12.000000 kirui-0.5.8/livesync/management/commands/liveserver.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-01-08 09:13:49.000000 kirui-0.5.8/livesync/management/commands/runserver.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.268595 kirui-0.5.8/livesync/tests/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/tests/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2887 2021-01-05 08:14:32.000000 kirui-0.5.8/livesync/tests/test_asyncserver.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1775 2021-01-07 17:41:40.000000 kirui-0.5.8/livesync/tests/test_command.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4436 2021-01-08 09:46:50.000000 kirui-0.5.8/livesync/tests/test_handlers.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2133 2021-01-07 18:06:56.000000 kirui-0.5.8/livesync/tests/test_middleware.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1394 2021-01-06 08:46:26.000000 kirui-0.5.8/livesync/tests/test_watchers.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.272595 kirui-0.5.8/samon/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       31 2020-07-06 15:29:55.000000 kirui-0.5.8/samon/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      349 2022-02-03 20:41:46.000000 kirui-0.5.8/samon/constants.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2528 2022-02-03 20:41:46.000000 kirui-0.5.8/samon/elements.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      673 2022-01-06 13:58:53.000000 kirui-0.5.8/samon/environment.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      342 2020-07-06 14:07:51.000000 kirui-0.5.8/samon/exceptions.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1476 2022-09-13 02:33:40.000000 kirui-0.5.8/samon/expressions.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      891 2022-03-16 07:34:02.000000 kirui-0.5.8/samon/loaders.py
-drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:14:59.272595 kirui-0.5.8/samon/parser/
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       67 2022-02-03 20:41:46.000000 kirui-0.5.8/samon/parser/__init__.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1486 2020-09-19 11:26:27.000000 kirui-0.5.8/samon/parser/json.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    17786 2022-02-03 20:41:46.000000 kirui-0.5.8/samon/parser/temp.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5677 2023-02-06 19:42:55.000000 kirui-0.5.8/samon/parser/xml.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1807 2020-09-20 18:45:49.000000 kirui-0.5.8/samon/registry.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8974 2023-04-30 07:50:30.000000 kirui-0.5.8/samon/render.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3066 2023-02-06 19:35:53.000000 kirui-0.5.8/samon/template.py
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       38 2023-05-01 06:14:59.272595 kirui-0.5.8/setup.cfg
--rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1486 2023-05-01 06:14:43.000000 kirui-0.5.8/setup.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.075987 kirui-0.5.9/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1068 2020-11-26 19:27:17.000000 kirui-0.5.9/LICENSE
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2021-06-24 09:46:54.000000 kirui-0.5.9/MANIFEST.in
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1246 2023-05-01 06:21:10.075987 kirui-0.5.9/PKG-INFO
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      272 2022-01-14 08:18:51.000000 kirui-0.5.9/README.rst
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.979984 kirui-0.5.9/browser/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      711 2022-02-03 20:41:46.000000 kirui-0.5.9/browser/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1664 2022-02-03 20:41:46.000000 kirui-0.5.9/browser/document.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      244 2022-02-03 20:41:46.000000 kirui-0.5.9/browser/webcomponent.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.979984 kirui-0.5.9/django_kirui/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-03-11 18:57:03.000000 kirui-0.5.9/django_kirui/__init__.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.979984 kirui-0.5.9/django_kirui/components/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       66 2021-05-23 14:50:55.000000 kirui-0.5.9/django_kirui/components/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1017 2022-02-06 21:05:45.000000 kirui-0.5.9/django_kirui/components/apps.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5289 2022-09-04 19:24:13.000000 kirui-0.5.9/django_kirui/components/forms.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      943 2022-11-19 12:19:34.000000 kirui-0.5.9/django_kirui/context_processors.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1513 2023-05-01 06:20:55.000000 kirui-0.5.9/django_kirui/http.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.987984 kirui-0.5.9/django_kirui/static/django_kirui/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   629187 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/brython.min.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  4014149 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/brython_stdlib.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    59913 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/kirui.brython.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269328 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/kirui.css
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   209892 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/kirui.react.css
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   714854 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/static/django_kirui/kirui.react.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.987984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/icons/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.991984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/icons/default/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65906 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/icons/default/icons.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/models/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.991984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/models/dom/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    95810 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/models/dom/model.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.991984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/lists/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    23336 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/lists/plugin.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.991984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/table/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    47025 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/table/plugin.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/content/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.991984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/content/default/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/content/default/content.min.css
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    23289 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/content.min.css
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    62904 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.min.css
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      508 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.shadowdom.min.css
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/themes/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/themes/silver/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   351095 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/themes/silver/theme.min.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   404769 2022-09-08 11:06:57.000000 kirui-0.5.9/django_kirui/static/django_kirui/tinymce/tinymce.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_kirui/templates/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-03-15 12:39:09.000000 kirui-0.5.9/django_kirui/templates/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2919 2023-02-06 20:07:55.000000 kirui-0.5.9/django_kirui/templates/samon.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_kirui/utils/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/utils/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      552 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/utils/paginator.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      189 2022-02-03 20:41:46.000000 kirui-0.5.9/django_kirui/widgets.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_static_bundler/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       96 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/django_static_bundler/templatetags/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/templatetags/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      348 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/templatetags/bundled_static.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      183 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/urls.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1515 2022-02-03 20:41:46.000000 kirui-0.5.9/django_static_bundler/views.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.995984 kirui-0.5.9/kirui/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       85 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/kirui/static/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/kirui/static/bootstrap/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.003985 kirui-0.5.9/kirui/static/bootstrap/font/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92240 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Italic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   101696 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Light.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92488 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    96932 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Regular.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   100820 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92180 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   120468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/bootstrap-icons.woff
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    90528 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/font/bootstrap-icons.woff2
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.003985 kirui-0.5.9/kirui/static/bootstrap/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      288 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/img/today_black_24dp.svg
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.003985 kirui-0.5.9/kirui/static/bootstrap/js/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    79665 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.007985 kirui-0.5.9/kirui/static/bootstrap/scss/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2621 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_accordion.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1474 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_alert.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      624 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_badge.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      923 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_breadcrumb.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2969 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_button-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2232 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_buttons.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4753 2022-09-03 05:43:23.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_card.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5623 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_carousel.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1127 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_close.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1196 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_containers.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5589 2022-04-24 21:33:18.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_dropdown.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      256 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_forms.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7906 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_functions.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      286 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      218 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_helpers.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1157 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_images.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4520 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_list-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      872 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_mixins.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5907 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_modal.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1147 2022-11-21 22:15:57.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_modal_side.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2668 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_nav.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6813 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_navbar.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_navbar_custom.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1761 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_offcanvas.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1681 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_pagination.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4402 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_popover.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1169 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_progress.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    12261 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_reboot.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      597 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_root.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1521 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_spinners.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4183 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_tables.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1631 2022-03-17 00:56:49.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_tables_custom.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1178 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_toasts.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2602 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_tooltip.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      320 2022-09-03 05:37:38.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_transitions.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1344 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_type.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    13405 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    63204 2022-09-02 16:40:13.000000 kirui-0.5.9/kirui/static/bootstrap/scss/_variables.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1334 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      693 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      393 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap-utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1203 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.011985 kirui-0.5.9/kirui/static/bootstrap/scss/forms/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2586 2023-01-04 08:00:48.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_datetime.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1709 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_floating-labels.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3865 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-check.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6729 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-control.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2795 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-range.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2039 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-select.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      219 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-text.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3364 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_input-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_labels.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       63 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_textbox.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      478 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/forms/_validation.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.011985 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       37 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_clearfix.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      326 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_colored-links.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      501 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_position.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_ratio.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_stretched-link.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       73 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_text-truncation.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      136 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/helpers/_visually-hidden.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.011985 kirui-0.5.9/kirui/static/bootstrap/scss/icons/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65703 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.011985 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      268 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_alert.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2031 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4484 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4224 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1473 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_caret.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      147 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      167 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_color-scheme.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      265 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_container.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3745 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_forms.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1965 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3973 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      395 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_image.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      509 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_lists.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      741 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      495 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      202 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_resize.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      980 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_table-variants.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      661 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_transition.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2286 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1011 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/bootstrap/scss/utilities/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1737 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/utilities/_api.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/bootstrap/scss/vendor/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8824 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui/static/bootstrap/scss/vendor/_rfs.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/codemirror/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8544 2022-06-08 07:59:01.000000 kirui-0.5.9/kirui/static/codemirror/closetag.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  1147989 2022-07-01 13:17:33.000000 kirui-0.5.9/kirui/static/codemirror/codemirror.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.971984 kirui-0.5.9/kirui/static/kirui/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/kirui/css/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269747 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui/static/kirui/css/kirui.css
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/kirui/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2238 2021-11-17 08:47:25.000000 kirui-0.5.9/kirui/static/kirui/img/favicon.ico
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.015985 kirui-0.5.9/kirui/static/kirui/js/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.019985 kirui-0.5.9/kirui/static/kirui/js/components/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      261 2023-01-29 18:51:20.000000 kirui-0.5.9/kirui/static/kirui/js/components/app.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2042 2023-01-14 05:21:22.000000 kirui-0.5.9/kirui/static/kirui/js/components/button.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.019985 kirui-0.5.9/kirui/static/kirui/js/components/charts/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   336739 2022-03-18 03:25:27.000000 kirui-0.5.9/kirui/static/kirui/js/components/charts/chart.esm.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.019985 kirui-0.5.9/kirui/static/kirui/js/components/charts/chunks/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    72331 2022-03-18 03:26:55.000000 kirui-0.5.9/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1163 2023-04-09 08:30:21.000000 kirui-0.5.9/kirui/static/kirui/js/components/charts/donut.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2022-09-30 02:44:06.000000 kirui-0.5.9/kirui/static/kirui/js/components/charts/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1360 2022-09-30 03:02:20.000000 kirui-0.5.9/kirui/static/kirui/js/components/charts/line.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.019985 kirui-0.5.9/kirui/static/kirui/js/components/forms/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6802 2023-02-06 20:17:08.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.023985 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      990 2022-02-07 04:59:21.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/checkbox.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5667 2023-01-08 22:54:28.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/date.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      842 2023-01-08 22:27:18.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/file.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      902 2022-02-06 19:56:33.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/input.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3923 2023-01-08 21:42:46.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      703 2022-02-06 19:56:47.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/select.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.023985 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/source_editor/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4966 2022-07-02 07:46:34.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      801 2022-07-02 07:51:41.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1756 2023-01-08 20:41:59.000000 kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/text.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.023985 kirui-0.5.9/kirui/static/kirui/js/components/kanban/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1261 2022-11-19 13:23:13.000000 kirui-0.5.9/kirui/static/kirui/js/components/kanban/board.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      541 2022-11-19 12:23:41.000000 kirui-0.5.9/kirui/static/kirui/js/components/kanban/card.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       76 2022-11-19 12:12:20.000000 kirui-0.5.9/kirui/static/kirui/js/components/kanban/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.023985 kirui-0.5.9/kirui/static/kirui/js/components/layout/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1523 2022-09-03 06:01:55.000000 kirui-0.5.9/kirui/static/kirui/js/components/layout/card.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       57 2022-09-02 13:19:07.000000 kirui-0.5.9/kirui/static/kirui/js/components/layout/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7921 2023-03-15 03:21:36.000000 kirui-0.5.9/kirui/static/kirui/js/components/layout/sidebar.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3415 2023-01-08 22:31:15.000000 kirui-0.5.9/kirui/static/kirui/js/components/modal.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.027985 kirui-0.5.9/kirui/static/kirui/js/components/tables/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      755 2022-03-18 01:00:06.000000 kirui-0.5.9/kirui/static/kirui/js/components/tables/filtered_table.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       89 2022-02-06 14:00:00.000000 kirui-0.5.9/kirui/static/kirui/js/components/tables/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3596 2022-03-18 01:24:06.000000 kirui-0.5.9/kirui/static/kirui/js/components/tables/table.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.027985 kirui-0.5.9/kirui/static/kirui/js/core/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      528 2023-01-08 18:14:24.000000 kirui-0.5.9/kirui/static/kirui/js/core/component.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1744 2022-07-22 08:30:59.000000 kirui-0.5.9/kirui/static/kirui/js/core/css-tag.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1410 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui/static/kirui/js/core/directive-helpers.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      481 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui/static/kirui/js/core/directive.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.027985 kirui-0.5.9/kirui/static/kirui/js/core/directives/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1128 2023-01-08 18:13:26.000000 kirui-0.5.9/kirui/static/kirui/js/core/directives/class-map.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      467 2022-12-11 11:05:37.000000 kirui-0.5.9/kirui/static/kirui/js/core/directives/keyed.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2735 2022-07-22 08:29:09.000000 kirui-0.5.9/kirui/static/kirui/js/core/lit-element.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1393 2022-07-22 08:25:51.000000 kirui-0.5.9/kirui/static/kirui/js/core/lit-element3_2_2.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8077 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui/static/kirui/js/core/lit-html.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7635 2022-07-22 08:23:55.000000 kirui-0.5.9/kirui/static/kirui/js/core/reactive-element.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2023-01-29 18:51:20.000000 kirui-0.5.9/kirui/static/kirui/js/entrypoint.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-04 07:04:25.000000 kirui-0.5.9/kirui/static/kirui/js/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.027985 kirui-0.5.9/kirui/static/kirui/js/pwa/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.031986 kirui-0.5.9/kirui/static/kirui/js/pwa/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6123 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    16805 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5812 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/apple-touch-icon.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      721 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon-16x16.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1227 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon-32x32.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    15086 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon.ico
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    33680 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/icon.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4778 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/img/mstile-150x150.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      452 2023-01-29 22:41:26.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/manifest.json
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      586 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/offline.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2649 2023-01-29 20:09:46.000000 kirui-0.5.9/kirui/static/kirui/js/pwa/service-worker.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.031986 kirui-0.5.9/kirui/static/kirui/js/utils/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1094 2022-03-16 07:48:55.000000 kirui-0.5.9/kirui/static/kirui/js/utils/http.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.999985 kirui-0.5.9/kirui.egg-info/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1246 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui.egg-info/PKG-INFO
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    24005 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui.egg-info/SOURCES.txt
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        1 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui.egg-info/dependency_links.txt
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui.egg-info/top_level.txt
+-rwxrwxr-x   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_dev
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.031986 kirui-0.5.9/kirui_devserver/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        7 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/__init__.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.031986 kirui-0.5.9/kirui_devserver/backend/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2020-12-07 07:48:35.000000 kirui-0.5.9/kirui_devserver/backend/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      106 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/backend/apps.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1778 2023-01-08 22:27:29.000000 kirui-0.5.9/kirui_devserver/backend/forms.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/backend/management/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/backend/management/__init__.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/backend/management/commands/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/backend/management/commands/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      895 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/backend/management/commands/proba.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/backend/migrations/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      485 2021-08-12 11:42:33.000000 kirui-0.5.9/kirui_devserver/backend/migrations/0001_initial.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      517 2021-08-12 11:46:18.000000 kirui-0.5.9/kirui_devserver/backend/migrations/0002_activity.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      765 2021-08-14 13:16:38.000000 kirui-0.5.9/kirui_devserver/backend/migrations/0003_auto_20210814_1316.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-08-12 11:42:33.000000 kirui-0.5.9/kirui_devserver/backend/migrations/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      437 2021-08-14 13:16:35.000000 kirui-0.5.9/kirui_devserver/backend/models.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/backend/templates/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/backend/templates/backend/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1111 2022-09-03 05:28:07.000000 kirui-0.5.9/kirui_devserver/backend/templates/backend/card.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      796 2022-09-30 02:51:40.000000 kirui-0.5.9/kirui_devserver/backend/templates/backend/charts.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      565 2022-03-16 07:42:03.000000 kirui-0.5.9/kirui_devserver/backend/templates/backend/filtered_table.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1561 2022-03-18 01:23:33.000000 kirui-0.5.9/kirui_devserver/backend/templates/backend/filtered_table_data.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      588 2022-11-19 12:06:38.000000 kirui-0.5.9/kirui_devserver/backend/templates/backend/kanban.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      516 2022-11-19 11:48:49.000000 kirui-0.5.9/kirui_devserver/backend/urls.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4511 2023-02-06 20:09:41.000000 kirui-0.5.9/kirui_devserver/backend/views.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      254 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/context_processors.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/django_static_bundler/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       96 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/django_static_bundler/templatetags/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/templatetags/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      348 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/templatetags/bundled_static.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      183 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/urls.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1515 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/django_static_bundler/views.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.035986 kirui-0.5.9/kirui_devserver/kirui/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       85 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/kirui/static/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.039986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92240 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Italic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   101696 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Light.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92488 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    96932 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Regular.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   100820 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    92180 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   120468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    90528 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff2
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.039986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      288 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/img/today_black_24dp.svg
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.039986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/js/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    79665 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/js/bootstrap.bundle.min.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.047986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2621 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_accordion.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1474 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_alert.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      624 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_badge.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      923 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_breadcrumb.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2969 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_button-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2232 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_buttons.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4753 2022-09-03 05:43:23.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_card.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5623 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_carousel.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1127 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_close.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1196 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_containers.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5589 2022-04-24 21:33:18.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_dropdown.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      256 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_forms.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7906 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_functions.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      286 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      218 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_helpers.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1157 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_images.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4520 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_list-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      872 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_mixins.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5907 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_modal.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1147 2022-11-21 22:15:57.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_modal_side.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2668 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_nav.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6813 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_navbar.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_navbar_custom.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1761 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_offcanvas.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1681 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_pagination.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4402 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_popover.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1169 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_progress.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    12261 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_reboot.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      597 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_root.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1521 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_spinners.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4183 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tables.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1631 2022-03-17 00:56:49.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tables_custom.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1178 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_toasts.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2602 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tooltip.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      320 2022-09-03 05:37:38.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_transitions.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1344 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_type.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    13405 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    63204 2022-09-02 16:40:13.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_variables.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1334 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      693 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-reboot.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      393 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1203 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.047986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2586 2023-01-04 08:00:48.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_datetime.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1709 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_floating-labels.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3865 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-check.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6729 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-control.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2795 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-range.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2039 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-select.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      219 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-text.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3364 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_input-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1216 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_labels.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2468 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       63 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_textbox.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      478 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_validation.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.047986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       37 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_clearfix.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      326 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_colored-links.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      501 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_position.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_ratio.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_stretched-link.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       73 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_text-truncation.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      136 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/helpers/_visually-hidden.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.047986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/icons/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    65703 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      268 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_alert.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2031 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_border-radius.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      398 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_box-shadow.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4484 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_breakpoints.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4224 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_buttons.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1473 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_caret.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      147 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_clearfix.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      167 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_color-scheme.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      265 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_container.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_deprecate.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3745 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_forms.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1965 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_gradients.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3973 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_grid.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      395 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_image.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      509 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_list-group.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_lists.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      741 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_pagination.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      495 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_reset-text.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      202 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_resize.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      980 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_table-variants.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      168 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_text-truncate.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      661 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_transition.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2286 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_utilities.scss
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1011 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/utilities/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1737 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/utilities/_api.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/vendor/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8824 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/vendor/_rfs.scss
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/codemirror/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8544 2022-06-08 07:59:01.000000 kirui-0.5.9/kirui_devserver/kirui/static/codemirror/closetag.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)  1147989 2022-07-01 13:17:33.000000 kirui-0.5.9/kirui_devserver/kirui/static/codemirror/codemirror.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/kirui/static/kirui/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/kirui/css/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   269747 2023-05-01 06:21:09.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/css/kirui.css
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/kirui/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2238 2021-11-17 08:47:25.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/img/favicon.ico
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.051986 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      261 2023-01-29 18:51:20.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/app.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2042 2023-01-14 05:21:22.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/button.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)   336739 2022-03-18 03:25:27.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/chart.esm.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    72331 2022-03-18 03:26:55.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1163 2023-04-09 08:30:21.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/donut.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       80 2022-09-30 02:44:06.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1360 2022-09-30 03:02:20.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/line.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6802 2023-02-06 20:17:08.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      990 2022-02-07 04:59:21.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/checkbox.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5667 2023-01-08 22:54:28.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/date.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      842 2023-01-08 22:27:18.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/file.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      902 2022-02-06 19:56:33.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/input.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3923 2023-01-08 21:42:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      703 2022-02-06 19:56:47.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/select.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4966 2022-07-02 07:46:34.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      801 2022-07-02 07:51:41.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1756 2023-01-08 20:41:59.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/text.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1261 2022-11-19 13:23:13.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/board.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      541 2022-11-19 12:23:41.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/card.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       76 2022-11-19 12:12:20.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1523 2022-09-03 06:01:55.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/card.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       57 2022-09-02 13:19:07.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7921 2023-03-15 03:21:36.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/sidebar.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3415 2023-01-08 22:31:15.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/modal.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      755 2022-03-18 01:00:06.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/filtered_table.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       89 2022-02-06 14:00:00.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/index.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3596 2022-03-18 01:24:06.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/table.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      528 2023-01-08 18:14:24.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/component.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1744 2022-07-22 08:30:59.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/css-tag.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1410 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directive-helpers.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      481 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directive.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directives/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1128 2023-01-08 18:13:26.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directives/class-map.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      467 2022-12-11 11:05:37.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directives/keyed.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2735 2022-07-22 08:29:09.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-element.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1393 2022-07-22 08:25:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-element3_2_2.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8077 1985-10-26 08:15:00.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-html.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     7635 2022-07-22 08:23:55.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/reactive-element.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      613 2023-01-29 18:51:20.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/entrypoint.js
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2022-02-04 07:04:25.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/index.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.055987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6123 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    16805 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5812 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/apple-touch-icon.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      721 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-16x16.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1227 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-32x32.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    15086 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon.ico
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    33680 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/icon.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4778 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/mstile-150x150.png
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      452 2023-01-29 22:41:26.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/manifest.json
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      586 2023-01-29 19:10:51.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/offline.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2649 2023-01-29 20:09:46.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/service-worker.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/utils/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1094 2022-03-16 07:48:55.000000 kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/utils/http.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      792 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/.gitignore
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-06 08:05:43.000000 kirui-0.5.9/kirui_devserver/livesync/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       92 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/asyncserver/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       62 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/asyncserver/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      730 2021-01-08 09:41:21.000000 kirui-0.5.9/kirui_devserver/livesync/asyncserver/dispatcher.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1558 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/asyncserver/handler.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      548 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/asyncserver/hub.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1386 2021-01-08 09:52:06.000000 kirui-0.5.9/kirui_devserver/livesync/asyncserver/server.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/core/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/core/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      235 2021-01-08 09:41:07.000000 kirui-0.5.9/kirui_devserver/livesync/core/event.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1767 2021-01-08 09:45:16.000000 kirui-0.5.9/kirui_devserver/livesync/core/handler.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      935 2021-01-07 17:49:54.000000 kirui-0.5.9/kirui_devserver/livesync/core/middleware.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       94 2021-12-26 10:19:21.000000 kirui-0.5.9/kirui_devserver/livesync/core/signals.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/fswatcher/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       72 2021-01-05 08:45:24.000000 kirui-0.5.9/kirui_devserver/livesync/fswatcher/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1080 2021-01-06 12:22:12.000000 kirui-0.5.9/kirui_devserver/livesync/fswatcher/handlers.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      301 2021-02-26 18:11:03.000000 kirui-0.5.9/kirui_devserver/livesync/fswatcher/utils.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      546 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/fswatcher/watcher.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/management/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/management/__init__.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.059987 kirui-0.5.9/kirui_devserver/livesync/management/commands/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/management/commands/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-12-28 19:00:12.000000 kirui-0.5.9/kirui_devserver/livesync/management/commands/liveserver.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-01-08 09:13:49.000000 kirui-0.5.9/kirui_devserver/livesync/management/commands/runserver.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/livesync/static/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      263 2021-01-04 13:04:14.000000 kirui-0.5.9/kirui_devserver/livesync/static/livesync.brython.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     6555 2021-01-08 08:43:50.000000 kirui-0.5.9/kirui_devserver/livesync/static/livesync.js
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/livesync/templates/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/livesync/templates/livesync/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      267 2021-01-07 11:27:59.000000 kirui-0.5.9/kirui_devserver/livesync/templates/livesync/livesync_scripts.html
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/livesync/tests/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/tests/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2887 2021-01-05 08:14:32.000000 kirui-0.5.9/kirui_devserver/livesync/tests/test_asyncserver.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1775 2021-01-07 17:41:40.000000 kirui-0.5.9/kirui_devserver/livesync/tests/test_command.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4436 2021-01-08 09:46:50.000000 kirui-0.5.9/kirui_devserver/livesync/tests/test_handlers.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2133 2021-01-07 18:06:56.000000 kirui-0.5.9/kirui_devserver/livesync/tests/test_middleware.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1394 2021-01-06 08:46:26.000000 kirui-0.5.9/kirui_devserver/livesync/tests/test_watchers.py
+-rwxrwxr-x   0 lovasb    (1000) lovasb    (1000)      662 2020-11-27 08:20:04.000000 kirui-0.5.9/kirui_devserver/manage.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/server/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2020-11-27 08:20:04.000000 kirui-0.5.9/kirui_devserver/server/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      389 2020-11-27 08:20:04.000000 kirui-0.5.9/kirui_devserver/server/asgi.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3671 2022-07-22 08:27:19.000000 kirui-0.5.9/kirui_devserver/server/settings.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      374 2023-01-29 19:49:18.000000 kirui-0.5.9/kirui_devserver/server/urls.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      405 2020-12-26 15:08:46.000000 kirui-0.5.9/kirui_devserver/server/wsgi.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/templates/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/templates/html/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1200 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/html/base.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      255 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/html/index.html
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.063987 kirui-0.5.9/kirui_devserver/templates/html/livesync/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      223 2021-03-06 03:49:34.000000 kirui-0.5.9/kirui_devserver/templates/html/livesync/livesync_scripts.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      207 2020-12-05 08:39:54.000000 kirui-0.5.9/kirui_devserver/templates/html/tests.html
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:09.975984 kirui-0.5.9/kirui_devserver/templates/samon/
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.067987 kirui-0.5.9/kirui_devserver/templates/samon/xml/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      808 2023-02-06 20:06:14.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/form.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      308 2022-03-17 06:32:41.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/form_data.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1533 2023-01-29 23:00:41.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/header.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      808 2023-01-29 22:45:56.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/index.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1554 2022-11-19 11:50:59.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/menu.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      513 2023-04-28 11:20:29.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/modal.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      824 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/sidebar_header.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      543 2022-04-24 13:34:28.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/table.html
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      965 2022-09-24 01:32:03.000000 kirui-0.5.9/kirui_devserver/templates/samon/xml/table_data.html
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/kirui_devserver/templates/xml_react/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1326 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/base.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      417 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/form.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      415 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/header.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      555 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/index.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      574 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/modal.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      932 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/panel.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1675 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/panel_data.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      913 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/table.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      547 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/table_data.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1221 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/topbar.xml
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      289 2022-02-03 20:41:46.000000 kirui-0.5.9/kirui_devserver/templates/xml_react/valami.xml
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-06 08:05:43.000000 kirui-0.5.9/livesync/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       92 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/apps.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/asyncserver/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       62 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/asyncserver/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      730 2021-01-08 09:41:21.000000 kirui-0.5.9/livesync/asyncserver/dispatcher.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1558 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/asyncserver/handler.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      548 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/asyncserver/hub.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1386 2021-01-08 09:52:06.000000 kirui-0.5.9/livesync/asyncserver/server.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/core/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/core/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      235 2021-01-08 09:41:07.000000 kirui-0.5.9/livesync/core/event.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1767 2021-01-08 09:45:16.000000 kirui-0.5.9/livesync/core/handler.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      935 2021-01-07 17:49:54.000000 kirui-0.5.9/livesync/core/middleware.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       94 2021-12-26 10:19:21.000000 kirui-0.5.9/livesync/core/signals.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/fswatcher/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       72 2021-01-05 08:45:24.000000 kirui-0.5.9/livesync/fswatcher/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1080 2021-01-06 12:22:12.000000 kirui-0.5.9/livesync/fswatcher/handlers.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      301 2021-02-26 18:11:03.000000 kirui-0.5.9/livesync/fswatcher/utils.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      546 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/fswatcher/watcher.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/management/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/management/__init__.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/management/commands/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/management/commands/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-12-28 19:00:12.000000 kirui-0.5.9/livesync/management/commands/liveserver.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4167 2021-01-08 09:13:49.000000 kirui-0.5.9/livesync/management/commands/runserver.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.071987 kirui-0.5.9/livesync/tests/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)        0 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/tests/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2887 2021-01-05 08:14:32.000000 kirui-0.5.9/livesync/tests/test_asyncserver.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1775 2021-01-07 17:41:40.000000 kirui-0.5.9/livesync/tests/test_command.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     4436 2021-01-08 09:46:50.000000 kirui-0.5.9/livesync/tests/test_handlers.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2133 2021-01-07 18:06:56.000000 kirui-0.5.9/livesync/tests/test_middleware.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1394 2021-01-06 08:46:26.000000 kirui-0.5.9/livesync/tests/test_watchers.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.075987 kirui-0.5.9/samon/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       31 2020-07-06 15:29:55.000000 kirui-0.5.9/samon/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      349 2022-02-03 20:41:46.000000 kirui-0.5.9/samon/constants.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     2528 2022-02-03 20:41:46.000000 kirui-0.5.9/samon/elements.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      673 2022-01-06 13:58:53.000000 kirui-0.5.9/samon/environment.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      342 2020-07-06 14:07:51.000000 kirui-0.5.9/samon/exceptions.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1476 2022-09-13 02:33:40.000000 kirui-0.5.9/samon/expressions.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)      891 2022-03-16 07:34:02.000000 kirui-0.5.9/samon/loaders.py
+drwxrwxr-x   0 lovasb    (1000) lovasb    (1000)        0 2023-05-01 06:21:10.075987 kirui-0.5.9/samon/parser/
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       67 2022-02-03 20:41:46.000000 kirui-0.5.9/samon/parser/__init__.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1486 2020-09-19 11:26:27.000000 kirui-0.5.9/samon/parser/json.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)    17786 2022-02-03 20:41:46.000000 kirui-0.5.9/samon/parser/temp.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     5677 2023-02-06 19:42:55.000000 kirui-0.5.9/samon/parser/xml.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1807 2020-09-20 18:45:49.000000 kirui-0.5.9/samon/registry.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     8974 2023-04-30 07:50:30.000000 kirui-0.5.9/samon/render.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     3066 2023-02-06 19:35:53.000000 kirui-0.5.9/samon/template.py
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)       38 2023-05-01 06:21:10.075987 kirui-0.5.9/setup.cfg
+-rw-rw-r--   0 lovasb    (1000) lovasb    (1000)     1486 2023-05-01 06:21:04.000000 kirui-0.5.9/setup.py
```

### Comparing `kirui-0.5.8/LICENSE` & `kirui-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/PKG-INFO` & `kirui-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirui
-Version: 0.5.8
+Version: 0.5.9
 Summary: UI framework with React / Preact and Django SSR backend
 Home-page: https://kirui.lovasb.com/
 Author: Bence Lovas
 Author-email: me@lovasb.com
 License: UNKNOWN
 Project-URL: Documentation, https://kirui.lovasb.com/
 Project-URL: Source, https://gitlab.com/lovasb/kirui
```

### Comparing `kirui-0.5.8/browser/__init__.py` & `kirui-0.5.9/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/browser/document.py` & `kirui-0.5.9/browser/document.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/components/apps.py` & `kirui-0.5.9/django_kirui/components/apps.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/components/forms.py` & `kirui-0.5.9/django_kirui/components/forms.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/context_processors.py` & `kirui-0.5.9/django_kirui/context_processors.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/http.py` & `kirui-0.5.9/django_kirui/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,21 +18,21 @@
     def to_200(self):
         data = get_template(self.template_name, using='samon').render(context=self.context, request=self.request, frame=self.frame)
         resp = HttpResponse(data)
         return resp
 
     def to_201(self):
         data = get_template(self.template_name, using='samon').render(context=self.context, request=self.request, frame=self.frame, to='js_template')
-        resp = HttpResponse('m.html`' + data + '`')
+        resp = HttpResponse('html`' + data + '`')
         resp.status_code = 201
         return resp
 
     def to_403(self):
         data = get_template(self.template_name, using='samon').render(context=self.context, request=self.request, frame=self.frame, to='js_template')
-        resp = HttpResponse('m.html`' + data + '`')
+        resp = HttpResponse('html`' + data + '`')
         resp.status_code = 403
         return resp
 
     def to_340(self, redirect_to):
         resp = HttpResponseRedirect(redirect_to=redirect_to)
         resp.status_code = 340
         return resp
```

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/brython.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/brython.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/brython_stdlib.js` & `kirui-0.5.9/django_kirui/static/django_kirui/brython_stdlib.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/kirui.brython.js` & `kirui-0.5.9/django_kirui/static/django_kirui/kirui.brython.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/kirui.css` & `kirui-0.5.9/django_kirui/static/django_kirui/kirui.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/kirui.react.css` & `kirui-0.5.9/django_kirui/static/django_kirui/kirui.react.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/kirui.react.js` & `kirui-0.5.9/django_kirui/static/django_kirui/kirui.react.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/icons/default/icons.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/icons/default/icons.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/models/dom/model.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/models/dom/model.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/lists/plugin.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/lists/plugin.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/plugins/table/plugin.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/plugins/table/plugin.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/content/default/content.min.css` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/content/default/content.min.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/content.min.css` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/content.min.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.min.css` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/skins/ui/oxide/skin.min.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/themes/silver/theme.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/themes/silver/theme.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/static/django_kirui/tinymce/tinymce.min.js` & `kirui-0.5.9/django_kirui/static/django_kirui/tinymce/tinymce.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/templates/samon.py` & `kirui-0.5.9/django_kirui/templates/samon.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_kirui/utils/paginator.py` & `kirui-0.5.9/django_kirui/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/django_static_bundler/views.py` & `kirui-0.5.9/django_static_bundler/views.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Italic.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Light.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-Regular.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf` & `kirui-0.5.9/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/bootstrap-icons.woff` & `kirui-0.5.9/kirui/static/bootstrap/font/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/font/bootstrap-icons.woff2` & `kirui-0.5.9/kirui/static/bootstrap/font/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/js/bootstrap.bundle.min.js` & `kirui-0.5.9/kirui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_accordion.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_alert.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_badge.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_breadcrumb.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_button-group.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_buttons.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_card.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_carousel.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_close.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_containers.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_dropdown.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_functions.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_images.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_list-group.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_mixins.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_modal.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_modal_side.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_modal_side.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_nav.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_navbar.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_navbar_custom.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_navbar_custom.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_offcanvas.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_pagination.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_popover.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_progress.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_reboot.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_root.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_spinners.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_tables.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_tables_custom.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_tables_custom.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_toasts.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_tooltip.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_type.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_utilities.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/_variables.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap-grid.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap-reboot.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap-reboot.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/bootstrap.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_datetime.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_datetime.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_floating-labels.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-check.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-control.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-range.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_form-select.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_input-group.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_labels.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_border-radius.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_breakpoints.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_buttons.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_caret.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_deprecate.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_forms.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_gradients.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_grid.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_pagination.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_pagination.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_table-variants.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_transition.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_utilities.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/utilities/_api.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/bootstrap/scss/vendor/_rfs.scss` & `kirui-0.5.9/kirui/static/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/codemirror/closetag.js` & `kirui-0.5.9/kirui/static/codemirror/closetag.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/codemirror/codemirror.js` & `kirui-0.5.9/kirui/static/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/css/kirui.css` & `kirui-0.5.9/kirui/static/kirui/css/kirui.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/img/favicon.ico` & `kirui-0.5.9/kirui/static/kirui/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/button.js` & `kirui-0.5.9/kirui/static/kirui/js/components/button.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/charts/chart.esm.js` & `kirui-0.5.9/kirui/static/kirui/js/components/charts/chart.esm.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js` & `kirui-0.5.9/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/charts/donut.js` & `kirui-0.5.9/kirui/static/kirui/js/components/charts/donut.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/charts/line.js` & `kirui-0.5.9/kirui/static/kirui/js/components/charts/line.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/index.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/index.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/checkbox.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/checkbox.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/date.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/date.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/file.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/file.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/input.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/input.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/select.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/select.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/forms/widgets/text.js` & `kirui-0.5.9/kirui/static/kirui/js/components/forms/widgets/text.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/kanban/board.js` & `kirui-0.5.9/kirui/static/kirui/js/components/kanban/board.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/kanban/card.js` & `kirui-0.5.9/kirui/static/kirui/js/components/kanban/card.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/layout/card.js` & `kirui-0.5.9/kirui/static/kirui/js/components/layout/card.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/layout/sidebar.js` & `kirui-0.5.9/kirui/static/kirui/js/components/layout/sidebar.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/modal.js` & `kirui-0.5.9/kirui/static/kirui/js/components/modal.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/tables/filtered_table.js` & `kirui-0.5.9/kirui/static/kirui/js/components/tables/filtered_table.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/components/tables/table.js` & `kirui-0.5.9/kirui/static/kirui/js/components/tables/table.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/component.js` & `kirui-0.5.9/kirui/static/kirui/js/core/component.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/css-tag.js` & `kirui-0.5.9/kirui/static/kirui/js/core/css-tag.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/directive-helpers.js` & `kirui-0.5.9/kirui/static/kirui/js/core/directive-helpers.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/directives/class-map.js` & `kirui-0.5.9/kirui/static/kirui/js/core/directives/class-map.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/lit-element.js` & `kirui-0.5.9/kirui/static/kirui/js/core/lit-element.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/lit-element3_2_2.js` & `kirui-0.5.9/kirui/static/kirui/js/core/lit-element3_2_2.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/lit-html.js` & `kirui-0.5.9/kirui/static/kirui/js/core/lit-html.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/core/reactive-element.js` & `kirui-0.5.9/kirui/static/kirui/js/core/reactive-element.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/entrypoint.js` & `kirui-0.5.9/kirui/static/kirui/js/entrypoint.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/apple-touch-icon.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon-16x16.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon-32x32.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/favicon.ico` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/icon.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/icon.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/img/mstile-150x150.png` & `kirui-0.5.9/kirui/static/kirui/js/pwa/img/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/offline.html` & `kirui-0.5.9/kirui/static/kirui/js/pwa/offline.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/pwa/service-worker.js` & `kirui-0.5.9/kirui/static/kirui/js/pwa/service-worker.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui/static/kirui/js/utils/http.js` & `kirui-0.5.9/kirui/static/kirui/js/utils/http.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui.egg-info/PKG-INFO` & `kirui-0.5.9/kirui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kirui
-Version: 0.5.8
+Version: 0.5.9
 Summary: UI framework with React / Preact and Django SSR backend
 Home-page: https://kirui.lovasb.com/
 Author: Bence Lovas
 Author-email: me@lovasb.com
 License: UNKNOWN
 Project-URL: Documentation, https://kirui.lovasb.com/
 Project-URL: Source, https://gitlab.com/lovasb/kirui
```

### Comparing `kirui-0.5.8/kirui.egg-info/SOURCES.txt` & `kirui-0.5.9/kirui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/forms.py` & `kirui-0.5.9/kirui_devserver/backend/forms.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/management/commands/proba.py` & `kirui-0.5.9/kirui_devserver/backend/management/commands/proba.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/migrations/0002_activity.py` & `kirui-0.5.9/kirui_devserver/backend/migrations/0002_activity.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/migrations/0003_auto_20210814_1316.py` & `kirui-0.5.9/kirui_devserver/backend/migrations/0003_auto_20210814_1316.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/templates/backend/card.html` & `kirui-0.5.9/kirui_devserver/backend/templates/backend/card.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/templates/backend/charts.html` & `kirui-0.5.9/kirui_devserver/backend/templates/backend/charts.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/templates/backend/filtered_table.html` & `kirui-0.5.9/kirui_devserver/backend/templates/backend/filtered_table.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/templates/backend/filtered_table_data.html` & `kirui-0.5.9/kirui_devserver/backend/templates/backend/filtered_table_data.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/templates/backend/kanban.html` & `kirui-0.5.9/kirui_devserver/backend/templates/backend/kanban.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/urls.py` & `kirui-0.5.9/kirui_devserver/backend/urls.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/backend/views.py` & `kirui-0.5.9/kirui_devserver/backend/views.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/django_static_bundler/views.py` & `kirui-0.5.9/kirui_devserver/django_static_bundler/views.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Italic.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Italic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Light.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Light.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Regular.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-Regular.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/OpenSans-SemiBoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff2` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/font/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/js/bootstrap.bundle.min.js` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_accordion.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_accordion.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_alert.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_alert.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_badge.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_badge.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_breadcrumb.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_breadcrumb.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_button-group.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_button-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_buttons.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_buttons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_card.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_card.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_carousel.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_carousel.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_close.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_close.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_containers.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_containers.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_dropdown.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_functions.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_functions.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_images.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_images.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_list-group.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_list-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_mixins.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_mixins.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_modal.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_modal.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_modal_side.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_modal_side.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_nav.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_navbar.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_navbar.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_navbar_custom.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_navbar_custom.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_offcanvas.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_offcanvas.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_pagination.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_pagination.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_popover.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_popover.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_progress.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_progress.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_reboot.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_reboot.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_root.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_root.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_spinners.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_spinners.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tables.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tables.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tables_custom.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tables_custom.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_toasts.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_toasts.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_tooltip.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_tooltip.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_type.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_type.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_utilities.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_utilities.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/_variables.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/_variables.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-grid.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-grid.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-reboot.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap-reboot.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/bootstrap.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/bootstrap.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_datetime.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_datetime.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_floating-labels.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_floating-labels.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-check.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-check.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-control.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-control.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-range.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-range.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-select.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_form-select.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_input-group.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_input-group.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_labels.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_labels.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/forms/_multi_select_dropdown.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_border-radius.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_border-radius.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_breakpoints.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_breakpoints.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_buttons.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_buttons.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_caret.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_caret.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_deprecate.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_deprecate.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_forms.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_forms.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_gradients.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_gradients.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_grid.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_grid.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_pagination.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_pagination.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_table-variants.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_table-variants.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_transition.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_transition.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_utilities.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_utilities.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/mixins/_visually-hidden.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/utilities/_api.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/utilities/_api.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/bootstrap/scss/vendor/_rfs.scss` & `kirui-0.5.9/kirui_devserver/kirui/static/bootstrap/scss/vendor/_rfs.scss`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/codemirror/closetag.js` & `kirui-0.5.9/kirui_devserver/kirui/static/codemirror/closetag.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/codemirror/codemirror.js` & `kirui-0.5.9/kirui_devserver/kirui/static/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/css/kirui.css` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/css/kirui.css`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/img/favicon.ico` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/button.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/button.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/chart.esm.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/chart.esm.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/donut.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/donut.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/charts/line.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/charts/line.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/index.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/index.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/checkbox.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/checkbox.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/date.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/date.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/file.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/file.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/input.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/input.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/multi_select_checkbox.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/select.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/select.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/codemirror.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/source_editor/index.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/text.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/forms/widgets/text.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/board.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/board.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/kanban/card.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/kanban/card.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/card.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/card.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/layout/sidebar.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/layout/sidebar.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/modal.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/modal.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/filtered_table.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/filtered_table.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/components/tables/table.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/components/tables/table.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/component.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/component.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/css-tag.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/css-tag.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directive-helpers.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directive-helpers.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/directives/class-map.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/directives/class-map.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-element.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-element.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-element3_2_2.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-element3_2_2.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/lit-html.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/lit-html.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/core/reactive-element.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/core/reactive-element.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/entrypoint.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/entrypoint.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/apple-touch-icon.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-16x16.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-32x32.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon.ico` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/icon.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/icon.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/img/mstile-150x150.png` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/img/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/offline.html` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/offline.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/pwa/service-worker.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/pwa/service-worker.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/kirui/static/kirui/js/utils/http.js` & `kirui-0.5.9/kirui_devserver/kirui/static/kirui/js/utils/http.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/.gitignore` & `kirui-0.5.9/kirui_devserver/livesync/.gitignore`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/asyncserver/dispatcher.py` & `kirui-0.5.9/kirui_devserver/livesync/asyncserver/dispatcher.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/asyncserver/handler.py` & `kirui-0.5.9/kirui_devserver/livesync/asyncserver/handler.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/asyncserver/hub.py` & `kirui-0.5.9/kirui_devserver/livesync/asyncserver/hub.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/asyncserver/server.py` & `kirui-0.5.9/kirui_devserver/livesync/asyncserver/server.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/core/handler.py` & `kirui-0.5.9/kirui_devserver/livesync/core/handler.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/core/middleware.py` & `kirui-0.5.9/kirui_devserver/livesync/core/middleware.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/fswatcher/handlers.py` & `kirui-0.5.9/kirui_devserver/livesync/fswatcher/handlers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/fswatcher/watcher.py` & `kirui-0.5.9/kirui_devserver/livesync/fswatcher/watcher.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/management/commands/liveserver.py` & `kirui-0.5.9/kirui_devserver/livesync/management/commands/liveserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/management/commands/runserver.py` & `kirui-0.5.9/kirui_devserver/livesync/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/static/livesync.js` & `kirui-0.5.9/kirui_devserver/livesync/static/livesync.js`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/tests/test_asyncserver.py` & `kirui-0.5.9/kirui_devserver/livesync/tests/test_asyncserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/tests/test_command.py` & `kirui-0.5.9/kirui_devserver/livesync/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/tests/test_handlers.py` & `kirui-0.5.9/kirui_devserver/livesync/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/tests/test_middleware.py` & `kirui-0.5.9/kirui_devserver/livesync/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/livesync/tests/test_watchers.py` & `kirui-0.5.9/kirui_devserver/livesync/tests/test_watchers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/manage.py` & `kirui-0.5.9/kirui_devserver/manage.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/server/settings.py` & `kirui-0.5.9/kirui_devserver/server/settings.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/html/base.html` & `kirui-0.5.9/kirui_devserver/templates/html/base.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/form.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/form.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/header.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/header.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/index.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/index.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/menu.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/menu.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/modal.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/modal.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/sidebar_header.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/sidebar_header.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/table.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/table.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/samon/xml/table_data.html` & `kirui-0.5.9/kirui_devserver/templates/samon/xml/table_data.html`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/base.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/base.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/index.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/index.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/modal.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/modal.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/panel.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/panel.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/panel_data.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/panel_data.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/table.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/table.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/table_data.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/table_data.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/kirui_devserver/templates/xml_react/topbar.xml` & `kirui-0.5.9/kirui_devserver/templates/xml_react/topbar.xml`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/asyncserver/dispatcher.py` & `kirui-0.5.9/livesync/asyncserver/dispatcher.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/asyncserver/handler.py` & `kirui-0.5.9/livesync/asyncserver/handler.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/asyncserver/hub.py` & `kirui-0.5.9/livesync/asyncserver/hub.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/asyncserver/server.py` & `kirui-0.5.9/livesync/asyncserver/server.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/core/handler.py` & `kirui-0.5.9/livesync/core/handler.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/core/middleware.py` & `kirui-0.5.9/livesync/core/middleware.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/fswatcher/handlers.py` & `kirui-0.5.9/livesync/fswatcher/handlers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/fswatcher/watcher.py` & `kirui-0.5.9/livesync/fswatcher/watcher.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/management/commands/liveserver.py` & `kirui-0.5.9/livesync/management/commands/liveserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/management/commands/runserver.py` & `kirui-0.5.9/livesync/management/commands/runserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/tests/test_asyncserver.py` & `kirui-0.5.9/livesync/tests/test_asyncserver.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/tests/test_command.py` & `kirui-0.5.9/livesync/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/tests/test_handlers.py` & `kirui-0.5.9/livesync/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/tests/test_middleware.py` & `kirui-0.5.9/livesync/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/livesync/tests/test_watchers.py` & `kirui-0.5.9/livesync/tests/test_watchers.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/elements.py` & `kirui-0.5.9/samon/elements.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/environment.py` & `kirui-0.5.9/samon/environment.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/expressions.py` & `kirui-0.5.9/samon/expressions.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/loaders.py` & `kirui-0.5.9/samon/loaders.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/parser/json.py` & `kirui-0.5.9/samon/parser/json.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/parser/temp.py` & `kirui-0.5.9/samon/parser/temp.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/parser/xml.py` & `kirui-0.5.9/samon/parser/xml.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/registry.py` & `kirui-0.5.9/samon/registry.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/render.py` & `kirui-0.5.9/samon/render.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/samon/template.py` & `kirui-0.5.9/samon/template.py`

 * *Files identical despite different names*

### Comparing `kirui-0.5.8/setup.py` & `kirui-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from setuptools import find_packages, setup
 
 try:
     with open('VERSION', 'r') as f:
         version = f.read().strip()
 except FileNotFoundError:
-    version = '0.5.8'
+    version = '0.5.9'
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='kirui',
```

