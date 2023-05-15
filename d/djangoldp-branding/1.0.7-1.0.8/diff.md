# Comparing `tmp/djangoldp_branding-1.0.7.tar.gz` & `tmp/djangoldp_branding-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_branding-1.0.7.tar", last modified: Fri Jul 15 11:29:50 2022, max compression
+gzip compressed data, was "dist/djangoldp_branding-1.0.8.tar", last modified: Wed Jul 20 09:38:46 2022, max compression
```

## Comparing `djangoldp_branding-1.0.7.tar` & `djangoldp_branding-1.0.8.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/
--rw-rw-rw-   0 root         (0) root         (0)     2358 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/README.md
--rw-rw-rw-   0 root         (0) root         (0)       92 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/setup.py
--rw-rw-rw-   0 root         (0) root         (0)       69 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)      569 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/
--rw-r--r--   0 root         (0) root         (0)      313 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2964 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      313 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/
--rw-rw-rw-   0 root         (0) root         (0)     2954 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/views.py
--rw-rw-rw-   0 root         (0) root         (0)      682 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/processor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/accessrequests/
--rw-rw-rw-   0 root         (0) root         (0)     2071 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/accessrequests/access_requested.html
--rw-rw-rw-   0 root         (0) root         (0)     2067 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/accessrequests/access_resolved.html
--rw-rw-rw-   0 root         (0) root         (0)     6040 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/base_email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/
--rw-rw-rw-   0 root         (0) root         (0)      353 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_done.html
--rw-rw-rw-   0 root         (0) root         (0)     2088 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_change_form.html
--rw-rw-rw-   0 root         (0) root         (0)     2094 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_email.html
--rw-rw-rw-   0 root         (0) root         (0)     1970 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_confirm.html
--rw-rw-rw-   0 root         (0) root         (0)      525 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     1288 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_form.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      538 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      497 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/lost_user.html
--rw-rw-rw-   0 root         (0) root         (0)      263 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/activate.html
--rw-rw-rw-   0 root         (0) root         (0)      459 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_email.txt
--rw-rw-rw-   0 root         (0) root         (0)      489 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/logged_out.html
--rw-rw-rw-   0 root         (0) root         (0)      545 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      482 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/logout.html
--rw-rw-rw-   0 root         (0) root         (0)     4159 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/login.html
--rw-rw-rw-   0 root         (0) root         (0)      500 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_change_done.html
--rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2103 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/joboffer/
--rw-rw-rw-   0 root         (0) root         (0)     2557 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/joboffer/email.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/admin/
--rw-rw-rw-   0 root         (0) root         (0)     4686 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/admin/base.html
--rw-rw-rw-   0 root         (0) root         (0)     2458 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/admin/login.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/oidc_provider/
--rw-rw-rw-   0 root         (0) root         (0)     2506 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/oidc_provider/authorize.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/password/
--rw-rw-rw-   0 root         (0) root         (0)     1791 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/password/email.html
--rw-rw-rw-   0 root         (0) root         (0)     2243 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/base.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/
--rw-rw-rw-   0 root         (0) root         (0)      551 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/activation_complete.html
--rw-rw-rw-   0 root         (0) root         (0)     2052 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/registration_form.html
--rw-rw-rw-   0 root         (0) root         (0)      275 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/registration_closed.html
--rw-rw-rw-   0 root         (0) root         (0)      266 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/registration_complete.html
--rw-rw-rw-   0 root         (0) root         (0)      380 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/activation_failed.html
--rw-rw-rw-   0 root         (0) root         (0)      567 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/djangoldp_urls.py
--rw-rw-rw-   0 root         (0) root         (0)       50 2022-07-15 11:29:48.000000 djangoldp_branding-1.0.7/djangoldp_branding/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/es/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15362 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/es/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     7249 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/es/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    15233 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     7176 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/en/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/en/LC_MESSAGES/
--rw-rw-rw-   0 root         (0) root         (0)    14897 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/en/LC_MESSAGES/django.po
--rw-rw-rw-   0 root         (0) root         (0)     6840 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/locale/en/LC_MESSAGES/django.mo
--rw-rw-rw-   0 root         (0) root         (0)      110 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/css/
--rw-rw-rw-   0 root         (0) root         (0)    19356 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/css/admin.css
--rw-rw-rw-   0 root         (0) root         (0)      432 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/css/main.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/images/
--rw-rw-rw-   0 root         (0) root         (0)      832 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/static/images/favicon.webp
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-15 11:29:50.000000 djangoldp_branding-1.0.7/djangoldp_branding/templatetags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templatetags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1177 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/templatetags/orbit.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2022-07-15 11:29:32.000000 djangoldp_branding-1.0.7/djangoldp_branding/djangoldp_settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/
+-rw-rw-rw-   0 root         (0) root         (0)     2358 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       92 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)       69 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)      569 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      313 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     2964 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      313 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/
+-rw-rw-rw-   0 root         (0) root         (0)     2954 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      735 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/processor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_requested.html
+-rw-rw-rw-   0 root         (0) root         (0)     2067 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_resolved.html
+-rw-rw-rw-   0 root         (0) root         (0)     6040 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/base_email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/
+-rw-rw-rw-   0 root         (0) root         (0)      353 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_done.html
+-rw-rw-rw-   0 root         (0) root         (0)     2088 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_form.html
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.html
+-rw-rw-rw-   0 root         (0) root         (0)     1970 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_confirm.html
+-rw-rw-rw-   0 root         (0) root         (0)      525 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_form.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      538 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      497 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/lost_user.html
+-rw-rw-rw-   0 root         (0) root         (0)      263 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activate.html
+-rw-rw-rw-   0 root         (0) root         (0)      459 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.txt
+-rw-rw-rw-   0 root         (0) root         (0)      489 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/logged_out.html
+-rw-rw-rw-   0 root         (0) root         (0)      545 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      482 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/logout.html
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/login.html
+-rw-rw-rw-   0 root         (0) root         (0)      500 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_done.html
+-rw-rw-rw-   0 root         (0) root         (0)      297 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2103 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/
+-rw-rw-rw-   0 root         (0) root         (0)     2557 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/email.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/
+-rw-rw-rw-   0 root         (0) root         (0)     4686 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/base.html
+-rw-rw-rw-   0 root         (0) root         (0)     2458 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/login.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/authorize.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/password/
+-rw-rw-rw-   0 root         (0) root         (0)     1791 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/password/email.html
+-rw-rw-rw-   0 root         (0) root         (0)     2279 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/base.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/
+-rw-rw-rw-   0 root         (0) root         (0)      551 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)     2052 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_form.html
+-rw-rw-rw-   0 root         (0) root         (0)      275 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_closed.html
+-rw-rw-rw-   0 root         (0) root         (0)      266 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_complete.html
+-rw-rw-rw-   0 root         (0) root         (0)      380 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_failed.html
+-rw-rw-rw-   0 root         (0) root         (0)      567 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_urls.py
+-rw-rw-rw-   0 root         (0) root         (0)       50 2022-07-20 09:38:44.000000 djangoldp_branding-1.0.8/djangoldp_branding/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15362 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    15233 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     7176 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0 root         (0) root         (0)    14897 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.po
+-rw-rw-rw-   0 root         (0) root         (0)     6840 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.mo
+-rw-rw-rw-   0 root         (0) root         (0)      110 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/
+-rw-rw-rw-   0 root         (0) root         (0)    19356 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/admin.css
+-rw-rw-rw-   0 root         (0) root         (0)      432 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/css/main.css
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/images/
+-rw-rw-rw-   0 root         (0) root         (0)      832 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/static/images/favicon.webp
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-07-20 09:38:46.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1177 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/templatetags/orbit.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2022-07-20 09:38:26.000000 djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_settings.py
```

### Comparing `djangoldp_branding-1.0.7/README.md` & `djangoldp_branding-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/setup.cfg` & `djangoldp_branding-1.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding.egg-info/SOURCES.txt` & `djangoldp_branding-1.0.8/djangoldp_branding.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/views.py` & `djangoldp_branding-1.0.8/djangoldp_branding/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/processor.py` & `djangoldp_branding-1.0.8/djangoldp_branding/processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,11 +17,12 @@
     except:
         logger.info('Error while loading config.json from the root of your server')
 
 ORBIT_JSON['debug_flag'] = settings.DEBUG
 ORBIT_JSON['default_client'] = settings.INSTANCE_DEFAULT_CLIENT
 ORBIT_JSON['base_url'] = settings.BASE_URL
 ORBIT_JSON['site_url'] = settings.SITE_URL
+ORBIT_JSON['client_settings'] = ORBIT_JSON['client']
 
 
 def branding_context(request):
     return ORBIT_JSON
```

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/accessrequests/access_requested.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_requested.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/accessrequests/access_resolved.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/accessrequests/access_resolved.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/base_email.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/base_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_change_form.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_email.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_confirm.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_confirm.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/activation_complete.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_form.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/password_reset_complete.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/password_reset_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/registration_closed.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/registration_closed.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/registration/login.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/email.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/joboffer/email.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/joboffer/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/admin/base.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/admin/login.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/oidc_provider/authorize.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/oidc_provider/authorize.html`

 * *Files 7% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 
 {% block title %}
   {% trans "Demande d'accès aux informations" %}
 {% endblock %}
 
 {% block content %}
 <div class="segment full whitespace-normal form">
-  <div class="instance-logo">
-    <img src="{% orbit 'client.logo' %}" style="max-width: 100%; max-height: 100%" />
-  </div>
   <form class="segment half sm-full whitespace-normal" method="post" action="{% url 'oidc_provider:authorize' %}">
     <h2 class="text-semibold text-left text-color-secondary">{% trans "Demande d'autorisation" %}</h2>
     {% csrf_token %}
     {{ hidden_inputs }}
     <div class="segment full text-left">
       {% if scopes|length > 0 %}
       <p class="text-semibold text-color-heading">{% trans "L'application" %} <strong>{{ client.name }}</strong> {% trans "demande à accéder à ces informations te concernant :" %}</p>
```

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/password/email.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/password/email.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/base.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/base.html`

 * *Files 5% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 {% load orbit %}
 {% load static %}
 {% get_current_language as LANGUAGE_CODE %}{% get_current_language_bidi as LANGUAGE_BIDI %}
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
   <head>
     <meta charset="UTF-8" />
-    <title>{% orbit 'client.name' %} - {% block title %}{{ title }}{% endblock %}</title>
+    <title>{% orbit 'client_settings.name' %} - {% block title %}{{ title }}{% endblock %}</title>
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <meta http-equiv="X-UA-Compatible" content="ie=edge" />
     <link rel="preconnect" href="https://fonts.gstatic.com" />
     <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&amp;display=swap" />
     <link rel="stylesheet" href="https://unpkg.com/@startinblox/orbit-styling-framework" />
     <link rel="stylesheet" href="{% static 'css/main.css' %}{% if debug_flag %}?{% now 'U' %}{% endif %}" />
     {% block extrastyle %}{% endblock %}
-    {% if "css" in client %}
+    {% if "css" in client_settings %}
     <link rel="stylesheet" href="{% orbit 'client.css' %}" />
     {% endif %}
-    {% if "favicon" in client %}
+    {% if "favicon" in client_settings %}
     <link rel="icon" type="image/webp" href="{% orbit 'client.favicon' %}">
     {% else %}
     <link rel="icon" type="image/webp" href="{% static 'images/favicon.webp' %}">
     {% endif %}
     {% block extrahead %}{% endblock %}
   </head>
 
   <body>
     <div class="segment full whitespace-normal">
       <div class="whitespace-normal padding-top-xxlarge padding-right-xsmall padding-bottom-xlarge padding-left-xsmall sm-padding-top-medium bg-color-secondary text-center content-index">
         <div class="segment two-third sm-full bg-color-white shadow border-rounded-xxsmall whitespace-normal">
-          {% if "logo" in client %}
+          {% if "logo" in client_settings %}
             <div class="instance-logo">
               <img src="{% orbit 'client.logo' %}" style="max-width: 100%; max-height: 100%" />
             </div>
           {% endif %}
           {% if debug_flag %}{% orbit "errors" %}{% endif %}
           <div class="segment full sm-full whitespace-normal">
             {% block content %}{% autoescape off %}{{ content }}{% endautoescape %}{% endblock %}
```

#### html2text {}

```diff
@@ -3,16 +3,16 @@
 
  }}"{% if LANGUAGE_BIDI %} dir="rtl"{% endif %}>
 
 
 
 
 
- {% block extrastyle %}{% endblock %} {% if "css" in client %}
- {% endif %} {% if "favicon" in client %}
+ {% block extrastyle %}{% endblock %} {% if "css" in client_settings %}
+ {% endif %} {% if "favicon" in client_settings %}
  {% else %}
  {% endif %} {% block extrahead %}{% endblock %}
-{% if "logo" in client %}
+{% if "logo" in client_settings %}
 [{% orbit 'client.logo' %}]
 {% endif %} {% if debug_flag %}{% orbit "errors" %}{% endif %}
 {% block content %}{% autoescape off %}{{ content }}{% endautoescape %}{%
 endblock %}
```

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/activation_complete.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/activation_complete.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templates/django_registration/registration_form.html` & `djangoldp_branding-1.0.8/djangoldp_branding/templates/django_registration/registration_form.html`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/djangoldp_urls.py` & `djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_urls.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/es/LC_MESSAGES/django.po` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/es/LC_MESSAGES/django.mo` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/LC_MESSAGES/django.po` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/en/LC_MESSAGES/django.po` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/locale/en/LC_MESSAGES/django.mo` & `djangoldp_branding-1.0.8/djangoldp_branding/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/static/css/admin.css` & `djangoldp_branding-1.0.8/djangoldp_branding/static/css/admin.css`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/static/images/favicon.webp` & `djangoldp_branding-1.0.8/djangoldp_branding/static/images/favicon.webp`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/templatetags/orbit.py` & `djangoldp_branding-1.0.8/djangoldp_branding/templatetags/orbit.py`

 * *Files identical despite different names*

### Comparing `djangoldp_branding-1.0.7/djangoldp_branding/djangoldp_settings.py` & `djangoldp_branding-1.0.8/djangoldp_branding/djangoldp_settings.py`

 * *Files identical despite different names*

